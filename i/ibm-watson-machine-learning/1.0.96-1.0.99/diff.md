# Comparing `tmp/ibm_watson_machine_learning-1.0.96.tar.gz` & `tmp/ibm_watson_machine_learning-1.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ibm_watson_machine_learning-1.0.96.tar", last modified: Fri May 28 11:31:02 2021, max compression
+gzip compressed data, was "dist/ibm_watson_machine_learning-1.0.99.tar", last modified: Wed Jun  9 14:15:08 2021, max compression
```

## Comparing `ibm_watson_machine_learning-1.0.96.tar` & `ibm_watson_machine_learning-1.0.99.tar`

### file list

```diff
@@ -1,756 +1,773 @@
-drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:02.000000 ibm_watson_machine_learning-1.0.96/
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)       16 2021-05-28 11:31:01.000000 ibm_watson_machine_learning-1.0.96/MANIFEST.in
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1904 2021-05-28 11:31:02.000000 ibm_watson_machine_learning-1.0.96/PKG-INFO
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      578 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/README.md
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)        7 2021-05-28 11:31:01.000000 ibm_watson_machine_learning-1.0.96/VERSION
-drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     7762 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/Set.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1343 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/__init__.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    31865 2021-05-28 11:30:28.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/assets.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    26409 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/client.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    22610 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/connections.py
-drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/deployment/
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      641 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/deployment/__init__.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    29456 2021-05-28 11:30:28.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/deployment/base_deployment.py
--rwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)    23278 2021-05-28 11:30:28.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/deployment/batch.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    10718 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/deployment/web_service.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    72352 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/deployments.py
-drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/experiment/
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      652 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/experiment/__init__.py
-drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/experiment/autoai/
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      580 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/experiment/autoai/__init__.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    19789 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/experiment/autoai/autoai.py
-drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/experiment/autoai/engines/
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      667 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/experiment/autoai/engines/__init__.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     2132 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/experiment/autoai/engines/base_engine.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    43737 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/experiment/autoai/engines/wml_engine.py
-drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/experiment/autoai/optimizers/
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      800 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/experiment/autoai/optimizers/__init__.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1878 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/experiment/autoai/optimizers/base_auto_pipelines.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    29767 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/experiment/autoai/optimizers/local_auto_pipelines.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    33005 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/experiment/autoai/optimizers/remote_auto_pipelines.py
-drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/experiment/autoai/runs/
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      793 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/experiment/autoai/runs/__init__.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    17348 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/experiment/autoai/runs/auto_pipelines_runs.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1736 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/experiment/autoai/runs/base_auto_pipelines_runs.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     9372 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/experiment/autoai/runs/local_auto_pipelines_runs.py
-drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/experiment/base_experiment/
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      678 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/experiment/base_experiment/__init__.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1019 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/experiment/base_experiment/base_experiment.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    23403 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/experiments.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    20611 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/export_assets.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    53372 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/functions.py
-drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/helpers/
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      921 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/helpers/__init__.py
-drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/helpers/connections/
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      930 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/helpers/connections/__init__.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      869 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/helpers/connections/base_connection.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    24195 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/helpers/connections/base_data_connection.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      919 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/helpers/connections/base_location.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    46604 2021-05-28 11:30:28.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/helpers/connections/connections.py
-drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/helpers/flight/
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/helpers/flight/__init__.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3482 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/helpers/flight/errors.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    15110 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/helpers/flight/service.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    11864 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/helpers/flight/utils.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3357 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/helpers/helpers.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5478 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/hpo.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    22441 2021-05-28 11:30:28.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/href_definitions.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    17343 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/hw_spec.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    15346 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/import_assets.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    10639 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/instance.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    15835 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/instance_new_plan.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    20082 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/learning_system.py
-drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      579 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/__init__.py
-drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/mlpipelinepy/
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      902 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/mlpipelinepy/__init__.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1949 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/mlpipelinepy/edge.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1002 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/mlpipelinepy/exception.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5877 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/mlpipelinepy/javaproxy.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    10776 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/mlpipelinepy/mlpipeline.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1289 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/mlpipelinepy/serialization.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1670 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/mlpipelinepy/utils.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      955 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/mlpipelinepy/version.py
-drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/pipeline/
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    12138 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/pipeline/DAG.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    14274 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/pipeline/IBMSparkPipeline.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6317 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/pipeline/IBMSparkPipelineModel.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3090 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/pipeline/Result.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     2493 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/pipeline/Sink.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     2527 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/pipeline/Source.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    11223 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/pipeline/Wrapper.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      804 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/pipeline/__init__.py
-drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6070 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/TestRepoSaveLoad.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      830 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/__init__.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1433 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/base_constants.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3462 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/ml_api_client.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     7251 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/ml_authorization.py
-drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepository/
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1711 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepository/__init__.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4318 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepository/artifact.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      931 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepository/artifact_reader.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1149 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepository/generic_archive_model_artifact.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1179 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepository/generic_archive_pipeline_artifact.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1117 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepository/hybrid_model_artifact.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    11184 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepository/meta_names.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1546 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepository/meta_props.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1433 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepository/model_artifact.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1044 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepository/pipeline_artifact.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1283 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepository/scikit_model_artifact.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1134 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepository/tensorflow_model_artifact.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1067 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepository/wml_experiment_artifact.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1049 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepository/wml_function_artifact.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1062 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepository/wml_libraries_artifact.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1061 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepository/wml_runtimes_artifact.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1120 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepository/xgboost_model_artifact.py
-drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     2782 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/__init__.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6718 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/content_loaders.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1966 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/experiment_artifact.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1990 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/function_artifact.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1558 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/function_artifact_loader.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1177 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/function_artifact_reader.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1175 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/function_loader.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6579 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/generic_archive_pipeline_model_artifact.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1694 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/generic_file_artifact_loader.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1286 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/generic_file_pipeline_model_loader.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1514 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/generic_file_reader.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4512 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/hybrid_artifact_loader.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     2302 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/hybrid_pipeline_model_artifact.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1231 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/hybrid_pipeline_model_loader.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     2384 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/hybrid_pipeline_model_reader.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3696 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/libraries_artifact.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1994 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/libraries_artifact_loader.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1169 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/libraries_artifact_reader.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      976 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/libraries_loader.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    19703 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/ml_repository_artifact.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      754 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/python_version.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     2913 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/runtimes_artifact.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     2037 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/runtimes_artifact_loader.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1174 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/runtimes_artifact_reader.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     2601 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/scikit_artifact_loader.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    14968 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/scikit_pipeline_model_artifact.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1496 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/scikit_pipeline_model_loader.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3245 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/scikit_pipeline_reader.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     2027 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/spark_artifact_loader.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     2939 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/spark_pipeline_artifact.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      905 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/spark_pipeline_loader.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    10858 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/spark_pipeline_model_artifact.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      936 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/spark_pipeline_model_loader.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     2561 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/spark_pipeline_reader.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1203 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/spark_version.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     2097 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/tensorflow_artifact_loader.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    10261 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/tensorflow_pipeline_model_artifact.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     2400 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/tensorflow_pipeline_model_loader.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4136 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/tensorflow_pipeline_reader.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6465 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/version_helper.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3071 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/xgboost_model_reader.py
-drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1627 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/__init__.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     2805 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/content_reader.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6830 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/experiment_adapter.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    18004 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/experiment_collection.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6335 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/function_adapter.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    15143 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/function_collection.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3099 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/libraries_adapter.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     9960 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/libraries_collection.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    11683 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/ml_repository_api.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5094 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/ml_repository_client.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    15089 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/model_adapter.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    60931 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/model_collection.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     2933 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/runtimes_adapter.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    10138 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/runtimes_collection.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3003 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/wml_experiment_adapter.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    22480 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/wml_experiment_collection.py
-drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    12612 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/__init__.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    23112 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/api_client.py
-drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/apis/
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      725 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/apis/__init__.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)   259498 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/apis/repository_api.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    12406 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/apis/token_api.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     9707 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/configuration.py
-drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    13430 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/__init__.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3364 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/array_data_input_repository.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5459 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/array_model_metrics_output.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5414 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/array_model_output.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3489 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/array_model_version_metrics_experiments.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5477 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/array_model_version_output.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5441 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/array_pipeline_output.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5504 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/array_pipeline_version_output.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4201 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/array_training_output_experiments.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5360 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/artifact_author.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6561 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/artifact_version_metadata.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5066 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/artifact_version_repository.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5921 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/artifact_version_short_metadata.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3949 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/author_experiments.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3838 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/author_repository.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5960 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/batch_deploy_output.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5500 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/batch_deploy_output_entity.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     8254 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/batch_deploy_output_entity_execution.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5850 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/batch_deploy_output_meta.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     7401 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/batch_input.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5912 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/batch_output.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5413 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/batch_output_array.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4777 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/cols_output.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4630 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/compute_configuration_experiments.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4777 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/connection.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5405 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/connection_object_source_experiments.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5405 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/connection_object_target_experiments.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5609 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/connection_object_with_name_repository.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6676 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/content_location.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4262 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/content_status.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4753 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/custom_models.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6274 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/deploy_input.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4496 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/error_bad_request_libraries_target.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5737 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/error_experiments.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4522 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/error_experiments_target.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     7035 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/error_message.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5544 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/error_repository.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4384 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/error_repository_target.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4633 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/error_schema_experiments.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4486 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/error_schema_repository.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6109 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/evaluation_definition.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5048 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/evaluation_definition_experiments.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6151 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/evaluation_definition_metrics.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5047 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/evaluation_definition_repository.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5740 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/evaluation_definition_repository_metrics.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     7751 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/experiment_input.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6911 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/experiment_input_settings.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4706 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/experiment_output.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5917 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/experiment_output_array.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3985 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/experiment_output_array_first.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3449 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/experiment_patch.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     9291 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/experiment_status_experiments.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6711 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/framework_output_repository.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4580 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/framework_output_repository_libraries.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4568 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/framework_output_repository_runtimes.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     7180 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/hyper_parameters.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     7821 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/hyper_parameters_experiments.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6100 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/hyper_parameters_experiments_double_range.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6100 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/hyper_parameters_experiments_inner_double_range.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6028 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/hyper_parameters_experiments_inner_int_range.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5344 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/hyper_parameters_experiments_inner_values_range.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6028 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/hyper_parameters_experiments_int_range.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3489 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/hyper_parameters_for_status_experiments.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4890 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/hyper_parameters_for_status_experiments_inner.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5132 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/hyper_parameters_optimization_experiments.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5288 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/hyper_parameters_optimization_experiments_method.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6480 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/hyper_parameters_optimization_experiments_method_parameters.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4788 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/input_data_schema.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6109 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/internal_input_batch.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6112 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/internal_output_batch.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4785 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/json_patch_array.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6533 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/json_patch_entity.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6444 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/libraries_definition_input.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4598 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/libraries_definition_input_platform.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5362 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/meta_object.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4123 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/meta_object_experiments.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5980 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/meta_object_experiments_metadata.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5768 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/meta_object_functions_metadata.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     9800 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/meta_object_metadata.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4009 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/meta_object_repository.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     8681 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/meta_object_repository_metadata.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4600 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/metric_object_experiments.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4755 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/metrics_models.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     7514 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_experiment_input.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4688 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_experiment_output.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4141 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_experiment_output_array.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     9094 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_function_input.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4641 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_functions_output.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6160 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_functions_output_array.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3958 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_functions_output_array_first.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4678 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_libraries_output.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6160 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_libraries_output_array.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3958 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_libraries_output_array_first.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    20734 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_model_input.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4638 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_model_output.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4075 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_model_output_array.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4728 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_patch_libraries_output.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4700 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_runtime_spec_output.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6214 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_runtime_spec_output_array.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3970 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_runtime_spec_output_array_first.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     2493 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_get_presigned_url_output.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     2504 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_model_size_output.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4561 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_patch_function.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3370 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_patch_libraries_input.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3374 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_patch_runtime_spec_input.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4682 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_patch_runtime_spec_output.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4697 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_upload_content_output.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4089 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_upload_content_output_entity.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5912 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_upload_content_output_metadata.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     7827 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/model_content_location.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3917 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/model_definition_models.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    13915 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/model_input.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6063 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/model_metrics.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5955 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/model_metrics_values.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5946 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/model_output.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    15820 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/model_output_entity.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6269 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/model_output_entity_pipeline_version.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6194 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/model_schemas.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6271 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/model_training_data_ref.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4776 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/model_type.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6389 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/model_version_input.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4738 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/model_version_metrics_experiments.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6037 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/model_version_output.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    11117 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/model_version_output_entity.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6027 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/model_version_output_entity_model.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5983 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/online_deploy_output.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5923 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/online_output.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5461 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/online_output_array.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4761 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/output_data_schema.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5998 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/patch_operation_experiments.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5844 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/patch_operation_functions.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5844 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/patch_operation_libraries.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5880 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/patch_operation_runtime_spec.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     8144 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/pipeline_input.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4417 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/pipeline_models.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5985 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/pipeline_output.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    10863 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/pipeline_output_entity.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4782 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/pipeline_type.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5724 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/pipeline_version_input.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6076 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/pipeline_version_output.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6356 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/pipeline_version_output_entity.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6115 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/pipeline_version_output_entity_parent.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4793 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/runtime_environment.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3925 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/runtime_models.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4480 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/runtime_output_repository.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     7166 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/runtime_spec_definition_input.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4072 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/runtime_spec_definition_input_custom_libraries.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4590 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/runtime_spec_definition_input_platform.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5485 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/runtime_spec_definition_input_public_libraries.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3940 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/runtime_spec_definition_input_repository.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4781 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/sample_scoring_input.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     7590 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/schemas.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5408 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/score_input.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5308 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/score_output.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6258 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/size_models.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3908 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/software_spec_models.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4395 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/space_models.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6135 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/spark_service.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6250 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/stream_input_internal.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     7487 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/stream_internal.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5922 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/stream_output.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5422 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/stream_output_array.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6320 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/stream_output_internal.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4576 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/tag_repository.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5331 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/token_response.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4782 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/training_data_schema.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3931 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/training_models.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4747 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/training_output_experiments.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     8939 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/training_reference_experiments.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    14844 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/training_status_experiments.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4213 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/training_status_experiments_result.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    13111 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/rest.py
-drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/util/
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      776 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/util/__init__.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      969 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/util/base_singleton.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1422 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/util/compression_util.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      793 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/util/exceptions.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      899 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/util/file_system_ops.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1243 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/util/generic_archive_file_check.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1515 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/util/json_2_object_mapper.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4252 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/util/library_imports.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     2779 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/util/spark_util.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      771 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/util/unique_id_gen.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    69996 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/metanames.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    15892 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/migration_v4ga_cloud.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    52929 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/model_definition.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)   151533 2021-05-28 11:30:28.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/models.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    31304 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/pipelines.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    23457 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/pkg_extn.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    32299 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/platform_spaces.py
-drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/preprocessing/
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      761 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/preprocessing/__init__.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    30660 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/preprocessing/data_join_pipeline.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    18341 2021-02-15 10:28:26.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/preprocessing/multiple_files_preprocessor.py
-drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/preprocessing/templates/
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      579 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/preprocessing/templates/__init__.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1498 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/preprocessing/templates/pretty_print_template.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    17709 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/remote_training_system.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    96144 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/repository.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    50300 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/runtimes.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    53325 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/script.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    45756 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/shiny.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    33243 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/spaces.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    26470 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/sw_spec.py
-drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/
-drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    12423 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/Connections_SPSS_BIGQUERY_MYSQL_spaces_cp4d_35.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    12000 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/Connections_SPSS_MSSQL_spaces_cp4d_35.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    12545 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/Connections_SPSS_TERADATA_MYSQL_spaces_cp4d_35.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     2406 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/DataAssets_spaces_cp4d_35.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    14215 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/Experiment_Pipeline_spaces_cp4d_35.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    12257 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/ExportImport_spaces_cp4d_35.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    14233 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/Functions_spaces_cp4d_35.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      978 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/HardwareSpec_spaces_cp4d_35.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    13061 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/ModeDoFromFile_spaces_cp4d_35.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4614 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/ModelDefinition_projects_dev_cp4d_35.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5727 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/ModelDefinition_spaces_cp4d_35.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4655 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/ModelPMML_spaces_cp4d_35.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    18665 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/Model_Hybrid_from_zipfile_spaces_cp4d_35.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4043 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/Model_keras_spaces_cp4d_35.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3834 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/Model_pmml_spaces_cp4d_35.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    11402 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/Model_scikit_learn_from_object_sw_spaces_cp4d_35.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5867 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/Model_spark_mllib_from_object_spaces_cp4d_35.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6922 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/Model_spss_from_file_spaces_cp4d_35.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3832 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/Model_tensorflow_spaces_cp4d_35.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6532 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/PkgExt_spaces_cp4d_35.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     9489 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/RScripts_spaces_cp4d_35.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3827 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/RShiny_projects_dev_cp4d_35.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     7133 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/RShiny_spaces_cp4d_35.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3810 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/Remote_training_systems_spaces_cp4d_35.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3995 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/Scripts_projects_dev_cp4d_35.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     9446 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/Scripts_spaces_cp4d_35.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3921 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/SoftwareSpec_projects_dev_cp4d_35.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4852 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/SoftwareSpec_spaces_cp4d_35.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/__init__.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5531 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/models_preparation.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    13538 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/preparation_and_cleaning.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     9578 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/spaces_cp4d_35.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    11346 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/test_CP4D_3_connections.py
-drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/Cloud/
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     2916 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/Cloud/DataAssets_spaces_cloud.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    14725 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/Cloud/Experiment_Pipeline_spaces_cloud.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    12736 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/Cloud/ExportImport_spaces_cloud.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    14404 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/Cloud/Functions_spaces_cloud.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      976 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/Cloud/HardwareSpec_spaces_cloud.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    13692 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/Cloud/ModeDoFromFile_spaces_cloud.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4612 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/Cloud/ModelDefinition_projects_dev_cloud.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6138 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/Cloud/ModelDefinition_spaces_cloud.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5191 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/Cloud/ModelPMML_spaces_cloud.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    19221 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/Cloud/Model_Hybrid_from_zipfile_spaces_cloud.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4747 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/Cloud/Model_keras_spaces_cloud.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4379 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/Cloud/Model_pmml_spaces_cloud.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    11938 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/Cloud/Model_scikit_learn_from_object_sw_spaces_cloud.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6297 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/Cloud/Model_spark_mllib_from_object_spaces_cloud.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     7447 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/Cloud/Model_spss_from_file_spaces_cloud.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4720 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/Cloud/Model_tensorflow_spaces_cloud.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6535 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/Cloud/PkgExt_spaces_cloud.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3825 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/Cloud/RShiny_projects_dev_cloud.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     7629 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/Cloud/RShiny_spaces_cloud.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4318 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/Cloud/Remote_training_systems_spaces_cloud.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3993 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/Cloud/Scripts_projects_dev_cloud.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    10025 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/Cloud/Scripts_spaces_cloud.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3919 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/Cloud/SoftwareSpec_projects_dev_cloud.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5245 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/Cloud/SoftwareSpec_spaces_cloud.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/Cloud/__init__.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5521 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/Cloud/models_preparation.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    13494 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/Cloud/preparation_and_cleaning.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    11254 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/Cloud/spaces_cloud.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1938 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/ConfigFileEncoder.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1530 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/ConfigFileGenerator.py
-drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/ICP/
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5172 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/ICP/CP4D_mllib_from_object.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/ICP/__init__.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5524 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/ICP/models_preparation.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    13270 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/ICP/preparation_and_cleaning.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     7058 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/ICP/test-CP4D_3_hybrid_autoai_model.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     8854 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/ICP/test_CP4D_3_connections.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     8434 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/ICP/test_CP4D_3_cross_deployment_model_function.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     8486 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/ICP/test_CP4D_3_cross_deployment_model_model.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    11913 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/ICP/test_CP4D_3_do_from_file.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6139 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/ICP/test_CP4D_3_functions_sw.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     9843 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/ICP/test_CP4D_3_import_export_spaces.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5289 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/ICP/test_CP4D_3_mllib_2_4_from_object_sw.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5189 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/ICP/test_CP4D_3_pkg_extn.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     7348 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/ICP/test_CP4D_3_rshiny.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     9751 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/ICP/test_CP4D_3_scikit_learn_from_object_sw.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     8641 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/ICP/test_CP4D_3_scripts.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3058 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/ICP/test_CP4D_3_software_spec.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6343 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/ICP/test_CP4D_3_spss_from_file.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6087 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/ICP/test_CP4D_functions.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5156 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/ICP/test_CP4D_runtimes.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     8029 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/ICP/test_CP4D_scikit_learn_from_object.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4836 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/ICP/test_CP4D_spaces.py
-drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/WSD/
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3907 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/WSD/WSD_functions.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     2431 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/WSD/WSD_mllib_from_object.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3245 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/WSD/WSD_scikit_learn_from_object.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/WSD/__init__.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5521 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/WSD/models_preparation.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    13270 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/WSD/preparation_and_cleaning.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/__init__.py
-drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/__init__.py
-drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/fvt/
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/fvt/__init__.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     8141 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/fvt/local_optimizer_for_CP4D35.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3839 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/fvt/test__lale__breast_cancer.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     9482 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/fvt/test_any_autoai_experiment__lale__.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     9992 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/fvt/test_breast_cancer_binary_lgbm.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     9996 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/fvt/test_breast_cancer_binary_sklearn.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     9987 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/fvt/test_breast_cancer_binary_xgboost.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4438 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/fvt/test_credit_risk_binary_local_ai4ml.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    16696 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/fvt/test_custom_separator_binary_multiclass_regression.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     9981 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/fvt/test_insurance_regression_lgbm.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     9896 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/fvt/test_insurance_regression_sklearn.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     9980 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/fvt/test_insurance_regression_xgboost.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    21581 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/fvt/test_iris_wml_autoai_multiclass_CP4D_3_5.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    15154 2021-04-21 14:01:07.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/fvt/test_local_optimizer_with_cos.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    38103 2021-04-21 14:01:07.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/fvt/test_obm_plus_kb_go_sales_multiclass.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     9805 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/fvt/test_student_multiclass_lgbm.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     9808 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/fvt/test_student_multiclass_sklearn.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     9804 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/fvt/test_student_multiclass_xgboost.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    19355 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/fvt/test_xlsx_read_binary_regression.py
-drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/manual/
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/manual/__init__.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    17335 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/manual/test_bank_binary.py
-drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/__init__.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3284 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/abstract_test_iris_using_database_connection.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3468 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/abstract_test_iris_using_database_data_asset.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    19330 2021-05-28 11:30:28.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/abstract_test_iris_wml_autoai_multiclass_connections.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    22067 2021-05-28 11:30:28.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_bank_wml_autoai_xlsx_binary.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    21285 2021-05-28 11:30:28.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_breast_cancer_wml_autoai_csv_binary.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    21930 2021-05-28 11:30:28.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_breast_cancer_wml_autoai_csv_binary_apikey_auth.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    21759 2021-05-28 11:30:28.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_breast_cancer_wml_autoai_csv_binary_token_auth.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    25024 2021-05-28 11:30:28.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_car_price_wml_autoai_regression.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    15410 2021-05-28 11:30:28.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_credit_risk_as_sample_notebook_binary.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    11682 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_drop_duplicates.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    14562 2021-05-28 11:30:28.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_insurance_wml_autoai_xlsx_regression.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4818 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_iris_using_data_asset_and_connected_asset.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4031 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_iris_using_data_asset_and_default.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3778 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_iris_using_data_connected_asset_and_connected_asset.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3534 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_iris_using_data_connected_asset_and_default.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4082 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_iris_using_data_connected_asset_and_s3.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4162 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_iris_using_data_s3_and_connected_asset.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3223 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_iris_using_data_s3_and_s3.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1162 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_iris_using_database_connection.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1402 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_iris_using_database_data_asset.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3251 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_iris_using_filesystem_and_connected_asset.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1512 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_iris_using_filesystem_and_default.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    23737 2021-05-28 11:30:28.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_iris_wml_autoai_multiclass.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    24647 2021-05-28 11:30:28.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_iris_wml_autoai_multiclass_connections.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    22279 2021-05-28 11:30:28.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_iris_wml_autoai_multiclass_space_only.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    22926 2021-05-28 11:30:28.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_iris_wml_autoai_multiclass_using_NFS.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    21160 2021-05-28 11:30:28.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_iris_wml_autoai_multiclass_using_data_asset.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    24499 2021-05-28 11:30:28.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_obm_group_customer.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    43413 2021-05-28 11:30:28.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_obm_plus_kb_group_customer_regression.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    44448 2021-05-28 11:30:28.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_obm_plus_kb_group_customer_regression_csv_only.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    42099 2021-05-28 11:30:28.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_obm_plus_kb_temp_binary.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    19778 2021-05-28 11:30:28.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_text_transformer_csv_multiclass.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    20033 2021-05-28 11:30:28.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_text_transformer_csv_regression.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    20364 2021-05-28 11:30:28.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_text_transformer_donorchoose_binary.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    21587 2021-05-28 11:30:28.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_text_transformer_fake_job_position_binary.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    20103 2021-05-28 11:30:28.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_twitter_wml_autoai_csv_forecasting.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    20104 2021-05-28 11:30:28.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_twitter_wml_autoai_csv_forecasting_multivariate.py
-drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/unit/
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/unit/__init__.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6294 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/unit/test_auto_pipeline_runs.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1560 2021-02-15 07:14:10.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/unit/test_check_dependencies_versions.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     8031 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/unit/test_data_connection.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     9446 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/unit/test_data_join_pipeline_graph.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4518 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/unit/test_get_obm_output.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4099 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/unit/test_local_auto_pipeline.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1504 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/unit/test_next_run_details_generator.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      804 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/unit/test_piepeline_to_script.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     2538 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/unit/test_prepare_auto_ai_model_to_publish.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4156 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/unit/test_prepare_cos_client.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4910 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/unit/test_tshirt_sizes_limitation.py
-drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/contract_tests/
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/contract_tests/__init__.py
-drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/deployment/
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/deployment/__init__.py
-drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/deployment/unit/
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/deployment/unit/__init__.py
--rwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)     7748 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/deployment/unit/test_batch.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5497 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/deployment/unit/test_web_service.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3132 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/install_requirements.py
-drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6017 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4functions.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5281 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4pipelines.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6830 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_ai_functions_from_func.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)   452070 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_ai_functions_from_func_sklearn_preprocessing.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3425 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_ai_functions_from_gz.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5679 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_ai_functions_from_gz_keras.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5100 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_ai_functions_from_gz_mandatory_params.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    11502 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_do_from_tar_gz.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    11829 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_experiment_and_pipelines.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6488 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_keras_from_file_V4.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     8922 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_keras_from_object_V4_disable.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     7521 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_keras_from_tgz.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5074 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_libraries_experiments.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6086 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_pmml_from_xml.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6463 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_pytorch_from_tar_gz.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3698 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_runtimes_custom_libs.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4142 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_runtimes_custom_libs_attaching_to_model_from_archive.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4379 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_runtimes_custom_libs_attaching_to_model_from_object.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3378 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_runtimes_custom_libs_delete_orphaned_libs.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3591 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_runtimes_custom_libs_yaml_upload.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1899 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_runtimes_mandatory_params.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     8452 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_scikit_learn_from_directory.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     7621 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_scikit_learn_from_object.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6152 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_scikit_learn_from_tar_gz.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5980 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_scikit_xgboost_from_directory.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5951 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_scikit_xgboost_from_object.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6265 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_scikit_xgboost_from_tar_gz.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4486 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_spaces.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5900 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_spark_mllib_from_object.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     8134 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_spark_mllib_from_tar_gz.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6554 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_spss_from_file.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5451 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_tensorflow_from_directory.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6526 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_tensorflow_from_file.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     8852 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_tensorflow_training.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     9421 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_training_from_pipeline.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6170 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_xgboost_from_directory.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     7180 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_xgboost_from_json.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6513 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_xgboost_from_object.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6059 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_xgboost_from_tar_gz.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/__init__.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     8800 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/_test_scikit_learn_grid_search_xgboost_panda_table_disable.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4590 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/_test_spark_mllib_from_directory_disable.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4601 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/cloud_mllib_from_object.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     7478 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/models_preparation.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    13270 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/preparation_and_cleaning.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4896 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/runtimesV4.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    12622 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_ai_functions_from_func_hitting_scoring_disable.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5287 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_ai_functions_from_gz_disable.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6165 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_ai_functions_from_wrapper_func_disable.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    16318 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_caffe_experiment_disable.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1977 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_clean_disable.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5420 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_coreml_from_caffe_200Mb_model_disable.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     7591 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_coreml_from_caffe_disable.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    13128 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_coreml_from_keras_disable.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4959 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_coreml_from_scikit_disable.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5106 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_coreml_from_xgboost_disable.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    16555 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_keras_experiment_disable.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    15154 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_keras_experiment_hpo_disable.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    11579 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_keras_experiment_learning_system_disable.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    21123 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_keras_experiment_monitor_metrics_disable.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3536 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_keras_from_file.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3178 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_load_30Mb_model_disable.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    20986 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_pytorch_experiment_disable.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    11727 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_repository_limit_disable.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4252 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_runtimes_custom_libs_attaching_to_simple_model_v4.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     7789 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_scikit_learn_from_object_refresh_token_disable.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     8439 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_scikit_learn_grid_search_xgboost_numpy_table_disable.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    10939 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_spark_mllib_with_learning_system_disable.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    12041 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_tensorflow_distributed_ddl_experiment_disable.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    14722 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_tensorflow_distributed_horovod_training_disable.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    15543 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_tensorflow_distributed_training_disable.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    14266 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_tensorflow_experiment_disable.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    15600 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_tensorflow_experiment_hpo_disable.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    14255 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_tensorflow_experiment_hpo_light_disable.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    12227 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_tensorflow_experiment_mandatory_params_only_disable.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    15084 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_tensorflow_experiment_monitor_metrics_disable.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    15717 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_tensorflow_experiment_sync_disable.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    13457 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_tensorflow_training_mandatory_params_only_disable.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    14671 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_tensorflow_training_v4_disable.py
-drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/utils/
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)       20 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/utils/__init__.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      254 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/utils/assertions.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     2368 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/utils/cleanup.py
-drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/utils/openshift/
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/utils/openshift/__init__.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      717 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/utils/openshift/cli.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     2188 2021-02-12 13:14:06.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/utils/openshift/prometheusapi.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    15370 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/utils/utils.py
-drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/workspace/
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-02-12 13:14:06.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/workspace/__init__.py
-drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/workspace/unit/
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-02-12 13:14:06.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/workspace/unit/__init__.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1304 2021-02-12 13:14:06.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/workspace/unit/test_workspace.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    50100 2021-05-28 11:30:28.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/training.py
-drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/utils/
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      634 2021-02-12 13:14:06.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/utils/__init__.py
-drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/utils/autoai/
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      579 2021-02-12 13:14:06.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/utils/autoai/__init__.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     7152 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/utils/autoai/connection.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6792 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/utils/autoai/enums.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    12866 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/utils/autoai/errors.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3458 2021-02-12 13:14:06.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/utils/autoai/local_training_message_handler.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     2461 2021-02-12 13:14:06.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/utils/autoai/progress_bar.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1524 2021-02-12 13:14:06.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/utils/autoai/training.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    64423 2021-05-28 11:30:28.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/utils/autoai/utils.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3104 2021-02-12 13:14:06.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/utils/autoai/watson_studio.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    23344 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/utils/autoai/wsd_ui.py
-drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/utils/deployment/
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      579 2021-02-12 13:14:06.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/utils/deployment/__init__.py
--rwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3126 2021-05-28 11:30:28.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/utils/deployment/errors.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    16263 2021-02-12 13:14:06.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/utils/utils.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    22363 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/volumes.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4684 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/wml_client_error.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    35991 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/wml_resource.py
-drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/workspace/
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      650 2021-02-12 13:14:06.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/workspace/__init__.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     7893 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/workspace/workspace.py
-drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:02.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning.egg-info/
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1904 2021-05-28 11:31:01.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning.egg-info/PKG-INFO
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    49738 2021-05-28 11:31:01.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning.egg-info/SOURCES.txt
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)        1 2021-05-28 11:31:01.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning.egg-info/dependency_links.txt
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)       92 2021-05-28 11:31:01.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning.egg-info/requires.txt
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)       34 2021-05-28 11:31:01.000000 ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning.egg-info/top_level.txt
-drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:02.000000 ibm_watson_machine_learning-1.0.96/ibmfl/
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:00.000000 ibm_watson_machine_learning-1.0.96/ibmfl/__init__.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)       22 2021-05-28 11:31:00.000000 ibm_watson_machine_learning-1.0.96/ibmfl/_version.py
-drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:02.000000 ibm_watson_machine_learning-1.0.96/ibmfl/connection/
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:00.000000 ibm_watson_machine_learning-1.0.96/ibmfl/connection/__init__.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     2945 2021-05-28 11:31:00.000000 ibm_watson_machine_learning-1.0.96/ibmfl/connection/connection.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3250 2021-05-28 11:31:00.000000 ibm_watson_machine_learning-1.0.96/ibmfl/connection/route_declarations.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     2400 2021-05-28 11:31:00.000000 ibm_watson_machine_learning-1.0.96/ibmfl/connection/router_handler.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    17900 2021-05-28 11:31:00.000000 ibm_watson_machine_learning-1.0.96/ibmfl/connection/websockets_connection.py
-drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:02.000000 ibm_watson_machine_learning-1.0.96/ibmfl/data/
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:00.000000 ibm_watson_machine_learning-1.0.96/ibmfl/data/__init__.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     7979 2021-05-28 11:31:00.000000 ibm_watson_machine_learning-1.0.96/ibmfl/data/data_handler.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    14780 2021-05-28 11:31:00.000000 ibm_watson_machine_learning-1.0.96/ibmfl/data/data_util.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      972 2021-05-28 11:31:00.000000 ibm_watson_machine_learning-1.0.96/ibmfl/data/env_data_handler.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1998 2021-05-28 11:31:00.000000 ibm_watson_machine_learning-1.0.96/ibmfl/data/env_spec.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     2196 2021-05-28 11:31:00.000000 ibm_watson_machine_learning-1.0.96/ibmfl/data/pandas_data_handler.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      744 2021-05-28 11:31:00.000000 ibm_watson_machine_learning-1.0.96/ibmfl/envs.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1287 2021-05-28 11:31:00.000000 ibm_watson_machine_learning-1.0.96/ibmfl/exceptions.py
-drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:02.000000 ibm_watson_machine_learning-1.0.96/ibmfl/message/
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:00.000000 ibm_watson_machine_learning-1.0.96/ibmfl/message/__init__.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1509 2021-05-28 11:31:00.000000 ibm_watson_machine_learning-1.0.96/ibmfl/message/json_serializer.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3749 2021-05-28 11:31:00.000000 ibm_watson_machine_learning-1.0.96/ibmfl/message/message.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1009 2021-05-28 11:31:00.000000 ibm_watson_machine_learning-1.0.96/ibmfl/message/message_type.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1570 2021-05-28 11:31:00.000000 ibm_watson_machine_learning-1.0.96/ibmfl/message/pickle_serializer.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      966 2021-05-28 11:31:00.000000 ibm_watson_machine_learning-1.0.96/ibmfl/message/serializer.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1359 2021-05-28 11:31:00.000000 ibm_watson_machine_learning-1.0.96/ibmfl/message/serializer_factory.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      430 2021-05-28 11:31:00.000000 ibm_watson_machine_learning-1.0.96/ibmfl/message/serializer_types.py
-drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:02.000000 ibm_watson_machine_learning-1.0.96/ibmfl/model/
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:00.000000 ibm_watson_machine_learning-1.0.96/ibmfl/model/__init__.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     9098 2021-05-28 11:31:00.000000 ibm_watson_machine_learning-1.0.96/ibmfl/model/fl_model.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     2125 2021-05-28 11:31:00.000000 ibm_watson_machine_learning-1.0.96/ibmfl/model/model_update.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     7719 2021-05-28 11:31:00.000000 ibm_watson_machine_learning-1.0.96/ibmfl/model/naive_bayes_fl_model.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    25829 2021-05-28 11:31:00.000000 ibm_watson_machine_learning-1.0.96/ibmfl/model/pytorch_fl_model.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    16578 2021-05-28 11:31:00.000000 ibm_watson_machine_learning-1.0.96/ibmfl/model/sklearn_SGD_linear_fl_model.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6978 2021-05-28 11:31:00.000000 ibm_watson_machine_learning-1.0.96/ibmfl/model/sklearn_fl_model.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     9205 2021-05-28 11:31:00.000000 ibm_watson_machine_learning-1.0.96/ibmfl/model/sklearn_kmeans_fl_model.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    23165 2021-05-28 11:31:00.000000 ibm_watson_machine_learning-1.0.96/ibmfl/model/tensorflow_fl_model.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    17461 2021-05-28 11:31:00.000000 ibm_watson_machine_learning-1.0.96/ibmfl/model/xgb_fl_model.py
-drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:02.000000 ibm_watson_machine_learning-1.0.96/ibmfl/party/
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:00.000000 ibm_watson_machine_learning-1.0.96/ibmfl/party/__init__.py
-drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:02.000000 ibm_watson_machine_learning-1.0.96/ibmfl/party/metrics/
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:00.000000 ibm_watson_machine_learning-1.0.96/ibmfl/party/metrics/__init__.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5955 2021-05-28 11:31:00.000000 ibm_watson_machine_learning-1.0.96/ibmfl/party/metrics/metrics_recorder.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    13130 2021-05-28 11:31:00.000000 ibm_watson_machine_learning-1.0.96/ibmfl/party/party.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    12625 2021-05-28 11:31:00.000000 ibm_watson_machine_learning-1.0.96/ibmfl/party/party_protocol_handler.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      533 2021-05-28 11:31:00.000000 ibm_watson_machine_learning-1.0.96/ibmfl/party/status_type.py
-drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:02.000000 ibm_watson_machine_learning-1.0.96/ibmfl/party/training/
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:00.000000 ibm_watson_machine_learning-1.0.96/ibmfl/party/training/__init__.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1342 2021-05-28 11:31:00.000000 ibm_watson_machine_learning-1.0.96/ibmfl/party/training/fedavg_local_training_handler.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    10626 2021-05-28 11:31:00.000000 ibm_watson_machine_learning-1.0.96/ibmfl/party/training/local_training_handler.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1958 2021-05-28 11:31:00.000000 ibm_watson_machine_learning-1.0.96/ibmfl/party/training/pfnm_local_training_handler.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    18051 2021-05-28 11:31:00.000000 ibm_watson_machine_learning-1.0.96/ibmfl/party/training/xgboost_local_training_handler.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1387 2021-05-28 11:31:00.000000 ibm_watson_machine_learning-1.0.96/ibmfl/party_env_validator.py
-drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:02.000000 ibm_watson_machine_learning-1.0.96/ibmfl/util/
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:00.000000 ibm_watson_machine_learning-1.0.96/ibmfl/util/__init__.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    19419 2021-05-28 11:31:00.000000 ibm_watson_machine_learning-1.0.96/ibmfl/util/config.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     7903 2021-05-28 11:31:00.000000 ibm_watson_machine_learning-1.0.96/ibmfl/util/fl_metrics.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5534 2021-05-28 11:31:00.000000 ibm_watson_machine_learning-1.0.96/ibmfl/util/log_config.py
-drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:02.000000 ibm_watson_machine_learning-1.0.96/ibmfl/util/pfnm/
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:00.000000 ibm_watson_machine_learning-1.0.96/ibmfl/util/pfnm/__init__.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     9849 2021-05-28 11:31:00.000000 ibm_watson_machine_learning-1.0.96/ibmfl/util/pfnm/core.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    12441 2021-05-28 11:31:00.000000 ibm_watson_machine_learning-1.0.96/ibmfl/util/pfnm/matching.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3027 2021-05-28 11:31:00.000000 ibm_watson_machine_learning-1.0.96/ibmfl/util/pfnm/utils.py
-drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-28 11:31:02.000000 ibm_watson_machine_learning-1.0.96/ibmfl/util/xgboost/
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      291 2021-05-28 11:31:00.000000 ibm_watson_machine_learning-1.0.96/ibmfl/util/xgboost/__init__.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4110 2021-05-28 11:31:00.000000 ibm_watson_machine_learning-1.0.96/ibmfl/util/xgboost/export.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     7774 2021-05-28 11:31:00.000000 ibm_watson_machine_learning-1.0.96/ibmfl/util/xgboost/hyperparams.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      777 2021-05-28 11:31:00.000000 ibm_watson_machine_learning-1.0.96/ibmfl/util/xgboost/utils.py
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      228 2021-05-28 11:31:02.000000 ibm_watson_machine_learning-1.0.96/setup.cfg
--rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     2715 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.96/setup.py
+drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:08.000000 ibm_watson_machine_learning-1.0.99/
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)       78 2021-06-09 14:15:07.000000 ibm_watson_machine_learning-1.0.99/MANIFEST.in
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1954 2021-06-09 14:15:08.000000 ibm_watson_machine_learning-1.0.99/PKG-INFO
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      578 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/README.md
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)        7 2021-06-09 14:15:07.000000 ibm_watson_machine_learning-1.0.99/VERSION
+drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:08.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     7762 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/Set.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1343 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/__init__.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    32184 2021-06-08 13:02:33.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/assets.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    24053 2021-06-02 07:52:53.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/client.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    22790 2021-06-08 13:02:33.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/connections.py
+drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:08.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/deployment/
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      641 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/deployment/__init__.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    29456 2021-05-28 11:30:28.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/deployment/base_deployment.py
+-rwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)    23366 2021-06-02 08:06:27.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/deployment/batch.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    10718 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/deployment/web_service.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    72352 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/deployments.py
+drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:08.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/experiment/
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      652 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/experiment/__init__.py
+drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:08.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/experiment/autoai/
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      580 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/experiment/autoai/__init__.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    21814 2021-06-08 13:05:40.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/experiment/autoai/autoai.py
+drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:08.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/experiment/autoai/engines/
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      667 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/experiment/autoai/engines/__init__.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     2132 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/experiment/autoai/engines/base_engine.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    44266 2021-06-08 13:05:40.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/experiment/autoai/engines/wml_engine.py
+drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:08.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/experiment/autoai/optimizers/
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      800 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/experiment/autoai/optimizers/__init__.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1878 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/experiment/autoai/optimizers/base_auto_pipelines.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    29767 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/experiment/autoai/optimizers/local_auto_pipelines.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    33165 2021-06-08 13:05:40.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/experiment/autoai/optimizers/remote_auto_pipelines.py
+drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:08.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/experiment/autoai/runs/
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      793 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/experiment/autoai/runs/__init__.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    17348 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/experiment/autoai/runs/auto_pipelines_runs.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1736 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/experiment/autoai/runs/base_auto_pipelines_runs.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     9372 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/experiment/autoai/runs/local_auto_pipelines_runs.py
+drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:08.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/experiment/base_experiment/
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      678 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/experiment/base_experiment/__init__.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1019 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/experiment/base_experiment/base_experiment.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    23394 2021-06-08 13:02:33.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/experiments.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    20611 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/export_assets.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    53372 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/functions.py
+drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:08.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/helpers/
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      921 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/helpers/__init__.py
+drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:08.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/helpers/connections/
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      930 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/helpers/connections/__init__.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      869 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/helpers/connections/base_connection.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    24253 2021-06-02 08:52:50.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/helpers/connections/base_data_connection.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      919 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/helpers/connections/base_location.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    47007 2021-06-08 12:18:03.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/helpers/connections/connections.py
+drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:08.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/helpers/flight/
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/helpers/flight/__init__.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3482 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/helpers/flight/errors.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    15392 2021-06-08 12:16:21.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/helpers/flight/service.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    11864 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/helpers/flight/utils.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3357 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/helpers/helpers.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5478 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/hpo.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    22441 2021-05-28 11:30:28.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/href_definitions.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    17343 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/hw_spec.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    15337 2021-06-08 13:02:33.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/import_assets.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    10632 2021-06-02 07:52:53.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/instance.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    15895 2021-06-02 07:52:53.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/instance_new_plan.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    20082 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/learning_system.py
+drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:08.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      579 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/__init__.py
+drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:08.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/mlpipelinepy/
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      902 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/mlpipelinepy/__init__.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1949 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/mlpipelinepy/edge.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1002 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/mlpipelinepy/exception.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5877 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/mlpipelinepy/javaproxy.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    10776 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/mlpipelinepy/mlpipeline.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1289 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/mlpipelinepy/serialization.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1670 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/mlpipelinepy/utils.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      955 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/mlpipelinepy/version.py
+drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:08.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/pipeline/
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    12138 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/pipeline/DAG.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    14274 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/pipeline/IBMSparkPipeline.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6317 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/pipeline/IBMSparkPipelineModel.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3090 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/pipeline/Result.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     2493 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/pipeline/Sink.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     2527 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/pipeline/Source.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    11223 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/pipeline/Wrapper.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      804 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/pipeline/__init__.py
+drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:08.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6070 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/TestRepoSaveLoad.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      830 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/__init__.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1433 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/base_constants.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3462 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/ml_api_client.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     7251 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/ml_authorization.py
+drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:08.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepository/
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1711 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepository/__init__.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4318 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepository/artifact.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      931 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepository/artifact_reader.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1149 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepository/generic_archive_model_artifact.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1179 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepository/generic_archive_pipeline_artifact.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1117 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepository/hybrid_model_artifact.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    11184 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepository/meta_names.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1546 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepository/meta_props.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1433 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepository/model_artifact.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1044 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepository/pipeline_artifact.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1283 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepository/scikit_model_artifact.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1134 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepository/tensorflow_model_artifact.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1067 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepository/wml_experiment_artifact.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1049 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepository/wml_function_artifact.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1062 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepository/wml_libraries_artifact.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1061 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepository/wml_runtimes_artifact.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1120 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepository/xgboost_model_artifact.py
+drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:08.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     2782 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/__init__.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6718 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/content_loaders.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1966 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/experiment_artifact.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1990 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/function_artifact.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1558 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/function_artifact_loader.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1177 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/function_artifact_reader.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1175 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/function_loader.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6579 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/generic_archive_pipeline_model_artifact.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1694 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/generic_file_artifact_loader.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1286 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/generic_file_pipeline_model_loader.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1514 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/generic_file_reader.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4512 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/hybrid_artifact_loader.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     2302 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/hybrid_pipeline_model_artifact.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1231 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/hybrid_pipeline_model_loader.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     2384 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/hybrid_pipeline_model_reader.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3696 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/libraries_artifact.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1994 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/libraries_artifact_loader.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1169 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/libraries_artifact_reader.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      976 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/libraries_loader.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    19703 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/ml_repository_artifact.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      754 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/python_version.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     2913 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/runtimes_artifact.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     2037 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/runtimes_artifact_loader.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1174 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/runtimes_artifact_reader.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     2601 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/scikit_artifact_loader.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    14968 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/scikit_pipeline_model_artifact.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1496 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/scikit_pipeline_model_loader.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3245 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/scikit_pipeline_reader.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     2027 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/spark_artifact_loader.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     2939 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/spark_pipeline_artifact.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      905 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/spark_pipeline_loader.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    10858 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/spark_pipeline_model_artifact.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      936 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/spark_pipeline_model_loader.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     2561 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/spark_pipeline_reader.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1203 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/spark_version.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     2097 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/tensorflow_artifact_loader.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    10261 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/tensorflow_pipeline_model_artifact.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     2400 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/tensorflow_pipeline_model_loader.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4136 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/tensorflow_pipeline_reader.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6465 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/version_helper.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3071 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/xgboost_model_reader.py
+drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:08.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1627 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/__init__.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     2805 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/content_reader.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6830 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/experiment_adapter.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    18004 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/experiment_collection.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6335 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/function_adapter.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    15143 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/function_collection.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3099 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/libraries_adapter.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     9960 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/libraries_collection.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    11683 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/ml_repository_api.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5094 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/ml_repository_client.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    15089 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/model_adapter.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    60931 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/model_collection.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     2933 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/runtimes_adapter.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    10138 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/runtimes_collection.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3003 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/wml_experiment_adapter.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    22480 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/wml_experiment_collection.py
+drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:08.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    12612 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/__init__.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    23112 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/api_client.py
+drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:08.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/apis/
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      725 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/apis/__init__.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)   259498 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/apis/repository_api.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    12406 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/apis/token_api.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     9707 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/configuration.py
+drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:08.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    13430 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/__init__.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3364 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/array_data_input_repository.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5459 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/array_model_metrics_output.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5414 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/array_model_output.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3489 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/array_model_version_metrics_experiments.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5477 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/array_model_version_output.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5441 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/array_pipeline_output.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5504 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/array_pipeline_version_output.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4201 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/array_training_output_experiments.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5360 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/artifact_author.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6561 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/artifact_version_metadata.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5066 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/artifact_version_repository.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5921 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/artifact_version_short_metadata.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3949 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/author_experiments.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3838 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/author_repository.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5960 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/batch_deploy_output.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5500 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/batch_deploy_output_entity.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     8254 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/batch_deploy_output_entity_execution.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5850 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/batch_deploy_output_meta.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     7401 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/batch_input.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5912 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/batch_output.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5413 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/batch_output_array.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4777 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/cols_output.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4630 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/compute_configuration_experiments.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4777 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/connection.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5405 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/connection_object_source_experiments.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5405 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/connection_object_target_experiments.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5609 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/connection_object_with_name_repository.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6676 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/content_location.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4262 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/content_status.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4753 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/custom_models.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6274 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/deploy_input.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4496 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/error_bad_request_libraries_target.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5737 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/error_experiments.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4522 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/error_experiments_target.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     7035 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/error_message.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5544 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/error_repository.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4384 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/error_repository_target.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4633 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/error_schema_experiments.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4486 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/error_schema_repository.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6109 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/evaluation_definition.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5048 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/evaluation_definition_experiments.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6151 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/evaluation_definition_metrics.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5047 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/evaluation_definition_repository.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5740 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/evaluation_definition_repository_metrics.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     7751 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/experiment_input.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6911 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/experiment_input_settings.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4706 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/experiment_output.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5917 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/experiment_output_array.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3985 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/experiment_output_array_first.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3449 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/experiment_patch.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     9291 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/experiment_status_experiments.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6711 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/framework_output_repository.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4580 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/framework_output_repository_libraries.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4568 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/framework_output_repository_runtimes.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     7180 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/hyper_parameters.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     7821 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/hyper_parameters_experiments.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6100 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/hyper_parameters_experiments_double_range.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6100 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/hyper_parameters_experiments_inner_double_range.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6028 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/hyper_parameters_experiments_inner_int_range.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5344 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/hyper_parameters_experiments_inner_values_range.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6028 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/hyper_parameters_experiments_int_range.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3489 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/hyper_parameters_for_status_experiments.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4890 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/hyper_parameters_for_status_experiments_inner.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5132 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/hyper_parameters_optimization_experiments.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5288 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/hyper_parameters_optimization_experiments_method.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6480 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/hyper_parameters_optimization_experiments_method_parameters.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4788 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/input_data_schema.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6109 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/internal_input_batch.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6112 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/internal_output_batch.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4785 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/json_patch_array.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6533 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/json_patch_entity.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6444 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/libraries_definition_input.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4598 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/libraries_definition_input_platform.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5362 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/meta_object.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4123 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/meta_object_experiments.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5980 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/meta_object_experiments_metadata.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5768 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/meta_object_functions_metadata.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     9800 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/meta_object_metadata.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4009 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/meta_object_repository.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     8681 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/meta_object_repository_metadata.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4600 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/metric_object_experiments.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4755 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/metrics_models.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     7514 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_experiment_input.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4688 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_experiment_output.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4141 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_experiment_output_array.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     9094 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_function_input.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4641 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_functions_output.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6160 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_functions_output_array.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3958 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_functions_output_array_first.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4678 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_libraries_output.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6160 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_libraries_output_array.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3958 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_libraries_output_array_first.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    20734 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_model_input.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4638 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_model_output.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4075 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_model_output_array.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4728 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_patch_libraries_output.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4700 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_runtime_spec_output.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6214 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_runtime_spec_output_array.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3970 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_runtime_spec_output_array_first.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     2493 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_get_presigned_url_output.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     2504 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_model_size_output.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4561 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_patch_function.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3370 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_patch_libraries_input.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3374 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_patch_runtime_spec_input.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4682 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_patch_runtime_spec_output.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4697 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_upload_content_output.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4089 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_upload_content_output_entity.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5912 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_upload_content_output_metadata.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     7827 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/model_content_location.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3917 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/model_definition_models.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    13915 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/model_input.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6063 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/model_metrics.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5955 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/model_metrics_values.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5946 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/model_output.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    15820 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/model_output_entity.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6269 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/model_output_entity_pipeline_version.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6194 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/model_schemas.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6271 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/model_training_data_ref.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4776 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/model_type.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6389 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/model_version_input.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4738 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/model_version_metrics_experiments.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6037 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/model_version_output.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    11117 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/model_version_output_entity.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6027 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/model_version_output_entity_model.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5983 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/online_deploy_output.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5923 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/online_output.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5461 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/online_output_array.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4761 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/output_data_schema.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5998 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/patch_operation_experiments.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5844 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/patch_operation_functions.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5844 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/patch_operation_libraries.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5880 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/patch_operation_runtime_spec.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     8144 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/pipeline_input.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4417 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/pipeline_models.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5985 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/pipeline_output.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    10863 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/pipeline_output_entity.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4782 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/pipeline_type.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5724 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/pipeline_version_input.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6076 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/pipeline_version_output.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6356 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/pipeline_version_output_entity.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6115 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/pipeline_version_output_entity_parent.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4793 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/runtime_environment.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3925 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/runtime_models.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4480 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/runtime_output_repository.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     7166 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/runtime_spec_definition_input.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4072 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/runtime_spec_definition_input_custom_libraries.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4590 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/runtime_spec_definition_input_platform.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5485 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/runtime_spec_definition_input_public_libraries.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3940 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/runtime_spec_definition_input_repository.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4781 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/sample_scoring_input.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     7590 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/schemas.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5408 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/score_input.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5308 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/score_output.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6258 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/size_models.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3908 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/software_spec_models.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4395 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/space_models.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6135 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/spark_service.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6250 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/stream_input_internal.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     7487 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/stream_internal.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5922 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/stream_output.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5422 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/stream_output_array.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6320 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/stream_output_internal.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4576 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/tag_repository.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5331 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/token_response.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4782 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/training_data_schema.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3931 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/training_models.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4747 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/training_output_experiments.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     8939 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/training_reference_experiments.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    14844 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/training_status_experiments.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4213 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/training_status_experiments_result.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    13111 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/rest.py
+drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:08.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/util/
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      776 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/util/__init__.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      969 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/util/base_singleton.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1422 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/util/compression_util.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      793 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/util/exceptions.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      899 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/util/file_system_ops.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1243 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/util/generic_archive_file_check.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1515 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/util/json_2_object_mapper.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4252 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/util/library_imports.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     2779 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/util/spark_util.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      771 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/util/unique_id_gen.py
+drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:08.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/messages/
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-02 07:52:53.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/messages/__init__.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      446 2021-06-02 07:52:53.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/messages/globalization_util.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     2041 2021-06-02 07:52:53.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/messages/messages.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     7051 2021-06-08 13:02:33.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/messages/messages_en.json
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    70272 2021-06-09 09:36:04.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/metanames.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    15892 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/migration_v4ga_cloud.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    52929 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/model_definition.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)   151533 2021-05-28 11:30:28.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/models.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    31295 2021-06-08 13:02:33.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/pipelines.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    23457 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/pkg_extn.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    32299 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/platform_spaces.py
+drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:08.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/preprocessing/
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      761 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/preprocessing/__init__.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    30660 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/preprocessing/data_join_pipeline.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    18341 2021-02-15 10:28:26.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/preprocessing/multiple_files_preprocessor.py
+drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:08.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/preprocessing/templates/
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      579 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/preprocessing/templates/__init__.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1498 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/preprocessing/templates/pretty_print_template.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    17709 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/remote_training_system.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    96117 2021-06-08 13:02:33.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/repository.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    50300 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/runtimes.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    53325 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/script.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    45756 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/shiny.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    33234 2021-06-08 13:02:33.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/spaces.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    26470 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/sw_spec.py
+drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:08.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/
+drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:08.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    12423 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/Connections_SPSS_BIGQUERY_MYSQL_spaces_cp4d_35.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    12000 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/Connections_SPSS_MSSQL_spaces_cp4d_35.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    12545 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/Connections_SPSS_TERADATA_MYSQL_spaces_cp4d_35.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     2406 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/DataAssets_spaces_cp4d_35.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    14215 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/Experiment_Pipeline_spaces_cp4d_35.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    12257 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/ExportImport_spaces_cp4d_35.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    14233 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/Functions_spaces_cp4d_35.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      978 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/HardwareSpec_spaces_cp4d_35.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    13061 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/ModeDoFromFile_spaces_cp4d_35.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4614 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/ModelDefinition_projects_dev_cp4d_35.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5727 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/ModelDefinition_spaces_cp4d_35.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4655 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/ModelPMML_spaces_cp4d_35.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    18665 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/Model_Hybrid_from_zipfile_spaces_cp4d_35.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4043 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/Model_keras_spaces_cp4d_35.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3834 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/Model_pmml_spaces_cp4d_35.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    11402 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/Model_scikit_learn_from_object_sw_spaces_cp4d_35.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5867 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/Model_spark_mllib_from_object_spaces_cp4d_35.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6922 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/Model_spss_from_file_spaces_cp4d_35.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3832 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/Model_tensorflow_spaces_cp4d_35.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6532 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/PkgExt_spaces_cp4d_35.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     9489 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/RScripts_spaces_cp4d_35.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3827 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/RShiny_projects_dev_cp4d_35.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     7133 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/RShiny_spaces_cp4d_35.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3810 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/Remote_training_systems_spaces_cp4d_35.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3995 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/Scripts_projects_dev_cp4d_35.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     9446 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/Scripts_spaces_cp4d_35.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3921 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/SoftwareSpec_projects_dev_cp4d_35.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4852 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/SoftwareSpec_spaces_cp4d_35.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/__init__.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5531 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/models_preparation.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    13538 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/preparation_and_cleaning.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     9578 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/spaces_cp4d_35.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    11346 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/test_CP4D_3_connections.py
+drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:08.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/Cloud/
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     2916 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/Cloud/DataAssets_spaces_cloud.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    14725 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/Cloud/Experiment_Pipeline_spaces_cloud.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    12736 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/Cloud/ExportImport_spaces_cloud.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    14404 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/Cloud/Functions_spaces_cloud.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      976 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/Cloud/HardwareSpec_spaces_cloud.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    13692 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/Cloud/ModeDoFromFile_spaces_cloud.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4612 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/Cloud/ModelDefinition_projects_dev_cloud.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6138 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/Cloud/ModelDefinition_spaces_cloud.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5191 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/Cloud/ModelPMML_spaces_cloud.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    19221 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/Cloud/Model_Hybrid_from_zipfile_spaces_cloud.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4747 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/Cloud/Model_keras_spaces_cloud.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4379 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/Cloud/Model_pmml_spaces_cloud.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    11938 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/Cloud/Model_scikit_learn_from_object_sw_spaces_cloud.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6297 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/Cloud/Model_spark_mllib_from_object_spaces_cloud.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     7447 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/Cloud/Model_spss_from_file_spaces_cloud.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4720 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/Cloud/Model_tensorflow_spaces_cloud.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6535 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/Cloud/PkgExt_spaces_cloud.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3825 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/Cloud/RShiny_projects_dev_cloud.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     7629 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/Cloud/RShiny_spaces_cloud.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4318 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/Cloud/Remote_training_systems_spaces_cloud.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3993 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/Cloud/Scripts_projects_dev_cloud.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    10025 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/Cloud/Scripts_spaces_cloud.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3919 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/Cloud/SoftwareSpec_projects_dev_cloud.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5245 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/Cloud/SoftwareSpec_spaces_cloud.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/Cloud/__init__.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5521 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/Cloud/models_preparation.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    13494 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/Cloud/preparation_and_cleaning.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    11254 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/Cloud/spaces_cloud.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1938 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/ConfigFileEncoder.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1530 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/ConfigFileGenerator.py
+drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:08.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/ICP/
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5172 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/ICP/CP4D_mllib_from_object.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/ICP/__init__.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5524 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/ICP/models_preparation.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    13270 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/ICP/preparation_and_cleaning.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     7058 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/ICP/test-CP4D_3_hybrid_autoai_model.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     8854 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/ICP/test_CP4D_3_connections.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     8434 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/ICP/test_CP4D_3_cross_deployment_model_function.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     8486 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/ICP/test_CP4D_3_cross_deployment_model_model.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    11913 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/ICP/test_CP4D_3_do_from_file.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6139 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/ICP/test_CP4D_3_functions_sw.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     9843 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/ICP/test_CP4D_3_import_export_spaces.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5289 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/ICP/test_CP4D_3_mllib_2_4_from_object_sw.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5189 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/ICP/test_CP4D_3_pkg_extn.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     7348 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/ICP/test_CP4D_3_rshiny.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     9751 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/ICP/test_CP4D_3_scikit_learn_from_object_sw.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     8641 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/ICP/test_CP4D_3_scripts.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3058 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/ICP/test_CP4D_3_software_spec.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6343 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/ICP/test_CP4D_3_spss_from_file.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6087 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/ICP/test_CP4D_functions.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5156 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/ICP/test_CP4D_runtimes.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     8029 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/ICP/test_CP4D_scikit_learn_from_object.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4836 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/ICP/test_CP4D_spaces.py
+drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:08.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/WSD/
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3907 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/WSD/WSD_functions.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     2431 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/WSD/WSD_mllib_from_object.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3245 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/WSD/WSD_scikit_learn_from_object.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/WSD/__init__.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5521 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/WSD/models_preparation.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    13270 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/WSD/preparation_and_cleaning.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/__init__.py
+drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:08.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-02-12 13:14:02.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/__init__.py
+drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:08.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/fvt/
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/fvt/__init__.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     8141 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/fvt/local_optimizer_for_CP4D35.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3839 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/fvt/test__lale__breast_cancer.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     9482 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/fvt/test_any_autoai_experiment__lale__.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     9992 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/fvt/test_breast_cancer_binary_lgbm.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     9996 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/fvt/test_breast_cancer_binary_sklearn.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     9987 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/fvt/test_breast_cancer_binary_xgboost.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4438 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/fvt/test_credit_risk_binary_local_ai4ml.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    16696 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/fvt/test_custom_separator_binary_multiclass_regression.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     9981 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/fvt/test_insurance_regression_lgbm.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     9896 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/fvt/test_insurance_regression_sklearn.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     9980 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/fvt/test_insurance_regression_xgboost.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    21581 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/fvt/test_iris_wml_autoai_multiclass_CP4D_3_5.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    15154 2021-04-21 14:01:07.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/fvt/test_local_optimizer_with_cos.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    38103 2021-04-21 14:01:07.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/fvt/test_obm_plus_kb_go_sales_multiclass.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     9805 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/fvt/test_student_multiclass_lgbm.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     9808 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/fvt/test_student_multiclass_sklearn.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     9804 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/fvt/test_student_multiclass_xgboost.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    19355 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/fvt/test_xlsx_read_binary_regression.py
+drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:08.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/manual/
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/manual/__init__.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    17335 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/manual/test_bank_binary.py
+drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:08.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/__init__.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3284 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/abstract_test_iris_using_database_connection.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3468 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/abstract_test_iris_using_database_data_asset.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    19330 2021-05-28 11:30:28.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/abstract_test_iris_wml_autoai_multiclass_connections.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    26783 2021-06-09 14:14:41.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_arabicghosts_multiclass_snapml.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     7868 2021-06-08 13:02:33.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_auth.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    21956 2021-06-08 13:02:33.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_bank_wml_autoai_xlsx_binary.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    21285 2021-05-28 11:30:28.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_breast_cancer_wml_autoai_csv_binary.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    21930 2021-05-28 11:30:28.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_breast_cancer_wml_autoai_csv_binary_apikey_auth.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    21759 2021-05-28 11:30:28.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_breast_cancer_wml_autoai_csv_binary_token_auth.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    24694 2021-06-02 07:52:53.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_car_price_wml_autoai_regression.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    15410 2021-05-28 11:30:28.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_credit_risk_as_sample_notebook_binary.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    27435 2021-06-09 14:14:41.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_credit_risk_binary_snapml.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    11682 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_drop_duplicates.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    18183 2021-06-08 13:05:40.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_drug_fairnessmetric_autoai_multiclass.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    28339 2021-06-09 14:14:41.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_housing_reegression_snapml.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    17996 2021-06-08 13:05:40.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_insurance_fairnessmetric_autoai_regression.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    14562 2021-05-28 11:30:28.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_insurance_wml_autoai_xlsx_regression.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4818 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_iris_using_data_asset_and_connected_asset.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4031 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_iris_using_data_asset_and_default.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3778 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_iris_using_data_connected_asset_and_connected_asset.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3534 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_iris_using_data_connected_asset_and_default.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4082 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_iris_using_data_connected_asset_and_s3.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4162 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_iris_using_data_s3_and_connected_asset.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3223 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_iris_using_data_s3_and_s3.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1162 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_iris_using_database_connection.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1402 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_iris_using_database_data_asset.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3251 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_iris_using_filesystem_and_connected_asset.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1512 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_iris_using_filesystem_and_default.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    23732 2021-06-02 07:52:53.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_iris_wml_autoai_multiclass.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    24647 2021-05-28 11:30:28.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_iris_wml_autoai_multiclass_connections.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    22279 2021-05-28 11:30:28.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_iris_wml_autoai_multiclass_space_only.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    22926 2021-05-28 11:30:28.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_iris_wml_autoai_multiclass_using_NFS.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    21160 2021-05-28 11:30:28.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_iris_wml_autoai_multiclass_using_data_asset.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    24493 2021-06-02 07:52:53.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_obm_group_customer.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    43413 2021-05-28 11:30:28.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_obm_plus_kb_group_customer_regression.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    43137 2021-06-02 07:52:53.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_obm_plus_kb_group_customer_regression_csv_only.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    40754 2021-06-02 07:52:53.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_obm_plus_kb_temp_binary.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    19778 2021-05-28 11:30:28.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_text_transformer_csv_multiclass.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    20033 2021-05-28 11:30:28.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_text_transformer_csv_regression.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    20364 2021-05-28 11:30:28.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_text_transformer_donorchoose_binary.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    21587 2021-05-28 11:30:28.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_text_transformer_fake_job_position_binary.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    20103 2021-05-28 11:30:28.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_twitter_wml_autoai_csv_forecasting.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    20104 2021-05-28 11:30:28.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_twitter_wml_autoai_csv_forecasting_multivariate.py
+drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:08.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/unit/
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/unit/__init__.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6294 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/unit/test_auto_pipeline_runs.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1560 2021-02-15 07:14:10.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/unit/test_check_dependencies_versions.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     8031 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/unit/test_data_connection.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     9446 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/unit/test_data_join_pipeline_graph.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4518 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/unit/test_get_obm_output.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4099 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/unit/test_local_auto_pipeline.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1504 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/unit/test_next_run_details_generator.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      804 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/unit/test_piepeline_to_script.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     2538 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/unit/test_prepare_auto_ai_model_to_publish.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4156 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/unit/test_prepare_cos_client.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4910 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/unit/test_tshirt_sizes_limitation.py
+drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:08.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/contract_tests/
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/contract_tests/__init__.py
+drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:08.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/deployment/
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/deployment/__init__.py
+drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:08.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/deployment/unit/
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/deployment/unit/__init__.py
+-rwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)     7748 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/deployment/unit/test_batch.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5497 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/deployment/unit/test_web_service.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3132 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/install_requirements.py
+drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:08.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6017 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4functions.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5281 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4pipelines.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6830 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_ai_functions_from_func.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)   452070 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_ai_functions_from_func_sklearn_preprocessing.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3425 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_ai_functions_from_gz.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5679 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_ai_functions_from_gz_keras.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5100 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_ai_functions_from_gz_mandatory_params.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    11502 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_do_from_tar_gz.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    11829 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_experiment_and_pipelines.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6488 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_keras_from_file_V4.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     8922 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_keras_from_object_V4_disable.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     7521 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_keras_from_tgz.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5074 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_libraries_experiments.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6086 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_pmml_from_xml.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6463 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_pytorch_from_tar_gz.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3698 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_runtimes_custom_libs.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4142 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_runtimes_custom_libs_attaching_to_model_from_archive.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4379 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_runtimes_custom_libs_attaching_to_model_from_object.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3378 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_runtimes_custom_libs_delete_orphaned_libs.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3591 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_runtimes_custom_libs_yaml_upload.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1899 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_runtimes_mandatory_params.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     8452 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_scikit_learn_from_directory.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     7621 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_scikit_learn_from_object.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6152 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_scikit_learn_from_tar_gz.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5980 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_scikit_xgboost_from_directory.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5951 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_scikit_xgboost_from_object.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6265 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_scikit_xgboost_from_tar_gz.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4486 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_spaces.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5900 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_spark_mllib_from_object.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     8134 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_spark_mllib_from_tar_gz.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6554 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_spss_from_file.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5451 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_tensorflow_from_directory.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6526 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_tensorflow_from_file.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     8852 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_tensorflow_training.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     9421 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_training_from_pipeline.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6170 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_xgboost_from_directory.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     7180 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_xgboost_from_json.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6513 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_xgboost_from_object.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6059 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_xgboost_from_tar_gz.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/__init__.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     8800 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/_test_scikit_learn_grid_search_xgboost_panda_table_disable.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4590 2021-02-12 13:14:04.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/_test_spark_mllib_from_directory_disable.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4601 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/cloud_mllib_from_object.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     7478 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/models_preparation.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    13270 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/preparation_and_cleaning.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4896 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/runtimesV4.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    12622 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_ai_functions_from_func_hitting_scoring_disable.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5287 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_ai_functions_from_gz_disable.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6165 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_ai_functions_from_wrapper_func_disable.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    16318 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_caffe_experiment_disable.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1977 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_clean_disable.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5420 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_coreml_from_caffe_200Mb_model_disable.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     7591 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_coreml_from_caffe_disable.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    13128 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_coreml_from_keras_disable.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4959 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_coreml_from_scikit_disable.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5106 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_coreml_from_xgboost_disable.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    16555 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_keras_experiment_disable.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    15154 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_keras_experiment_hpo_disable.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    11579 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_keras_experiment_learning_system_disable.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    21123 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_keras_experiment_monitor_metrics_disable.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3536 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_keras_from_file.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3178 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_load_30Mb_model_disable.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    20986 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_pytorch_experiment_disable.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    11727 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_repository_limit_disable.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4252 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_runtimes_custom_libs_attaching_to_simple_model_v4.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     7789 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_scikit_learn_from_object_refresh_token_disable.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     8439 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_scikit_learn_grid_search_xgboost_numpy_table_disable.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    10939 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_spark_mllib_with_learning_system_disable.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    12041 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_tensorflow_distributed_ddl_experiment_disable.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    14722 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_tensorflow_distributed_horovod_training_disable.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    15543 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_tensorflow_distributed_training_disable.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    14266 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_tensorflow_experiment_disable.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    15600 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_tensorflow_experiment_hpo_disable.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    14255 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_tensorflow_experiment_hpo_light_disable.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    12227 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_tensorflow_experiment_mandatory_params_only_disable.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    15084 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_tensorflow_experiment_monitor_metrics_disable.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    15717 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_tensorflow_experiment_sync_disable.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    13457 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_tensorflow_training_mandatory_params_only_disable.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    14671 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_tensorflow_training_v4_disable.py
+drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:08.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/utils/
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)       20 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/utils/__init__.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      254 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/utils/assertions.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     2368 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/utils/cleanup.py
+drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:08.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/utils/openshift/
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/utils/openshift/__init__.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      717 2021-02-12 13:14:05.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/utils/openshift/cli.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     2188 2021-02-12 13:14:06.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/utils/openshift/prometheusapi.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    15370 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/utils/utils.py
+drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:08.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/workspace/
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-02-12 13:14:06.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/workspace/__init__.py
+drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:08.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/workspace/unit/
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-02-12 13:14:06.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/workspace/unit/__init__.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1304 2021-02-12 13:14:06.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/workspace/unit/test_workspace.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    50091 2021-06-08 13:02:33.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/training.py
+drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:08.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/utils/
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      634 2021-02-12 13:14:06.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/utils/__init__.py
+drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:08.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/utils/autoai/
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      579 2021-02-12 13:14:06.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/utils/autoai/__init__.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     7152 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/utils/autoai/connection.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     8598 2021-06-09 14:14:41.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/utils/autoai/enums.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    12866 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/utils/autoai/errors.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3458 2021-02-12 13:14:06.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/utils/autoai/local_training_message_handler.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     2461 2021-02-12 13:14:06.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/utils/autoai/progress_bar.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1524 2021-02-12 13:14:06.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/utils/autoai/training.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    65718 2021-06-08 13:05:40.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/utils/autoai/utils.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3104 2021-02-12 13:14:06.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/utils/autoai/watson_studio.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    23344 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/utils/autoai/wsd_ui.py
+drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:08.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/utils/deployment/
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      579 2021-02-12 13:14:06.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/utils/deployment/__init__.py
+-rwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3126 2021-05-28 11:30:28.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/utils/deployment/errors.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    16263 2021-02-12 13:14:06.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/utils/utils.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    22363 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/volumes.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4684 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/wml_client_error.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    35991 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/wml_resource.py
+drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:08.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/workspace/
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      650 2021-02-12 13:14:06.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/workspace/__init__.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     7893 2021-05-27 09:56:16.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/workspace/workspace.py
+drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:08.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning.egg-info/
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1954 2021-06-09 14:15:07.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning.egg-info/PKG-INFO
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    50589 2021-06-09 14:15:07.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning.egg-info/SOURCES.txt
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)        1 2021-06-09 14:15:07.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning.egg-info/dependency_links.txt
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)       92 2021-06-09 14:15:07.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning.egg-info/requires.txt
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)       34 2021-06-09 14:15:07.000000 ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning.egg-info/top_level.txt
+drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:08.000000 ibm_watson_machine_learning-1.0.99/ibmfl/
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:06.000000 ibm_watson_machine_learning-1.0.99/ibmfl/__init__.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)       22 2021-06-09 14:15:06.000000 ibm_watson_machine_learning-1.0.99/ibmfl/_version.py
+drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:08.000000 ibm_watson_machine_learning-1.0.99/ibmfl/connection/
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:06.000000 ibm_watson_machine_learning-1.0.99/ibmfl/connection/__init__.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     2945 2021-06-09 14:15:06.000000 ibm_watson_machine_learning-1.0.99/ibmfl/connection/connection.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     2467 2021-06-09 14:15:06.000000 ibm_watson_machine_learning-1.0.99/ibmfl/connection/route_declarations.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     2400 2021-06-09 14:15:06.000000 ibm_watson_machine_learning-1.0.99/ibmfl/connection/router_handler.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    17900 2021-06-09 14:15:06.000000 ibm_watson_machine_learning-1.0.99/ibmfl/connection/websockets_connection.py
+drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:08.000000 ibm_watson_machine_learning-1.0.99/ibmfl/data/
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:06.000000 ibm_watson_machine_learning-1.0.99/ibmfl/data/__init__.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     7979 2021-06-09 14:15:06.000000 ibm_watson_machine_learning-1.0.99/ibmfl/data/data_handler.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    14780 2021-06-09 14:15:06.000000 ibm_watson_machine_learning-1.0.99/ibmfl/data/data_util.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      972 2021-06-09 14:15:06.000000 ibm_watson_machine_learning-1.0.99/ibmfl/data/env_data_handler.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1998 2021-06-09 14:15:06.000000 ibm_watson_machine_learning-1.0.99/ibmfl/data/env_spec.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     2196 2021-06-09 14:15:06.000000 ibm_watson_machine_learning-1.0.99/ibmfl/data/pandas_data_handler.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      744 2021-06-09 14:15:06.000000 ibm_watson_machine_learning-1.0.99/ibmfl/envs.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1388 2021-06-09 14:15:06.000000 ibm_watson_machine_learning-1.0.99/ibmfl/exceptions.py
+drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:08.000000 ibm_watson_machine_learning-1.0.99/ibmfl/message/
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:06.000000 ibm_watson_machine_learning-1.0.99/ibmfl/message/__init__.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1509 2021-06-09 14:15:06.000000 ibm_watson_machine_learning-1.0.99/ibmfl/message/json_serializer.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3749 2021-06-09 14:15:06.000000 ibm_watson_machine_learning-1.0.99/ibmfl/message/message.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      919 2021-06-09 14:15:06.000000 ibm_watson_machine_learning-1.0.99/ibmfl/message/message_type.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1570 2021-06-09 14:15:06.000000 ibm_watson_machine_learning-1.0.99/ibmfl/message/pickle_serializer.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      966 2021-06-09 14:15:06.000000 ibm_watson_machine_learning-1.0.99/ibmfl/message/serializer.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1359 2021-06-09 14:15:06.000000 ibm_watson_machine_learning-1.0.99/ibmfl/message/serializer_factory.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      430 2021-06-09 14:15:06.000000 ibm_watson_machine_learning-1.0.99/ibmfl/message/serializer_types.py
+drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:08.000000 ibm_watson_machine_learning-1.0.99/ibmfl/model/
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:06.000000 ibm_watson_machine_learning-1.0.99/ibmfl/model/__init__.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     9098 2021-06-09 14:15:06.000000 ibm_watson_machine_learning-1.0.99/ibmfl/model/fl_model.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     2469 2021-06-09 14:15:06.000000 ibm_watson_machine_learning-1.0.99/ibmfl/model/model_update.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     7719 2021-06-09 14:15:06.000000 ibm_watson_machine_learning-1.0.99/ibmfl/model/naive_bayes_fl_model.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    25853 2021-06-09 14:15:06.000000 ibm_watson_machine_learning-1.0.99/ibmfl/model/pytorch_fl_model.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    16578 2021-06-09 14:15:06.000000 ibm_watson_machine_learning-1.0.99/ibmfl/model/sklearn_SGD_linear_fl_model.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     6978 2021-06-09 14:15:06.000000 ibm_watson_machine_learning-1.0.99/ibmfl/model/sklearn_fl_model.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     9205 2021-06-09 14:15:06.000000 ibm_watson_machine_learning-1.0.99/ibmfl/model/sklearn_kmeans_fl_model.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    23149 2021-06-09 14:15:06.000000 ibm_watson_machine_learning-1.0.99/ibmfl/model/tensorflow_fl_model.py
+drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:08.000000 ibm_watson_machine_learning-1.0.99/ibmfl/model/v2/
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:06.000000 ibm_watson_machine_learning-1.0.99/ibmfl/model/v2/__init__.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    17981 2021-06-09 14:15:06.000000 ibm_watson_machine_learning-1.0.99/ibmfl/model/v2/xgb_fl_model.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    17463 2021-06-09 14:15:06.000000 ibm_watson_machine_learning-1.0.99/ibmfl/model/xgb_fl_model.py
+drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:08.000000 ibm_watson_machine_learning-1.0.99/ibmfl/party/
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:06.000000 ibm_watson_machine_learning-1.0.99/ibmfl/party/__init__.py
+drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:08.000000 ibm_watson_machine_learning-1.0.99/ibmfl/party/metrics/
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:06.000000 ibm_watson_machine_learning-1.0.99/ibmfl/party/metrics/__init__.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5955 2021-06-09 14:15:06.000000 ibm_watson_machine_learning-1.0.99/ibmfl/party/metrics/metrics_recorder.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    14886 2021-06-09 14:15:06.000000 ibm_watson_machine_learning-1.0.99/ibmfl/party/party.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    12625 2021-06-09 14:15:06.000000 ibm_watson_machine_learning-1.0.99/ibmfl/party/party_protocol_handler.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      533 2021-06-09 14:15:06.000000 ibm_watson_machine_learning-1.0.99/ibmfl/party/status_type.py
+drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:08.000000 ibm_watson_machine_learning-1.0.99/ibmfl/party/training/
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:06.000000 ibm_watson_machine_learning-1.0.99/ibmfl/party/training/__init__.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1342 2021-06-09 14:15:06.000000 ibm_watson_machine_learning-1.0.99/ibmfl/party/training/fedavg_local_training_handler.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    10626 2021-06-09 14:15:06.000000 ibm_watson_machine_learning-1.0.99/ibmfl/party/training/local_training_handler.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     1958 2021-06-09 14:15:06.000000 ibm_watson_machine_learning-1.0.99/ibmfl/party/training/pfnm_local_training_handler.py
+drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:08.000000 ibm_watson_machine_learning-1.0.99/ibmfl/party/training/v2/
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:06.000000 ibm_watson_machine_learning-1.0.99/ibmfl/party/training/v2/__init__.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    18950 2021-06-09 14:15:06.000000 ibm_watson_machine_learning-1.0.99/ibmfl/party/training/v2/xgboost_local_training_handler.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    18053 2021-06-09 14:15:06.000000 ibm_watson_machine_learning-1.0.99/ibmfl/party/training/xgboost_local_training_handler.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     2178 2021-06-09 14:15:06.000000 ibm_watson_machine_learning-1.0.99/ibmfl/party_env_validator.py
+drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:08.000000 ibm_watson_machine_learning-1.0.99/ibmfl/util/
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:06.000000 ibm_watson_machine_learning-1.0.99/ibmfl/util/__init__.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    19492 2021-06-09 14:15:06.000000 ibm_watson_machine_learning-1.0.99/ibmfl/util/config.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     7903 2021-06-09 14:15:06.000000 ibm_watson_machine_learning-1.0.99/ibmfl/util/fl_metrics.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     5534 2021-06-09 14:15:06.000000 ibm_watson_machine_learning-1.0.99/ibmfl/util/log_config.py
+drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:08.000000 ibm_watson_machine_learning-1.0.99/ibmfl/util/pfnm/
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:06.000000 ibm_watson_machine_learning-1.0.99/ibmfl/util/pfnm/__init__.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     9849 2021-06-09 14:15:06.000000 ibm_watson_machine_learning-1.0.99/ibmfl/util/pfnm/core.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)    12441 2021-06-09 14:15:06.000000 ibm_watson_machine_learning-1.0.99/ibmfl/util/pfnm/matching.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     3027 2021-06-09 14:15:06.000000 ibm_watson_machine_learning-1.0.99/ibmfl/util/pfnm/utils.py
+drwxr-xr-x   0 amadeusz.masny1@ibm.com   (501) staff       (20)        0 2021-06-09 14:15:08.000000 ibm_watson_machine_learning-1.0.99/ibmfl/util/xgboost/
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      291 2021-06-09 14:15:06.000000 ibm_watson_machine_learning-1.0.99/ibmfl/util/xgboost/__init__.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     4110 2021-06-09 14:15:06.000000 ibm_watson_machine_learning-1.0.99/ibmfl/util/xgboost/export.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     7769 2021-06-09 14:15:06.000000 ibm_watson_machine_learning-1.0.99/ibmfl/util/xgboost/hyperparams.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      777 2021-06-09 14:15:06.000000 ibm_watson_machine_learning-1.0.99/ibmfl/util/xgboost/utils.py
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)      228 2021-06-09 14:15:08.000000 ibm_watson_machine_learning-1.0.99/setup.cfg
+-rw-r--r--   0 amadeusz.masny1@ibm.com   (501) staff       (20)     2827 2021-06-08 13:02:33.000000 ibm_watson_machine_learning-1.0.99/setup.py
```

### Comparing `ibm_watson_machine_learning-1.0.96/PKG-INFO` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ibm_watson_machine_learning
-Version: 1.0.96
+Name: ibm-watson-machine-learning
+Version: 1.0.99
 Summary: IBM Watson Machine Learning API Client
 Home-page: http://ibm-wml-api-pyclient.mybluemix.net
 Author: IBM
 Author-email: svagaral@in.ibm.com, kaganesa@in.ibm.com, vbmithun@in.ibm.com, amadeusz.masny1@ibm.com
 License: BSD
 Description: ******************************************
         ## Welcome to `ibm-watson-machine-learning`
@@ -18,14 +18,15 @@
         
 Keywords: watson,machine learning,IBM,Bluemix,client,API,IBM Cloud
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `ibm_watson_machine_learning-1.0.96/README.md` & `ibm_watson_machine_learning-1.0.99/README.md`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/Set.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/Set.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/__init__.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/assets.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/assets.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import print_function
 import requests
+
+from ibm_watson_machine_learning.messages.messages import Messages
 from ibm_watson_machine_learning.utils import SPACES_DETAILS_TYPE, INSTANCE_DETAILS_TYPE, MEMBER_DETAILS_TYPE,DATA_ASSETS_DETAILS_TYPE, STR_TYPE, STR_TYPE_NAME, docstring_parameter, meta_props_str_conv, str_type_conv, get_file_from_cos
 from ibm_watson_machine_learning.metanames import AssetsMetaNames
 from ibm_watson_machine_learning.wml_resource import WMLResource
 from ibm_watson_machine_learning.wml_client_error import WMLClientError, ApiRequestFailure
 import os
 
 _DEFAULT_LIST_LENGTH = 50
@@ -192,15 +194,15 @@
         if desc is None:
             desc = ""
         if connection_id is None:
             f = {'file': open(file_path, 'rb')}
         try:
             import mimetypes
         except Exception as e:
-            raise WMLClientError(u'Module mimetypes not found.', e)
+            raise WMLClientError(Messages.get_message(message_id="module_mimetypes_not_found"), e)
         mime_type = mimetypes.MimeTypes().guess_type(file_path)[0]
         if mime_type is None:
             mime_type = "application/octet-stream"
 
         asset_meta = {
             "metadata": {
                 "name": name,
@@ -215,15 +217,15 @@
                 }
             }
         }
         if connection_id is not None:
             asset_meta["metadata"].update({"tags": ["connected-data"]})
 
         #Step1  : Create an asset
-        print("Creating data asset...")
+        print(Messages.get_message(message_id="creating_data_asset"))
 
         if self._client.WSD:
             # For WSD the asset creation is done within _wsd_create_asset function using polyglot
             # Thus using the same for data_assets type
             input_payload = {
                     "name": name,
                     "mime_type": mime_type
@@ -316,30 +318,30 @@
                                 complete_response = requests.post(
                                     self._client.service_instance._href_definitions.get_attachment_href(asset_id,attachment_id)+"/complete",
                                     headers=self._client._get_headers(),
                                     params=self._client._params(),
                                     verify=False
                                 )
                             if complete_response.status_code == 200:
-                                print("SUCCESS")
+                                print(Messages.get_message(message_id="success"))
                                 return self._get_required_element_from_response(asset_details)
                             else:
                                 self._delete(asset_id)
-                                raise WMLClientError("Failed while creating a data asset. Try again.")
+                                raise WMLClientError(Messages.get_message(message_id="failed_while_creating_a_data_asset"))
                         else:
                             self._delete(asset_id)
-                            raise WMLClientError("Failed while creating a data asset. Try again.")
+                            raise WMLClientError(Messages.get_message(message_id="failed_while_creating_a_data_asset"))
                     else:
-                        print("SUCCESS")
+                        print(Messages.get_message(message_id="success"))
                         return self._get_required_element_from_response(asset_details)
                 else:
                     self._delete(asset_id)
-                    raise WMLClientError("Failed while creating a data asset. Try again.")
+                    raise WMLClientError(Messages.get_message(message_id="failed_while_creating_a_data_asset"))
             else:
-                raise WMLClientError("Failed while creating a data asset. Try again.")
+                raise WMLClientError(Messages.get_message(message_id="failed_while_creating_a_data_asset"))
 
     def list(self, limit=None):
         """
            List stored data assets. If limit is set to None there will be only first 50 records shown.
 
            **Parameters**
 
@@ -423,24 +425,24 @@
             attachment_url = asset_details['attachments'][0]['object_key']
             artifact_content_url = self._client.service_instance._href_definitions.get_wsd_model_attachment_href() + \
                                    urllib.parse.quote('data_asset/' + attachment_url, safe='')
 
             r = requests.get(artifact_content_url, params=self._client._params(), headers=self._client._get_headers(),
                              stream=True, verify=False)
             if r.status_code != 200:
-                raise ApiRequestFailure(u'Failure during {}.'.format("downloading data asset"), r)
+                raise ApiRequestFailure(Messages.get_message(message_id="failure_during_downloading_data_asset"), r)
 
             downloaded_asset = r.content
             try:
                 with open(filename, 'wb') as f:
                     f.write(downloaded_asset)
-                print(u'Successfully saved data asset content to file: \'{}\''.format(filename))
+                print(Messages.get_message(filename, message_id="successfully_saved_data_asset_content_to_file"))
                 return os.getcwd() + "/" + filename
             except IOError as e:
-                raise WMLClientError(u'Saving data asset with artifact_url: \'{}\'  to local file failed.'.format(filename), e)
+                raise WMLClientError(Messages.get_message(filename, message_id="saving_data_asset_to_local_file_failed"), e)
         else:
             attachment_id = asset_details["attachments"][0]["id"]
             if not self._ICP and not self._client.WSD:
                 response = requests.get(self._client.service_instance._href_definitions.get_attachment_href(asset_uid,attachment_id), params=self._client._params(),
                                         headers=self._client._get_headers())
             else:
                 response = requests.get(self._client.service_instance._href_definitions.get_attachment_href(asset_uid,attachment_id), params=self._client._params(),
@@ -456,39 +458,38 @@
                         attachment_signed_url = response.json()["url"]
                         if not self._ICP:
                             att_response = requests.get(attachment_signed_url)
                         else:
                             att_response = requests.get(attachment_signed_url,
                                                         verify=False)
                     else:
-                        raise WMLClientError('Download API is not supported for Data Assets created using all connections. \
-                         It is supported only for Cloud storage data source type connections ')
+                        raise WMLClientError(Messages.get_message(message_id="download_api_not_supported_for_this_connection_type"))
                 else:
                     attachment_signed_url = response.json()["url"]
                     if not self._ICP and not self._client.WSD:
                         if self._client.CLOUD_PLATFORM_SPACES:
                             att_response = requests.get(attachment_signed_url)
                         else:
                             att_response = requests.get(self._wml_credentials["url"]+attachment_signed_url)
                     else:
                         att_response = requests.get(self._wml_credentials["url"]+attachment_signed_url,
                                                 verify=False)
                 if att_response.status_code != 200:
-                    raise ApiRequestFailure(u'Failure during {}.'.format("downloading asset"), att_response)
+                    raise ApiRequestFailure(Messages.get_message(message_id="failure_during_downloading_data_asset"), att_response)
 
                 downloaded_asset = att_response.content
                 try:
                     with open(filename, 'wb') as f:
                         f.write(downloaded_asset)
-                    print(u'Successfully saved data asset content to file: \'{}\''.format(filename))
+                    print(Messages.get_message(filename, message_id="successfully_saved_data_asset_content_to_file"))
                     return os.getcwd() + "/" + filename
                 except IOError as e:
-                    raise WMLClientError(u'Saving asset with artifact_url to local file: \'{}\' failed.'.format(filename), e)
+                    raise WMLClientError(Messages.get_message(filename, message_id="saving_data_asset_to_local_file_failed"), e)
             else:
-                raise WMLClientError("Failed while downloading the asset " + asset_uid)
+                raise WMLClientError(Messages.get_message(message_id="failure_during_downloading_data_asset"))
 
     @staticmethod
     @docstring_parameter({'str_type': STR_TYPE_NAME})
     def get_uid(asset_details):
         """
                 Get Unique Id  of stored data asset. Deprecated!! Use get_id(details) instead
 
@@ -700,8 +701,8 @@
                 if "attachments" in response_data and response_data[u'attachments']:
                     new_el[u'metadata'].update({'attachment_id': response_data[u'attachments'][0][u'id']})
             if self._client.CLOUD_PLATFORM_SPACES or self._client.ICP_PLATFORM_SPACES:
                 href_without_host = response_data['href'].split('.com')[-1]
                 new_el[u'metadata'].update({'href':href_without_host})
             return new_el
         except Exception as e:
-            raise WMLClientError("Failed to read Response from down-stream service: " + response_data)
+            raise WMLClientError(Messages.get_message(response_data, message_id="failed_to_read_response_from_down_stream_service"))
```

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/client.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/client.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import logging
+
+from ibm_watson_machine_learning.messages.messages import Messages
 from ibm_watson_machine_learning.utils import version
 
 #from ibm_watson_machine_learning.learning_system import LearningSystem
 from ibm_watson_machine_learning.experiments import Experiments
 from ibm_watson_machine_learning.repository import Repository
 from ibm_watson_machine_learning.model_definition import ModelDefinition
 from ibm_watson_machine_learning.models import Models
@@ -111,52 +113,59 @@
                                                    '2.0', '2.0.1', '2.0.2', '2.5.0',
                                                    '3.0.0', '3.0.1', '3.5', '4.0']
         self.__wsd_supported_version_list = ['1.0', '1.1', '2.0']
         self.__predefined_instance_type_list = ['icp', 'openshift', 'wml_local', 'wsd_local']
         os.environ['WSD_PLATFORM'] = 'False'
         if wml_credentials is None:
             raise NoWMLCredentialsProvided()
+        if 'url' not in self.wml_credentials:
+            raise WMLClientError(Messages.get_message(message_id="url_not_provided"))
+        if not self.wml_credentials['url'].startswith('https://'):
+            raise WMLClientError(Messages.get_message(message_id="invalid_url"))
         if self.wml_credentials['url'][-1] == "/":
             self.wml_credentials['url'] = self.wml_credentials['url'].rstrip('/')
 
         if 'instance_id' not in wml_credentials.keys():
             self.CLOUD_PLATFORM_SPACES = True
             self.wml_credentials[u'instance_id'] = 'invalid'  # This is applicable only via space instance_id
             self.ICP = False
             self.CAMS = False
 
             if wml_credentials[u'url'] in self.PLATFORM_URLS_MAP.keys():
                 self.PLATFORM_URL = self.PLATFORM_URLS_MAP[wml_credentials[u'url']]
                 self.CAMS_URL = self.PLATFORM_URLS_MAP[wml_credentials[u'url']]
             else:
-                raise WMLClientError("Provided 'url' is not valid")
+                raise WMLClientError(Messages.get_message(message_id="invalid_cloud_scenario_url"))
 
             if not self._is_IAM():
-                raise WMLClientError('apikey for IAM token is not provided in credentials for the client')
+                raise WMLClientError(Messages.get_message(message_id="apikey_not_provided"))
         else:
             if 'icp' == wml_credentials[u'instance_id'].lower() or 'openshift' == wml_credentials[
                 u'instance_id'].lower() or 'wml_local' == wml_credentials[u'instance_id'].lower():
                 self.ICP = True
                 os.environ["DEPLOYMENT_PLATFORM"] = "private"
                 ##Condition for CAMS related changes to take effect (Might change)
+                if 'version' not in wml_credentials:
+                    raise WMLClientError(Messages.get_message(self.__wml_local_supported_version_list, message_id="version_not_provided"))
+
                 if 'version' in wml_credentials.keys() and (
                         '2.0.1' == wml_credentials[u'version'].lower() or '2.5.0' == wml_credentials[
                     u'version'].lower() or
                         '3.0.0' == wml_credentials[u'version'].lower() or '3.0.1' == wml_credentials[
                             u'version'].lower() or '3.5' == wml_credentials[u'version'].lower() or
                         '4.0' == wml_credentials[u'version'].lower() or
                         '1.1' == wml_credentials[u'version'].lower() or '2.0' == wml_credentials[u'version'].lower()):
                     self.CAMS = True
                     os.environ["DEPLOYMENT_PRIVATE"] = "icp4d"
                     if 'wml_local' == wml_credentials[u'instance_id'].lower() and \
                             ('1.1' == wml_credentials[u'version'].lower() or '2.0' == wml_credentials[
                                 u'version'].lower()):
                         url_port = wml_credentials[u'url'].split(':')[-1]
                         if not url_port.isdigit():
-                            raise WMLClientError("It is mandatory to have port number as part of url for wml_local.")
+                            raise WMLClientError(Messages.get_message(message_id="no_port_number_for_wml_local"))
 
                     if '3.0.0' == wml_credentials[u'version'].lower() or \
                             '3.0.1' == wml_credentials[u'version'].lower() or \
                             '2.0' == wml_credentials[u'version'].lower():
                         self.ICP_30 = True
 
                     # For Cloud convergence related functionalities brought into CP4D 3.5
@@ -170,38 +179,39 @@
                         if 'bedrock_url' not in wml_credentials:
                             self.wml_credentials['bedrock_url'] = '.'.join(['https://cp-console'] + wml_credentials['url'].split('.')[1:])
                             self._is_bedrock_url_autogenerated = True
 
                 else:
                     if 'version' in wml_credentials.keys() and \
                             wml_credentials[u'version'].lower() not in self.__wml_local_supported_version_list:
-                        raise WMLClientError(
-                            "Invalid value for 'version' provided in wml_credentials. Please check the wml_credentials provided." +
-                            "Supported value for version field are: " + ', '.join(
-                                self.__wml_local_supported_version_list))
+                        raise WMLClientError(Messages.get_message(
+                            ', '.join(self.__wml_local_supported_version_list),
+                            message_id="invalid_version"))
 
                     self.CAMS = False
             else:
                 if ('wsd_local' == wml_credentials[u'instance_id'].lower()) and \
                         ('1.1' == wml_credentials[u'version'].lower() or '2.0' == wml_credentials[u'version'].lower()):
                     self.WSD = True
                     os.environ['WSD_PLATFORM'] = 'True'
                     if '2.0' == wml_credentials[u'version'].lower():
                         self.WSD_20 = True
                 else:
                     if ('wsd_local' == wml_credentials[u'instance_id'].lower()) and \
                             'version' in wml_credentials.keys() and \
                             wml_credentials[u'version'].lower() not in self.__wsd_supported_version_list:
-                        raise WMLClientError(
-                            "Invalid value for 'version' provided in wml_credentials. Please check the wml_credentials provided." +
-                            "Supported value for version field are: " + ', '.join(self.__wsd_supported_version_list))
+                        raise WMLClientError(Messages.get_message(
+                            ', '.join(self.__wsd_supported_version_list),
+                            message_id="invalid_version"))
 
                     if 'instance_id' in wml_credentials.keys():
-                        raise WMLClientError(
-                            "Provided credentials are invalid. 'instance_id' should not be used in cloud scenario. Please check the wml_credentials provided.")
+                        if wml_credentials['url'] in self.PLATFORM_URLS_MAP:
+                            raise WMLClientError(Messages.get_message(message_id="instance_id_in_cloud_scenario"))
+                        else:
+                            raise WMLClientError(Messages.get_message(message_id="invalid_instance_id"))
 
                     self.ICP = False
                     self.CAMS = False
 
                     self.service_instance = ServiceInstanceNewPlan(self)
 
                     headers = self._get_headers()
@@ -228,98 +238,77 @@
                                     not self.CREATED_IN_V1_PLAN and\
                                     response_get_instance.json()[u'entity'][u'plan']['name'] != 'lite':
                                 self.CLOUD_PLATFORM_SPACES = True
 
                                 # If v1 lite converted to v2 plan, tags : ["created_in_v1_plan"]
 
                                 if not self._is_IAM():
-                                    raise WMLClientError('apikey for IAM token is not provided in credentials for '
-                                                         'the client.')
+                                    raise WMLClientError(Messages.get_message(message_id="apikey_not_provided"))
 
                                 if wml_credentials[u'url'] in self.PLATFORM_URLS_MAP.keys():
                                     self.PLATFORM_URL = self.PLATFORM_URLS_MAP[wml_credentials[u'url']]
                                     self.CAMS_URL = self.PLATFORM_URLS_MAP[wml_credentials[u'url']]
                                 else:
-                                    raise WMLClientError("No 'url' provided")
+                                    raise WMLClientError(Messages.get_message(message_id="url_not_provided"))
 
                                 if self.CLOUD_PLATFORM_SPACES:
-                                    print("Note that if you are using any of v2 instance plans, then 'instance_id' is"
-                                          " not required to be provided here. It will be picked up from space when "
-                                          "client.set.default_space(space_id) is called ")
+                                    print(Messages.get_message(message_id="instance_id_is_not_required_for_v2_plans"))
 
                             if not self.CLOUD_PLATFORM_SPACES:
                                 self.CLOUD_BETA_FLOW = True
-                                print("NOTE!! DEPRECATED!! Creating assets using this flow(v4 beta) is deprecated"
-                                      " starting Sep 1st, 2020 and will be discontinued at the end of the migration period. "
-                                      "Refer to the documentation at 'https://dataplatform.cloud.ibm.com/docs/content/wsj/analyze-data/wml-ai.html' "
-                                      "for the migration process to be able to access new features")
+                                print(Messages.get_message(message_id="creating_assets_using_v4_beta_flow_is_deprecated"))
                     elif response_get_instance.status_code == 404:
-                        raise WMLClientError("instance_id not found. Note that if you are using "
-                                             "any of new instance plans [], then 'instance_id' is not required "
-                                             "to be provided here. It will be picked up from space when "
-                                             "client.set.default_space(space_id) is called ")
+                        raise WMLClientError(Messages.get_message(message_id="instance_id_not_found"))
                     elif response_get_instance.status_code == 401:
-                        raise WMLClientError("Not authorized to access the instance_id  Note that if you are using "
-                                             "any of new instance plans [], then 'instance_id' is not required "
-                                             "to be provided here. It will be picked up from space when "
-                                             "client.set.default_space(space_id) is called")
+                        raise WMLClientError(Messages.get_message(message_id="not_authorized_to_access_the_instance_id"))
                     else:
                         # if someone is using beta flow and using instance api key
                         response_get_instance_v1 = requests.get(
                             u'{}/v3/wml_instances/{}'.format(self.wml_credentials['url'],
                                                              self.wml_credentials['instance_id']),
                             headers=self._get_headers()
                         )
 
                         if response_get_instance_v1.status_code != 200:
-                            raise WMLClientError("Failed to get instance details. Note that if you are using "
-                                                 "any of new instance plans [], then 'instance_id' is not required "
-                                                 "to be provided here. It will be picked up from space when "
-                                                 "client.set.default_space(space_id) is called.\n  Error:" + response_get_instance.text)
+                            raise WMLClientError(Messages.get_message(
+                                response_get_instance.text,
+                                message_id="failed_to_get_instance_details"))
 
                         self.CLOUD_BETA_FLOW = True
-                        print("NOTE!! DEPRECATED!! Creating assets using this flow(v4 beta) is deprecated"
-                              " starting Sep 1st, 2020 and will be discontinued at the end of the migration period. "
-                              "Refer to the documentation at 'https://dataplatform.cloud.ibm.com/docs/content/wsj/analyze-data/wml-ai.html' "
-                              "for the migration process to be able to access new features")
+                        print(Messages.get_message(message_id="creating_assets_using_v4_beta_flow_is_deprecated"))
             if "token" in wml_credentials:
                 self.proceed = True
             else:
                 self.proceed = False
 
         if 'instance_id' in wml_credentials.keys() and \
                 (wml_credentials['instance_id'].lower() not in self.__predefined_instance_type_list) and \
                 'version' in wml_credentials.keys():
-            raise WMLClientError("Provided credentials are invalid. 'instance_id' and 'version' keys provided are not correct. Please check the wml_credentials provided."  )
+            raise WMLClientError(Messages.get_message(message_id="provided_credentials_are_invalid"))
 
         self.project_id = project_id
         self.wml_token = None
 
         if not self.CLOUD_PLATFORM_SPACES and not self.ICP_PLATFORM_SPACES and not self.CLOUD_BETA_FLOW:
-            raise WMLClientError("This client is not supported in this release. Refer to the documentation at "
-                                 "http://ibm-wml-api-pyclient.mybluemix.net to know what releases are supported")
+            raise WMLClientError(Messages.get_message(message_id="client_is_not_supported_in_this_release"))
 
         # if not self.ICP and not self.ICP_30 and not self.WSD:
         if not self.WSD and not self.CLOUD_PLATFORM_SPACES and not self.ICP_PLATFORM_SPACES:
             self.service_instance = ServiceInstance(self)
             self.service_instance.details = self.service_instance.get_details()
 
         if self.CLOUD_PLATFORM_SPACES or self.ICP_PLATFORM_SPACES:
             # For cloud, service_instance.details will be set during space creation( if instance is associated ) or
             # while patching a space with an instance
             import sys
             if (3 == sys.version_info.major) and (6 == sys.version_info.minor):
                 if self.CLOUD_PLATFORM_SPACES:
-                    print("DEPRECATED!! Python 3.6 framework is deprecated and will be removed on Apr 8th, 2021. "
-                          "It will be read-only mode starting Nov 20th, 2020. i.e you won't be able to create new assets using this client. "
-                          "Use Python 3.7 instead. For details, see https://dataplatform.cloud.ibm.com/docs/content/wsj/analyze-data/pm_service_supported_frameworks.html")
+                    print(Messages.get_message(message_id="python_3_6_framework_is_deprecated"))
                 elif self.ICP_PLATFORM_SPACES:
-                    print("DEPRECATED!! The Python 3.6 framework is deprecated and will be removed from a future release. "
-                    "We recommend you migrate your assets and use a Python 3.7 framework instead. "
-                    "For details, see https://www.ibm.com/support/knowledgecenter/SSQNUZ_current/wsj/analyze-data/pm_service_supported_frameworks.html")
+                    print(Messages.get_message(message_id="python_3_6_framework_is_deprecated_cp4d"))
 
             self.service_instance = ServiceInstanceNewPlan(self)
             self.volumes = Volume(self)
 
             if self.ICP_PLATFORM_SPACES:
                 self.service_instance.details = self.service_instance.get_details()
 
@@ -382,48 +371,47 @@
             self.runtimes = Runtimes(self)
             self.deployments = Deployments(self)
             self.training = Training(self)
             self.spaces = Spaces(self)
             self.connections = Connections(self)
             self.experiments = Experiments(self)
 
-        self._logger.info(u'Client successfully initialized')
+        self._logger.info(Messages.get_message(message_id="client_successfully_initialized"))
         self.version = version()
 
     def _check_if_either_is_set(self):
         if self.CAMS or self.CLOUD_PLATFORM_SPACES:
             if self.default_space_id is None and self.default_project_id is None:
-                raise WMLClientError("It is mandatory to set the space/project id. Use client.set.default_space(<SPACE_UID>)/client.set.default_project(<PROJECT_UID>) to proceed.")
+                raise WMLClientError(Messages.get_message(message_id="it_is_mandatory_to_set_the_space_project_id"))
 
     def _check_if_space_is_set(self):
         if self.CAMS or self.CLOUD_PLATFORM_SPACES:
             if self.default_space_id is None:
-                raise WMLClientError("It is mandatory to set the space. Use client.set.default_space(<SPACE_UID>) to proceed.")
+                raise WMLClientError(Messages.get_message(message_id="it_is_mandatory_to_set_the_space_id"))
 
     def _params(self, skip_space_project_chk=False, skip_for_create=False):
         params = {}
         if self.CAMS or self.CLOUD_PLATFORM_SPACES:
             if self.CLOUD_PLATFORM_SPACES or self.ICP_PLATFORM_SPACES:
                 params.update({'version': self.version_param})
             if not skip_for_create:
                 if self.default_space_id is not None:
                     params.update({'space_id': self.default_space_id})
                 elif self.default_project_id is not None:
                     params.update({'project_id': self.default_project_id})
                 else:
                     # For system software/hardware specs
                     if skip_space_project_chk is False:
-                        raise WMLClientError("It is mandatory to set the space/project id. Use client.set.default_space(<SPACE_UID>)/client.set.default_project(<PROJECT_UID>) to proceed.")
+                        raise WMLClientError(Messages.get_message(message_id="it_is_mandatory_to_set_the_space_project_id"))
 
         if self.WSD:
             if self.default_project_id is not None:
                 params.update({'project_id': self.default_project_id})
             else:
-                raise WMLClientError(
-                    "It is mandatory to set the project id. Use client.set.default_project(<PROJECT_UID>) to proceed.")
+                raise WMLClientError(Messages.get_message(message_id="it_is_mandatory_to_set_the_project_id"))
 
         if self.project_type == 'local_git_storage':
             params.update({'userfs': 'true'})
 
         if self.project_type != 'local_git_storage' and 'userfs' in params:
             del params['userfs']
 
@@ -478,15 +466,15 @@
         return False
 
     def _is_IAM(self):
         if('apikey' in self.wml_credentials.keys()):
             if (self.wml_credentials['apikey'] != ''):
                 return True
             else:
-                raise WMLClientError('apikey value cannot be \'\'. Pass a valid apikey for IAM token.')
+                raise WMLClientError(Messages.get_message(message_id="apikey_value_cannot_be_empty"))
         elif('token' in self.wml_credentials.keys()):
             if (self.wml_credentials['token'] != ''):
                 return True
             else:
-                raise WMLClientError('token value cannot be \'\'. Pass a valid token for IAM token.')
+                raise WMLClientError(Messages.get_message(message_id="token_value_cannot_be_empty"))
         else:
             return False
```

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/connections.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/connections.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import print_function
 import requests
+
+from ibm_watson_machine_learning.messages.messages import Messages
 from ibm_watson_machine_learning.utils import SPACES_DETAILS_TYPE, INSTANCE_DETAILS_TYPE, MEMBER_DETAILS_TYPE,DATA_ASSETS_DETAILS_TYPE, STR_TYPE, STR_TYPE_NAME, docstring_parameter, meta_props_str_conv, str_type_conv, get_file_from_cos
 from ibm_watson_machine_learning.metanames import ConnectionMetaNames
 from ibm_watson_machine_learning.wml_resource import WMLResource
 from ibm_watson_machine_learning.wml_client_error import WMLClientError, ApiRequestFailure
 import os
 import json
 
@@ -98,15 +100,15 @@
                             href_without_host = response_data['href'].split('.com')[-1]
                             new_el[u'metadata'].update({'href': href_without_host})
                         else:
                             new_el['metadata'].update({'href': response_data['href']})
 
             return new_el
         except Exception as e:
-            raise WMLClientError("Failed to read Response from down-stream service: " + response_data)
+            raise WMLClientError(Messages.get_message(response_data, message_id="failed_to_read_response_from_down_stream_service"))
 
     @docstring_parameter({'str_type': STR_TYPE_NAME})
     def get_details(self, connection_id=None):
         """
         Get connection details for the given unique Connection id. If no connection_id is passed, details for all connections will be returned.
 
         **Parameters**
@@ -263,15 +265,15 @@
             if 'private_key' in connection_meta[u'properties']:
                 result = json.dumps(connection_meta[u'properties'], separators=(',\n', ':'))
                 newmap = {"credentials": result}
                 connection_meta[u'properties'] = newmap
 
         connection_meta.update({'origin_country': 'US'})
         #Step1  : Create an asset
-        print("Creating connections...")
+        print(Messages.get_message(message_id="creating_connections"))
 
         if self._client.WSD:
             header_param = self._client._get_headers(wsdconnection_api_req=True)
         else:
             header_param = self._client._get_headers()
 
         if not self._client.ICP_30 and not self._client.ICP and not self._client.WSD:
@@ -288,18 +290,18 @@
                 json=connection_meta,
                 params=self._client._params(),
                 verify=False
             )
         connection_details = self._handle_response(201, u'creating new connection', creation_response)
         if creation_response.status_code == 201:
             connection_id = connection_details["metadata"]["asset_id"]
-            print("SUCCESS")
+            print(Messages.get_message(message_id="success"))
             return self._get_required_element_from_response(connection_details)
         else:
-            raise WMLClientError("Failed while creating a Connections. Try again.")
+            raise WMLClientError(Messages.get_message(message_id="failed_while_creating_connections"))
 
     @docstring_parameter({'str_type': STR_TYPE_NAME})
     def delete(self, connection_id):
         """
             Delete a stored Connection.
 
             **Parameters**
```

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/deployment/__init__.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/deployment/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/deployment/base_deployment.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/deployment/base_deployment.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/deployment/batch.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/deployment/batch.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import io
+import os
 import time
 from typing import TYPE_CHECKING, Any, Dict, Union, List, Optional
 
 from pandas import DataFrame, concat
 
 from .base_deployment import BaseDeployment
 from ..helpers import DataConnection, AssetLocation
@@ -476,15 +477,16 @@
                 conn._wml_client = self._target_workspace.wml_client
                 if len(scoring_params['input_data_references']) > 1 and not self._target_workspace.wml_client.ICP:
                     conn._obm = True
                     # TODO: remove S3 implementation
                     if conn.type == DataConnectionTypes.S3:
                         conn._obm_cos_path = scoring_params['output_data_reference']['location']['path']
 
-                    elif conn.type == DataConnectionTypes.CA and conn._check_if_connection_asset_is_s3():
+                    elif (conn.type == DataConnectionTypes.CA and
+                          (os.environ.get('USER_ACCESS_TOKEN') is None and conn._check_if_connection_asset_is_s3())):
                         conn._obm_cos_path = scoring_params['output_data_reference']['location']['path']
 
                 return conn.read() # if in future output may be excel file or with custom separator, here it should be recognized
         else:
             raise MissingScoringResults(scoring_job_id, reason="Scoring is not completed.")
 
     @BaseDeployment._project_to_space_to_project
```

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/deployment/web_service.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/deployment/web_service.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/deployments.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/deployments.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/experiment/__init__.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/experiment/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/experiment/autoai/__init__.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/experiment/autoai/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/experiment/autoai/autoai.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/experiment/autoai/autoai.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 
 import copy
 from typing import List, Union
 
 from ibm_watson_machine_learning.preprocessing import DataJoinGraph
 from ibm_watson_machine_learning.utils.autoai.enums import (
     TShirtSize, ClassificationAlgorithms, RegressionAlgorithms, ForecastingAlgorithms, PredictionType, Metrics,\
-    Transformers, DataConnectionTypes, PipelineTypes, PositiveLabelClass)
+    Transformers, DataConnectionTypes, PipelineTypes, PositiveLabelClass, ClassificationAlgorithmsCP4D,
+    RegressionAlgorithmsCP4D, ForecastingAlgorithmsCP4D)
 from ibm_watson_machine_learning.utils.autoai.errors import LocalInstanceButRemoteParameter, MissingPositiveLabel, \
     NonForecastPredictionColumnMissing, ForecastPredictionColumnsMissing, ForecastingCannotBeRunAsLocalScenario, \
     TSNotSupported, ParamOutOfRange
 from ibm_watson_machine_learning.utils.autoai.utils import check_dependencies_versions, \
     validate_additional_params_for_optimizer, validate_optimizer_enum_values
 from ibm_watson_machine_learning.workspace import WorkSpace
 from .engines import WMLEngine
@@ -64,25 +65,27 @@
     >>>              "instance_id": "...",
     >>>              "url": "https://us-south.ml.cloud.ibm.com"
     >>>            },
     >>>         project_id="...",
     >>>         space_id="...")
     """
     # note: initialization of AutoAI enums as class properties
+
+    # note: Enums with estimators can be overwritten  in _init based on environment type (CPD or Cloud)
     ClassificationAlgorithms = ClassificationAlgorithms
     RegressionAlgorithms = RegressionAlgorithms
     ForecastingAlgorithms = ForecastingAlgorithms
+    # end note
     TShirtSize = TShirtSize
     PredictionType = PredictionType
     Metrics = Metrics
     Transformers = Transformers
     DataConnectionTypes = DataConnectionTypes
     PipelineTypes = PipelineTypes
 
-
     def __init__(self,
                  wml_credentials: Union[dict, 'WorkSpace'] = None,
                  project_id: str = None,
                  space_id: str = None) -> None:
         # note: as workspace is not clear enough to understand, there is a possibility to use pure
         # wml credentials with project and space IDs, but in addition we
         # leave a possibility to use a previous WorkSpace implementation, it could be passed as a first argument
@@ -99,14 +102,16 @@
                                             space_id=space_id)
 
             self.project_id = self._workspace.project_id
             self.space_id = self._workspace.space_id
             self.runs = AutoPipelinesRuns(engine=WMLEngine(self._workspace))
             self.runs._workspace = self._workspace
 
+        self._init_estimator_enums()
+
         self._20_class_limit_removal_test = False
         # --- end note
 
     def runs(self, *, filter: str) -> Union['AutoPipelinesRuns', 'LocalAutoPipelinesRuns']:
         """
         Get the historical runs but with WML Pipeline name filter (for remote scenario).
         Get the historical runs but with experiment name filter (for local scenario).
@@ -159,14 +164,15 @@
                   data_join_graph: 'DataJoinGraph' = None,
                   csv_separator: Union[List[str], str] = ',',
                   excel_sheet: Union[str, int] = 0,
                   encoding: str = 'utf-8',
                   positive_label: str = None,
                   data_join_only: bool = False,
                   drop_duplicates: bool = True,
+                  # fairness_info: dict = None, #TODO: Uncomment to add fairness support
                   text_processing: bool = None,
                   word2vec_feature_number: int = None,
                   daub_give_priority_to_runtime: float = None,
                   **kwargs) -> Union['RemoteAutoPipelines', 'LocalAutoPipelines']:
         """
         Initialize an AutoAi optimizer.
 
@@ -282,14 +288,15 @@
         RemoteAutoPipelines or LocalAutoPipelines, depends on how you initialize the AutoAI object.
 
         Example
         -------
         >>> from ibm_watson_machine_learning.experiment import AutoAI
         >>> experiment = AutoAI(...)
         >>>
+        >>>
         >>> optimizer = experiment.optimizer(
         >>>        name="name of the optimizer.",
         >>>        prediction_type=AutoAI.PredictionType.BINARY,
         >>>        prediction_column="y",
         >>>        scoring=AutoAI.Metrics.ROC_AUC_SCORE,
         >>>        desc="Some description.",
         >>>        holdout_size=0.1,
@@ -305,14 +312,32 @@
         >>>        prediction_type=AutoAI.PredictionType.MULTICLASS,
         >>>        prediction_column="y",
         >>>        scoring=AutoAI.Metrics.ROC_AUC_SCORE,
         >>>        desc="Some description.",
         >>>    )
         """
 
+        # # TODO: Pass the fairness info description and example when adding fairness support and
+        #
+        # """
+        # fairness_info: dict, optional
+        #     Dictionary that  specifies metadata needed for measuring fairness. It contains two key values:
+        #     favorable_labels and protected_attributes. The favorable_labels attribute indicates that when the class
+        #     column contains one of the value from list, that is considered a positive outcome.
+        #     A protected attribute is a feature that partitions the population into groups whose outcome should have parity.
+        #     If passed fairness metric will be calculated.
+        # >>> fairness_info = {
+        # >>>        "protected_attributes": [
+        # >>>            {"feature": "Sex", "privileged_groups": ['female']},
+        # >>>             {"feature": "Age", "privileged_groups": [[20, 40], [60, 90]]}
+        # >>>        ],
+        # >>>        "favorable_labels": ["No Risk"]
+        # >>>    }
+        # """
+
         if prediction_type == PredictionType.FORECASTING and self._workspace.wml_client.ICP and \
                 (self._workspace.wml_client.wml_credentials['version'].startswith('2.5') or \
                         self._workspace.wml_client.wml_credentials['version'].startswith('3.0') or \
                         self._workspace.wml_client.wml_credentials['version'].startswith('3.5')):
             raise TSNotSupported()
 
         if prediction_type == PredictionType.FORECASTING:
@@ -336,15 +361,16 @@
 
         validate_optimizer_enum_values(
             prediction_type=prediction_type,
             daub_include_only_estimators=daub_include_only_estimators,
             include_only_estimators=include_only_estimators,
             cognito_transform_names=cognito_transform_names,
             scoring=scoring,
-            t_shirt_size=kwargs.get("t_shirt_size", TShirtSize.M)
+            t_shirt_size=kwargs.get("t_shirt_size", TShirtSize.M),
+            is_cpd=self._workspace.wml_client.ICP
         )
 
         if daub_give_priority_to_runtime is not None:
             if daub_give_priority_to_runtime < 0.0 or daub_give_priority_to_runtime > 5.0:
                 raise ParamOutOfRange('daub_give_priority_to_runtime', daub_give_priority_to_runtime, 0.0, 5.0)
 
         if data_join_graph:
@@ -434,11 +460,22 @@
                 positive_label=positive_label,
                 data_join_only=data_join_only,
                 engine=engine,
                 daub_give_priority_to_runtime=daub_give_priority_to_runtime,
                 notebooks=kwargs.get('notebooks', True),
                 autoai_pod_version=kwargs.get('autoai_pod_version', None),
                 obm_pod_version=kwargs.get('obm_pod_version', None),
+                # fairness_info=fairness_info, #TODO: Uncomment to add fairness support
                 **reduced_kwargs
             )
             optimizer._workspace = self._workspace
             return optimizer
+
+    def _init_estimator_enums(self):
+        if self._workspace and self._workspace.wml_client.ICP:
+            self.ClassificationAlgorithms = ClassificationAlgorithmsCP4D
+            self.RegressionAlgorithms = RegressionAlgorithmsCP4D
+            self.ForecastingAlgorithms = ForecastingAlgorithmsCP4D
+        else:
+            self.ClassificationAlgorithms = ClassificationAlgorithms
+            self.RegressionAlgorithms = RegressionAlgorithms
+            self.ForecastingAlgorithms = ForecastingAlgorithms
```

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/experiment/autoai/engines/__init__.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/experiment/autoai/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/experiment/autoai/engines/base_engine.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/experiment/autoai/engines/base_engine.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/experiment/autoai/engines/wml_engine.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/experiment/autoai/engines/wml_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import TYPE_CHECKING, List, Dict, Tuple
 
 from pandas import DataFrame, MultiIndex
 import json
+import os
 from time import sleep
 import warnings
 import logging
 
 from lomond import WebSocket
 from ibm_watson_machine_learning.utils.autoai.enums import (
     PredictionType, RegressionAlgorithms, ClassificationAlgorithms, RunStateTypes)
@@ -128,14 +129,21 @@
                 self._wml_pipeline_metadata[self._wml_client.pipelines.ConfigurationMetaNames.DOCUMENT][
                     'pipelines'][0]['nodes'][0]['parameters']['optimization'][
                     'text_processing_options'] = {'word2vec':
                                                 {'output_dim': self._auto_pipelines_parameters.get('word2vec_feature_number')}}
 
         # end of section
 
+        # pass fairness info if not CPD
+        if not self._wml_client.ICP:
+            if self._auto_pipelines_parameters.get('fairness_info') is not None:
+                self._wml_pipeline_metadata[self._wml_client.pipelines.ConfigurationMetaNames.DOCUMENT][
+                    'pipelines'][0]['nodes'][0]['parameters']['optimization'][
+                    'fairness_info'] = self._auto_pipelines_parameters.get('fairness_info')
+        # end of section
 
         if self._auto_pipelines_parameters.get('prediction_type') == PredictionType.FORECASTING:
             self._wml_pipeline_metadata[self._wml_client.pipelines.ConfigurationMetaNames.DOCUMENT][
                 'pipelines'][0]['nodes'][0]['parameters']['optimization'][
                 'target_columns'] = self._auto_pipelines_parameters['prediction_columns']
             self._wml_pipeline_metadata[self._wml_client.pipelines.ConfigurationMetaNames.DOCUMENT][
                 'pipelines'][0]['nodes'][0]['parameters']['optimization'][
@@ -808,15 +816,16 @@
         # end note
 
         run_params = self._wml_client.training.get_details(training_uid=self._current_run_id)
 
         # note: recreation of s3 creds from connection asset
         results_reference = DataConnection._from_dict(run_params['entity']['results_reference'])
         results_reference._wml_client = self._wml_client
-        results_reference._check_if_connection_asset_is_s3()
+        if os.environ.get('USER_ACCESS_TOKEN') is None:
+            results_reference._check_if_connection_asset_is_s3()
         run_params['entity']['results_reference'] = results_reference._to_dict()
         # --- end note
 
         if 'timeseries' in run_params['entity']['status']['metrics'][0]['context']:
             raise ForecastingUnsupportedOperation()
 
         try:
```

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/experiment/autoai/optimizers/__init__.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/experiment/autoai/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/experiment/autoai/optimizers/base_auto_pipelines.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/experiment/autoai/optimizers/base_auto_pipelines.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/experiment/autoai/optimizers/local_auto_pipelines.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/experiment/autoai/optimizers/local_auto_pipelines.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/experiment/autoai/optimizers/remote_auto_pipelines.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/experiment/autoai/optimizers/remote_auto_pipelines.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,14 +142,15 @@
                  drop_duplicates: bool = True,
                  text_processing: bool = True,
                  word2vec_feature_number: int = None,
                  daub_give_priority_to_runtime: float = None,
                  notebooks=False,
                  autoai_pod_version=None,
                  obm_pod_version=None,
+                 # fairness_info=None,  TODO: uncomment to add fairness info
                  **kwargs):
         self.params = {
             'name': name,
             'desc': desc if desc else '',
             'prediction_type': prediction_type if prediction_type != 'timeseries' else 'forecasting',
             'prediction_column': prediction_column,
             'prediction_columns': prediction_columns,
@@ -171,14 +172,15 @@
             'encoding': encoding,
             'positive_label': positive_label,
             'data_join_only': data_join_only,
             'drop_duplicates': drop_duplicates,
             'notebooks': notebooks,
             'autoai_pod_version': autoai_pod_version,
             'obm_pod_version': obm_pod_version,
+            # 'fairness_info': fairness_info, TODO: uncomment to add fairness info
             'text_processing': text_processing,
             'word2vec_feature_number': word2vec_feature_number,
             'daub_give_priority_to_runtime': daub_give_priority_to_runtime
         }
         self._engine: 'WMLEngine' = engine
         self._engine.initiate_remote_resources(params=self.params, **kwargs)
         self.best_pipeline = None
```

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/experiment/autoai/runs/__init__.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/experiment/autoai/runs/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/experiment/autoai/runs/auto_pipelines_runs.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/experiment/autoai/runs/auto_pipelines_runs.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/experiment/autoai/runs/base_auto_pipelines_runs.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/experiment/autoai/runs/base_auto_pipelines_runs.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/experiment/autoai/runs/local_auto_pipelines_runs.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/experiment/autoai/runs/local_auto_pipelines_runs.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/experiment/base_experiment/__init__.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/experiment/base_experiment/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/experiment/base_experiment/base_experiment.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/experiment/base_experiment/base_experiment.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/experiments.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/experiments.py`

 * *Files 0% similar despite different names*

```diff
@@ -460,15 +460,15 @@
          """
         self._client._check_if_either_is_set()
         model_uid = str_type_conv(experiment_uid)
         Experiments._validate_type(experiment_uid, u'experiment_uid', STR_TYPE, True)
         Experiments._validate_type(rev_uid, u'rev_uid', int, True)
         if not self._client.ICP_30 and not self._client.CLOUD_PLATFORM_SPACES and not self._client.ICP_PLATFORM_SPACES:
             raise WMLClientError(
-                'Not supported. Revisions APIs are supported only for IBM Cloud Pak® for Data for Data 3.0 and above.')
+                'Not supported. Revisions APIs are supported only for IBM Cloud Pak® for Data 3.0 and above.')
         else:
             url = self._client.service_instance._href_definitions.get_experiment_href(experiment_uid)
             return self._get_with_or_without_limit(url, limit=None, op_name="experiments",
                                                    summary=None, pre_defined=None, revision=rev_uid)
 
     @docstring_parameter({'str_type': STR_TYPE_NAME})
     def list_revisions(self, experiment_uid, limit=None):
```

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/export_assets.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/export_assets.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/functions.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/functions.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/helpers/__init__.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/helpers/connections/__init__.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/helpers/connections/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/helpers/connections/base_connection.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/helpers/connections/base_connection.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/helpers/connections/base_data_connection.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/helpers/connections/base_data_connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 __all__ = [
     "BaseDataConnection"
 ]
 
 import io
 import json
+import os
 
 from abc import ABC, abstractmethod
 from typing import Union, Tuple, TYPE_CHECKING
 from warnings import warn
 
 import requests
 from pandas import concat, DataFrame
@@ -154,15 +155,15 @@
                     raise ApiRequestFailure(u'Failure during {}.'.format("downloading json"), file_response)
 
                 downloaded_asset = file_response.content
                 buffer = io.BytesIO(downloaded_asset)
                 json_content = json.loads(buffer.getvalue().decode('utf-8'))
 
         elif self.type == DataConnectionTypes.CA:
-            if self._check_if_connection_asset_is_s3():
+            if os.environ.get('USER_ACCESS_TOKEN') is None and self._check_if_connection_asset_is_s3():
                 cos_client = self._init_cos_client()
 
                 try:
                     file = cos_client.Object(self.location.bucket, path).get()
                     content = file["Body"].read()
                     json_content = json.loads(content.decode('utf-8'))
```

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/helpers/connections/base_location.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/helpers/connections/base_location.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/helpers/connections/connections.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/helpers/connections/connections.py`

 * *Files 1% similar despite different names*

```diff
@@ -342,15 +342,16 @@
 
         return data_connection
 
     def read(self,
              with_holdout_split: bool = False,
              csv_separator: str = ',',
              excel_sheet: Union[str, int] = 0,
-             encoding: Optional[str] = 'utf-8') -> Union['DataFrame', Tuple['DataFrame', 'DataFrame']]:
+             encoding: Optional[str] = 'utf-8',
+             **kwargs) -> Union['DataFrame', Tuple['DataFrame', 'DataFrame']]:
         """
         Download dataset stored in remote data storage.
 
         Parameters
         ----------
         with_holdout_split: bool, optional
             If True, data will be split to train and holdout dataset as it was by AutoAI.
@@ -422,15 +423,15 @@
 
         elif self.type == DataConnectionTypes.DS:
 
             if self._obm:
                 raise NotImplementedError("Multiple files for CP4D / WML Server is not yet supported.")
 
             try:
-                if self._check_if_connection_asset_is_s3():
+                if os.environ.get('USER_ACCESS_TOKEN') is None and self._check_if_connection_asset_is_s3():
                     cos_client = self._init_cos_client()
                     data = self._download_data_from_cos(cos_client=cos_client)
                 else:
                     data = self._download_training_data_from_data_asset_storage()
 
             except NotImplementedError as e:
                 raise e
@@ -444,28 +445,29 @@
 
                 try_import_pyarrow()
 
                 flight_service = FlightService(
                     wml_client=self._wml_client,
                     params=self.auto_pipeline_params,
                     data_location=data_location,
+                    experiment_metadata=kwargs.get('experiment_metadata')
                 )
 
                 data = flight_service.read()
 
         elif self.type == DataConnectionTypes.FS:
 
             if self._obm:
                 data = self._download_obm_data_from_file_system()
             else:
                 data = self._download_training_data_from_file_system()
 
         elif self.type == DataConnectionTypes.CA:
 
-            if self._check_if_connection_asset_is_s3():
+            if os.environ.get('USER_ACCESS_TOKEN') is None and self._check_if_connection_asset_is_s3():
                 cos_client = self._init_cos_client()
 
                 try:
                     if self._obm:
                         data = self._download_obm_data_from_cos(cos_client=cos_client)
 
                     else:
@@ -483,14 +485,15 @@
 
                     flight_service = FlightService(
                         wml_client=self._wml_client,
                         params=self.auto_pipeline_params,
                         data_location={'location': self.location.to_dict(),
                                        'type': self.type,
                                        "connection": self.connection.to_dict()},
+                        experiment_metadata=kwargs.get('experiment_metadata')
                     )
 
                     data = flight_service.read()
 
         if isinstance(data, DataFrame) and 'Unnamed: 0' in data.columns.tolist():
             data.drop(['Unnamed: 0'], axis=1, inplace=True)
 
@@ -535,15 +538,15 @@
             data_holdout[self.auto_pipeline_params['prediction_column']] = y_holdout
 
             return data_train, data_holdout
         # --- end note
 
         return data
 
-    def write(self, data: Union[str, 'DataFrame'], remote_name: str = None) -> None:
+    def write(self, data: Union[str, 'DataFrame'], remote_name: str = None, **kwargs) -> None:
         """
         Upload file to a remote data storage.
 
         Parameters
         ----------
         data: str, required
             Local path to the dataset or pandas.DataFrame with data.
@@ -573,15 +576,15 @@
                     cos_resource_client.Object(self.location.bucket, remote_name).upload_fileobj(
                         Fileobj=io.BytesIO(bytes(f.read().encode())))
 
             else:
                 raise TypeError("data should be either of type \"str\" or \"pandas.DataFrame\"")
 
         elif self.type == DataConnectionTypes.CA:
-            if self._check_if_connection_asset_is_s3():
+            if os.environ.get('USER_ACCESS_TOKEN') is None and self._check_if_connection_asset_is_s3():
                 cos_resource_client = self._init_cos_client()
                 if isinstance(data, str):
                     with open(data, "rb") as file_data:
                         cos_resource_client.Object(self.location.bucket, remote_name).upload_fileobj(
                             Fileobj=file_data)
 
                 elif isinstance(data, DataFrame):
@@ -602,14 +605,15 @@
 
                 flight_service = FlightService(
                     wml_client=self._wml_client,
                     params=self.auto_pipeline_params,
                     data_location={'location': self.location.to_dict(),
                                    'type': self.type,
                                    "connection": self.connection.to_dict()},
+                    experiment_metadata=kwargs.get('experiment_metadata')
                 )
 
                 if isinstance(data, str):
                     raise TypeError(f"'data' should be of pandas.DataFrame type if "
                                     f"you want to store it with connection asset.")
 
                 elif isinstance(data, DataFrame):
```

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/helpers/flight/errors.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/helpers/flight/errors.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/helpers/flight/service.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/helpers/flight/service.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,19 +51,21 @@
 
     """
 
     def __init__(self,
                  wml_client: 'APIClient',
                  params: dict,
                  n_batches: Optional[int] = 1,
-                 data_location: dict = None,) -> None:
+                 data_location: dict = None,
+                 experiment_metadata: dict = None) -> None:
         self.wml_client = wml_client
         self.params = params
         self.n_batches = n_batches
         self.data_source_type = None
+        self.experiment_metadata = experiment_metadata
 
         self.data_location = data_location
 
         self.lock_read = threading.Lock()
         self.stop_reading = False
 
         from pyarrow import flight
@@ -305,15 +307,20 @@
         # when dataset is small we received empty dfs, it is ok (15 is optimum for larger than 1 GB)
         command = {
             "num_partitions": 15,
         }
 
         # note: WS scenario
         if self.wml_client is None:
-            command['project_id'] = os.environ.get('PROJECT_ID')
+            project_id = os.environ.get('PROJECT_ID')
+            if project_id is None:
+                command['project_id'] = self.experiment_metadata.get('project_id')
+
+            else:
+                command['project_id'] = project_id
 
         else:
             if self.wml_client.default_space_id is not None:
                 command['space_id'] = self.wml_client.default_space_id
 
             elif self.wml_client.default_project_id is not None:
                 command['project_id'] = self.wml_client.default_project_id
```

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/helpers/flight/utils.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/helpers/flight/utils.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/helpers/helpers.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/hpo.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/hpo.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/href_definitions.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/href_definitions.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/hw_spec.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/hw_spec.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/import_assets.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/import_assets.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
         self._client = client
 
     @docstring_parameter({'str_type': STR_TYPE_NAME})
     def start(self, file_path=None, space_id=None, project_id=None):
         """
             Start the import. Either space_id or project_id has to be provided and is mandatory. Note that
-            on IBM Cloud Pak® for Data for Data 3.5, import into non-empty space/project is not supported
+            on IBM Cloud Pak® for Data 3.5, import into non-empty space/project is not supported
 
            **Parameters**
 
            .. important::
                 #. **meta_props**:  meta data. To see available meta names use **client.import_assets.ConfigurationMetaNames.get()**\n
                    **type**: dict\n
                 #. **space_id**:  Space identifier**\n
```

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/instance.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/instance.py`

 * *Files 0% similar despite different names*

```diff
@@ -267,15 +267,15 @@
             data=mystr,
             headers=headers
         )
 
         if response.status_code == 200:
             token = response.json().get(u'access_token')
         else:
-            raise ApiRequestFailure(u'Error during getting IAM Token.', response)
+            raise ApiRequestFailure(u'Error getting IAM Token.', response)
         return token
 
     def _create_zen_token(self):
         token_url = self._wml_credentials['url'] + '/icp4d-api/v1/authorize'
         headers = {
             'Content-type' :'application/json',
             'cache-control': 'no-cache'
```

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/instance_new_plan.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/instance_new_plan.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,14 @@
     """
 
     def __init__(self, client):
         self._logger = logging.getLogger(__name__)
         self._client = client
         self._wml_credentials = client.wml_credentials
         self._expiration_datetime = None
-        self._is_iam_token = None
 
         if self._client.ICP_PLATFORM_SPACES:
             if self.get_instance_id() == 'openshift' or self.get_instance_id() == 'wml_local':
                 self._wml_credentials[u'url'] = self.get_url()
             else:
                 self._wml_credentials[u'url'] = self.get_url() + ':31843'
             # TODO: Check if this is used anywhere.. from initial searches, doesn't seem like
@@ -116,15 +115,18 @@
                 **return type**: str
 
              **Example**
 
              >>> instance_details = client.service_instance.get_username()
         """
         if self._client.ICP_PLATFORM_SPACES:
-            return self._wml_credentials['username']
+            try:
+                return self._wml_credentials['username']
+            except:
+                raise WMLClientError('`username` missing in wml_credentials.')
         else:
             raise WMLClientError("Not applicable for Cloud")
 
     def get_password(self):
         """
              Get password for your Watson Machine Learning service. Applicable only for IBM Cloud Pak® for Data
 
@@ -136,15 +138,18 @@
                 **return type**: str
 
              **Example**
 
              >>> instance_details = client.service_instance.get_password()
         """
         if self._client.ICP_PLATFORM_SPACES:
-            return self._wml_credentials['password']
+            try:
+                return self._wml_credentials['password']
+            except:
+                raise WMLClientError('`password` missing in wml_credentials.')
         else:
             raise WMLClientError("Not applicable for Cloud")
 
     def get_details(self):
         """
              Get information about your Watson Machine Learning instance.
 
@@ -244,23 +249,23 @@
         token_padded = token_parts[1] + '=' * (len(token_parts[1]) % 4)
         token_info = json.loads(base64.b64decode(token_padded).decode('utf-8'))
         token_expire = token_info.get('exp')
 
         return datetime.fromtimestamp(token_expire)
 
     def _is_iam(self):
-        if self._is_iam_token is not None:
-            return self._is_iam_token
-
-        token_parts = self._client.wml_token.split('.')
-        token_padded = token_parts[1] + '=' * (len(token_parts[1]) % 4)
-        token_info = json.loads(base64.b64decode(token_padded).decode('utf-8'))
-        instanceId = token_info.get('instanceId')
-
-        return instanceId
+        try:
+            token_parts = self._client.wml_token.split('.')
+            token_padded = token_parts[1] + '=' * (len(token_parts[1]) % 4)
+            token_info = json.loads(base64.b64decode(token_padded).decode('utf-8'))
+            instanceId = token_info.get('instanceId')
+
+            return instanceId
+        except:
+            return False
 
     def _get_IAM_token(self):
         if self._client.proceed is True:
             return self._wml_credentials["token"]
         headers = {
             'Content-Type': 'application/x-www-form-urlencoded',
             'Authorization': 'Basic Yng6Yng='
@@ -272,17 +277,16 @@
             data=mystr,
             headers=headers
         )
 
         if response.status_code == 200:
             token = response.json().get(u'access_token')
             self._expiration_datetime = None
-            self._is_iam_token = None
         else:
-            raise WMLClientError(u'Error during getting IAM Token.', response)
+            raise WMLClientError(u'Error getting IAM Token.', response)
         return token
 
     def _is_token_refresh_possible(self):
         """
         Checks if necessary credentials were passed for token refresh.
         For CP4D we need (username & password)/(username & api_key).
         For Cloud we need api_key.
@@ -331,48 +335,46 @@
                                      'Content-Type': 'application/json'
                                  },
                                  data=self._get_cpd_auth_pair(),
                                  verify=False)
 
         if response.status_code == 200:
             self._expiration_datetime = None
-            self._is_iam_token = None
             return response.json().get(u'token')
         else:
-            raise WMLClientError(u'Error during refreshing the token.', response)
+            raise WMLClientError(u'Error refreshing the token.', response)
 
     def _get_cpd_token_from_request_new_auth_flow(self):
         bedrock_url = self._href_definitions.get_cpd_bedrock_token_endpoint_href()
         response = requests.post(bedrock_url,
                                  headers={
                                      'Content-Type': 'application/x-www-form-urlencoded;charset=UTF-8'
                                  },
                                  data=self._get_cpd_bedrock_auth_data(),
                                  verify=False)
 
         if response.status_code != 200:
-            raise WMLClientError(u'Error during refreshing the token.', response, logg_messages=False)
+            raise WMLClientError(u'Error refreshing the token.', response, logg_messages=False)
 
         iam_token = response.json()['access_token']
         self._expiration_datetime = datetime.now() + timedelta(seconds=response.json()['expires_in'])
-        self._is_iam_token = True
         # refresh_token = response.json()['refresh_token']
 
         token_url = self._href_definitions.get_cpd_validation_token_endpoint_href()
         response = requests.get(token_url,
                                 headers={
                                     'username': 'admin',
                                     'iam-token': iam_token
                                 },
                                 verify=False)
 
         if response.status_code == 200:
             return response.json()['accessToken']
         else:
-            raise WMLClientError(u'Error during refreshing the token.', response)
+            raise WMLClientError(u'Error refreshing the token.', response)
 
     def _get_cpd_token_from_request(self):
         """
         Send a request for token on CPD.
 
         **Output**
             **returns**: Newly created token if returned if no errors occurred.\n
```

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/learning_system.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/learning_system.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/__init__.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/mlpipelinepy/__init__.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/mlpipelinepy/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/mlpipelinepy/edge.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/mlpipelinepy/edge.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/mlpipelinepy/exception.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/mlpipelinepy/exception.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/mlpipelinepy/javaproxy.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/mlpipelinepy/javaproxy.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/mlpipelinepy/mlpipeline.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/mlpipelinepy/mlpipeline.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/mlpipelinepy/serialization.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/mlpipelinepy/serialization.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/mlpipelinepy/utils.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/mlpipelinepy/utils.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/mlpipelinepy/version.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/mlpipelinepy/version.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/pipeline/DAG.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/pipeline/DAG.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/pipeline/IBMSparkPipeline.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/pipeline/IBMSparkPipeline.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/pipeline/IBMSparkPipelineModel.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/pipeline/IBMSparkPipelineModel.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/pipeline/Result.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/pipeline/Result.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/pipeline/Sink.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/pipeline/Sink.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/pipeline/Source.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/pipeline/Source.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/pipeline/Wrapper.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/pipeline/Wrapper.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/pipeline/__init__.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/TestRepoSaveLoad.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/TestRepoSaveLoad.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/__init__.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/base_constants.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/base_constants.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/ml_api_client.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/ml_api_client.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/ml_authorization.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/ml_authorization.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepository/__init__.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepository/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepository/artifact.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepository/artifact.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepository/artifact_reader.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepository/artifact_reader.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepository/generic_archive_model_artifact.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepository/generic_archive_model_artifact.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepository/generic_archive_pipeline_artifact.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepository/generic_archive_pipeline_artifact.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepository/hybrid_model_artifact.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepository/hybrid_model_artifact.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepository/meta_names.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepository/meta_names.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepository/meta_props.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepository/meta_props.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepository/model_artifact.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepository/model_artifact.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepository/pipeline_artifact.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepository/pipeline_artifact.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepository/scikit_model_artifact.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepository/scikit_model_artifact.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepository/tensorflow_model_artifact.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepository/tensorflow_model_artifact.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepository/wml_experiment_artifact.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepository/wml_experiment_artifact.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepository/wml_function_artifact.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepository/wml_function_artifact.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepository/wml_libraries_artifact.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepository/wml_libraries_artifact.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepository/wml_runtimes_artifact.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepository/wml_runtimes_artifact.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepository/xgboost_model_artifact.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepository/xgboost_model_artifact.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/__init__.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/content_loaders.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/content_loaders.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/experiment_artifact.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/experiment_artifact.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/function_artifact.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/function_artifact.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/function_artifact_loader.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/function_artifact_loader.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/function_artifact_reader.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/function_artifact_reader.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/function_loader.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/function_loader.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/generic_archive_pipeline_model_artifact.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/generic_archive_pipeline_model_artifact.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/generic_file_artifact_loader.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/generic_file_artifact_loader.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/generic_file_pipeline_model_loader.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/generic_file_pipeline_model_loader.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/generic_file_reader.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/generic_file_reader.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/hybrid_artifact_loader.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/hybrid_artifact_loader.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/hybrid_pipeline_model_artifact.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/hybrid_pipeline_model_artifact.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/hybrid_pipeline_model_loader.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/hybrid_pipeline_model_loader.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/hybrid_pipeline_model_reader.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/hybrid_pipeline_model_reader.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/libraries_artifact.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/libraries_artifact.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/libraries_artifact_loader.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/libraries_artifact_loader.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/libraries_artifact_reader.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/libraries_artifact_reader.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/libraries_loader.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/libraries_loader.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/ml_repository_artifact.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/ml_repository_artifact.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/python_version.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/python_version.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/runtimes_artifact.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/runtimes_artifact.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/runtimes_artifact_loader.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/runtimes_artifact_loader.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/runtimes_artifact_reader.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/runtimes_artifact_reader.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/scikit_artifact_loader.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/scikit_artifact_loader.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/scikit_pipeline_model_artifact.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/scikit_pipeline_model_artifact.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/scikit_pipeline_model_loader.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/scikit_pipeline_model_loader.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/scikit_pipeline_reader.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/scikit_pipeline_reader.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/spark_artifact_loader.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/spark_artifact_loader.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/spark_pipeline_artifact.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/spark_pipeline_artifact.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/spark_pipeline_loader.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/spark_pipeline_loader.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/spark_pipeline_model_artifact.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/spark_pipeline_model_artifact.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/spark_pipeline_model_loader.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/spark_pipeline_model_loader.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/spark_pipeline_reader.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/spark_pipeline_reader.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/spark_version.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/spark_version.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/tensorflow_artifact_loader.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/tensorflow_artifact_loader.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/tensorflow_pipeline_model_artifact.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/tensorflow_pipeline_model_artifact.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/tensorflow_pipeline_model_loader.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/tensorflow_pipeline_model_loader.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/tensorflow_pipeline_reader.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/tensorflow_pipeline_reader.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/version_helper.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/version_helper.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/xgboost_model_reader.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryartifact/xgboost_model_reader.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/__init__.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/content_reader.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/content_reader.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/experiment_adapter.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/experiment_adapter.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/experiment_collection.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/experiment_collection.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/function_adapter.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/function_adapter.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/function_collection.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/function_collection.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/libraries_adapter.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/libraries_adapter.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/libraries_collection.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/libraries_collection.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/ml_repository_api.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/ml_repository_api.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/ml_repository_client.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/ml_repository_client.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/model_adapter.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/model_adapter.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/model_collection.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/model_collection.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/runtimes_adapter.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/runtimes_adapter.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/runtimes_collection.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/runtimes_collection.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/wml_experiment_adapter.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/wml_experiment_adapter.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/wml_experiment_collection.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/mlrepositoryclient/wml_experiment_collection.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/__init__.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/api_client.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/api_client.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/apis/__init__.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/apis/repository_api.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/apis/repository_api.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/apis/token_api.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/apis/token_api.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/configuration.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/configuration.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/__init__.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/array_data_input_repository.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/array_data_input_repository.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/array_model_metrics_output.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/array_model_metrics_output.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/array_model_output.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/array_model_output.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/array_model_version_metrics_experiments.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/array_model_version_metrics_experiments.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/array_model_version_output.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/array_model_version_output.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/array_pipeline_output.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/array_pipeline_output.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/array_pipeline_version_output.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/array_pipeline_version_output.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/array_training_output_experiments.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/array_training_output_experiments.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/artifact_author.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/artifact_author.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/artifact_version_metadata.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/artifact_version_metadata.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/artifact_version_repository.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/artifact_version_repository.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/artifact_version_short_metadata.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/artifact_version_short_metadata.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/author_experiments.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/author_experiments.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/author_repository.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/author_repository.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/batch_deploy_output.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/batch_deploy_output.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/batch_deploy_output_entity.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/batch_deploy_output_entity.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/batch_deploy_output_entity_execution.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/batch_deploy_output_entity_execution.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/batch_deploy_output_meta.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/batch_deploy_output_meta.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/batch_input.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/batch_input.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/batch_output.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/batch_output.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/batch_output_array.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/batch_output_array.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/cols_output.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/cols_output.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/compute_configuration_experiments.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/compute_configuration_experiments.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/connection.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/connection.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/connection_object_source_experiments.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/connection_object_source_experiments.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/connection_object_target_experiments.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/connection_object_target_experiments.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/connection_object_with_name_repository.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/connection_object_with_name_repository.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/content_location.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/content_location.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/content_status.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/content_status.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/custom_models.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/custom_models.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/deploy_input.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/deploy_input.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/error_bad_request_libraries_target.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/error_bad_request_libraries_target.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/error_experiments.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/error_experiments.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/error_experiments_target.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/error_experiments_target.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/error_message.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/error_message.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/error_repository.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/error_repository.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/error_repository_target.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/error_repository_target.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/error_schema_experiments.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/error_schema_experiments.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/error_schema_repository.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/error_schema_repository.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/evaluation_definition.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/evaluation_definition.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/evaluation_definition_experiments.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/evaluation_definition_experiments.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/evaluation_definition_metrics.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/evaluation_definition_metrics.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/evaluation_definition_repository.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/evaluation_definition_repository.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/evaluation_definition_repository_metrics.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/evaluation_definition_repository_metrics.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/experiment_input.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/experiment_input.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/experiment_input_settings.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/experiment_input_settings.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/experiment_output.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/experiment_output.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/experiment_output_array.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/experiment_output_array.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/experiment_output_array_first.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/experiment_output_array_first.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/experiment_patch.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/experiment_patch.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/experiment_status_experiments.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/experiment_status_experiments.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/framework_output_repository.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/framework_output_repository.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/framework_output_repository_libraries.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/framework_output_repository_libraries.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/framework_output_repository_runtimes.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/framework_output_repository_runtimes.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/hyper_parameters.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/hyper_parameters.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/hyper_parameters_experiments.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/hyper_parameters_experiments.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/hyper_parameters_experiments_double_range.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/hyper_parameters_experiments_double_range.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/hyper_parameters_experiments_inner_double_range.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/hyper_parameters_experiments_inner_double_range.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/hyper_parameters_experiments_inner_int_range.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/hyper_parameters_experiments_inner_int_range.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/hyper_parameters_experiments_inner_values_range.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/hyper_parameters_experiments_inner_values_range.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/hyper_parameters_experiments_int_range.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/hyper_parameters_experiments_int_range.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/hyper_parameters_for_status_experiments.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/hyper_parameters_for_status_experiments.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/hyper_parameters_for_status_experiments_inner.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/hyper_parameters_for_status_experiments_inner.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/hyper_parameters_optimization_experiments.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/hyper_parameters_optimization_experiments.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/hyper_parameters_optimization_experiments_method.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/hyper_parameters_optimization_experiments_method.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/hyper_parameters_optimization_experiments_method_parameters.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/hyper_parameters_optimization_experiments_method_parameters.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/input_data_schema.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/input_data_schema.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/internal_input_batch.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/internal_input_batch.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/internal_output_batch.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/internal_output_batch.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/json_patch_array.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/json_patch_array.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/json_patch_entity.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/json_patch_entity.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/libraries_definition_input.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/libraries_definition_input.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/libraries_definition_input_platform.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/libraries_definition_input_platform.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/meta_object.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/meta_object.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/meta_object_experiments.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/meta_object_experiments.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/meta_object_experiments_metadata.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/meta_object_experiments_metadata.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/meta_object_functions_metadata.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/meta_object_functions_metadata.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/meta_object_metadata.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/meta_object_metadata.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/meta_object_repository.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/meta_object_repository.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/meta_object_repository_metadata.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/meta_object_repository_metadata.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/metric_object_experiments.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/metric_object_experiments.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/metrics_models.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/metrics_models.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_experiment_input.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_experiment_input.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_experiment_output.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_experiment_output.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_experiment_output_array.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_experiment_output_array.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_function_input.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_function_input.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_functions_output.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_functions_output.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_functions_output_array.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_functions_output_array.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_functions_output_array_first.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_functions_output_array_first.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_libraries_output.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_libraries_output.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_libraries_output_array.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_libraries_output_array.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_libraries_output_array_first.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_libraries_output_array_first.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_model_input.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_model_input.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_model_output.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_model_output.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_model_output_array.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_model_output_array.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_patch_libraries_output.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_patch_libraries_output.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_runtime_spec_output.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_runtime_spec_output.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_runtime_spec_output_array.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_runtime_spec_output_array.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_runtime_spec_output_array_first.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_create_runtime_spec_output_array_first.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_get_presigned_url_output.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_get_presigned_url_output.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_model_size_output.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_model_size_output.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_patch_function.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_patch_function.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_patch_libraries_input.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_patch_libraries_input.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_patch_runtime_spec_input.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_patch_runtime_spec_input.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_patch_runtime_spec_output.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_patch_runtime_spec_output.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_upload_content_output.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_upload_content_output.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_upload_content_output_entity.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_upload_content_output_entity.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_upload_content_output_metadata.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/ml_assets_upload_content_output_metadata.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/model_content_location.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/model_content_location.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/model_definition_models.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/model_definition_models.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/model_input.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/model_input.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/model_metrics.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/model_metrics.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/model_metrics_values.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/model_metrics_values.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/model_output.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/model_output.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/model_output_entity.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/model_output_entity.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/model_output_entity_pipeline_version.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/model_output_entity_pipeline_version.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/model_schemas.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/model_schemas.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/model_training_data_ref.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/model_training_data_ref.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/model_type.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/model_type.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/model_version_input.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/model_version_input.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/model_version_metrics_experiments.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/model_version_metrics_experiments.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/model_version_output.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/model_version_output.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/model_version_output_entity.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/model_version_output_entity.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/model_version_output_entity_model.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/model_version_output_entity_model.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/online_deploy_output.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/online_deploy_output.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/online_output.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/online_output.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/online_output_array.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/online_output_array.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/output_data_schema.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/output_data_schema.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/patch_operation_experiments.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/patch_operation_experiments.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/patch_operation_functions.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/patch_operation_functions.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/patch_operation_libraries.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/patch_operation_libraries.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/patch_operation_runtime_spec.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/patch_operation_runtime_spec.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/pipeline_input.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/pipeline_input.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/pipeline_models.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/pipeline_models.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/pipeline_output.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/pipeline_output.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/pipeline_output_entity.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/pipeline_output_entity.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/pipeline_type.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/pipeline_type.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/pipeline_version_input.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/pipeline_version_input.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/pipeline_version_output.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/pipeline_version_output.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/pipeline_version_output_entity.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/pipeline_version_output_entity.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/pipeline_version_output_entity_parent.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/pipeline_version_output_entity_parent.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/runtime_environment.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/runtime_environment.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/runtime_models.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/runtime_models.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/runtime_output_repository.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/runtime_output_repository.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/runtime_spec_definition_input.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/runtime_spec_definition_input.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/runtime_spec_definition_input_custom_libraries.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/runtime_spec_definition_input_custom_libraries.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/runtime_spec_definition_input_platform.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/runtime_spec_definition_input_platform.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/runtime_spec_definition_input_public_libraries.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/runtime_spec_definition_input_public_libraries.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/runtime_spec_definition_input_repository.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/runtime_spec_definition_input_repository.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/sample_scoring_input.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/sample_scoring_input.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/schemas.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/schemas.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/score_input.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/score_input.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/score_output.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/score_output.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/size_models.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/size_models.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/software_spec_models.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/software_spec_models.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/space_models.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/space_models.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/spark_service.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/spark_service.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/stream_input_internal.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/stream_input_internal.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/stream_internal.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/stream_internal.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/stream_output.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/stream_output.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/stream_output_array.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/stream_output_array.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/stream_output_internal.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/stream_output_internal.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/tag_repository.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/tag_repository.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/token_response.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/token_response.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/training_data_schema.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/training_data_schema.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/training_models.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/training_models.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/training_output_experiments.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/training_output_experiments.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/training_reference_experiments.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/training_reference_experiments.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/training_status_experiments.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/training_status_experiments.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/models/training_status_experiments_result.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/models/training_status_experiments_result.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/swagger_client/rest.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/swagger_client/rest.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/util/__init__.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/util/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/util/base_singleton.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/util/base_singleton.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/util/compression_util.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/util/compression_util.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/util/exceptions.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/util/file_system_ops.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/util/file_system_ops.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/util/generic_archive_file_check.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/util/generic_archive_file_check.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/util/json_2_object_mapper.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/util/json_2_object_mapper.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/util/library_imports.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/util/library_imports.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/util/spark_util.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/util/spark_util.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/libs/repo/util/unique_id_gen.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/libs/repo/util/unique_id_gen.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/metanames.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/metanames.py`

 * *Files 1% similar despite different names*

```diff
@@ -458,15 +458,15 @@
         MetaProp('INPUT_DATA_SCHEMA',       INPUT_DATA_SCHEMA,           list,       False,  example_value={"id":"1","type": "struct", "fields": [{"name": "x", "type": "double", "nullable": False, "metadata": {}}, {"name": "y", "type": "double", "nullable": False, "metadata": {}}]}, path="/input_data_schema",schema={u'id(required)':u'string',u'fields(required)':[{u'name(required)':u'string',u'type(required)':u'string',u'nullable(optional)':u'string'}]}),
         MetaProp('TRAINING_DATA_REFERENCES',TRAINING_DATA_REFERENCES,     list,       False,  [], path="/training_data_references",schema=[{"name(optional)":"string","type(required)":"string",u'connection(required)':{u'endpoint_url(required)': u'string',u'access_key_id(required)':u'string',u'secret_access_key(required)':u'string'},u'location(required)':{u'bucket':u'string',u'path':u'string'},u'schema(optional)':{u'id(required)':u'string',u'fields(required)':[{u'name(required)':u'string',u'type(required)':u'string',u'nullable(optional)':u'string'}]}}]),
         MetaProp('OUTPUT_DATA_SCHEMA',      OUTPUT_DATA_SCHEMA,          dict,       False,  example_value={"id":"1","type": "struct", "fields": [{"name": "x", "type": "double", "nullable": False, "metadata": {}}, {"name": "y", "type": "double", "nullable": False, "metadata": {}}]}, path="/output_data_schema",schema={u'id(required)':u'string',u'fields(required)':[{u'name(required)':u'string',u'type(required)':u'string',u'nullable(optional)':u'string'}]}),
         MetaProp('LABEL_FIELD',             LABEL_FIELD,                 STR_TYPE,   False,  example_value='PRODUCT_LINE', path="/label_column"),
         MetaProp('TRANSFORMED_LABEL_FIELD', TRANSFORMED_LABEL_FIELD,     STR_TYPE,   False,  example_value='PRODUCT_LINE_IX', path="/transformed_label"),
         MetaProp('TAGS',                    TAGS,                        list,       False,  example_value=["string","string"],schema=[ u'string', u'string']),
         MetaProp('SIZE',                    SIZE,                        dict,       False, example_value={"in_memory": 0,"content": 0},schema={u'in_memory(optional)': u'string', u'content(optional)': u'string'}),
-        MetaProp('SPACE_UID',                   SPACE_UID,                       STR_TYPE,   False,  example_value="53628d69-ced9-4f43-a8cd-9954344039a8", path="/space/href"),
+        MetaProp('SPACE_UID',                   SPACE_UID,                       STR_TYPE,   False,  example_value="53628d69-ced9-4f43-a8cd-9954344039a8", path="/space/href", hidden=True),
         MetaProp('PIPELINE_UID',                PIPELINE_UID,                    STR_TYPE,   False,  example_value="53628d69-ced9-4f43-a8cd-9954344039a8", path="/pipeline/href"),
         MetaProp('RUNTIME_UID', RUNTIME_UID, STR_TYPE, False, example_value="53628d69-ced9-4f43-a8cd-9954344039a8",path="/runtime/href"),
         MetaProp('TYPE',                    TYPE,                        STR_TYPE,   True,  example_value="mllib_2.1", path="/type"),
         MetaProp('CUSTOM',                  CUSTOM ,                      dict,     False, example_value={}),
         MetaProp('DOMAIN',                  DOMAIN,                       STR_TYPE, False, example_value="Watson Machine Learning"),
         MetaProp('HYPER_PARAMETERS', HYPER_PARAMETERS,                    dict, False, example_value=""),
         MetaProp('METRICS',                 METRICS,                      list, False, example_value=""),
@@ -474,15 +474,17 @@
         MetaProp('TRAINING_LIB_UID',     TRAINING_LIB_UID,    STR_TYPE, False,  example_value="53628d69-ced9-4f43-a8cd-9954344039a8", path="/training_lib"),
         MetaProp('MODEL_DEFINITION_UID',MODEL_DEFINITION_UID, STR_TYPE, False, example_value="53628d6_cdee13-35d3-s8989343", path="/model_definition"),
         MetaProp('SOFTWARE_SPEC_UID', SOFTWARE_SPEC_UID, STR_TYPE, False, example_value="53628d69-ced9-4f43-a8cd-9954344039a8", path="/software_spec/id", transform=lambda x, client: x),
         MetaProp('TF_MODEL_PARAMS',   TF_MODEL_PARAMS,   dict,     False, example_value={"save_format": "None", "signatures": "struct","options": "None", "custom_objects": "string"},path="/tf_model_params")
     ]
 
 
-    __doc__ = MetaNamesBase(_meta_props_definitions)._generate_doc('models')
+    __doc__ = MetaNamesBase(_meta_props_definitions)._generate_doc('models') + '''
+**Note:** `project` (MetaNames.PROJECT_UID) and `space` (MetaNames.SPACE_UID) meta names are not supported and considered as invalid. Instead use client.set.default_space(<SPACE_GUID>) to set the space or client.set.default_project(<PROJECT_GUID>).
+    '''
 
     def __init__(self):
         MetaNamesBase.__init__(self, self._meta_props_definitions)
 
 
 class PayloadLoggingMetaNames(MetaNamesBase):
     PAYLOAD_DATA_REFERENCE = "payload_store"
```

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/migration_v4ga_cloud.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/migration_v4ga_cloud.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/model_definition.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/model_definition.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/models.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/models.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/pipelines.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/pipelines.py`

 * *Files 0% similar despite different names*

```diff
@@ -487,15 +487,15 @@
                 In cloud platform, this method returns all the revision details of given pipeline_uid. rev_uid parameter is not applicable in Cloud platform.
          """
         pipeline_uid = str_type_conv(pipeline_uid)
         Pipelines._validate_type(pipeline_uid, u'pipeline_uid', STR_TYPE, True)
         Pipelines._validate_type(rev_uid, u'rev_uid', int, True)
         if not self._client.ICP_30 and not self._client.CLOUD_PLATFORM_SPACES and not self._client.ICP_35 and not self._client.ICP_40:
             raise WMLClientError(
-                'Not supported. Revisions APIs are supported only for IBM Cloud Pak® for Data for Data 3.0 and above.')
+                'Not supported. Revisions APIs are supported only for IBM Cloud Pak® for Data 3.0 and above.')
         else:
             url = self._client.service_instance._href_definitions.get_pipeline_href(pipeline_uid)
         return self._get_with_or_without_limit(url, limit=None, op_name="pipeline",
                                                summary=None, pre_defined=None, revision=rev_uid)
 
     @staticmethod
     @docstring_parameter({'str_type': STR_TYPE_NAME})
```

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/pkg_extn.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/pkg_extn.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/platform_spaces.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/platform_spaces.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/preprocessing/__init__.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/preprocessing/data_join_pipeline.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/preprocessing/data_join_pipeline.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/preprocessing/multiple_files_preprocessor.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/preprocessing/multiple_files_preprocessor.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/preprocessing/templates/__init__.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/preprocessing/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/preprocessing/templates/pretty_print_template.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/preprocessing/templates/pretty_print_template.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/remote_training_system.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/remote_training_system.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/repository.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/repository.py`

 * *Files 0% similar despite different names*

```diff
@@ -1139,15 +1139,15 @@
            **Example**
 
                  >>> model_rev_details = client.respository.get_model_revision_details(model_uid, rev_uid)
 
         """
 
         if not self._client.ICP_30 and not self._client.CLOUD_PLATFORM_SPACES and not self._client.ICP_PLATFORM_SPACES:
-            raise WMLClientError('Not supported. Revisions APIs are supported only for IBM Cloud Pak® for Data for Data 3.0 and above.')
+            raise WMLClientError('Not supported. Revisions APIs are supported only for IBM Cloud Pak® for Data 3.0 and above.')
         return self._client._models.get_revision_details(model_uid, rev_uid)
 
     @docstring_parameter({'str_type': STR_TYPE_NAME})
     def get_experiment_details(self, experiment_uid=None, limit=None):
         """
            Get metadata of experiment. If no experiment_uid is specified all experiments metadata is returned.
 
@@ -1209,15 +1209,15 @@
 
                  >>> experiment_rev_details = client.respository.get_experiment__revision_details(experiment_uid, rev_uid)
 
         """
 
         if not self._client.ICP_30 and not self._client.CLOUD_PLATFORM_SPACES and not self._client.ICP_PLATFORM_SPACES:
             raise WMLClientError(
-                'Not supported. Revisions APIs are supported only for IBM Cloud Pak® for Data for Data 3.0 and above.')
+                'Not supported. Revisions APIs are supported only for IBM Cloud Pak® for Data 3.0 and above.')
 
         return self._client.experiments.get_revision_details(experiment_uid, rev_id)
 
 
     @docstring_parameter({'str_type': STR_TYPE_NAME})
     def get_function_details(self, function_uid=None, limit=None):
         """
@@ -1334,15 +1334,15 @@
            **Example**
 
                 >>> pipeline_rev_details = client.repository.get_pipeline_revision_details(pipeline_uid, rev_id)
         """
 
         if not self._client.ICP_30 and not self._client.CLOUD_PLATFORM_SPACES and not self._client.ICP_PLATFORM_SPACES:
             raise WMLClientError(
-                'Not supported. Revisions APIs are supported only for IBM Cloud Pak® for Data for Data 3.0 and above.')
+                'Not supported. Revisions APIs are supported only for IBM Cloud Pak® for Data 3.0 and above.')
         return self._client.pipelines.get_revision_details(pipeline_uid, rev_id)
 
 
     @docstring_parameter({'str_type': STR_TYPE_NAME})
     def get_space_details(self, space_uid=None, limit=None):
         """
            Get metadata of stored space. If space_uid is not specified returns all model spaces metadata.
```

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/runtimes.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/runtimes.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/script.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/script.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/shiny.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/shiny.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/spaces.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/spaces.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 
 _DEFAULT_LIST_LENGTH = 50
 
 
 class Spaces(WMLResource):
     """
-    Store and manage your spaces. This is applicable only for IBM Cloud Pak® for Data for Data
+    Store and manage your spaces. This is applicable only for IBM Cloud Pak® for Data
     """
     ConfigurationMetaNames = SpacesMetaNames()
     MemberMetaNames = MemberMetaNames()
     ExportMetaNames = ExportMetaNames()
     """MetaNames for spaces creation."""
 
     def __init__(self, client):
```

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/sw_spec.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/sw_spec.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/Connections_SPSS_BIGQUERY_MYSQL_spaces_cp4d_35.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/Connections_SPSS_BIGQUERY_MYSQL_spaces_cp4d_35.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/Connections_SPSS_MSSQL_spaces_cp4d_35.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/Connections_SPSS_MSSQL_spaces_cp4d_35.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/Connections_SPSS_TERADATA_MYSQL_spaces_cp4d_35.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/Connections_SPSS_TERADATA_MYSQL_spaces_cp4d_35.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/DataAssets_spaces_cp4d_35.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/DataAssets_spaces_cp4d_35.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/Experiment_Pipeline_spaces_cp4d_35.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/Experiment_Pipeline_spaces_cp4d_35.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/ExportImport_spaces_cp4d_35.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/ExportImport_spaces_cp4d_35.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/Functions_spaces_cp4d_35.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/Functions_spaces_cp4d_35.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/HardwareSpec_spaces_cp4d_35.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/HardwareSpec_spaces_cp4d_35.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/ModeDoFromFile_spaces_cp4d_35.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/ModeDoFromFile_spaces_cp4d_35.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/ModelDefinition_projects_dev_cp4d_35.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/ModelDefinition_projects_dev_cp4d_35.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/ModelDefinition_spaces_cp4d_35.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/ModelDefinition_spaces_cp4d_35.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/ModelPMML_spaces_cp4d_35.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/ModelPMML_spaces_cp4d_35.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/Model_Hybrid_from_zipfile_spaces_cp4d_35.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/Model_Hybrid_from_zipfile_spaces_cp4d_35.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/Model_keras_spaces_cp4d_35.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/Model_keras_spaces_cp4d_35.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/Model_pmml_spaces_cp4d_35.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/Model_pmml_spaces_cp4d_35.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/Model_scikit_learn_from_object_sw_spaces_cp4d_35.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/Model_scikit_learn_from_object_sw_spaces_cp4d_35.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/Model_spark_mllib_from_object_spaces_cp4d_35.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/Model_spark_mllib_from_object_spaces_cp4d_35.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/Model_spss_from_file_spaces_cp4d_35.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/Model_spss_from_file_spaces_cp4d_35.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/Model_tensorflow_spaces_cp4d_35.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/Model_tensorflow_spaces_cp4d_35.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/PkgExt_spaces_cp4d_35.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/PkgExt_spaces_cp4d_35.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/RScripts_spaces_cp4d_35.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/RScripts_spaces_cp4d_35.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/RShiny_projects_dev_cp4d_35.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/RShiny_projects_dev_cp4d_35.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/RShiny_spaces_cp4d_35.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/RShiny_spaces_cp4d_35.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/Remote_training_systems_spaces_cp4d_35.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/Remote_training_systems_spaces_cp4d_35.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/Scripts_projects_dev_cp4d_35.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/Scripts_projects_dev_cp4d_35.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/Scripts_spaces_cp4d_35.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/Scripts_spaces_cp4d_35.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/SoftwareSpec_projects_dev_cp4d_35.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/SoftwareSpec_projects_dev_cp4d_35.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/SoftwareSpec_spaces_cp4d_35.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/SoftwareSpec_spaces_cp4d_35.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/models_preparation.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/models_preparation.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/preparation_and_cleaning.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/preparation_and_cleaning.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/spaces_cp4d_35.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/spaces_cp4d_35.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/CP4D_35/test_CP4D_3_connections.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/CP4D_35/test_CP4D_3_connections.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/Cloud/DataAssets_spaces_cloud.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/Cloud/DataAssets_spaces_cloud.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/Cloud/Experiment_Pipeline_spaces_cloud.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/Cloud/Experiment_Pipeline_spaces_cloud.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/Cloud/ExportImport_spaces_cloud.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/Cloud/ExportImport_spaces_cloud.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/Cloud/Functions_spaces_cloud.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/Cloud/Functions_spaces_cloud.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/Cloud/HardwareSpec_spaces_cloud.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/Cloud/HardwareSpec_spaces_cloud.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/Cloud/ModeDoFromFile_spaces_cloud.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/Cloud/ModeDoFromFile_spaces_cloud.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/Cloud/ModelDefinition_projects_dev_cloud.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/Cloud/ModelDefinition_projects_dev_cloud.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/Cloud/ModelDefinition_spaces_cloud.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/Cloud/ModelDefinition_spaces_cloud.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/Cloud/ModelPMML_spaces_cloud.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/Cloud/ModelPMML_spaces_cloud.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/Cloud/Model_Hybrid_from_zipfile_spaces_cloud.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/Cloud/Model_Hybrid_from_zipfile_spaces_cloud.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/Cloud/Model_keras_spaces_cloud.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/Cloud/Model_keras_spaces_cloud.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/Cloud/Model_pmml_spaces_cloud.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/Cloud/Model_pmml_spaces_cloud.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/Cloud/Model_scikit_learn_from_object_sw_spaces_cloud.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/Cloud/Model_scikit_learn_from_object_sw_spaces_cloud.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/Cloud/Model_spark_mllib_from_object_spaces_cloud.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/Cloud/Model_spark_mllib_from_object_spaces_cloud.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/Cloud/Model_spss_from_file_spaces_cloud.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/Cloud/Model_spss_from_file_spaces_cloud.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/Cloud/Model_tensorflow_spaces_cloud.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/Cloud/Model_tensorflow_spaces_cloud.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/Cloud/PkgExt_spaces_cloud.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/Cloud/PkgExt_spaces_cloud.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/Cloud/RShiny_projects_dev_cloud.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/Cloud/RShiny_projects_dev_cloud.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/Cloud/RShiny_spaces_cloud.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/Cloud/RShiny_spaces_cloud.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/Cloud/Remote_training_systems_spaces_cloud.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/Cloud/Remote_training_systems_spaces_cloud.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/Cloud/Scripts_projects_dev_cloud.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/Cloud/Scripts_projects_dev_cloud.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/Cloud/Scripts_spaces_cloud.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/Cloud/Scripts_spaces_cloud.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/Cloud/SoftwareSpec_projects_dev_cloud.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/Cloud/SoftwareSpec_projects_dev_cloud.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/Cloud/SoftwareSpec_spaces_cloud.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/Cloud/SoftwareSpec_spaces_cloud.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/Cloud/models_preparation.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/Cloud/models_preparation.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/Cloud/preparation_and_cleaning.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/Cloud/preparation_and_cleaning.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/Cloud/spaces_cloud.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/Cloud/spaces_cloud.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/ConfigFileEncoder.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/ConfigFileEncoder.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/ConfigFileGenerator.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/ConfigFileGenerator.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/ICP/CP4D_mllib_from_object.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/ICP/CP4D_mllib_from_object.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/ICP/models_preparation.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/ICP/models_preparation.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/ICP/preparation_and_cleaning.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/ICP/preparation_and_cleaning.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/ICP/test-CP4D_3_hybrid_autoai_model.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/ICP/test-CP4D_3_hybrid_autoai_model.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/ICP/test_CP4D_3_connections.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/ICP/test_CP4D_3_connections.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/ICP/test_CP4D_3_cross_deployment_model_function.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/ICP/test_CP4D_3_cross_deployment_model_function.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/ICP/test_CP4D_3_cross_deployment_model_model.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/ICP/test_CP4D_3_cross_deployment_model_model.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/ICP/test_CP4D_3_do_from_file.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/ICP/test_CP4D_3_do_from_file.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/ICP/test_CP4D_3_functions_sw.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/ICP/test_CP4D_3_functions_sw.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/ICP/test_CP4D_3_import_export_spaces.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/ICP/test_CP4D_3_import_export_spaces.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/ICP/test_CP4D_3_mllib_2_4_from_object_sw.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/ICP/test_CP4D_3_mllib_2_4_from_object_sw.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/ICP/test_CP4D_3_pkg_extn.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/ICP/test_CP4D_3_pkg_extn.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/ICP/test_CP4D_3_rshiny.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/ICP/test_CP4D_3_rshiny.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/ICP/test_CP4D_3_scikit_learn_from_object_sw.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/ICP/test_CP4D_3_scikit_learn_from_object_sw.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/ICP/test_CP4D_3_scripts.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/ICP/test_CP4D_3_scripts.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/ICP/test_CP4D_3_software_spec.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/ICP/test_CP4D_3_software_spec.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/ICP/test_CP4D_3_spss_from_file.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/ICP/test_CP4D_3_spss_from_file.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/ICP/test_CP4D_functions.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/ICP/test_CP4D_functions.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/ICP/test_CP4D_runtimes.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/ICP/test_CP4D_runtimes.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/ICP/test_CP4D_scikit_learn_from_object.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/ICP/test_CP4D_scikit_learn_from_object.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/ICP/test_CP4D_spaces.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/ICP/test_CP4D_spaces.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/WSD/WSD_functions.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/WSD/WSD_functions.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/WSD/WSD_mllib_from_object.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/WSD/WSD_mllib_from_object.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/WSD/WSD_scikit_learn_from_object.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/WSD/WSD_scikit_learn_from_object.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/WSD/models_preparation.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/WSD/models_preparation.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/WSD/preparation_and_cleaning.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/WSD/preparation_and_cleaning.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/fvt/local_optimizer_for_CP4D35.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/fvt/local_optimizer_for_CP4D35.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/fvt/test__lale__breast_cancer.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/fvt/test__lale__breast_cancer.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/fvt/test_any_autoai_experiment__lale__.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/fvt/test_any_autoai_experiment__lale__.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/fvt/test_breast_cancer_binary_lgbm.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/fvt/test_breast_cancer_binary_lgbm.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/fvt/test_breast_cancer_binary_sklearn.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/fvt/test_breast_cancer_binary_sklearn.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/fvt/test_breast_cancer_binary_xgboost.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/fvt/test_breast_cancer_binary_xgboost.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/fvt/test_credit_risk_binary_local_ai4ml.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/fvt/test_credit_risk_binary_local_ai4ml.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/fvt/test_custom_separator_binary_multiclass_regression.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/fvt/test_custom_separator_binary_multiclass_regression.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/fvt/test_insurance_regression_lgbm.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/fvt/test_insurance_regression_lgbm.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/fvt/test_insurance_regression_sklearn.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/fvt/test_insurance_regression_sklearn.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/fvt/test_insurance_regression_xgboost.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/fvt/test_insurance_regression_xgboost.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/fvt/test_iris_wml_autoai_multiclass_CP4D_3_5.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/fvt/test_iris_wml_autoai_multiclass_CP4D_3_5.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/fvt/test_local_optimizer_with_cos.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/fvt/test_local_optimizer_with_cos.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/fvt/test_obm_plus_kb_go_sales_multiclass.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/fvt/test_obm_plus_kb_go_sales_multiclass.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/fvt/test_student_multiclass_lgbm.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/fvt/test_student_multiclass_lgbm.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/fvt/test_student_multiclass_sklearn.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/fvt/test_student_multiclass_sklearn.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/fvt/test_student_multiclass_xgboost.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/fvt/test_student_multiclass_xgboost.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/fvt/test_xlsx_read_binary_regression.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/fvt/test_xlsx_read_binary_regression.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/manual/test_bank_binary.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/manual/test_bank_binary.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/abstract_test_iris_using_database_connection.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/abstract_test_iris_using_database_connection.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/abstract_test_iris_using_database_data_asset.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/abstract_test_iris_using_database_data_asset.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/abstract_test_iris_wml_autoai_multiclass_connections.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/abstract_test_iris_wml_autoai_multiclass_connections.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_bank_wml_autoai_xlsx_binary.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_bank_wml_autoai_xlsx_binary.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,27 +103,26 @@
             cls.cos_credentials = get_cos_credentials()
             cls.cos_endpoint = cls.cos_credentials.get('endpoint_url')
             cls.cos_resource_instance_id = cls.cos_credentials.get('resource_instance_id')
 
         cls.wml_client = APIClient(wml_credentials=cls.wml_credentials)
         cls.project_id = cls.wml_credentials.get('project_id')
 
+        cls.wml_client.set.default_project(cls.project_id)
+
 
     def test_00a_space_cleanup(self):
         space_cleanup(self.wml_client,
                       get_space_id(self.wml_client, self.space_name,
                                    cos_resource_instance_id=self.cos_resource_instance_id),
                       days_old=7)
         TestAutoAIRemote.space_id = get_space_id(self.wml_client, self.space_name,
                                                  cos_resource_instance_id=self.cos_resource_instance_id)
 
-        if self.wml_client.ICP:
-            self.wml_client.set.default_project(self.project_id)
-        else:
-            self.wml_client.set.default_space(self.space_id)
+
 
     def test_00b_prepare_COS_instance(self):
         if self.wml_client.ICP:
             self.skipTest("Prepare COS is available only for Cloud")
 
         import ibm_boto3
         cos_resource = ibm_boto3.resource(
@@ -232,17 +231,14 @@
         self.assertNotEqual(status, RunStateTypes.COMPLETED)
 
     def test_06b_get_run_details(self):
         parameters = self.remote_auto_pipelines.get_run_details()
         # print(parameters)
         self.assertIsNotNone(parameters)
 
-    def test_06c_get_metrics(self):
-        self.wml_client.training.get_metrics(self.run_id)
-
     def test_07_get_summary(self):
 
         print(f"Run status = {self.remote_auto_pipelines.get_run_status()}")
         # note: check if first pipeline was generated
 
         metrics = self.wml_client.training.get_details(self.run_id)['entity']['status'].get('metrics', [])
         while chose_model_output("1") not in str(metrics) and self.remote_auto_pipelines.get_run_status() not in [
@@ -287,14 +283,17 @@
 
         TestAutoAIRemote.best_pipeline_name_so_far = summary_df.index[0]
         print("\nGetting best calculated pipeline: ", self.best_pipeline_name_so_far)
 
         pipeline = self.remote_auto_pipelines.get_pipeline()
         print(f"Fetched pipeline type: {type(pipeline)}")
 
+    def test_09b_get_metrics(self):
+        self.wml_client.training.get_metrics(self.run_id)
+
     #################################
     #      DEPLOYMENT SECTION       #
     #################################
 
     def test_10_deployment_setup_and_preparation(self):
         TestAutoAIRemote.service = WebService(source_wml_credentials=self.wml_credentials.copy(),
                                               source_project_id=self.project_id,
```

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_breast_cancer_wml_autoai_csv_binary.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_breast_cancer_wml_autoai_csv_binary.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_breast_cancer_wml_autoai_csv_binary_apikey_auth.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_breast_cancer_wml_autoai_csv_binary_apikey_auth.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_breast_cancer_wml_autoai_csv_binary_token_auth.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_breast_cancer_wml_autoai_csv_binary_token_auth.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_car_price_wml_autoai_regression.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_car_price_wml_autoai_regression.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,14 +116,15 @@
             cls.cos_resource_instance_id = cls.cos_credentials.get('resource_instance_id')
         else:
             # note: xlsx is not supported on WMLS
             cls.data_location = './autoai/data/CarPrice_Assignment.csv'
             # --- end note
 
         cls.project_id = cls.wml_credentials.get('project_id')
+        cls.wml_client.set.default_project(cls.project_id)
 
     def _check_optimizer_parameters(self, parameters):
         # check_pipeline_parameters:
         self.assertIsNotNone(parameters.get('name'))
 
         self.assertEqual(parameters.get('prediction_column'), self.prediction_column)
         self.assertEqual(parameters.get('text_processing'), self.text_processing)
@@ -134,18 +135,14 @@
     def test_00a_space_cleanup(self):
         space_cleanup(self.wml_client,
                       get_space_id(self.wml_client, self.space_name,
                                    cos_resource_instance_id=self.cos_resource_instance_id),
                       days_old=7)
         TestAutoAIRemote.space_id = get_space_id(self.wml_client, self.space_name,
                                      cos_resource_instance_id=self.cos_resource_instance_id)
-        if self.wml_client.ICP:
-            self.wml_client.set.default_project(self.project_id)
-        else:
-            self.wml_client.set.default_space(self.space_id)
 
     def test_00b_prepare_COS_instance(self):
         if self.wml_client.ICP or self.wml_client.WSD:
             self.skipTest("Prepare COS is available only for Cloud")
         import ibm_boto3
         cos_resource = ibm_boto3.resource(
             service_name="s3",
@@ -262,17 +259,14 @@
         self.assertNotEqual(status, RunStateTypes.COMPLETED)
 
     def test_07_get_run_details(self):
         parameters = self.remote_auto_pipelines.get_run_details()
         # print(parameters)
         self.assertIsNotNone(parameters)
 
-    def test_07b_get_metrics(self):
-        self.wml_client.training.get_metrics(self.run_id)
-
     def test_08_get_summary(self):
 
         print(f"Run status = {self.remote_auto_pipelines.get_run_status()}")
         # note: check if first pipeline was generated
 
         metrics = self.wml_client.training.get_details(self.run_id)['entity']['status'].get('metrics', [])
         while chose_model_output("1") not in str(metrics) and self.remote_auto_pipelines.get_run_status() not in ['failed', 'canceled']:
@@ -315,14 +309,17 @@
 
         summary_df = self.remote_auto_pipelines.summary()
         print(summary_df)
 
         pipeline = self.remote_auto_pipelines.get_pipeline()
         print(f"Fetched pipeline type: {type(pipeline)}")
 
+    def test_10b_get_metrics(self):
+        self.wml_client.training.get_metrics(self.run_id)
+
     def test_11_waiting_for_fitted_completed(self):
         while self.remote_auto_pipelines.get_run_status() == 'running':
             time.sleep(10)
 
         status = self.remote_auto_pipelines.get_run_status()
 
         self.assertEqual(status, RunStateTypes.COMPLETED, msg="AutoAI run didn't finished successfully. Status: {}".format(status))
@@ -434,22 +431,18 @@
         self.wml_client.set.default_project(self.project_id) if is_cp4d() else None
 
     #########################
     #  Batch deployment
     #########################
 
     def test_30_batch_deployment_setup_and_preparation(self):
-        if self.wml_client.ICP:
-            TestAutoAIRemote.service_batch = Batch(source_wml_credentials=self.wml_credentials.copy(),
-                                                   source_project_id=self.project_id,
-                                                   target_wml_credentials=self.wml_credentials,
-                                                   target_space_id=self.space_id)
-        else:
-            TestAutoAIRemote.service_batch = Batch(self.wml_credentials,
-                                                   source_space_id=self.space_id)
+        TestAutoAIRemote.service_batch = Batch(source_wml_credentials=self.wml_credentials.copy(),
+                                               source_project_id=self.project_id,
+                                               target_wml_credentials=self.wml_credentials,
+                                               target_space_id=self.space_id)
 
         self.assertIsInstance(self.service_batch, Batch, msg="Deployment is not of Batch type.")
         self.assertIsInstance(self.service_batch._source_workspace, WorkSpace, msg="Workspace set incorrectly.")
         self.assertEqual(self.service_batch.id, None, msg="Deployment ID initialized incorrectly")
         self.assertEqual(self.service_batch.name, None, msg="Deployment name initialized incorrectly")
 
     def test_32__deploy__batch_deploy_pipeline_from_autoai_on_wml(self):
```

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_credit_risk_as_sample_notebook_binary.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_credit_risk_as_sample_notebook_binary.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_drop_duplicates.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_drop_duplicates.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_insurance_wml_autoai_xlsx_regression.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_insurance_wml_autoai_xlsx_regression.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_iris_using_data_asset_and_connected_asset.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_iris_using_data_asset_and_connected_asset.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_iris_using_data_asset_and_default.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_iris_using_data_asset_and_default.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_iris_using_data_connected_asset_and_connected_asset.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_iris_using_data_connected_asset_and_connected_asset.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_iris_using_data_connected_asset_and_default.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_iris_using_data_connected_asset_and_default.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_iris_using_data_connected_asset_and_s3.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_iris_using_data_connected_asset_and_s3.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_iris_using_data_s3_and_connected_asset.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_iris_using_data_s3_and_connected_asset.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_iris_using_data_s3_and_s3.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_iris_using_data_s3_and_s3.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_iris_using_database_connection.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_iris_using_database_connection.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_iris_using_database_data_asset.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_iris_using_database_data_asset.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_iris_using_filesystem_and_connected_asset.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_iris_using_filesystem_and_connected_asset.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_iris_using_filesystem_and_default.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_iris_using_filesystem_and_default.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_iris_wml_autoai_multiclass.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_iris_wml_autoai_multiclass.py`

 * *Files 0% similar despite different names*

```diff
@@ -346,15 +346,15 @@
         self.assertIn('prediction_type', run_params,
                       msg="prediction_type field not fount in run_params. Run_params are: {}".format(run_params))\
 
         historical_opt = self.experiment.runs.get_optimizer(self.random_run_id)
         self.assertIsInstance(historical_opt, RemoteAutoPipelines,
                               msg="historical_optimizer is not type RemoteAutoPipelines. It's type of {}".format(
                                   type(historical_opt)))
-        summary = self.historical_opt.summary()
+        summary = historical_opt.summary()
 
         self.assertGreater(len(summary), 0, msg=f"No pipelines found for optimizer with run_id = {self.random_run_id},"
                                                 f" and parameters: {run_params}")
         pipeline_name = summary.index.values[0]
         pipeline = historical_opt.get_pipeline(pipeline_name, self.experiment.PipelineTypes.SKLEARN)
         print(type(pipeline))
         self.assertIsInstance(pipeline, Pipeline)
```

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_iris_wml_autoai_multiclass_connections.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_iris_wml_autoai_multiclass_connections.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_iris_wml_autoai_multiclass_space_only.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_iris_wml_autoai_multiclass_space_only.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_iris_wml_autoai_multiclass_using_NFS.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_iris_wml_autoai_multiclass_using_NFS.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_iris_wml_autoai_multiclass_using_data_asset.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_iris_wml_autoai_multiclass_using_data_asset.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_obm_group_customer.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_obm_group_customer.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 from ibm_watson_machine_learning.experiment import AutoAI
 from ibm_watson_machine_learning.deployment import Batch
 from ibm_watson_machine_learning.preprocessing import DataJoinGraph
 from ibm_watson_machine_learning.preprocessing.data_join_pipeline import OBMPipelineGraphBuilder
 
 from ibm_watson_machine_learning.helpers.connections import S3Connection, S3Location, DataConnection, FSLocation
+from ibm_watson_machine_learning.utils import WMLClientError
 
 from ibm_watson_machine_learning.experiment.autoai.optimizers import RemoteAutoPipelines
 
 from ibm_watson_machine_learning.tests.utils import bucket_exists, \
     create_bucket, get_space_id
 
 from ibm_watson_machine_learning.tests.utils.cleanup import space_cleanup
@@ -103,28 +104,26 @@
             cls.cos_credentials = get_cos_credentials()
             if 'endpoint_url' in cls.cos_credentials:
                 cls.cos_endpoint = cls.cos_credentials['endpoint_url']
             cls.cos_resource_instance_id = cls.cos_credentials.get('resource_instance_id')
 
         cls.wml_client = APIClient(wml_credentials=cls.wml_credentials.copy())
         cls.project_id = cls.wml_credentials.get('project_id')
+        cls.wml_client.set.default_project(cls.project_id)
+
+    # @print_test_separators
+    # def test_00a_space_cleanup(self):
+    #     space_cleanup(self.wml_client,
+    #                   get_space_id(self.wml_client, self.space_name,
+    #                                cos_resource_instance_id=self.cos_resource_instance_id),
+    #                   days_old=7)
+    #     TestOBMOnly.space_id = get_space_id(self.wml_client, self.space_name,
+    #                                  cos_resource_instance_id=self.cos_resource_instance_id)
 
-    @print_test_separators
-    def test_00a_space_cleanup(self):
-        space_cleanup(self.wml_client,
-                      get_space_id(self.wml_client, self.space_name,
-                                   cos_resource_instance_id=self.cos_resource_instance_id),
-                      days_old=7)
-        TestOBMOnly.space_id = get_space_id(self.wml_client, self.space_name,
-                                     cos_resource_instance_id=self.cos_resource_instance_id)
 
-        if self.wml_client.ICP:
-            self.wml_client.set.default_project(self.project_id)
-        else:
-            self.wml_client.set.default_space(self.space_id)
 
     @print_test_separators
     def test_00b_prepare_COS_instance(self):
         if self.wml_client.ICP or self.wml_client.WSD:
             self.skipTest("Prepare COS is available only for Cloud")
 
         import ibm_boto3
@@ -255,16 +254,15 @@
     #     print("Visualizing data_join_graph...")
     #     self.data_join_graph.visualize()
 
     @print_test_separators
     def test_04_initialize_AutoAI_experiment__pass_credentials__object_initialized(self):
         print("Initializing AutoAI experiment...")
         TestOBMOnly.experiment = AutoAI(wml_credentials=self.wml_credentials.copy(),
-                                        project_id=self.project_id,
-                                        space_id=self.space_id)
+                                        project_id=self.project_id)
 
         self.assertIsInstance(self.experiment, AutoAI, msg="Experiment is not of type AutoAI.")
 
     @print_test_separators
     def test_05_save_remote_data_and_DataConnection_setup(self):
         print("Writing multiple data files to COS...")
         if is_cp4d():
@@ -476,15 +474,16 @@
     def test_14_get_run_details(self):
         print("Getting training details...")
         parameters = self.remote_auto_pipelines.get_run_details()
         print(parameters)
         self.assertIsNotNone(parameters)
 
     def test_14b_get_metrics(self):
-        self.wml_client.training.get_metrics(self.run_id)
+        with self.assertRaises(WMLClientError, msg="No metrics available for obm only"):
+            self.wml_client.training.get_metrics(self.run_id)
 
     @print_test_separators
     def test_15__get_data_connections__return_a_list_with_data_connections_with_optimizer_params(self):
         print("Getting all data connections...")
         data_connections = self.remote_auto_pipelines.get_data_connections()
         self.assertIsInstance(data_connections, list, msg="There should be a list container returned")
         self.assertIsInstance(data_connections[0], DataConnection,
```

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_obm_plus_kb_group_customer_regression.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_obm_plus_kb_group_customer_regression.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_obm_plus_kb_group_customer_regression_csv_only.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_obm_plus_kb_group_customer_regression_csv_only.py`

 * *Files 7% similar despite different names*

```diff
@@ -119,28 +119,26 @@
         if not is_cp4d():
             cls.cos_credentials = get_cos_credentials()
             cls.cos_endpoint = cls.cos_credentials.get('endpoint_url')
             cls.cos_resource_instance_id = cls.cos_credentials.get('resource_instance_id')
 
         cls.wml_client = APIClient(wml_credentials=cls.wml_credentials.copy())
         cls.project_id = cls.wml_credentials.get('project_id')
+        cls.wml_client.set.default_project(cls.project_id)
+
 
     @print_test_separators
     def test_00a_space_cleanup(self):
         space_cleanup(self.wml_client,
                       get_space_id(self.wml_client, self.space_name,
                                    cos_resource_instance_id=self.cos_resource_instance_id),
                       days_old=7)
         TestOBMAndKB.space_id = get_space_id(self.wml_client, self.space_name,
                                              cos_resource_instance_id=self.cos_resource_instance_id)
 
-        if self.wml_client.ICP:
-            self.wml_client.set.default_project(self.project_id)
-        else:
-            self.wml_client.set.default_space(self.space_id)
 
     @print_test_separators
     def test_00b_prepare_COS_instance(self):
         if self.wml_client.ICP or self.wml_client.WSD:
             self.skipTest("Prepare COS is available only for Cloud")
 
         import ibm_boto3
@@ -278,16 +276,15 @@
     #     print("Visualizing data_join_graph...")
     #     self.data_join_graph.visualize()
 
     @print_test_separators
     def test_04_initialize_AutoAI_experiment__pass_credentials__object_initialized(self):
         print("Initializing AutoAI experiment...")
         TestOBMAndKB.experiment = AutoAI(wml_credentials=self.wml_credentials.copy(),
-                                         project_id=self.project_id,
-                                         space_id=self.space_id)
+                                         project_id=self.project_id)
 
         self.assertIsInstance(self.experiment, AutoAI, msg="Experiment is not of type AutoAI.")
 
     @print_test_separators
     def test_05_save_remote_data_and_DataConnection_setup(self):
         print("Writing multiple data files to COS...")
         if is_cp4d():
@@ -695,35 +692,27 @@
 
     #################################
     #      DEPLOYMENT SECTION       #
     #################################
 
     @print_test_separators
     def test_26_batch_deployment_setup_and_preparation(self):
-        if is_cp4d():
-            TestOBMAndKB.service = Batch(source_wml_credentials=self.wml_credentials.copy(),
-                                         source_project_id=self.project_id,
-                                         target_wml_credentials=self.wml_credentials.copy(),
-                                         target_space_id=self.space_id)
-        else:
-            TestOBMAndKB.service = Batch(self.wml_credentials,
-                                         source_space_id=self.space_id,
-                                         target_wml_credentials=self.wml_credentials,
-                                         target_space_id=self.space_id)
+        TestOBMAndKB.service = Batch(source_wml_credentials=self.wml_credentials.copy(),
+                                     source_project_id=self.project_id,
+                                     target_wml_credentials=self.wml_credentials.copy(),
+                                     target_space_id=self.space_id)
 
-        self.wml_client.set.default_space(self.space_id) if self.wml_client.ICP else None
 
     @print_test_separators
     def test_27_deploy__deploy_best_computed_pipeline_from_autoai_on_wml(self):
         self.service.create(
             experiment_run_id=self.remote_auto_pipelines._engine._current_run_id,
             model=self.pipeline_name,
             deployment_name=self.DEPLOYMENT_NAME)
 
-        self.wml_client.set.default_project(self.project_id) if self.wml_client.ICP else None
 
     @print_test_separators
     def test_28_score_deployed_model(self):
         from ibm_watson_machine_learning.helpers.connections import DeploymentOutputAssetLocation
         if is_cp4d():
             scoring_params = self.service.run_job(
                 payload=self.data_connections_space_only,
@@ -839,36 +828,27 @@
         assert isinstance(data_join_pipeline._pipeline_json, list)
         assert '40 [label=NumberSet]' in data_join_pipeline._graph.__str__()
 
     #     data_join_pipeline.visualize()
 
     @print_test_separators
     def test_35_batch_deployment_setup_and_preparation_notebook(self):
-        if is_cp4d():
-            TestOBMAndKB.service = Batch(source_wml_credentials=self.wml_credentials.copy(),
-                                         source_project_id=self.project_id,
-                                         target_wml_credentials=self.wml_credentials.copy(),
-                                         target_space_id=self.space_id)
-        else:
-            TestOBMAndKB.service = Batch(self.wml_credentials,
-                                         source_space_id=self.space_id,
-                                         source_project_id=self.project_id,
-                                         target_wml_credentials=self.wml_credentials,
-                                         target_space_id=self.space_id)
+        TestOBMAndKB.service = Batch(source_wml_credentials=self.wml_credentials.copy(),
+                                     source_project_id=self.project_id,
+                                     target_wml_credentials=self.wml_credentials.copy(),
+                                     target_space_id=self.space_id)
 
-        self.wml_client.set.default_space(self.space_id) if self.wml_client.ICP else None
 
     @print_test_separators
     def test_36__deploy__deploy_best_computed_pipeline_from_autoai_on_wml_notebook(self):
         self.service.create(
             metadata=self.metadata,
             model=self.pipeline_name,
             deployment_name=self.DEPLOYMENT_NAME)
 
-        self.wml_client.set.default_project(self.project_id) if self.wml_client.ICP else None
 
     @print_test_separators
     def test_37a_score_deployed_model_notebook(self):
         from ibm_watson_machine_learning.helpers.connections import DeploymentOutputAssetLocation
         if is_cp4d():
             scoring_params = self.service.run_job(
                 payload=self.data_connections_space_only,
```

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_obm_plus_kb_temp_binary.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_obm_plus_kb_temp_binary.py`

 * *Files 6% similar despite different names*

```diff
@@ -110,29 +110,26 @@
 
         if not is_cp4d():
             cls.cos_credentials = get_cos_credentials()
             cls.cos_endpoint = cls.cos_credentials.get('endpoint_url')
             cls.cos_resource_instance_id = cls.cos_credentials.get('resource_instance_id')
 
         cls.wml_client = APIClient(wml_credentials=cls.wml_credentials.copy())
-        cls.project_id = cls.wml_credentials.get('project_id')
+        # cls.project_id = cls.wml_credentials.get('project_id')
 
     @print_test_separators
     def test_00a_space_cleanup(self):
         space_cleanup(self.wml_client,
                       get_space_id(self.wml_client, self.space_name,
                                    cos_resource_instance_id=self.cos_resource_instance_id),
                       days_old=7)
         TestOBMAndKB.space_id = get_space_id(self.wml_client, self.space_name,
                                      cos_resource_instance_id=self.cos_resource_instance_id)
 
-        if self.wml_client.ICP:
-            self.wml_client.set.default_project(self.project_id)
-        else:
-            self.wml_client.set.default_space(self.space_id)
+        self.wml_client.set.default_space(self.space_id)
 
     @print_test_separators
     def test_00b_prepare_COS_instance(self):
         if self.wml_client.ICP or self.wml_client.WSD:
             self.skipTest("Prepare COS is available only for Cloud")
 
         import ibm_boto3
@@ -260,16 +257,15 @@
     # def test_03_data_join_graph_visualization(self):
     #     print("Visualizing data_join_graph...")
     #     self.data_join_graph.visualize()
 
     @print_test_separators
     def test_04_initialize_AutoAI_experiment__pass_credentials__object_initialized(self):
         print("Initializing AutoAI experiment...")
-        TestOBMAndKB.experiment = AutoAI(wml_credentials=self.wml_credentials.copy(),
-                                         project_id=self.project_id,
+        TestOBMAndKB.experiment = AutoAI(wml_credentials=self.wml_credentials,
                                          space_id=self.space_id)
 
         self.assertIsInstance(self.experiment, AutoAI, msg="Experiment is not of type AutoAI.")
 
     @print_test_separators
     def test_05_save_remote_data_and_DataConnection_setup(self):
         print("Writing multiple data files to COS...")
@@ -659,37 +655,28 @@
 
     #################################
     #      DEPLOYMENT SECTION       #
     #################################
 
     @print_test_separators
     def test_26_batch_deployment_setup_and_preparation(self):
-        if is_cp4d():
-            TestOBMAndKB.service = Batch(source_wml_credentials=self.wml_credentials,
-                                         source_project_id=self.project_id,
-                                         target_wml_credentials=self.wml_credentials,
-                                         target_space_id=self.space_id)
-
-        else:
-            TestOBMAndKB.service = Batch(source_wml_credentials=self.wml_credentials,
-                                         source_space_id=self.space_id,
-                                         target_wml_credentials=self.wml_credentials,
-                                         target_space_id=self.space_id)
+        TestOBMAndKB.service = Batch(source_wml_credentials=self.wml_credentials,
+                                     source_space_id=self.space_id,
+                                     target_wml_credentials=self.wml_credentials,
+                                     target_space_id=self.space_id)
 
         self.wml_client.set.default_space(self.space_id) if self.wml_client.ICP else None
 
     @print_test_separators
     def test_27_deploy__deploy_best_computed_pipeline_from_autoai_on_wml(self):
         self.service.create(
             experiment_run_id=self.remote_auto_pipelines._engine._current_run_id,
             model="Pipeline_3",
             deployment_name=self.DEPLOYMENT_NAME)
 
-        self.wml_client.set.default_project(self.project_id) if self.wml_client.ICP else None
-
     @print_test_separators
     def test_28_score_deployed_model(self):
         if is_cp4d():
             payload_reference = self.data_connections_space_only
             output_data_reference = DataConnection(location=DeploymentOutputAssetLocation(name="batch_output_obm.csv"))
         else:
             payload_reference = self.data_connections
@@ -717,15 +704,14 @@
 
     @print_test_separators
     def test_30_delete_deployment(self):
         print("Delete current deployment: {}".format(self.service.deployment_id))
         self.service.delete()
         self.wml_client.set.default_space(self.space_id) if not self.wml_client.default_space_id else None
         self.wml_client.repository.delete(self.service.asset_id)
-        self.wml_client.set.default_project(self.project_id) if is_cp4d() else None
 
     #################################
     #      NOTEBOOK SECTION       #
     #################################
 
     @print_test_separators
     @unittest.skipIf( is_cp4d(), "Flow with notebook metadata works only on WS")
@@ -794,38 +780,29 @@
     #     assert isinstance(data_join_pipeline._pipeline_json, list)
     #     assert '40 [label=NumberSet]' in data_join_pipeline._graph.__str__()
     # #     data_join_pipeline.visualize()
 
     @print_test_separators
     @unittest.skipIf( is_cp4d(), "Flow with notebook metadata works only on WS")
     def test_35_batch_deployment_setup_and_preparation_notebook(self):
-        if is_cp4d():
-            TestOBMAndKB.service = Batch(self.wml_credentials,
-                                         source_project_id=self.project_id,
-                                         target_wml_credentials=self.wml_credentials,
-                                         target_space_id=self.space_id)
-        else:
-            TestOBMAndKB.service = Batch(self.wml_credentials,
-                                         source_space_id=self.space_id,
-                                         source_project_id=self.project_id,
-                                         target_wml_credentials=self.wml_credentials,
-                                         target_space_id=self.space_id)
+        TestOBMAndKB.service = Batch(self.wml_credentials,
+                                     source_space_id=self.space_id,
+                                     target_wml_credentials=self.wml_credentials,
+                                     target_space_id=self.space_id)
 
         self.wml_client.set.default_space(self.space_id) if self.wml_client.ICP else None
 
     @print_test_separators
     @unittest.skipIf( is_cp4d(), "Flow with notebook metadata works only on WS")
     def test_36__deploy__deploy_best_computed_pipeline_from_autoai_on_wml_notebook(self):
         self.service.create(
             metadata=self.metadata,
             model=self.pipeline_name,
             deployment_name=self.DEPLOYMENT_NAME)
 
-        self.wml_client.set.default_project(self.project_id) if self.wml_client.ICP else None
-
     @print_test_separators
     @unittest.skipIf( is_cp4d(), "Flow with notebook metadata works only on WS")
     def test_37a_score_deployed_model_notebook(self):
         if is_cp4d():
             payload_reference = self.data_connections_space_only
             output_data_reference = DataConnection(
                 location=DeploymentOutputAssetLocation(name="batch_output_obm.csv"))
@@ -877,11 +854,10 @@
     @print_test_separators
     @unittest.skipIf(is_cp4d(), "Flow with notebook metadata works only on WS")
     def test_39_delete_deployment_notebook(self):
         print("Delete current deployment: {}".format(self.service.deployment_id))
         self.service.delete()
         self.wml_client.set.default_space(self.space_id) if not self.wml_client.default_space_id else None
         self.wml_client.repository.delete(self.service.asset_id)
-        self.wml_client.set.default_project(self.project_id) if is_cp4d() else None
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_text_transformer_csv_multiclass.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_text_transformer_csv_multiclass.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_text_transformer_csv_regression.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_text_transformer_csv_regression.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_text_transformer_donorchoose_binary.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_text_transformer_donorchoose_binary.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_text_transformer_fake_job_position_binary.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_text_transformer_fake_job_position_binary.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_twitter_wml_autoai_csv_forecasting.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_twitter_wml_autoai_csv_forecasting.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/svt/test_twitter_wml_autoai_csv_forecasting_multivariate.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/svt/test_twitter_wml_autoai_csv_forecasting_multivariate.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/unit/test_auto_pipeline_runs.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/unit/test_auto_pipeline_runs.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/unit/test_check_dependencies_versions.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/unit/test_check_dependencies_versions.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/unit/test_data_connection.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/unit/test_data_connection.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/unit/test_data_join_pipeline_graph.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/unit/test_data_join_pipeline_graph.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/unit/test_get_obm_output.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/unit/test_get_obm_output.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/unit/test_local_auto_pipeline.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/unit/test_local_auto_pipeline.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/unit/test_next_run_details_generator.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/unit/test_next_run_details_generator.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/unit/test_piepeline_to_script.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/unit/test_piepeline_to_script.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/unit/test_prepare_auto_ai_model_to_publish.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/unit/test_prepare_auto_ai_model_to_publish.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/unit/test_prepare_cos_client.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/unit/test_prepare_cos_client.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/autoai/unit/test_tshirt_sizes_limitation.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/autoai/unit/test_tshirt_sizes_limitation.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/deployment/unit/test_batch.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/deployment/unit/test_batch.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/deployment/unit/test_web_service.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/deployment/unit/test_web_service.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/install_requirements.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/install_requirements.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4functions.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4functions.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4pipelines.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4pipelines.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_ai_functions_from_func.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_ai_functions_from_func.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_ai_functions_from_func_sklearn_preprocessing.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_ai_functions_from_func_sklearn_preprocessing.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_ai_functions_from_gz.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_ai_functions_from_gz.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_ai_functions_from_gz_keras.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_ai_functions_from_gz_keras.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_ai_functions_from_gz_mandatory_params.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_ai_functions_from_gz_mandatory_params.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_do_from_tar_gz.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_do_from_tar_gz.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_experiment_and_pipelines.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_experiment_and_pipelines.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_keras_from_file_V4.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_keras_from_file_V4.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_keras_from_object_V4_disable.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_keras_from_object_V4_disable.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_keras_from_tgz.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_keras_from_tgz.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_libraries_experiments.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_libraries_experiments.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_pmml_from_xml.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_pmml_from_xml.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_pytorch_from_tar_gz.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_pytorch_from_tar_gz.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_runtimes_custom_libs.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_runtimes_custom_libs.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_runtimes_custom_libs_attaching_to_model_from_archive.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_runtimes_custom_libs_attaching_to_model_from_archive.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_runtimes_custom_libs_attaching_to_model_from_object.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_runtimes_custom_libs_attaching_to_model_from_object.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_runtimes_custom_libs_delete_orphaned_libs.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_runtimes_custom_libs_delete_orphaned_libs.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_runtimes_custom_libs_yaml_upload.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_runtimes_custom_libs_yaml_upload.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_runtimes_mandatory_params.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_runtimes_mandatory_params.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_scikit_learn_from_directory.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_scikit_learn_from_directory.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_scikit_learn_from_object.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_scikit_learn_from_object.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_scikit_learn_from_tar_gz.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_scikit_learn_from_tar_gz.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_scikit_xgboost_from_directory.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_scikit_xgboost_from_directory.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_scikit_xgboost_from_object.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_scikit_xgboost_from_object.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_scikit_xgboost_from_tar_gz.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_scikit_xgboost_from_tar_gz.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_spaces.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_spaces.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_spark_mllib_from_object.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_spark_mllib_from_object.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_spark_mllib_from_tar_gz.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_spark_mllib_from_tar_gz.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_spss_from_file.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_spss_from_file.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_tensorflow_from_directory.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_tensorflow_from_directory.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_tensorflow_from_file.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_tensorflow_from_file.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_tensorflow_training.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_tensorflow_training.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_training_from_pipeline.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_training_from_pipeline.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_xgboost_from_directory.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_xgboost_from_directory.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_xgboost_from_json.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_xgboost_from_json.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_xgboost_from_object.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_xgboost_from_object.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/V4test_xgboost_from_tar_gz.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/V4test_xgboost_from_tar_gz.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/_test_scikit_learn_grid_search_xgboost_panda_table_disable.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/_test_scikit_learn_grid_search_xgboost_panda_table_disable.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/_test_spark_mllib_from_directory_disable.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/_test_spark_mllib_from_directory_disable.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/cloud_mllib_from_object.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/cloud_mllib_from_object.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/models_preparation.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/models_preparation.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/preparation_and_cleaning.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/preparation_and_cleaning.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/runtimesV4.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/runtimesV4.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_ai_functions_from_func_hitting_scoring_disable.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_ai_functions_from_func_hitting_scoring_disable.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_ai_functions_from_gz_disable.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_ai_functions_from_gz_disable.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_ai_functions_from_wrapper_func_disable.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_ai_functions_from_wrapper_func_disable.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_caffe_experiment_disable.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_caffe_experiment_disable.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_clean_disable.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_clean_disable.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_coreml_from_caffe_200Mb_model_disable.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_coreml_from_caffe_200Mb_model_disable.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_coreml_from_caffe_disable.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_coreml_from_caffe_disable.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_coreml_from_keras_disable.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_coreml_from_keras_disable.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_coreml_from_scikit_disable.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_coreml_from_scikit_disable.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_coreml_from_xgboost_disable.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_coreml_from_xgboost_disable.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_keras_experiment_disable.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_keras_experiment_disable.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_keras_experiment_hpo_disable.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_keras_experiment_hpo_disable.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_keras_experiment_learning_system_disable.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_keras_experiment_learning_system_disable.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_keras_experiment_monitor_metrics_disable.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_keras_experiment_monitor_metrics_disable.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_keras_from_file.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_keras_from_file.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_load_30Mb_model_disable.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_load_30Mb_model_disable.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_pytorch_experiment_disable.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_pytorch_experiment_disable.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_repository_limit_disable.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_repository_limit_disable.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_runtimes_custom_libs_attaching_to_simple_model_v4.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_runtimes_custom_libs_attaching_to_simple_model_v4.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_scikit_learn_from_object_refresh_token_disable.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_scikit_learn_from_object_refresh_token_disable.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_scikit_learn_grid_search_xgboost_numpy_table_disable.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_scikit_learn_grid_search_xgboost_numpy_table_disable.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_spark_mllib_with_learning_system_disable.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_spark_mllib_with_learning_system_disable.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_tensorflow_distributed_ddl_experiment_disable.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_tensorflow_distributed_ddl_experiment_disable.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_tensorflow_distributed_horovod_training_disable.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_tensorflow_distributed_horovod_training_disable.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_tensorflow_distributed_training_disable.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_tensorflow_distributed_training_disable.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_tensorflow_experiment_disable.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_tensorflow_experiment_disable.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_tensorflow_experiment_hpo_disable.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_tensorflow_experiment_hpo_disable.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_tensorflow_experiment_hpo_light_disable.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_tensorflow_experiment_hpo_light_disable.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_tensorflow_experiment_mandatory_params_only_disable.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_tensorflow_experiment_mandatory_params_only_disable.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_tensorflow_experiment_monitor_metrics_disable.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_tensorflow_experiment_monitor_metrics_disable.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_tensorflow_experiment_sync_disable.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_tensorflow_experiment_sync_disable.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_tensorflow_training_mandatory_params_only_disable.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_tensorflow_training_mandatory_params_only_disable.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/svt/test_tensorflow_training_v4_disable.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/svt/test_tensorflow_training_v4_disable.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/utils/cleanup.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/utils/cleanup.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/utils/openshift/cli.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/utils/openshift/cli.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/utils/openshift/prometheusapi.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/utils/openshift/prometheusapi.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/utils/utils.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/utils/utils.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/tests/workspace/unit/test_workspace.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/tests/workspace/unit/test_workspace.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/training.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/training.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,15 +238,15 @@
 
         .. important::
 
             **returns**: Metadata of the training created\n
             **return type**: dict\n
 
         **Examples**
-         Example meta_props for Training run creation in IBM Cloud Pak® for Data for Data version 3.0.1 or above:\n
+         Example meta_props for Training run creation in IBM Cloud Pak® for Data version 3.0.1 or above:\n
          >>> metadata = {
          >>>  client.training.ConfigurationMetaNames.NAME: 'Hand-written Digit Recognition',
          >>>  client.training.ConfigurationMetaNames.DESCRIPTION: 'Hand-written Digit Recognition Training',
          >>>  client.training.ConfigurationMetaNames.PIPELINE: {
          >>>                "id": "4cedab6d-e8e4-4214-b81a-2ddb122db2ab",
          >>>                "rev": "12",
          >>>                "model_type": "string",
```

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/utils/__init__.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/utils/autoai/__init__.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/utils/autoai/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/utils/autoai/connection.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/utils/autoai/connection.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/utils/autoai/enums.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/utils/autoai/enums.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,16 +12,19 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from enum import Enum
 
 __all__ = [
     "ClassificationAlgorithms",
+    "ClassificationAlgorithmsCP4D",
     "RegressionAlgorithms",
+    "RegressionAlgorithmsCP4D",
     "ForecastingAlgorithms",
+    "ForecastingAlgorithmsCP4D",
     "PredictionType",
     "Metrics",
     "Transformers",
     "DataConnectionTypes",
     "RunStateTypes",
     "PipelineTypes",
     "Directions",
@@ -29,38 +32,79 @@
     "MetricsToDirections",
     'PositiveLabelClass',
     'VisualizationTypes'
 ]
 
 
 class ClassificationAlgorithms(Enum):
-    """Classification algorithms that AutoAI could use."""
+    """Classification algorithms that AutoAI could use for IBM Cloud."""
+    EX_TREES = "ExtraTreesClassifierEstimator"
+    GB = "GradientBoostingClassifierEstimator"
+    LGBM = "LGBMClassifierEstimator"
+    LR = "LogisticRegressionEstimator"
+    RF = "RandomForestClassifierEstimator"
+    XGB = "XGBClassifierEstimator"
+    DT = "DecisionTreeClassifierEstimator"
+    SnapDT = "SnapDecisionTreeClassifier"
+    SnapRF = "SnapRandomForestClassifier"
+    SnapSVM = "SnapSVMClassifier",
+    SnapLR = "SnapLogisticRegression"
+
+
+class ClassificationAlgorithmsCP4D(Enum):
+    """Classification algorithms that AutoAI could use for IBM Cloud Pak® for Data(CP4D)."""
     EX_TREES = "ExtraTreesClassifierEstimator"
     GB = "GradientBoostingClassifierEstimator"
     LGBM = "LGBMClassifierEstimator"
     LR = "LogisticRegressionEstimator"
     RF = "RandomForestClassifierEstimator"
     XGB = "XGBClassifierEstimator"
     DT = "DecisionTreeClassifierEstimator"
 
 
 class RegressionAlgorithms(Enum):
-    """Regression algorithms that AutoAI could use."""
+    """Regression algorithms that AutoAI could use for IBM Cloud."""
+    RF = "RandomForestRegressorEstimator"
+    RIDGE = "RidgeEstimator"
+    EX_TREES = "ExtraTreesRegressorEstimator"
+    GB = "GradientBoostingRegressorEstimator"
+    LR = "LinearRegressionEstimator"
+    XGB = "XGBRegressorEstimator"
+    LGBM = "LGBMRegressorEstimator"
+    DT = "DecisionTreeRegressorEstimator"
+    SnapDT = "SnapDecisionTreeRegressor"
+    SnapRF = "SnapRandomForestRegressor"
+    SnapBM = "SnapBoostingMachineRegressor"
+
+
+class RegressionAlgorithmsCP4D(Enum):
+    """Regression algorithms that AutoAI could use for IBM Cloud Pak® for Data(CP4D)."""
     RF = "RandomForestRegressorEstimator"
     RIDGE = "RidgeEstimator"
     EX_TREES = "ExtraTreesRegressorEstimator"
     GB = "GradientBoostingRegressorEstimator"
     LR = "LinearRegressionEstimator"
     XGB = "XGBRegressorEstimator"
     LGBM = "LGBMRegressorEstimator"
     DT = "DecisionTreeRegressorEstimator"
 
 
+class ForecastingAlgorithmsCP4D(Enum):
+    """Forecasting algorithms that AutoAI could use for IBM Cloud."""
+    LR = "LinearRegression"
+    ENSEMBLER = "Ensembler"
+    ARIMA = "ARIMA"
+    HW = "HoltWinters"
+    BATS = "BATS"
+    RF = "RandomForest"
+    SVM = "SVM"
+
+
 class ForecastingAlgorithms(Enum):
-    """Forecasting algorithms that AutoAI could use."""
+    """Forecasting algorithms that AutoAI could use for IBM Cloud Pak® for Data(CP4D)."""
     LR = "LinearRegression"
     ENSEMBLER = "Ensembler"
     ARIMA = "ARIMA"
     HW = "HoltWinters"
     BATS = "BATS"
     RF = "RandomForest"
     SVM = "SVM"
@@ -97,14 +141,15 @@
 
 class Metrics:
     """
         Supported types of classification and regression metrics in autoai.
 
     """
     ACCURACY_SCORE = "accuracy"
+    # ACCURACY_AND_DISPARATE_IMPACT_SCORE = "accuracy_and_disparate_impact" TODO: uncomment to add fairness support
     AVERAGE_PRECISION_SCORE = "average_precision"
     F1_SCORE = "f1"
     LOG_LOSS = "neg_log_loss"
     PRECISION_SCORE = "precision"
     RECALL_SCORE = "recall"
     ROC_AUC_SCORE = "roc_auc"
 
@@ -122,14 +167,15 @@
     MEAN_ABSOLUTE_ERROR = "neg_mean_absolute_error"
     MEAN_SQUARED_ERROR = "neg_mean_squared_error"
     MEAN_SQUARED_LOG_ERROR = "neg_mean_squared_log_error"
     MEDIAN_ABSOLUTE_ERROR = "neg_median_absolute_error"
     ROOT_MEAN_SQUARED_ERROR = "neg_root_mean_squared_error"
     ROOT_MEAN_SQUARED_LOG_ERROR = "neg_root_mean_squared_log_error"
     R2_SCORE = "r2"
+    # R2_AND_DISPARATE_IMPACT_SCORE = "r2_and_disparate_impact" TODO: uncomment to add fairness support
 
 
 class Transformers:
     """
     Supported types of congito transformers names in autoai.
     """
     SQRT = "sqrt"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/utils/autoai/errors.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/utils/autoai/errors.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/utils/autoai/local_training_message_handler.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/utils/autoai/local_training_message_handler.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/utils/autoai/progress_bar.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/utils/autoai/progress_bar.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/utils/autoai/training.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/utils/autoai/training.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/utils/autoai/utils.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/utils/autoai/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,16 @@
 from zipfile import ZipFile
 from collections.abc import Sequence
 
 import pkg_resources
 import requests
 from packaging import version
 
-from .enums import (RegressionAlgorithms, ClassificationAlgorithms, ForecastingAlgorithms, Transformers,
+from .enums import (RegressionAlgorithms, RegressionAlgorithmsCP4D, ClassificationAlgorithms,
+                    ClassificationAlgorithmsCP4D, ForecastingAlgorithms, ForecastingAlgorithmsCP4D, Transformers,
                     Metrics, TShirtSize, PredictionType)
 from .errors import (MissingPipeline, DataFormatNotSupported, LibraryNotCompatible,
                      CannotInstallLibrary, CannotDownloadTrainingDetails, CannotDownloadWMLPipelineDetails,
                      VisualizationFailed, AdditionalParameterIsUnexpected, InvalidSequenceValue, NoAvailableMetrics)
 
 if TYPE_CHECKING:
     from io import BytesIO, BufferedIOBase
@@ -129,25 +130,29 @@
     List of sklearn Pipelines or None if load_pipelines is set to False.
     """
 
     def check_pipeline_nodes(pipeline: dict, request_json: dict, wml_client) -> bool:
         """
         Automate check all pipeline nodes to find xgboost or lightgbm dependency.
         """
+        snapml_estimators = [i.value for i in ClassificationAlgorithms if 'Snap' in i.value] + [
+            i.value for i in RegressionAlgorithms if 'Snap' in i.value]
         xgboost_estimators = ['XGBClassifierEstimator', 'XGBRegressorEstimator', 'XGBClassifier', 'XGBRegressor']
         lightgbm_estimators = ['LGBMClassifierEstimator', 'LGBMRegressorEstimator', 'LGBMClassifier', 'LGBMRegressor']
 
         # note: check dependencies for estimators and other packages
         estimator_name = pipeline['context']['intermediate_model'].get('pipeline_nodes', [None])[-1]
         if estimator_name in xgboost_estimators:
             check_lale = check_dependencies_versions(request_json, wml_client, 'xgboost')
 
         elif estimator_name in lightgbm_estimators:
             check_lale = check_dependencies_versions(request_json, wml_client, 'lightgbm')
 
+        elif estimator_name in snapml_estimators:
+            check_lale = check_dependencies_versions(request_json, wml_client, 'snapml')
         else:
             check_lale = check_dependencies_versions(request_json, wml_client, None)
 
         # TODO: When another package estimators will be available update above!
         # --- end note
 
         return check_lale
@@ -1062,19 +1067,21 @@
                 try:
                     installed_module_version = fallback_to_pip_for_version_check(package)
 
                 except Exception:
                     installed_module_version = pkg_resources.get_distribution(package['name']).version
 
                 # workaround for autai-libs and numpy versions in SW spec
-                if package['name'] == 'autoai-libs' or package['name'] == 'numpy' or package['name'] == 'lale':
+                if package['name'] == 'autoai-libs' or package['name'] == 'numpy' \
+                        or package['name'] == 'lale' or package['name'] == 'snapml':
                     if version.parse(installed_module_version) < version.parse(package['version']):
-                        # we should produce different error for lale as only 2 major numbers are significant
-                        if package['name'] == 'lale' and len(package['version'].split('.')) == 3:
-                            _version = package['version'].split('.')
+                        # we should produce different error for lale and snap_ml as only 2 major numbers are significant
+                        packages_less_strict_error_list = ['lale', 'snapml'],
+                        if package['name'] in packages_less_strict_error_list and len(package['version'].split('.')) >= 3:
+                            _version = package['version'].split('.')[:2]  # take only 3 major version number
                             _version[-1] = 'x'
                             package['version'] = '.'.join(_version)
 
                         errored_packages.append(package)
 
                 else:
                     if installed_module_version != package['version']:
@@ -1139,21 +1146,23 @@
         return cos_client
 
     cos_client_results = None
     data_cos_clients = []
 
     if training_result_reference is not None:
         if (isinstance(training_result_reference.connection, S3Connection) or
-                training_result_reference._check_if_connection_asset_is_s3()):
+                (os.environ.get('USER_ACCESS_TOKEN') is None and
+                 training_result_reference._check_if_connection_asset_is_s3())):
             cos_client_results = (training_result_reference,
                                   differentiate_between_credentials(connection=training_result_reference.connection))
 
     if training_data_references is not None:
         for reference in training_data_references:
-            if isinstance(reference.connection, S3Connection) or reference._check_if_connection_asset_is_s3():
+            if (isinstance(reference.connection, S3Connection) or
+                    (os.environ.get('USER_ACCESS_TOKEN') is None and reference._check_if_connection_asset_is_s3())):
                 data_cos_clients.append((reference,
                                          differentiate_between_credentials(connection=reference.connection)))
 
     return data_cos_clients, cos_client_results
 
 
 def create_summary(details: dict, scoring: str) -> 'DataFrame':
@@ -1478,15 +1487,15 @@
         'train_sample_columns_index_list', 'preprocessor_cat_imp_strategy', 'preprocessor_cat_enc_encoding',
         'preprocessor_num_imp_strategy', 'preprocessor_num_scaler_use_scaler_flag', 'preprocessor_num_scaler_with_mean',
         'preprocessor_num_scaler_with_std', 'preprocessor_string_compress_type', 'FE_drop_unique_columns_flag',
         'FE_drop_constant_columns_flag', 'FE_add_frequency_columns_flag', 'FE_add_missing_indicator_columns_flag',
         'data_provenance', 'target_label_name', 'preprocessor_data_filename', 'cognito_data_filename',
         'holdout_roc_curve_max_size', 'holdout_reg_pred_obs_max_size', 'max_estimator_n_jobs',
         'enabled_feature_engineering_as_json', 'fairness_info', 'text_processing', 'word2vec_feature_number',
-        '_enable_snapml_estimators'
+        '_enable_snapml_estimators','return_holdout_indices', 'retrain_pipelines_on_holdout_data'
     ]
 
     for k in params:
         if k not in expected_params:
             raise AdditionalParameterIsUnexpected(k)
 
 
@@ -1574,15 +1583,16 @@
                                                  RegressionAlgorithms,
                                                  ForecastingAlgorithms]],
         include_only_estimators: List[Union[ClassificationAlgorithms,
                                                  RegressionAlgorithms,
                                                  ForecastingAlgorithms]],
         cognito_transform_names: List[Transformers],
         scoring: str,
-        t_shirt_size: str) -> None:
+        t_shirt_size: str,
+        is_cpd = False) -> None:
     """
     Validate if passed optimizer variables takes values from defined enums.
 
     Parameters
     ----------
     prediction_type: str
         Type of the prediction.
@@ -1592,25 +1602,35 @@
         List of estimators.
     cognito_transform_names: list
         List of transformers.
     scoring: str
         Type of the metric to optimize with.
     t_shirt_size: str
         The size of the remote AutoAI POD instance.
+    is_cpd: bool
+        True if run on CP4D environment. CP4D estimators will be used to check.
 
     Raises
     ------
     InvalidSequenceValue, If element is not from enum class values.
     """
-    if prediction_type == PredictionType.REGRESSION:
-        estimators_enum = RegressionAlgorithms
-    elif prediction_type == PredictionType.FORECASTING:
-        estimators_enum = ForecastingAlgorithms
+    if is_cpd:
+        if prediction_type == PredictionType.REGRESSION:
+            estimators_enum = RegressionAlgorithmsCP4D
+        elif prediction_type == PredictionType.FORECASTING:
+            estimators_enum = ForecastingAlgorithmsCP4D
+        else:
+            estimators_enum = ClassificationAlgorithmsCP4D
     else:
-        estimators_enum = ClassificationAlgorithms
+        if prediction_type == PredictionType.REGRESSION:
+            estimators_enum = RegressionAlgorithms
+        elif prediction_type == PredictionType.FORECASTING:
+            estimators_enum = ForecastingAlgorithms
+        else:
+            estimators_enum = ClassificationAlgorithms
     for (sequence, enum_class) in (
             ([prediction_type], PredictionType),
             (daub_include_only_estimators, estimators_enum),
             (include_only_estimators, estimators_enum),
             (cognito_transform_names, Transformers),
             ([t_shirt_size], TShirtSize)):
         is_list_composed_from_enum(sequence, enum_class)
```

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/utils/autoai/watson_studio.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/utils/autoai/watson_studio.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/utils/autoai/wsd_ui.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/utils/autoai/wsd_ui.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/utils/deployment/__init__.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/utils/deployment/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/utils/deployment/errors.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/utils/deployment/errors.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/utils/utils.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/utils/utils.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/volumes.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/volumes.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/wml_client_error.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/wml_client_error.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/wml_resource.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/wml_resource.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/workspace/__init__.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/workspace/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning/workspace/workspace.py` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning/workspace/workspace.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning.egg-info/PKG-INFO` & `ibm_watson_machine_learning-1.0.99/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ibm-watson-machine-learning
-Version: 1.0.96
+Name: ibm_watson_machine_learning
+Version: 1.0.99
 Summary: IBM Watson Machine Learning API Client
 Home-page: http://ibm-wml-api-pyclient.mybluemix.net
 Author: IBM
 Author-email: svagaral@in.ibm.com, kaganesa@in.ibm.com, vbmithun@in.ibm.com, amadeusz.masny1@ibm.com
 License: BSD
 Description: ******************************************
         ## Welcome to `ibm-watson-machine-learning`
@@ -18,14 +18,15 @@
         
 Keywords: watson,machine learning,IBM,Bluemix,client,API,IBM Cloud
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `ibm_watson_machine_learning-1.0.96/ibm_watson_machine_learning.egg-info/SOURCES.txt` & `ibm_watson_machine_learning-1.0.99/ibm_watson_machine_learning.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -353,14 +353,18 @@
 ibm_watson_machine_learning/libs/repo/util/exceptions.py
 ibm_watson_machine_learning/libs/repo/util/file_system_ops.py
 ibm_watson_machine_learning/libs/repo/util/generic_archive_file_check.py
 ibm_watson_machine_learning/libs/repo/util/json_2_object_mapper.py
 ibm_watson_machine_learning/libs/repo/util/library_imports.py
 ibm_watson_machine_learning/libs/repo/util/spark_util.py
 ibm_watson_machine_learning/libs/repo/util/unique_id_gen.py
+ibm_watson_machine_learning/messages/__init__.py
+ibm_watson_machine_learning/messages/globalization_util.py
+ibm_watson_machine_learning/messages/messages.py
+ibm_watson_machine_learning/messages/messages_en.json
 ibm_watson_machine_learning/preprocessing/__init__.py
 ibm_watson_machine_learning/preprocessing/data_join_pipeline.py
 ibm_watson_machine_learning/preprocessing/multiple_files_preprocessor.py
 ibm_watson_machine_learning/preprocessing/templates/__init__.py
 ibm_watson_machine_learning/preprocessing/templates/pretty_print_template.py
 ibm_watson_machine_learning/tests/ConfigFileEncoder.py
 ibm_watson_machine_learning/tests/ConfigFileGenerator.py
@@ -477,21 +481,27 @@
 ibm_watson_machine_learning/tests/autoai/fvt/test_xlsx_read_binary_regression.py
 ibm_watson_machine_learning/tests/autoai/manual/__init__.py
 ibm_watson_machine_learning/tests/autoai/manual/test_bank_binary.py
 ibm_watson_machine_learning/tests/autoai/svt/__init__.py
 ibm_watson_machine_learning/tests/autoai/svt/abstract_test_iris_using_database_connection.py
 ibm_watson_machine_learning/tests/autoai/svt/abstract_test_iris_using_database_data_asset.py
 ibm_watson_machine_learning/tests/autoai/svt/abstract_test_iris_wml_autoai_multiclass_connections.py
+ibm_watson_machine_learning/tests/autoai/svt/test_arabicghosts_multiclass_snapml.py
+ibm_watson_machine_learning/tests/autoai/svt/test_auth.py
 ibm_watson_machine_learning/tests/autoai/svt/test_bank_wml_autoai_xlsx_binary.py
 ibm_watson_machine_learning/tests/autoai/svt/test_breast_cancer_wml_autoai_csv_binary.py
 ibm_watson_machine_learning/tests/autoai/svt/test_breast_cancer_wml_autoai_csv_binary_apikey_auth.py
 ibm_watson_machine_learning/tests/autoai/svt/test_breast_cancer_wml_autoai_csv_binary_token_auth.py
 ibm_watson_machine_learning/tests/autoai/svt/test_car_price_wml_autoai_regression.py
 ibm_watson_machine_learning/tests/autoai/svt/test_credit_risk_as_sample_notebook_binary.py
+ibm_watson_machine_learning/tests/autoai/svt/test_credit_risk_binary_snapml.py
 ibm_watson_machine_learning/tests/autoai/svt/test_drop_duplicates.py
+ibm_watson_machine_learning/tests/autoai/svt/test_drug_fairnessmetric_autoai_multiclass.py
+ibm_watson_machine_learning/tests/autoai/svt/test_housing_reegression_snapml.py
+ibm_watson_machine_learning/tests/autoai/svt/test_insurance_fairnessmetric_autoai_regression.py
 ibm_watson_machine_learning/tests/autoai/svt/test_insurance_wml_autoai_xlsx_regression.py
 ibm_watson_machine_learning/tests/autoai/svt/test_iris_using_data_asset_and_connected_asset.py
 ibm_watson_machine_learning/tests/autoai/svt/test_iris_using_data_asset_and_default.py
 ibm_watson_machine_learning/tests/autoai/svt/test_iris_using_data_connected_asset_and_connected_asset.py
 ibm_watson_machine_learning/tests/autoai/svt/test_iris_using_data_connected_asset_and_default.py
 ibm_watson_machine_learning/tests/autoai/svt/test_iris_using_data_connected_asset_and_s3.py
 ibm_watson_machine_learning/tests/autoai/svt/test_iris_using_data_s3_and_connected_asset.py
@@ -667,25 +677,29 @@
 ibmfl/model/naive_bayes_fl_model.py
 ibmfl/model/pytorch_fl_model.py
 ibmfl/model/sklearn_SGD_linear_fl_model.py
 ibmfl/model/sklearn_fl_model.py
 ibmfl/model/sklearn_kmeans_fl_model.py
 ibmfl/model/tensorflow_fl_model.py
 ibmfl/model/xgb_fl_model.py
+ibmfl/model/v2/__init__.py
+ibmfl/model/v2/xgb_fl_model.py
 ibmfl/party/__init__.py
 ibmfl/party/party.py
 ibmfl/party/party_protocol_handler.py
 ibmfl/party/status_type.py
 ibmfl/party/metrics/__init__.py
 ibmfl/party/metrics/metrics_recorder.py
 ibmfl/party/training/__init__.py
 ibmfl/party/training/fedavg_local_training_handler.py
 ibmfl/party/training/local_training_handler.py
 ibmfl/party/training/pfnm_local_training_handler.py
 ibmfl/party/training/xgboost_local_training_handler.py
+ibmfl/party/training/v2/__init__.py
+ibmfl/party/training/v2/xgboost_local_training_handler.py
 ibmfl/util/__init__.py
 ibmfl/util/config.py
 ibmfl/util/fl_metrics.py
 ibmfl/util/log_config.py
 ibmfl/util/pfnm/__init__.py
 ibmfl/util/pfnm/core.py
 ibmfl/util/pfnm/matching.py
```

### Comparing `ibm_watson_machine_learning-1.0.96/ibmfl/connection/connection.py` & `ibm_watson_machine_learning-1.0.99/ibmfl/connection/connection.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibmfl/connection/route_declarations.py` & `ibm_watson_machine_learning-1.0.99/ibmfl/connection/route_declarations.py`

 * *Files 16% similar despite different names*

```diff
@@ -72,30 +72,10 @@
     :return: None
     """
     router.add_routes({
         '{}'.format(MessageType.TRAIN.value): party_proto_handler.handle_async_request,
         '{}'.format(MessageType.SAVE_MODEL.value): party_proto_handler.handle_request,
         '{}'.format(MessageType.EVAL_MODEL.value): party_proto_handler.handle_request,
         '{}'.format(MessageType.SYNC_MODEL.value): party_proto_handler.handle_request,
-        '{}'.format(
-            MessageType.DECRYPT_FUSED.value): party_proto_handler.handle_request,
         '{}'.format(MessageType.STOP.value): party_proto_handler.handle_request,
         'default': default_end_point
     })
-
-
-def get_authority_router(router, authority_proto_handler):
-    """
-    Route for authority party
-
-    :param router: Router object
-    :type router: `Router`
-    :param authority_proto_handler: ProtoHandler object
-    :type authority_proto_handler: `ProtoHandler`
-    :return: None
-    """
-    router.add_routes({
-        '{}'.format(MessageType.PUBLIC_PARAMETER.value): authority_proto_handler.handle_request_public_parameter,
-        '{}'.format(MessageType.SECRET_KEY.value): authority_proto_handler.handle_request_secret_key,
-        '{}'.format(MessageType.DECRYPT_KEY.value): authority_proto_handler.handle_request_decrypt_key,
-        'default': default_end_point
-    })
```

### Comparing `ibm_watson_machine_learning-1.0.96/ibmfl/connection/router_handler.py` & `ibm_watson_machine_learning-1.0.99/ibmfl/connection/router_handler.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibmfl/connection/websockets_connection.py` & `ibm_watson_machine_learning-1.0.99/ibmfl/connection/websockets_connection.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibmfl/data/data_handler.py` & `ibm_watson_machine_learning-1.0.99/ibmfl/data/data_handler.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibmfl/data/data_util.py` & `ibm_watson_machine_learning-1.0.99/ibmfl/data/data_util.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibmfl/data/env_data_handler.py` & `ibm_watson_machine_learning-1.0.99/ibmfl/data/env_data_handler.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibmfl/data/env_spec.py` & `ibm_watson_machine_learning-1.0.99/ibmfl/data/env_spec.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibmfl/data/pandas_data_handler.py` & `ibm_watson_machine_learning-1.0.99/ibmfl/data/pandas_data_handler.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibmfl/envs.py` & `ibm_watson_machine_learning-1.0.99/ibmfl/envs.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibmfl/exceptions.py` & `ibm_watson_machine_learning-1.0.99/ibmfl/exceptions.py`

 * *Files 7% similar despite different names*

```diff
@@ -63,14 +63,22 @@
     pass
 
 
 class CryptoException(FLException):
     pass
 
 
+class AuthorityException(FLException):
+    pass
+
+
+class KeyManagerException(FLException):
+    pass
+
+
 class WarmStartException(FLException):
     pass
 
 
 class FusionException(FLException):
     pass
```

### Comparing `ibm_watson_machine_learning-1.0.96/ibmfl/message/json_serializer.py` & `ibm_watson_machine_learning-1.0.99/ibmfl/message/json_serializer.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibmfl/message/message.py` & `ibm_watson_machine_learning-1.0.99/ibmfl/message/message.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibmfl/message/message_type.py` & `ibm_watson_machine_learning-1.0.99/ibmfl/message/message_type.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,13 +27,9 @@
     REGISTER = 6
     TRAIN = 7
     SAVE_MODEL = 8
     PREDICT_MODEL = 9
     EVAL_MODEL = 10
     ACK = 11
     SYNC_MODEL = 12
-    DECRYPT_FUSED = 13
     STOP = 14
-    PUBLIC_PARAMETER = 15
-    SECRET_KEY = 16
-    DECRYPT_KEY = 17
     ERROR_AUTH = 400
```

### Comparing `ibm_watson_machine_learning-1.0.96/ibmfl/message/pickle_serializer.py` & `ibm_watson_machine_learning-1.0.99/ibmfl/message/pickle_serializer.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibmfl/message/serializer.py` & `ibm_watson_machine_learning-1.0.99/ibmfl/message/serializer.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibmfl/message/serializer_factory.py` & `ibm_watson_machine_learning-1.0.99/ibmfl/message/serializer_factory.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibmfl/model/fl_model.py` & `ibm_watson_machine_learning-1.0.99/ibmfl/model/fl_model.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibmfl/model/model_update.py` & `ibm_watson_machine_learning-1.0.99/ibmfl/model/model_update.py`

 * *Files 11% similar despite different names*

```diff
@@ -62,7 +62,18 @@
         if key not in self.__updates:
             logger.error("Key "+key+" not found in model updates")
             raise ModelUpdateException(
                 "Invalid key was requested from model update")
 
         ret_val = loads(self.__updates[key])
         return ret_val
+
+    def exist_key(self, key):
+        """
+        Check if a specified key is used in model update dictionary
+
+        :param key: Identifier which represents the update
+        :type key: `str`
+        :return: check result of existing the key
+        :rtype: True or False
+        """
+        return True if key in self.__updates else False
```

### Comparing `ibm_watson_machine_learning-1.0.96/ibmfl/model/naive_bayes_fl_model.py` & `ibm_watson_machine_learning-1.0.99/ibmfl/model/naive_bayes_fl_model.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibmfl/model/pytorch_fl_model.py` & `ibm_watson_machine_learning-1.0.99/ibmfl/model/pytorch_fl_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -395,14 +395,15 @@
         f_history = None
         if optimizer_filename is not None:
             f_optimizer = super().get_model_absolute_path(optimizer_filename)
         if history_filename is not None:
             f_history = super().get_model_absolute_path(history_filename)
         self.model.save_params(
             f_params=f_params, f_optimizer=f_optimizer, f_history=f_history)
+        return filename
 
     def load_model(self, pytorch_module, model_filename, optimizer_filename=None, history_filename=None, optimizer=None,
                    module_init_params=None):
         """
         Loads a model from disk given the specified file_name
 
         :param pytorch_module: uninstantiated pytorch model class
```

### Comparing `ibm_watson_machine_learning-1.0.96/ibmfl/model/sklearn_SGD_linear_fl_model.py` & `ibm_watson_machine_learning-1.0.99/ibmfl/model/sklearn_SGD_linear_fl_model.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibmfl/model/sklearn_fl_model.py` & `ibm_watson_machine_learning-1.0.99/ibmfl/model/sklearn_fl_model.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibmfl/model/sklearn_kmeans_fl_model.py` & `ibm_watson_machine_learning-1.0.99/ibmfl/model/sklearn_kmeans_fl_model.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibmfl/model/tensorflow_fl_model.py` & `ibm_watson_machine_learning-1.0.99/ibmfl/model/tensorflow_fl_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -296,15 +296,15 @@
         :param filename: Name of the file where to store the model.
         :type filename: `str`
         :return: filename
         :rtype `string`
         """
         if filename is None:
             file = self.model_name if self.model_name else self.model_type
-            filename = '{}_{}'.format(file, time.time())
+            filename = '{}'.format(file)
 
         full_path = super().get_model_absolute_path(filename)
         self.model.save(full_path)
         logger.info('Model saved in path: %s.', full_path)
         return filename
 
     @staticmethod
```

### Comparing `ibm_watson_machine_learning-1.0.96/ibmfl/model/xgb_fl_model.py` & `ibm_watson_machine_learning-1.0.99/ibmfl/model/xgb_fl_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -356,16 +356,16 @@
         enc_y = lab_enc.fit_transform(y).astype(np.float64, copy=False)
 
         # Extract Encoded Target Sizes
         self.classes_ = lab_enc.classes_
         if self.classes_.shape[0] != self.num_classes:
             raise ValueError('Number of classes defined in configuration file '
                              'and the classes derived from the data does not '
-                             'match. Found %d classes, while config file '
-                             'is defined as %d classes.'.format(
+                             'match. Found {0} classes, while config file '
+                             'is defined as {1} classes.'.format(
                              self.classes_.shape[0], self.num_classes))
 
         if self.loss == 'auto':
             self.n_trees = 1 if self.classes_.shape[0] <= 2 else self.classes_.shape[0]
         else:
             self.n_trees = 1 if self.num_classes <= 2 else self.num_classes
```

### Comparing `ibm_watson_machine_learning-1.0.96/ibmfl/party/metrics/metrics_recorder.py` & `ibm_watson_machine_learning-1.0.99/ibmfl/party/metrics/metrics_recorder.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibmfl/party/party.py` & `ibm_watson_machine_learning-1.0.99/ibmfl/party/party.py`

 * *Files 15% similar despite different names*

```diff
@@ -45,25 +45,40 @@
         either a yaml file or a dictionary.
         :param config_file: path to yml file with the configuration of the party
         :type config_file: `str`
         :param config_dict: dictionary containing the configuration of the party
         :type config_dict: `dict`
         :return None
         """
+        self.isCloud = False
+        self.isXGB = False
         log_level = kwargs.get('log_level', 'INFO')
         configure_logging_from_file(log_level=log_level)
 
         config_file = kwargs.get('config_file')
         config_dict = kwargs.get('config_dict')
         if config_file != None: 
             config_dict = fl_config.read_yaml_config(config_file=config_file)
 
         config_dict['connection']['name'] = 'WSConnection'
         config_dict['connection']['path'] = 'ibmfl.connection.websockets_connection'
+
+        if config_dict.get('aggregator', None) is not None:
+            if config_dict.get('aggregator').get('ip', None) is not None:
+                if "cloud.ibm.com" in config_dict.get('aggregator').get('ip'):
+                    self.isCloud = True       
+                    if config_dict.get('local_training', None) is not None:
+                        if config_dict.get('local_training').get('path', None) is not None:
+                            if "ibmfl.party.training.xgboost_local_training_handler" in config_dict.get('local_training').get('path'):
+                                self.isXGB = True
+                                config_dict['local_training']['path'] = 'ibmfl.party.training.v2.xgboost_local_training_handler'
         
+        logger.info("IS CLOUD = " + str(self.isCloud))
+        logger.info("IS XGB = " + str(self.isXGB))
+
         cls_config = fl_config.get_cls_by_config(config_dict)
 
         self.party_config = cls_config
 
         self.data_handler = None
         self.fl_model = None
         self.is_running = False
@@ -131,19 +146,29 @@
 
 
     def initialize_model_config(self):
         logger.info('Initializing model configuration')
         cls_config = self.party_config
         model_config = cls_config.get('model')
         lt_config = cls_config.get('local_training')
+
         try:
             
             # Read and create model (optional field)
             # In some cases aggregator doesn't need to load the model:
             model_cls_ref = model_config.get('cls_ref')
+            if self.isCloud and self.isXGB:
+                previous_cls_ref = fl_config.get_class_by_name("ibmfl.model.xgb_fl_model", "XGBClassifierFLModel")
+                if model_cls_ref == previous_cls_ref:
+                    model_cls_ref = fl_config.get_class_by_name("ibmfl.model.v2.xgb_fl_model", "XGBClassifierFLModel")
+                else:
+                    previous_cls_ref = fl_config.get_class_by_name("ibmfl.model.xgb_fl_model", "XGBRegressorFLModel")
+                    if model_cls_ref == previous_cls_ref:
+                        model_cls_ref = fl_config.get_class_by_name("ibmfl.model.v2.xgb_fl_model", "XGBRegressorFLModel")
+
             spec = model_config.get('spec')
             self.fl_model = model_cls_ref('', spec)
 
             # Load hyperparams
             self.hyperparams = cls_config.get('hyperparams')
 
             lt_cls_ref = lt_config.get('cls_ref')
@@ -182,14 +207,16 @@
                     logger.info('Registration Successful')
                     returnValue = True
                 else:
                     logger.info('Registration Failed: Model processing error')
                     returnValue = False
             else:
                 logger.error('Registration Failed: Failure status from aggregator')
+                if response is not None:
+                    logger.error(response.get_data().get('detail', "No Detail Provided"))
         except Exception as ex:
             logger.error("Error occurred during registration" + str(ex))
 
         return returnValue
 
     def stop_connection(self):
         """
@@ -233,14 +260,16 @@
 
         if not self.is_running:
             logger.info('Party not registered yet.')
             if self.register_party():
                 logger.info('Listening for commands from Aggregator')
                 self.is_running = True
                 self.initialize_model_config()
+            else:
+                self.stop_connection()
         else:
             logger.info('Party already running.')
 
     def extract_model_from_stream(self, data):
         """Read model from response stream and extract the content.
         :param data: response data recieved from aggregator.
         :type data: `json` 
@@ -314,15 +343,15 @@
     parser = argparse.ArgumentParser(
         description='WML Federated Learning Party')
     parser.add_argument('config_file', help='yaml configuration file')
     parser.add_argument('token', help='authentication token')
     parser.add_argument('-s', '--self_signed_cert', help='flag for self-signed certificate', action='store_true')
     parser.add_argument('-i', '--interactive',
                         help='run interactively', action='store_true')
-    parser.add_argument('log_level', type=str, default="INFO", required=False,
+    parser.add_argument('-l', '--log_level', type=str, default="INFO", required=False,
                         help='log_level should be a value from [DEBUG, INFO, WARNING, ERROR, CRITICAL]')
     args = parser.parse_args()
 
     if (args.self_signed_cert):
         self_signed_cert_arg = True
     else:
         self_signed_cert_arg = None
```

### Comparing `ibm_watson_machine_learning-1.0.96/ibmfl/party/party_protocol_handler.py` & `ibm_watson_machine_learning-1.0.99/ibmfl/party/party_protocol_handler.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibmfl/party/status_type.py` & `ibm_watson_machine_learning-1.0.99/ibmfl/party/status_type.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibmfl/party/training/fedavg_local_training_handler.py` & `ibm_watson_machine_learning-1.0.99/ibmfl/party/training/fedavg_local_training_handler.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibmfl/party/training/local_training_handler.py` & `ibm_watson_machine_learning-1.0.99/ibmfl/party/training/local_training_handler.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibmfl/party/training/pfnm_local_training_handler.py` & `ibm_watson_machine_learning-1.0.99/ibmfl/party/training/pfnm_local_training_handler.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibmfl/party/training/xgboost_local_training_handler.py` & `ibm_watson_machine_learning-1.0.99/ibmfl/party/training/xgboost_local_training_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -408,16 +408,16 @@
         enc_y = lab_enc.fit_transform(y).astype(np.float64, copy=False)
 
         # Extract Encoded Target Sizes
         self.classes_ = lab_enc.classes_
         if self.classes_.shape[0] != self.num_classes:
             raise ValueError('Number of classes defined in configuration file '
                              'and the classes derived from the data does not '
-                             'match. Found %d classes, while config file '
-                             'is defined as %d classes.'.format(
+                             'match. Found {0} classes, while config file '
+                             'is defined as {1} classes.'.format(
                              self.classes_.shape[0], self.num_classes))
 
         if self.loss == 'auto':
             self.n_trees = 1 if self.classes_.shape[0] <= 2 else self.classes_.shape[0]
         else:
             self.n_trees = 1 if self.num_classes <= 2 else self.num_classes
```

### Comparing `ibm_watson_machine_learning-1.0.96/ibmfl/util/config.py` & `ibm_watson_machine_learning-1.0.99/ibmfl/util/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,14 +189,15 @@
     cls_config['hyperparams'] = config_dict.get('hyperparams')
     cls_config['aggregator'] = config_dict.get('aggregator')
     cls_config['local_training'] = get_lt_from_config(
         config_dict.get('local_training'))
     cls_config['privacy'] = config_dict.get('privacy')
     cls_config['metrics'] = get_mh_from_config(config_dict.get('metrics'))
     cls_config['key_generators'] = config_dict.get('key_generators')
+    cls_config['access_white_lst'] = config_dict.get('access_white_lst')
 
     return cls_config
 
 
 def get_connection_from_config(config):
     """ Load connection class information from params provided in config file
     :param config: dictionary of configuration
```

### Comparing `ibm_watson_machine_learning-1.0.96/ibmfl/util/fl_metrics.py` & `ibm_watson_machine_learning-1.0.99/ibmfl/util/fl_metrics.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibmfl/util/log_config.py` & `ibm_watson_machine_learning-1.0.99/ibmfl/util/log_config.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibmfl/util/pfnm/core.py` & `ibm_watson_machine_learning-1.0.99/ibmfl/util/pfnm/core.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibmfl/util/pfnm/matching.py` & `ibm_watson_machine_learning-1.0.99/ibmfl/util/pfnm/matching.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibmfl/util/pfnm/utils.py` & `ibm_watson_machine_learning-1.0.99/ibmfl/util/pfnm/utils.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibmfl/util/xgboost/export.py` & `ibm_watson_machine_learning-1.0.99/ibmfl/util/xgboost/export.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/ibmfl/util/xgboost/hyperparams.py` & `ibm_watson_machine_learning-1.0.99/ibmfl/util/xgboost/hyperparams.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         # Global Hyperparameter Check
         if 'global' in hyperparams:
             params = hyperparams['global']
         else:
             raise ValueError('Global parameters have not been defined.')
 
         if 'learning_rate' in params:
-            if params['learning_rate'] < 0:
+            if params['learning_rate'] <= 0:
                 raise ValueError('learning_rate={} must be strictly '
                                  'positive'.format(params['learning_rate']))
         else:
             raise ValueError('learning_rate has not been defined.')
 
         if 'loss' in params:
             if params['loss'] not in VALID_LOSSES:
@@ -94,17 +94,17 @@
             if params['max_iter'] < 1:
                 raise ValueError('max_iter={} must not be smaller '
                                  'than 1.'.format(params['max_iter']))
         else:
             raise ValueError('max_iter has not been defined.')
 
         if 'max_depth' in params:
-            if params['max_depth'] is not None and params['max_depth'] <= 1:
+            if params['max_depth'] is not None and params['max_depth'] < 0:
                 raise ValueError('max_depth={} must be strictly greater'
-                                 'than 1.'.format(params['max_leaf_nodes']))
+                                 'than 0.'.format(params['max_depth']))
 
         if 'max_leaf_nodes' in params:
             if params['max_leaf_nodes'] is not None and params['max_leaf_nodes'] <= 1:
                 raise ValueError('max_leaf_nodes={} must be strictly greater'
                                  'than 1.'.format(params['max_leaf_nodes']))
 
         if 'min_samples_leaf' in params:
```

### Comparing `ibm_watson_machine_learning-1.0.96/ibmfl/util/xgboost/utils.py` & `ibm_watson_machine_learning-1.0.99/ibmfl/util/xgboost/utils.py`

 * *Files identical despite different names*

### Comparing `ibm_watson_machine_learning-1.0.96/setup.py` & `ibm_watson_machine_learning-1.0.99/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,28 +38,30 @@
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='BSD',
     classifiers=['Development Status :: 5 - Production/Stable',
                  'Natural Language :: English',
                  'License :: OSI Approved :: BSD License',
                  'Programming Language :: Python :: 3.7',
+                 'Programming Language :: Python :: 3.8',
                  'Operating System :: MacOS :: MacOS X',
                  'Operating System :: POSIX :: Linux',
                  'Operating System :: Microsoft :: Windows',
                  'Intended Audience :: Science/Research',
                  'Intended Audience :: Developers',
                  'Intended Audience :: Information Technology',
                  'Topic :: Software Development :: Libraries',
                  'Topic :: Software Development :: Libraries :: Python Modules',
                  'Topic :: Scientific/Engineering :: Artificial Intelligence',
                  'Topic :: Scientific/Engineering :: Information Analysis',
                  'Topic :: Internet'],
     keywords=["watson", "machine learning", "IBM", "Bluemix", "client", "API", "IBM Cloud"],
     url='http://ibm-wml-api-pyclient.mybluemix.net',
     packages=find_packages(),
+    package_data={'': ['messages/messages_en.json']},
     install_requires=[
         'requests',
         'urllib3',
         'pandas<1.3.0,>=0.24.2',
         'certifi',
         'lomond',
         'tabulate',
```

