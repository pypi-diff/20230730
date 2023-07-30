# Comparing `tmp/data_ecosystem_services-202307.0.8.tar.gz` & `tmp/data_ecosystem_services-202307.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_ecosystem_services-202307.0.8.tar", max compression
+gzip compressed data, was "data_ecosystem_services-202307.0.9.tar", max compression
```

## Comparing `data_ecosystem_services-202307.0.8.tar` & `data_ecosystem_services-202307.0.9.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0      918 2023-07-25 19:38:09.834920 data_ecosystem_services-202307.0.8/data_ecosystem_services/__main__.py
--rw-r--r--   0        0        0     1264 2023-07-25 19:38:09.834920 data_ecosystem_services-202307.0.8/data_ecosystem_services/alation_service/__init__.py
--rw-r--r--   0        0        0     5030 2023-07-25 19:38:09.834920 data_ecosystem_services-202307.0.8/data_ecosystem_services/alation_service/column.py
--rw-r--r--   0        0        0    25117 2023-07-25 19:38:09.834920 data_ecosystem_services-202307.0.8/data_ecosystem_services/alation_service/customfieldsendpoint.py
--rw-r--r--   0        0        0    13816 2023-07-25 19:38:09.834920 data_ecosystem_services-202307.0.8/data_ecosystem_services/alation_service/datasource.py
--rw-r--r--   0        0        0     2037 2023-07-25 19:38:09.834920 data_ecosystem_services-202307.0.8/data_ecosystem_services/alation_service/endpoint.py
--rw-r--r--   0        0        0    13626 2023-07-25 19:38:09.834920 data_ecosystem_services-202307.0.8/data_ecosystem_services/alation_service/excelmetadata.py
--rw-r--r--   0        0        0      566 2023-07-25 19:38:09.834920 data_ecosystem_services-202307.0.8/data_ecosystem_services/alation_service/execution_session.py
--rw-r--r--   0        0        0     7568 2023-07-25 19:38:09.834920 data_ecosystem_services-202307.0.8/data_ecosystem_services/alation_service/idfinderendpoint.py
--rw-r--r--   0        0        0    16676 2023-07-25 19:38:09.834920 data_ecosystem_services-202307.0.8/data_ecosystem_services/alation_service/manifest.py
--rw-r--r--   0        0        0    10973 2023-07-25 19:38:09.834920 data_ecosystem_services-202307.0.8/data_ecosystem_services/alation_service/query.py
--rw-r--r--   0        0        0    55259 2023-07-25 19:38:09.834920 data_ecosystem_services-202307.0.8/data_ecosystem_services/alation_service/schema.py
--rw-r--r--   0        0        0     7368 2023-07-25 19:38:09.834920 data_ecosystem_services-202307.0.8/data_ecosystem_services/alation_service/table.py
--rw-r--r--   0        0        0     1486 2023-07-25 19:38:09.834920 data_ecosystem_services-202307.0.8/data_ecosystem_services/alation_service/tagsendpoint.py
--rw-r--r--   0        0        0    25982 2023-07-25 19:38:09.834920 data_ecosystem_services-202307.0.8/data_ecosystem_services/alation_service/tokenendpoint.py
--rw-r--r--   0        0        0     1044 2023-07-25 19:38:09.834920 data_ecosystem_services-202307.0.8/data_ecosystem_services/az_client_service/__init__.py
--rw-r--r--   0        0        0       41 2023-07-25 19:38:09.834920 data_ecosystem_services-202307.0.8/data_ecosystem_services/az_client_service/az_client.py
--rw-r--r--   0        0        0     4570 2023-07-25 19:38:09.834920 data_ecosystem_services-202307.0.8/data_ecosystem_services/az_client_service/azd_client.py
--rw-r--r--   0        0        0     1050 2023-07-25 19:38:09.834920 data_ecosystem_services-202307.0.8/data_ecosystem_services/az_key_vault_service/__init__.py
--rw-r--r--   0        0        0     8967 2023-07-25 19:38:09.834920 data_ecosystem_services-202307.0.8/data_ecosystem_services/az_key_vault_service/az_key_vault.py
--rw-r--r--   0        0        0     1073 2023-07-25 19:38:09.834920 data_ecosystem_services-202307.0.8/data_ecosystem_services/az_storage_service/__init__.py
--rw-r--r--   0        0        0     2665 2023-07-25 19:38:09.834920 data_ecosystem_services-202307.0.8/data_ecosystem_services/az_storage_service/az_storage_queue.py
--rw-r--r--   0        0        0     1024 2023-07-25 19:38:09.834920 data_ecosystem_services-202307.0.8/data_ecosystem_services/cdc_admin_service/__init__.py
--rw-r--r--   0        0        0    15940 2023-07-25 19:38:09.834920 data_ecosystem_services-202307.0.8/data_ecosystem_services/cdc_admin_service/environment_logging.py
--rw-r--r--   0        0        0     8398 2023-07-25 19:38:09.834920 data_ecosystem_services-202307.0.8/data_ecosystem_services/cdc_admin_service/environment_tracing.py
--rw-r--r--   0        0        0     1013 2023-07-25 19:38:09.834920 data_ecosystem_services-202307.0.8/data_ecosystem_services/cdc_security_service/__init__.py
--rw-r--r--   0        0        0        0 2023-07-25 19:38:09.834920 data_ecosystem_services-202307.0.8/data_ecosystem_services/cdc_security_service/security_base64.py
--rw-r--r--   0        0        0    21410 2023-07-25 19:38:09.834920 data_ecosystem_services-202307.0.8/data_ecosystem_services/cdc_security_service/security_core.py
--rw-r--r--   0        0        0     1175 2023-07-25 19:38:09.834920 data_ecosystem_services-202307.0.8/data_ecosystem_services/cdc_self_service/__init__.py
--rw-r--r--   0        0        0    42751 2023-07-25 19:38:09.834920 data_ecosystem_services-202307.0.8/data_ecosystem_services/cdc_self_service/dataset_metadata.py
--rw-r--r--   0        0        0    40188 2023-07-25 19:38:09.834920 data_ecosystem_services-202307.0.8/data_ecosystem_services/cdc_self_service/environment_metadata.py
--rw-r--r--   0        0        0    36068 2023-07-25 19:38:09.838920 data_ecosystem_services-202307.0.8/data_ecosystem_services/cdc_self_service/job_metadata.py
--rw-r--r--   0        0        0     2254 2023-07-25 19:38:09.838920 data_ecosystem_services-202307.0.8/data_ecosystem_services/cdc_self_service/logging_metadata.py
--rw-r--r--   0        0        0    22352 2023-07-25 19:38:09.838920 data_ecosystem_services-202307.0.8/data_ecosystem_services/cdc_self_service/pipeline_metadata.py
--rw-r--r--   0        0        0     1727 2023-07-25 19:38:09.838920 data_ecosystem_services-202307.0.8/data_ecosystem_services/cdc_tech_environment_service/__init__.py
--rw-r--r--   0        0        0    33787 2023-07-25 19:38:09.838920 data_ecosystem_services-202307.0.8/data_ecosystem_services/cdc_tech_environment_service/dataset_convert.py
--rw-r--r--   0        0        0     8962 2023-07-25 19:38:09.838920 data_ecosystem_services-202307.0.8/data_ecosystem_services/cdc_tech_environment_service/dataset_core.py
--rw-r--r--   0        0        0    25880 2023-07-25 19:38:09.838920 data_ecosystem_services-202307.0.8/data_ecosystem_services/cdc_tech_environment_service/dataset_crud.py
--rw-r--r--   0        0        0     3825 2023-07-25 19:38:09.838920 data_ecosystem_services-202307.0.8/data_ecosystem_services/cdc_tech_environment_service/dataset_extract.py
--rw-r--r--   0        0        0     3949 2023-07-25 19:38:09.838920 data_ecosystem_services-202307.0.8/data_ecosystem_services/cdc_tech_environment_service/environment_core.py
--rw-r--r--   0        0        0    50039 2023-07-25 19:38:09.838920 data_ecosystem_services-202307.0.8/data_ecosystem_services/cdc_tech_environment_service/environment_file.py
--rw-r--r--   0        0        0     5323 2023-07-25 19:38:09.838920 data_ecosystem_services-202307.0.8/data_ecosystem_services/cdc_tech_environment_service/environment_http.py
--rw-r--r--   0        0        0     4903 2023-07-25 19:38:09.838920 data_ecosystem_services-202307.0.8/data_ecosystem_services/cdc_tech_environment_service/environment_spark.py
--rw-r--r--   0        0        0     4648 2023-07-25 19:38:09.838920 data_ecosystem_services-202307.0.8/data_ecosystem_services/cdc_tech_environment_service/job_core.py
--rw-r--r--   0        0        0    17832 2023-07-25 19:38:09.838920 data_ecosystem_services-202307.0.8/data_ecosystem_services/cdc_tech_environment_service/repo_core.py
--rw-r--r--   0        0        0     8956 2023-07-25 19:38:09.838920 data_ecosystem_services-202307.0.8/data_ecosystem_services/directory_paths.txt
--rw-r--r--   0        0        0      827 2023-07-25 19:38:09.838920 data_ecosystem_services-202307.0.8/data_ecosystem_services/github_service/__init__.py
--rw-r--r--   0        0        0     7250 2023-07-25 19:38:09.838920 data_ecosystem_services-202307.0.8/data_ecosystem_services/github_service/github_secret.py
--rw-r--r--   0        0        0     1707 2023-07-25 19:38:09.838920 data_ecosystem_services-202307.0.8/data_ecosystem_services/jira_service/__init__.py
--rw-r--r--   0        0        0     6295 2023-07-25 19:38:09.838920 data_ecosystem_services-202307.0.8/data_ecosystem_services/jira_service/jira_client.py
--rw-r--r--   0        0        0       44 2023-07-25 19:38:09.838920 data_ecosystem_services-202307.0.8/data_ecosystem_services/output.txt
--rw-r--r--   0        0        0      869 2023-07-25 19:38:09.838920 data_ecosystem_services-202307.0.8/data_ecosystem_services/posit_service/__init__.py
--rw-r--r--   0        0        0    21050 2023-07-25 19:38:09.838920 data_ecosystem_services-202307.0.8/data_ecosystem_services/posit_service/posit_connect.py
--rw-r--r--   0        0        0      825 2023-07-25 19:38:09.838920 data_ecosystem_services-202307.0.8/data_ecosystem_services/python_service/__init__.py
--rw-r--r--   0        0        0       24 2023-07-25 19:38:09.838920 data_ecosystem_services-202307.0.8/data_ecosystem_services/python_service/python_client.py
--rw-r--r--   0        0        0    15021 2023-07-25 19:38:09.838920 data_ecosystem_services-202307.0.8/data_ecosystem_services/requirements.txt
--rw-r--r--   0        0        0      832 2023-07-25 19:38:09.838920 data_ecosystem_services-202307.0.8/data_ecosystem_services/windows_service/__init__.py
--rw-r--r--   0        0        0     2499 2023-07-25 19:38:09.838920 data_ecosystem_services-202307.0.8/data_ecosystem_services/windows_service/windows_credential.py
--rw-r--r--   0        0        0    11357 2023-07-25 19:38:09.842920 data_ecosystem_services-202307.0.8/license.md
--rw-r--r--   0        0        0     3915 2023-07-25 19:40:59.217430 data_ecosystem_services-202307.0.8/pyproject.toml
--rw-r--r--   0        0        0    52428 2023-07-25 19:38:09.846921 data_ecosystem_services-202307.0.8/readme.md
--rw-r--r--   0        0        0      129 2023-07-25 19:38:09.846921 data_ecosystem_services-202307.0.8/setup.cfg
--rw-r--r--   0        0        0      127 2023-07-25 19:38:09.846921 data_ecosystem_services-202307.0.8/setup.py
--rw-r--r--   0        0        0    55939 1970-01-01 00:00:00.000000 data_ecosystem_services-202307.0.8/PKG-INFO
+-rw-r--r--   0        0        0      918 2023-07-25 19:41:14.054138 data_ecosystem_services-202307.0.9/data_ecosystem_services/__main__.py
+-rw-r--r--   0        0        0     1264 2023-07-25 19:41:14.054138 data_ecosystem_services-202307.0.9/data_ecosystem_services/alation_service/__init__.py
+-rw-r--r--   0        0        0     5030 2023-07-25 19:41:14.054138 data_ecosystem_services-202307.0.9/data_ecosystem_services/alation_service/column.py
+-rw-r--r--   0        0        0    25117 2023-07-25 19:41:14.054138 data_ecosystem_services-202307.0.9/data_ecosystem_services/alation_service/customfieldsendpoint.py
+-rw-r--r--   0        0        0    13816 2023-07-25 19:41:14.054138 data_ecosystem_services-202307.0.9/data_ecosystem_services/alation_service/datasource.py
+-rw-r--r--   0        0        0     2037 2023-07-25 19:41:14.054138 data_ecosystem_services-202307.0.9/data_ecosystem_services/alation_service/endpoint.py
+-rw-r--r--   0        0        0    13626 2023-07-25 19:41:14.054138 data_ecosystem_services-202307.0.9/data_ecosystem_services/alation_service/excelmetadata.py
+-rw-r--r--   0        0        0      566 2023-07-25 19:41:14.054138 data_ecosystem_services-202307.0.9/data_ecosystem_services/alation_service/execution_session.py
+-rw-r--r--   0        0        0     7568 2023-07-25 19:41:14.054138 data_ecosystem_services-202307.0.9/data_ecosystem_services/alation_service/idfinderendpoint.py
+-rw-r--r--   0        0        0    16676 2023-07-25 19:41:14.054138 data_ecosystem_services-202307.0.9/data_ecosystem_services/alation_service/manifest.py
+-rw-r--r--   0        0        0    10973 2023-07-25 19:41:14.054138 data_ecosystem_services-202307.0.9/data_ecosystem_services/alation_service/query.py
+-rw-r--r--   0        0        0    55259 2023-07-25 19:41:14.054138 data_ecosystem_services-202307.0.9/data_ecosystem_services/alation_service/schema.py
+-rw-r--r--   0        0        0     7368 2023-07-25 19:41:14.054138 data_ecosystem_services-202307.0.9/data_ecosystem_services/alation_service/table.py
+-rw-r--r--   0        0        0     1486 2023-07-25 19:41:14.054138 data_ecosystem_services-202307.0.9/data_ecosystem_services/alation_service/tagsendpoint.py
+-rw-r--r--   0        0        0    25982 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/alation_service/tokenendpoint.py
+-rw-r--r--   0        0        0     1044 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/az_client_service/__init__.py
+-rw-r--r--   0        0        0       41 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/az_client_service/az_client.py
+-rw-r--r--   0        0        0     4570 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/az_client_service/azd_client.py
+-rw-r--r--   0        0        0     1050 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/az_key_vault_service/__init__.py
+-rw-r--r--   0        0        0     8967 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/az_key_vault_service/az_key_vault.py
+-rw-r--r--   0        0        0     1073 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/az_storage_service/__init__.py
+-rw-r--r--   0        0        0     2665 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/az_storage_service/az_storage_queue.py
+-rw-r--r--   0        0        0     1024 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_admin_service/__init__.py
+-rw-r--r--   0        0        0    15940 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_admin_service/environment_logging.py
+-rw-r--r--   0        0        0     8398 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_admin_service/environment_tracing.py
+-rw-r--r--   0        0        0     1013 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_security_service/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_security_service/security_base64.py
+-rw-r--r--   0        0        0    21410 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_security_service/security_core.py
+-rw-r--r--   0        0        0     1175 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_self_service/__init__.py
+-rw-r--r--   0        0        0    42751 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_self_service/dataset_metadata.py
+-rw-r--r--   0        0        0    40188 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_self_service/environment_metadata.py
+-rw-r--r--   0        0        0    36068 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_self_service/job_metadata.py
+-rw-r--r--   0        0        0     2254 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_self_service/logging_metadata.py
+-rw-r--r--   0        0        0    22352 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_self_service/pipeline_metadata.py
+-rw-r--r--   0        0        0     1727 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_tech_environment_service/__init__.py
+-rw-r--r--   0        0        0    33787 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_tech_environment_service/dataset_convert.py
+-rw-r--r--   0        0        0     8962 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_tech_environment_service/dataset_core.py
+-rw-r--r--   0        0        0    25880 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_tech_environment_service/dataset_crud.py
+-rw-r--r--   0        0        0     3825 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_tech_environment_service/dataset_extract.py
+-rw-r--r--   0        0        0     3949 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_tech_environment_service/environment_core.py
+-rw-r--r--   0        0        0    50039 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_tech_environment_service/environment_file.py
+-rw-r--r--   0        0        0     5323 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_tech_environment_service/environment_http.py
+-rw-r--r--   0        0        0     4903 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_tech_environment_service/environment_spark.py
+-rw-r--r--   0        0        0     4648 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_tech_environment_service/job_core.py
+-rw-r--r--   0        0        0    17832 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_tech_environment_service/repo_core.py
+-rw-r--r--   0        0        0     8956 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/directory_paths.txt
+-rw-r--r--   0        0        0      827 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/github_service/__init__.py
+-rw-r--r--   0        0        0     7250 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/github_service/github_secret.py
+-rw-r--r--   0        0        0     1707 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/jira_service/__init__.py
+-rw-r--r--   0        0        0     6295 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/jira_service/jira_client.py
+-rw-r--r--   0        0        0       44 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/output.txt
+-rw-r--r--   0        0        0      869 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/posit_service/__init__.py
+-rw-r--r--   0        0        0    21050 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/posit_service/posit_connect.py
+-rw-r--r--   0        0        0      825 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/python_service/__init__.py
+-rw-r--r--   0        0        0       24 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/python_service/python_client.py
+-rw-r--r--   0        0        0    15021 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/requirements.txt
+-rw-r--r--   0        0        0      832 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/windows_service/__init__.py
+-rw-r--r--   0        0        0     2499 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/windows_service/windows_credential.py
+-rw-r--r--   0        0        0    11357 2023-07-25 19:41:14.066138 data_ecosystem_services-202307.0.9/license.md
+-rw-r--r--   0        0        0     3915 2023-07-25 19:44:28.350867 data_ecosystem_services-202307.0.9/pyproject.toml
+-rw-r--r--   0        0        0    52428 2023-07-25 19:41:14.066138 data_ecosystem_services-202307.0.9/readme.md
+-rw-r--r--   0        0        0      129 2023-07-25 19:41:14.066138 data_ecosystem_services-202307.0.9/setup.cfg
+-rw-r--r--   0        0        0      127 2023-07-25 19:41:14.066138 data_ecosystem_services-202307.0.9/setup.py
+-rw-r--r--   0        0        0    55939 1970-01-01 00:00:00.000000 data_ecosystem_services-202307.0.9/PKG-INFO
```

### Comparing `data_ecosystem_services-202307.0.8/data_ecosystem_services/__main__.py` & `data_ecosystem_services-202307.0.9/data_ecosystem_services/__main__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.8/data_ecosystem_services/alation_service/__init__.py` & `data_ecosystem_services-202307.0.9/data_ecosystem_services/alation_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.8/data_ecosystem_services/alation_service/column.py` & `data_ecosystem_services-202307.0.9/data_ecosystem_services/alation_service/column.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.8/data_ecosystem_services/alation_service/customfieldsendpoint.py` & `data_ecosystem_services-202307.0.9/data_ecosystem_services/alation_service/customfieldsendpoint.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.8/data_ecosystem_services/alation_service/datasource.py` & `data_ecosystem_services-202307.0.9/data_ecosystem_services/alation_service/datasource.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.8/data_ecosystem_services/alation_service/endpoint.py` & `data_ecosystem_services-202307.0.9/data_ecosystem_services/alation_service/endpoint.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.8/data_ecosystem_services/alation_service/excelmetadata.py` & `data_ecosystem_services-202307.0.9/data_ecosystem_services/alation_service/excelmetadata.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.8/data_ecosystem_services/alation_service/execution_session.py` & `data_ecosystem_services-202307.0.9/data_ecosystem_services/alation_service/execution_session.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.8/data_ecosystem_services/alation_service/idfinderendpoint.py` & `data_ecosystem_services-202307.0.9/data_ecosystem_services/alation_service/idfinderendpoint.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.8/data_ecosystem_services/alation_service/manifest.py` & `data_ecosystem_services-202307.0.9/data_ecosystem_services/alation_service/manifest.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.8/data_ecosystem_services/alation_service/query.py` & `data_ecosystem_services-202307.0.9/data_ecosystem_services/alation_service/query.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.8/data_ecosystem_services/alation_service/schema.py` & `data_ecosystem_services-202307.0.9/data_ecosystem_services/alation_service/schema.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.8/data_ecosystem_services/alation_service/table.py` & `data_ecosystem_services-202307.0.9/data_ecosystem_services/alation_service/table.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.8/data_ecosystem_services/alation_service/tagsendpoint.py` & `data_ecosystem_services-202307.0.9/data_ecosystem_services/alation_service/tagsendpoint.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.8/data_ecosystem_services/alation_service/tokenendpoint.py` & `data_ecosystem_services-202307.0.9/data_ecosystem_services/alation_service/tokenendpoint.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.8/data_ecosystem_services/az_client_service/__init__.py` & `data_ecosystem_services-202307.0.9/data_ecosystem_services/az_client_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.8/data_ecosystem_services/az_client_service/azd_client.py` & `data_ecosystem_services-202307.0.9/data_ecosystem_services/az_client_service/azd_client.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.8/data_ecosystem_services/az_key_vault_service/__init__.py` & `data_ecosystem_services-202307.0.9/data_ecosystem_services/az_key_vault_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.8/data_ecosystem_services/az_key_vault_service/az_key_vault.py` & `data_ecosystem_services-202307.0.9/data_ecosystem_services/az_key_vault_service/az_key_vault.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.8/data_ecosystem_services/az_storage_service/__init__.py` & `data_ecosystem_services-202307.0.9/data_ecosystem_services/az_storage_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.8/data_ecosystem_services/az_storage_service/az_storage_queue.py` & `data_ecosystem_services-202307.0.9/data_ecosystem_services/az_storage_service/az_storage_queue.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.8/data_ecosystem_services/cdc_admin_service/__init__.py` & `data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_admin_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.8/data_ecosystem_services/cdc_admin_service/environment_logging.py` & `data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_admin_service/environment_logging.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.8/data_ecosystem_services/cdc_admin_service/environment_tracing.py` & `data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_admin_service/environment_tracing.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.8/data_ecosystem_services/cdc_security_service/__init__.py` & `data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_security_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.8/data_ecosystem_services/cdc_security_service/security_core.py` & `data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_security_service/security_core.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.8/data_ecosystem_services/cdc_self_service/__init__.py` & `data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_self_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.8/data_ecosystem_services/cdc_self_service/dataset_metadata.py` & `data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_self_service/dataset_metadata.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.8/data_ecosystem_services/cdc_self_service/environment_metadata.py` & `data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_self_service/environment_metadata.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.8/data_ecosystem_services/cdc_self_service/job_metadata.py` & `data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_self_service/job_metadata.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.8/data_ecosystem_services/cdc_self_service/logging_metadata.py` & `data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_self_service/logging_metadata.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.8/data_ecosystem_services/cdc_self_service/pipeline_metadata.py` & `data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_self_service/pipeline_metadata.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.8/data_ecosystem_services/cdc_tech_environment_service/__init__.py` & `data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_tech_environment_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.8/data_ecosystem_services/cdc_tech_environment_service/dataset_convert.py` & `data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_tech_environment_service/dataset_convert.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.8/data_ecosystem_services/cdc_tech_environment_service/dataset_core.py` & `data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_tech_environment_service/dataset_core.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.8/data_ecosystem_services/cdc_tech_environment_service/dataset_crud.py` & `data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_tech_environment_service/dataset_crud.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.8/data_ecosystem_services/cdc_tech_environment_service/dataset_extract.py` & `data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_tech_environment_service/dataset_extract.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.8/data_ecosystem_services/cdc_tech_environment_service/environment_core.py` & `data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_tech_environment_service/environment_core.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.8/data_ecosystem_services/cdc_tech_environment_service/environment_file.py` & `data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_tech_environment_service/environment_file.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.8/data_ecosystem_services/cdc_tech_environment_service/environment_http.py` & `data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_tech_environment_service/environment_http.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.8/data_ecosystem_services/cdc_tech_environment_service/environment_spark.py` & `data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_tech_environment_service/environment_spark.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.8/data_ecosystem_services/cdc_tech_environment_service/job_core.py` & `data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_tech_environment_service/job_core.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.8/data_ecosystem_services/cdc_tech_environment_service/repo_core.py` & `data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_tech_environment_service/repo_core.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.8/data_ecosystem_services/directory_paths.txt` & `data_ecosystem_services-202307.0.9/data_ecosystem_services/directory_paths.txt`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.8/data_ecosystem_services/github_service/__init__.py` & `data_ecosystem_services-202307.0.9/data_ecosystem_services/github_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.8/data_ecosystem_services/github_service/github_secret.py` & `data_ecosystem_services-202307.0.9/data_ecosystem_services/github_service/github_secret.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.8/data_ecosystem_services/jira_service/__init__.py` & `data_ecosystem_services-202307.0.9/data_ecosystem_services/jira_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.8/data_ecosystem_services/jira_service/jira_client.py` & `data_ecosystem_services-202307.0.9/data_ecosystem_services/jira_service/jira_client.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.8/data_ecosystem_services/posit_service/__init__.py` & `data_ecosystem_services-202307.0.9/data_ecosystem_services/posit_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.8/data_ecosystem_services/posit_service/posit_connect.py` & `data_ecosystem_services-202307.0.9/data_ecosystem_services/posit_service/posit_connect.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.8/data_ecosystem_services/python_service/__init__.py` & `data_ecosystem_services-202307.0.9/data_ecosystem_services/python_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.8/data_ecosystem_services/requirements.txt` & `data_ecosystem_services-202307.0.9/data_ecosystem_services/requirements.txt`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.8/data_ecosystem_services/windows_service/__init__.py` & `data_ecosystem_services-202307.0.9/data_ecosystem_services/windows_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.8/data_ecosystem_services/windows_service/windows_credential.py` & `data_ecosystem_services-202307.0.9/data_ecosystem_services/windows_service/windows_credential.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.8/license.md` & `data_ecosystem_services-202307.0.9/license.md`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.8/pyproject.toml` & `data_ecosystem_services-202307.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 [project.urls]
 "Homepage" = "https://test.pypi.org/project/data-ecosystem-services"
 "Documentation" = "https://gift.readthedocs.io"
 "Repository" = "https://github.com/cdcent/data-ecosystem-services"
 
 [tool.poetry]
 name="data_ecosystem_services"
-version="202307.0.8"
+version="202307.0.9"
 description="Program Agnostic Data Ecosystem (PADE) - Python Services"
 authors=["John Bowyer <zfi4@cdc.gov>"]
 readme = "readme.md"
 license="Apache"
 homepage="https://test.pypi.org/project/data-ecosystem-services"
 repository="https://github.com/cdcent/data-ecosystem-services"
 classifiers=[
```

### Comparing `data_ecosystem_services-202307.0.8/readme.md` & `data_ecosystem_services-202307.0.9/readme.md`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.8/PKG-INFO` & `data_ecosystem_services-202307.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-ecosystem-services
-Version: 202307.0.8
+Version: 202307.0.9
 Summary: Program Agnostic Data Ecosystem (PADE) - Python Services
 Home-page: https://test.pypi.org/project/data-ecosystem-services
 License: Apache
 Author: John Bowyer
 Author-email: zfi4@cdc.gov
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

