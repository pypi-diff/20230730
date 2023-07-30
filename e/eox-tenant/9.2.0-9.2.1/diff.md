# Comparing `tmp/eox-tenant-9.2.0.tar.gz` & `tmp/eox-tenant-9.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eox-tenant-9.2.0.tar", last modified: Thu Jun 29 19:31:26 2023, max compression
+gzip compressed data, was "eox-tenant-9.2.1.tar", last modified: Sun Jul 30 14:27:07 2023, max compression
```

## Comparing `eox-tenant-9.2.0.tar` & `eox-tenant-9.2.1.tar`

### file list

```diff
@@ -1,139 +1,136 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:26.546257 eox-tenant-9.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7574 2023-06-29 19:31:26.546257 eox-tenant-9.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:26.534257 eox-tenant-9.2.0/eox_tenant/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8485 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:26.538257 eox-tenant-9.2.0/eox_tenant/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/api/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:26.538257 eox-tenant-9.2.0/eox_tenant/api/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/api/v1/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/api/v1/routers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/api/v1/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:26.538257 eox-tenant-9.2.0/eox_tenant/api/v1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/api/v1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/api/v1/tests/test_microsites.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/api/v1/tests/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/api/v1/tests/test_routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/api/v1/tests/test_tenant_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/api/v1/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    15315 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/api/v1/viewsets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/async_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:26.538257 eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:26.542257 eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/backends/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/backends/bearer_authentication_l_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/backends/bearer_authentication_test_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/backends/branding_api_l_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/backends/dark_lang_middleware_o_test_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/backends/dark_lang_middleware_o_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/backends/edx_auth_i_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/backends/edxmako_l_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/backends/oauth_dispatch_j_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/backends/site_configuration_module_i_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/backends/site_configuration_module_test_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/backends/theming_helpers_h_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/backends/theming_helpers_test_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/backends/users_l_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/backends/users_test_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/bearer_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/branding_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/dark_lang_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/edxmako_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/get_common_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/oauth_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/site_configuration_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/theming_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:26.542257 eox-tenant-9.2.0/eox_tenant/filters/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/filters/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:26.542257 eox-tenant-9.2.0/eox_tenant/filters/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/filters/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/filters/test/test_pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:26.542257 eox-tenant-9.2.0/eox_tenant/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:26.542257 eox-tenant-9.2.0/eox_tenant/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/management/commands/change_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/management/commands/change_signup_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/management/commands/edit_tenant_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/management/commands/synchronize_organizations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:26.542257 eox-tenant-9.2.0/eox_tenant/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/migrations/0003_auto_20190620_1704.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/migrations/0005_auto_20191226_1225.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/migrations/0006_tenantorganization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/migrations/0007_auto_20200922_1421.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/migrations/0008_synchronize_tenants.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7303 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/organizations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/receivers_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:26.542257 eox-tenant-9.2.0/eox_tenant/settings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/settings/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/settings/production.py
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/settings/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8612 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:26.530257 eox-tenant-9.2.0/eox_tenant/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:26.542257 eox-tenant-9.2.0/eox_tenant/templates/eox-tenant/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/templates/eox-tenant/not_found.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:26.546257 eox-tenant-9.2.0/eox_tenant/templates/eox-tenant/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/templates/eox-tenant/widgets/json_widget.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:26.546257 eox-tenant-9.2.0/eox_tenant/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/templatetags/ednx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:26.546257 eox-tenant-9.2.0/eox_tenant/tenant_aware_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/tenant_aware_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/tenant_aware_functions/enrollments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/tenant_aware_functions/released_languages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:26.546257 eox-tenant-9.2.0/eox_tenant/tenant_wise/
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/tenant_wise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/tenant_wise/context_managers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/tenant_wise/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:26.546257 eox-tenant-9.2.0/eox_tenant/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/test/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/test/test_async_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9983 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/test/test_auth_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/test/test_change_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/test/test_change_signupsource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/test/test_edit_tenant_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/test/test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/test/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/test/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/test/test_receivers_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12458 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/test/test_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/test/test_tenant_aware_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/test/test_tenant_wise.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/test/test_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/test/test_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:26.538257 eox-tenant-9.2.0/eox_tenant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7574 2023-06-29 19:31:26.000000 eox-tenant-9.2.0/eox_tenant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-06-29 19:31:26.000000 eox-tenant-9.2.0/eox_tenant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 19:31:26.000000 eox-tenant-9.2.0/eox_tenant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-29 19:31:26.000000 eox-tenant-9.2.0/eox_tenant.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 19:31:26.000000 eox-tenant-9.2.0/eox_tenant.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 19:31:26.000000 eox-tenant-9.2.0/eox_tenant.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6498 2023-06-29 19:31:26.550257 eox-tenant-9.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:27:07.047352 eox-tenant-9.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7574 2023-07-30 14:27:07.047352 eox-tenant-9.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:27:07.019351 eox-tenant-9.2.1/eox_tenant/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8485 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:27:07.023352 eox-tenant-9.2.1/eox_tenant/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/api/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:27:07.023352 eox-tenant-9.2.1/eox_tenant/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/api/v1/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/api/v1/routers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/api/v1/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:27:07.027351 eox-tenant-9.2.1/eox_tenant/api/v1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/api/v1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/api/v1/tests/test_microsites.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/api/v1/tests/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/api/v1/tests/test_routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/api/v1/tests/test_tenant_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/api/v1/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15315 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/api/v1/viewsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/async_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:27:07.027351 eox-tenant-9.2.1/eox_tenant/edxapp_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/edxapp_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/edxapp_wrapper/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:27:07.031351 eox-tenant-9.2.1/eox_tenant/edxapp_wrapper/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/edxapp_wrapper/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/edxapp_wrapper/backends/bearer_authentication_l_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/edxapp_wrapper/backends/bearer_authentication_test_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/edxapp_wrapper/backends/branding_api_l_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/edxapp_wrapper/backends/edx_auth_i_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/edxapp_wrapper/backends/edxmako_l_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/edxapp_wrapper/backends/oauth_dispatch_j_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/edxapp_wrapper/backends/site_configuration_module_i_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/edxapp_wrapper/backends/site_configuration_module_test_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/edxapp_wrapper/backends/theming_helpers_h_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/edxapp_wrapper/backends/theming_helpers_test_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/edxapp_wrapper/backends/users_l_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/edxapp_wrapper/backends/users_test_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/edxapp_wrapper/bearer_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/edxapp_wrapper/branding_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/edxapp_wrapper/edxmako_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/edxapp_wrapper/get_common_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/edxapp_wrapper/oauth_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/edxapp_wrapper/site_configuration_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/edxapp_wrapper/theming_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/edxapp_wrapper/users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:27:07.031351 eox-tenant-9.2.1/eox_tenant/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/filters/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:27:07.035352 eox-tenant-9.2.1/eox_tenant/filters/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/filters/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/filters/test/test_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:27:07.035352 eox-tenant-9.2.1/eox_tenant/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:27:07.035352 eox-tenant-9.2.1/eox_tenant/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/management/commands/change_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/management/commands/change_signup_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/management/commands/edit_tenant_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/management/commands/synchronize_organizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:27:07.039352 eox-tenant-9.2.1/eox_tenant/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/migrations/0003_auto_20190620_1704.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/migrations/0005_auto_20191226_1225.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/migrations/0006_tenantorganization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/migrations/0007_auto_20200922_1421.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/migrations/0008_synchronize_tenants.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7303 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/receivers_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:27:07.039352 eox-tenant-9.2.1/eox_tenant/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/settings/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/settings/production.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/settings/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8612 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:27:07.011351 eox-tenant-9.2.1/eox_tenant/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:27:07.039352 eox-tenant-9.2.1/eox_tenant/templates/eox-tenant/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/templates/eox-tenant/not_found.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:27:07.039352 eox-tenant-9.2.1/eox_tenant/templates/eox-tenant/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/templates/eox-tenant/widgets/json_widget.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:27:07.039352 eox-tenant-9.2.1/eox_tenant/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/templatetags/ednx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:27:07.039352 eox-tenant-9.2.1/eox_tenant/tenant_aware_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/tenant_aware_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/tenant_aware_functions/enrollments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/tenant_aware_functions/released_languages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:27:07.043352 eox-tenant-9.2.1/eox_tenant/tenant_wise/
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/tenant_wise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/tenant_wise/context_managers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6254 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/tenant_wise/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:27:07.047352 eox-tenant-9.2.1/eox_tenant/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/test/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/test/test_async_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9983 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/test/test_auth_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/test/test_change_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/test/test_change_signupsource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/test/test_edit_tenant_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/test/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/test/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/test/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/test/test_receivers_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12458 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/test/test_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/test/test_tenant_aware_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/test/test_tenant_wise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/test/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/test/test_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/eox_tenant/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:27:07.023352 eox-tenant-9.2.1/eox_tenant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7574 2023-07-30 14:27:06.000000 eox-tenant-9.2.1/eox_tenant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-07-30 14:27:07.000000 eox-tenant-9.2.1/eox_tenant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 14:27:06.000000 eox-tenant-9.2.1/eox_tenant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-30 14:27:06.000000 eox-tenant-9.2.1/eox_tenant.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 14:27:06.000000 eox-tenant-9.2.1/eox_tenant.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-30 14:27:06.000000 eox-tenant-9.2.1/eox_tenant.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6498 2023-07-30 14:27:07.047352 eox-tenant-9.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-30 14:26:51.000000 eox-tenant-9.2.1/setup.py
```

### Comparing `eox-tenant-9.2.0/LICENSE.txt` & `eox-tenant-9.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.2.0/PKG-INFO` & `eox-tenant-9.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eox-tenant
-Version: 9.2.0
+Version: 9.2.1
 Summary: Edunext Open edx extensions tenant.
 Author: eduNEXT
 Author-email: contact@edunext.co
 License: AGPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.2
```

### Comparing `eox-tenant-9.2.0/README.rst` & `eox-tenant-9.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.2.0/eox_tenant/admin.py` & `eox-tenant-9.2.1/eox_tenant/admin.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.2.0/eox_tenant/api/v1/permissions.py` & `eox-tenant-9.2.1/eox_tenant/api/v1/permissions.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.2.0/eox_tenant/api/v1/serializers.py` & `eox-tenant-9.2.1/eox_tenant/api/v1/serializers.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.2.0/eox_tenant/api/v1/tests/test_microsites.py` & `eox-tenant-9.2.1/eox_tenant/api/v1/tests/test_microsites.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.2.0/eox_tenant/api/v1/tests/test_permissions.py` & `eox-tenant-9.2.1/eox_tenant/api/v1/tests/test_permissions.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.2.0/eox_tenant/api/v1/tests/test_routes.py` & `eox-tenant-9.2.1/eox_tenant/api/v1/tests/test_routes.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.2.0/eox_tenant/api/v1/tests/test_tenant_config.py` & `eox-tenant-9.2.1/eox_tenant/api/v1/tests/test_tenant_config.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.2.0/eox_tenant/api/v1/viewsets.py` & `eox-tenant-9.2.1/eox_tenant/api/v1/viewsets.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.2.0/eox_tenant/apps.py` & `eox-tenant-9.2.1/eox_tenant/apps.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.2.0/eox_tenant/async_utils.py` & `eox-tenant-9.2.1/eox_tenant/async_utils.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.2.0/eox_tenant/auth.py` & `eox-tenant-9.2.1/eox_tenant/auth.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/auth.py` & `eox-tenant-9.2.1/eox_tenant/edxapp_wrapper/auth.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/backends/bearer_authentication_l_v1.py` & `eox-tenant-9.2.1/eox_tenant/edxapp_wrapper/backends/bearer_authentication_l_v1.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/backends/edx_auth_i_v1.py` & `eox-tenant-9.2.1/eox_tenant/edxapp_wrapper/backends/edx_auth_i_v1.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/backends/site_configuration_module_test_v1.py` & `eox-tenant-9.2.1/eox_tenant/edxapp_wrapper/backends/site_configuration_module_test_v1.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/site_configuration_module.py` & `eox-tenant-9.2.1/eox_tenant/edxapp_wrapper/site_configuration_module.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.2.0/eox_tenant/filters/pipeline.py` & `eox-tenant-9.2.1/eox_tenant/filters/pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,30 +9,30 @@
 
 
 class FilterUserCourseEnrollmentsByTenant(PipelineStep):
     """
     Filter enrollments list by a tenant.
     """
 
-    def run_filter(self, context):  # pylint: disable=arguments-differ
+    def run_filter(self, enrollments):  # pylint: disable=arguments-differ
         """
         Filter especific user course enrollments by tenant request.
         Example Usage:
-        Add the following configurations to you configuration file
+        Add the following configurations to your configuration file
             "OPEN_EDX_FILTERS_CONFIG": {
-                "org.openedx.learning.course_enrollments_site.filter.requested.v1": {
+                "org.openedx.learning.course_enrollment_queryset.requested.v1": {
                     "fail_silently": false,
                     "pipeline": [
                         "eox_tenant.filters.pipeline.FilterUserCourseEnrollmentsByTenant"
                     ]
                 }
             }
         """
-        tenant_enrollments = filter_enrollments(context)
-        return {"context": tenant_enrollments}
+        tenant_enrollments = filter_enrollments(enrollments)
+        return {"enrollments": tenant_enrollments}
 
 
 class FilterRenderCertificatesByOrg(PipelineStep):
     """
     Stop certificate generation process raising a exception
     if course org is different to tenant orgs.
     Example usage:
```

### Comparing `eox-tenant-9.2.0/eox_tenant/filters/test/test_pipeline.py` & `eox-tenant-9.2.1/eox_tenant/filters/test/test_pipeline.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,41 +2,20 @@
 Test cases for Open edX Filters steps.
 """
 from unittest.mock import MagicMock
 
 import ddt
 import mock
 from django.test import TestCase, override_settings
-from openedx_filters.learning.filters import CertificateRenderStarted
-from openedx_filters.tooling import OpenEdxPublicFilter
+from openedx_filters.learning.filters import CertificateRenderStarted, CourseEnrollmentQuerysetRequested
 
 from eox_tenant.filters.pipeline import FilterRenderCertificatesByOrg
 from eox_tenant.tenant_aware_functions.enrollments import filter_enrollments
 
 
-# This class was temporarily added while the filter is added in openedx-filters.
-class CourseEnrollmentSiteFilterRequested(OpenEdxPublicFilter):
-    """
-    Custom class used to filter user's course enrollments by site.
-    """
-
-    filter_type = "org.openedx.learning.course_enrollments_site.filter.requested.v1"
-
-    @classmethod
-    def run_filter(cls, context):
-        """
-        Execute a filter with the signature specified.
-
-        Arguments:
-        context (QuerySet): list of all user's course enrollments.
-        """
-        data = super().run_pipeline(context=context)
-        return data.get("context")
-
-
 class FilterUserCourseEnrollmentsByTenantTestCase(TestCase):
     """
     FilterUserCourseEnrollmentsByTenant test cases.
     """
 
     def setUp(self):
         """This method creates Microsite objects in database"""
@@ -48,15 +27,15 @@
             enroll_mock = MagicMock()
             enroll_mock.course_id.org = org
             enrolls.append(enroll_mock)
         self.course_enrollments = enrolls
 
     @override_settings(
         OPEN_EDX_FILTERS_CONFIG={
-            "org.openedx.learning.course_enrollments_site.filter.requested.v1": {
+            "org.openedx.learning.course_enrollment_queryset.requested.v1": {
                 "fail_silently": False,
                 "pipeline": [
                     "eox_tenant.filters.pipeline.FilterUserCourseEnrollmentsByTenant"
                 ],
             }
         }
     )
@@ -84,26 +63,26 @@
         theming_helpers_mock.is_request_in_themed_site.return_value = True
 
         get_conf_helpers_mock.return_value = conf_helpers_mock
         get_theming_helpers_mock.return_value = theming_helpers_mock
 
         expected_result = filter_enrollments(self.course_enrollments)
 
-        result = CourseEnrollmentSiteFilterRequested.run_filter(
-            context=self.course_enrollments
+        result = CourseEnrollmentQuerysetRequested.run_filter(
+            enrollments=self.course_enrollments
         )
         expected_result = list(expected_result)
         result = list(result)
 
         self.assertListEqual(expected_result, result)
         self.assertEqual(expected_result[0].course_id.org, result[0].course_id.org)
 
     @override_settings(
         OPEN_EDX_FILTERS_CONFIG={
-            "org.openedx.learning.course_enrollments_site.filter.requested.v1": {
+            "org.openedx.learning.course_enrollment_queryset.requested.v1": {
                 "fail_silently": False,
                 "pipeline": [
                     "eox_tenant.filters.pipeline.FilterUserCourseEnrollmentsByTenant"
                 ],
             }
         }
     )
@@ -132,16 +111,16 @@
         conf_helpers_mock.get_all_orgs.return_value = ["org1", "demo", "org3"]
 
         get_conf_helpers_mock.return_value = conf_helpers_mock
         get_theming_helpers_mock.return_value = theming_helpers_mock
 
         expected_result = filter_enrollments(self.course_enrollments)
 
-        result = CourseEnrollmentSiteFilterRequested.run_filter(
-            context=self.course_enrollments
+        result = CourseEnrollmentQuerysetRequested.run_filter(
+            enrollments=self.course_enrollments
         )
 
         self.assertListEqual(list(expected_result), list(result))
 
 
 @ddt.ddt
 class FilterRenderCertificatesByOrgTestCase(TestCase):
```

### Comparing `eox-tenant-9.2.0/eox_tenant/management/commands/change_domain.py` & `eox-tenant-9.2.1/eox_tenant/management/commands/change_domain.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.2.0/eox_tenant/management/commands/change_signup_sources.py` & `eox-tenant-9.2.1/eox_tenant/management/commands/change_signup_sources.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.2.0/eox_tenant/management/commands/edit_tenant_values.py` & `eox-tenant-9.2.1/eox_tenant/management/commands/edit_tenant_values.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.2.0/eox_tenant/management/commands/synchronize_organizations.py` & `eox-tenant-9.2.1/eox_tenant/management/commands/synchronize_organizations.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.2.0/eox_tenant/middleware.py` & `eox-tenant-9.2.1/eox_tenant/middleware.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.2.0/eox_tenant/migrations/0001_initial.py` & `eox-tenant-9.2.1/eox_tenant/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.2.0/eox_tenant/migrations/0003_auto_20190620_1704.py` & `eox-tenant-9.2.1/eox_tenant/migrations/0003_auto_20190620_1704.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.2.0/eox_tenant/migrations/0005_auto_20191226_1225.py` & `eox-tenant-9.2.1/eox_tenant/migrations/0005_auto_20191226_1225.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.2.0/eox_tenant/migrations/0006_tenantorganization.py` & `eox-tenant-9.2.1/eox_tenant/migrations/0006_tenantorganization.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.2.0/eox_tenant/migrations/0007_auto_20200922_1421.py` & `eox-tenant-9.2.1/eox_tenant/migrations/0007_auto_20200922_1421.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.2.0/eox_tenant/models.py` & `eox-tenant-9.2.1/eox_tenant/models.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.2.0/eox_tenant/permissions.py` & `eox-tenant-9.2.1/eox_tenant/permissions.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.2.0/eox_tenant/pipeline.py` & `eox-tenant-9.2.1/eox_tenant/pipeline.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.2.0/eox_tenant/receivers_helpers.py` & `eox-tenant-9.2.1/eox_tenant/receivers_helpers.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.2.0/eox_tenant/settings/common.py` & `eox-tenant-9.2.1/eox_tenant/settings/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,15 +44,14 @@
     settings.EOX_TENANT_EDX_AUTH_BACKEND = "eox_tenant.edxapp_wrapper.backends.edx_auth_i_v1"
     settings.EOX_TENANT_USERS_BACKEND = 'eox_tenant.edxapp_wrapper.backends.users_l_v1'
     settings.EOX_TENANT_BEARER_AUTHENTICATION = 'eox_tenant.edxapp_wrapper.backends.bearer_authentication_l_v1'
     settings.EOX_MAX_CONFIG_OVERRIDE_SECONDS = 300
     settings.EDXMAKO_MODULE_BACKEND = 'eox_tenant.edxapp_wrapper.backends.edxmako_l_v1'
     settings.UTILS_MODULE_BACKEND = 'eox_tenant.edxapp_wrapper.backends.util_h_v1'
     settings.CHANGE_DOMAIN_DEFAULT_SITE_NAME = "stage.edunext.co"
-    settings.DARK_LANG_MIDDLEWARE = 'eox_tenant.edxapp_wrapper.backends.dark_lang_middleware_o_v1'
     settings.EOX_TENANT_LOAD_PERMISSIONS = True
     settings.EOX_TENANT_APPEND_LMS_MIDDLEWARE_CLASSES = False
     settings.USE_EOX_TENANT = False
 
     settings.EOX_TENANT_ASYNC_TASKS_HANDLER_DICT = {
         "openedx.core.djangoapps.schedules.tasks.ScheduleRecurringNudge": "get_host_from_siteid",
     }
```

### Comparing `eox-tenant-9.2.0/eox_tenant/settings/production.py` & `eox-tenant-9.2.1/eox_tenant/settings/production.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.2.0/eox_tenant/settings/test.py` & `eox-tenant-9.2.1/eox_tenant/settings/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,14 @@
         INSTALLED_APPS.append(app)
 
 GET_CERTIFICATES_MODULE = 'eox_tenant.edxapp_wrapper.backends.certificates_module_test_v1'
 GET_SITE_CONFIGURATION_MODULE = 'eox_tenant.edxapp_wrapper.backends.site_configuration_module_test_v1'
 GET_THEMING_HELPERS = 'eox_tenant.edxapp_wrapper.backends.theming_helpers_test_v1'
 EOX_TENANT_USERS_BACKEND = 'eox_tenant.edxapp_wrapper.backends.users_test_v1'
 EOX_TENANT_BEARER_AUTHENTICATION = 'eox_tenant.edxapp_wrapper.backends.bearer_authentication_test_v1'
-DARK_LANG_MIDDLEWARE = 'eox_tenant.edxapp_wrapper.backends.dark_lang_middleware_o_test_v1'
 
 COURSE_KEY_PATTERN = r'(?P<course_key_string>[^/+]+(/|\+)[^/+]+(/|\+)[^/?]+)'
 COURSE_ID_PATTERN = COURSE_KEY_PATTERN.replace('course_key_string', 'course_id')
 
 TEST_DICT_OVERRIDE_TEST = {
     'key1': 'Some Value'
 }
```

### Comparing `eox-tenant-9.2.0/eox_tenant/signals.py` & `eox-tenant-9.2.1/eox_tenant/signals.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.2.0/eox_tenant/templatetags/ednx.py` & `eox-tenant-9.2.1/eox_tenant/templatetags/ednx.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.2.0/eox_tenant/tenant_aware_functions/enrollments.py` & `eox-tenant-9.2.1/eox_tenant/tenant_aware_functions/enrollments.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.2.0/eox_tenant/tenant_aware_functions/released_languages.py` & `eox-tenant-9.2.1/eox_tenant/tenant_aware_functions/released_languages.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.2.0/eox_tenant/tenant_wise/__init__.py` & `eox-tenant-9.2.1/eox_tenant/tenant_wise/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from importlib import import_module
 
 import six
 from django.conf import settings
 
 from eox_tenant.constants import LMS_ENVIRONMENT
 from eox_tenant.tenant_aware_functions.released_languages import tenant_languages
-from eox_tenant.tenant_wise.proxies import DarkLangMiddlewareProxy, TenantSiteConfigProxy
+from eox_tenant.tenant_wise.proxies import TenantSiteConfigProxy
 
 
 def load_tenant_wise_overrides():
     """
     Here are all the necessary overrides for the platform models.
     """
     if getattr(settings, 'USE_EOX_TENANT', False):
@@ -35,19 +35,14 @@
 
             if settings.FEATURES.get("EDNX_SITE_AWARE_LOCALE", False):
                 set_as_proxy(
                     modules='openedx.core.djangoapps.lang_pref.api',
                     model='released_languages',
                     proxy=tenant_languages
                 )
-                set_as_proxy(
-                    modules='openedx.core.djangoapps.dark_lang.middleware',
-                    model='DarkLangMiddleware',
-                    proxy=DarkLangMiddlewareProxy
-                )
 
 
 def set_as_proxy(modules, model, proxy):
     """
     Helper to patch a loaded module with a proxy object that has all the Tenant wise properties.
     """
     if isinstance(modules, six.string_types):
```

### Comparing `eox-tenant-9.2.0/eox_tenant/tenant_wise/context_managers.py` & `eox-tenant-9.2.1/eox_tenant/tenant_wise/context_managers.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.2.0/eox_tenant/tenant_wise/proxies.py` & `eox-tenant-9.2.1/eox_tenant/tenant_wise/proxies.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,21 +5,19 @@
 import logging
 from itertools import chain
 
 import six
 from django.conf import settings
 from django.core.cache import cache
 
-from eox_tenant.edxapp_wrapper.dark_lang_middleware import get_dark_lang_middleware
 from eox_tenant.edxapp_wrapper.site_configuration_module import get_site_configuration_models
 from eox_tenant.models import Microsite, TenantConfig, TenantOrganization
 from eox_tenant.utils import clean_serializable_values
 
 SiteConfigurationModels = get_site_configuration_models()
-DarkLangMiddleware = get_dark_lang_middleware()
 
 TENANT_ALL_ORGS_CACHE_KEY = "tenant.all_orgs_list"
 EOX_TENANT_CACHE_KEY_TIMEOUT = getattr(
     settings,
     "EOX_TENANT_CACHE_KEY_TIMEOUT",
     300
 )
@@ -194,43 +192,7 @@
                 org_filter = [org_filter]
 
             for org in org_filter:
                 key = "org-value-{}-{}".format(org, val_name)
                 cls.set_key_to_cache(key, result)
 
         cls.set_key_to_cache(pre_load_value_key, True)
-
-
-class DarkLangMiddlewareProxy(DarkLangMiddleware):
-    """This Middleware will be used if you have FEATURES["EDNX_SITE_AWARE_LOCALE"] in True.
-    This take the released_languages from the site aware settings, and set a HTTP_ACCEPT_LANGUAGE if
-    you don't have one."""
-
-    class Meta:
-        """ Set as a proxy model. """
-        proxy = True
-
-    @property
-    def released_langs(self):
-        """
-        Current list of released languages from settings.
-        """
-
-        get_language_options = getattr(settings, "released_languages", "")
-        language_options = [lang.lower().strip() for lang in get_language_options.split(',')]
-        if settings.LANGUAGE_CODE not in language_options:
-            language_options.append(settings.LANGUAGE_CODE)
-        return language_options
-
-    def process_request(self, request):
-        """
-        This will be run when you do a request, and prevent user from requesting un-released languages.
-        """
-
-        # If the request doesn't have HTTP_ACCEPT_LANGUAGE, eduNEXT set it to
-        # settings.LANGUAGE_CODE that is site aware so that
-        # django.utils.locale.LocaleMiddleware can pick it up
-        accept = request.META.get('HTTP_ACCEPT_LANGUAGE', None)
-        if not accept:
-            request.META['HTTP_ACCEPT_LANGUAGE'] = f"{settings.LANGUAGE_CODE};q=0.1"
-
-        self._clean_accept_headers(request)
```

### Comparing `eox-tenant-9.2.0/eox_tenant/test/test_admin.py` & `eox-tenant-9.2.1/eox_tenant/test/test_admin.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.2.0/eox_tenant/test/test_async_utils.py` & `eox-tenant-9.2.1/eox_tenant/test/test_async_utils.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.2.0/eox_tenant/test/test_auth_backend.py` & `eox-tenant-9.2.1/eox_tenant/test/test_auth_backend.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.2.0/eox_tenant/test/test_change_domain.py` & `eox-tenant-9.2.1/eox_tenant/test/test_change_domain.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.2.0/eox_tenant/test/test_change_signupsource.py` & `eox-tenant-9.2.1/eox_tenant/test/test_change_signupsource.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.2.0/eox_tenant/test/test_edit_tenant_values.py` & `eox-tenant-9.2.1/eox_tenant/test/test_edit_tenant_values.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.2.0/eox_tenant/test/test_middleware.py` & `eox-tenant-9.2.1/eox_tenant/test/test_middleware.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.2.0/eox_tenant/test/test_models.py` & `eox-tenant-9.2.1/eox_tenant/test/test_models.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.2.0/eox_tenant/test/test_pipeline.py` & `eox-tenant-9.2.1/eox_tenant/test/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.2.0/eox_tenant/test/test_receivers_helpers.py` & `eox-tenant-9.2.1/eox_tenant/test/test_receivers_helpers.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.2.0/eox_tenant/test/test_signals.py` & `eox-tenant-9.2.1/eox_tenant/test/test_signals.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.2.0/eox_tenant/test/test_tenant_aware_functions.py` & `eox-tenant-9.2.1/eox_tenant/test/test_tenant_aware_functions.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.2.0/eox_tenant/test/test_tenant_wise.py` & `eox-tenant-9.2.1/eox_tenant/test/test_tenant_wise.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.2.0/eox_tenant/test/test_utils.py` & `eox-tenant-9.2.1/eox_tenant/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.2.0/eox_tenant/test/test_views.py` & `eox-tenant-9.2.1/eox_tenant/test/test_views.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.2.0/eox_tenant/test/test_wrappers.py` & `eox-tenant-9.2.1/eox_tenant/test/test_wrappers.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.2.0/eox_tenant/utils.py` & `eox-tenant-9.2.1/eox_tenant/utils.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.2.0/eox_tenant/validators.py` & `eox-tenant-9.2.1/eox_tenant/validators.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.2.0/eox_tenant/views.py` & `eox-tenant-9.2.1/eox_tenant/views.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.2.0/eox_tenant/widgets.py` & `eox-tenant-9.2.1/eox_tenant/widgets.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.2.0/eox_tenant.egg-info/PKG-INFO` & `eox-tenant-9.2.1/eox_tenant.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eox-tenant
-Version: 9.2.0
+Version: 9.2.1
 Summary: Edunext Open edx extensions tenant.
 Author: eduNEXT
 Author-email: contact@edunext.co
 License: AGPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.2
```

### Comparing `eox-tenant-9.2.0/eox_tenant.egg-info/SOURCES.txt` & `eox-tenant-9.2.1/eox_tenant.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -41,27 +41,24 @@
 eox_tenant/api/v1/tests/test_permissions.py
 eox_tenant/api/v1/tests/test_routes.py
 eox_tenant/api/v1/tests/test_tenant_config.py
 eox_tenant/edxapp_wrapper/__init__.py
 eox_tenant/edxapp_wrapper/auth.py
 eox_tenant/edxapp_wrapper/bearer_authentication.py
 eox_tenant/edxapp_wrapper/branding_api.py
-eox_tenant/edxapp_wrapper/dark_lang_middleware.py
 eox_tenant/edxapp_wrapper/edxmako_module.py
 eox_tenant/edxapp_wrapper/get_common_util.py
 eox_tenant/edxapp_wrapper/oauth_dispatch.py
 eox_tenant/edxapp_wrapper/site_configuration_module.py
 eox_tenant/edxapp_wrapper/theming_helpers.py
 eox_tenant/edxapp_wrapper/users.py
 eox_tenant/edxapp_wrapper/backends/__init__.py
 eox_tenant/edxapp_wrapper/backends/bearer_authentication_l_v1.py
 eox_tenant/edxapp_wrapper/backends/bearer_authentication_test_v1.py
 eox_tenant/edxapp_wrapper/backends/branding_api_l_v1.py
-eox_tenant/edxapp_wrapper/backends/dark_lang_middleware_o_test_v1.py
-eox_tenant/edxapp_wrapper/backends/dark_lang_middleware_o_v1.py
 eox_tenant/edxapp_wrapper/backends/edx_auth_i_v1.py
 eox_tenant/edxapp_wrapper/backends/edxmako_l_v1.py
 eox_tenant/edxapp_wrapper/backends/oauth_dispatch_j_v1.py
 eox_tenant/edxapp_wrapper/backends/site_configuration_module_i_v1.py
 eox_tenant/edxapp_wrapper/backends/site_configuration_module_test_v1.py
 eox_tenant/edxapp_wrapper/backends/theming_helpers_h_v1.py
 eox_tenant/edxapp_wrapper/backends/theming_helpers_test_v1.py
```

### Comparing `eox-tenant-9.2.0/setup.cfg` & `eox-tenant-9.2.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 9.2.0
+current_version = 9.2.1
 commit = False
 tag = False
 
 [bumpversion:file:eox_tenant/__init__.py]
 
 [coverage:run]
 data_file = .coverage
```

### Comparing `eox-tenant-9.2.0/setup.py` & `eox-tenant-9.2.1/setup.py`

 * *Files identical despite different names*

