# Comparing `tmp/jobbergate_api-3.5.0a7.tar.gz` & `tmp/jobbergate_api-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jobbergate_api-3.5.0a7.tar", max compression
+gzip compressed data, was "jobbergate_api-3.6.0.tar", max compression
```

## Comparing `jobbergate_api-3.5.0a7.tar` & `jobbergate_api-3.6.0.tar`

### file list

```diff
@@ -1,61 +1,62 @@
--rw-r--r--   0        0        0     1082 2023-06-28 19:08:34.886780 jobbergate_api-3.5.0a7/LICENSE
--rw-r--r--   0        0        0      738 2023-06-28 19:08:34.886780 jobbergate_api-3.5.0a7/README.rst
--rw-r--r--   0        0        0      169 2023-06-28 19:08:34.890780 jobbergate_api-3.5.0a7/jobbergate_api/__init__.py
--rw-r--r--   0        0        0       30 2023-06-28 19:08:34.890780 jobbergate_api-3.5.0a7/jobbergate_api/apps/__init__.py
--rw-r--r--   0        0        0       41 2023-06-28 19:08:34.890780 jobbergate_api-3.5.0a7/jobbergate_api/apps/applications/__init__.py
--rw-r--r--   0        0        0     5655 2023-06-28 19:08:34.890780 jobbergate_api-3.5.0a7/jobbergate_api/apps/applications/application_files.py
--rw-r--r--   0        0        0      234 2023-06-28 19:08:34.890780 jobbergate_api-3.5.0a7/jobbergate_api/apps/applications/constants.py
--rw-r--r--   0        0        0     9408 2023-06-28 19:08:34.890780 jobbergate_api-3.5.0a7/jobbergate_api/apps/applications/file_validation.py
--rw-r--r--   0        0        0     1474 2023-06-28 19:08:34.890780 jobbergate_api-3.5.0a7/jobbergate_api/apps/applications/models.py
--rw-r--r--   0        0        0    15491 2023-06-28 19:08:34.890780 jobbergate_api-3.5.0a7/jobbergate_api/apps/applications/routers.py
--rw-r--r--   0        0        0     7421 2023-06-28 19:08:34.890780 jobbergate_api-3.5.0a7/jobbergate_api/apps/applications/schemas.py
--rw-r--r--   0        0        0       40 2023-06-28 19:08:34.890780 jobbergate_api-3.5.0a7/jobbergate_api/apps/job_scripts/__init__.py
--rw-r--r--   0        0        0    12639 2023-06-28 19:08:34.890780 jobbergate_api-3.5.0a7/jobbergate_api/apps/job_scripts/job_script_files.py
--rw-r--r--   0        0        0     1287 2023-06-28 19:08:34.890780 jobbergate_api-3.5.0a7/jobbergate_api/apps/job_scripts/models.py
--rw-r--r--   0        0        0    17918 2023-06-28 19:08:34.890780 jobbergate_api-3.5.0a7/jobbergate_api/apps/job_scripts/routers.py
--rw-r--r--   0        0        0     3800 2023-06-28 19:08:34.890780 jobbergate_api-3.5.0a7/jobbergate_api/apps/job_scripts/schemas.py
--rw-r--r--   0        0        0       44 2023-06-28 19:08:34.890780 jobbergate_api-3.5.0a7/jobbergate_api/apps/job_submissions/__init__.py
--rw-r--r--   0        0        0      529 2023-06-28 19:08:34.890780 jobbergate_api-3.5.0a7/jobbergate_api/apps/job_submissions/constants.py
--rw-r--r--   0        0        0     1909 2023-06-28 19:08:34.890780 jobbergate_api-3.5.0a7/jobbergate_api/apps/job_submissions/models.py
--rw-r--r--   0        0        0    12331 2023-06-28 19:08:34.890780 jobbergate_api-3.5.0a7/jobbergate_api/apps/job_submissions/properties_parser.py
--rw-r--r--   0        0        0    19283 2023-06-28 19:08:34.890780 jobbergate_api-3.5.0a7/jobbergate_api/apps/job_submissions/routers.py
--rw-r--r--   0        0        0    15946 2023-06-28 19:08:34.890780 jobbergate_api-3.5.0a7/jobbergate_api/apps/job_submissions/schemas.py
--rw-r--r--   0        0        0     1313 2023-06-28 19:08:34.890780 jobbergate_api-3.5.0a7/jobbergate_api/apps/permissions.py
--rw-r--r--   0        0        0     3621 2023-06-28 19:08:34.890780 jobbergate_api-3.5.0a7/jobbergate_api/config.py
--rw-r--r--   0        0        0     2466 2023-06-28 19:08:34.890780 jobbergate_api-3.5.0a7/jobbergate_api/email_notification.py
--rw-r--r--   0        0        0     3268 2023-06-28 19:08:34.890780 jobbergate_api-3.5.0a7/jobbergate_api/main.py
--rw-r--r--   0        0        0     3433 2023-06-28 19:08:34.890780 jobbergate_api-3.5.0a7/jobbergate_api/meta_mapper.py
--rw-r--r--   0        0        0       96 2023-06-28 19:08:34.890780 jobbergate_api-3.5.0a7/jobbergate_api/metadata.py
--rw-r--r--   0        0        0     3470 2023-06-28 19:08:34.890780 jobbergate_api-3.5.0a7/jobbergate_api/pagination.py
--rw-r--r--   0        0        0     2284 2023-06-28 19:08:34.890780 jobbergate_api-3.5.0a7/jobbergate_api/s3_manager.py
--rw-r--r--   0        0        0     2166 2023-06-28 19:08:34.890780 jobbergate_api-3.5.0a7/jobbergate_api/security.py
--rw-r--r--   0        0        0     5580 2023-06-28 19:08:34.890780 jobbergate_api-3.5.0a7/jobbergate_api/storage.py
--rw-r--r--   0        0        0       40 2023-06-28 19:08:34.890780 jobbergate_api-3.5.0a7/jobbergate_api/tests/__init__.py
--rw-r--r--   0        0        0       28 2023-06-28 19:08:34.890780 jobbergate_api-3.5.0a7/jobbergate_api/tests/apps/__init__.py
--rw-r--r--   0        0        0       44 2023-06-28 19:08:34.890780 jobbergate_api-3.5.0a7/jobbergate_api/tests/apps/applications/__init__.py
--rw-r--r--   0        0        0    10634 2023-06-28 19:08:34.890780 jobbergate_api-3.5.0a7/jobbergate_api/tests/apps/applications/test_application_files.py
--rw-r--r--   0        0        0     1967 2023-06-28 19:08:34.890780 jobbergate_api-3.5.0a7/jobbergate_api/tests/apps/applications/test_file_validation.py
--rw-r--r--   0        0        0    50586 2023-06-28 19:08:34.890780 jobbergate_api-3.5.0a7/jobbergate_api/tests/apps/applications/test_routers.py
--rw-r--r--   0        0        0     5180 2023-06-28 19:08:34.890780 jobbergate_api-3.5.0a7/jobbergate_api/tests/apps/applications/test_schemas.py
--rw-r--r--   0        0        0     2756 2023-06-28 19:08:34.890780 jobbergate_api-3.5.0a7/jobbergate_api/tests/apps/conftest.py
--rw-r--r--   0        0        0       42 2023-06-28 19:08:34.890780 jobbergate_api-3.5.0a7/jobbergate_api/tests/apps/job_scripts/__init__.py
--rw-r--r--   0        0        0     1376 2023-06-28 19:08:34.890780 jobbergate_api-3.5.0a7/jobbergate_api/tests/apps/job_scripts/conftest.py
--rw-r--r--   0        0        0    11518 2023-06-28 19:08:34.890780 jobbergate_api-3.5.0a7/jobbergate_api/tests/apps/job_scripts/test_job_script_files.py
--rw-r--r--   0        0        0    57121 2023-06-28 19:08:34.890780 jobbergate_api-3.5.0a7/jobbergate_api/tests/apps/job_scripts/test_routers.py
--rw-r--r--   0        0        0       46 2023-06-28 19:08:34.890780 jobbergate_api-3.5.0a7/jobbergate_api/tests/apps/job_submissions/__init__.py
--rw-r--r--   0        0        0    24706 2023-06-28 19:08:34.890780 jobbergate_api-3.5.0a7/jobbergate_api/tests/apps/job_submissions/test_properties_parser.py
--rw-r--r--   0        0        0    80706 2023-06-28 19:08:34.890780 jobbergate_api-3.5.0a7/jobbergate_api/tests/apps/job_submissions/test_routers.py
--rw-r--r--   0        0        0      511 2023-06-28 19:08:34.890780 jobbergate_api-3.5.0a7/jobbergate_api/tests/apps/test_main.py
--rw-r--r--   0        0        0     8900 2023-06-28 19:08:34.890780 jobbergate_api-3.5.0a7/jobbergate_api/tests/conftest.py
--rw-r--r--   0        0        0     4503 2023-06-28 19:08:34.890780 jobbergate_api-3.5.0a7/jobbergate_api/tests/integration/draft_test_jobbergate_slurm_job_properties.py
--rw-r--r--   0        0        0     3215 2023-06-28 19:08:34.890780 jobbergate_api-3.5.0a7/jobbergate_api/tests/test_config.py
--rw-r--r--   0        0        0     4974 2023-06-28 19:08:34.890780 jobbergate_api-3.5.0a7/jobbergate_api/tests/test_email_notification.py
--rw-r--r--   0        0        0     3177 2023-06-28 19:08:34.890780 jobbergate_api-3.5.0a7/jobbergate_api/tests/test_meta_mapper.py
--rw-r--r--   0        0        0     3959 2023-06-28 19:08:34.890780 jobbergate_api-3.5.0a7/jobbergate_api/tests/test_pagination.py
--rw-r--r--   0        0        0     1146 2023-06-28 19:08:34.890780 jobbergate_api-3.5.0a7/jobbergate_api/tests/test_s3_manager.py
--rw-r--r--   0        0        0     2718 2023-06-28 19:08:34.890780 jobbergate_api-3.5.0a7/jobbergate_api/tests/test_security.py
--rw-r--r--   0        0        0     4512 2023-06-28 19:08:34.890780 jobbergate_api-3.5.0a7/jobbergate_api/tests/test_storage.py
--rw-r--r--   0        0        0     2777 2023-06-28 19:08:34.890780 jobbergate_api-3.5.0a7/jobbergate_api/tests/test_version.py
--rw-r--r--   0        0        0     1102 2023-06-28 19:08:34.894780 jobbergate_api-3.5.0a7/jobbergate_api/version.py
--rw-r--r--   0        0        0     2898 2023-06-28 19:08:34.894780 jobbergate_api-3.5.0a7/pyproject.toml
--rw-r--r--   0        0        0     2756 1970-01-01 00:00:00.000000 jobbergate_api-3.5.0a7/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-07-30 04:37:48.598570 jobbergate_api-3.6.0/LICENSE
+-rw-r--r--   0        0        0      738 2023-07-30 04:37:48.598570 jobbergate_api-3.6.0/README.rst
+-rw-r--r--   0        0        0      169 2023-07-30 04:37:48.598570 jobbergate_api-3.6.0/jobbergate_api/__init__.py
+-rw-r--r--   0        0        0       30 2023-07-30 04:37:48.598570 jobbergate_api-3.6.0/jobbergate_api/apps/__init__.py
+-rw-r--r--   0        0        0       41 2023-07-30 04:37:48.598570 jobbergate_api-3.6.0/jobbergate_api/apps/applications/__init__.py
+-rw-r--r--   0        0        0     6079 2023-07-30 04:37:48.598570 jobbergate_api-3.6.0/jobbergate_api/apps/applications/application_files.py
+-rw-r--r--   0        0        0      234 2023-07-30 04:37:48.598570 jobbergate_api-3.6.0/jobbergate_api/apps/applications/constants.py
+-rw-r--r--   0        0        0     9408 2023-07-30 04:37:48.598570 jobbergate_api-3.6.0/jobbergate_api/apps/applications/file_validation.py
+-rw-r--r--   0        0        0     1474 2023-07-30 04:37:48.598570 jobbergate_api-3.6.0/jobbergate_api/apps/applications/models.py
+-rw-r--r--   0        0        0    16375 2023-07-30 04:37:48.598570 jobbergate_api-3.6.0/jobbergate_api/apps/applications/routers.py
+-rw-r--r--   0        0        0     7414 2023-07-30 04:37:48.598570 jobbergate_api-3.6.0/jobbergate_api/apps/applications/schemas.py
+-rw-r--r--   0        0        0       40 2023-07-30 04:37:48.598570 jobbergate_api-3.6.0/jobbergate_api/apps/job_scripts/__init__.py
+-rw-r--r--   0        0        0    13063 2023-07-30 04:37:48.598570 jobbergate_api-3.6.0/jobbergate_api/apps/job_scripts/job_script_files.py
+-rw-r--r--   0        0        0     1287 2023-07-30 04:37:48.598570 jobbergate_api-3.6.0/jobbergate_api/apps/job_scripts/models.py
+-rw-r--r--   0        0        0    18011 2023-07-30 04:37:48.598570 jobbergate_api-3.6.0/jobbergate_api/apps/job_scripts/routers.py
+-rw-r--r--   0        0        0     3800 2023-07-30 04:37:48.598570 jobbergate_api-3.6.0/jobbergate_api/apps/job_scripts/schemas.py
+-rw-r--r--   0        0        0       44 2023-07-30 04:37:48.598570 jobbergate_api-3.6.0/jobbergate_api/apps/job_submissions/__init__.py
+-rw-r--r--   0        0        0      529 2023-07-30 04:37:48.602570 jobbergate_api-3.6.0/jobbergate_api/apps/job_submissions/constants.py
+-rw-r--r--   0        0        0     1909 2023-07-30 04:37:48.602570 jobbergate_api-3.6.0/jobbergate_api/apps/job_submissions/models.py
+-rw-r--r--   0        0        0    12416 2023-07-30 04:37:48.602570 jobbergate_api-3.6.0/jobbergate_api/apps/job_submissions/properties_parser.py
+-rw-r--r--   0        0        0    19181 2023-07-30 04:37:48.602570 jobbergate_api-3.6.0/jobbergate_api/apps/job_submissions/routers.py
+-rw-r--r--   0        0        0    16079 2023-07-30 04:37:48.602570 jobbergate_api-3.6.0/jobbergate_api/apps/job_submissions/schemas.py
+-rw-r--r--   0        0        0     1313 2023-07-30 04:37:48.602570 jobbergate_api-3.6.0/jobbergate_api/apps/permissions.py
+-rw-r--r--   0        0        0     3766 2023-07-30 04:37:48.602570 jobbergate_api-3.6.0/jobbergate_api/config.py
+-rw-r--r--   0        0        0     2466 2023-07-30 04:37:48.602570 jobbergate_api-3.6.0/jobbergate_api/email_notification.py
+-rw-r--r--   0        0        0     3265 2023-07-30 04:37:48.602570 jobbergate_api-3.6.0/jobbergate_api/main.py
+-rw-r--r--   0        0        0     3433 2023-07-30 04:37:48.602570 jobbergate_api-3.6.0/jobbergate_api/meta_mapper.py
+-rw-r--r--   0        0        0       96 2023-07-30 04:37:48.602570 jobbergate_api-3.6.0/jobbergate_api/metadata.py
+-rw-r--r--   0        0        0     3549 2023-07-30 04:37:48.602570 jobbergate_api-3.6.0/jobbergate_api/pagination.py
+-rw-r--r--   0        0        0     2284 2023-07-30 04:37:48.602570 jobbergate_api-3.6.0/jobbergate_api/s3_manager.py
+-rw-r--r--   0        0        0     3214 2023-07-30 04:37:48.602570 jobbergate_api-3.6.0/jobbergate_api/security.py
+-rw-r--r--   0        0        0    13053 2023-07-30 04:37:48.602570 jobbergate_api-3.6.0/jobbergate_api/storage.py
+-rw-r--r--   0        0        0       40 2023-07-30 04:37:48.602570 jobbergate_api-3.6.0/jobbergate_api/tests/__init__.py
+-rw-r--r--   0        0        0       28 2023-07-30 04:37:48.602570 jobbergate_api-3.6.0/jobbergate_api/tests/apps/__init__.py
+-rw-r--r--   0        0        0       44 2023-07-30 04:37:48.602570 jobbergate_api-3.6.0/jobbergate_api/tests/apps/applications/__init__.py
+-rw-r--r--   0        0        0    10634 2023-07-30 04:37:48.602570 jobbergate_api-3.6.0/jobbergate_api/tests/apps/applications/test_application_files.py
+-rw-r--r--   0        0        0     1967 2023-07-30 04:37:48.602570 jobbergate_api-3.6.0/jobbergate_api/tests/apps/applications/test_file_validation.py
+-rw-r--r--   0        0        0    50991 2023-07-30 04:37:48.602570 jobbergate_api-3.6.0/jobbergate_api/tests/apps/applications/test_routers.py
+-rw-r--r--   0        0        0     5180 2023-07-30 04:37:48.602570 jobbergate_api-3.6.0/jobbergate_api/tests/apps/applications/test_schemas.py
+-rw-r--r--   0        0        0     2756 2023-07-30 04:37:48.602570 jobbergate_api-3.6.0/jobbergate_api/tests/apps/conftest.py
+-rw-r--r--   0        0        0       42 2023-07-30 04:37:48.602570 jobbergate_api-3.6.0/jobbergate_api/tests/apps/job_scripts/__init__.py
+-rw-r--r--   0        0        0     1376 2023-07-30 04:37:48.602570 jobbergate_api-3.6.0/jobbergate_api/tests/apps/job_scripts/conftest.py
+-rw-r--r--   0        0        0    11518 2023-07-30 04:37:48.602570 jobbergate_api-3.6.0/jobbergate_api/tests/apps/job_scripts/test_job_script_files.py
+-rw-r--r--   0        0        0    56571 2023-07-30 04:37:48.602570 jobbergate_api-3.6.0/jobbergate_api/tests/apps/job_scripts/test_routers.py
+-rw-r--r--   0        0        0       46 2023-07-30 04:37:48.602570 jobbergate_api-3.6.0/jobbergate_api/tests/apps/job_submissions/__init__.py
+-rw-r--r--   0        0        0    24841 2023-07-30 04:37:48.602570 jobbergate_api-3.6.0/jobbergate_api/tests/apps/job_submissions/test_properties_parser.py
+-rw-r--r--   0        0        0    84061 2023-07-30 04:37:48.602570 jobbergate_api-3.6.0/jobbergate_api/tests/apps/job_submissions/test_routers.py
+-rw-r--r--   0        0        0      511 2023-07-30 04:37:48.602570 jobbergate_api-3.6.0/jobbergate_api/tests/apps/test_main.py
+-rw-r--r--   0        0        0     9724 2023-07-30 04:37:48.602570 jobbergate_api-3.6.0/jobbergate_api/tests/conftest.py
+-rw-r--r--   0        0        0     4503 2023-07-30 04:37:48.602570 jobbergate_api-3.6.0/jobbergate_api/tests/integration/draft_test_jobbergate_slurm_job_properties.py
+-rw-r--r--   0        0        0     3215 2023-07-30 04:37:48.602570 jobbergate_api-3.6.0/jobbergate_api/tests/test_config.py
+-rw-r--r--   0        0        0     4974 2023-07-30 04:37:48.602570 jobbergate_api-3.6.0/jobbergate_api/tests/test_email_notification.py
+-rw-r--r--   0        0        0     3177 2023-07-30 04:37:48.602570 jobbergate_api-3.6.0/jobbergate_api/tests/test_meta_mapper.py
+-rw-r--r--   0        0        0    12498 2023-07-30 04:37:48.602570 jobbergate_api-3.6.0/jobbergate_api/tests/test_multi_tenancy.py
+-rw-r--r--   0        0        0     3668 2023-07-30 04:37:48.602570 jobbergate_api-3.6.0/jobbergate_api/tests/test_pagination.py
+-rw-r--r--   0        0        0     1146 2023-07-30 04:37:48.602570 jobbergate_api-3.6.0/jobbergate_api/tests/test_s3_manager.py
+-rw-r--r--   0        0        0     4883 2023-07-30 04:37:48.602570 jobbergate_api-3.6.0/jobbergate_api/tests/test_security.py
+-rw-r--r--   0        0        0     6796 2023-07-30 04:37:48.606570 jobbergate_api-3.6.0/jobbergate_api/tests/test_storage.py
+-rw-r--r--   0        0        0     2777 2023-07-30 04:37:48.606570 jobbergate_api-3.6.0/jobbergate_api/tests/test_version.py
+-rw-r--r--   0        0        0     1102 2023-07-30 04:37:48.606570 jobbergate_api-3.6.0/jobbergate_api/version.py
+-rw-r--r--   0        0        0     2927 2023-07-30 04:37:48.606570 jobbergate_api-3.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2746 1970-01-01 00:00:00.000000 jobbergate_api-3.6.0/PKG-INFO
```

### Comparing `jobbergate_api-3.5.0a7/LICENSE` & `jobbergate_api-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a7/README.rst` & `jobbergate_api-3.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a7/jobbergate_api/apps/applications/application_files.py` & `jobbergate_api-3.6.0/jobbergate_api/apps/applications/application_files.py`

 * *Files 9% similar despite different names*

```diff
@@ -39,20 +39,20 @@
     source_file: Optional[str] = Field(None, alias="application_source_file")
     templates: Dict[str, str] = Field(default_factory=dict, alias="application_templates")
 
     class Config:
         allow_population_by_field_name = True
 
     @classmethod
-    def get_from_s3(cls, application_id: int):
+    def get_from_s3(cls, application_id: int, override_bucket_name: Optional[str] = None):
         """
         Alternative method to initialize the model getting the objects from S3.
         """
         logger.debug(f"Getting application files from S3: {application_id=}")
-        file_manager = cls.file_manager_factory(application_id)
+        file_manager = cls.file_manager_factory(application_id, override_bucket_name=override_bucket_name)
 
         logger.debug(
             f"The number of files available for {application_id=} is {len(file_manager)}. "
             f"They are: {', '.join(map(str, file_manager.keys()))}"
         )
 
         application_files = cls(
@@ -69,33 +69,39 @@
             logger.warning(f"No template file was found for {application_id=}")
 
         logger.debug("Success getting application files from S3")
 
         return application_files
 
     @classmethod
-    def delete_from_s3(cls, application_id: int):
+    def delete_from_s3(cls, application_id: int, override_bucket_name: Optional[str] = None):
         """
         Delete the files associated with the given id.
         """
-        file_manager = cls.file_manager_factory(application_id)
+        file_manager = cls.file_manager_factory(application_id, override_bucket_name=override_bucket_name)
         logger.debug(
             f"Deleting from S3 the files associated to {application_id=}. "
             f"Files to be deleted: {', '.join(map(str, file_manager.keys()))}"
         )
         file_manager.clear()
         logger.debug(f"Files were deleted for {application_id=}")
 
-    def write_to_s3(self, application_id: int, *, remove_previous_files: bool = True):
+    def write_to_s3(
+        self,
+        application_id: int,
+        *,
+        remove_previous_files: bool = True,
+        override_bucket_name: Optional[str] = None,
+    ):
         """
         Write to s3 the files associated with a given id.
         """
         logger.debug(f"Writing the application files to S3: {application_id=}")
 
-        file_manager = self.file_manager_factory(application_id)
+        file_manager = self.file_manager_factory(application_id, override_bucket_name=override_bucket_name)
 
         if remove_previous_files and file_manager:
             self.delete_from_s3(application_id)
 
         if self.config_file:
             path = Path(APPLICATION_CONFIG_FILE_NAME)
             file_manager[path] = self.config_file
@@ -133,22 +139,24 @@
                 application_files.templates[filename] = file_data
 
         logger.debug("Success getting application files from the uploaded files")
 
         return application_files
 
     @classmethod
-    def file_manager_factory(self, application_id: int) -> FileManager:
+    def file_manager_factory(
+        self, application_id: int, override_bucket_name: Optional[str] = None
+    ) -> FileManager:
         """
         Build an application file manager.
         """
         return cast(
             FileManager,
             file_manager_factory(
                 id=application_id,
                 s3_client=s3_client,
-                bucket_name=settings.S3_BUCKET_NAME,
+                bucket_name=settings.S3_BUCKET_NAME if override_bucket_name is None else override_bucket_name,
                 work_directory=Path(APPLICATIONS_WORK_DIR),
                 manager_cls=FileManager,
                 transformations=IO_TRANSFORMATIONS,
             ),
         )
```

### Comparing `jobbergate_api-3.5.0a7/jobbergate_api/apps/applications/file_validation.py` & `jobbergate_api-3.6.0/jobbergate_api/apps/applications/file_validation.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a7/jobbergate_api/apps/applications/models.py` & `jobbergate_api-3.6.0/jobbergate_api/apps/applications/models.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a7/jobbergate_api/apps/applications/schemas.py` & `jobbergate_api-3.6.0/jobbergate_api/apps/applications/schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,15 +172,15 @@
 class ApplicationCreateRequest(BaseModel):
     """
     Request model for creating Application instances.
     """
 
     application_name: str
     application_identifier: Optional[str]
-    application_description: Optional[str] = None
+    application_description: Optional[str]
 
     class Config:
         schema_extra = application_meta_mapper
 
 
 class ApplicationUpdateRequest(BaseModel):
     """
```

### Comparing `jobbergate_api-3.5.0a7/jobbergate_api/apps/job_scripts/job_script_files.py` & `jobbergate_api-3.6.0/jobbergate_api/apps/job_scripts/job_script_files.py`

 * *Files 4% similar despite different names*

```diff
@@ -156,20 +156,20 @@
         main_file_path = Path(".", upload_file.filename)
         return cls(
             main_file_path=main_file_path,
             files={main_file_path: upload_file.file.read().decode("utf-8")},
         )
 
     @classmethod
-    def get_from_s3(cls, job_script_id: int):
+    def get_from_s3(cls, job_script_id: int, override_bucket_name: Optional[str] = None):
         """
         Alternative method to initialize the model getting the objects from S3.
         """
         logger.debug(f"Getting job-script files from S3: {job_script_id=}")
-        file_manager = cls.file_manager_factory(job_script_id)
+        file_manager = cls.file_manager_factory(job_script_id, override_bucket_name=override_bucket_name)
 
         files = {}
         main_file_path = None
         main_file_counter = 0
 
         for s3_path in file_manager.keys():
             foldername = s3_path.parts[0]
@@ -190,33 +190,39 @@
         jobscript_files = cls(main_file_path=main_file_path, files=files)
 
         logger.debug(f"Done getting job-script files from S3: {job_script_id=}")
 
         return jobscript_files
 
     @classmethod
-    def delete_from_s3(cls, job_script_id: int):
+    def delete_from_s3(cls, job_script_id: int, override_bucket_name: Optional[str] = None):
         """
         Delete the files associated with the given id.
         """
-        file_manager = cls.file_manager_factory(job_script_id)
+        file_manager = cls.file_manager_factory(job_script_id, override_bucket_name=override_bucket_name)
         logger.debug(
             f"Deleting from S3 the files associated to {job_script_id=}. "
             f"Files to be deleted: {', '.join(map(str, file_manager.keys()))}"
         )
         file_manager.clear()
         logger.debug(f"Files were deleted for {job_script_id=}")
 
-    def write_to_s3(self, job_script_id: int, *, remove_previous_files: bool = True):
+    def write_to_s3(
+        self,
+        job_script_id: int,
+        *,
+        remove_previous_files: bool = True,
+        override_bucket_name: Optional[str] = None,
+    ):
         """
         Write to s3 the files associated with a given id.
         """
         logger.debug(f"Writing job-script files to S3: {job_script_id=}")
 
-        file_manager = self.file_manager_factory(job_script_id)
+        file_manager = self.file_manager_factory(job_script_id, override_bucket_name=override_bucket_name)
 
         if remove_previous_files and file_manager:
             self.delete_from_s3(job_script_id)
 
         for dict_path, content in self.files.items():
             if dict_path == self.main_file_path:
                 s3_path = JOBSCRIPTS_MAIN_FILE_FOLDER / dict_path
@@ -313,22 +319,24 @@
                         ).render(data=param_dict_flat)
 
         logger.debug("Done rendering job-script files from an application")
 
         return jobscript_files
 
     @classmethod
-    def file_manager_factory(cls, job_script_id: int) -> FileManager:
+    def file_manager_factory(
+        cls, job_script_id: int, override_bucket_name: Optional[str] = None
+    ) -> FileManager:
         """
         Build an application file manager.
         """
         return cast(
             FileManager,
             file_manager_factory(
                 id=job_script_id,
                 s3_client=s3_client,
-                bucket_name=settings.S3_BUCKET_NAME,
+                bucket_name=settings.S3_BUCKET_NAME if override_bucket_name is None else override_bucket_name,
                 work_directory=Path(JOBSCRIPTS_WORK_DIR),
                 manager_cls=FileManager,
                 transformations=IO_TRANSFORMATIONS,
             ),
         )
```

### Comparing `jobbergate_api-3.5.0a7/jobbergate_api/apps/job_scripts/models.py` & `jobbergate_api-3.6.0/jobbergate_api/apps/job_scripts/models.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a7/jobbergate_api/apps/job_scripts/schemas.py` & `jobbergate_api-3.6.0/jobbergate_api/apps/job_scripts/schemas.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a7/jobbergate_api/apps/job_submissions/constants.py` & `jobbergate_api-3.6.0/jobbergate_api/apps/job_submissions/constants.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a7/jobbergate_api/apps/job_submissions/models.py` & `jobbergate_api-3.6.0/jobbergate_api/apps/job_submissions/models.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a7/jobbergate_api/apps/job_submissions/properties_parser.py` & `jobbergate_api-3.6.0/jobbergate_api/apps/job_submissions/properties_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Parser for Slurm REST API parameters from SBATCH parameters at the job script file.
 """
 from argparse import ArgumentParser
 from dataclasses import dataclass, field
 from itertools import chain
 from shlex import split
-from typing import Any, Dict, List, Union
+from typing import Any, Dict, List, Optional, Union
 
 from bidict import bidict
 from loguru import logger
 
 from jobbergate_api.apps.job_scripts.job_script_files import JobScriptFiles
 from jobbergate_api.apps.job_submissions.schemas import JobProperties
 
@@ -286,22 +286,24 @@
     Parse all SBATCH parameters from a job script, map their names to Slurm API parameters.
 
     They are returned as a key-value pairing dictionary.
     """
     return convert_sbatch_to_slurm_api(jobscript_to_dict(jobscript))
 
 
-def get_job_properties_from_job_script(job_script_id: int, **kwargs) -> JobProperties:
+def get_job_properties_from_job_script(
+    job_script_id: int, bucket_name: Optional[str] = None, **kwargs
+) -> JobProperties:
     """
     Get the job properties for Slurm REST API from a job script file, given its id.
 
     Extra keyword arguments can be used to overwrite any parameter from the
     job script, like name or current_working_directory.
     """
-    job_script_files = JobScriptFiles.get_from_s3(job_script_id)
+    job_script_files = JobScriptFiles.get_from_s3(job_script_id, override_bucket_name=bucket_name)
     slurm_parameters = get_job_parameters(job_script_files.main_file)
     merged_parameters = {**slurm_parameters, **kwargs}
     return JobProperties.parse_obj(merged_parameters)
 
 
 parser = build_parser()
 mapping_sbatch_to_slurm = build_mapping_sbatch_to_slurm()
```

### Comparing `jobbergate_api-3.5.0a7/jobbergate_api/apps/job_submissions/routers.py` & `jobbergate_api-3.6.0/jobbergate_api/apps/job_submissions/routers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """
 Router for the JobSubmission resource.
 """
 from typing import Any, Dict, List, Optional
 
-from armasec import TokenPayload
 from fastapi import APIRouter, Body, Depends, HTTPException, Query, status
 from loguru import logger
-from sqlalchemy import join, select
+from sqlalchemy.future import select
 
 from jobbergate_api.apps.applications.models import applications_table
 from jobbergate_api.apps.job_scripts.job_script_files import JobScriptFiles
 from jobbergate_api.apps.job_scripts.models import job_scripts_table
 from jobbergate_api.apps.job_submissions.constants import JobSubmissionStatus
 from jobbergate_api.apps.job_submissions.models import (
     job_submissions_table,
@@ -22,161 +21,166 @@
     ActiveJobSubmission,
     JobSubmissionCreateRequest,
     JobSubmissionResponse,
     JobSubmissionUpdateRequest,
     PendingJobSubmission,
 )
 from jobbergate_api.apps.permissions import Permissions, check_owner
+from jobbergate_api.config import settings
 from jobbergate_api.email_notification import notify_submission_rejected
 from jobbergate_api.pagination import Pagination, ok_response, package_response
-from jobbergate_api.security import IdentityClaims, guard
 from jobbergate_api.storage import (
     INTEGRITY_CHECK_EXCEPTIONS,
-    database,
+    SecureSession,
+    fetch_data,
+    fetch_instance,
     render_sql,
     search_clause,
+    secure_session,
     sort_clause,
 )
 
 router = APIRouter()
 
 
-async def _fetch_job_submission_by_id(job_submission_id: int) -> JobSubmissionResponse:
+async def _fetch_job_submission_by_id(
+    secure_session: SecureSession,
+    job_submission_id: int,
+) -> JobSubmissionResponse:
     """
     Fetch a job_submission from the database by its id.
     """
-    select_query = job_submissions_table.select().where(job_submissions_table.c.id == job_submission_id)
-    raw_job_submission = await database.fetch_one(select_query)
+    return await fetch_instance(
+        secure_session.session, job_submission_id, job_submissions_table, JobSubmissionResponse
+    )
 
-    if not raw_job_submission:
-        message = f"Job Submission with {job_submission_id=} was not found."
-        logger.error(message)
-        raise HTTPException(status_code=status.HTTP_404_NOT_FOUND, detail=message)
 
-    return JobSubmissionResponse.parse_obj(raw_job_submission)
+def _get_override_bucket_name(secure_session: SecureSession) -> Optional[str]:
+    """
+    Get the override_bucket_name based on organization_id if multi-tenancy is enabled.
+    """
+    if settings.MULTI_TENANCY_ENABLED:
+        return secure_session.identity_payload.organization_id
+    return None
 
 
 @router.post(
     "/job-submissions",
     status_code=201,
     description="Endpoint for job_submission creation",
     response_model=JobSubmissionResponse,
 )
 async def job_submission_create(
     job_submission: JobSubmissionCreateRequest,
-    token_payload: TokenPayload = Depends(guard.lockdown(Permissions.JOB_SUBMISSIONS_EDIT)),
+    secure_session: SecureSession = Depends(secure_session(Permissions.JOB_SUBMISSIONS_EDIT)),
 ):
     """
     Create a new job submission.
 
     Make a post request to this endpoint with the required values to create a new job submission.
     """
     logger.debug(f"Creating {job_submission=}")
 
-    identity_claims = IdentityClaims.from_token_payload(token_payload)
-    client_id = job_submission.client_id or identity_claims.client_id
+    client_id = job_submission.client_id or secure_session.identity_payload.client_id
     if client_id is None:
         message = "Could not find a client_id in the request body or auth token."
         logger.warning(message)
         raise HTTPException(
             status_code=status.HTTP_400_BAD_REQUEST,
             detail=message,
         )
 
     new_job_submission_data: Dict[str, Any] = dict(
         **job_submission.dict(exclude_unset=True),
-        job_submission_owner_email=identity_claims.email,
+        job_submission_owner_email=secure_session.identity_payload.email,
         status=JobSubmissionStatus.CREATED,
     )
     if job_submission.client_id is None:
         new_job_submission_data.update(client_id=client_id)
 
     exec_dir = new_job_submission_data.pop("execution_directory", None)
     if exec_dir is not None:
         new_job_submission_data.update(execution_directory=str(exec_dir))
 
-    select_query = job_scripts_table.select().where(job_scripts_table.c.id == job_submission.job_script_id)
-    logger.trace(f"job_scripts select_query = {render_sql(select_query)}")
-    raw_job_script = await database.fetch_one(select_query)
-
-    if not raw_job_script:
-        message = f"JobScript id={job_submission.job_script_id} not found."
-        logger.warning(message)
-        raise HTTPException(
-            status_code=status.HTTP_404_NOT_FOUND,
-            detail=message,
-        )
+    job_script_data = await fetch_data(
+        secure_session.session,
+        job_submission.job_script_id,
+        job_scripts_table,
+        trace_query=True,
+    )
 
     try:
         job_properties = get_job_properties_from_job_script(
-            job_submission.job_script_id, **job_submission.execution_parameters.dict(exclude_unset=True)
+            job_submission.job_script_id,
+            _get_override_bucket_name(secure_session=secure_session),
+            **job_submission.execution_parameters.dict(exclude_unset=True),
         )
         new_job_submission_data["execution_parameters"] = job_properties.dict(exclude_unset=True)
     except Exception as e:
         message = f"Error extracting execution parameters from job script: {str(e)}"
         logger.error(message)
         raise HTTPException(status_code=status.HTTP_422_UNPROCESSABLE_ENTITY, detail=message)
 
     logger.debug("Inserting job-submission")
 
-    async with database.transaction():
-        try:
-            insert_query = job_submissions_table.insert().returning(job_submissions_table)
-            logger.trace(f"job_submissions insert_query = {render_sql(insert_query)}")
-            job_submission_data = await database.fetch_one(query=insert_query, values=new_job_submission_data)
-
-        except INTEGRITY_CHECK_EXCEPTIONS as e:
-            logger.error(f"Reverting database transaction: {str(e)}")
-            raise HTTPException(status_code=status.HTTP_422_UNPROCESSABLE_ENTITY, detail=str(e))
-
-    logger.debug(f"Job-submission created: {job_submission_data=}")
+    try:
+        insert_query = job_submissions_table.insert().returning(job_submissions_table)
+        logger.trace(f"job_submissions insert_query = {render_sql(secure_session.session, insert_query)}")
+        raw_result = await secure_session.session.execute(insert_query, new_job_submission_data)
+
+    except INTEGRITY_CHECK_EXCEPTIONS as e:
+        logger.error(f"Reverting database transaction: {str(e)}")
+        raise HTTPException(status_code=status.HTTP_422_UNPROCESSABLE_ENTITY, detail=str(e))
+
+    new_job_submission = JobSubmissionResponse.from_orm(raw_result.one())
+    new_job_submission.job_script_name = job_script_data.job_script_name
+    logger.debug(f"Job-submission created: {new_job_submission=}")
 
-    return JobSubmissionResponse(
-        **job_submission_data, job_script_name=raw_job_script.get("job_script_name")  # type: ignore
-    )
+    return new_job_submission
 
 
 @router.get(
     "/job-submissions/{job_submission_id}",
     description="Endpoint to get a job_submission",
     response_model=JobSubmissionResponse,
-    dependencies=[Depends(guard.lockdown(Permissions.JOB_SUBMISSIONS_VIEW))],
 )
-async def job_submission_get(job_submission_id: int = Query(...)):
+async def job_submission_get(
+    job_submission_id: int = Query(...),
+    secure_session: SecureSession = Depends(secure_session(Permissions.JOB_SUBMISSIONS_VIEW)),
+):
     """
     Return the job_submission given it's id.
     """
     logger.debug(f"Getting {job_submission_id=}")
 
     query = (
-        select([job_submissions_table, job_scripts_table.c.job_script_name])
-        .select_from(
-            join(
-                job_submissions_table,
-                job_scripts_table,
-                job_submissions_table.c.job_script_id == job_scripts_table.c.id,
-                isouter=True,
-            )
-        )
+        select(job_submissions_table.c, job_scripts_table.c.job_script_name)
         .where(job_submissions_table.c.id == job_submission_id)
+        .join(
+            job_scripts_table,
+            job_scripts_table.columns.id == job_submissions_table.columns.job_script_id,
+            isouter=True,
+        )
     )
-    logger.trace(f"query = {render_sql(query)}")
-    job_submission_data = await database.fetch_one(query)
+    logger.trace(f"query = {render_sql(secure_session.session, query)}")
+    raw_result = await secure_session.session.execute(query)
+    job_submission_data = raw_result.one_or_none()
 
     if not job_submission_data:
         message = f"JobSubmission with id={job_submission_id} not found."
         logger.warning(message)
         raise HTTPException(
             status_code=status.HTTP_404_NOT_FOUND,
             detail=message,
         )
 
-    logger.debug(f"Job-submission data: {job_submission_data=}")
+    job_submission = JobSubmissionResponse.from_orm(job_submission_data)
+    logger.debug(f"Job-submission data: {job_submission}")
 
-    return JobSubmissionResponse(**job_submission_data)  # type: ignore
+    return job_submission
 
 
 @router.get(
     "/job-submissions",
     description="Endpoint to list job_submissions",
     responses=ok_response(JobSubmissionResponse),
 )
@@ -197,37 +201,30 @@
     search: Optional[str] = Query(None),
     sort_field: Optional[str] = Query(None),
     from_job_script_id: Optional[int] = Query(
         None,
         description="Filter job-submissions by the job-script-id they were created from.",
     ),
     sort_ascending: bool = Query(True),
-    token_payload: TokenPayload = Depends(guard.lockdown(Permissions.JOB_SUBMISSIONS_VIEW)),
+    secure_session: SecureSession = Depends(secure_session(Permissions.JOB_SUBMISSIONS_VIEW)),
 ):
     """
     List job_submissions for the authenticated user.
     """
     logger.debug("Fetching job submissions")
-    identity_claims = IdentityClaims.from_token_payload(token_payload)
-    logger.debug(f"Extracted identity claims from token: {identity_claims}")
-    query = select([job_submissions_table, job_scripts_table.c.job_script_name]).select_from(
-        join(
-            job_submissions_table,
-            job_scripts_table,
-            job_submissions_table.c.job_script_id == job_scripts_table.c.id,
-            isouter=True,
-        )
-    )
 
     logger.debug("Building query")
+    query = select(job_submissions_table.c, job_scripts_table.c.job_script_name)
     if submit_status:
         query = query.where(job_submissions_table.c.status == submit_status)
 
     if not all:
-        query = query.where(job_submissions_table.c.job_submission_owner_email == identity_claims.email)
+        query = query.where(
+            job_submissions_table.c.job_submission_owner_email == secure_session.identity_payload.email
+        )
 
     if from_job_script_id is not None:
         query = query.where(job_submissions_table.c.job_script_id == from_job_script_id)
     if slurm_job_ids is not None and slurm_job_ids != "":
         try:
             job_ids = [int(i) for i in slurm_job_ids.split(",")]
         except Exception:
@@ -239,68 +236,76 @@
     if search is not None:
         query = query.where(search_clause(search, searchable_fields))
     if sort_field is not None:
         query = query.order_by(sort_clause(sort_field, sortable_fields, sort_ascending))
     else:
         query = query.order_by(job_submissions_table.c.id.asc())
 
-    logger.trace(f"Query built as: {render_sql(query)}")
+    full_query = query.join(
+        job_scripts_table,
+        job_scripts_table.columns.id == job_submissions_table.columns.job_script_id,
+        isouter=True,
+    )
+
+    logger.trace(f"Query built as: {render_sql(secure_session.session, full_query)}")
 
     logger.debug("Awaiting query and response package")
-    response = await package_response(JobSubmissionResponse, query, pagination)
+    response = await package_response(secure_session.session, JobSubmissionResponse, full_query, pagination)
+
     logger.debug(f"Response built as: {response}")
     return response
 
 
 @router.delete(
     "/job-submissions/{job_submission_id}",
     status_code=status.HTTP_204_NO_CONTENT,
     description="Endpoint to delete job submission",
 )
 async def job_submission_delete(
     job_submission_id: int = Query(..., description="id of the job submission to delete"),
-    token_payload: TokenPayload = Depends(guard.lockdown(Permissions.JOB_SUBMISSIONS_EDIT)),
+    secure_session: SecureSession = Depends(secure_session(Permissions.JOB_SUBMISSIONS_EDIT)),
 ):
     """
     Delete job_submission given its id.
     """
     logger.debug(f"Deleting {job_submission_id=}")
 
-    identity_claims = IdentityClaims.from_token_payload(token_payload)
-    job_submission = await _fetch_job_submission_by_id(job_submission_id)
+    job_submission = await _fetch_job_submission_by_id(secure_session, job_submission_id)
     check_owner(
-        job_submission.job_submission_owner_email, identity_claims.email, job_submission_id, "job_submission"
+        job_submission.job_submission_owner_email,
+        secure_session.identity_payload.email,
+        job_submission_id,
+        "job_submission",
     )
 
     delete_query = job_submissions_table.delete().where(job_submissions_table.c.id == job_submission_id)
-    logger.trace(f"delete_query = {render_sql(delete_query)}")
-    await database.execute(delete_query)
+    logger.trace(f"delete_query = {render_sql(secure_session.session, delete_query)}")
+    await secure_session.session.execute(delete_query)
 
 
 @router.put(
     "/job-submissions/{job_submission_id}",
     status_code=status.HTTP_200_OK,
     description="Endpoint to update a job_submission given the id",
     response_model=JobSubmissionResponse,
 )
 async def job_submission_update(
     job_submission_id: int,
     job_submission: JobSubmissionUpdateRequest,
-    token_payload: TokenPayload = Depends(guard.lockdown(Permissions.JOB_SUBMISSIONS_EDIT)),
+    secure_session: SecureSession = Depends(secure_session(Permissions.JOB_SUBMISSIONS_EDIT)),
 ):
     """
     Update a job_submission given its id.
     """
     logger.debug(f"Updating {job_submission_id=}")
 
-    identity_claims = IdentityClaims.from_token_payload(token_payload)
-    old_job_submission = await _fetch_job_submission_by_id(job_submission_id)
+    old_job_submission = await _fetch_job_submission_by_id(secure_session, job_submission_id)
     check_owner(
         old_job_submission.job_submission_owner_email,
-        identity_claims.email,
+        secure_session.identity_payload.email,
         job_submission_id,
         "job_submission",
     )
 
     update_dict = job_submission.dict(exclude_unset=True)
     exec_dir = update_dict.pop("execution_directory", None)
     if exec_dir is not None:
@@ -308,92 +313,97 @@
 
     update_query = (
         job_submissions_table.update()
         .where(job_submissions_table.c.id == job_submission_id)
         .values(update_dict)
         .returning(job_submissions_table)
     )
-    logger.trace(f"update_query = {render_sql(update_query)}")
-    async with database.transaction():
-        try:
-            job_submission_data = await database.fetch_one(update_query)
+    logger.trace(f"update_query = {render_sql(secure_session.session, update_query)}")
+    try:
+        raw_result = await secure_session.session.execute(update_query)
+    except INTEGRITY_CHECK_EXCEPTIONS as e:
+        logger.error(f"Reverting database transaction: {str(e)}")
+        raise HTTPException(status_code=status.HTTP_409_CONFLICT, detail=str(e))
 
-        except INTEGRITY_CHECK_EXCEPTIONS as e:
-            logger.error(f"Reverting database transaction: {str(e)}")
-            raise HTTPException(status_code=status.HTTP_409_CONFLICT, detail=str(e))
-
-        if not job_submission_data:
-            message = f"JobSubmission with id={job_submission_id} not found."
-            logger.warning(message)
-            raise HTTPException(
-                status_code=status.HTTP_404_NOT_FOUND,
-                detail=message,
-            )
+    job_submission_data = raw_result.one_or_none()
+    if not job_submission_data:
+        message = f"JobSubmission with id={job_submission_id} not found."
+        logger.warning(message)
+        raise HTTPException(
+            status_code=status.HTTP_404_NOT_FOUND,
+            detail=message,
+        )
 
-    return JobSubmissionResponse(**job_submission_data)  # type: ignore
+    return job_submission_data
 
 
 # The "agent" routes are used for agents to fetch pending job submissions and update their statuses
 @router.get(
     "/job-submissions/agent/pending",
     description="Endpoint to list pending job_submissions for the requesting client",
     response_model=List[PendingJobSubmission],
 )
 async def job_submissions_agent_pending(
-    token_payload: TokenPayload = Depends(guard.lockdown(Permissions.JOB_SUBMISSIONS_VIEW)),
+    secure_session: SecureSession = Depends(secure_session(Permissions.JOB_SUBMISSIONS_VIEW)),
 ):
     """
     Get a list of pending job submissions for the cluster-agent.
     """
     logger.debug("Agent is requesting a list of pending job submissions")
 
-    identity_claims = IdentityClaims.from_token_payload(token_payload)
-    if identity_claims.client_id is None:
+    if secure_session.identity_payload.client_id is None:
         message = "Access token does not contain a `client_id`. Cannot fetch pending submissions"
         logger.warning(message)
         raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST, detail=message)
 
-    logger.info(f"Fetching newly created job_submissions for client_id: {identity_claims.client_id}")
+    logger.info(
+        f"Fetching newly created job_submissions for client_id: {secure_session.identity_payload.client_id}"
+    )
 
     query = (
         select(
-            columns=[
-                job_submissions_table.c.id,
-                job_submissions_table.c.job_submission_name,
-                job_submissions_table.c.job_submission_owner_email,
-                job_submissions_table.c.execution_directory,
-                job_submissions_table.c.execution_parameters,
-                job_submissions_table.c.job_script_id,
-                job_scripts_table.c.job_script_name,
-                applications_table.c.application_name,
-            ]
-        )
-        .select_from(job_submissions_table.join(job_scripts_table).join(applications_table))
-        .where(
-            job_submissions_table.c.status == JobSubmissionStatus.CREATED,
+            job_submissions_table.c.id,
+            job_submissions_table.c.job_submission_name,
+            job_submissions_table.c.job_submission_owner_email,
+            job_submissions_table.c.execution_directory,
+            job_submissions_table.c.execution_parameters,
+            job_submissions_table.c.job_script_id,
+            job_scripts_table.c.job_script_name,
+            applications_table.c.application_name,
+        )
+        .where(job_submissions_table.c.status == JobSubmissionStatus.CREATED)
+        .where(job_submissions_table.c.client_id == secure_session.identity_payload.client_id)
+        .join(
+            job_scripts_table,
+            job_scripts_table.columns.id == job_submissions_table.columns.job_script_id,
+            isouter=True,
         )
-        .where(
-            job_submissions_table.c.client_id == identity_claims.client_id,
+        .join(
+            applications_table,
+            applications_table.columns.id == job_scripts_table.columns.application_id,
+            isouter=True,
         )
     )
-    logger.trace(f"query = {render_sql(query)}")
-    rows = await database.fetch_all(query)
+
+    logger.trace(f"query = {render_sql(secure_session.session, query)}")
+    raw_result = await secure_session.session.execute(query)
+    rows = raw_result.fetchall()
 
     response = []
     missing_ids = set()
 
     for row in rows:
+        jobscript_id = row.job_script_id
         try:
-            jobscript_id = int(row["job_script_id"])
             job_script_files = JobScriptFiles.get_from_s3(jobscript_id)
         except (KeyError, ValueError) as e:
             logger.error(f"Error getting files for {jobscript_id=}: {str(e)}")
             missing_ids.add(jobscript_id)
         else:
-            response.append(PendingJobSubmission(**row, job_script_files=job_script_files))
+            response.append(PendingJobSubmission(**row._mapping, job_script_files=job_script_files))
 
     if missing_ids:
         message = f"JobScript file(s) not found, the missing ids are: {', '.join(map(str, missing_ids))}"
         logger.error(message)
         raise HTTPException(
             status_code=status.HTTP_404_NOT_FOUND,
             detail=message,
@@ -409,105 +419,105 @@
     response_model=JobSubmissionResponse,
 )
 async def job_submission_agent_update(
     job_submission_id: int,
     new_status: str = Body(..., embed=True),
     slurm_job_id: Optional[int] = Body(None, embed=True),
     report_message: Optional[str] = Body(None, embed=True),
-    token_payload: TokenPayload = Depends(guard.lockdown(Permissions.JOB_SUBMISSIONS_EDIT)),
+    secure_session: SecureSession = Depends(secure_session(Permissions.JOB_SUBMISSIONS_EDIT)),
 ):
     """
     Update a job_submission with a new status.
 
     Make a put request to this endpoint with the new status to update a job_submission.
     """
     logger.debug(f"Agent is requesting to update {job_submission_id=}")
 
-    identity_claims = IdentityClaims.from_token_payload(token_payload)
-    if identity_claims.client_id is None:
+    if secure_session.identity_payload.client_id is None:
         logger.error("Access token does not contain a client_id")
         raise HTTPException(
             status_code=status.HTTP_400_BAD_REQUEST,
             detail="Access token does not contain a `client_id`. Cannot update job_submission",
         )
 
     logger.info(
         f"Setting status to: {new_status} "
         f"for job_submission: {job_submission_id} "
-        f"on client_id: {identity_claims.client_id}"
+        f"on client_id: {secure_session.identity_payload.client_id}"
     )
 
     update_values: Dict[str, Any] = dict(status=new_status)
     if slurm_job_id is not None:
         update_values.update(slurm_job_id=slurm_job_id)
 
     if report_message:
         update_values.update(report_message=report_message)
 
     update_query = (
         job_submissions_table.update()
         .where(job_submissions_table.c.id == job_submission_id)
-        .where(job_submissions_table.c.client_id == identity_claims.client_id)
+        .where(job_submissions_table.c.client_id == secure_session.identity_payload.client_id)
         .values(**update_values)
         .returning(job_submissions_table)
     )
-    logger.trace(f"update_query = {render_sql(update_query)}")
-    job_submission_data = await database.fetch_one(update_query)
+    logger.trace(f"update_query = {render_sql(secure_session.session, update_query)}")
+
+    raw_result = await secure_session.session.execute(update_query)
+    job_submission_data = raw_result.one_or_none()
 
     if job_submission_data is None:
         message = (
             f"JobSubmission with id={job_submission_id} "
-            f"and client_id={identity_claims.client_id} not found."
+            f"and client_id={secure_session.identity_payload.client_id} not found."
         )
         logger.warning(message)
         raise HTTPException(
             status_code=status.HTTP_404_NOT_FOUND,
             detail=(message),
         )
 
     if report_message and new_status == JobSubmissionStatus.REJECTED:
         notify_submission_rejected(
-            job_submission_id, report_message, job_submission_data["job_submission_owner_email"]
+            job_submission_id, report_message, job_submission_data.job_submission_owner_email
         )
 
-    return JobSubmissionResponse(**job_submission_data)  # type: ignore
+    return job_submission_data
 
 
 @router.get(
     "/job-submissions/agent/active",
     description="Endpoint to list active job_submissions for the requesting client",
     response_model=List[ActiveJobSubmission],
 )
 async def job_submissions_agent_active(
-    token_payload: TokenPayload = Depends(guard.lockdown(Permissions.JOB_SUBMISSIONS_VIEW)),
+    secure_session: SecureSession = Depends(secure_session(Permissions.JOB_SUBMISSIONS_VIEW)),
 ):
     """
     Get a list of active job submissions for the cluster-agent.
     """
     logger.debug("Agent is requesting a list of active job submissions")
 
-    identity_claims = IdentityClaims.from_token_payload(token_payload)
-    if identity_claims.client_id is None:
+    if secure_session.identity_payload.client_id is None:
         logger.error("Access token does not contain a client_id")
         raise HTTPException(
             status_code=status.HTTP_400_BAD_REQUEST,
             detail="Access token does not contain a `client_id`. Cannot fetch pending submissions",
         )
 
-    logger.info(f"Fetching active job_submissions for client_id: {identity_claims.client_id}")
+    logger.info(f"Fetching active job_submissions for client_id: {secure_session.identity_payload.client_id}")
 
     query = (
         job_submissions_table.select()
         .where(job_submissions_table.c.status == JobSubmissionStatus.SUBMITTED)
-        .where(job_submissions_table.c.client_id == identity_claims.client_id)
+        .where(job_submissions_table.c.client_id == secure_session.identity_payload.client_id)
     )
-    logger.trace(f"query = {render_sql(query)}")
+    logger.trace(f"query = {render_sql(secure_session.session, query)}")
 
-    rows = await database.fetch_all(query)
-    return rows
+    raw_result = await secure_session.session.execute(query)
+    return raw_result.fetchall()
 
 
 def include_router(app):
     """
     Include the router for this module in the app.
     """
     app.include_router(router)
```

### Comparing `jobbergate_api-3.5.0a7/jobbergate_api/apps/job_submissions/schemas.py` & `jobbergate_api-3.6.0/jobbergate_api/apps/job_submissions/schemas.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """
 JobSubmission resource schema.
 """
 import re
 from datetime import datetime
 from pathlib import Path
-from typing import Dict, List, Literal, Optional
+from typing import Dict, List, Optional
 
 from pydantic import BaseModel, Extra, Field, validator
+from typing_extensions import Literal
 
 from jobbergate_api.apps.job_scripts.job_script_files import JobScriptFiles
 from jobbergate_api.apps.job_submissions.constants import JobSubmissionStatus
 from jobbergate_api.meta_mapper import MetaField, MetaMapper
 
 job_submission_meta_mapper = MetaMapper(
     id=MetaField(
@@ -347,15 +348,15 @@
     job_script_name: Optional[str] = None
 
     class Config:
         orm_mode = True
         schema_extra = job_submission_meta_mapper
 
 
-class PendingJobSubmission(BaseModel, extra=Extra.ignore):
+class PendingJobSubmission(BaseModel):
     """
     Specialized model for the cluster-agent to pull pending job_submissions.
 
     Model also includes data from its job_script and application sources.
     """
 
     id: Optional[int] = Field(None)
@@ -363,16 +364,24 @@
     job_submission_owner_email: str
     execution_directory: Optional[Path]
     execution_parameters: Dict = Field(default_factory=dict)
     job_script_name: str
     application_name: str
     job_script_files: JobScriptFiles
 
+    class Config:
+        extra = Extra.ignore
+        orm_mode = True
+
 
-class ActiveJobSubmission(BaseModel, extra=Extra.ignore):
+class ActiveJobSubmission(BaseModel):
     """
     Specialized model for the cluster-agent to pull an active job_submission.
     """
 
     id: int
     job_submission_name: str
     slurm_job_id: int
+
+    class Config:
+        extra = Extra.ignore
+        orm_mode = True
```

### Comparing `jobbergate_api-3.5.0a7/jobbergate_api/apps/permissions.py` & `jobbergate_api-3.6.0/jobbergate_api/apps/permissions.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a7/jobbergate_api/config.py` & `jobbergate_api-3.6.0/jobbergate_api/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -79,14 +79,17 @@
     # Maximum number of bytes allowed for file uploads
     MAX_UPLOAD_FILE_SIZE: int = 100 * 1024 * 1024  # 100 MB
 
     # Sendgrid configuration for email notification
     SENDGRID_FROM_EMAIL: Optional[str]
     SENDGRID_API_KEY: Optional[str]
 
+    # Enable multi-tenancy so that the database is determined by the client_id in the auth token
+    MULTI_TENANCY_ENABLED: bool = Field(False)
+
     @root_validator(pre=True)
     def remove_blank_env(cls, values):
         """
         Remove any settings from the environment that are blank strings.
 
         This allows the defaults to be set if ``docker-compose`` defaults a missing
         environment variable to a blank string.
```

### Comparing `jobbergate_api-3.5.0a7/jobbergate_api/email_notification.py` & `jobbergate_api-3.6.0/jobbergate_api/email_notification.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a7/jobbergate_api/main.py` & `jobbergate_api-3.6.0/jobbergate_api/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 """
 Main file to startup the fastapi server.
 """
 import sys
 import typing
+from contextlib import asynccontextmanager
 
 import asyncpg
 import sentry_sdk
 from fastapi import FastAPI, HTTPException, Request, Response, status
 from fastapi.exceptions import RequestValidationError
 from loguru import logger
 from sentry_sdk.integrations.asgi import SentryAsgiMiddleware
 from starlette.middleware.cors import CORSMiddleware
 
 from jobbergate_api import __version__
 from jobbergate_api.apps.applications.routers import router as applications_router
 from jobbergate_api.apps.job_scripts.routers import router as job_scripts_router
 from jobbergate_api.apps.job_submissions.routers import router as job_submissions_router
 from jobbergate_api.config import settings
-from jobbergate_api.storage import database, handle_fk_error
+from jobbergate_api.storage import engine_factory, handle_fk_error
 
 subapp = FastAPI(
     title="Jobbergate-API",
     version=__version__,
     contact={
         "name": "Omnivector Solutions",
         "url": "https://www.omnivector.solutions/",
@@ -67,44 +68,35 @@
     """
     Provide a health-check endpoint for the app.
     """
     logger.debug("CHECKING HEALTH")
     return Response(status_code=status.HTTP_204_NO_CONTENT)
 
 
-app = FastAPI()
-app.mount("/jobbergate", subapp)
+@asynccontextmanager
+async def lifespan(_: FastAPI):
+    """
+    Provide a lifespan context for the app.
 
+    Will set up logging and cleanup database engines when the app is shut down.
 
-@app.on_event("startup")
-def init_logger():
-    """
-    Initialize logging.
+    This is the preferred method of handling lifespan events in FastAPI.
+    For mor details, see: https://fastapi.tiangolo.com/advanced/events/
     """
     logger.remove()
     logger.add(sys.stderr, level=settings.LOG_LEVEL)
     logger.info(f"Logging configured 📝 Level: {settings.LOG_LEVEL}")
 
+    yield
 
-@app.on_event("startup")
-async def init_database():
-    """
-    Connect the database; create it if necessary.
-    """
-    logger.debug("Initializing database")
-    await database.connect()
+    await engine_factory.cleanup()
 
 
-@app.on_event("shutdown")
-async def disconnect_database():
-    """
-    Disconnect the database.
-    """
-    logger.debug("Disconnecting database")
-    await database.disconnect()
+app = FastAPI(lifespan=lifespan)
+app.mount("/jobbergate", subapp)
 
 
 @app.exception_handler(RequestValidationError)
 async def validation_exception_handler(request: Request, err: RequestValidationError):
     """
     Handle exceptions from pydantic validators.
     """
```

### Comparing `jobbergate_api-3.5.0a7/jobbergate_api/meta_mapper.py` & `jobbergate_api-3.6.0/jobbergate_api/meta_mapper.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a7/jobbergate_api/pagination.py` & `jobbergate_api-3.6.0/jobbergate_api/pagination.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 from typing import Dict, Generic, List, Optional, Type, TypeVar, Union
 
 from fastapi.encoders import jsonable_encoder
 from fastapi.responses import JSONResponse
 from pydantic import BaseModel, Field
 from pydantic.generics import GenericModel
 from sqlalchemy import func, select
-
-from jobbergate_api.storage import database
+from sqlalchemy.ext.asyncio import AsyncSession
 
 
 class Pagination(BaseModel):
     """
     Basic pagination class.
     """
 
@@ -76,15 +75,20 @@
     The typing is intense here, but is just basically saying that given some generic model input,
     return a dictionary that contains a ``Response`` for that model type.
 
     """
     return {200: {"model": Response[TResponseModel]}}
 
 
-async def package_response(model: Type[TResponseModel], query, pagination: Pagination) -> JSONResponse:
+async def package_response(
+    session: AsyncSession,
+    model: Type[TResponseModel],
+    query,
+    pagination: Pagination,
+) -> JSONResponse:
     """
     Package the response in an envelope that includes the response and the metadata.
 
     Return a JSONResponse containing the packaged data.
 
     Structure of response is::
 
@@ -98,17 +102,20 @@
         }
 
     If pagination.start is None, no pagination is performed
     """
     # The explicit order_by removes any sorting added to the query for the total computation
     # total = await database.fetch_val(query.with_only_columns([func.count()]).order_by(None))
     count_query = select(func.count()).select_from(query.subquery())
-    total = await database.fetch_val(query=count_query)
+    raw_response = await session.execute(count_query)
+    total = raw_response.scalar_one()
+
     if pagination.start is not None:
         query = query.limit(pagination.limit).offset(pagination.start * pagination.limit)
-    raw_response = await database.fetch_all(query)
+
+    raw_response = await session.execute(query)
     validated_response = Response[TResponseModel](
-        results=[model.parse_obj(x) for x in raw_response],
+        results=[model.from_orm(x) for x in raw_response],
         pagination=ResponsePagination(total=total, **pagination.dict()),
     )
     jsonable_response = jsonable_encoder(validated_response)
     return JSONResponse(content=jsonable_response)
```

### Comparing `jobbergate_api-3.5.0a7/jobbergate_api/s3_manager.py` & `jobbergate_api-3.6.0/jobbergate_api/s3_manager.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a7/jobbergate_api/security.py` & `jobbergate_api-3.6.0/jobbergate_api/security.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,16 +3,18 @@
 
 Also provides a factory function for TokenSecurity to reduce boilerplate.
 """
 from typing import List, Optional
 
 from armasec import Armasec, TokenPayload
 from armasec.schemas import DomainConfig
+from armasec.token_security import PermissionMode
+from fastapi import Depends
 from loguru import logger
-from pydantic import BaseModel, EmailStr
+from pydantic import EmailStr, root_validator
 
 from jobbergate_api.config import settings
 
 
 def get_domain_configs() -> List[DomainConfig]:
     """
     Return a list of DomainConfig objects based on the input variables for the Settings class.
@@ -45,29 +47,55 @@
 
 guard = Armasec(
     domain_configs=get_domain_configs(),
     debug_logger=logger.debug if settings.ARMASEC_DEBUG else None,
 )
 
 
-class IdentityClaims(BaseModel):
+class IdentityPayload(TokenPayload):
     """
-    Provide a pydantic data model containing user data extracted from an access token.
+    Provide an extension of TokenPayload that includes the user's identity.
     """
 
-    email: Optional[EmailStr]
-    client_id: Optional[str]
+    email: Optional[EmailStr] = None
+    organization_id: Optional[str] = None
 
-    @classmethod
-    def from_token_payload(cls, payload: TokenPayload) -> "IdentityClaims":
+    @root_validator(pre=True)
+    def extract_organization(cls, values):
         """
-        Create an instance from a Token payload.
+        Extract the organization_id from the organization payload.
 
-        Automatically validates that the email is an email address if it is provided.
+        The payload is expected to look like:
+        {
+            ...,
+            "organization": {
+                "adf99e01-5cd5-41ac-a1af-191381ad7780": {
+                    ...
+                }
+            }
+        }
         """
-        init_kwargs = dict(
-            client_id=payload.client_id,
-        )
-        email = getattr(payload, "email", None)
-        if email is not None:
-            init_kwargs.update(email=email)
-        return cls(**init_kwargs)
+        organization_dict = values.pop("organization", None)
+        if organization_dict is None:
+            return values
+
+        if not isinstance(organization_dict, dict):
+            raise ValueError(f"Invalid organization payload: {organization_dict}")
+        elif len(organization_dict) != 1:
+            raise ValueError(f"Organization payload did not include exactly one value: {organization_dict}")
+        return {**values, "organization_id": next(iter(organization_dict))}
+
+
+def lockdown_with_identity(*scopes: str, permission_mode: PermissionMode = PermissionMode.ALL):
+    """
+    Provide a wrapper to be used with dependency injection to extract identity on a secured route.
+    """
+
+    def dependency(
+        token_payload: TokenPayload = Depends(guard.lockdown(*scopes, permission_mode=permission_mode))
+    ) -> IdentityPayload:
+        """
+        Provide an injectable function to lockdown a route and extract the identity payload.
+        """
+        return IdentityPayload.parse_obj(token_payload)
+
+    return dependency
```

### Comparing `jobbergate_api-3.5.0a7/jobbergate_api/tests/apps/applications/test_application_files.py` & `jobbergate_api-3.6.0/jobbergate_api/tests/apps/applications/test_application_files.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a7/jobbergate_api/tests/apps/applications/test_file_validation.py` & `jobbergate_api-3.6.0/jobbergate_api/tests/apps/applications/test_file_validation.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a7/jobbergate_api/tests/apps/applications/test_routers.py` & `jobbergate_api-3.6.0/jobbergate_api/tests/apps/applications/test_routers.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,266 +7,249 @@
 from fastapi import status
 
 from jobbergate_api.apps.applications.application_files import ApplicationFiles
 from jobbergate_api.apps.applications.models import applications_table
 from jobbergate_api.apps.applications.schemas import ApplicationPartialResponse
 from jobbergate_api.apps.job_scripts.models import job_scripts_table
 from jobbergate_api.apps.permissions import Permissions
-from jobbergate_api.storage import database, fetch_instance
-
-# Force the async event loop at the app to begin.
-# Since this is a time consuming fixture, it is just used where strict necessary.
-pytestmark = pytest.mark.usefixtures("startup_event_force")
+from jobbergate_api.storage import fetch_all, fetch_count, fetch_instance, insert_data
 
 
 @pytest.mark.asyncio
 async def test_create_application(
+    synth_session,
     fill_application_data,
     client,
     inject_security_header,
     time_frame,
 ):
     """
     Test POST /applications/ correctly creates an application.
 
     This test proves that an application is successfully created via a POST request to the /applications/
     endpoint. We show this by asserting that the application is created in the database after the post
     request is made and the correct status code (201) is returned.
     """
-    id_rows = await database.fetch_all("SELECT id FROM applications")
-    assert len(id_rows) == 0
+    rows = await fetch_all(synth_session, applications_table, ApplicationPartialResponse)
+    assert len(rows) == 0
 
     inject_security_header("owner1@org.com", Permissions.APPLICATIONS_EDIT)
     with time_frame() as window:
         response = await client.post(
             "/jobbergate/applications/",
             json=fill_application_data(
                 application_name="test-name",
                 application_identifier="test-identifier",
             ),
         )
 
     assert response.status_code == status.HTTP_201_CREATED
-
-    id_rows = await database.fetch_all("SELECT id FROM applications")
-    assert len(id_rows) == 1
-
     application = ApplicationPartialResponse(**response.json())
 
-    assert application.id == id_rows[0][0]
+    rows = await fetch_all(synth_session, applications_table, ApplicationPartialResponse)
+    assert len(rows) == 1
+    assert application.id == rows[0].id
     assert application.application_name == "test-name"
     assert application.application_identifier == "test-identifier"
     assert application.application_owner_email == "owner1@org.com"
-    assert application.application_description is None
+    assert application.application_description == ""
     assert application.created_at in window
     assert application.updated_at in window
 
 
 @pytest.mark.asyncio
 async def test_create_application_bad_permission(
+    synth_session,
     application_data,
     client,
     inject_security_header,
 ):
     """
     Test that it is not possible to create application without proper permission.
 
     This test proves that is not possible to create an application without the proper permission.
     We show this by trying to create an application without an permission that allow "create" then assert
     that the application still does not exists in the database and that the correct status code (403) is
     returned.
     """
-    count = await database.fetch_all("SELECT COUNT(*) FROM applications")
-    assert count[0][0] == 0
-
+    assert await fetch_count(synth_session, applications_table) == 0
     inject_security_header("owner1@org.com", "INVALID_PERMISSION")
     response = await client.post("/jobbergate/applications/", json=application_data)
     assert response.status_code == status.HTTP_403_FORBIDDEN
-
-    count = await database.fetch_all("SELECT COUNT(*) FROM applications")
-    assert count[0][0] == 0
+    assert await fetch_count(synth_session, applications_table) == 0
 
 
 @pytest.mark.asyncio
 async def test_create_without_application_name(
+    synth_session,
     application_data,
     client,
     inject_security_header,
 ):
     """
     Test that is not possible to create an application without the required body fields.
 
     This test proves that is not possible to create an application without the name. We show this by
     trying to create an application without the application_name in the request then assert that the
     application still does not exists in the database and the correct status code (422) is returned.
     """
+    assert await fetch_count(synth_session, applications_table) == 0
     inject_security_header("owner1@org.com", Permissions.APPLICATIONS_EDIT)
     response = await client.post(
         "/jobbergate/applications/",
         json={k: v for (k, v) in application_data.items() if k != "application_name"},
     )
     assert response.status_code == status.HTTP_422_UNPROCESSABLE_ENTITY
-
-    count = await database.fetch_all("SELECT COUNT(*) FROM applications")
-    assert count[0][0] == 0
+    assert await fetch_count(synth_session, applications_table) == 0
 
 
 @pytest.mark.asyncio
 @mock.patch("jobbergate_api.apps.applications.routers.ApplicationFiles.delete_from_s3")
 async def test_delete_application_no_file_uploaded(
-    mocked_application_deleter, client, fill_application_data, inject_security_header
+    mocked_application_deleter, synth_session, client, fill_application_data, inject_security_header
 ):
     """
     Test DELETE /applications/<id> correctly deletes an application.
 
     This test proves that an application is successfully deleted via a DELETE request to the
     /applications/<id> endpoint. We show this by asserting that the application no longer exists in the
     database after the delete request is made and the correct status code is returned.
     """
-    inserted_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(
-            application_owner_email="owner1@org.com",
-        ),
+    inserted_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(application_owner_email="owner1@org.com"),
     )
-    count = await database.fetch_all("SELECT COUNT(*) FROM applications")
-    assert count[0][0] == 1
+    assert await fetch_count(synth_session, applications_table) == 1
 
     inject_security_header("owner1@org.com", Permissions.APPLICATIONS_EDIT)
     response = await client.delete(f"/jobbergate/applications/{inserted_id}")
 
     assert response.status_code == status.HTTP_204_NO_CONTENT
-    count = await database.fetch_all("SELECT COUNT(*) FROM applications")
-    assert count[0][0] == 0
+    assert await fetch_count(synth_session, applications_table) == 0
 
-    mocked_application_deleter.assert_called_once_with(inserted_id)
+    mocked_application_deleter.assert_called_once_with(inserted_id, override_bucket_name=None)
 
 
 @pytest.mark.asyncio
 @mock.patch("jobbergate_api.apps.applications.routers.ApplicationFiles.delete_from_s3")
 async def test_delete_application_with_uploaded_file(
-    mocked_application_deleter, client, fill_application_data, inject_security_header
+    mocked_application_deleter, synth_session, client, fill_application_data, inject_security_header
 ):
     """
     Test DELETE /applications/<id> correctly deletes an application and it's file.
 
     This test proves that an application is successfully deleted via a DELETE request to the
     /applications/<id> endpoint. We show this by asserting that the application no longer exists in the
     database after the delete request is made, the correct status code is returned and the correct boto3
     method was called.
     """
-    inserted_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(
-            application_owner_email="owner1@org.com",
-        ),
+    inserted_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(application_owner_email="owner1@org.com"),
     )
-    count = await database.fetch_all("SELECT COUNT(*) FROM applications")
-    assert count[0][0] == 1
+    assert await fetch_count(synth_session, applications_table) == 1
 
     inject_security_header("owner1@org.com", Permissions.APPLICATIONS_EDIT)
     response = await client.delete(f"/jobbergate/applications/{inserted_id}")
 
     assert response.status_code == status.HTTP_204_NO_CONTENT
-    count = await database.fetch_all("SELECT COUNT(*) FROM applications")
-    assert count[0][0] == 0
+    assert await fetch_count(synth_session, applications_table) == 0
 
-    mocked_application_deleter.assert_called_once_with(inserted_id)
+    mocked_application_deleter.assert_called_once_with(inserted_id, override_bucket_name=None)
 
 
 @pytest.mark.asyncio
 @mock.patch("jobbergate_api.apps.applications.routers.ApplicationFiles.delete_from_s3")
 async def test_delete_application_by_identifier(
-    mocked_application_deleter, client, fill_application_data, inject_security_header
+    mocked_application_deleter, synth_session, client, fill_application_data, inject_security_header
 ):
     """
     Test DELETE /applications?identifier=<identifier> correctly deletes an application and it's file.
 
     This test proves that an application is successfully deleted via a DELETE request to the
     /applications?identifier=<identifier> endpoint. We show this by asserting that the application no longer
     exists in the database after the delete request is made, the correct status code is returned and the
     correct boto3 method was called.
     """
-    inserted_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(
+    inserted_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(
             application_owner_email="owner1@org.com",
             application_identifier="test-identifier",
         ),
     )
-    count = await database.fetch_all("SELECT COUNT(*) FROM applications")
-    assert count[0][0] == 1
+    assert await fetch_count(synth_session, applications_table) == 1
 
     inject_security_header("owner1@org.com", Permissions.APPLICATIONS_EDIT)
     response = await client.delete("/jobbergate/applications?identifier=test-identifier")
 
     assert response.status_code == status.HTTP_204_NO_CONTENT
-    count = await database.fetch_all("SELECT COUNT(*) FROM applications")
-    assert count[0][0] == 0
+    assert await fetch_count(synth_session, applications_table) == 0
 
-    mocked_application_deleter.assert_called_once_with(inserted_id)
+    mocked_application_deleter.assert_called_once_with(inserted_id, override_bucket_name=None)
 
 
 @pytest.mark.asyncio
 async def test_delete_application_bad_permission(
+    synth_session,
     client,
     fill_application_data,
     inject_security_header,
 ):
     """
     Test that it is not possible to delete application without proper permission.
 
     This test proves that an application is not deleted via a DELETE request to the /applications/<id>
     endpoint. We show this by asserting that the application still exists in the database after the delete
     request is made and the correct status code is returned.
     """
-    inserted_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(
-            application_owner_email="owner1@org.com",
-        ),
+    inserted_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(application_owner_email="owner1@org.com"),
     )
-    count = await database.fetch_all("SELECT COUNT(*) FROM applications")
-    assert count[0][0] == 1
+    assert await fetch_count(synth_session, applications_table) == 1
 
     inject_security_header("owner1@org.com", "INVALID_PERMISSION")
     response = await client.delete(f"/jobbergate/applications/{inserted_id}")
     assert response.status_code == status.HTTP_403_FORBIDDEN
-    count = await database.fetch_all("SELECT COUNT(*) FROM applications")
-    assert count[0][0] == 1
+
+    assert await fetch_count(synth_session, applications_table) == 1
 
 
 @pytest.mark.asyncio
 async def test_delete_application_non_owner(
+    synth_session,
     client,
     fill_application_data,
     inject_security_header,
 ):
     """
     Test that it is not possible to delete application if you are not the owner.
 
     This test proves that an application is not deleted via a DELETE request to the /applications/<id>
     endpoint. We show this by asserting that the application still exists in the database after the delete
     request is made and the correct status code is returned.
     """
-    inserted_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(
-            application_owner_email="owner1@org.com",
-        ),
+    inserted_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(application_owner_email="owner1@org.com"),
     )
-    count = await database.fetch_all("SELECT COUNT(*) FROM applications")
-    assert count[0][0] == 1
+    assert await fetch_count(synth_session, applications_table) == 1
 
     inject_security_header("other-owner@other.com", Permissions.APPLICATIONS_EDIT)
     response = await client.delete(f"/jobbergate/applications/{inserted_id}")
     assert response.status_code == status.HTTP_403_FORBIDDEN
     assert "does not own" in response.text
-    count = await database.fetch_all("SELECT COUNT(*) FROM applications")
-    assert count[0][0] == 1
+
+    assert await fetch_count(synth_session, applications_table) == 1
 
 
 @pytest.mark.asyncio
 async def test_delete_application_not_found(client, inject_security_header):
     """
     Test DELETE /applications/<id> the correct response code when the application doesn't exist.
 
@@ -278,86 +261,88 @@
     response = await client.delete("/jobbergate/applications/999")
     assert response.status_code == status.HTTP_404_NOT_FOUND
 
 
 @pytest.mark.asyncio
 @mock.patch("jobbergate_api.apps.applications.routers.ApplicationFiles.delete_from_s3")
 async def test_delete_application__unlinks_job_scripts(
-    mocked_application_deleter,
+    _,
+    synth_session,
     client,
     fill_application_data,
     job_script_data,
     inject_security_header,
 ):
     """
     Test DELETE /applications/<id> correctly deletes an application linked to a job_script.
 
     Test that a the application_id field for connected job_scripts is set to null.
     """
-    inserted_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(
-            application_owner_email="owner1@org.com",
-        ),
-    )
-    count = await database.fetch_all("SELECT COUNT(*) FROM applications")
-    assert count[0][0] == 1
-
-    await database.execute(
-        query=job_scripts_table.insert(),
-        values=dict(
+    inserted_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(application_owner_email="owner1@org.com"),
+    )
+    assert await fetch_count(synth_session, applications_table) == 1
+
+    await insert_data(
+        synth_session,
+        job_scripts_table,
+        dict(
             **job_script_data,
             application_id=inserted_id,
         ),
     )
-    count = await database.fetch_all("SELECT COUNT(*) FROM job_scripts")
-    assert count[0][0] == 1
-    count = await database.fetch_all(
-        "SELECT COUNT(*) FROM job_scripts where application_id=:inserted_id",
-        values=dict(inserted_id=inserted_id),
+    assert await fetch_count(synth_session, job_scripts_table) == 1
+    assert (
+        await fetch_count(synth_session, job_scripts_table, job_scripts_table.c.application_id == inserted_id)
+        == 1
     )
-    assert count[0][0] == 1
 
     inject_security_header("owner1@org.com", Permissions.APPLICATIONS_EDIT)
     response = await client.delete(f"/jobbergate/applications/{inserted_id}")
     assert response.status_code == status.HTTP_204_NO_CONTENT
-    count = await database.fetch_all("SELECT COUNT(*) FROM applications")
-    assert count[0][0] == 0
 
-    count = await database.fetch_all(
-        "SELECT COUNT(*) FROM job_scripts where application_id=:inserted_id",
-        values=dict(inserted_id=inserted_id),
+    assert await fetch_count(synth_session, applications_table) == 0
+    assert (
+        await fetch_count(
+            synth_session,
+            job_scripts_table,
+            job_scripts_table.c.application_id == inserted_id,
+        )
+        == 0
     )
-    assert count[0][0] == 0
 
 
 @pytest.mark.asyncio
 async def test_get_application_by_id__files_not_uploaded(
+    synth_session,
     client,
     fill_application_data,
     inject_security_header,
 ):
     """
     Test GET /applications/<id> when the application files were not uploaded.
 
     This test proves that GET /applications/<id> returns the correct application, owned by
     the user making the request. We show this by asserting that the application data
     returned in the response is equal to the application data that exists in the database
     for the given application id.
     """
-    inserted_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(application_identifier="app1"),
-    )
-    await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(application_identifier="app2"),
+    inserted_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(application_identifier="app1"),
+    )
+    await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(application_identifier="app2"),
     )
-    count = await database.fetch_all("SELECT COUNT(*) FROM applications")
-    assert count[0][0] == 2
+    assert await fetch_count(synth_session, applications_table) == 2
 
     inject_security_header("owner1@org.com", Permissions.APPLICATIONS_VIEW)
     response = await client.get(f"/jobbergate/applications/{inserted_id}")
     assert response.status_code == status.HTTP_200_OK
 
     data = response.json()
     assert data["id"] == inserted_id
@@ -367,14 +352,15 @@
     assert data["application_templates"] is None
 
 
 @pytest.mark.asyncio
 @mock.patch("jobbergate_api.apps.applications.routers.ApplicationFiles.get_from_s3")
 async def test_get_application_by_id__files_uploaded(
     mocked_get_application_files_from_s3,
+    synth_session,
     client,
     fill_application_data,
     inject_security_header,
     dummy_application_config,
     dummy_application_source_file,
     dummy_template,
 ):
@@ -382,35 +368,35 @@
     Test GET /applications/<id> when the application files were uploaded.
 
     This test proves that GET /applications/<id> returns the correct application, owned by
     the user making the request. We show this by asserting that the application data
     returned in the response is equal to the application data that exists in the database
     for the given application id, and the application files are recovered from S3.
     """
-    inserted_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(
+    inserted_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(
             application_identifier="app1",
             application_uploaded=True,
         ),
     )
-    await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(application_identifier="app2"),
+    await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(application_identifier="app2"),
     )
+    assert await fetch_count(synth_session, applications_table) == 2
 
     mocked_get_application_files_from_s3.return_value = ApplicationFiles(
         templates={"test_job_script.sh": dummy_template},
         source_file=dummy_application_source_file,
         config_file=dummy_application_config,
     )
 
-    count = await database.fetch_all("SELECT COUNT(*) FROM applications")
-    assert count[0][0] == 2
-
     inject_security_header("owner1@org.com", Permissions.APPLICATIONS_VIEW)
     response = await client.get(f"/jobbergate/applications/{inserted_id}")
     assert response.status_code == status.HTTP_200_OK
 
     data = response.json()
     assert data["id"] == inserted_id
     assert data["application_identifier"] == "app1"
@@ -432,60 +418,62 @@
     inject_security_header("owner1@org.com", Permissions.APPLICATIONS_VIEW)
     response = await client.get("/jobbergate/applications/10")
     assert response.status_code == status.HTTP_404_NOT_FOUND
 
 
 @pytest.mark.asyncio
 async def test_get_application_by_id_bad_permission(
+    synth_session,
     client,
     application_data,
     inject_security_header,
 ):
     """
     Test that it is not possible to get application without proper permission.
 
     This test proves that GET /application/<id> returns the correct response code when the
     user don't have the proper permission. We show this by asserting that the status code
     returned is what we would expect (403).
     """
-    inserted_id = await database.execute(
-        query=applications_table.insert(),
-        values=application_data,
+    inserted_id = await insert_data(
+        synth_session,
+        applications_table,
+        application_data,
     )
 
     inject_security_header("owner1@org.com", "INVALID_PERMISSION")
     response = await client.get(f"/jobbergate/applications/{inserted_id}")
     assert response.status_code == status.HTTP_403_FORBIDDEN
 
 
 @pytest.mark.asyncio
 async def test_get_applications__no_params(
+    synth_session,
     client,
     fill_all_application_data,
     inject_security_header,
 ):
     """
     Test GET /applications returns only applications owned by the user making the request.
 
     This test proves that GET /applications returns the correct applications for the user making
     the request. We show this by asserting that the applications returned in the response are
     only applications owned by the user making the request. This test also ensures that archived
     applications are not included by default.
     """
-    await database.execute_many(
-        applications_table.insert(),
-        values=fill_all_application_data(
+    query = applications_table.insert().values(
+        fill_all_application_data(
             dict(application_identifier="app1"),
             dict(application_identifier="app2"),
             dict(application_identifier="app3"),
             dict(application_identifier="app4", is_archived=True),
         ),
     )
-    count = await database.fetch_all("SELECT COUNT(*) FROM applications")
-    assert count[0][0] == 4
+    await synth_session.execute(query)
+    assert await fetch_count(synth_session, applications_table) == 4
 
     inject_security_header("owner1@org.com", Permissions.APPLICATIONS_VIEW)
     response = await client.get("/jobbergate/applications/")
     assert response.status_code == status.HTTP_200_OK
 
     data = response.json()
     results = data.get("results")
@@ -502,74 +490,74 @@
         start=None,
         limit=None,
     )
 
 
 @pytest.mark.asyncio
 async def test_get_application___bad_permission(
+    synth_session,
     client,
     fill_all_application_data,
     inject_security_header,
 ):
     """
     Test that it is not possible to list applications without proper permission.
 
     This test proves that the GET /applications returns 403 as status code in the response.
     We show this by making a request with an user without creating the permission, and then asserting the
     status code in the response.
     """
-    await database.execute_many(
-        query=applications_table.insert(),
-        values=fill_all_application_data(
+    query = applications_table.insert().values(
+        fill_all_application_data(
             dict(application_identifier="app1"),
             dict(application_identifier="app2"),
             dict(application_identifier="app3"),
         ),
     )
-    count = await database.fetch_all("SELECT COUNT(*) FROM applications")
-    assert count[0][0] == 3
+    await synth_session.execute(query)
+    assert await fetch_count(synth_session, applications_table) == 3
 
     inject_security_header("owner1@org.com", "INVALID_PERMISSION")
     response = await client.get("/jobbergate/applications/")
     assert response.status_code == status.HTTP_403_FORBIDDEN
 
 
 @pytest.mark.asyncio
 async def test_get_applications__with_user_param(
+    synth_session,
     client,
     fill_all_application_data,
     inject_security_header,
 ):
     """
     Test applications list doesn't include applications owned by other users with `user` param.
 
     This test proves that the user making the request cannot see applications owned by other users.
     We show this by creating applications that are owned by another user id and assert that
     the user making the request to list applications doesn't see any of the other user's
     applications in the response.
     """
-    await database.execute_many(
-        query=applications_table.insert(),
-        values=fill_all_application_data(
+    query = applications_table.insert().values(
+        fill_all_application_data(
             dict(
                 application_identifier="app1",
                 application_owner_email="owner1@org.com",
             ),
             dict(
                 application_identifier="app2",
                 application_owner_email="owner1@org.com",
             ),
             dict(
                 application_identifier="app3",
                 application_owner_email="owner999@org.com",
             ),
         ),
     )
-    count = await database.fetch_all("SELECT COUNT(*) FROM applications")
-    assert count[0][0] == 3
+    await synth_session.execute(query)
+    assert await fetch_count(synth_session, applications_table) == 3
 
     inject_security_header("owner1@org.com", Permissions.APPLICATIONS_VIEW)
     response = await client.get("/jobbergate/applications")
     assert response.status_code == status.HTTP_200_OK
 
     data = response.json()
     results = data.get("results")
@@ -595,36 +583,36 @@
         start=None,
         limit=None,
     )
 
 
 @pytest.mark.asyncio
 async def test_get_applications__with_all_param(
+    synth_session,
     client,
     fill_all_application_data,
     inject_security_header,
 ):
     """
     Test that listing applications, when all=True, contains applications without identifiers.
 
     This test proves that the user making the request can see applications owned by other users.
     We show this by creating three applications, two that are owned by the user making the request, and one
     owned by another user. Assert that the response to GET /applications/?all=True includes all three
     applications.
     """
-    await database.execute_many(
-        query=applications_table.insert(),
-        values=fill_all_application_data(
+    query = applications_table.insert().values(
+        fill_all_application_data(
             dict(application_identifier="app1", application_owner_email="owner1@org.com"),
-            dict(application_owner_email="owner1@org.com"),
+            dict(application_identifier=None, application_owner_email="owner1@org.com"),
             dict(application_identifier="app3", application_owner_email="owner999@org.com"),
         ),
     )
-    count = await database.fetch_all("SELECT COUNT(*) FROM applications")
-    assert count[0][0] == 3
+    await synth_session.execute(query)
+    assert await fetch_count(synth_session, applications_table) == 3
 
     inject_security_header("owner1@org.com", Permissions.APPLICATIONS_VIEW)
 
     response = await client.get("/jobbergate/applications")
     assert response.status_code == status.HTTP_200_OK
 
     data = response.json()
@@ -649,35 +637,35 @@
         start=None,
         limit=None,
     )
 
 
 @pytest.mark.asyncio
 async def test_get_applications__with_include_archived_param(
+    synth_session,
     client,
     fill_all_application_data,
     inject_security_header,
 ):
     """
     Test that listing applications, when include_archived=True, contains archived applications.
 
     This test proves that the user making the request can see archived applications.
     We show this by creating three applications, two that are normal, and one that is archived.
     Assert that the response to GET /applications/?include_archived=True includes all three applications.
     """
-    await database.execute_many(
-        query=applications_table.insert(),
-        values=fill_all_application_data(
-            dict(application_identifier="app1"),
+    query = applications_table.insert().values(
+        fill_all_application_data(
+            dict(application_identifier="app1", is_archived=False),
             dict(application_identifier="app2", is_archived=True),
-            dict(application_identifier="app3"),
+            dict(application_identifier="app3", is_archived=False),
         ),
     )
-    count = await database.fetch_all("SELECT COUNT(*) FROM applications")
-    assert count[0][0] == 3
+    await synth_session.execute(query)
+    assert await fetch_count(synth_session, applications_table) == 3
 
     inject_security_header("owner1@org.com", Permissions.APPLICATIONS_VIEW)
 
     response = await client.get("/jobbergate/applications")
     assert response.status_code == status.HTTP_200_OK
 
     data = response.json()
@@ -702,49 +690,51 @@
         start=None,
         limit=None,
     )
 
 
 @pytest.mark.asyncio
 async def test_get_applications__with_search_param(
+    synth_session,
     client,
     fill_all_application_data,
     inject_security_header,
 ):
     """
     Test that listing applications, when search=<search terms>, returns matches.
 
     This test proves that the user making the request will be shown applications that match the search string.
     We show this by creating applications and using various search queries to match against them.
 
     Assert that the response to GET /applications?search=<search terms> includes correct matches.
     """
-    await database.execute_many(
-        query=applications_table.insert(),
-        values=fill_all_application_data(
+    query = applications_table.insert().values(
+        fill_all_application_data(
             dict(
                 application_name="test name one",
                 application_identifier="app1",
                 application_owner_email="one@org.com",
+                application_description=None,
             ),
             dict(
                 application_name="test name two",
                 application_identifier="app2",
                 application_owner_email="two@org.com",
+                application_description=None,
             ),
             dict(
                 application_name="test name twenty-two",
                 application_identifier="app22",
                 application_owner_email="twenty-two@org.com",
                 application_description="a long description of this application",
             ),
         ),
     )
-    count = await database.fetch_all("SELECT COUNT(*) FROM applications")
-    assert count[0][0] == 3
+    await synth_session.execute(query)
+    assert await fetch_count(synth_session, applications_table) == 3
 
     inject_security_header("admin@org.com", Permissions.APPLICATIONS_VIEW)
 
     response = await client.get("/jobbergate/applications?all=true&search=one")
     assert response.status_code == status.HTTP_200_OK
     data = response.json()
     results = data.get("results")
@@ -767,38 +757,38 @@
     data = response.json()
     results = data.get("results")
     assert sorted([d["application_identifier"] for d in results]) == ["app1", "app2", "app22"]
 
 
 @pytest.mark.asyncio
 async def test_get_applications__with_sort_params(
+    synth_session,
     client,
     fill_all_application_data,
     inject_security_header,
 ):
     """
     Test that listing applications with sort params returns correctly ordered matches.
 
     This test proves that the user making the request will be shown applications sorted in the correct order
     according to the ``sort_field`` and ``sort_ascending`` parameters.
     We show this by creating applications and using various sort parameters to order them.
 
     Assert that the response to GET /applications?sort_field=<field>&sort_ascending=<bool> includes correctly
     sorted applications.
     """
-    await database.execute_many(
-        query=applications_table.insert(),
-        values=fill_all_application_data(
+    query = applications_table.insert().values(
+        fill_all_application_data(
             dict(application_name="A", application_identifier="Z"),
             dict(application_name="B", application_identifier="Y"),
             dict(application_name="C", application_identifier="X"),
         ),
     )
-    count = await database.fetch_all("SELECT COUNT(*) FROM applications")
-    assert count[0][0] == 3
+    await synth_session.execute(query)
+    assert await fetch_count(synth_session, applications_table) == 3
 
     inject_security_header("admin@org.com", Permissions.APPLICATIONS_VIEW)
 
     response = await client.get("/jobbergate/applications?all=true&sort_field=application_name")
     assert response.status_code == status.HTTP_200_OK
     data = response.json()
     results = data.get("results")
@@ -821,36 +811,36 @@
     response = await client.get("/jobbergate/applications?all=true&sort_field=application_config")
     assert response.status_code == status.HTTP_400_BAD_REQUEST
     assert "Invalid sorting column requested" in response.text
 
 
 @pytest.mark.asyncio
 async def test_get_applications__with_pagination(
+    synth_session,
     client,
     fill_all_application_data,
     inject_security_header,
 ):
     """
     Test that listing applications works with pagination.
 
     This test proves that the user making the request can see applications paginated.
     We show this by creating three applications and assert that the response is correctly paginated.
     """
-    await database.execute_many(
-        query=applications_table.insert(),
-        values=fill_all_application_data(
+    query = applications_table.insert().values(
+        fill_all_application_data(
             dict(application_identifier="app1", application_owner_email="owner1@org.com"),
             dict(application_identifier="app2", application_owner_email="owner1@org.com"),
             dict(application_identifier="app3", application_owner_email="owner1@org.com"),
             dict(application_identifier="app4", application_owner_email="owner1@org.com"),
             dict(application_identifier="app5", application_owner_email="owner1@org.com"),
         ),
     )
-    count = await database.fetch_all("SELECT COUNT(*) FROM applications")
-    assert count[0][0] == 5
+    await synth_session.execute(query)
+    assert await fetch_count(synth_session, applications_table) == 5
 
     inject_security_header("owner1@org.com", Permissions.APPLICATIONS_VIEW)
     response = await client.get(
         "/jobbergate/applications/?start=0&limit=1&all=true&sort_field=application_identifier"
     )
     assert response.status_code == status.HTTP_200_OK
 
@@ -895,42 +885,42 @@
         start=2,
         limit=2,
     )
 
 
 @pytest.mark.asyncio
 async def test_update_application(
+    synth_session,
     client,
     fill_application_data,
     inject_security_header,
     time_frame,
 ):
     """
     Test that an application is updated via PUT.
 
     This test proves that an application's values are correctly updated following a PUT request to the
     /application/<id> endpoint. We show this by asserting that the values provided to update the
     application are returned in the response made to the PUT /application/<id> endpoint.
     """
-    await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(
+    inserted_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(
             application_identifier="old_identifier",
             application_owner_email="owner1@org.com",
             application_description="old description",
         ),
     )
-    rows = await database.fetch_all("select id from applications")
-    assert len(rows) == 1
-    id = rows[0][0]
+    assert await fetch_count(synth_session, applications_table) == 1
 
     inject_security_header("owner1@org.com", Permissions.APPLICATIONS_EDIT)
     with time_frame() as window:
         response = await client.put(
-            f"/jobbergate/applications/{id}",
+            f"/jobbergate/applications/{inserted_id}",
             json=dict(
                 application_name="new_name",
                 application_identifier="new_identifier",
                 application_description="new_description",
                 is_archived=True,
             ),
         )
@@ -938,126 +928,132 @@
 
     data = response.json()
     assert data["application_name"] == "new_name"
     assert data["application_identifier"] == "new_identifier"
     assert data["application_description"] == "new_description"
     assert data["is_archived"] is True
 
-    query = applications_table.select(applications_table.c.id == id)
-    result = await database.fetch_one(query)
+    updated_application = await fetch_instance(
+        synth_session, inserted_id, applications_table, ApplicationPartialResponse
+    )
 
-    assert result is not None
-    assert result["application_name"] == "new_name"
-    assert result["application_identifier"] == "new_identifier"
-    assert result["application_owner_email"] == "owner1@org.com"
-    assert result["application_description"] == "new_description"
-    assert result["is_archived"] is True
-    assert result["updated_at"] in window
+    assert updated_application is not None
+    assert updated_application.application_name == "new_name"
+    assert updated_application.application_identifier == "new_identifier"
+    assert updated_application.application_owner_email == "owner1@org.com"
+    assert updated_application.application_description == "new_description"
+    assert updated_application.is_archived is True
+    assert updated_application.updated_at in window
 
 
 @pytest.mark.asyncio
 async def test_update_application_bad_permission(
+    synth_session,
     client,
     fill_application_data,
     inject_security_header,
 ):
     """
     Test that it is not possible to update applications without proper permission.
 
     This test proves that an application's values are not updated following a PUT request to the
     /application/<id> endpoint by a user without permission. We show this by asserting that the status code
     403 is returned and that the application_data is still the same as before.
     """
-    inserted_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(
+    inserted_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(
             application_name="old-name",
             application_identifier="old_identifier",
             application_owner_email="owner1@org.com",
             application_description="old description",
         ),
     )
-    count = await database.fetch_all("SELECT COUNT(*) FROM applications")
-    assert count[0][0] == 1
+    assert await fetch_count(synth_session, applications_table) == 1
 
     inject_security_header("owner1@org.com", "INVALID_PERMISSION")
     response = await client.put(
         f"/jobbergate/applications/{inserted_id}",
         json=dict(
             application_name="new_name",
             application_identifier="new_identifier",
             application_description="new_description",
         ),
     )
     assert response.status_code == status.HTTP_403_FORBIDDEN
 
-    query = applications_table.select(applications_table.c.id == inserted_id)
-    result = await database.fetch_one(query)
+    unaltered_application = await fetch_instance(
+        synth_session, inserted_id, applications_table, ApplicationPartialResponse
+    )
 
-    assert result is not None
-    assert result["application_name"] == "old-name"
-    assert result["application_identifier"] == "old_identifier"
-    assert result["application_description"] == "old description"
+    assert unaltered_application is not None
+    assert unaltered_application.application_name == "old-name"
+    assert unaltered_application.application_identifier == "old_identifier"
+    assert unaltered_application.application_description == "old description"
 
 
 @pytest.mark.asyncio
 async def test_update_application_non_owner(
+    synth_session,
     client,
     fill_application_data,
     inject_security_header,
 ):
     """
     Test that it is not possible to update applications if you are not the owner.
 
     This test proves that an application's values are not updated following a PUT request to the
     /application/<id> endpoint by a user without permission. We show this by asserting that the status code
     403 is returned and that the application_data is still the same as before.
     """
-    inserted_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(
+    inserted_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(
             application_name="old-name",
             application_identifier="old_identifier",
             application_owner_email="owner1@org.com",
             application_description="old description",
         ),
     )
-    count = await database.fetch_all("SELECT COUNT(*) FROM applications")
-    assert count[0][0] == 1
+    assert await fetch_count(synth_session, applications_table) == 1
 
     inject_security_header("other-owner@org.com", Permissions.APPLICATIONS_EDIT)
     response = await client.put(
         f"/jobbergate/applications/{inserted_id}",
         json=dict(
             application_name="new_name",
             application_identifier="new_identifier",
             application_description="new_description",
         ),
     )
     assert response.status_code == status.HTTP_403_FORBIDDEN
     assert "does not own" in response.text
 
-    query = applications_table.select(applications_table.c.id == inserted_id)
-    result = await database.fetch_one(query)
+    unaltered_application = await fetch_instance(
+        synth_session, inserted_id, applications_table, ApplicationPartialResponse
+    )
 
-    assert result is not None
-    assert result["application_name"] == "old-name"
-    assert result["application_identifier"] == "old_identifier"
-    assert result["application_description"] == "old description"
+    assert unaltered_application is not None
+    assert unaltered_application.application_name == "old-name"
+    assert unaltered_application.application_identifier == "old_identifier"
+    assert unaltered_application.application_description == "old description"
 
 
 @pytest.mark.asyncio
 @mock.patch("jobbergate_api.apps.applications.routers.ApplicationFiles.write_to_s3")
 @mock.patch(
     "jobbergate_api.apps.applications.routers.ApplicationFiles.get_from_upload_files",
     return_value=ApplicationFiles(),
 )
 async def test_upload_file__works_with_small_file(
     mocked_application_writer,
     mocked_application_get_upload,
+    synth_session,
     client,
     inject_security_header,
     fill_application_data,
     tweak_settings,
     make_dummy_file,
     dummy_application_config,
     make_files_param,
@@ -1066,19 +1062,24 @@
     Test that a file is uploaded.
 
     This test proves that an application's file is uploaded by making sure that the
     boto3 put_object method is called once and a 201 status code is returned. It also
     checks to make sure that the application row in the database has
     `application_uploaded` set.
     """
-    inserted_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(application_owner_email="owner1@org.com"),
+    inserted_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(application_owner_email="owner1@org.com"),
+    )
+    assert await fetch_count(synth_session, applications_table) == 1
+
+    application = await fetch_instance(
+        synth_session, inserted_id, applications_table, ApplicationPartialResponse
     )
-    application = await fetch_instance(inserted_id, applications_table, ApplicationPartialResponse)
     assert not application.application_uploaded
 
     dummy_file = make_dummy_file("jobbergate.yaml", content=dummy_application_config)
     inject_security_header("owner1@org.com", Permissions.APPLICATIONS_EDIT)
     with tweak_settings(MAX_UPLOAD_FILE_SIZE=600):
         with make_files_param(dummy_file) as files_param:
             response = await client.post(
@@ -1086,35 +1087,44 @@
                 files=files_param,
             )
 
     assert response.status_code == status.HTTP_201_CREATED
     mocked_application_writer.assert_called_once()
     mocked_application_get_upload.assert_called_once()
 
-    application = await fetch_instance(inserted_id, applications_table, ApplicationPartialResponse)
+    application = await fetch_instance(
+        synth_session, inserted_id, applications_table, ApplicationPartialResponse
+    )
+    assert application.application_uploaded
 
 
 @pytest.mark.asyncio
 async def test_upload_file__fails_for_non_owner(
+    synth_session,
     client,
     inject_security_header,
     fill_application_data,
     tweak_settings,
     make_dummy_file,
     dummy_application_config,
     make_files_param,
 ):
     """
     Test that a file cannot be uploaded by a non-owner.
     """
-    inserted_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(application_owner_email="owner1@org.com"),
+    inserted_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(application_owner_email="owner1@org.com"),
+    )
+    assert await fetch_count(synth_session, applications_table) == 1
+
+    application = await fetch_instance(
+        synth_session, inserted_id, applications_table, ApplicationPartialResponse
     )
-    application = await fetch_instance(inserted_id, applications_table, ApplicationPartialResponse)
     assert not application.application_uploaded
 
     dummy_file = make_dummy_file("jobbergate.yaml", content=dummy_application_config)
     inject_security_header("non-owner@org.com", Permissions.APPLICATIONS_EDIT)
     with tweak_settings(MAX_UPLOAD_FILE_SIZE=600):
         with make_files_param(dummy_file) as files_param:
             response = await client.post(
@@ -1127,14 +1137,15 @@
     assert not application.application_uploaded
 
 
 @pytest.mark.asyncio
 @mock.patch("jobbergate_api.apps.applications.routers.ApplicationFiles.write_to_s3")
 async def test_upload_file_individually__success(
     mocked_application_writer,
+    synth_session,
     client,
     inject_security_header,
     fill_application_data,
     tweak_settings,
     make_dummy_file,
     dummy_application_config,
     dummy_template,
@@ -1143,19 +1154,24 @@
 ):
     """
     Test that the application files can be patched individually.
 
     This test proves that any application file, i.e. config, source or template,
     can be patched individually.
     """
-    inserted_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(application_owner_email="owner1@org.com"),
+    inserted_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(application_owner_email="owner1@org.com"),
+    )
+    assert await fetch_count(synth_session, applications_table) == 1
+
+    application = await fetch_instance(
+        synth_session, inserted_id, applications_table, ApplicationPartialResponse
     )
-    application = await fetch_instance(inserted_id, applications_table, ApplicationPartialResponse)
     assert not application.application_uploaded
 
     dummy_config_file = make_dummy_file("jobbergate.yaml", content=dummy_application_config)
     dummy_source_file = make_dummy_file("jobbergate.py", content=dummy_application_source_file)
     dummy_template_file = make_dummy_file("jobbergate.yaml", content=dummy_template)
 
     inject_security_header("owner1@org.com", Permissions.APPLICATIONS_EDIT)
@@ -1223,34 +1239,40 @@
             "config_file": open(dummy_config_file, "rb"),
         },
     )
 
     assert response.status_code == status.HTTP_204_NO_CONTENT
 
     mocked_application_writer.assert_has_calls(
-        [mock.call(inserted_id, remove_previous_files=False) for _ in range(7)]
+        [mock.call(inserted_id, remove_previous_files=False, override_bucket_name=None) for _ in range(7)]
     )
 
 
 @pytest.mark.asyncio
 async def test_upload_file_individually__fails_on_non_owner(
+    synth_session,
     client,
     inject_security_header,
     fill_application_data,
     make_dummy_file,
     dummy_application_source_file,
 ):
     """
     Test that the application files cannot be patched individually by a non-owner.
     """
-    inserted_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(application_owner_email="owner1@org.com"),
+    inserted_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(application_owner_email="owner1@org.com"),
+    )
+    assert await fetch_count(synth_session, applications_table) == 1
+
+    application = await fetch_instance(
+        synth_session, inserted_id, applications_table, ApplicationPartialResponse
     )
-    application = await fetch_instance(inserted_id, applications_table, ApplicationPartialResponse)
     assert not application.application_uploaded
 
     dummy_source_file = make_dummy_file("jobbergate.py", content=dummy_application_source_file)
 
     inject_security_header("non-owner@org.com", Permissions.APPLICATIONS_EDIT)
 
     response = await client.patch(
@@ -1288,55 +1310,63 @@
 
     mocked_application_writer.assert_not_called()
 
 
 @pytest.mark.asyncio
 @mock.patch("jobbergate_api.apps.applications.routers.ApplicationFiles.delete_from_s3")
 async def test_delete_file_success(
-    mocked_application_deleter, client, inject_security_header, fill_application_data
+    mocked_application_deleter, synth_session, client, inject_security_header, fill_application_data
 ):
     """
     Test that a file is deleted.
 
     This test proves that an application's file is deleted by making sure that the boto3 put_object method
     is called once and a 201 status code is returned.
     """
-    inserted_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(application_owner_email="owner1@org.com", application_uploaded=True),
+    inserted_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(application_owner_email="owner1@org.com", application_uploaded=True),
     )
-    application: ApplicationPartialResponse = await fetch_instance(
-        inserted_id, applications_table, ApplicationPartialResponse
+    assert await fetch_count(synth_session, applications_table) == 1
+
+    application = await fetch_instance(
+        synth_session, inserted_id, applications_table, ApplicationPartialResponse
     )
     assert application.application_uploaded
 
     inject_security_header("owner1@org.com", Permissions.APPLICATIONS_EDIT)
     response = await client.delete(f"/jobbergate/applications/{inserted_id}/upload")
 
     assert response.status_code == status.HTTP_204_NO_CONTENT
-    mocked_application_deleter.assert_called_once_with(inserted_id)
+    mocked_application_deleter.assert_called_once_with(inserted_id, override_bucket_name=None)
 
-    application = await fetch_instance(inserted_id, applications_table, ApplicationPartialResponse)
+    application = await fetch_instance(
+        synth_session, inserted_id, applications_table, ApplicationPartialResponse
+    )
     assert not application.application_uploaded
 
 
 @pytest.mark.asyncio
 @mock.patch("jobbergate_api.apps.applications.routers.ApplicationFiles.delete_from_s3")
 async def test_delete_file__fails_with_403_for_non_owner(
-    mocked_application_deleter, client, inject_security_header, fill_application_data
+    mocked_application_deleter, synth_session, client, inject_security_header, fill_application_data
 ):
     """
     Test that a file is not deleted if the requester is not the owner.
     """
-    inserted_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(application_owner_email="owner1@org.com", application_uploaded=True),
+    inserted_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(application_owner_email="owner1@org.com", application_uploaded=True),
     )
-    application: ApplicationPartialResponse = await fetch_instance(
-        inserted_id, applications_table, ApplicationPartialResponse
+    assert await fetch_count(synth_session, applications_table) == 1
+
+    application = await fetch_instance(
+        synth_session, inserted_id, applications_table, ApplicationPartialResponse
     )
     assert application.application_uploaded
 
     inject_security_header("non-owner@org.com", Permissions.APPLICATIONS_EDIT)
     response = await client.delete(f"/jobbergate/applications/{inserted_id}/upload")
 
     assert response.status_code == status.HTTP_403_FORBIDDEN
```

### Comparing `jobbergate_api-3.5.0a7/jobbergate_api/tests/apps/applications/test_schemas.py` & `jobbergate_api-3.6.0/jobbergate_api/tests/apps/applications/test_schemas.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a7/jobbergate_api/tests/apps/conftest.py` & `jobbergate_api-3.6.0/jobbergate_api/tests/apps/conftest.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a7/jobbergate_api/tests/apps/job_scripts/conftest.py` & `jobbergate_api-3.6.0/jobbergate_api/tests/apps/job_scripts/conftest.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a7/jobbergate_api/tests/apps/job_scripts/test_job_script_files.py` & `jobbergate_api-3.6.0/jobbergate_api/tests/apps/job_scripts/test_job_script_files.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a7/jobbergate_api/tests/apps/job_scripts/test_routers.py` & `jobbergate_api-3.6.0/jobbergate_api/tests/apps/job_scripts/test_routers.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,19 +11,15 @@
 from jobbergate_api.apps.applications.application_files import ApplicationFiles
 from jobbergate_api.apps.applications.models import applications_table
 from jobbergate_api.apps.job_scripts.job_script_files import JobScriptFiles
 from jobbergate_api.apps.job_scripts.models import job_scripts_table
 from jobbergate_api.apps.job_scripts.schemas import JobScriptResponse
 from jobbergate_api.apps.job_submissions.models import job_submissions_table
 from jobbergate_api.apps.permissions import Permissions
-from jobbergate_api.storage import database
-
-# Force the async event loop at the app to begin.
-# Since this is a time consuming fixture, it is just used where strict necessary.
-pytestmark = pytest.mark.usefixtures("startup_event_force")
+from jobbergate_api.storage import fetch_all, fetch_count, fetch_instance, insert_data
 
 
 @pytest.fixture
 def job_script_data_as_string():
     """
     Provide a fixture that returns an example of a default application script.
     """
@@ -72,18 +68,18 @@
     """
     Provide a fixture that returns string content of the argument --sbatch-params.
     """
     return ["--comment=some_comment", "--nice=-1", "-N 10"]
 
 
 @pytest.mark.asyncio
-@database.transaction(force_rollback=True)
 @mock.patch("jobbergate_api.apps.job_scripts.job_script_files.JobScriptFiles.write_to_s3")
 async def test_create_job_script__with_application(
     mocked_write_job_script_files_to_s3,
+    synth_session,
     fill_application_data,
     job_script_data,
     fill_job_script_data,
     param_dict,
     client,
     inject_security_header,
     time_frame,
@@ -96,17 +92,18 @@
     """
     Test POST /job_scripts/ correctly creates a job_script with a source application.
 
     This test proves that a job_script is successfully created via a POST request to the /job-scripts/
     endpoint. We show this by asserting that the job_script is created in the database after the post
     request is made, the correct status code (201) is returned.
     """
-    inserted_application_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(
+    inserted_application_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(
             application_owner_email="owner1@org.com",
             application_uploaded=True,
         ),
     )
 
     ApplicationFiles(
         templates={"test_job_script.sh": dummy_template},
@@ -121,36 +118,35 @@
             json=fill_job_script_data(
                 application_id=inserted_application_id,
                 param_dict=param_dict,
             ),
         )
 
     assert response.status_code == status.HTTP_201_CREATED
-
-    id_rows = await database.fetch_all("SELECT id FROM job_scripts")
-    assert len(id_rows) == 1
+    rows = await fetch_all(synth_session, job_scripts_table, JobScriptResponse)
+    assert len(rows) == 1
 
     job_script = JobScriptResponse(**response.json())
 
-    mocked_write_job_script_files_to_s3.assert_called_once_with(job_script.id)
+    mocked_write_job_script_files_to_s3.assert_called_once_with(job_script.id, override_bucket_name=None)
 
-    assert job_script.id == id_rows[0][0]
+    assert job_script.id == rows[0].id
     assert job_script.job_script_name == job_script_data["job_script_name"]
     assert job_script.job_script_owner_email == "owner1@org.com"
-    assert job_script.job_script_description is None
+    assert job_script.job_script_description == ""
     assert job_script.job_script_files.main_file
     assert job_script.application_id == inserted_application_id
     assert job_script.created_at in window
     assert job_script.updated_at in window
     assert job_script.job_script_files.main_file == job_script_data_as_string
 
 
 @pytest.mark.asyncio
-@database.transaction(force_rollback=True)
 async def test_create_job_script__without_application(
+    synth_session,
     job_script_data,
     fill_job_script_data,
     param_dict,
     client,
     inject_security_header,
     time_frame,
 ):
@@ -168,104 +164,105 @@
             json=fill_job_script_data(
                 param_dict=param_dict,
             ),
         )
 
     assert response.status_code == status.HTTP_201_CREATED
 
-    id_rows = await database.fetch_all("SELECT id FROM job_scripts")
-    assert len(id_rows) == 1
+    rows = await fetch_all(synth_session, job_scripts_table, JobScriptResponse)
+    assert len(rows) == 1
 
     job_script = JobScriptResponse(**response.json())
 
-    assert job_script.id == id_rows[0][0]
+    assert job_script.id == rows[0].id
     assert job_script.job_script_name == job_script_data["job_script_name"]
     assert job_script.job_script_owner_email == "owner1@org.com"
-    assert job_script.job_script_description is None
+    assert job_script.job_script_description == ""
     assert job_script.job_script_files is None
     assert job_script.application_id is None
     assert job_script.created_at in window
     assert job_script.updated_at in window
 
 
 @pytest.mark.asyncio
-@database.transaction(force_rollback=True)
 async def test_create_job_script_application_not_uploaded(
+    synth_session,
     fill_application_data,
     fill_job_script_data,
     param_dict,
     client,
     inject_security_header,
 ):
     """
     Test that it is not possible to create job_script when the application is marked as not uploaded.
     """
-    inserted_application_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(
+    inserted_application_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(
             application_owner_email="owner1@org.com",
             application_uploaded=False,
         ),
     )
+    assert await fetch_count(synth_session, applications_table) == 1
 
     inject_security_header("owner1@org.com", Permissions.JOB_SCRIPTS_EDIT)
     response = await client.post(
         "/jobbergate/job-scripts/",
         json=fill_job_script_data(
             application_id=inserted_application_id,
             param_dict=param_dict,
         ),
     )
 
     assert response.status_code == status.HTTP_422_UNPROCESSABLE_ENTITY
-
-    count = await database.fetch_all("SELECT COUNT(*) FROM job_scripts")
-    assert count[0][0] == 0
+    assert await fetch_count(synth_session, job_scripts_table) == 0
 
 
 @pytest.mark.asyncio
-@database.transaction(force_rollback=True)
 async def test_create_job_script_bad_permission(
+    synth_session,
     fill_application_data,
     fill_job_script_data,
     param_dict,
     client,
     inject_security_header,
 ):
     """
     Test that it is not possible to create job_script without proper permission.
 
     This test proves that is not possible to create a job_script without the proper permission.
     We show this by trying to create a job_script without a permission that allow "create" then assert
     that the job_script still does not exists in the database, and the correct status code (403) is returned.
     and that the boto3 method is never called.
     """
-    inserted_application_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(application_owner_email="owner1@org.com"),
+    inserted_application_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(
+            application_owner_email="owner1@org.com",
+        ),
     )
 
     inject_security_header("owner1@org.com", "INVALID_PERMISSION")
     response = await client.post(
         "/jobbergate/job-scripts/",
         json=fill_job_script_data(
             application_id=inserted_application_id,
             param_dict=param_dict,
         ),
     )
 
     assert response.status_code == status.HTTP_403_FORBIDDEN
-
-    count = await database.fetch_all("SELECT COUNT(*) FROM job_scripts")
-    assert count[0][0] == 0
+    assert await fetch_count(synth_session, job_scripts_table) == 0
 
 
 @pytest.mark.asyncio
-@database.transaction(force_rollback=True)
 async def test_create_job_script_without_application(
+    synth_session,
     fill_job_script_data,
     param_dict,
     client,
     inject_security_header,
 ):
     """
     Test that is not possible to create a job_script without an application.
@@ -278,24 +275,22 @@
 
     response = await client.post(
         "/jobbergate/job-scripts/",
         json=fill_job_script_data(application_id=9999, param_dict=param_dict),
     )
 
     assert response.status_code == status.HTTP_404_NOT_FOUND
-
-    count = await database.fetch_all("SELECT COUNT(*) FROM job_scripts")
-    assert count[0][0] == 0
+    assert await fetch_count(synth_session, job_scripts_table) == 0
 
 
-@database.transaction(force_rollback=True)
 @pytest.mark.asyncio
 @mock.patch("jobbergate_api.apps.applications.application_files.ApplicationFiles.get_from_s3")
 async def test_create_job_script_file_not_found(
     mocked_get_application_files_from_s3,
+    synth_session,
     fill_application_data,
     fill_job_script_data,
     param_dict,
     client,
     inject_security_header,
 ):
     """
@@ -303,94 +298,91 @@
 
     This test proves that is not possible to create a job_script with an existing application in the
     database but not in S3, this covers for when for some reason the application file in S3 is deleted but it
     remains in the database. We show this by trying to create a job_script with an existing application that
     is not in S3 (raises BotoCoreError), then assert that the job_script still does not exists in the
     database, the correct status code (404) is returned and that the boto3 method was called.
     """
-    inserted_application_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(
+    inserted_application_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(
             application_owner_email="owner1@org.com",
-            application_uploaded=True,
+            application_uploaded=False,
         ),
     )
+    assert await fetch_count(synth_session, applications_table) == 1
 
     mocked_get_application_files_from_s3.return_value = ApplicationFiles()
 
     inject_security_header("owner1@org.com", Permissions.JOB_SCRIPTS_EDIT)
     response = await client.post(
         "/jobbergate/job-scripts/",
         json=fill_job_script_data(
             application_id=inserted_application_id,
             param_dict=param_dict,
         ),
     )
 
     assert response.status_code == status.HTTP_422_UNPROCESSABLE_ENTITY
+    assert await fetch_count(synth_session, job_scripts_table) == 0
 
-    count = await database.fetch_all("SELECT COUNT(*) FROM job_scripts")
-    assert count[0][0] == 0
 
-
-@database.transaction(force_rollback=True)
 @pytest.mark.asyncio
 async def test_create_job_script_unable_to_write_file_to_s3(
+    synth_session,
     fill_application_data,
     fill_job_script_data,
     param_dict,
     client,
     inject_security_header,
     dummy_application_config,
     dummy_application_source_file,
     dummy_template,
     mocked_file_manager_factory,
 ):
     """
     Test that a job script is not added to the database when S3 manager gets an error.
     """
-    inserted_application_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(
+    inserted_application_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(
             application_owner_email="owner1@org.com",
-            application_uploaded=True,
+            application_uploaded=False,
         ),
     )
+    assert await fetch_count(synth_session, applications_table) == 1
 
     ApplicationFiles(
         templates={"test_job_script.sh": dummy_template},
         source_file=dummy_application_source_file,
         config_file=dummy_application_config,
     ).write_to_s3(inserted_application_id)
 
-    actual_id_rows = await database.fetch_all("SELECT id FROM job_scripts")
-
     inject_security_header("owner1@org.com", Permissions.JOB_SCRIPTS_EDIT)
     with mock.patch(
         "jobbergate_api.apps.job_scripts.job_script_files.JobScriptFiles.write_to_s3",
         side_effect=KeyError,
     ):
         response = await client.post(
             "/jobbergate/job-scripts/",
             json=fill_job_script_data(
                 application_id=inserted_application_id,
                 param_dict=param_dict,
             ),
         )
 
     assert response.status_code == status.HTTP_422_UNPROCESSABLE_ENTITY
-
-    desired_id_rows = await database.fetch_all("SELECT id FROM job_scripts")
-
-    assert actual_id_rows == desired_id_rows
+    assert await fetch_count(synth_session, job_scripts_table) == 0
 
 
 @pytest.mark.asyncio
-@database.transaction(force_rollback=True)
 async def test_get_job_script_by_id(
+    synth_session,
     client,
     fill_application_data,
     job_script_data,
     fill_job_script_data,
     inject_security_header,
     mocked_file_manager_factory,
 ):
@@ -398,150 +390,151 @@
     Test GET /job-scripts/<id>.
 
     This test proves that GET /job-scripts/<id> returns the correct job-script, owned by
     the user making the request. We show this by asserting that the job_script data
     returned in the response is equal to the job_script data that exists in the database
     for the given job_script id.
     """
-    inserted_application_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(application_owner_email="owner1@org.com"),
-    )
-    inserted_job_script_id = await database.execute(
-        query=job_scripts_table.insert(),
-        values=fill_job_script_data(application_id=inserted_application_id),
+    inserted_application_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(
+            application_owner_email="owner1@org.com",
+            application_name="dummy-application",
+        ),
+    )
+    assert await fetch_count(synth_session, applications_table) == 1
+
+    inserted_job_script_id = await insert_data(
+        synth_session,
+        job_scripts_table,
+        fill_job_script_data(application_id=inserted_application_id),
     )
+    assert await fetch_count(synth_session, job_scripts_table) == 1
 
     main_file_path = pathlib.Path("jobbergate.py")
     dummy_job_script_files = JobScriptFiles(
         main_file_path=main_file_path, files={main_file_path: "print(__name__)"}
     )
     dummy_job_script_files.write_to_s3(inserted_job_script_id)
 
-    count = await database.fetch_all("SELECT COUNT(*) FROM job_scripts")
-    assert count[0][0] == 1
-
     inject_security_header("owner1@org.com", Permissions.JOB_SCRIPTS_VIEW)
-
     response = await client.get(f"/jobbergate/job-scripts/{inserted_job_script_id}")
 
     assert response.status_code == status.HTTP_200_OK
 
     data = response.json()
     assert data["id"] == inserted_job_script_id
     assert data["job_script_name"] == job_script_data["job_script_name"]
     assert data["job_script_owner_email"] == "owner1@org.com"
     assert data["application_id"] == inserted_application_id
+    assert data["application_name"] == "dummy-application"
     assert JobScriptFiles(**data["job_script_files"]) == dummy_job_script_files
 
 
 @pytest.mark.asyncio
-@database.transaction(force_rollback=True)
 async def test_download_job_script_file_by_id__success(
+    synth_session,
     client,
     fill_job_script_data,
     inject_security_header,
     mocked_file_manager_factory,
 ):
     """Test that a job script file can be downloaded."""
-    inserted_job_script_id = await database.execute(
-        query=job_scripts_table.insert(),
-        values=fill_job_script_data(),
+    inserted_job_script_id = await insert_data(
+        synth_session,
+        job_scripts_table,
+        fill_job_script_data(),
     )
+    assert await fetch_count(synth_session, job_scripts_table) == 1
 
     main_file_path = pathlib.Path("jobbergate.py")
     expected_file_content = "print(__name__)"
 
     dummy_job_script_files = JobScriptFiles(
         main_file_path=main_file_path, files={main_file_path: expected_file_content}
     )
     dummy_job_script_files.write_to_s3(inserted_job_script_id)
 
-    count = await database.fetch_all("SELECT COUNT(*) FROM job_scripts")
-    assert count[0][0] == 1
-
     inject_security_header("owner1@org.com", Permissions.JOB_SCRIPTS_VIEW)
     response = await client.get(f"/jobbergate/job-scripts/{inserted_job_script_id}/download")
 
     assert response.status_code == status.HTTP_200_OK
 
     assert response.read() == expected_file_content.encode()
     assert response.headers["filename"] == main_file_path.as_posix()
 
 
 @pytest.mark.asyncio
-@database.transaction(force_rollback=True)
 async def test_download_job_script_file_by_id__job_script_not_found(
+    synth_session,
     client,
     inject_security_header,
 ):
     """Test that a job script file can not be downloaded when its id is not found at the database."""
-    count = await database.fetch_all("SELECT COUNT(*) FROM job_scripts")
-    assert count[0][0] == 0
+    assert await fetch_count(synth_session, job_scripts_table) == 0
 
     inject_security_header("owner1@org.com", Permissions.JOB_SCRIPTS_VIEW)
     response = await client.get("/jobbergate/job-scripts/1/download")
 
     assert response.status_code == status.HTTP_404_NOT_FOUND
-    assert "JobScript with id=1 was not found." in response.text
+    assert "Could not find job_scripts instance with id 1" in response.text
 
 
 @pytest.mark.asyncio
-@database.transaction(force_rollback=True)
 async def test_download_job_script_file_by_id__job_script_file_not_found(
+    synth_session,
     client,
     fill_job_script_data,
     inject_security_header,
     mocked_file_manager_factory,
 ):
     """Test that a job script file can not be downloaded when its not found at s3."""
-    inserted_job_script_id = await database.execute(
-        query=job_scripts_table.insert(),
-        values=fill_job_script_data(),
+    inserted_job_script_id = await insert_data(
+        synth_session,
+        job_scripts_table,
+        fill_job_script_data(),
     )
-
-    count = await database.fetch_all("SELECT COUNT(*) FROM job_scripts")
-    assert count[0][0] == 1
+    assert await fetch_count(synth_session, job_scripts_table) == 1
 
     inject_security_header("owner1@org.com", Permissions.JOB_SCRIPTS_VIEW)
     response = await client.get(f"/jobbergate/job-scripts/{inserted_job_script_id}/download")
 
     assert response.status_code == status.HTTP_404_NOT_FOUND
     assert f"Main file from job_script_id={inserted_job_script_id} was not found." in response.text
 
 
 @pytest.mark.asyncio
-@database.transaction(force_rollback=True)
 async def test_upload_job_script_file_by_id__success(
+    synth_session,
     client,
     fill_job_script_data,
     inject_security_header,
     make_dummy_file,
     time_frame,
     mocked_file_manager_factory,
 ):
     """Test that a job script file can be uploaded."""
-    inserted_job_script_id = await database.execute(
-        query=job_scripts_table.insert(),
-        values=fill_job_script_data(),
+    inserted_job_script_id = await insert_data(
+        synth_session,
+        job_scripts_table,
+        fill_job_script_data(),
     )
+    assert await fetch_count(synth_session, job_scripts_table) == 1
 
     main_file_path = pathlib.Path("jobbergate.py")
 
     old_file_content = "I'm going to be replaced"
     new_file_content = "I'm the new content"
 
     dummy_job_script_files = JobScriptFiles(
         main_file_path=main_file_path, files={main_file_path: old_file_content}
     )
     dummy_job_script_files.write_to_s3(inserted_job_script_id)
 
-    count = await database.fetch_all("SELECT COUNT(*) FROM job_scripts")
-    assert count[0][0] == 1
-
     new_job_script_file = make_dummy_file(main_file_path, content=new_file_content)
 
     inject_security_header("owner1@org.com", Permissions.JOB_SCRIPTS_EDIT)
 
     with time_frame() as window:
         response = await client.patch(
             f"/jobbergate/job-scripts/{inserted_job_script_id}/upload",
@@ -553,242 +546,250 @@
     expected_job_script_files = JobScriptFiles(
         main_file_path=main_file_path, files={main_file_path: new_file_content}
     )
     actual_job_script_files = JobScriptFiles.get_from_s3(inserted_job_script_id)
 
     assert actual_job_script_files == expected_job_script_files
 
-    query = job_scripts_table.select(job_scripts_table.c.id == inserted_job_script_id)
-    job_script = JobScriptResponse.parse_obj(await database.fetch_one(query))
-
+    job_script = await fetch_instance(
+        synth_session, inserted_job_script_id, job_scripts_table, JobScriptResponse
+    )
     assert job_script.updated_at in window
 
 
 @pytest.mark.asyncio
-@database.transaction(force_rollback=True)
 async def test_upload_job_script_file_by_id__job_script_not_found(
+    synth_session,
     client,
     inject_security_header,
     make_dummy_file,
 ):
-    """Test that a job script file can be uploaded when its id is not found at the database."""
-    count = await database.fetch_all("SELECT COUNT(*) FROM job_scripts")
-    assert count[0][0] == 0
+    """Test that a job script file cannot be uploaded when its id is not found at the database."""
+    assert await fetch_count(synth_session, job_scripts_table) == 0
 
     main_file_path = pathlib.Path("jobbergate.py")
     main_file_content = "I'm going to be replaced"
 
     new_job_script_file = make_dummy_file(main_file_path, content=main_file_content)
 
     inject_security_header("owner1@org.com", Permissions.JOB_SCRIPTS_EDIT)
 
     response = await client.patch(
         "/jobbergate/job-scripts/1/upload",
         files={"job_script_file": open(new_job_script_file, "rb")},
     )
 
     assert response.status_code == status.HTTP_404_NOT_FOUND
-    assert "Job Script with job_script_id=1 was not found." in response.text
+    assert "Could not find job_scripts instance with id 1" in response.text
 
 
 @pytest.mark.asyncio
-@database.transaction(force_rollback=True)
 async def test_upload_job_script_file_by_id__job_script_file_not_found(
+    synth_session,
     client,
     fill_job_script_data,
     inject_security_header,
     make_dummy_file,
     mocked_file_manager_factory,
 ):
     """Test that a job script file can not be uploaded when its not found at s3."""
-    inserted_job_script_id = await database.execute(
-        query=job_scripts_table.insert(),
-        values=fill_job_script_data(),
+    inserted_job_script_id = await insert_data(
+        synth_session,
+        job_scripts_table,
+        fill_job_script_data(),
     )
-
-    main_file_path = pathlib.Path("jobbergate.py")
+    assert await fetch_count(synth_session, job_scripts_table) == 1
 
     main_file_path = pathlib.Path("jobbergate.py")
     new_file_content = "I'm going to be replaced"
-
-    new_job_script_file = make_dummy_file(main_file_path, content=new_file_content)
-
-    count = await database.fetch_all("SELECT COUNT(*) FROM job_scripts")
-    assert count[0][0] == 1
-
     new_job_script_file = make_dummy_file(main_file_path, content=new_file_content)
 
     inject_security_header("owner1@org.com", Permissions.JOB_SCRIPTS_EDIT)
 
     response = await client.patch(
         f"/jobbergate/job-scripts/{inserted_job_script_id}/upload",
         files={"job_script_file": open(new_job_script_file, "rb")},
     )
 
     assert response.status_code == status.HTTP_404_NOT_FOUND
     assert f"Main file from job_script_id={inserted_job_script_id} was not found." in response.text
 
 
 @pytest.mark.asyncio
-@database.transaction(force_rollback=True)
 async def test_upload_job_script_file_by_id__fails_for_non_owner(
+    synth_session,
     client,
     fill_job_script_data,
     inject_security_header,
     make_dummy_file,
 ):
     """Test that a job script file can not be uploaded by a non owner."""
-    inserted_job_script_id = await database.execute(
-        query=job_scripts_table.insert(),
-        values=fill_job_script_data(
+    inserted_job_script_id = await insert_data(
+        synth_session,
+        job_scripts_table,
+        fill_job_script_data(
             job_script_owner_email="owner1@org.com",
         ),
     )
 
     main_file_path = pathlib.Path("jobbergate.py")
-
     new_file_content = "I'm the new content"
-
-    count = await database.fetch_all("SELECT COUNT(*) FROM job_scripts")
-    assert count[0][0] == 1
-
     new_job_script_file = make_dummy_file(main_file_path, content=new_file_content)
 
     inject_security_header("non-owner@org.com", Permissions.JOB_SCRIPTS_EDIT)
 
     response = await client.patch(
         f"/jobbergate/job-scripts/{inserted_job_script_id}/upload",
         files={"job_script_file": open(new_job_script_file, "rb")},
     )
 
     assert response.status_code == status.HTTP_403_FORBIDDEN
     assert "does not own" in response.text
 
 
 @pytest.mark.asyncio
-@database.transaction(force_rollback=True)
 async def test_get_job_script_by_id_file_not_found_at_s3(
+    synth_session,
     client,
     fill_application_data,
     fill_job_script_data,
     inject_security_header,
     mocked_file_manager_factory,
 ):
     """
     Test if 404 is returned if a jobscript exists in the database but the file was not found in S3.
     """
-    inserted_application_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(application_owner_email="owner1@org.com"),
-    )
-    inserted_job_script_id = await database.execute(
-        query=job_scripts_table.insert(),
-        values=fill_job_script_data(application_id=inserted_application_id),
+    inserted_application_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(
+            application_owner_email="owner1@org.com",
+        ),
     )
+    assert await fetch_count(synth_session, applications_table) == 1
 
-    inject_security_header("owner1@org.com", Permissions.JOB_SCRIPTS_VIEW)
+    inserted_job_script_id = await insert_data(
+        synth_session,
+        job_scripts_table,
+        fill_job_script_data(application_id=inserted_application_id),
+    )
+    assert await fetch_count(synth_session, job_scripts_table) == 1
 
+    inject_security_header("owner1@org.com", Permissions.JOB_SCRIPTS_VIEW)
     response = await client.get(f"/jobbergate/job-scripts/{inserted_job_script_id}")
 
     assert response.status_code == status.HTTP_404_NOT_FOUND
     assert "JobScript file not found for id=" in response.text
 
 
 @pytest.mark.asyncio
-@database.transaction(force_rollback=True)
 async def test_get_job_script_by_id_invalid(client, inject_security_header):
     """
     Test the correct response code is returned when a job_script does not exist.
 
     This test proves that GET /job-script/<id> returns the correct response code when the
     requested job_script does not exist. We show this by asserting that the status code
     returned is what we would expect given the job_script requested doesn't exist (404).
     """
     inject_security_header("owner1@org.com", Permissions.JOB_SCRIPTS_VIEW)
     response = await client.get("/jobbergate/job-scripts/9999")
     assert response.status_code == status.HTTP_404_NOT_FOUND
 
 
 @pytest.mark.asyncio
-@database.transaction(force_rollback=True)
 async def test_get_job_script_by_id_bad_permission(
+    synth_session,
     client,
     fill_application_data,
     fill_job_script_data,
     inject_security_header,
 ):
     """
     Test the correct response code is returned when the user don't have the proper permission.
 
     This test proves that GET /job-script/<id> returns the correct response code when the
     user don't have the proper permission. We show this by asserting that the status code
     returned is what we would expect (403).
     """
-    inserted_application_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(application_owner_email="owner1@org.com"),
-    )
-    inserted_job_script_id = await database.execute(
-        query=job_scripts_table.insert(),
-        values=fill_job_script_data(application_id=inserted_application_id),
+    inserted_application_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(
+            application_owner_email="owner1@org.com",
+        ),
+    )
+    assert await fetch_count(synth_session, applications_table) == 1
+
+    inserted_job_script_id = await insert_data(
+        synth_session,
+        job_scripts_table,
+        fill_job_script_data(application_id=inserted_application_id),
     )
+    assert await fetch_count(synth_session, job_scripts_table) == 1
+
     inject_security_header("owner1@org.com", "INVALID_PERMISSION")
     response = await client.get(f"/jobbergate/job-scripts/{inserted_job_script_id}")
     assert response.status_code == status.HTTP_403_FORBIDDEN
 
 
 @pytest.mark.asyncio
-@database.transaction(force_rollback=True)
-async def test_get_job_script__no_params(
+async def test_get_job_scripts__no_params(
+    synth_session,
     client,
     fill_application_data,
     fill_all_job_script_data,
     inject_security_header,
 ):
     """
     Test GET /job-scripts/ returns only job_scripts owned by the user making the request.
 
     This test proves that GET /job-scripts/ returns the correct job_scripts for the user making
     the request. We show this by asserting that the job_scripts returned in the response are
     only job_scripts owned by the user making the request. This test also ensures that archived
     job_scripts are not included by default.
     """
-    inserted_application_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(application_owner_email="owner1@org.com"),
-    )
-    await database.execute_many(
-        query=job_scripts_table.insert(),
-        values=fill_all_job_script_data(
+    inserted_application_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(
+            application_owner_email="owner1@org.com",
+        ),
+    )
+    assert await fetch_count(synth_session, applications_table) == 1
+
+    await synth_session.execute(
+        job_scripts_table.insert(),
+        fill_all_job_script_data(
             dict(
                 job_script_name="js1",
                 job_script_owner_email="owner1@org.com",
                 application_id=inserted_application_id,
+                is_archived=False,
             ),
             dict(
                 job_script_name="js2",
                 job_script_owner_email="owner999@org.com",
                 application_id=inserted_application_id,
+                is_archived=False,
             ),
             dict(
                 job_script_name="js3",
                 job_script_owner_email="owner1@org.com",
                 application_id=inserted_application_id,
+                is_archived=False,
             ),
             dict(
                 job_script_name="js4",
                 job_script_owner_email="owner1@org.com",
                 application_id=inserted_application_id,
                 is_archived=True,
             ),
         ),
     )
-
-    count = await database.fetch_all("SELECT COUNT(*) FROM job_scripts")
-    assert count[0][0] == 4
+    assert await fetch_count(synth_session, job_scripts_table) == 4
 
     inject_security_header("owner1@org.com", Permissions.JOB_SCRIPTS_VIEW)
     response = await client.get("/jobbergate/job-scripts/")
     assert response.status_code == status.HTTP_200_OK
 
     data = response.json()
     results = data.get("results")
@@ -800,87 +801,94 @@
         total=2,
         start=None,
         limit=None,
     )
 
 
 @pytest.mark.asyncio
-@database.transaction(force_rollback=True)
 async def test_get_job_scripts__bad_permission(
+    synth_session,
     client,
     fill_application_data,
     fill_job_script_data,
     inject_security_header,
 ):
     """
     Test GET /job-scripts/ returns 403 since the user don't have the proper permission.
 
     This test proves that GET /job-scripts/ returns the 403 status code when the user making the request
     don't have the permission to list. We show this by asserting that the response status code is 403.
     """
-    inserted_application_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(application_owner_email="owner1@org.com"),
-    )
-    await database.execute(
-        query=job_scripts_table.insert(),
-        values=fill_job_script_data(application_id=inserted_application_id),
+    inserted_application_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(
+            application_owner_email="owner1@org.com",
+        ),
     )
+    assert await fetch_count(synth_session, applications_table) == 1
 
-    count = await database.fetch_all("SELECT COUNT(*) FROM job_scripts")
-    assert count[0][0] == 1
+    await insert_data(
+        synth_session,
+        job_scripts_table,
+        fill_job_script_data(application_id=inserted_application_id),
+    )
+    assert await fetch_count(synth_session, job_scripts_table) == 1
 
     inject_security_header("owner1@org.com", "INVALID_PERMISSION")
     response = await client.get("/jobbergate/job-scripts/")
     assert response.status_code == status.HTTP_403_FORBIDDEN
 
 
 @pytest.mark.asyncio
-@database.transaction(force_rollback=True)
 async def test_get_job_scripts__with_all_param(
+    synth_session,
     client,
     fill_application_data,
     fill_all_job_script_data,
     inject_security_header,
 ):
     """
     Test that listing job_scripts, when all=True, contains job_scripts owned by other users.
 
     This test proves that the user making the request can see job_scripts owned by other users.
     We show this by creating three job_scripts, one that are owned by the user making the request, and two
     owned by another user. Assert that the response to GET /job-scripts/?all=True includes all three
     job_scripts.
     """
-    inserted_application_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(application_owner_email="owner1@org.com"),
-    )
-    await database.execute_many(
-        query=job_scripts_table.insert(),
-        values=fill_all_job_script_data(
-            {
-                "job_script_name": "script1",
-                "job_script_owner_email": "owner1@org.com",
-                "application_id": inserted_application_id,
-            },
-            {
-                "job_script_name": "script2",
-                "job_script_owner_email": "owner999@org.com",
-                "application_id": inserted_application_id,
-            },
-            {
-                "job_script_name": "script3",
-                "job_script_owner_email": "owner1@org.com",
-                "application_id": inserted_application_id,
-            },
+    inserted_application_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(
+            application_owner_email="owner1@org.com",
         ),
     )
+    assert await fetch_count(synth_session, applications_table) == 1
 
-    count = await database.fetch_all("SELECT COUNT(*) FROM job_scripts")
-    assert count[0][0] == 3
+    await synth_session.execute(
+        job_scripts_table.insert(),
+        fill_all_job_script_data(
+            dict(
+                job_script_name="script1",
+                job_script_owner_email="owner1@org.com",
+                application_id=inserted_application_id,
+            ),
+            dict(
+                job_script_name="script2",
+                job_script_owner_email="owner999@org.com",
+                application_id=inserted_application_id,
+            ),
+            dict(
+                job_script_name="script3",
+                job_script_owner_email="owner1@org.com",
+                application_id=inserted_application_id,
+            ),
+        ),
+    )
+    assert await fetch_count(synth_session, job_scripts_table) == 3
 
     inject_security_header("owner1@org.com", Permissions.JOB_SCRIPTS_VIEW)
     response = await client.get("/jobbergate/job-scripts/?all=True")
     assert response.status_code == status.HTTP_200_OK
 
     data = response.json()
     results = data.get("results")
@@ -892,56 +900,61 @@
         total=3,
         start=None,
         limit=None,
     )
 
 
 @pytest.mark.asyncio
-@database.transaction(force_rollback=True)
 async def test_get_job_scripts__with_include_archived_param(
+    synth_session,
     client,
     fill_application_data,
     fill_all_job_script_data,
     inject_security_header,
 ):
     """
     Test that listing job_scripts, when include_archived=True, contains archived job_scripts.
 
     This test proves that the user making the request can see archived job_scripts.
     We show this by creating three job_scripts, one that is archived, and two that are not.
     Assert that the response to GET /job-scripts/?include_archived=True includes all three job_scripts.
     """
-    inserted_application_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(application_owner_email="owner1@org.com"),
-    )
-    await database.execute_many(
-        query=job_scripts_table.insert(),
-        values=fill_all_job_script_data(
-            {
-                "job_script_name": "script1",
-                "job_script_owner_email": "owner1@org.com",
-                "application_id": inserted_application_id,
-            },
-            {
-                "job_script_name": "script2",
-                "job_script_owner_email": "owner1@org.com",
-                "application_id": inserted_application_id,
-                "is_archived": True,
-            },
-            {
-                "job_script_name": "script3",
-                "job_script_owner_email": "owner1@org.com",
-                "application_id": inserted_application_id,
-            },
+    inserted_application_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(
+            application_owner_email="owner1@org.com",
         ),
     )
+    assert await fetch_count(synth_session, applications_table) == 1
 
-    count = await database.fetch_all("SELECT COUNT(*) FROM job_scripts")
-    assert count[0][0] == 3
+    await synth_session.execute(
+        job_scripts_table.insert(),
+        fill_all_job_script_data(
+            dict(
+                job_script_name="script1",
+                job_script_owner_email="owner1@org.com",
+                application_id=inserted_application_id,
+                is_archived=False,
+            ),
+            dict(
+                job_script_name="script2",
+                job_script_owner_email="owner1@org.com",
+                application_id=inserted_application_id,
+                is_archived=True,
+            ),
+            dict(
+                job_script_name="script3",
+                job_script_owner_email="owner1@org.com",
+                application_id=inserted_application_id,
+                is_archived=False,
+            ),
+        ),
+    )
+    assert await fetch_count(synth_session, job_scripts_table) == 3
 
     inject_security_header("owner1@org.com", Permissions.JOB_SCRIPTS_VIEW)
     response = await client.get("/jobbergate/job-scripts/?include_archived=True")
     assert response.status_code == status.HTTP_200_OK
 
     data = response.json()
     results = data.get("results")
@@ -953,55 +966,62 @@
         total=3,
         start=None,
         limit=None,
     )
 
 
 @pytest.mark.asyncio
-@database.transaction(force_rollback=True)
-async def test_get_job_scripts__with_search_param(client, inject_security_header, fill_application_data):
+async def test_get_job_scripts__with_search_param(
+    synth_session, client, inject_security_header, fill_application_data
+):
     """
     Test that listing job scripts, when search=<search terms>, returns matches.
 
     This test proves that the user making the request will be shown job scripts that match the search string.
     We show this by creating job scripts and using various search queries to match against them.
 
     Assert that the response to GET /job_scripts?search=<search terms> includes correct matches.
     """
-    inserted_application_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(application_owner_email="owner1@org.com"),
+    inserted_application_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(
+            application_owner_email="owner1@org.com",
+        ),
     )
+    assert await fetch_count(synth_session, applications_table) == 1
+
     common = dict(application_id=inserted_application_id)
-    await database.execute_many(
-        query=job_scripts_table.insert(),
-        values=[
+    await synth_session.execute(
+        job_scripts_table.insert(),
+        [
             dict(
                 id=1,
                 job_script_name="test name one",
                 job_script_owner_email="one@org.com",
+                job_script_description=None,
                 **common,
             ),
             dict(
                 id=2,
                 job_script_name="test name two",
                 job_script_owner_email="two@org.com",
+                job_script_description=None,
                 **common,
             ),
             dict(
                 id=22,
                 job_script_name="test name twenty-two",
                 job_script_owner_email="twenty-two@org.com",
                 job_script_description="a long description of this job_script",
                 **common,
             ),
         ],
     )
-    count = await database.fetch_all("SELECT COUNT(*) FROM job_scripts")
-    assert count[0][0] == 3
+    assert await fetch_count(synth_session, job_scripts_table) == 3
 
     inject_security_header("admin@org.com", Permissions.JOB_SCRIPTS_VIEW)
 
     response = await client.get("/jobbergate/job-scripts?all=true&search=one")
     assert response.status_code == status.HTTP_200_OK
     data = response.json()
     results = data.get("results")
@@ -1023,57 +1043,61 @@
     assert response.status_code == status.HTTP_200_OK
     data = response.json()
     results = data.get("results")
     assert [d["id"] for d in results] == [1, 2, 22]
 
 
 @pytest.mark.asyncio
-@database.transaction(force_rollback=True)
 async def test_get_job_scripts__with_sort_params(
+    synth_session,
     client,
     fill_application_data,
     inject_security_header,
 ):
     """
     Test that listing job_scripts with sort params returns correctly ordered matches.
 
     This test proves that the user making the request will be shown job_scripts sorted in the correct order
     according to the ``sort_field`` and ``sort_ascending`` parameters.
     We show this by creating job_scripts and using various sort parameters to order them.
 
     Assert that the response to GET /job_scripts?sort_field=<field>&sort_ascending=<bool> includes correctly
     sorted job_script.
     """
-    inserted_application_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(application_owner_email="admin@org.com"),
+    inserted_application_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(
+            application_owner_email="owner1@org.com",
+        ),
     )
+    assert await fetch_count(synth_session, applications_table) == 1
+
     common = dict(
         job_script_owner_email="admin@org.com",
         application_id=inserted_application_id,
     )
-    await database.execute_many(
-        query=job_scripts_table.insert(),
-        values=[
+    await synth_session.execute(
+        job_scripts_table.insert(),
+        [
             dict(
                 job_script_name="Z",
                 **common,
             ),
             dict(
                 job_script_name="Y",
                 **common,
             ),
             dict(
                 job_script_name="X",
                 **common,
             ),
         ],
     )
-    count = await database.fetch_all("SELECT COUNT(*) FROM job_scripts")
-    assert count[0][0] == 3
+    assert await fetch_count(synth_session, job_scripts_table) == 3
 
     inject_security_header("admin@org.com", Permissions.JOB_SCRIPTS_VIEW)
 
     response = await client.get("/jobbergate/job-scripts?sort_field=id")
     assert response.status_code == status.HTTP_200_OK
     data = response.json()
     results = data.get("results")
@@ -1093,45 +1117,48 @@
 
     response = await client.get("/jobbergate/job-scripts?all=true&sort_field=job_script_data_as_string")
     assert response.status_code == status.HTTP_400_BAD_REQUEST
     assert "Invalid sorting column requested" in response.text
 
 
 @pytest.mark.asyncio
-@database.transaction(force_rollback=True)
 async def test_get_job_scripts__with_pagination(
+    synth_session,
     client,
     fill_application_data,
     fill_job_script_data,
     inject_security_header,
 ):
     """
     Test that listing job_scripts works with pagination.
 
     This test proves that the user making the request can see job_scripts paginated.
     We show this by creating three job_scripts and assert that the response is correctly paginated.
     """
-    inserted_application_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(application_owner_email="owner1@org.com"),
-    )
-    await database.execute_many(
-        query=job_scripts_table.insert(),
-        values=[
+    inserted_application_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(
+            application_owner_email="owner1@org.com",
+        ),
+    )
+    assert await fetch_count(synth_session, applications_table) == 1
+
+    await synth_session.execute(
+        job_scripts_table.insert(),
+        [
             fill_job_script_data(
                 job_script_name=f"script{i}",
                 job_script_owner_email="owner1@org.com",
                 application_id=inserted_application_id,
             )
             for i in range(1, 6)
         ],
     )
-
-    count = await database.fetch_all("SELECT COUNT(*) FROM job_scripts")
-    assert count[0][0] == 5
+    assert await fetch_count(synth_session, job_scripts_table) == 5
 
     inject_security_header("owner1@org.com", Permissions.JOB_SCRIPTS_VIEW)
     response = await client.get("/jobbergate/job-scripts?start=0&limit=1")
     assert response.status_code == status.HTTP_200_OK
 
     data = response.json()
     results = data.get("results")
@@ -1161,52 +1188,47 @@
     assert [d["job_script_name"] for d in results] == ["script5"]
 
     pagination = data.get("pagination")
     assert pagination == dict(total=5, start=2, limit=2)
 
 
 @pytest.mark.asyncio
-@database.transaction(force_rollback=True)
 async def test_get_job_scripts__from_application_id(
+    synth_session,
     client,
     fill_application_data,
     fill_all_job_script_data,
     inject_security_header,
 ):
     """
     Test listing job_scripts when from_application_id=<num> is present.
 
     Only the job-scripts produced from the application with id=<num> should be returned.
     """
-    inserted_application_id_1 = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(application_owner_email="owner1@org.com"),
-    )
-    inserted_application_id_2 = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(application_owner_email="owner1@org.com"),
-    )
-    inserted_application_id_3 = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(application_owner_email="owner1@org.com"),
-    )
-    await database.execute_many(
-        query=job_scripts_table.insert(),
-        values=fill_all_job_script_data(
-            {"application_id": inserted_application_id_1},
-            {"application_id": inserted_application_id_1},
-            {"application_id": inserted_application_id_2},
-            {"application_id": inserted_application_id_2},
-            {"application_id": inserted_application_id_3},
-            {"application_id": inserted_application_id_3},
+    raw_results = await synth_session.execute(
+        applications_table.insert().returning(applications_table.c.id),
+        [fill_application_data(application_owner_email="owner1@org.com")] * 3,
+    )
+    (inserted_application_id_1, inserted_application_id_2, inserted_application_id_3) = (
+        r.id for r in raw_results
+    )
+    assert await fetch_count(synth_session, applications_table) == 3
+
+    await synth_session.execute(
+        job_scripts_table.insert(),
+        fill_all_job_script_data(
+            dict(application_id=inserted_application_id_1),
+            dict(application_id=inserted_application_id_1),
+            dict(application_id=inserted_application_id_2),
+            dict(application_id=inserted_application_id_2),
+            dict(application_id=inserted_application_id_3),
+            dict(application_id=inserted_application_id_3),
         ),
     )
-
-    count = await database.fetch_all("SELECT COUNT(*) FROM job_scripts")
-    assert count[0][0] == 6
+    assert await fetch_count(synth_session, job_scripts_table) == 6
 
     inject_security_header("owner1@org.com", Permissions.JOB_SCRIPTS_VIEW)
 
     for application_id in [inserted_application_id_1, inserted_application_id_2, inserted_application_id_3]:
         response = await client.get(
             f"/jobbergate/job-scripts/?from_application_id={application_id}",
         )
@@ -1215,38 +1237,45 @@
         data = response.json()
         results = data.get("results")
         assert {d["application_id"] for d in results} == {application_id}, f"{application_id=}"
 
 
 @pytest.mark.freeze_time
 @pytest.mark.asyncio
-@database.transaction(force_rollback=True)
 async def test_update_job_script(
+    synth_session,
     client,
     fill_application_data,
     fill_job_script_data,
     inject_security_header,
     time_frame,
     mocked_file_manager_factory,
 ):
     """
     Test update job_script via PUT.
 
     This test proves that the job_script values are correctly updated following a PUT request to the
     /job-scripts/<id> endpoint. We show this by assert the response status code to 201, the response data
     corresponds to the updated data, and the data in the database is also updated.
     """
-    inserted_application_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(application_owner_email="owner1@org.com"),
-    )
-    inserted_job_script_id = await database.execute(
-        query=job_scripts_table.insert(),
-        values=fill_job_script_data(application_id=inserted_application_id),
+    inserted_application_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(
+            application_owner_email="owner1@org.com",
+        ),
     )
+    assert await fetch_count(synth_session, applications_table) == 1
+
+    inserted_job_script_id = await insert_data(
+        synth_session,
+        job_scripts_table,
+        fill_job_script_data(application_id=inserted_application_id),
+    )
+    assert await fetch_count(synth_session, job_scripts_table) == 1
 
     main_file_path = "jobbergate.py"
     main_file_content = "print(__name__)"
     dummy_job_script_files = JobScriptFiles(
         main_file_path=main_file_path, files={main_file_path: main_file_content}
     )
 
@@ -1271,26 +1300,25 @@
     assert data["job_script_name"] == "new name"
     assert data["job_script_description"] == "new description"
     assert JobScriptFiles(**data["job_script_files"]) == dummy_job_script_files
     assert JobScriptFiles.get_from_s3(inserted_job_script_id) == dummy_job_script_files
     assert data["id"] == inserted_job_script_id
     assert data["is_archived"] is True
 
-    query = job_scripts_table.select(job_scripts_table.c.id == inserted_job_script_id)
-    job_script = JobScriptResponse.parse_obj(await database.fetch_one(query))
-
+    job_script = await fetch_instance(
+        synth_session, inserted_job_script_id, job_scripts_table, JobScriptResponse
+    )
     assert job_script is not None
     assert job_script.job_script_name == "new name"
     assert job_script.job_script_description == "new description"
     assert job_script.updated_at in window
     assert job_script.is_archived
 
 
 @pytest.mark.asyncio
-@database.transaction(force_rollback=True)
 async def test_update_job_script_not_found(
     client,
     inject_security_header,
 ):
     """
     Test that it is not possible to update a job_script not found.
 
@@ -1299,42 +1327,43 @@
     """
     inject_security_header("owner1@org.com", Permissions.JOB_SCRIPTS_EDIT)
     response = await client.put("/jobbergate/job-scripts/123", json={"job_script_name": "new name"})
 
     assert response.status_code == status.HTTP_404_NOT_FOUND
 
 
-@database.transaction(force_rollback=True)
 @pytest.mark.asyncio
 async def test_update_job_script_unable_to_write_file_to_s3(
+    synth_session,
     fill_application_data,
     fill_job_script_data,
     client,
     inject_security_header,
     mocked_file_manager_factory,
 ):
     """
     Test that a job script is not updated to the database when S3 manager gets an error.
     """
-    inserted_application_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(application_owner_email="owner1@org.com"),
+    inserted_application_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(
+            application_owner_email="owner1@org.com",
+        ),
     )
+    assert await fetch_count(synth_session, applications_table) == 1
 
-    inserted_job_script_id = await database.execute(
-        query=job_scripts_table.insert(),
-        values=fill_job_script_data(application_id=inserted_application_id),
+    inserted_job_script_id = await insert_data(
+        synth_session,
+        job_scripts_table,
+        fill_job_script_data(application_id=inserted_application_id),
     )
-
-    query = job_scripts_table.select(job_scripts_table.c.id == inserted_job_script_id)
-
-    desired_jobscript_data = JobScriptResponse.parse_obj(await database.fetch_one(query))
+    assert await fetch_count(synth_session, job_scripts_table) == 1
 
     inject_security_header("owner1@org.com", Permissions.JOB_SCRIPTS_EDIT)
-
     with mock.patch(
         "jobbergate_api.apps.job_scripts.job_script_files.JobScriptFiles.write_to_s3",
         side_effect=KeyError,
     ):
         response = await client.put(
             f"/jobbergate/job-scripts/{inserted_job_script_id}",
             json={
@@ -1343,250 +1372,270 @@
                 "job_script_data_as_string": "new value",
             },
         )
 
     assert response.status_code == status.HTTP_404_NOT_FOUND
     assert "not found in S3" in response.text
 
-    actual_jobscript_data = JobScriptResponse.parse_obj(await database.fetch_one(query))
-
-    assert desired_jobscript_data.json() == actual_jobscript_data.json()
-
 
 @pytest.mark.asyncio
-@database.transaction(force_rollback=True)
 async def test_update_job_script_bad_permission(
+    synth_session,
     client,
     fill_application_data,
     fill_job_script_data,
     inject_security_header,
 ):
     """
     Test that it is not possible to update a job_script if the user don't have the proper permission.
 
     This test proves that it is not possible to update a job_script if the user don't have permission. We
     show this by asserting that the response status code of the request is 403, and that the data stored in
     the database for the job_script is not updated.
     """
-    inserted_application_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(application_owner_email="owner1@org.com"),
-    )
-    await database.execute(
-        query=job_scripts_table.insert(),
-        values=fill_job_script_data(job_script_name="target-js", application_id=inserted_application_id),
+    inserted_application_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(
+            application_owner_email="owner1@org.com",
+        ),
     )
+    assert await fetch_count(synth_session, applications_table) == 1
+
+    inserted_job_script_id = await insert_data(
+        synth_session,
+        job_scripts_table,
+        fill_job_script_data(job_script_name="target-js", application_id=inserted_application_id),
+    )
+    assert await fetch_count(synth_session, job_scripts_table) == 1
 
     inject_security_header("owner1@org.com", "INVALID_PERMISSION")
     response = await client.put("/jobbergate/job-scripts/1", data={"job_script_name": "new name"})
 
     assert response.status_code == status.HTTP_403_FORBIDDEN
 
-    query = job_scripts_table.select(job_scripts_table.c.job_script_name == "target-js")
-    job_script_row = await database.fetch_one(query)
-
-    assert job_script_row is not None
-    assert job_script_row["job_script_name"] == "target-js"
+    job_script = await fetch_instance(
+        synth_session, inserted_job_script_id, job_scripts_table, JobScriptResponse
+    )
+    assert job_script is not None
+    assert job_script.job_script_name == "target-js"
 
 
 @pytest.mark.asyncio
-@database.transaction(force_rollback=True)
 async def test_update_job_script_non_owner(
+    synth_session,
     client,
     fill_application_data,
     fill_job_script_data,
     inject_security_header,
 ):
     """
     Test that it is not possible to update a job_script if the user is not the owner.
     """
-    inserted_application_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(application_owner_email="owner1@org.com"),
-    )
-    job_script_id = await database.execute(
-        query=job_scripts_table.insert(),
-        values=fill_job_script_data(job_script_name="target-js", application_id=inserted_application_id),
+    inserted_application_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(
+            application_owner_email="owner1@org.com",
+        ),
     )
+    assert await fetch_count(synth_session, applications_table) == 1
+
+    inserted_job_script_id = await insert_data(
+        synth_session,
+        job_scripts_table,
+        fill_job_script_data(job_script_name="target-js", application_id=inserted_application_id),
+    )
+    assert await fetch_count(synth_session, job_scripts_table) == 1
 
     inject_security_header("non-owner@org.com", Permissions.JOB_SCRIPTS_EDIT)
     response = await client.put(
-        f"/jobbergate/job-scripts/{job_script_id}", json={"job_script_name": "new name"}
+        f"/jobbergate/job-scripts/{inserted_job_script_id}", json={"job_script_name": "new name"}
     )
 
     assert response.status_code == status.HTTP_403_FORBIDDEN
     assert "does not own" in response.text
 
 
 @pytest.mark.asyncio
-@database.transaction(force_rollback=True)
 async def test_delete_job_script(
+    synth_session,
     client,
     fill_application_data,
     fill_job_script_data,
     inject_security_header,
 ):
     """
     Test delete job_script via DELETE.
 
     This test proves that a job_script is successfully deleted via a DELETE request to the /job-scripts/<id>
     endpoint. We show this by asserting that the job_script no longer exists in the database after the
     request is made and the correct status code is returned (204).
     """
-    inserted_application_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(),
-    )
-    inserted_job_script_id = await database.execute(
-        query=job_scripts_table.insert(),
-        values=fill_job_script_data(application_id=inserted_application_id),
+    inserted_application_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(),
+    )
+    assert await fetch_count(synth_session, applications_table) == 1
+
+    inserted_job_script_id = await insert_data(
+        synth_session,
+        job_scripts_table,
+        fill_job_script_data(application_id=inserted_application_id),
     )
-
-    count = await database.fetch_all("SELECT COUNT(*) FROM job_scripts")
-    assert count[0][0] == 1
+    assert await fetch_count(synth_session, job_scripts_table) == 1
 
     with mock.patch(
         "jobbergate_api.apps.job_scripts.job_script_files.JobScriptFiles.delete_from_s3",
     ) as mocked_delete:
         inject_security_header("owner1@org.com", Permissions.JOB_SCRIPTS_EDIT)
         response = await client.delete(f"/jobbergate/job-scripts/{inserted_job_script_id}")
 
     assert response.status_code == status.HTTP_204_NO_CONTENT
 
     mocked_delete.assert_called_once()
 
-    count = await database.fetch_all("SELECT COUNT(*) FROM job_scripts")
-    assert count[0][0] == 0
+    assert await fetch_count(synth_session, job_scripts_table) == 0
 
 
 @pytest.mark.asyncio
-@database.transaction(force_rollback=True)
 async def test_delete_job_script_not_found(client, inject_security_header):
     """
     Test that it is not possible to delete a job_script that is not found.
 
     This test proves that it is not possible to delete a job_script if it does not exists. We show this by
     assert that a 404 response status code is returned.
     """
     inject_security_header("owner1@org.com", Permissions.JOB_SCRIPTS_EDIT)
     response = await client.delete("/jobbergate/job-scripts/9999")
 
     assert response.status_code == status.HTTP_404_NOT_FOUND
 
 
 @pytest.mark.asyncio
-@database.transaction(force_rollback=True)
 async def test_delete_job_script_bad_permission(
+    synth_session,
     client,
     fill_application_data,
     fill_job_script_data,
     inject_security_header,
 ):
     """
     Test that it is not possible to delete a job_script when the user don't have the permission.
 
     This test proves that it is not possible to delete a job_script if the user don't have the permission.
     We show this by assert that a 403 response status code is returned and the job_script still exists in
     the database after the request.
     """
-    inserted_application_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(),
-    )
-    inserted_job_script_id = await database.execute(
-        query=job_scripts_table.insert(),
-        values=fill_job_script_data(application_id=inserted_application_id),
+    inserted_application_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(),
+    )
+    assert await fetch_count(synth_session, applications_table) == 1
+
+    inserted_job_script_id = await insert_data(
+        synth_session,
+        job_scripts_table,
+        fill_job_script_data(application_id=inserted_application_id),
     )
-
-    count = await database.fetch_all("SELECT COUNT(*) FROM job_scripts")
-    assert count[0][0] == 1
+    assert await fetch_count(synth_session, job_scripts_table) == 1
 
     inject_security_header("owner1@org.com", "INVALID_PERMISSION")
     response = await client.delete(f"/jobbergate/job-scripts/{inserted_job_script_id}")
 
     assert response.status_code == status.HTTP_403_FORBIDDEN
 
-    count = await database.fetch_all("SELECT COUNT(*) FROM job_scripts")
-    assert count[0][0] == 1
+    assert await fetch_count(synth_session, job_scripts_table) == 1
 
 
 @pytest.mark.asyncio
-@database.transaction(force_rollback=True)
 async def test_delete_job_script_non_owner(
+    synth_session,
     client,
     fill_application_data,
     fill_job_script_data,
     inject_security_header,
 ):
     """
     Test that it is not possible to delete a job_script when the user is not the owner.
     """
-    inserted_application_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(),
-    )
-    inserted_job_script_id = await database.execute(
-        query=job_scripts_table.insert(),
-        values=fill_job_script_data(application_id=inserted_application_id),
+    inserted_application_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(),
+    )
+    assert await fetch_count(synth_session, applications_table) == 1
+
+    inserted_job_script_id = await insert_data(
+        synth_session,
+        job_scripts_table,
+        fill_job_script_data(application_id=inserted_application_id),
     )
-
-    count = await database.fetch_all("SELECT COUNT(*) FROM job_scripts")
-    assert count[0][0] == 1
+    assert await fetch_count(synth_session, job_scripts_table) == 1
 
     inject_security_header("non-owner@org.com", Permissions.JOB_SCRIPTS_EDIT)
     response = await client.delete(f"/jobbergate/job-scripts/{inserted_job_script_id}")
 
     assert response.status_code == status.HTTP_403_FORBIDDEN
     assert "does not own" in response.text
 
 
 @pytest.mark.asyncio
-@database.transaction(force_rollback=True)
 async def test_delete_job_script__unlinks_job_submissions(
+    synth_session,
     client,
     fill_application_data,
     fill_job_script_data,
     fill_job_submission_data,
     inject_security_header,
 ):
     """
     Test DELETE /job_scripts/<id> correctly deletes a job_script linked to a job_submission.
 
     Test that a the job_script_id field for connected job_submissions is set to null.
     """
-    inserted_application_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(),
-    )
-    inserted_job_script_id = await database.execute(
-        query=job_scripts_table.insert(),
-        values=fill_job_script_data(application_id=inserted_application_id),
-    )
-
-    count = await database.fetch_all("SELECT COUNT(*) FROM job_scripts")
-    assert count[0][0] == 1
-
-    await database.execute(
-        query=job_submissions_table.insert(),
-        values=fill_job_submission_data(job_script_id=inserted_job_script_id),
-    )
-    count = await database.fetch_all("SELECT COUNT(*) FROM job_submissions")
-    assert count[0][0] == 1
-    count = await database.fetch_all(
-        "SELECT COUNT(*) FROM job_submissions where job_script_id=:inserted_id",
-        values=dict(inserted_id=inserted_job_script_id),
+    inserted_application_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(),
+    )
+    assert await fetch_count(synth_session, applications_table) == 1
+
+    inserted_job_script_id = await insert_data(
+        synth_session,
+        job_scripts_table,
+        fill_job_script_data(application_id=inserted_application_id),
+    )
+    assert await fetch_count(synth_session, job_scripts_table) == 1
+
+    await insert_data(
+        synth_session,
+        job_submissions_table,
+        fill_job_submission_data(job_script_id=inserted_job_script_id),
+    )
+    assert (
+        await fetch_count(
+            synth_session,
+            job_submissions_table,
+            job_submissions_table.c.job_script_id == inserted_job_script_id,
+        )
+        == 1
     )
-    assert count[0][0] == 1
 
     inject_security_header("owner1@org.com", Permissions.JOB_SCRIPTS_EDIT)
     with mock.patch("jobbergate_api.apps.job_scripts.job_script_files.JobScriptFiles.delete_from_s3"):
         response = await client.delete(f"/jobbergate/job-scripts/{inserted_job_script_id}")
         assert response.status_code == status.HTTP_204_NO_CONTENT
 
-    count = await database.fetch_all("SELECT COUNT(*) FROM job_scripts")
-    assert count[0][0] == 0
+    assert await fetch_count(synth_session, job_scripts_table) == 0
 
-    count = await database.fetch_all(
-        "SELECT COUNT(*) FROM job_submissions where job_script_id=:inserted_id",
-        values=dict(inserted_id=inserted_job_script_id),
+    assert await fetch_count(synth_session, job_submissions_table) == 1
+    assert (
+        await fetch_count(
+            synth_session,
+            job_submissions_table,
+            job_submissions_table.c.job_script_id == inserted_job_script_id,
+        )
+        == 0
     )
-    assert count[0][0] == 0
```

### Comparing `jobbergate_api-3.5.0a7/jobbergate_api/tests/apps/job_submissions/test_properties_parser.py` & `jobbergate_api-3.6.0/jobbergate_api/tests/apps/job_submissions/test_properties_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -450,28 +450,28 @@
         Base case, not SBATCH parameters on the job script and no extra parameters.
         """
         job_script_id = 1
         desired_job_properties = JobProperties()
 
         with mock_job_script_files("almost-empty-file") as mocked:
             actual_job_properties = get_job_properties_from_job_script(job_script_id)
-            mocked.assert_called_once_with(job_script_id)
+            mocked.assert_called_once_with(job_script_id, override_bucket_name=None)
 
         assert actual_job_properties == desired_job_properties
 
     def test_properties_only_from_file(self, mock_job_script_files):
         """
         Job properties are obtained only from the job script.
         """
         job_script_id = 1
         desired_job_properties = JobProperties(exclusive="exclusive", name="test-test")
 
         with mock_job_script_files("#SBATCH --exclusive\n#SBATCH -J test-test") as mocked:
             actual_job_properties = get_job_properties_from_job_script(job_script_id)
-            mocked.assert_called_once_with(job_script_id)
+            mocked.assert_called_once_with(job_script_id, override_bucket_name=None)
 
         assert actual_job_properties == desired_job_properties
 
     def test_properties_only_from_arguments(self, mock_job_script_files):
         """
         Job properties are obtained only from the extra arguments.
         """
@@ -481,15 +481,15 @@
         desired_job_properties = JobProperties.parse_obj(job_properties)
 
         with mock_job_script_files("almost-empty-file") as mocked:
             actual_job_properties = get_job_properties_from_job_script(
                 job_script_id,
                 **job_properties,
             )
-            mocked.assert_called_once_with(job_script_id)
+            mocked.assert_called_once_with(job_script_id, override_bucket_name=None)
 
         assert actual_job_properties == desired_job_properties
 
     def test_properties_priority_when_both_are_provided(self, mock_job_script_files):
         """
         Job properties are obtained from the job script and from the extra arguments.
 
@@ -501,28 +501,28 @@
         desired_job_properties = JobProperties.parse_obj(job_properties)
 
         with mock_job_script_files("#SBATCH --exclusive\n#SBATCH -J test-test") as mocked:
             actual_job_properties = get_job_properties_from_job_script(
                 job_script_id,
                 **job_properties,
             )
-            mocked.assert_called_once_with(job_script_id)
+            mocked.assert_called_once_with(job_script_id, override_bucket_name=None)
 
         assert actual_job_properties == desired_job_properties
 
     def test_properties_fails_with_unknown_field(self, mock_job_script_files):
         """
         The function fails when the extra arguments contain unknown fields.
         """
         job_script_id = 1
 
         with mock_job_script_files("almost-empty-file") as mocked:
             with pytest.raises(ValidationError, match="1 validation error for JobProperties"):
                 get_job_properties_from_job_script(job_script_id, foo="bar")
-            mocked.assert_called_once_with(job_script_id)
+            mocked.assert_called_once_with(job_script_id, override_bucket_name=None)
 
 
 class TestBidictMapping:
     """
     Integration test with the requirement bidict (used for two-way mapping).
     """
```

### Comparing `jobbergate_api-3.5.0a7/jobbergate_api/tests/apps/job_submissions/test_routers.py` & `jobbergate_api-3.6.0/jobbergate_api/tests/apps/job_submissions/test_routers.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,23 +10,20 @@
 from jobbergate_api.apps.applications.models import applications_table
 from jobbergate_api.apps.job_scripts.job_script_files import JobScriptFiles
 from jobbergate_api.apps.job_scripts.models import job_scripts_table
 from jobbergate_api.apps.job_submissions.constants import JobSubmissionStatus
 from jobbergate_api.apps.job_submissions.models import job_submissions_table
 from jobbergate_api.apps.job_submissions.schemas import JobProperties, JobSubmissionResponse
 from jobbergate_api.apps.permissions import Permissions
-from jobbergate_api.storage import database
-
-# Force the async event loop at the app to begin.
-# Since this is a time consuming fixture, it is just used where strict necessary.
-pytestmark = pytest.mark.usefixtures("startup_event_force")
+from jobbergate_api.storage import fetch_all, fetch_count, fetch_instance, insert_data
 
 
 @pytest.mark.asyncio
 async def test_create_job_submission__with_client_id_in_token(
+    synth_session,
     fill_application_data,
     fill_job_script_data,
     fill_job_submission_data,
     job_script_data,
     client,
     inject_security_header,
     time_frame,
@@ -35,22 +32,29 @@
     Test POST /job-submissions/ correctly creates a job_submission.
 
     This test proves that a job_submission is successfully created via a POST request to the /job-submissions/
     endpoint. We show this by asserting that the job_submission is created in the database after the post
     request is made, the correct status code (201) is returned. We also show that the ``client_id``
     is pulled from the token and the created job_submission is connected to that client id.
     """
-    inserted_application_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(),
-    )
-    inserted_job_script_id = await database.execute(
-        query=job_scripts_table.insert(),
-        values=fill_job_script_data(application_id=inserted_application_id),
+    inserted_application_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(
+            application_owner_email="owner1@org.com",
+        ),
+    )
+    assert await fetch_count(synth_session, applications_table) == 1
+
+    inserted_job_script_id = await insert_data(
+        synth_session,
+        job_scripts_table,
+        fill_job_script_data(application_id=inserted_application_id),
     )
+    assert await fetch_count(synth_session, job_scripts_table) == 1
 
     inject_security_header(
         "owner1@org.com",
         Permissions.JOB_SUBMISSIONS_EDIT,
         client_id="dummy-cluster-client",
     )
     create_data = fill_job_submission_data(
@@ -65,57 +69,46 @@
 
     with mock.patch(
         "jobbergate_api.apps.job_submissions.routers.get_job_properties_from_job_script"
     ) as mocked:
         mocked.return_value = JobProperties.parse_obj(create_data["execution_parameters"])
         with time_frame() as window:
             response = await client.post("/jobbergate/job-submissions/", json=create_data)
+
+        assert response.status_code == status.HTTP_201_CREATED
         mocked.assert_called_once_with(
             inserted_job_script_id,
+            None,
             **create_data["execution_parameters"],
         )
 
-    assert response.status_code == status.HTTP_201_CREATED
-
-    count = await database.fetch_all("SELECT COUNT(*) FROM job_submissions")
-    assert count[0][0] == 1
-
-    id_rows = await database.fetch_all("SELECT id FROM job_submissions")
-    assert len(id_rows) == 1
+    rows = await fetch_all(synth_session, job_submissions_table, JobSubmissionResponse)
+    assert len(rows) == 1
 
     job_submission = JobSubmissionResponse(**response.json())
 
-    # Check that the response correspond to the entry in the database
-    job_submission_raw_data = await database.fetch_one(
-        query=job_submissions_table.select().where(job_submissions_table.c.id == id_rows[0][0])
-    )
-    assert job_submission_raw_data is not None
-    assert job_submission == JobSubmissionResponse(
-        **{**job_submission_raw_data, **job_script_data}
-    )  # type: ignore
-
-    # Check that each field is correctly set
-    assert job_submission.id == job_submission_raw_data.get("id")
+    assert job_submission.id == rows[0].id
     assert job_submission.job_submission_name == "sub1"
     assert job_submission.job_submission_owner_email == "owner1@org.com"
-    assert job_submission.job_submission_description is None
+    assert job_submission.job_submission_description == ""
     assert job_submission.job_script_id == inserted_job_script_id
     assert job_submission.execution_directory is None
     assert job_submission.client_id == "dummy-cluster-client"
     assert job_submission.status == JobSubmissionStatus.CREATED
     assert job_submission.created_at in window
     assert job_submission.updated_at in window
 
     assert job_submission.execution_parameters is not None
     assert job_submission.execution_parameters.name == "job-submission-name"
     assert job_submission.execution_parameters.comment == "I am a comment"
 
 
 @pytest.mark.asyncio
 async def test_create_job_submission__without_execution_parameters(
+    synth_session,
     fill_application_data,
     fill_job_script_data,
     fill_job_submission_data,
     job_script_data,
     client,
     inject_security_header,
     time_frame,
@@ -127,22 +120,29 @@
     endpoint. We show this by asserting that the job_submission is created in the database after the post
     request is made, the correct status code (201) is returned. We also show that the ``client_id``
     is pulled from the token and the created job_submission is connected to that client id.
 
     This test is the same as the previous one, but it does not include the ``execution_parameters``
     in the payload, since they are optional.
     """
-    inserted_application_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(),
-    )
-    inserted_job_script_id = await database.execute(
-        query=job_scripts_table.insert(),
-        values=fill_job_script_data(application_id=inserted_application_id),
+    inserted_application_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(
+            application_owner_email="owner1@org.com",
+        ),
+    )
+    assert await fetch_count(synth_session, applications_table) == 1
+
+    inserted_job_script_id = await insert_data(
+        synth_session,
+        job_scripts_table,
+        fill_job_script_data(application_id=inserted_application_id),
     )
+    assert await fetch_count(synth_session, job_scripts_table) == 1
 
     dummy_client_id = "dummy-cluster-client"
     inject_security_header(
         "owner1@org.com",
         Permissions.JOB_SUBMISSIONS_EDIT,
         client_id=dummy_client_id,
     )
@@ -161,40 +161,27 @@
 
     with mock.patch(
         "jobbergate_api.apps.job_submissions.routers.get_job_properties_from_job_script"
     ) as mocked:
         mocked.return_value = JobProperties()
         with time_frame() as window:
             response = await client.post("/jobbergate/job-submissions/", json=create_data)
-        mocked.assert_called_once_with(inserted_job_script_id)
+        mocked.assert_called_once_with(inserted_job_script_id, None)
 
     assert response.status_code == status.HTTP_201_CREATED
 
-    count = await database.fetch_all("SELECT COUNT(*) FROM job_submissions")
-    assert count[0][0] == 1
-
-    id_rows = await database.fetch_all("SELECT id FROM job_submissions")
-    assert len(id_rows) == 1
-
+    rows = await fetch_all(synth_session, job_submissions_table, JobSubmissionResponse)
+    assert len(rows) == 1
     job_submission = JobSubmissionResponse(**response.json())
 
-    # Check that the response correspond to the entry in the database
-    job_submission_raw_data = await database.fetch_one(
-        query=job_submissions_table.select().where(job_submissions_table.c.id == id_rows[0][0])
-    )
-    assert job_submission_raw_data is not None
-    assert job_submission == JobSubmissionResponse(
-        **{**job_submission_raw_data, **job_script_data}
-    )  # type: ignore
-
     # Check that each field is correctly set
-    assert job_submission.id == job_submission_raw_data.get("id")
+    assert job_submission.id == rows[0].id
     assert job_submission.job_submission_name == create_data.get("job_submission_name")
     assert job_submission.job_submission_owner_email == create_data.get("job_submission_owner_email")
-    assert job_submission.job_submission_description == create_data.get("job_submission_description")
+    assert job_submission.job_submission_description == create_data.get("job_submission_description", "")
     assert job_submission.job_script_id == create_data.get("job_script_id")
     assert job_submission.execution_directory == create_data.get("execution_directory")
 
     # client_id was not on the payload, it should be set by other mechanisms
     assert create_data.get("client_id") is None
     assert job_submission.client_id == dummy_client_id
 
@@ -203,14 +190,15 @@
     assert job_submission.updated_at in window
 
     assert job_submission.execution_parameters == JobProperties().dict()
 
 
 @pytest.mark.asyncio
 async def test_create_job_submission__with_client_id_in_request_body(
+    synth_session,
     fill_application_data,
     fill_job_script_data,
     fill_job_submission_data,
     job_script_data,
     client,
     inject_security_header,
     time_frame,
@@ -219,22 +207,29 @@
     Test POST /job-submissions/ correctly creates a job_submission.
 
     This test proves that a job_submission is successfully created via a POST request to the /job-submissions/
     endpoint. We show this by asserting that the job_submission is created in the database after the post
     request is made, the correct status code (201) is returned. We also show that the ``client_id``
     in the request body overrides the client id in the token.
     """
-    inserted_application_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(),
-    )
-    inserted_job_script_id = await database.execute(
-        query=job_scripts_table.insert(),
-        values=fill_job_script_data(application_id=inserted_application_id),
+    inserted_application_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(
+            application_owner_email="owner1@org.com",
+        ),
+    )
+    assert await fetch_count(synth_session, applications_table) == 1
+
+    inserted_job_script_id = await insert_data(
+        synth_session,
+        job_scripts_table,
+        fill_job_script_data(application_id=inserted_application_id),
     )
+    assert await fetch_count(synth_session, job_scripts_table) == 1
 
     inject_security_header(
         "owner1@org.com",
         Permissions.JOB_SUBMISSIONS_EDIT,
         client_id="dummy-cluster-client",
     )
 
@@ -257,49 +252,37 @@
                     client_id="silly-cluster-client",
                     execution_parameters=execution_parameters,
                 ),
             )
 
     assert response.status_code == status.HTTP_201_CREATED
 
-    count = await database.fetch_all("SELECT COUNT(*) FROM job_submissions")
-    assert count[0][0] == 1
-
-    id_rows = await database.fetch_all("SELECT id FROM job_submissions")
-    assert len(id_rows) == 1
-
+    rows = await fetch_all(synth_session, job_submissions_table, JobSubmissionResponse)
+    assert len(rows) == 1
     job_submission = JobSubmissionResponse(**response.json())
 
-    # Check that the response correspond to the entry in the database
-    job_submission_raw_data = await database.fetch_one(
-        query=job_submissions_table.select().where(job_submissions_table.c.id == id_rows[0][0])
-    )
-    assert job_submission_raw_data is not None
-    assert job_submission == JobSubmissionResponse(
-        **{**job_submission_raw_data, **job_script_data}
-    )  # type: ignore
-
     # Check that each field is correctly set
-    assert job_submission.id == job_submission_raw_data.get("id")
+    assert job_submission.id == rows[0].id
     assert job_submission.job_submission_name == "sub1"
     assert job_submission.job_submission_owner_email == "owner1@org.com"
-    assert job_submission.job_submission_description is None
+    assert job_submission.job_submission_description == ""
     assert job_submission.job_script_id == inserted_job_script_id
     assert job_submission.client_id == "silly-cluster-client"
     assert job_submission.status == JobSubmissionStatus.CREATED
     assert job_submission.created_at in window
     assert job_submission.updated_at in window
 
     assert job_submission.execution_parameters is not None
     assert job_submission.execution_parameters.name == "job-submission-name"
     assert job_submission.execution_parameters.comment == "I am a comment"
 
 
 @pytest.mark.asyncio
 async def test_create_job_submission__with_execution_directory(
+    synth_session,
     fill_application_data,
     fill_job_script_data,
     fill_job_submission_data,
     job_script_data,
     client,
     inject_security_header,
     time_frame,
@@ -308,22 +291,29 @@
     Test POST /job-submissions/ correctly creates a job_submission with an execution directory.
 
     This test proves that a job_submission is successfully created via a POST request to the /job-submissions/
     endpoint with an attached execution directory. We show this by asserting that the job_submission is
     created in the database after the post request is made, the correct status code (201) is returned.
     We also show that the ``execution_directory`` is correctly set.
     """
-    inserted_application_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(),
-    )
-    inserted_job_script_id = await database.execute(
-        query=job_scripts_table.insert(),
-        values=fill_job_script_data(application_id=inserted_application_id),
+    inserted_application_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(
+            application_owner_email="owner1@org.com",
+        ),
+    )
+    assert await fetch_count(synth_session, applications_table) == 1
+
+    inserted_job_script_id = await insert_data(
+        synth_session,
+        job_scripts_table,
+        fill_job_script_data(application_id=inserted_application_id),
     )
+    assert await fetch_count(synth_session, job_scripts_table) == 1
 
     inject_security_header(
         "owner1@org.com",
         Permissions.JOB_SUBMISSIONS_EDIT,
         client_id="dummy-cluster-client",
     )
     create_data = fill_job_submission_data(
@@ -341,54 +331,43 @@
         "jobbergate_api.apps.job_submissions.routers.get_job_properties_from_job_script"
     ) as mocked:
         mocked.return_value = JobProperties.parse_obj(create_data["execution_parameters"])
         with time_frame() as window:
             response = await client.post("/jobbergate/job-submissions/", json=create_data)
         mocked.assert_called_once_with(
             inserted_job_script_id,
+            None,
             **create_data["execution_parameters"],
         )
 
     assert response.status_code == status.HTTP_201_CREATED
 
-    count = await database.fetch_all("SELECT COUNT(*) FROM job_submissions")
-    assert count[0][0] == 1
-
-    id_rows = await database.fetch_all("SELECT id FROM job_submissions")
-    assert len(id_rows) == 1
-
+    rows = await fetch_all(synth_session, job_submissions_table, JobSubmissionResponse)
+    assert len(rows) == 1
     job_submission = JobSubmissionResponse(**response.json())
 
-    # Check that the response correspond to the entry in the database
-    job_submission_raw_data = await database.fetch_one(
-        query=job_submissions_table.select().where(job_submissions_table.c.id == id_rows[0][0])
-    )
-    assert job_submission_raw_data is not None
-    assert job_submission == JobSubmissionResponse(
-        **{**job_submission_raw_data, **job_script_data}
-    )  # type: ignore
-
-    assert job_submission.id == job_submission_raw_data.get("id")
+    assert job_submission.id == rows[0].id
     assert job_submission.job_submission_name == "sub1"
     assert job_submission.job_submission_owner_email == "owner1@org.com"
-    assert job_submission.job_submission_description is None
+    assert job_submission.job_submission_description == ""
     assert job_submission.job_script_id == inserted_job_script_id
     assert job_submission.execution_directory == pathlib.Path("/some/fake/path")
     assert job_submission.client_id == "dummy-cluster-client"
     assert job_submission.status == JobSubmissionStatus.CREATED
     assert job_submission.created_at in window
     assert job_submission.updated_at in window
 
     assert job_submission.execution_parameters is not None
     assert job_submission.execution_parameters.name == "job-submission-name"
     assert job_submission.execution_parameters.comment == "I am a comment"
 
 
 @pytest.mark.asyncio
 async def test_create_job_submission_without_job_script(
+    synth_session,
     client,
     fill_job_submission_data,
     inject_security_header,
 ):
     """
     Test that is not possible to create a job_submission without a job_script.
 
@@ -397,77 +376,89 @@
     the job_submission still does not exists in the database, the correct status code (404) is returned.
     """
     inject_security_header("owner1@org.com", Permissions.JOB_SUBMISSIONS_EDIT)
     response = await client.post(
         "/jobbergate/job-submissions/", json=fill_job_submission_data(job_script_id=9999)
     )
     assert response.status_code == status.HTTP_404_NOT_FOUND
-
-    count = await database.fetch_all("SELECT COUNT(*) FROM job_submissions")
-    assert count[0][0] == 0
+    assert await fetch_count(synth_session, job_submissions_table) == 0
 
 
 @pytest.mark.asyncio
 async def test_create_job_submission_bad_permission(
+    synth_session,
     client,
     fill_application_data,
     fill_job_script_data,
     fill_job_submission_data,
     inject_security_header,
 ):
     """
     Test that is not possible to create a job_submission without the permission.
 
     This test proves that is not possible to create a job_submission using a user without the permission.
     We show this by trying to create a job_submission with a user without permission, then assert that
     the job_submission still does not exists in the database and the correct status code (403) is returned.
     """
-    inserted_application_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(),
-    )
-    inserted_job_script_id = await database.execute(
-        query=job_scripts_table.insert(),
-        values=fill_job_script_data(application_id=inserted_application_id),
+    inserted_application_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(
+            application_owner_email="owner1@org.com",
+        ),
+    )
+    assert await fetch_count(synth_session, applications_table) == 1
+
+    inserted_job_script_id = await insert_data(
+        synth_session,
+        job_scripts_table,
+        fill_job_script_data(application_id=inserted_application_id),
     )
+    assert await fetch_count(synth_session, job_scripts_table) == 1
 
     inject_security_header("owner1@org.com", "INVALID_PERMISSION")
     response = await client.post(
         "/jobbergate/job-submissions/",
         json=fill_job_submission_data(job_script_id=inserted_job_script_id),
     )
     assert response.status_code == status.HTTP_403_FORBIDDEN
-
-    count = await database.fetch_all("SELECT COUNT(*) FROM job_submissions")
-    assert count[0][0] == 0
+    assert await fetch_count(synth_session, job_submissions_table) == 0
 
 
 @pytest.mark.asyncio
 async def test_create_job_submission_without_client_id(
+    synth_session,
     fill_application_data,
     fill_job_script_data,
     fill_job_submission_data,
     client,
     inject_security_header,
 ):
     """
     Test that it is not possible to create a job_submission without a ``client_id``.
 
     This test proves that it is not possible to create a job_submission without including a
     ``client_id`` in either the request body or embedded in the access token. If none are supplied,
     we assert that a 400 response is returned.k
     """
-    inserted_application_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(),
-    )
-    inserted_job_script_id = await database.execute(
-        query=job_scripts_table.insert(),
-        values=fill_job_script_data(application_id=inserted_application_id),
+    inserted_application_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(
+            application_owner_email="owner1@org.com",
+        ),
+    )
+    assert await fetch_count(synth_session, applications_table) == 1
+
+    inserted_job_script_id = await insert_data(
+        synth_session,
+        job_scripts_table,
+        fill_job_script_data(application_id=inserted_application_id),
     )
+    assert await fetch_count(synth_session, job_scripts_table) == 1
 
     inject_security_header(
         "owner1@org.com",
         Permissions.JOB_SUBMISSIONS_EDIT,
     )
     create_data = fill_job_submission_data(
         job_script_id=inserted_job_script_id,
@@ -477,54 +468,60 @@
     create_data.pop("client_id", None)
     response = await client.post(
         "/jobbergate/job-submissions/",
         json=create_data,
     )
 
     assert response.status_code == status.HTTP_400_BAD_REQUEST
-
-    count = await database.fetch_all("SELECT COUNT(*) FROM job_submissions")
-    assert count[0][0] == 0
+    assert await fetch_count(synth_session, job_submissions_table) == 0
 
 
 @pytest.mark.asyncio
 async def test_get_job_submission_by_id(
+    synth_session,
     client,
     fill_application_data,
     fill_job_script_data,
     fill_job_submission_data,
     inject_security_header,
 ):
     """
     Test GET /job-submissions/<id>.
 
     This test proves that GET /job-submissions/<id> returns the correct job-submission, owned by
     the user making the request. We show this by asserting that the job_submission data
     returned in the response is equal to the job_submission data that exists in the database
     for the given job_submission id.
     """
-    inserted_application_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(),
-    )
-    inserted_job_script_id = await database.execute(
-        query=job_scripts_table.insert(),
-        values=fill_job_script_data(application_id=inserted_application_id),
-    )
-    inserted_job_submission_id = await database.execute(
-        query=job_submissions_table.insert(),
-        values=fill_job_submission_data(
+    inserted_application_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(
+            application_owner_email="owner1@org.com",
+        ),
+    )
+    assert await fetch_count(synth_session, applications_table) == 1
+
+    inserted_job_script_id = await insert_data(
+        synth_session,
+        job_scripts_table,
+        fill_job_script_data(application_id=inserted_application_id),
+    )
+    assert await fetch_count(synth_session, job_scripts_table) == 1
+
+    inserted_job_submission_id = await insert_data(
+        synth_session,
+        job_submissions_table,
+        fill_job_submission_data(
             job_script_id=inserted_job_script_id,
             job_submission_name="sub1",
             job_submission_owner_email="owner1@org.com",
         ),
     )
-
-    count = await database.fetch_all("SELECT COUNT(*) FROM job_submissions")
-    assert count[0][0] == 1
+    assert await fetch_count(synth_session, job_submissions_table) == 1
 
     inject_security_header("owner1@org.com", Permissions.JOB_SUBMISSIONS_VIEW)
     response = await client.get(f"/jobbergate/job-submissions/{inserted_job_submission_id}")
     assert response.status_code == status.HTTP_200_OK
 
     data = response.json()
     assert data["id"] == inserted_job_submission_id
@@ -534,41 +531,53 @@
 
     assert data["execution_parameters"]["name"] == "job-submission-name"
     assert data["execution_parameters"]["comment"] == "I am a comment"
 
 
 @pytest.mark.asyncio
 async def test_get_job_submission_by_id_bad_permission(
+    synth_session,
     client,
     fill_application_data,
     fill_job_script_data,
     fill_job_submission_data,
     inject_security_header,
 ):
     """
     Test the correct response code is returned when the user don't have the proper permission.
 
     This test proves that GET /job-submissions/<id> returns the correct response code when the user don't
     have proper permission. We show this by asserting that the status code returned is 403.
     """
-    inserted_application_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(),
-    )
-    inserted_job_script_id = await database.execute(
-        query=job_scripts_table.insert(),
-        values=fill_job_script_data(application_id=inserted_application_id),
-    )
-    inserted_job_submission_id = await database.execute(
-        query=job_submissions_table.insert(),
-        values=fill_job_submission_data(
+    inserted_application_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(
+            application_owner_email="owner1@org.com",
+        ),
+    )
+    assert await fetch_count(synth_session, applications_table) == 1
+
+    inserted_job_script_id = await insert_data(
+        synth_session,
+        job_scripts_table,
+        fill_job_script_data(application_id=inserted_application_id),
+    )
+    assert await fetch_count(synth_session, job_scripts_table) == 1
+
+    inserted_job_submission_id = await insert_data(
+        synth_session,
+        job_submissions_table,
+        fill_job_submission_data(
             job_script_id=inserted_job_script_id,
+            job_submission_name="sub1",
             job_submission_owner_email="owner1@org.com",
         ),
     )
+    assert await fetch_count(synth_session, job_submissions_table) == 1
 
     inject_security_header("owner1@org.com", "INVALID_PERMISSION")
     response = await client.get(f"/jobbergate/job-submissions/{inserted_job_submission_id}")
     assert response.status_code == status.HTTP_403_FORBIDDEN
 
 
 @pytest.mark.asyncio
@@ -583,38 +592,47 @@
     inject_security_header("owner1@org.com", Permissions.JOB_SUBMISSIONS_VIEW)
     response = await client.get("/jobbergate/job-submissions/9999")
     assert response.status_code == status.HTTP_404_NOT_FOUND
 
 
 @pytest.mark.asyncio
 async def test_get_job_submissions__no_param(
+    synth_session,
     client,
     fill_application_data,
     fill_job_script_data,
     fill_all_job_submission_data,
     inject_security_header,
 ):
     """
     Test GET /job-submissions/ returns only job_submissions owned by the user making the request.
 
     This test proves that GET /job-submissions/ returns the correct job_submissions for the user making
     the request. We show this by asserting that the job_submissions returned in the response are
     only job_submissions owned by the user making the request.
     """
-    inserted_application_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(),
-    )
-    inserted_job_script_id = await database.execute(
-        query=job_scripts_table.insert(),
-        values=fill_job_script_data(application_id=inserted_application_id),
-    )
-    await database.execute_many(
-        query=job_submissions_table.insert(),
-        values=fill_all_job_submission_data(
+    inserted_application_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(
+            application_owner_email="owner1@org.com",
+        ),
+    )
+    assert await fetch_count(synth_session, applications_table) == 1
+
+    inserted_job_script_id = await insert_data(
+        synth_session,
+        job_scripts_table,
+        fill_job_script_data(application_id=inserted_application_id),
+    )
+    assert await fetch_count(synth_session, job_scripts_table) == 1
+
+    await synth_session.execute(
+        job_submissions_table.insert(),
+        fill_all_job_submission_data(
             dict(
                 job_script_id=inserted_job_script_id,
                 job_submission_name="sub1",
                 job_submission_owner_email="owner1@org.com",
                 execution_parameters={
                     "name": "job-submission-name-1",
                     "comment": "I am a comment",
@@ -636,17 +654,15 @@
                 execution_parameters={
                     "name": "job-submission-name-3",
                     "comment": "I am a comment",
                 },
             ),
         ),
     )
-
-    count = await database.fetch_all("SELECT COUNT(*) FROM job_submissions")
-    assert count[0][0] == 3
+    assert await fetch_count(synth_session, job_submissions_table) == 3
 
     inject_security_header("owner1@org.com", Permissions.JOB_SUBMISSIONS_VIEW)
     response = await client.get("/jobbergate/job-submissions/")
     assert response.status_code == status.HTTP_200_OK
 
     data = response.json()
     results = data.get("results")
@@ -659,77 +675,94 @@
         start=None,
         limit=None,
     )
 
 
 @pytest.mark.asyncio
 async def test_get_job_submissions__bad_permission(
+    synth_session,
     client,
     fill_application_data,
     fill_job_script_data,
     fill_job_submission_data,
     inject_security_header,
 ):
     """
     Test GET /job-submissions/ returns 403 for a user without permission.
 
     This test proves that GET /job-submissions/ returns the correct status code (403) for a user without
     permission. We show this by asserting that the status code of the response is 403.
     """
-    inserted_application_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(),
-    )
-    inserted_job_script_id = await database.execute(
-        query=job_scripts_table.insert(),
-        values=fill_job_script_data(application_id=inserted_application_id),
-    )
-    await database.execute(
-        query=job_submissions_table.insert(),
-        values=fill_job_submission_data(
+    inserted_application_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(
+            application_owner_email="owner1@org.com",
+        ),
+    )
+    assert await fetch_count(synth_session, applications_table) == 1
+
+    inserted_job_script_id = await insert_data(
+        synth_session,
+        job_scripts_table,
+        fill_job_script_data(application_id=inserted_application_id),
+    )
+    assert await fetch_count(synth_session, job_scripts_table) == 1
+
+    await insert_data(
+        synth_session,
+        job_submissions_table,
+        fill_job_submission_data(
             job_script_id=inserted_job_script_id,
             job_submission_owner_email="owner1@org.com",
         ),
     )
-
-    count = await database.fetch_all("SELECT COUNT(*) FROM job_submissions")
-    assert count[0][0] == 1
+    assert await fetch_count(synth_session, job_submissions_table) == 1
 
     inject_security_header("owner1@org.com", "INVALID_PERMISSION")
     response = await client.get("/jobbergate/job-submissions/")
     assert response.status_code == status.HTTP_403_FORBIDDEN
 
 
 @pytest.mark.asyncio
 async def test_get_job_submissions__with_all_param(
+    synth_session,
     client,
     fill_application_data,
     fill_job_script_data,
     fill_all_job_submission_data,
     inject_security_header,
 ):
     """
     Test that listing job_submissions, when all=True, contains job_submissions owned by other users.
 
     This test proves that the user making the request can see job_submissions owned by other users.
     We show this by creating three job_submissions, one that are owned by the user making the request, and two
     owned by another user. Assert that the response to GET /job-submissions/?all=True includes all three
     job_submissions.
     """
-    inserted_application_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(),
-    )
-    inserted_job_script_id = await database.execute(
-        query=job_scripts_table.insert(),
-        values=fill_job_script_data(application_id=inserted_application_id),
-    )
-    await database.execute_many(
-        query=job_submissions_table.insert(),
-        values=fill_all_job_submission_data(
+    inserted_application_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(
+            application_owner_email="owner1@org.com",
+        ),
+    )
+    assert await fetch_count(synth_session, applications_table) == 1
+
+    inserted_job_script_id = await insert_data(
+        synth_session,
+        job_scripts_table,
+        fill_job_script_data(application_id=inserted_application_id),
+    )
+    assert await fetch_count(synth_session, job_scripts_table) == 1
+
+    await synth_session.execute(
+        job_submissions_table.insert(),
+        fill_all_job_submission_data(
             dict(
                 job_script_id=inserted_job_script_id,
                 job_submission_name="sub1",
                 job_submission_owner_email="owner1@org.com",
                 execution_parameters={
                     "name": "job-submission-name-1",
                     "comment": "I am a comment",
@@ -751,17 +784,15 @@
                 execution_parameters={
                     "name": "job-submission-name-3",
                     "comment": "I am a comment",
                 },
             ),
         ),
     )
-
-    count = await database.fetch_all("SELECT COUNT(*) FROM job_submissions")
-    assert count[0][0] == 3
+    assert await fetch_count(synth_session, job_submissions_table) == 3
 
     inject_security_header("owner1@org.com", Permissions.JOB_SUBMISSIONS_VIEW)
     response = await client.get("/jobbergate/job-submissions/?all=True")
     assert response.status_code == status.HTTP_200_OK
 
     data = response.json()
     results = data.get("results")
@@ -774,55 +805,55 @@
         start=None,
         limit=None,
     )
 
 
 @pytest.mark.asyncio
 async def test_get_job_submissions__from_job_script_id(
+    synth_session,
     client,
     fill_application_data,
     fill_job_script_data,
     fill_all_job_submission_data,
     inject_security_header,
 ):
     """
     Test listing job-submissions when from_job_script_id=<num> is present.
 
     Only the job-submissions produced from the job-script with id=<num> should be returned.
     """
-    inserted_application_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(),
-    )
-    inserted_job_script_id_1 = await database.execute(
-        query=job_scripts_table.insert(),
-        values=fill_job_script_data(application_id=inserted_application_id),
-    )
-    inserted_job_script_id_2 = await database.execute(
-        query=job_scripts_table.insert(),
-        values=fill_job_script_data(application_id=inserted_application_id),
-    )
-    inserted_job_script_id_3 = await database.execute(
-        query=job_scripts_table.insert(),
-        values=fill_job_script_data(application_id=inserted_application_id),
-    )
-    await database.execute_many(
-        query=job_submissions_table.insert(),
-        values=fill_all_job_submission_data(
-            {"job_script_id": inserted_job_script_id_1},
-            {"job_script_id": inserted_job_script_id_1},
-            {"job_script_id": inserted_job_script_id_2},
-            {"job_script_id": inserted_job_script_id_2},
-            {"job_script_id": inserted_job_script_id_3},
-            {"job_script_id": inserted_job_script_id_3},
+    inserted_application_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(
+            application_owner_email="owner1@org.com",
         ),
     )
+    assert await fetch_count(synth_session, applications_table) == 1
 
-    count = await database.fetch_all("SELECT COUNT(*) FROM job_submissions")
-    assert count[0][0] == 6
+    raw_results = await synth_session.execute(
+        job_scripts_table.insert().returning(job_scripts_table.c.id),
+        [fill_job_script_data(application_id=inserted_application_id)] * 3,
+    )
+    (inserted_job_script_id_1, inserted_job_script_id_2, inserted_job_script_id_3) = (
+        r.id for r in raw_results
+    )
+
+    await synth_session.execute(
+        job_submissions_table.insert(),
+        fill_all_job_submission_data(
+            dict(job_script_id=inserted_job_script_id_1),
+            dict(job_script_id=inserted_job_script_id_1),
+            dict(job_script_id=inserted_job_script_id_2),
+            dict(job_script_id=inserted_job_script_id_2),
+            dict(job_script_id=inserted_job_script_id_3),
+            dict(job_script_id=inserted_job_script_id_3),
+        ),
+    )
+    assert await fetch_count(synth_session, job_submissions_table) == 6
 
     inject_security_header("owner1@org.com", Permissions.JOB_SUBMISSIONS_VIEW)
 
     for job_script_id in [inserted_job_script_id_1, inserted_job_script_id_2, inserted_job_script_id_3]:
         response = await client.get(f"/jobbergate/job-submissions/?from_job_script_id={job_script_id}")
         assert response.status_code == status.HTTP_200_OK
 
@@ -830,37 +861,46 @@
         results = data.get("results")
 
         assert {d["job_script_id"] for d in results} == {job_script_id}
 
 
 @pytest.mark.asyncio
 async def test_get_job_submissions__with_status_param(
+    synth_session,
     client,
     fill_application_data,
     fill_job_script_data,
     fill_all_job_submission_data,
     inject_security_header,
 ):
     """
     Test that listing job_submissions, when status is set, contains job_submissions with matching status.
 
     This test proves that job_submissions are filtered by the status parameter. We do this by setting the
     status param and making sure that only job_submissions with that status are returned.
     """
-    inserted_application_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(),
-    )
-    inserted_job_script_id = await database.execute(
-        query=job_scripts_table.insert(),
-        values=fill_job_script_data(application_id=inserted_application_id),
-    )
-    await database.execute_many(
-        query=job_submissions_table.insert(),
-        values=fill_all_job_submission_data(
+    inserted_application_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(
+            application_owner_email="owner1@org.com",
+        ),
+    )
+    assert await fetch_count(synth_session, applications_table) == 1
+
+    inserted_job_script_id = await insert_data(
+        synth_session,
+        job_scripts_table,
+        fill_job_script_data(application_id=inserted_application_id),
+    )
+    assert await fetch_count(synth_session, job_scripts_table) == 1
+
+    await synth_session.execute(
+        job_submissions_table.insert(),
+        fill_all_job_submission_data(
             dict(
                 job_script_id=inserted_job_script_id,
                 job_submission_name="sub1",
                 job_submission_owner_email="owner1@org.com",
                 status=JobSubmissionStatus.CREATED,
             ),
             dict(
@@ -873,17 +913,15 @@
                 job_script_id=inserted_job_script_id,
                 job_submission_name="sub3",
                 job_submission_owner_email="owner1@org.com",
                 status=JobSubmissionStatus.COMPLETED,
             ),
         ),
     )
-
-    count = await database.fetch_all("SELECT COUNT(*) FROM job_submissions")
-    assert count[0][0] == 3
+    assert await fetch_count(synth_session, job_submissions_table) == 3
 
     inject_security_header("owner1@org.com", Permissions.JOB_SUBMISSIONS_VIEW)
     response = await client.get(f"/jobbergate/job-submissions/?submit_status={JobSubmissionStatus.CREATED}")
     assert response.status_code == status.HTTP_200_OK
 
     data = response.json()
     results = data.get("results")
@@ -896,59 +934,69 @@
         start=None,
         limit=None,
     )
 
 
 @pytest.mark.asyncio
 async def test_get_job_submissions__with_search_param(
+    synth_session,
     client,
     inject_security_header,
     fill_application_data,
     fill_job_script_data,
     fill_all_job_submission_data,
 ):
     """
     Test that listing job submissions, when search=<search terms>, returns matches.
 
     This test proves that the user making the request will be shown job submissions that match the search
     string.  We show this by creating job submissions and using various search queries to match against them.
 
     Assert that the response to GET /job_submissions?search=<search temrms> includes correct matches.
     """
-    inserted_application_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(),
-    )
-    inserted_job_script_id = await database.execute(
-        query=job_scripts_table.insert(),
-        values=fill_job_script_data(application_id=inserted_application_id),
-    )
-    await database.execute_many(
-        query=job_submissions_table.insert(),
-        values=fill_all_job_submission_data(
+    inserted_application_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(
+            application_owner_email="owner1@org.com",
+        ),
+    )
+    assert await fetch_count(synth_session, applications_table) == 1
+
+    inserted_job_script_id = await insert_data(
+        synth_session,
+        job_scripts_table,
+        fill_job_script_data(application_id=inserted_application_id),
+    )
+    assert await fetch_count(synth_session, job_scripts_table) == 1
+
+    await synth_session.execute(
+        job_submissions_table.insert(),
+        fill_all_job_submission_data(
             dict(
                 job_script_id=inserted_job_script_id,
                 job_submission_name="test name one",
                 job_submission_owner_email="one@org.com",
+                job_submission_description=None,
             ),
             dict(
                 job_script_id=inserted_job_script_id,
                 job_submission_name="test name two",
                 job_submission_owner_email="two@org.com",
+                job_submission_description=None,
             ),
             dict(
                 job_script_id=inserted_job_script_id,
                 job_submission_name="test name twenty-two",
                 job_submission_owner_email="twenty-two@org.com",
                 job_submission_description="a long description of this job_script",
             ),
         ),
     )
-    count = await database.fetch_all("SELECT COUNT(*) FROM job_submissions")
-    assert count[0][0] == 3
+    assert await fetch_count(synth_session, job_submissions_table) == 3
 
     inject_security_header("admin@org.com", Permissions.JOB_SUBMISSIONS_VIEW)
 
     response = await client.get("/jobbergate/job-submissions?all=true&search=one")
     assert response.status_code == status.HTTP_200_OK
     data = response.json()
     results = data.get("results")
@@ -975,14 +1023,15 @@
         "test name two",
         "test name twenty-two",
     ]
 
 
 @pytest.mark.asyncio
 async def test_get_job_submissions_with_sort_params(
+    synth_session,
     client,
     fill_application_data,
     fill_job_script_data,
     fill_all_job_submission_data,
     inject_security_header,
 ):
     """
@@ -991,25 +1040,33 @@
     This test proves that the user making the request will be shown job_submissions sorted in the correct
     order according to the ``sort_field`` and ``sort_ascending`` parameters.
     We show this by creating job_submissions and using various sort parameters to order them.
 
     Assert that the response to GET /job_submissions?sort_field=<field>&sort_ascending=<bool> includes
     correctly sorted job_submissions.
     """
-    inserted_application_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(),
-    )
-    inserted_job_script_id = await database.execute(
-        query=job_scripts_table.insert(),
-        values=fill_job_script_data(application_id=inserted_application_id),
-    )
-    await database.execute_many(
-        query=job_submissions_table.insert(),
-        values=fill_all_job_submission_data(
+    inserted_application_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(
+            application_owner_email="owner1@org.com",
+        ),
+    )
+    assert await fetch_count(synth_session, applications_table) == 1
+
+    inserted_job_script_id = await insert_data(
+        synth_session,
+        job_scripts_table,
+        fill_job_script_data(application_id=inserted_application_id),
+    )
+    assert await fetch_count(synth_session, job_scripts_table) == 1
+
+    await synth_session.execute(
+        job_submissions_table.insert(),
+        fill_all_job_submission_data(
             dict(
                 job_script_id=inserted_job_script_id,
                 job_submission_name="Z",
                 job_submission_owner_email="admin@org.com",
                 status=JobSubmissionStatus.REJECTED,
             ),
             dict(
@@ -1022,16 +1079,15 @@
                 job_script_id=inserted_job_script_id,
                 job_submission_name="X",
                 job_submission_owner_email="admin@org.com",
                 status=JobSubmissionStatus.FAILED,
             ),
         ),
     )
-    count = await database.fetch_all("SELECT COUNT(*) FROM job_submissions")
-    assert count[0][0] == 3
+    assert await fetch_count(synth_session, job_submissions_table) == 3
 
     inject_security_header("admin@org.com", Permissions.JOB_SUBMISSIONS_VIEW)
 
     response = await client.get("/jobbergate/job-submissions?sort_field=id")
     assert response.status_code == status.HTTP_200_OK
     data = response.json()
     results = data.get("results")
@@ -1058,50 +1114,57 @@
     response = await client.get("/jobbergate/job-submissions?all=true&sort_field=job_submission_description")
     assert response.status_code == status.HTTP_400_BAD_REQUEST
     assert "Invalid sorting column requested" in response.text
 
 
 @pytest.mark.asyncio
 async def test_list_job_submission_pagination(
+    synth_session,
     client,
     fill_application_data,
     fill_job_script_data,
     fill_all_job_submission_data,
     inject_security_header,
 ):
     """
     Test that listing job_submissions works with pagination.
 
     this test proves that the user making the request can see job_submisions paginated.
     We show this by creating three job_submissions and assert that the response is correctly paginated.
     """
-    inserted_application_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(application_owner_email="owner1@org.com"),
-    )
-    inserted_job_script_id = await database.execute(
-        query=job_scripts_table.insert(),
-        values=fill_job_script_data(application_id=inserted_application_id),
-    )
-    await database.execute_many(
-        query=job_submissions_table.insert(),
-        values=fill_all_job_submission_data(
+    inserted_application_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(
+            application_owner_email="owner1@org.com",
+        ),
+    )
+    assert await fetch_count(synth_session, applications_table) == 1
+
+    inserted_job_script_id = await insert_data(
+        synth_session,
+        job_scripts_table,
+        fill_job_script_data(application_id=inserted_application_id),
+    )
+    assert await fetch_count(synth_session, job_scripts_table) == 1
+
+    await synth_session.execute(
+        job_submissions_table.insert(),
+        fill_all_job_submission_data(
             *[
                 dict(
                     job_submission_name=f"sub{i}",
                     job_script_id=inserted_job_script_id,
                     job_submission_owner_email="owner1@org.com",
                 )
                 for i in range(1, 6)
             ]
         ),
     )
-
-    count = await database.fetch_all("SELECT COUNT(*) FROM job_submissions")
-    assert count[0][0] == 5
+    assert await fetch_count(synth_session, job_submissions_table) == 5
 
     inject_security_header("owner1@org.com", Permissions.JOB_SUBMISSIONS_VIEW)
     response = await client.get("/jobbergate/job-submissions/?start=0&limit=1")
     assert response.status_code == status.HTTP_200_OK
 
     data = response.json()
     results = data.get("results")
@@ -1140,38 +1203,47 @@
 
     pagination = data.get("pagination")
     assert pagination == dict(total=5, start=2, limit=2)
 
 
 @pytest.mark.asyncio
 async def test_get_job_submissions_with_slurm_job_ids_param(
+    synth_session,
     client,
     fill_application_data,
     fill_job_script_data,
     fill_all_job_submission_data,
     inject_security_header,
 ):
     """
     Test GET /job-submissions/ returns only job_submissions that have one of the supplied slurm job ids.
 
     This test proves that GET /job-submissions returns the correct job_submissions with matching slurm_job_id.
     We show this by asserting that the job_submissions returned in the response have one of the supplied
     slurm job ids.
     """
-    inserted_application_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(),
-    )
-    inserted_job_script_id = await database.execute(
-        query=job_scripts_table.insert(),
-        values=fill_job_script_data(application_id=inserted_application_id),
-    )
-    await database.execute_many(
-        query=job_submissions_table.insert(),
-        values=fill_all_job_submission_data(
+    inserted_application_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(
+            application_owner_email="owner1@org.com",
+        ),
+    )
+    assert await fetch_count(synth_session, applications_table) == 1
+
+    inserted_job_script_id = await insert_data(
+        synth_session,
+        job_scripts_table,
+        fill_job_script_data(application_id=inserted_application_id),
+    )
+    assert await fetch_count(synth_session, job_scripts_table) == 1
+
+    await synth_session.execute(
+        job_submissions_table.insert(),
+        fill_all_job_submission_data(
             dict(
                 job_submission_name="sub1",
                 job_script_id=inserted_job_script_id,
                 job_submission_owner_email="owner1@org.com",
                 slurm_job_id=101,
             ),
             dict(
@@ -1184,17 +1256,15 @@
                 job_submission_name="sub3",
                 job_script_id=inserted_job_script_id,
                 job_submission_owner_email="owner1@org.com",
                 slurm_job_id=103,
             ),
         ),
     )
-
-    count = await database.fetch_all("SELECT COUNT(*) FROM job_submissions")
-    assert count[0][0] == 3
+    assert await fetch_count(synth_session, job_submissions_table) == 3
 
     inject_security_header("owner1@org.com", Permissions.JOB_SUBMISSIONS_VIEW)
     response = await client.get("/jobbergate/job-submissions?slurm_job_ids=101,103")
     assert response.status_code == status.HTTP_200_OK
 
     data = response.json()
     results = data.get("results")
@@ -1207,37 +1277,46 @@
         start=None,
         limit=None,
     )
 
 
 @pytest.mark.asyncio
 async def test_get_job_submissions_applies_no_slurm_filter_if_slurm_job_ids_is_empty(
+    synth_session,
     client,
     inject_security_header,
     fill_application_data,
     fill_job_script_data,
     fill_all_job_submission_data,
 ):
     """
     Test GET /job-submissions/ skips filtering on slurm_job_id if the param is an empty string.
 
     This test proves that GET /job-submissions doesn't use the slurm_job_id filter if it is an empty string.
     We show this by asserting that passing an empty string as a parameter has no effect.
     """
-    inserted_application_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(),
-    )
-    inserted_job_script_id = await database.execute(
-        query=job_scripts_table.insert(),
-        values=fill_job_script_data(application_id=inserted_application_id),
-    )
-    await database.execute_many(
-        query=job_submissions_table.insert(),
-        values=fill_all_job_submission_data(
+    inserted_application_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(
+            application_owner_email="owner1@org.com",
+        ),
+    )
+    assert await fetch_count(synth_session, applications_table) == 1
+
+    inserted_job_script_id = await insert_data(
+        synth_session,
+        job_scripts_table,
+        fill_job_script_data(application_id=inserted_application_id),
+    )
+    assert await fetch_count(synth_session, job_scripts_table) == 1
+
+    await synth_session.execute(
+        job_submissions_table.insert(),
+        fill_all_job_submission_data(
             dict(
                 job_script_id=inserted_job_script_id,
                 job_submission_owner_email="owner1@org.com",
                 slurm_job_id=101,
             ),
             dict(
                 job_script_id=inserted_job_script_id,
@@ -1247,17 +1326,15 @@
             dict(
                 job_script_id=inserted_job_script_id,
                 job_submission_owner_email="owner1@org.com",
                 slurm_job_id=103,
             ),
         ),
     )
-
-    count = await database.fetch_all("SELECT COUNT(*) FROM job_submissions")
-    assert count[0][0] == 3
+    assert await fetch_count(synth_session, job_submissions_table) == 3
 
     inject_security_header("owner1@org.com", Permissions.JOB_SUBMISSIONS_VIEW)
 
     with_empty_param_response = await client.get("/jobbergate/job-submissions?slurm_job_ids=")
     assert with_empty_param_response.status_code == status.HTTP_200_OK
 
     without_param_response = await client.get("/jobbergate/job-submissions")
@@ -1286,43 +1363,54 @@
     assert response.status_code == status.HTTP_422_UNPROCESSABLE_ENTITY
     assert "Invalid slurm_job_ids" in response.text
 
 
 @pytest.mark.freeze_time
 @pytest.mark.asyncio
 async def test_update_job_submission__basic(
+    synth_session,
     client,
     fill_application_data,
     fill_job_script_data,
     fill_job_submission_data,
     inject_security_header,
     time_frame,
 ):
     """
     Test update job_submission via PUT.
 
     This test proves that the job_submission values are correctly updated following a PUT request to the
     /job-submissions/<id> endpoint. We show this by assert the response status code to 201, the response data
     corresponds to the updated data, and the data in the database is also updated.
     """
-    inserted_application_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(),
-    )
-    inserted_job_script_id = await database.execute(
-        query=job_scripts_table.insert(),
-        values=fill_job_script_data(application_id=inserted_application_id),
-    )
-    inserted_job_submission_id = await database.execute(
-        query=job_submissions_table.insert(),
-        values=fill_job_submission_data(
+    inserted_application_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(
+            application_owner_email="owner1@org.com",
+        ),
+    )
+    assert await fetch_count(synth_session, applications_table) == 1
+
+    inserted_job_script_id = await insert_data(
+        synth_session,
+        job_scripts_table,
+        fill_job_script_data(application_id=inserted_application_id),
+    )
+    assert await fetch_count(synth_session, job_scripts_table) == 1
+
+    inserted_job_submission_id = await insert_data(
+        synth_session,
+        job_submissions_table,
+        fill_job_submission_data(
             job_script_id=inserted_job_script_id,
             job_submission_owner_email="owner1@org.com",
         ),
     )
+    assert await fetch_count(synth_session, job_submissions_table) == 1
 
     inject_security_header("owner1@org.com", Permissions.JOB_SUBMISSIONS_EDIT)
     with time_frame() as window:
         response = await client.put(
             f"/jobbergate/job-submissions/{inserted_job_submission_id}",
             json=dict(job_submission_name="new name", job_submission_description="new description"),
         )
@@ -1330,75 +1418,87 @@
     assert response.status_code == status.HTTP_200_OK
     data = response.json()
 
     assert data["job_submission_name"] == "new name"
     assert data["job_submission_description"] == "new description"
     assert data["id"] == inserted_job_submission_id
 
-    query = job_submissions_table.select(job_submissions_table.c.id == inserted_job_submission_id)
-    job_submission_data = await database.fetch_one(query)
+    job_submission = await fetch_instance(
+        synth_session, inserted_job_submission_id, job_submissions_table, JobSubmissionResponse
+    )
 
-    assert job_submission_data is not None
-    assert job_submission_data["job_submission_name"] == "new name"
-    assert job_submission_data["job_submission_description"] == "new description"
-    assert job_submission_data["updated_at"] in window
+    assert job_submission.job_submission_name == "new name"
+    assert job_submission.job_submission_description == "new description"
+    assert job_submission.updated_at in window
 
 
 @pytest.mark.freeze_time
 @pytest.mark.asyncio
 async def test_update_job_submission__with_execution_dir(
+    synth_session,
     client,
     fill_application_data,
     fill_job_script_data,
     fill_job_submission_data,
     inject_security_header,
     time_frame,
 ):
     """
     Test update job_submission via PUT can set execution directory.
 
     This test proves that the job_submission values are correctly updated following a PUT request to the
     /job-submissions/<id> endpoint. We show this by assert the response status code to 201, the response data
     corresponds to the updated data, and the execution_directory is correctly updated.
     """
-    inserted_application_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(),
-    )
-    inserted_job_script_id = await database.execute(
-        query=job_scripts_table.insert(),
-        values=fill_job_script_data(application_id=inserted_application_id),
-    )
-    inserted_job_submission_id = await database.execute(
-        query=job_submissions_table.insert(),
-        values=fill_job_submission_data(
+    inserted_application_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(
+            application_owner_email="owner1@org.com",
+        ),
+    )
+    assert await fetch_count(synth_session, applications_table) == 1
+
+    inserted_job_script_id = await insert_data(
+        synth_session,
+        job_scripts_table,
+        fill_job_script_data(application_id=inserted_application_id),
+    )
+    assert await fetch_count(synth_session, job_scripts_table) == 1
+
+    inserted_job_submission_id = await insert_data(
+        synth_session,
+        job_submissions_table,
+        fill_job_submission_data(
             job_script_id=inserted_job_script_id,
             job_submission_owner_email="owner1@org.com",
         ),
     )
+    assert await fetch_count(synth_session, job_submissions_table) == 1
 
     inject_security_header("owner1@org.com", Permissions.JOB_SUBMISSIONS_EDIT)
     with time_frame() as window:
         response = await client.put(
             f"/jobbergate/job-submissions/{inserted_job_submission_id}",
             json=dict(execution_directory="/some/fake/path"),
         )
 
     assert response.status_code == status.HTTP_200_OK
     data = response.json()
 
     assert data["id"] == inserted_job_submission_id
     assert data["execution_directory"] == "/some/fake/path"
 
-    query = job_submissions_table.select(job_submissions_table.c.id == inserted_job_submission_id)
-    job_submission_data = await database.fetch_one(query)
+    job_submission = await fetch_instance(
+        synth_session, inserted_job_submission_id, job_submissions_table, JobSubmissionResponse
+    )
 
-    assert job_submission_data is not None
-    assert job_submission_data["execution_directory"] == "/some/fake/path"
-    assert job_submission_data["updated_at"] in window
+    assert job_submission is not None
+    assert str(job_submission.execution_directory) == "/some/fake/path"
+    assert job_submission.updated_at in window
 
 
 @pytest.mark.asyncio
 async def test_update_job_submission_not_found(client, inject_security_header):
     """
     Test that it is not possible to update a job_submission not found.
 
@@ -1409,138 +1509,167 @@
     response = await client.put("/jobbergate/job-submissions/9999", json=dict(job_submission_name="new name"))
 
     assert response.status_code == status.HTTP_404_NOT_FOUND
 
 
 @pytest.mark.asyncio
 async def test_update_job_submission_bad_permission(
+    synth_session,
     client,
     fill_application_data,
     fill_job_script_data,
     fill_job_submission_data,
     inject_security_header,
 ):
     """
     Test that it is not possible to update a job_submission without the permission.
 
     This test proves that it is not possible to update a job_submission if the user don't have the permission.
     We show this by asserting that the response status code of the request is 403, and that the data stored in
     the database for the job_submission is not updated.
     """
-    inserted_application_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(),
-    )
-    inserted_job_script_id = await database.execute(
-        query=job_scripts_table.insert(),
-        values=fill_job_script_data(application_id=inserted_application_id),
-    )
-    inserted_job_submission_id = await database.execute(
-        query=job_submissions_table.insert(),
-        values=fill_job_submission_data(
+    inserted_application_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(
+            application_owner_email="owner1@org.com",
+        ),
+    )
+    assert await fetch_count(synth_session, applications_table) == 1
+
+    inserted_job_script_id = await insert_data(
+        synth_session,
+        job_scripts_table,
+        fill_job_script_data(application_id=inserted_application_id),
+    )
+    assert await fetch_count(synth_session, job_scripts_table) == 1
+
+    inserted_job_submission_id = await insert_data(
+        synth_session,
+        job_submissions_table,
+        fill_job_submission_data(
             job_script_id=inserted_job_script_id,
             job_submission_name="old name",
             job_submission_owner_email="owner1@org.com",
         ),
     )
+    assert await fetch_count(synth_session, job_submissions_table) == 1
 
     inject_security_header("owner1@org.com", "INVALID_PERMISSION")
     response = await client.put(
         f"/jobbergate/job-submissions/{inserted_job_submission_id}",
         json=dict(job_submission_name="new name"),
     )
 
     assert response.status_code == status.HTTP_403_FORBIDDEN
 
-    query = job_submissions_table.select(job_submissions_table.c.id == inserted_job_submission_id)
-    job_submission = JobSubmissionResponse.parse_obj(await database.fetch_one(query))
+    job_submission = await fetch_instance(
+        synth_session, inserted_job_submission_id, job_submissions_table, JobSubmissionResponse
+    )
 
     assert job_submission is not None
     assert job_submission.job_submission_name == "old name"
 
 
 @pytest.mark.asyncio
 async def test_update_job_submission_non_owner(
+    synth_session,
     client,
     fill_application_data,
     fill_job_script_data,
     fill_job_submission_data,
     inject_security_header,
 ):
     """
     Test that it is not possible to update a job_submission if you are not the owner.
     """
-    inserted_application_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(),
-    )
-    inserted_job_script_id = await database.execute(
-        query=job_scripts_table.insert(),
-        values=fill_job_script_data(application_id=inserted_application_id),
-    )
-    inserted_job_submission_id = await database.execute(
-        query=job_submissions_table.insert(),
-        values=fill_job_submission_data(
+    inserted_application_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(
+            application_owner_email="owner1@org.com",
+        ),
+    )
+    assert await fetch_count(synth_session, applications_table) == 1
+
+    inserted_job_script_id = await insert_data(
+        synth_session,
+        job_scripts_table,
+        fill_job_script_data(application_id=inserted_application_id),
+    )
+    assert await fetch_count(synth_session, job_scripts_table) == 1
+
+    inserted_job_submission_id = await insert_data(
+        synth_session,
+        job_submissions_table,
+        fill_job_submission_data(
             job_script_id=inserted_job_script_id,
             job_submission_name="old name",
             job_submission_owner_email="owner1@org.com",
         ),
     )
+    assert await fetch_count(synth_session, job_submissions_table) == 1
 
     inject_security_header("non-owner@org.com", Permissions.JOB_SUBMISSIONS_EDIT)
     response = await client.put(
         f"/jobbergate/job-submissions/{inserted_job_submission_id}",
         json=dict(job_submission_name="new name"),
     )
 
     assert response.status_code == status.HTTP_403_FORBIDDEN
     assert "does not own" in response.text
 
 
 @pytest.mark.asyncio
 async def test_delete_job_submission(
+    synth_session,
     client,
     fill_application_data,
     fill_job_script_data,
     fill_job_submission_data,
     inject_security_header,
 ):
     """
     Test delete job_submission via DELETE.
 
     This test proves that a job_submission is successfully deleted via a DELETE request to the
     /job-submissions/<id> endpoint. We show this by asserting that the job_submission no longer exists in
     the database after the request is made and the correct status code is returned (204).
     """
-    inserted_application_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(),
-    )
-    inserted_job_script_id = await database.execute(
-        query=job_scripts_table.insert(),
-        values=fill_job_script_data(application_id=inserted_application_id),
-    )
-    inserted_job_submission_id = await database.execute(
-        query=job_submissions_table.insert(),
-        values=fill_job_submission_data(
+    inserted_application_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(
+            application_owner_email="owner1@org.com",
+        ),
+    )
+    assert await fetch_count(synth_session, applications_table) == 1
+
+    inserted_job_script_id = await insert_data(
+        synth_session,
+        job_scripts_table,
+        fill_job_script_data(application_id=inserted_application_id),
+    )
+    assert await fetch_count(synth_session, job_scripts_table) == 1
+
+    inserted_job_submission_id = await insert_data(
+        synth_session,
+        job_submissions_table,
+        fill_job_submission_data(
             job_script_id=inserted_job_script_id,
             job_submission_owner_email="owner1@org.com",
         ),
     )
-
-    count = await database.fetch_all("SELECT COUNT(*) FROM job_submissions")
-    assert count[0][0] == 1
+    assert await fetch_count(synth_session, job_submissions_table) == 1
 
     inject_security_header("owner1@org.com", Permissions.JOB_SUBMISSIONS_EDIT)
     response = await client.delete(f"/jobbergate/job-submissions/{inserted_job_submission_id}")
 
     assert response.status_code == status.HTTP_204_NO_CONTENT
-
-    count = await database.fetch_all("SELECT COUNT(*) FROM job_submissions")
-    assert count[0][0] == 0
+    assert await fetch_count(synth_session, job_submissions_table) == 0
 
 
 @pytest.mark.asyncio
 async def test_delete_job_submission_not_found(client, inject_security_header):
     """
     Test that it is not possible to delete a job_submission that is not found.
 
@@ -1551,94 +1680,109 @@
     response = await client.delete("/jobbergate/job-submissions/9999")
 
     assert response.status_code == status.HTTP_404_NOT_FOUND
 
 
 @pytest.mark.asyncio
 async def test_delete_job_submission_bad_permission(
+    synth_session,
     client,
     fill_application_data,
     fill_job_script_data,
     fill_job_submission_data,
     inject_security_header,
 ):
     """
     Test that it is not possible to delete a job_submission with an user without proper permission.
 
     This test proves that it is not possible to delete a job_submission if the user don't have the permission.
     We show this by asserting that a 403 response status code is returned and the job_submission still exists
     in the database after the request.
     """
-    inserted_application_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(),
-    )
-    inserted_job_script_id = await database.execute(
-        query=job_scripts_table.insert(),
-        values=fill_job_script_data(application_id=inserted_application_id),
-    )
-    inserted_job_submission_id = await database.execute(
-        query=job_submissions_table.insert(),
-        values=fill_job_submission_data(
+    inserted_application_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(
+            application_owner_email="owner1@org.com",
+        ),
+    )
+    assert await fetch_count(synth_session, applications_table) == 1
+
+    inserted_job_script_id = await insert_data(
+        synth_session,
+        job_scripts_table,
+        fill_job_script_data(application_id=inserted_application_id),
+    )
+    assert await fetch_count(synth_session, job_scripts_table) == 1
+
+    inserted_job_submission_id = await insert_data(
+        synth_session,
+        job_submissions_table,
+        fill_job_submission_data(
             job_script_id=inserted_job_script_id,
             job_submission_owner_email="owner1@org.com",
         ),
     )
-
-    count = await database.fetch_all("SELECT COUNT(*) FROM job_submissions")
-    assert count[0][0] == 1
+    assert await fetch_count(synth_session, job_submissions_table) == 1
 
     inject_security_header("owner1@org.com", "INVALID_PERMISSION")
     response = await client.delete(f"/jobbergate/job-submissions/{inserted_job_submission_id}")
 
     assert response.status_code == status.HTTP_403_FORBIDDEN
-
-    count = await database.fetch_all("SELECT COUNT(*) FROM job_submissions")
-    assert count[0][0] == 1
+    assert await fetch_count(synth_session, job_submissions_table) == 1
 
 
 @pytest.mark.asyncio
 async def test_delete_job_submission_non_owner(
+    synth_session,
     client,
     fill_application_data,
     fill_job_script_data,
     fill_job_submission_data,
     inject_security_header,
 ):
     """
     Test that it is not possible to delete a job_submission if you are not the owner.
     """
-    inserted_application_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(),
-    )
-    inserted_job_script_id = await database.execute(
-        query=job_scripts_table.insert(),
-        values=fill_job_script_data(application_id=inserted_application_id),
-    )
-    inserted_job_submission_id = await database.execute(
-        query=job_submissions_table.insert(),
-        values=fill_job_submission_data(
+    inserted_application_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(
+            application_owner_email="owner1@org.com",
+        ),
+    )
+    assert await fetch_count(synth_session, applications_table) == 1
+
+    inserted_job_script_id = await insert_data(
+        synth_session,
+        job_scripts_table,
+        fill_job_script_data(application_id=inserted_application_id),
+    )
+    assert await fetch_count(synth_session, job_scripts_table) == 1
+
+    inserted_job_submission_id = await insert_data(
+        synth_session,
+        job_submissions_table,
+        fill_job_submission_data(
             job_script_id=inserted_job_script_id,
             job_submission_owner_email="owner1@org.com",
         ),
     )
-
-    count = await database.fetch_all("SELECT COUNT(*) FROM job_submissions")
-    assert count[0][0] == 1
+    assert await fetch_count(synth_session, job_submissions_table) == 1
 
     inject_security_header("non-owner@org.com", Permissions.JOB_SUBMISSIONS_EDIT)
     response = await client.delete(f"/jobbergate/job-submissions/{inserted_job_submission_id}")
 
     assert response.status_code == status.HTTP_403_FORBIDDEN
     assert "does not own" in response.text
 
 
 @pytest.mark.asyncio
 async def test_job_submissions_agent_pending__success(
+    synth_session,
     client,
     fill_application_data,
     fill_job_script_data,
     fill_all_job_submission_data,
     inject_security_header,
     mocked_file_manager_factory,
 ):
@@ -1647,32 +1791,39 @@
 
     This test proves that GET /job-submissions/agent/pending returns the correct job_submissions for the agent
     making the request. We show this by asserting that the job_submissions returned in the response are
     only job_submissions with a ``client_id`` that matches the ``client_id`` found in the request's
     token payload. We also make sure that the response includes job_script_data_as_string,
     as it is fundamental for the integration with the agent.
     """
-    inserted_application_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(),
-    )
-    inserted_job_script_id = await database.execute(
-        query=job_scripts_table.insert(),
-        values=fill_job_script_data(application_id=inserted_application_id),
+    inserted_application_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(
+            application_owner_email="owner1@org.com",
+        ),
+    )
+    assert await fetch_count(synth_session, applications_table) == 1
+
+    inserted_job_script_id = await insert_data(
+        synth_session,
+        job_scripts_table,
+        fill_job_script_data(application_id=inserted_application_id),
     )
+    assert await fetch_count(synth_session, job_scripts_table) == 1
 
     main_file_path = pathlib.Path("jobbergate.py")
     dummy_job_script_files = JobScriptFiles(
         main_file_path=main_file_path, files={main_file_path: "print(__name__)"}
     )
     dummy_job_script_files.write_to_s3(inserted_job_script_id)
 
-    await database.execute_many(
-        query=job_submissions_table.insert(),
-        values=fill_all_job_submission_data(
+    await synth_session.execute(
+        job_submissions_table.insert(),
+        fill_all_job_submission_data(
             dict(
                 job_script_id=inserted_job_script_id,
                 job_submission_name="sub1",
                 job_submission_owner_email="email1@dummy.com",
                 status=JobSubmissionStatus.CREATED,
                 client_id="dummy-client",
                 execution_parameters={
@@ -1711,17 +1862,15 @@
                 execution_parameters={
                     "name": "job-submission-name-4",
                     "comment": "I am a comment",
                 },
             ),
         ),
     )
-
-    count = await database.fetch_all("SELECT COUNT(*) FROM job_submissions")
-    assert count[0][0] == 4
+    assert await fetch_count(synth_session, job_submissions_table) == 4
 
     inject_security_header(
         "who@cares.com",
         Permissions.JOB_SUBMISSIONS_VIEW,
         client_id="dummy-client",
     )
     response = await client.get("/jobbergate/job-submissions/agent/pending")
@@ -1732,40 +1881,48 @@
     assert sorted(d["job_submission_name"] for d in data) == ["sub1", "sub4"]
     assert sorted(d["job_submission_owner_email"] for d in data) == ["email1@dummy.com", "email4@dummy.com"]
     assert [JobScriptFiles(**d["job_script_files"]) for d in data] == [dummy_job_script_files] * 2
 
 
 @pytest.mark.asyncio
 async def test_job_submissions_agent_pending__missing_job_script_file(
+    synth_session,
     client,
     fill_application_data,
     fill_job_script_data,
     fill_all_job_submission_data,
     inject_security_header,
     mocked_file_manager_factory,
 ):
     """
     Test GET /job-submissions/agent/pending returns a 404.
 
     This test proves that GET /job-submissions/agent/pending returns a 404 status
     if any of the job-script files is not found. It also makes sure that the missing
     id(s) are included in the response to support debugging.
     """
-    inserted_application_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(),
-    )
-    inserted_job_script_id = await database.execute(
-        query=job_scripts_table.insert(),
-        values=fill_job_script_data(application_id=inserted_application_id),
+    inserted_application_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(
+            application_owner_email="owner1@org.com",
+        ),
+    )
+    assert await fetch_count(synth_session, applications_table) == 1
+
+    inserted_job_script_id = await insert_data(
+        synth_session,
+        job_scripts_table,
+        fill_job_script_data(application_id=inserted_application_id),
     )
+    assert await fetch_count(synth_session, job_scripts_table) == 1
 
-    await database.execute_many(
-        query=job_submissions_table.insert(),
-        values=fill_all_job_submission_data(
+    await synth_session.execute(
+        job_submissions_table.insert(),
+        fill_all_job_submission_data(
             dict(
                 job_script_id=inserted_job_script_id,
                 job_submission_name="sub1",
                 job_submission_owner_email="email1@dummy.com",
                 status=JobSubmissionStatus.CREATED,
                 client_id="dummy-client",
             ),
@@ -1788,17 +1945,15 @@
                 job_submission_name="sub4",
                 job_submission_owner_email="email4@dummy.com",
                 status=JobSubmissionStatus.CREATED,
                 client_id="dummy-client",
             ),
         ),
     )
-
-    count = await database.fetch_all("SELECT COUNT(*) FROM job_submissions")
-    assert count[0][0] == 4
+    assert await fetch_count(synth_session, job_submissions_table) == 4
 
     inject_security_header(
         "who@cares.com",
         Permissions.JOB_SUBMISSIONS_VIEW,
         client_id="dummy-client",
     )
     response = await client.get("/jobbergate/job-submissions/agent/pending")
@@ -1825,39 +1980,48 @@
     response = await client.get("/jobbergate/job-submissions/agent/pending")
     assert response.status_code == status.HTTP_400_BAD_REQUEST
     assert "token does not contain a `client_id`" in response.text
 
 
 @pytest.mark.asyncio
 async def test_job_submissions_agent_update__success(
+    synth_session,
     fill_application_data,
     fill_job_script_data,
     fill_all_job_submission_data,
     client,
     inject_security_header,
 ):
     """
     Test PUT /job-submissions/{job_submission_id} correctly updates a job_submission status.
 
     This test proves that a job_submission is successfully updated via a PUT request to the
     /job-submissions/{job_submission_id} endpoint. We show this by asserting that the job_submission is
     updated in the database after the post request is made, the correct status code (200) is returned.
     We also show that the ``status`` column is set to the new status value.
     """
-    inserted_application_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(),
-    )
-    inserted_job_script_id = await database.execute(
-        query=job_scripts_table.insert(),
-        values=fill_job_script_data(application_id=inserted_application_id),
-    )
-    await database.execute_many(
-        query=job_submissions_table.insert(),
-        values=fill_all_job_submission_data(
+    inserted_application_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(
+            application_owner_email="owner1@org.com",
+        ),
+    )
+    assert await fetch_count(synth_session, applications_table) == 1
+
+    inserted_job_script_id = await insert_data(
+        synth_session,
+        job_scripts_table,
+        fill_job_script_data(application_id=inserted_application_id),
+    )
+    assert await fetch_count(synth_session, job_scripts_table) == 1
+
+    await synth_session.execute(
+        job_submissions_table.insert(),
+        fill_all_job_submission_data(
             dict(
                 job_script_id=inserted_job_script_id,
                 job_submission_name="sub1",
                 status=JobSubmissionStatus.CREATED,
                 client_id="dummy-client",
                 slurm_job_id=None,
             ),
@@ -1880,23 +2044,22 @@
                 job_submission_name="sub4",
                 status=JobSubmissionStatus.CREATED,
                 client_id="dummy-client",
                 slurm_job_id=None,
             ),
         ),
     )
+    assert await fetch_count(synth_session, job_submissions_table) == 4
 
-    count = await database.fetch_all("SELECT COUNT(*) FROM job_submissions")
-    assert count[0][0] == 4
-
-    target_job_submission = await database.fetch_one(
-        query=job_submissions_table.select().where(job_submissions_table.c.job_submission_name == "sub1")
+    raw_result = await synth_session.execute(
+        job_submissions_table.select().where(job_submissions_table.c.job_submission_name == "sub1")
     )
+    target_job_submission = raw_result.one_or_none()
     assert target_job_submission is not None
-    job_submission_id = target_job_submission["id"]
+    job_submission_id = target_job_submission.id
 
     inject_security_header(
         "who@cares.com",
         Permissions.JOB_SUBMISSIONS_EDIT,
         client_id="dummy-client",
     )
     response = await client.put(
@@ -1913,79 +2076,90 @@
     assert data["status"] == JobSubmissionStatus.SUBMITTED
     assert data["slurm_job_id"] == 111
     assert data["execution_directory"] is None
 
 
 @pytest.mark.asyncio
 async def test_job_submissions_agent_update__job_rejected(
+    synth_session,
     fill_application_data,
     fill_job_script_data,
     fill_all_job_submission_data,
     client,
     inject_security_header,
 ):
     """
     Test PUT /job-submissions/{job_submission_id} correctly updates a job_submission status to rejected.
 
     This test proves that a job_submission is successfully updated via a PUT request to the
     /job-submissions/{job_submission_id} endpoint. We show this by asserting that the job_submission is
     updated in the database after the post request is made, the correct status code (200) is returned.
     We also show that the ``status`` column is set to the new status value.
     """
-    inserted_application_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(),
-    )
-    inserted_job_script_id = await database.execute(
-        query=job_scripts_table.insert(),
-        values=fill_job_script_data(application_id=inserted_application_id),
-    )
-    await database.execute_many(
-        query=job_submissions_table.insert(),
-        values=fill_all_job_submission_data(
+    inserted_application_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(
+            application_owner_email="owner1@org.com",
+        ),
+    )
+    assert await fetch_count(synth_session, applications_table) == 1
+
+    inserted_job_script_id = await insert_data(
+        synth_session,
+        job_scripts_table,
+        fill_job_script_data(application_id=inserted_application_id),
+    )
+    assert await fetch_count(synth_session, job_scripts_table) == 1
+
+    await synth_session.execute(
+        job_submissions_table.insert(),
+        fill_all_job_submission_data(
             dict(
                 job_script_id=inserted_job_script_id,
                 job_submission_name="sub1",
                 status=JobSubmissionStatus.CREATED,
                 client_id="dummy-client",
                 slurm_job_id=None,
                 execution_parameters={"name": "job-submission-name", "comment": "I am a comment"},
             ),
             dict(
                 job_script_id=inserted_job_script_id,
                 job_submission_name="sub2",
                 status=JobSubmissionStatus.COMPLETED,
                 client_id="dummy-client",
                 slurm_job_id=None,
+                execution_parameters=None,
             ),
             dict(
                 job_script_id=inserted_job_script_id,
                 job_submission_name="sub3",
                 status=JobSubmissionStatus.CREATED,
                 client_id="silly-client",
                 slurm_job_id=None,
+                execution_parameters=None,
             ),
             dict(
                 job_script_id=inserted_job_script_id,
                 job_submission_name="sub4",
                 status=JobSubmissionStatus.CREATED,
                 client_id="dummy-client",
                 slurm_job_id=None,
+                execution_parameters=None,
             ),
         ),
     )
+    assert await fetch_count(synth_session, job_submissions_table) == 4
 
-    count = await database.fetch_all("SELECT COUNT(*) FROM job_submissions")
-    assert count[0][0] == 4
-
-    target_job_submission = await database.fetch_one(
-        query=job_submissions_table.select().where(job_submissions_table.c.job_submission_name == "sub1")
+    raw_result = await synth_session.execute(
+        job_submissions_table.select().where(job_submissions_table.c.job_submission_name == "sub1")
     )
+    target_job_submission = raw_result.one_or_none()
     assert target_job_submission is not None
-    job_submission_id = target_job_submission["id"]
+    job_submission_id = target_job_submission.id
 
     inject_security_header(
         "who@cares.com",
         Permissions.JOB_SUBMISSIONS_EDIT,
         client_id="dummy-client",
     )
     response = await client.put(
@@ -2029,39 +2203,48 @@
     )
     assert response.status_code == status.HTTP_400_BAD_REQUEST
     assert "token does not contain a `client_id`" in response.text
 
 
 @pytest.mark.asyncio
 async def test_job_submissions_agent_active__success(
+    synth_session,
     client,
     fill_application_data,
     fill_job_script_data,
     fill_all_job_submission_data,
     inject_security_header,
 ):
     """
     Test GET /job-submissions/agent/active returns only active job_submissions owned by the requesting agent.
 
     This test proves that GET /job-submissions/agent/active returns the correct job_submissions for the agent
     making the request. We show this by asserting that the job_submissions returned in the response are
     only job_submissions with a ``client_id`` that matches the ``client_id`` found in the request's
     token payload and have a status of ``SUBMITTED``.
     """
-    inserted_application_id = await database.execute(
-        query=applications_table.insert(),
-        values=fill_application_data(),
-    )
-    inserted_job_script_id = await database.execute(
-        query=job_scripts_table.insert(),
-        values=fill_job_script_data(application_id=inserted_application_id),
-    )
-    await database.execute_many(
-        query=job_submissions_table.insert(),
-        values=fill_all_job_submission_data(
+    inserted_application_id = await insert_data(
+        synth_session,
+        applications_table,
+        fill_application_data(
+            application_owner_email="owner1@org.com",
+        ),
+    )
+    assert await fetch_count(synth_session, applications_table) == 1
+
+    inserted_job_script_id = await insert_data(
+        synth_session,
+        job_scripts_table,
+        fill_job_script_data(application_id=inserted_application_id),
+    )
+    assert await fetch_count(synth_session, job_scripts_table) == 1
+
+    await synth_session.execute(
+        job_submissions_table.insert(),
+        fill_all_job_submission_data(
             dict(
                 job_script_id=inserted_job_script_id,
                 job_submission_name="sub1",
                 status=JobSubmissionStatus.CREATED,
                 client_id="dummy-client",
                 slurm_job_id=11,
             ),
@@ -2084,17 +2267,15 @@
                 job_submission_name="sub4",
                 status=JobSubmissionStatus.SUBMITTED,
                 client_id="dummy-client",
                 slurm_job_id=44,
             ),
         ),
     )
-
-    count = await database.fetch_all("SELECT COUNT(*) FROM job_submissions")
-    assert count[0][0] == 4
+    assert await fetch_count(synth_session, job_submissions_table) == 4
 
     inject_security_header(
         "who@cares.com",
         Permissions.JOB_SUBMISSIONS_VIEW,
         client_id="dummy-client",
     )
     response = await client.get("/jobbergate/job-submissions/agent/active")
```

### Comparing `jobbergate_api-3.5.0a7/jobbergate_api/tests/conftest.py` & `jobbergate_api-3.6.0/jobbergate_api/tests/conftest.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,72 +1,86 @@
 """
 Configuration of pytest.
 """
 
+import asyncio
 import contextlib
 import dataclasses
 import datetime
 import random
 import string
 import typing
 from textwrap import dedent
 from unittest.mock import patch
 
 import pytest
-import sqlalchemy
-from asgi_lifespan import LifespanManager
 from file_storehouse.engine import EngineLocal
 from httpx import AsyncClient
 
-from jobbergate_api.apps.applications.models import applications_table
-from jobbergate_api.apps.job_scripts.models import job_scripts_table
-from jobbergate_api.apps.job_submissions.models import job_submissions_table
 from jobbergate_api.config import settings
 from jobbergate_api.main import app
 from jobbergate_api.metadata import metadata
 from jobbergate_api.s3_manager import file_manager_factory
-from jobbergate_api.storage import build_db_url, database
+from jobbergate_api.storage import engine_factory
 
 # Charset for producing random strings
 CHARSET = string.ascii_letters + string.digits + string.punctuation
 
 
-@pytest.fixture(autouse=True, scope="session")
-async def database_engine():
-    """
-    Provide a fixture to get access to the database engine with a fixture.
+@pytest.fixture(scope="session", autouse=True)
+def event_loop():
     """
-    engine = sqlalchemy.create_engine(build_db_url())
-    yield engine
+    Create an instance of the default event loop for each test case.
 
+    This fixture is used to run each test in a different async loop. Running all
+    in the same loop causes errors with SQLAlchemy. See the following two issues:
 
-@pytest.fixture(autouse=True, scope="session")
-async def enforce_empty_database(database_engine):
-    """
-    Make sure our database is empty at the end of each test.
-    """
-    metadata.create_all(database_engine)
-    yield
-
-    await database.connect()
-    for table in (applications_table, job_scripts_table, job_submissions_table):
-        count = await database.execute(sqlalchemy.select([sqlalchemy.func.count()]).select_from(table))
-        assert count == 0
-    await database.disconnect()
+    1. https://github.com/tiangolo/fastapi/issues/5692
+    2. https://github.com/encode/starlette/issues/1315
 
-    metadata.drop_all(database_engine)
+    [Reference](https://tonybaloney.github.io/posts/async-test-patterns-for-pytest-and-unittest.html)
+    """
+    loop = asyncio.get_event_loop_policy().new_event_loop()
+    yield loop
+    loop.close()
 
 
-@pytest.fixture()
-async def startup_event_force():
+@pytest.fixture(autouse=True, scope="session")
+async def synth_engine():
     """
-    Force the async event loop to begin.
+    Provide a fixture to prepare the test database.
     """
-    async with LifespanManager(app):
-        yield
+    engine = engine_factory.get_engine()
+    async with engine.begin() as connection:
+        await connection.run_sync(metadata.create_all, checkfirst=True)
+    try:
+        yield engine
+    finally:
+        async with engine.begin() as connection:
+            for table in reversed(metadata.sorted_tables):
+                await connection.execute(table.delete())
+        await engine_factory.cleanup()
+
+
+@pytest.fixture(scope="function")
+async def synth_session():
+    """
+    Get a session from the engine_factory for the current test function.
+
+    This is necessary to make sure that the test code uses the same session as the one returned by
+    the dependency injection for the router code. Otherwise, changes made in the router's session would not
+    be visible in the test code. Not that changes made in this synthesized session are always rolled back
+    and never committed.
+    """
+    session = engine_factory.get_session()
+    with patch("jobbergate_api.storage.engine_factory.get_session", return_value=session):
+        await session.begin_nested()
+        yield session
+        await session.rollback()
+        await session.close()
 
 
 @pytest.fixture(autouse=True)
 def enforce_mocked_oidc_provider(mock_openid_server):
     """
     Enforce that the OIDC provider used by armasec is the mock_openid_server provided as a fixture.
 
@@ -94,19 +108,21 @@
     will be injected into the custom identity claims.
     """
 
     def _helper(
         owner_email: str,
         *permissions: typing.List[str],
         client_id: typing.Optional[str] = None,
+        organization_id: typing.Optional[str] = None,
     ):
-        claim_overrides = dict(
+        claim_overrides: typing.Dict = dict(
             email=owner_email,
             client_id=client_id,
             permissions=permissions,
+            organization={organization_id: dict()},
         )
         token = build_rs256_token(claim_overrides=claim_overrides)
         client.headers.update({"Authorization": f"Bearer {token}"})
 
     return _helper
```

### Comparing `jobbergate_api-3.5.0a7/jobbergate_api/tests/integration/draft_test_jobbergate_slurm_job_properties.py` & `jobbergate_api-3.6.0/jobbergate_api/tests/integration/draft_test_jobbergate_slurm_job_properties.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a7/jobbergate_api/tests/test_config.py` & `jobbergate_api-3.6.0/jobbergate_api/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a7/jobbergate_api/tests/test_email_notification.py` & `jobbergate_api-3.6.0/jobbergate_api/tests/test_email_notification.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a7/jobbergate_api/tests/test_meta_mapper.py` & `jobbergate_api-3.6.0/jobbergate_api/tests/test_meta_mapper.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a7/jobbergate_api/tests/test_pagination.py` & `jobbergate_api-3.6.0/jobbergate_api/tests/test_pagination.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,19 +6,14 @@
 
 import pytest
 from pydantic import ValidationError
 
 from jobbergate_api.apps.applications.models import applications_table
 from jobbergate_api.apps.applications.schemas import ApplicationResponse
 from jobbergate_api.pagination import Pagination, Response, package_response
-from jobbergate_api.storage import database
-
-# Force the async event loop at the app to begin.
-# Since this is a time consuming fixture, it is just used where strict necessary.
-pytestmark = pytest.mark.usefixtures("startup_event_force")
 
 
 def test_init_fails_on_invalid_parameters():
     """
     Tests that the parameters are valid or an exception will be raised.
     """
     with pytest.raises(ValidationError, match="ensure this value is greater than or equal to 0"):
@@ -45,33 +40,32 @@
     assert pagination.dict() == dict(start=13, limit=21)
 
     pagination = Pagination(start=None, limit=999)
     assert pagination.dict() == dict()
 
 
 @pytest.mark.asyncio
-@database.transaction(force_rollback=True)
-async def test_package_response__without_pagination():
+async def test_package_response__without_pagination(synth_session):
     """
     Test the package_response method without pagination.
     """
-    await database.execute_many(
-        query=applications_table.insert(),
-        values=[
+    await synth_session.execute(
+        applications_table.insert(),
+        [
             dict(
                 application_owner_email=f"owner{i}@org.com",
                 application_name=f"app{i}",
             )
             for i in range(1, 6)
         ],
     )
 
     query = applications_table.select()
     pagination = Pagination()
-    raw_response = await package_response(ApplicationResponse, query, pagination)
+    raw_response = await package_response(synth_session, ApplicationResponse, query, pagination)
     response = Response[ApplicationResponse].parse_obj(json.loads(raw_response.body))
 
     results = response.results
     assert len(results) == 5
     for (i, result) in enumerate(results):
         assert isinstance(result, ApplicationResponse)
         assert result.application_name == f"app{i + 1}"
@@ -82,36 +76,35 @@
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize(
     "start,limit,total",
     [(0, 1, 1), (6, 2, 13), (2, 3, 10), (7, 2, 13)],
 )
-@database.transaction(force_rollback=True)
-async def test_package_response__with_pagination(start, limit, total):
+async def test_package_response__with_pagination(start, limit, total, synth_session):
     """
     Test the package_response method with pagination.
 
     Parameters test pagination at upper bound and lower bound of total
     """
-    await database.execute_many(
-        query=applications_table.insert(),
-        values=[
+    await synth_session.execute(
+        applications_table.insert(),
+        [
             dict(
                 id=i,
                 application_owner_email=f"owner{i}@org.com",
                 application_name=f"app{i}",
             )
             for i in range(1, total + 1)
         ],
     )
 
     query = applications_table.select()
     pagination = Pagination(start=start, limit=limit)
-    raw_response = await package_response(ApplicationResponse, query, pagination)
+    raw_response = await package_response(synth_session, ApplicationResponse, query, pagination)
     response = Response[ApplicationResponse].parse_obj(json.loads(raw_response.body))
 
     results = response.results
     # Clamps the expected count at upper bound
     expected_count = max(0, min(total - start * limit, limit))
     assert len(results) == expected_count
     for (i, result) in enumerate(results):
```

### Comparing `jobbergate_api-3.5.0a7/jobbergate_api/tests/test_s3_manager.py` & `jobbergate_api-3.6.0/jobbergate_api/tests/test_s3_manager.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a7/jobbergate_api/tests/test_version.py` & `jobbergate_api-3.6.0/jobbergate_api/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a7/jobbergate_api/version.py` & `jobbergate_api-3.6.0/jobbergate_api/version.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a7/pyproject.toml` & `jobbergate_api-3.6.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jobbergate-api"
-version = "3.5.0a7"
+version = "3.6.0"
 description = "Jobbergate API"
 authors = ["Omnivector Solutions <info@omnivector.solutions>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/omnivector-solutions/jobbergate"
 classifiers = [
     "License :: OSI Approved :: MIT License",
@@ -24,29 +24,29 @@
 fastapi = "^0.68.0"
 email_validator = "^1.1.0"
 passlib = "^1.7.2"
 python-multipart = "^0.0.5"
 python-dotenv = "^0.20.0"
 boto3 = "^1.17.51"
 Jinja2 = "^3.0.3"
-asyncpg = "^0.22.0"
+asyncpg = "^0.27"
 loguru = "^0.6.0"
 uvicorn = "^0.15.0"
 armasec = "^0.11.0"
 sentry-sdk = "^1.5.0"
 yarl = "^1.7.2"
 alembic = "^1.7.5"
 typer = "^0.4.0"
-databases = {extras = ["postgresql"], version = "^0.5.5"}
 PyYAML = "^6.0"
 sendgrid = "^6.9.7"
 file-storehouse = "0.5.0"
 py-buzz = "^3.2.1"
 toml = "^0.10.2"
 bidict = "^0.22.0"
+sqlalchemy = {extras = ["mypy"], version = "^2.0.17"}
 
 [tool.poetry.dev-dependencies]
 black = "^22"
 pre-commit = "^2.9.2"
 pytest = "^6.2"
 pytest-asyncio = "^0.12"
 pytest-cov = "^2.8"
@@ -54,15 +54,14 @@
 requests = "^2.23.0"
 nest_asyncio = "^1.3.3"
 coverage = "^5.1"
 pgcli = "^3.1.0"
 ipython = "^7.31.1"
 pytest-freezegun = "^0.4.2"
 pytest-env = "^0.6.2"
-asgi-lifespan = "^1.0.1"
 pytest-random-order = "^1.0.4"
 mypy = "^0.910"
 sqlalchemy-stubs = "^0.4"
 isort = "^5.9.3"
 respx = "^0.17.1"
 py-docker-gadgets = "^0.1.1"
 pyproject-flake8 = "^0.0.1-alpha.2"
@@ -79,15 +78,15 @@
 line_length = 110
 multi_line_output = 3
 include_trailing_comma = true
 
 [tool.flake8]
 max_line_length = 110
 exclude = "alembic/*"
-ignore = "D200,D106,D402"
+ignore = "D200,D106,D402,W503"
 
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = ["--random-order", "--cov=jobbergate_api"]
 testpaths = ["jobbergate_api/tests"]
 env = [
@@ -95,15 +94,15 @@
     "ARMASEC_DOMAIN = armasec.dev",  # Must align with the rs256_domain fixture in armasec's pytest extension
     "ARMASEC_DEBUG = False",  # Set this to True to debug armasec issues by seeing verbose logging
     "SENDGRID_FROM_EMAIL = info@pytesting.com",
     "SENDGRID_API_KEY = test-api-key",
 ]
 
 [tool.coverage.report]
-    fail_under = 95
+    fail_under = 90  # Temporarily reduced until Jobbergate 4.x is completed
     show_missing = true
 
 [[tool.mypy.overrides]]
 module = [
     "boto3",
     "botocore.*",
     "uvicorn",
```

### Comparing `jobbergate_api-3.5.0a7/PKG-INFO` & `jobbergate_api-3.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jobbergate-api
-Version: 3.5.0a7
+Version: 3.6.0
 Summary: Jobbergate API
 Home-page: https://github.com/omnivector-solutions/jobbergate
 License: MIT
 Author: Omnivector Solutions
 Author-email: info@omnivector.solutions
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,28 +18,28 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Requires-Dist: Jinja2 (>=3.0.3,<4.0.0)
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: alembic (>=1.7.5,<2.0.0)
 Requires-Dist: armasec (>=0.11.0,<0.12.0)
-Requires-Dist: asyncpg (>=0.22.0,<0.23.0)
+Requires-Dist: asyncpg (>=0.27,<0.28)
 Requires-Dist: bidict (>=0.22.0,<0.23.0)
 Requires-Dist: boto3 (>=1.17.51,<2.0.0)
-Requires-Dist: databases[postgresql] (>=0.5.5,<0.6.0)
 Requires-Dist: email_validator (>=1.1.0,<2.0.0)
 Requires-Dist: fastapi (>=0.68.0,<0.69.0)
 Requires-Dist: file-storehouse (==0.5.0)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: passlib (>=1.7.2,<2.0.0)
 Requires-Dist: py-buzz (>=3.2.1,<4.0.0)
 Requires-Dist: python-dotenv (>=0.20.0,<0.21.0)
 Requires-Dist: python-multipart (>=0.0.5,<0.0.6)
 Requires-Dist: sendgrid (>=6.9.7,<7.0.0)
 Requires-Dist: sentry-sdk (>=1.5.0,<2.0.0)
+Requires-Dist: sqlalchemy[mypy] (>=2.0.17,<3.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: typer (>=0.4.0,<0.5.0)
 Requires-Dist: uvicorn (>=0.15.0,<0.16.0)
 Requires-Dist: yarl (>=1.7.2,<2.0.0)
 Project-URL: Bug Tracker, https://github.com/omnivector-solutions/jobbergate/issues
 Project-URL: Changelog, https://github.com/omnivector-solutions/jobbergate/blob/main/jobbergate-api/CHANGELOG.rst
 Project-URL: Repository, https://github.com/omnivector-solutions/jobbergate
```

