# Comparing `tmp/domain-admin-1.5.8.tar.gz` & `tmp/domain-admin-1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domain-admin-1.5.8.tar", last modified: Mon Jul 24 15:15:14 2023, max compression
+gzip compressed data, was "domain-admin-1.5.9.tar", last modified: Sun Jul 30 05:37:42 2023, max compression
```

## Comparing `domain-admin-1.5.8.tar` & `domain-admin-1.5.9.tar`

### file list

```diff
@@ -1,458 +1,461 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.793414 domain-admin-1.5.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-24 15:14:59.000000 domain-admin-1.5.8/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (123)      417 2023-07-24 15:14:59.000000 domain-admin-1.5.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    18454 2023-07-24 15:15:14.793414 domain-admin-1.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17012 2023-07-24 15:14:59.000000 domain-admin-1.5.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.737414 domain-admin-1.5.8/domain_admin/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.741413 domain-admin-1.5.8/domain_admin/api/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/api/address_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/api/auth_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/api/cert_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    17243 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/api/domain_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    16941 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/api/domain_info_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/api/group_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/api/group_user_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/api/ip_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/api/issue_certificate_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/api/log_async_task_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/api/log_operation_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/api/log_scheduler_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6461 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/api/notify_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/api/prometheus_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/api/system_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/api/user_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/api/whois_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.741413 domain-admin-1.5.8/domain_admin/config/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/config/default_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/config/env_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/config/runtime_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.741413 domain-admin-1.5.8/domain_admin/enums/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/enums/config_key_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/enums/event_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/enums/notify_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/enums/operation_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/enums/role_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/enums/status_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/enums/version_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.745413 domain-admin-1.5.8/domain_admin/migrate/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/migrate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/migrate/migrate_102_to_103.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/migrate/migrate_106_to_110.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/migrate/migrate_110_to_1212.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/migrate/migrate_1212_to_1213.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/migrate/migrate_1213_to_131.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/migrate/migrate_136_to_140_alpha.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/migrate/migrate_140_alpha_to_140.py
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/migrate/migrate_1413_to_1414.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/migrate/migrate_1422_to_1423.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/migrate/migrate_143_to_144.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/migrate/migrate_145_to_146.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/migrate/migrate_151_to_152.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/migrate/migrate_154_to_155.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/migrate/migrate_common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.745413 domain-admin-1.5.8/domain_admin/model/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/model/address_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/model/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/model/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/model/domain_info_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/model/domain_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/model/group_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/model/group_user_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/model/issue_certificate_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/model/log_async_task_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/model/log_operation_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/model/log_scheduler_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/model/notify_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/model/system_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/model/user_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/model/version_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.745413 domain-admin-1.5.8/domain_admin/public/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.749413 domain-admin-1.5.8/domain_admin/public/.git/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/FETCH_HEAD
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/HEAD
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/config
--rwxr-xr-x   0 runner    (1001) docker     (123)       73 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/description
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.749413 domain-admin-1.5.8/domain_admin/public/.git/hooks/
--rwxr-xr-x   0 runner    (1001) docker     (123)      478 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/hooks/applypatch-msg.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      896 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/hooks/commit-msg.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     4726 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/hooks/fsmonitor-watchman.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      189 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/hooks/post-update.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      424 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/hooks/pre-applypatch.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     1643 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/hooks/pre-commit.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      416 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/hooks/pre-merge-commit.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     1374 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/hooks/pre-push.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     4898 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/hooks/pre-rebase.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      544 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/hooks/pre-receive.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     1492 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/hooks/prepare-commit-msg.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     2783 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/hooks/push-to-checkout.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     2308 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/hooks/sendemail-validate.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     3650 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/hooks/update.sample
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/index
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.749413 domain-admin-1.5.8/domain_admin/public/.git/info/
--rwxr-xr-x   0 runner    (1001) docker     (123)      240 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/info/exclude
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.749413 domain-admin-1.5.8/domain_admin/public/.git/logs/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/logs/HEAD
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.725413 domain-admin-1.5.8/domain_admin/public/.git/logs/refs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.749413 domain-admin-1.5.8/domain_admin/public/.git/logs/refs/heads/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/logs/refs/heads/dist
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.725413 domain-admin-1.5.8/domain_admin/public/.git/logs/refs/remotes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.749413 domain-admin-1.5.8/domain_admin/public/.git/logs/refs/remotes/origin/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/logs/refs/remotes/origin/dist
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.729413 domain-admin-1.5.8/domain_admin/public/.git/objects/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.749413 domain-admin-1.5.8/domain_admin/public/.git/objects/19/
--r--r--r--   0 runner    (1001) docker     (123)    64350 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/19/7f5cf73cf11d43d915904e0d8aad4736a77d63
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.749413 domain-admin-1.5.8/domain_admin/public/.git/objects/21/
--r--r--r--   0 runner    (1001) docker     (123)       61 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/21/00bd7d2219a26827cc80aa37fe72fcb303bb50
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.749413 domain-admin-1.5.8/domain_admin/public/.git/objects/2b/
--r--r--r--   0 runner    (1001) docker     (123)      223 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/2b/3195083ee5802a2c60fdb9919fbf35e18e6478
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.749413 domain-admin-1.5.8/domain_admin/public/.git/objects/32/
--r--r--r--   0 runner    (1001) docker     (123)     1435 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/32/dd3b54be707f423bd7375381bbc2baede37f8c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.749413 domain-admin-1.5.8/domain_admin/public/.git/objects/37/
--r--r--r--   0 runner    (1001) docker     (123)     1700 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/37/11576f2b615224b9477da0a0a9a43c17539d12
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.753414 domain-admin-1.5.8/domain_admin/public/.git/objects/3c/
--r--r--r--   0 runner    (1001) docker     (123)     3081 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/3c/0f2e923566dc74d04e67d46d8b722923ed1949
--r--r--r--   0 runner    (1001) docker     (123)   148706 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/3c/2434ab20d756f0a95ad24f6a5adb7e1219a7d1
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.753414 domain-admin-1.5.8/domain_admin/public/.git/objects/3e/
--r--r--r--   0 runner    (1001) docker     (123)     1736 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/3e/24054f5e3a680f56b9276efe009e73b7133a99
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.753414 domain-admin-1.5.8/domain_admin/public/.git/objects/4b/
--r--r--r--   0 runner    (1001) docker     (123)     8843 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/4b/f6af202944cd3e22f8a375977737ce52b17763
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.753414 domain-admin-1.5.8/domain_admin/public/.git/objects/52/
--r--r--r--   0 runner    (1001) docker     (123)    62564 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/52/c1926de72b181c9b7faf597fb8f71f48565462
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.753414 domain-admin-1.5.8/domain_admin/public/.git/objects/55/
--r--r--r--   0 runner    (1001) docker     (123)      119 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/55/1103b11c4b699a3b4107d3a2ab173dfe238556
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.753414 domain-admin-1.5.8/domain_admin/public/.git/objects/57/
--r--r--r--   0 runner    (1001) docker     (123)     5129 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/57/bd1a9bfce972b50e5efecf11f71a3f5b2ec3d3
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.753414 domain-admin-1.5.8/domain_admin/public/.git/objects/5f/
--r--r--r--   0 runner    (1001) docker     (123)      530 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/5f/a7faf700c98850aa96022ab07af6a07b854f34
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.753414 domain-admin-1.5.8/domain_admin/public/.git/objects/60/
--r--r--r--   0 runner    (1001) docker     (123)      464 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/60/727d43f26f701780e7c55e90cb084973a1be9e
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.753414 domain-admin-1.5.8/domain_admin/public/.git/objects/69/
--r--r--r--   0 runner    (1001) docker     (123)   279936 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/69/a9dda41cf39bb60d1dc5b1158ffba197580b6a
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.753414 domain-admin-1.5.8/domain_admin/public/.git/objects/6c/
--r--r--r--   0 runner    (1001) docker     (123)      155 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/6c/3e3059f9ec00c015681abca34b751c3439513d
--r--r--r--   0 runner    (1001) docker     (123)     6011 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/6c/f21ee6e3a69b2e234f6012f1636e3621d25db8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.753414 domain-admin-1.5.8/domain_admin/public/.git/objects/6d/
--r--r--r--   0 runner    (1001) docker     (123)      612 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/6d/15191314c9b832ac41056a30bf0bf6533a29dc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.753414 domain-admin-1.5.8/domain_admin/public/.git/objects/71/
--r--r--r--   0 runner    (1001) docker     (123)      100 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/71/6b5718c659ed5a85d4f93a2cf25fc5ff5031cb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.753414 domain-admin-1.5.8/domain_admin/public/.git/objects/79/
--r--r--r--   0 runner    (1001) docker     (123)   105817 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/79/404c2464172f80b414d111f49718327b3ef93b
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.753414 domain-admin-1.5.8/domain_admin/public/.git/objects/7c/
--r--r--r--   0 runner    (1001) docker     (123)    17315 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/7c/7a565bed760068496030f030f2b05ede1bec4b
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.753414 domain-admin-1.5.8/domain_admin/public/.git/objects/7f/
--r--r--r--   0 runner    (1001) docker     (123)      368 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/7f/64d8af0501887e805dc9ccf8228f4fb5e73fdb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.753414 domain-admin-1.5.8/domain_admin/public/.git/objects/88/
--r--r--r--   0 runner    (1001) docker     (123)     5817 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/88/eed16a647060a310c6f8fd8cbf109ad11d1211
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.753414 domain-admin-1.5.8/domain_admin/public/.git/objects/89/
--r--r--r--   0 runner    (1001) docker     (123)      106 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/89/0f3ed83973272c63b56a722a88fe25160d11d2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.753414 domain-admin-1.5.8/domain_admin/public/.git/objects/8c/
--r--r--r--   0 runner    (1001) docker     (123)       69 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/8c/f880f5a9481ef71cd22e08d59e7d366775b360
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.753414 domain-admin-1.5.8/domain_admin/public/.git/objects/8f/
--r--r--r--   0 runner    (1001) docker     (123)     1895 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/8f/3fc862ebdfdd80953e51ae5e44e7862b79ad63
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.753414 domain-admin-1.5.8/domain_admin/public/.git/objects/92/
--r--r--r--   0 runner    (1001) docker     (123)      200 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/92/cfface0a460c51331fb8f25083a09948e00cbf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.757413 domain-admin-1.5.8/domain_admin/public/.git/objects/95/
--r--r--r--   0 runner    (1001) docker     (123)      118 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/95/f07af46d709638b20c0b2c66cdf6de8e89a7e4
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.757413 domain-admin-1.5.8/domain_admin/public/.git/objects/9a/
--r--r--r--   0 runner    (1001) docker     (123)     3440 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/9a/44f010e55bd5cd3a7d60bcd86ee9b8e7ef2cef
--r--r--r--   0 runner    (1001) docker     (123)      177 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/9a/4e8fcc1912f0c1af9a1836ebd9847d8b0e3118
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.757413 domain-admin-1.5.8/domain_admin/public/.git/objects/a5/
--r--r--r--   0 runner    (1001) docker     (123)    11673 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/a5/6b22c2eacca280122dde700a98068ebdd8c5af
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.757413 domain-admin-1.5.8/domain_admin/public/.git/objects/a7/
--r--r--r--   0 runner    (1001) docker     (123)     4249 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/a7/49320e6e50d7593d7d1d30ee0159023cd4e422
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.757413 domain-admin-1.5.8/domain_admin/public/.git/objects/ae/
--r--r--r--   0 runner    (1001) docker     (123)     1815 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/ae/1c9a7def175d7a6389679bf822a6a9219c3ca3
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.757413 domain-admin-1.5.8/domain_admin/public/.git/objects/b2/
--r--r--r--   0 runner    (1001) docker     (123)     1021 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/b2/9b2820070fd0808f478afc2a5995aaee9cd79f
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.757413 domain-admin-1.5.8/domain_admin/public/.git/objects/b3/
--r--r--r--   0 runner    (1001) docker     (123)    41902 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/b3/1cb2667f48424e34cf9517362eadf899f704ad
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.757413 domain-admin-1.5.8/domain_admin/public/.git/objects/c4/
--r--r--r--   0 runner    (1001) docker     (123)       61 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/c4/c46ae2c464a49661d7793709077759039f0b5e
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.757413 domain-admin-1.5.8/domain_admin/public/.git/objects/c9/
--r--r--r--   0 runner    (1001) docker     (123)     2690 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/c9/3d3f53fd06fdbc8587e3a8f37876356c5cdb56
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.757413 domain-admin-1.5.8/domain_admin/public/.git/objects/cc/
--r--r--r--   0 runner    (1001) docker     (123)   361458 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/cc/bfeaa0b21986ed309cbb83d17585b54f3b2fb9
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.757413 domain-admin-1.5.8/domain_admin/public/.git/objects/d2/
--r--r--r--   0 runner    (1001) docker     (123)     1024 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/d2/5bbe60e329a2e662af042df10825c9dcdc3887
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.757413 domain-admin-1.5.8/domain_admin/public/.git/objects/e0/
--r--r--r--   0 runner    (1001) docker     (123)      312 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/e0/6f4cc670d4bb8f606c4edfb9d7aa51becaaf2a
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.757413 domain-admin-1.5.8/domain_admin/public/.git/objects/e1/
--r--r--r--   0 runner    (1001) docker     (123)    23927 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/e1/13bfd922675ce50e68cdf88cd94d16130ad58b
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.757413 domain-admin-1.5.8/domain_admin/public/.git/objects/e6/
--r--r--r--   0 runner    (1001) docker     (123)      229 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/e6/8884f9d8cc37153041b8b82943d995c95ba1aa
--r--r--r--   0 runner    (1001) docker     (123)      637 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/e6/e9c9b85a9477efa2c8f05874bd09fa93a6b34c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.757413 domain-admin-1.5.8/domain_admin/public/.git/objects/e9/
--r--r--r--   0 runner    (1001) docker     (123)      474 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/e9/8d4dd298d6c05d0bfa2fbe9182ec7cddde7926
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.757413 domain-admin-1.5.8/domain_admin/public/.git/objects/f9/
--r--r--r--   0 runner    (1001) docker     (123)      694 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/f9/78f4b33c1fdc0cb74f1df45d0fc049f5da1c89
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.757413 domain-admin-1.5.8/domain_admin/public/.git/objects/fb/
--r--r--r--   0 runner    (1001) docker     (123)     7633 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/fb/ac0b57e4138b4fca9c9f5babf558611a38e6d0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.757413 domain-admin-1.5.8/domain_admin/public/.git/objects/fd/
--r--r--r--   0 runner    (1001) docker     (123)     5204 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/fd/bd32c675f85af4ed57021ac0638a21a3c6cad3
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.757413 domain-admin-1.5.8/domain_admin/public/.git/objects/ff/
--r--r--r--   0 runner    (1001) docker     (123)    13943 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/objects/ff/9c65dfdc7a16150c07745e0030a9d6373920cd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.733413 domain-admin-1.5.8/domain_admin/public/.git/refs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.761413 domain-admin-1.5.8/domain_admin/public/.git/refs/heads/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/refs/heads/dist
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.733413 domain-admin-1.5.8/domain_admin/public/.git/refs/remotes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.761413 domain-admin-1.5.8/domain_admin/public/.git/refs/remotes/origin/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/refs/remotes/origin/dist
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/.git/shallow
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.761413 domain-admin-1.5.8/domain_admin/public/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/css/ConditionFilterGroup.a91875e6.css
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/css/index.302e10d7.css
--rw-r--r--   0 runner    (1001) docker     (123)   331526 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/css/index.69a97337.css
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/css/index.93c714bb.css
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/css/index.a676cc2e.css
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/css/index.b285e10a.css
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/css/index.cf805e1c.css
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/css/index.d028ae37.css
--rwxr-xr-x   0 runner    (1001) docker     (123)    15406 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.761413 domain-admin-1.5.8/domain_admin/public/gif/
--rw-r--r--   0 runner    (1001) docker     (123)     6334 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/gif/user-avatar.ea67286d.gif
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.761413 domain-admin-1.5.8/domain_admin/public/jpg/
--rw-r--r--   0 runner    (1001) docker     (123)    14271 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/jpg/chatpet-white.10f4f36c.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    24940 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/jpg/chatpet.fce5580e.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.769414 domain-admin-1.5.8/domain_admin/public/js/
--rw-r--r--   0 runner    (1001) docker     (123)    18591 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/js/ConditionFilterGroup.3c6ac067.js
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/js/ConnectStatus.a429b01b.js
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/js/SearchUser.f8e52158.js
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/js/SelectGroup.53d83114.js
--rw-r--r--   0 runner    (1001) docker     (123)   390997 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/js/codemirror-lib.a3a39aa0.js
--rw-r--r--   0 runner    (1001) docker     (123)   195335 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/js/element-icon.1ce1c350.js
--rw-r--r--   0 runner    (1001) docker     (123)   749914 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/js/element-plus.30eb1cab.js
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/js/event-enums.6c6f25e7.js
--rw-r--r--   0 runner    (1001) docker     (123)  1058329 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/js/highlight-lib.3654f6d3.js
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/js/highlight-util.a4f1867f.js
--rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/js/index.0963ab53.js
--rw-r--r--   0 runner    (1001) docker     (123)    15553 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/js/index.0d4c27ce.js
--rw-r--r--   0 runner    (1001) docker     (123)    64712 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/js/index.165f9ce1.js
--rw-r--r--   0 runner    (1001) docker     (123)    28081 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/js/index.24e255af.js
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/js/index.2ab02c40.js
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/js/index.3b5a616c.js
--rw-r--r--   0 runner    (1001) docker     (123)     8982 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/js/index.5b4cd516.js
--rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/js/index.5f8ece3f.js
--rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/js/index.654f7830.js
--rw-r--r--   0 runner    (1001) docker     (123)     9882 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/js/index.8c31b31b.js
--rw-r--r--   0 runner    (1001) docker     (123)    39363 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/js/index.a8bb8abf.js
--rw-r--r--   0 runner    (1001) docker     (123)    28958 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/js/index.af06b2dc.js
--rw-r--r--   0 runner    (1001) docker     (123)    21499 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/js/index.c22f6489.js
--rw-r--r--   0 runner    (1001) docker     (123)     9652 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/js/index.deff2c63.js
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/js/index.ef82c865.js
--rw-r--r--   0 runner    (1001) docker     (123)   312580 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/js/vendor-lib.76301fc3.js
--rw-r--r--   0 runner    (1001) docker     (123)    94202 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/js/vendor-vue.9e61e0af.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.769414 domain-admin-1.5.8/domain_admin/public/m/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.773414 domain-admin-1.5.8/domain_admin/public/m/.git/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/FETCH_HEAD
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/HEAD
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/config
--rwxr-xr-x   0 runner    (1001) docker     (123)       73 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/description
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.773414 domain-admin-1.5.8/domain_admin/public/m/.git/hooks/
--rwxr-xr-x   0 runner    (1001) docker     (123)      478 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/hooks/applypatch-msg.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      896 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/hooks/commit-msg.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     4726 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/hooks/fsmonitor-watchman.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      189 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/hooks/post-update.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      424 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/hooks/pre-applypatch.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     1643 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/hooks/pre-commit.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      416 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/hooks/pre-merge-commit.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     1374 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/hooks/pre-push.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     4898 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/hooks/pre-rebase.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      544 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/hooks/pre-receive.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     1492 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/hooks/prepare-commit-msg.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     2783 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/hooks/push-to-checkout.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     2308 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/hooks/sendemail-validate.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     3650 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/hooks/update.sample
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/index
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.773414 domain-admin-1.5.8/domain_admin/public/m/.git/info/
--rwxr-xr-x   0 runner    (1001) docker     (123)      240 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/info/exclude
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.773414 domain-admin-1.5.8/domain_admin/public/m/.git/logs/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/logs/HEAD
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.733413 domain-admin-1.5.8/domain_admin/public/m/.git/logs/refs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.773414 domain-admin-1.5.8/domain_admin/public/m/.git/logs/refs/heads/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/logs/refs/heads/dist
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.733413 domain-admin-1.5.8/domain_admin/public/m/.git/logs/refs/remotes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.773414 domain-admin-1.5.8/domain_admin/public/m/.git/logs/refs/remotes/origin/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/logs/refs/remotes/origin/dist
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.733413 domain-admin-1.5.8/domain_admin/public/m/.git/objects/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.773414 domain-admin-1.5.8/domain_admin/public/m/.git/objects/2d/
--r--r--r--   0 runner    (1001) docker     (123)      814 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/objects/2d/7cec3e00ed3b3b835eb233ae4bb2ea21fb5a0b
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.773414 domain-admin-1.5.8/domain_admin/public/m/.git/objects/43/
--r--r--r--   0 runner    (1001) docker     (123)     1262 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/objects/43/c4fcdf29fe10c6256aa4e9cf00f534e6933efc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.773414 domain-admin-1.5.8/domain_admin/public/m/.git/objects/4b/
--r--r--r--   0 runner    (1001) docker     (123)     5351 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/objects/4b/63cfa29bd94b198d895f7a64e10c20f167e65b
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.773414 domain-admin-1.5.8/domain_admin/public/m/.git/objects/5c/
--r--r--r--   0 runner    (1001) docker     (123)       60 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/objects/5c/98d16331bcc99b0cbbe89a3ffb23e3f5918ff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.773414 domain-admin-1.5.8/domain_admin/public/m/.git/objects/61/
--r--r--r--   0 runner    (1001) docker     (123)      421 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/objects/61/05f9fd4f4b11812fcca0d2e0704e4c8dd6e7a3
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.773414 domain-admin-1.5.8/domain_admin/public/m/.git/objects/62/
--r--r--r--   0 runner    (1001) docker     (123)      222 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/objects/62/59838c4de171bc95a934ee2384d626eeb3040a
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.773414 domain-admin-1.5.8/domain_admin/public/m/.git/objects/67/
--r--r--r--   0 runner    (1001) docker     (123)      478 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/objects/67/d2a69f1213016d777c02e0c99a38871d07da5b
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.773414 domain-admin-1.5.8/domain_admin/public/m/.git/objects/6f/
--r--r--r--   0 runner    (1001) docker     (123)      725 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/objects/6f/9d23d38fd97c94c1dccf971fd7b7636cc075d2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.773414 domain-admin-1.5.8/domain_admin/public/m/.git/objects/71/
--r--r--r--   0 runner    (1001) docker     (123)     2231 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/objects/71/4dbccc412b153f5044c269745126581e3cf373
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.777413 domain-admin-1.5.8/domain_admin/public/m/.git/objects/7a/
--r--r--r--   0 runner    (1001) docker     (123)     2494 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/objects/7a/694f3c8aca1586dc6f0e6e9e2773e207992329
--r--r--r--   0 runner    (1001) docker     (123)      968 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/objects/7a/c4cdd0b7c56c8fe9f98aaf044df58bef26b7a5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.777413 domain-admin-1.5.8/domain_admin/public/m/.git/objects/8e/
--r--r--r--   0 runner    (1001) docker     (123)     2655 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/objects/8e/ff5bef00cd2492d9b806988ea99996d636c126
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.777413 domain-admin-1.5.8/domain_admin/public/m/.git/objects/93/
--r--r--r--   0 runner    (1001) docker     (123)     1108 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/objects/93/85587145f9afbabe2aa1a489d24fd1f489e5c6
--r--r--r--   0 runner    (1001) docker     (123)     4673 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/objects/93/db3989e7874cd6b75bc0e984690ffa16666ea6
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.777413 domain-admin-1.5.8/domain_admin/public/m/.git/objects/98/
--r--r--r--   0 runner    (1001) docker     (123)     5141 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/objects/98/1e059e0de4604a5dec80930d8ff7cdf84e0006
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.777413 domain-admin-1.5.8/domain_admin/public/m/.git/objects/a9/
--r--r--r--   0 runner    (1001) docker     (123)     1110 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/objects/a9/a1035a25ce05f60741e3f70716a18d93322203
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.777413 domain-admin-1.5.8/domain_admin/public/m/.git/objects/b0/
--r--r--r--   0 runner    (1001) docker     (123)     1821 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/objects/b0/ecf609c3df960010b6f7877bc379ea45d1e9da
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.777413 domain-admin-1.5.8/domain_admin/public/m/.git/objects/c2/
--r--r--r--   0 runner    (1001) docker     (123)      505 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/objects/c2/c748e84bc4d5118b0e33d6e0073e315a36d034
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.777413 domain-admin-1.5.8/domain_admin/public/m/.git/objects/c7/
--r--r--r--   0 runner    (1001) docker     (123)    31300 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/objects/c7/ef9b19427f9af9e445bb5d63231ccd58ef5b28
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.777413 domain-admin-1.5.8/domain_admin/public/m/.git/objects/c8/
--r--r--r--   0 runner    (1001) docker     (123)   143922 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/objects/c8/bec3f3e9b26642a8221c20a5e422bc2cada687
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.777413 domain-admin-1.5.8/domain_admin/public/m/.git/objects/d9/
--r--r--r--   0 runner    (1001) docker     (123)      119 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/objects/d9/d9ca2809d6994fef91c1ee2d22bc7a54b8b4a5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.777413 domain-admin-1.5.8/domain_admin/public/m/.git/objects/ed/
--r--r--r--   0 runner    (1001) docker     (123)      979 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/objects/ed/50570bc6865f7dff2468d49072d7f4e4cb81d4
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.777413 domain-admin-1.5.8/domain_admin/public/m/.git/objects/f0/
--r--r--r--   0 runner    (1001) docker     (123)      755 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/objects/f0/a3f5a57d6bdb9961c3a56f4a992a08a0ecd671
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.777413 domain-admin-1.5.8/domain_admin/public/m/.git/objects/f8/
--r--r--r--   0 runner    (1001) docker     (123)     1082 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/objects/f8/0169320ed23edd9889e4de7631267635bfec27
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.777413 domain-admin-1.5.8/domain_admin/public/m/.git/objects/fd/
--r--r--r--   0 runner    (1001) docker     (123)     5204 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/objects/fd/bd32c675f85af4ed57021ac0638a21a3c6cad3
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.733413 domain-admin-1.5.8/domain_admin/public/m/.git/refs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.777413 domain-admin-1.5.8/domain_admin/public/m/.git/refs/heads/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/refs/heads/dist
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.733413 domain-admin-1.5.8/domain_admin/public/m/.git/refs/remotes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.777413 domain-admin-1.5.8/domain_admin/public/m/.git/refs/remotes/origin/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/refs/remotes/origin/dist
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/.git/shallow
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.781414 domain-admin-1.5.8/domain_admin/public/m/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/assets/common-c7dd5d89.css
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/assets/common.6194c42f.js
--rw-r--r--   0 runner    (1001) docker     (123)     8065 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/assets/index-5eda257b.css
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/assets/index-958ae3a0.css
--rw-r--r--   0 runner    (1001) docker     (123)   379599 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/assets/index-9c365a03.js
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/assets/index-ad047368.css
--rw-r--r--   0 runner    (1001) docker     (123)     5447 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/assets/index-e8224928.css
--rw-r--r--   0 runner    (1001) docker     (123)    53115 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/assets/index-f79acb3d.css
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/assets/index.1a0d1182.js
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/assets/index.1d067866.js
--rw-r--r--   0 runner    (1001) docker     (123)    10416 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/assets/index.daaf9893.js
--rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/assets/index.feef7c0f.js
--rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/assets/login-cb9f43ad.css
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/assets/pages-cert-list-cert-list.e9ecbf65.js
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/assets/pages-domain-list-domain-list.da5e6454.js
--rw-r--r--   0 runner    (1001) docker     (123)    10670 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/assets/pages-login-login.09426b90.js
--rw-r--r--   0 runner    (1001) docker     (123)    12225 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/assets/pages-user-index-user-index.d8efba8c.js
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/assets/uni.06dd3c8e.css
--rw-r--r--   0 runner    (1001) docker     (123)     9118 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/assets/user-index-be7005ab.css
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.781414 domain-admin-1.5.8/domain_admin/public/m/static/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6334 2023-07-24 15:15:12.000000 domain-admin-1.5.8/domain_admin/public/m/static/user-avatar.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.781414 domain-admin-1.5.8/domain_admin/public/svg/
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-24 15:15:11.000000 domain-admin-1.5.8/domain_admin/public/svg/logo.184a2d7d.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.781414 domain-admin-1.5.8/domain_admin/router/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/router/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7829 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/router/api_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/router/permission.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.785414 domain-admin-1.5.8/domain_admin/service/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/service/async_task_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/service/auth_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/service/common_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/service/domain_info_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    12015 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/service/domain_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/service/file_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/service/group_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/service/group_user_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/service/issue_certificate_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    11701 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/service/notify_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/service/operation_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/service/render_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/service/scheduler_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/service/system_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/service/token_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     8731 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/service/version_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.785414 domain-admin-1.5.8/domain_admin/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    11659 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/templates/cert-email.html
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/templates/cert-export.csv
--rw-r--r--   0 runner    (1001) docker     (123)    10396 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/templates/domain-email.html
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/templates/domain-export.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.785414 domain-admin-1.5.8/domain_admin/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.785414 domain-admin-1.5.8/domain_admin/utils/acme_util/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/acme_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/acme_util/acme_v2_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/bcrypt_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.789414 domain-admin-1.5.8/domain_admin/utils/cert_util/
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/cert_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/cert_util/cert_common.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/cert_util/cert_consts.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/cert_util/cert_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/cert_util/cert_openssl_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/cert_util/cert_socket.py
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/cert_util/cert_socket_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/datetime_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/domain_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/email_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/file_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.789414 domain-admin-1.5.8/domain_admin/utils/flask_ext/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/flask_ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/flask_ext/api_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/flask_ext/app_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/flask_ext/flask_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/flask_ext/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/flask_ext/http_code_enum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.789414 domain-admin-1.5.8/domain_admin/utils/flask_ext/json/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/flask_ext/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/flask_ext/json/default.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/flask_ext/json/json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/flask_ext/json/json_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/flask_ext/register.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/flask_ext/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/icp_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/ip_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/json_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/md5_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.789414 domain-admin-1.5.8/domain_admin/utils/open_api/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/open_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/open_api/crtsh_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/open_api/ding_talk_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/open_api/feishu_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/open_api/work_weixin_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.789414 domain-admin-1.5.8/domain_admin/utils/peewee_ext/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/peewee_ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/peewee_ext/model_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/secret_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/text_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/time_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.789414 domain-admin-1.5.8/domain_admin/utils/whois_util/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/whois_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/whois_util/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/whois_util/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    25912 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/whois_util/whois-servers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/utils/whois_util/whois_util.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      236 2023-07-24 15:14:59.000000 domain-admin-1.5.8/domain_admin/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.737414 domain-admin-1.5.8/domain_admin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18454 2023-07-24 15:15:14.000000 domain-admin-1.5.8/domain_admin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16270 2023-07-24 15:15:14.000000 domain-admin-1.5.8/domain_admin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 15:15:14.000000 domain-admin-1.5.8/domain_admin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-24 15:15:14.000000 domain-admin-1.5.8/domain_admin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-24 15:15:14.000000 domain-admin-1.5.8/domain_admin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 15:15:14.000000 domain-admin-1.5.8/domain_admin.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:15:14.789414 domain-admin-1.5.8/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-24 15:14:59.000000 domain-admin-1.5.8/requirements/production.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 15:15:14.793414 domain-admin-1.5.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3190 2023-07-24 15:14:59.000000 domain-admin-1.5.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.735468 domain-admin-1.5.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-30 05:37:27.000000 domain-admin-1.5.9/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (123)      417 2023-07-30 05:37:27.000000 domain-admin-1.5.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-07-30 05:37:42.735468 domain-admin-1.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-07-30 05:37:27.000000 domain-admin-1.5.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.667468 domain-admin-1.5.9/domain_admin/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.667468 domain-admin-1.5.9/domain_admin/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/api/address_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/api/auth_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/api/cert_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17243 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/api/domain_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16941 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/api/domain_info_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/api/group_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/api/group_user_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/api/host_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/api/ip_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6636 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/api/issue_certificate_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/api/log_async_task_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/api/log_operation_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/api/log_scheduler_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6461 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/api/notify_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/api/prometheus_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/api/system_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/api/user_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/api/whois_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.671468 domain-admin-1.5.9/domain_admin/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/config/default_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/config/env_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/config/runtime_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.671468 domain-admin-1.5.9/domain_admin/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/enums/config_key_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/enums/event_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/enums/notify_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/enums/operation_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/enums/role_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/enums/status_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/enums/version_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.671468 domain-admin-1.5.9/domain_admin/migrate/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/migrate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/migrate/migrate_102_to_103.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/migrate/migrate_106_to_110.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/migrate/migrate_110_to_1212.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/migrate/migrate_1212_to_1213.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/migrate/migrate_1213_to_131.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/migrate/migrate_136_to_140_alpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/migrate/migrate_140_alpha_to_140.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/migrate/migrate_1413_to_1414.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/migrate/migrate_1422_to_1423.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/migrate/migrate_143_to_144.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/migrate/migrate_145_to_146.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/migrate/migrate_151_to_152.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/migrate/migrate_154_to_155.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/migrate/migrate_158_to_159.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/migrate/migrate_common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.675468 domain-admin-1.5.9/domain_admin/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/model/address_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/model/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/model/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/model/domain_info_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/model/domain_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/model/group_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/model/group_user_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/model/host_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/model/issue_certificate_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/model/log_async_task_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/model/log_operation_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/model/log_scheduler_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/model/notify_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/model/system_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/model/user_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/model/version_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.675468 domain-admin-1.5.9/domain_admin/public/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.675468 domain-admin-1.5.9/domain_admin/public/.git/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/.git/FETCH_HEAD
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/.git/HEAD
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/.git/config
+-rwxr-xr-x   0 runner    (1001) docker     (123)       73 2023-07-30 05:37:38.000000 domain-admin-1.5.9/domain_admin/public/.git/description
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.675468 domain-admin-1.5.9/domain_admin/public/.git/hooks/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      478 2023-07-30 05:37:38.000000 domain-admin-1.5.9/domain_admin/public/.git/hooks/applypatch-msg.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      896 2023-07-30 05:37:38.000000 domain-admin-1.5.9/domain_admin/public/.git/hooks/commit-msg.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4726 2023-07-30 05:37:38.000000 domain-admin-1.5.9/domain_admin/public/.git/hooks/fsmonitor-watchman.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      189 2023-07-30 05:37:38.000000 domain-admin-1.5.9/domain_admin/public/.git/hooks/post-update.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      424 2023-07-30 05:37:38.000000 domain-admin-1.5.9/domain_admin/public/.git/hooks/pre-applypatch.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1643 2023-07-30 05:37:38.000000 domain-admin-1.5.9/domain_admin/public/.git/hooks/pre-commit.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      416 2023-07-30 05:37:38.000000 domain-admin-1.5.9/domain_admin/public/.git/hooks/pre-merge-commit.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1374 2023-07-30 05:37:38.000000 domain-admin-1.5.9/domain_admin/public/.git/hooks/pre-push.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4898 2023-07-30 05:37:38.000000 domain-admin-1.5.9/domain_admin/public/.git/hooks/pre-rebase.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      544 2023-07-30 05:37:38.000000 domain-admin-1.5.9/domain_admin/public/.git/hooks/pre-receive.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1492 2023-07-30 05:37:38.000000 domain-admin-1.5.9/domain_admin/public/.git/hooks/prepare-commit-msg.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2783 2023-07-30 05:37:38.000000 domain-admin-1.5.9/domain_admin/public/.git/hooks/push-to-checkout.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2308 2023-07-30 05:37:38.000000 domain-admin-1.5.9/domain_admin/public/.git/hooks/sendemail-validate.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3650 2023-07-30 05:37:38.000000 domain-admin-1.5.9/domain_admin/public/.git/hooks/update.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/.git/index
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.679468 domain-admin-1.5.9/domain_admin/public/.git/info/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      240 2023-07-30 05:37:38.000000 domain-admin-1.5.9/domain_admin/public/.git/info/exclude
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.679468 domain-admin-1.5.9/domain_admin/public/.git/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/.git/logs/HEAD
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.655468 domain-admin-1.5.9/domain_admin/public/.git/logs/refs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.679468 domain-admin-1.5.9/domain_admin/public/.git/logs/refs/heads/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/.git/logs/refs/heads/dist
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.655468 domain-admin-1.5.9/domain_admin/public/.git/logs/refs/remotes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.679468 domain-admin-1.5.9/domain_admin/public/.git/logs/refs/remotes/origin/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/.git/logs/refs/remotes/origin/dist
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.659468 domain-admin-1.5.9/domain_admin/public/.git/objects/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.679468 domain-admin-1.5.9/domain_admin/public/.git/objects/00/
+-r--r--r--   0 runner    (1001) docker     (123)     8844 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/.git/objects/00/f7c6e2fba3e12bc14ab61c148b4ba2a64e38a3
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.679468 domain-admin-1.5.9/domain_admin/public/.git/objects/19/
+-r--r--r--   0 runner    (1001) docker     (123)    64350 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/.git/objects/19/7f5cf73cf11d43d915904e0d8aad4736a77d63
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.679468 domain-admin-1.5.9/domain_admin/public/.git/objects/21/
+-r--r--r--   0 runner    (1001) docker     (123)       61 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/.git/objects/21/00bd7d2219a26827cc80aa37fe72fcb303bb50
+-r--r--r--   0 runner    (1001) docker     (123)     1893 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/.git/objects/21/39b81dcd444515633d19490097a6b348cde5c5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.679468 domain-admin-1.5.9/domain_admin/public/.git/objects/25/
+-r--r--r--   0 runner    (1001) docker     (123)      228 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/.git/objects/25/295734aef0855e20af49f3eeabf0b66868f6ba
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.679468 domain-admin-1.5.9/domain_admin/public/.git/objects/28/
+-r--r--r--   0 runner    (1001) docker     (123)     1815 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/.git/objects/28/f9bf1d51da58ca27d653eb24726bf24710ad77
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.679468 domain-admin-1.5.9/domain_admin/public/.git/objects/29/
+-r--r--r--   0 runner    (1001) docker     (123)      637 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/.git/objects/29/a4c85c52713f69636b86696e2d2c46f10a6da0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.679468 domain-admin-1.5.9/domain_admin/public/.git/objects/2d/
+-r--r--r--   0 runner    (1001) docker     (123)     4250 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/.git/objects/2d/8a41ec985b9d8eae83de5d090acfcfc3c41242
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.679468 domain-admin-1.5.9/domain_admin/public/.git/objects/2e/
+-r--r--r--   0 runner    (1001) docker     (123)      314 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/.git/objects/2e/ae458563637ec44c6387b9169f3abfdb3e6c29
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.679468 domain-admin-1.5.9/domain_admin/public/.git/objects/3c/
+-r--r--r--   0 runner    (1001) docker     (123)     3081 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/.git/objects/3c/0f2e923566dc74d04e67d46d8b722923ed1949
+-r--r--r--   0 runner    (1001) docker     (123)   148706 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/.git/objects/3c/2434ab20d756f0a95ad24f6a5adb7e1219a7d1
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.679468 domain-admin-1.5.9/domain_admin/public/.git/objects/43/
+-r--r--r--   0 runner    (1001) docker     (123)      200 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/.git/objects/43/cf76d02df6959240541fad0a582a256c9d1d9f
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.679468 domain-admin-1.5.9/domain_admin/public/.git/objects/52/
+-r--r--r--   0 runner    (1001) docker     (123)    62564 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/.git/objects/52/c1926de72b181c9b7faf597fb8f71f48565462
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.679468 domain-admin-1.5.9/domain_admin/public/.git/objects/55/
+-r--r--r--   0 runner    (1001) docker     (123)      119 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/.git/objects/55/1103b11c4b699a3b4107d3a2ab173dfe238556
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.679468 domain-admin-1.5.9/domain_admin/public/.git/objects/59/
+-r--r--r--   0 runner    (1001) docker     (123)      466 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/.git/objects/59/7a1712f21c02c83dc657e1eb2287fcbba0b692
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.679468 domain-admin-1.5.9/domain_admin/public/.git/objects/5f/
+-r--r--r--   0 runner    (1001) docker     (123)      530 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/.git/objects/5f/a7faf700c98850aa96022ab07af6a07b854f34
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.679468 domain-admin-1.5.9/domain_admin/public/.git/objects/69/
+-r--r--r--   0 runner    (1001) docker     (123)   279936 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/.git/objects/69/a9dda41cf39bb60d1dc5b1158ffba197580b6a
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.679468 domain-admin-1.5.9/domain_admin/public/.git/objects/6a/
+-r--r--r--   0 runner    (1001) docker     (123)      172 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/.git/objects/6a/6a1ab9b562bb27239abdcdf8e1a772761b4dee
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.683468 domain-admin-1.5.9/domain_admin/public/.git/objects/6c/
+-r--r--r--   0 runner    (1001) docker     (123)      155 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/.git/objects/6c/3e3059f9ec00c015681abca34b751c3439513d
+-r--r--r--   0 runner    (1001) docker     (123)      475 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/.git/objects/6c/eb074240765b4f5dba74a28f57ff96fa54f33c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.683468 domain-admin-1.5.9/domain_admin/public/.git/objects/6d/
+-r--r--r--   0 runner    (1001) docker     (123)      612 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/.git/objects/6d/15191314c9b832ac41056a30bf0bf6533a29dc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.683468 domain-admin-1.5.9/domain_admin/public/.git/objects/6f/
+-r--r--r--   0 runner    (1001) docker     (123)      694 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/.git/objects/6f/0100c1cf8791c558a0116b7ca1e59de431ee28
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.683468 domain-admin-1.5.9/domain_admin/public/.git/objects/72/
+-r--r--r--   0 runner    (1001) docker     (123)     1433 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/.git/objects/72/d994916434598d7948b1adb0815369eccbd518
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.683468 domain-admin-1.5.9/domain_admin/public/.git/objects/75/
+-r--r--r--   0 runner    (1001) docker     (123)     7633 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/.git/objects/75/d9dfaadcdfe57a016666775b36754ff77ec7d4
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.683468 domain-admin-1.5.9/domain_admin/public/.git/objects/79/
+-r--r--r--   0 runner    (1001) docker     (123)   105817 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/.git/objects/79/404c2464172f80b414d111f49718327b3ef93b
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.683468 domain-admin-1.5.9/domain_admin/public/.git/objects/7f/
+-r--r--r--   0 runner    (1001) docker     (123)      368 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/.git/objects/7f/64d8af0501887e805dc9ccf8228f4fb5e73fdb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.683468 domain-admin-1.5.9/domain_admin/public/.git/objects/85/
+-r--r--r--   0 runner    (1001) docker     (123)    11700 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/.git/objects/85/33870af4bccab767938338b23bf5d1ef5b3f3b
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.683468 domain-admin-1.5.9/domain_admin/public/.git/objects/89/
+-r--r--r--   0 runner    (1001) docker     (123)      106 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/.git/objects/89/0f3ed83973272c63b56a722a88fe25160d11d2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.683468 domain-admin-1.5.9/domain_admin/public/.git/objects/8c/
+-r--r--r--   0 runner    (1001) docker     (123)     1700 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/.git/objects/8c/c916b983bc8c1f7df16b9f5741cfad4d2a4fcc
+-r--r--r--   0 runner    (1001) docker     (123)       69 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/.git/objects/8c/f880f5a9481ef71cd22e08d59e7d366775b360
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.683468 domain-admin-1.5.9/domain_admin/public/.git/objects/91/
+-r--r--r--   0 runner    (1001) docker     (123)     1022 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/.git/objects/91/886bd903574b0bfe9b1ba9364bb716a6b8757b
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.683468 domain-admin-1.5.9/domain_admin/public/.git/objects/95/
+-r--r--r--   0 runner    (1001) docker     (123)      118 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/.git/objects/95/f07af46d709638b20c0b2c66cdf6de8e89a7e4
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.683468 domain-admin-1.5.9/domain_admin/public/.git/objects/9a/
+-r--r--r--   0 runner    (1001) docker     (123)    17968 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/.git/objects/9a/395cf124caea477b9f8061fbf89228b989a948
+-r--r--r--   0 runner    (1001) docker     (123)      177 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/.git/objects/9a/4e8fcc1912f0c1af9a1836ebd9847d8b0e3118
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.683468 domain-admin-1.5.9/domain_admin/public/.git/objects/9e/
+-r--r--r--   0 runner    (1001) docker     (123)     2690 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/.git/objects/9e/0266769577ed8db9863f40a1ce18c97e9c85ca
+-r--r--r--   0 runner    (1001) docker     (123)     5817 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/.git/objects/9e/16d5586b2b1ccd986fa841aadcf150ccf4ccf3
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.683468 domain-admin-1.5.9/domain_admin/public/.git/objects/a1/
+-r--r--r--   0 runner    (1001) docker     (123)      222 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/.git/objects/a1/13e44b9d9526cfc9b780807dbca0935bcbc9ad
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.683468 domain-admin-1.5.9/domain_admin/public/.git/objects/ad/
+-r--r--r--   0 runner    (1001) docker     (123)     1024 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/.git/objects/ad/38c27c881e48722da8bb9bc7f410189a334108
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.683468 domain-admin-1.5.9/domain_admin/public/.git/objects/b3/
+-r--r--r--   0 runner    (1001) docker     (123)    41902 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/.git/objects/b3/1cb2667f48424e34cf9517362eadf899f704ad
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.683468 domain-admin-1.5.9/domain_admin/public/.git/objects/c1/
+-r--r--r--   0 runner    (1001) docker     (123)     6011 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/.git/objects/c1/9a2a5676c89fe224b74ec4fb000399048d1a78
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.683468 domain-admin-1.5.9/domain_admin/public/.git/objects/c4/
+-r--r--r--   0 runner    (1001) docker     (123)       61 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/.git/objects/c4/c46ae2c464a49661d7793709077759039f0b5e
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.687468 domain-admin-1.5.9/domain_admin/public/.git/objects/cc/
+-r--r--r--   0 runner    (1001) docker     (123)   361458 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/.git/objects/cc/bfeaa0b21986ed309cbb83d17585b54f3b2fb9
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.687468 domain-admin-1.5.9/domain_admin/public/.git/objects/e1/
+-r--r--r--   0 runner    (1001) docker     (123)    23927 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/.git/objects/e1/13bfd922675ce50e68cdf88cd94d16130ad58b
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.687468 domain-admin-1.5.9/domain_admin/public/.git/objects/e6/
+-r--r--r--   0 runner    (1001) docker     (123)     1737 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/.git/objects/e6/327e057f2a2d4a5a57f21379f407da0db060e2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.687468 domain-admin-1.5.9/domain_admin/public/.git/objects/f1/
+-r--r--r--   0 runner    (1001) docker     (123)    45439 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/.git/objects/f1/9692949226c296834afeb8669582e799d94a3f
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.687468 domain-admin-1.5.9/domain_admin/public/.git/objects/f3/
+-r--r--r--   0 runner    (1001) docker     (123)     3443 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/.git/objects/f3/fe7436cf05ee53d3fe361b83e4e9d498a8c106
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.687468 domain-admin-1.5.9/domain_admin/public/.git/objects/fd/
+-r--r--r--   0 runner    (1001) docker     (123)     5204 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/.git/objects/fd/bd32c675f85af4ed57021ac0638a21a3c6cad3
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.687468 domain-admin-1.5.9/domain_admin/public/.git/objects/ff/
+-r--r--r--   0 runner    (1001) docker     (123)    13943 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/.git/objects/ff/9c65dfdc7a16150c07745e0030a9d6373920cd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.659468 domain-admin-1.5.9/domain_admin/public/.git/refs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.687468 domain-admin-1.5.9/domain_admin/public/.git/refs/heads/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/.git/refs/heads/dist
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.659468 domain-admin-1.5.9/domain_admin/public/.git/refs/remotes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.687468 domain-admin-1.5.9/domain_admin/public/.git/refs/remotes/origin/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/.git/refs/remotes/origin/dist
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/.git/shallow
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.687468 domain-admin-1.5.9/domain_admin/public/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/css/ConditionFilterGroup.a91875e6.css
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/css/index.26827e91.css
+-rw-r--r--   0 runner    (1001) docker     (123)   331526 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/css/index.69a97337.css
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/css/index.a676cc2e.css
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/css/index.b285e10a.css
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/css/index.cf805e1c.css
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/css/index.d028ae37.css
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/css/index.e21504c8.css
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15406 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.687468 domain-admin-1.5.9/domain_admin/public/gif/
+-rw-r--r--   0 runner    (1001) docker     (123)     6334 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/gif/user-avatar.ea67286d.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.687468 domain-admin-1.5.9/domain_admin/public/jpg/
+-rw-r--r--   0 runner    (1001) docker     (123)    14271 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/jpg/chatpet-white.10f4f36c.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    24940 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/jpg/chatpet.fce5580e.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.699468 domain-admin-1.5.9/domain_admin/public/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    18591 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/js/ConditionFilterGroup.8b8592a5.js
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/js/ConnectStatus.8f8cc994.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/js/SearchUser.8714bea9.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/js/SelectGroup.e46bb885.js
+-rw-r--r--   0 runner    (1001) docker     (123)   390997 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/js/codemirror-lib.a3a39aa0.js
+-rw-r--r--   0 runner    (1001) docker     (123)   195335 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/js/element-icon.1ce1c350.js
+-rw-r--r--   0 runner    (1001) docker     (123)   749914 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/js/element-plus.30eb1cab.js
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/js/event-enums.6c6f25e7.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1058329 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/js/highlight-lib.3654f6d3.js
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/js/highlight-util.a4f1867f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/js/index.006f8a9f.js
+-rw-r--r--   0 runner    (1001) docker     (123)    39589 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/js/index.0bc39ff5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/js/index.1cd93e88.js
+-rw-r--r--   0 runner    (1001) docker     (123)    28081 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/js/index.22cdc255.js
+-rw-r--r--   0 runner    (1001) docker     (123)   132683 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/js/index.34d377d3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8982 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/js/index.435ed104.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9882 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/js/index.47fd0142.js
+-rw-r--r--   0 runner    (1001) docker     (123)    67289 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/js/index.5c3a2f20.js
+-rw-r--r--   0 runner    (1001) docker     (123)    21499 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/js/index.61002253.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/js/index.8410f64d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/js/index.ab4c92d7.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/js/index.b9d6d972.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/js/index.bc114a13.js
+-rw-r--r--   0 runner    (1001) docker     (123)    28958 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/js/index.c1800b79.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9652 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/js/index.e0890673.js
+-rw-r--r--   0 runner    (1001) docker     (123)   312580 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/js/vendor-lib.76301fc3.js
+-rw-r--r--   0 runner    (1001) docker     (123)    94202 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/js/vendor-vue.9e61e0af.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.699468 domain-admin-1.5.9/domain_admin/public/m/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.703468 domain-admin-1.5.9/domain_admin/public/m/.git/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/.git/FETCH_HEAD
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/.git/HEAD
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/.git/config
+-rwxr-xr-x   0 runner    (1001) docker     (123)       73 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/.git/description
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.703468 domain-admin-1.5.9/domain_admin/public/m/.git/hooks/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      478 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/.git/hooks/applypatch-msg.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      896 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/.git/hooks/commit-msg.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4726 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/.git/hooks/fsmonitor-watchman.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      189 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/.git/hooks/post-update.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      424 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/.git/hooks/pre-applypatch.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1643 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/.git/hooks/pre-commit.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      416 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/.git/hooks/pre-merge-commit.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1374 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/.git/hooks/pre-push.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4898 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/.git/hooks/pre-rebase.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      544 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/.git/hooks/pre-receive.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1492 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/.git/hooks/prepare-commit-msg.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2783 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/.git/hooks/push-to-checkout.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2308 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/.git/hooks/sendemail-validate.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3650 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/.git/hooks/update.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/.git/index
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.703468 domain-admin-1.5.9/domain_admin/public/m/.git/info/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      240 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/.git/info/exclude
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.707468 domain-admin-1.5.9/domain_admin/public/m/.git/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/.git/logs/HEAD
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.659468 domain-admin-1.5.9/domain_admin/public/m/.git/logs/refs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.707468 domain-admin-1.5.9/domain_admin/public/m/.git/logs/refs/heads/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/.git/logs/refs/heads/dist
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.663468 domain-admin-1.5.9/domain_admin/public/m/.git/logs/refs/remotes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.707468 domain-admin-1.5.9/domain_admin/public/m/.git/logs/refs/remotes/origin/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/.git/logs/refs/remotes/origin/dist
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.663468 domain-admin-1.5.9/domain_admin/public/m/.git/objects/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.707468 domain-admin-1.5.9/domain_admin/public/m/.git/objects/2d/
+-r--r--r--   0 runner    (1001) docker     (123)      814 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/.git/objects/2d/7cec3e00ed3b3b835eb233ae4bb2ea21fb5a0b
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.707468 domain-admin-1.5.9/domain_admin/public/m/.git/objects/43/
+-r--r--r--   0 runner    (1001) docker     (123)     1262 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/.git/objects/43/c4fcdf29fe10c6256aa4e9cf00f534e6933efc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.707468 domain-admin-1.5.9/domain_admin/public/m/.git/objects/4b/
+-r--r--r--   0 runner    (1001) docker     (123)     5351 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/.git/objects/4b/63cfa29bd94b198d895f7a64e10c20f167e65b
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.707468 domain-admin-1.5.9/domain_admin/public/m/.git/objects/5c/
+-r--r--r--   0 runner    (1001) docker     (123)       60 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/.git/objects/5c/98d16331bcc99b0cbbe89a3ffb23e3f5918ff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.707468 domain-admin-1.5.9/domain_admin/public/m/.git/objects/61/
+-r--r--r--   0 runner    (1001) docker     (123)      421 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/.git/objects/61/05f9fd4f4b11812fcca0d2e0704e4c8dd6e7a3
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.707468 domain-admin-1.5.9/domain_admin/public/m/.git/objects/62/
+-r--r--r--   0 runner    (1001) docker     (123)      222 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/.git/objects/62/59838c4de171bc95a934ee2384d626eeb3040a
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.707468 domain-admin-1.5.9/domain_admin/public/m/.git/objects/67/
+-r--r--r--   0 runner    (1001) docker     (123)      478 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/.git/objects/67/d2a69f1213016d777c02e0c99a38871d07da5b
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.707468 domain-admin-1.5.9/domain_admin/public/m/.git/objects/6f/
+-r--r--r--   0 runner    (1001) docker     (123)      725 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/.git/objects/6f/9d23d38fd97c94c1dccf971fd7b7636cc075d2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.707468 domain-admin-1.5.9/domain_admin/public/m/.git/objects/71/
+-r--r--r--   0 runner    (1001) docker     (123)     2231 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/.git/objects/71/4dbccc412b153f5044c269745126581e3cf373
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.707468 domain-admin-1.5.9/domain_admin/public/m/.git/objects/7a/
+-r--r--r--   0 runner    (1001) docker     (123)     2494 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/.git/objects/7a/694f3c8aca1586dc6f0e6e9e2773e207992329
+-r--r--r--   0 runner    (1001) docker     (123)      968 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/.git/objects/7a/c4cdd0b7c56c8fe9f98aaf044df58bef26b7a5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.707468 domain-admin-1.5.9/domain_admin/public/m/.git/objects/8e/
+-r--r--r--   0 runner    (1001) docker     (123)     2655 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/.git/objects/8e/ff5bef00cd2492d9b806988ea99996d636c126
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.707468 domain-admin-1.5.9/domain_admin/public/m/.git/objects/93/
+-r--r--r--   0 runner    (1001) docker     (123)     1108 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/.git/objects/93/85587145f9afbabe2aa1a489d24fd1f489e5c6
+-r--r--r--   0 runner    (1001) docker     (123)     4673 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/.git/objects/93/db3989e7874cd6b75bc0e984690ffa16666ea6
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.707468 domain-admin-1.5.9/domain_admin/public/m/.git/objects/98/
+-r--r--r--   0 runner    (1001) docker     (123)     5141 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/.git/objects/98/1e059e0de4604a5dec80930d8ff7cdf84e0006
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.707468 domain-admin-1.5.9/domain_admin/public/m/.git/objects/a9/
+-r--r--r--   0 runner    (1001) docker     (123)     1110 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/.git/objects/a9/a1035a25ce05f60741e3f70716a18d93322203
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.707468 domain-admin-1.5.9/domain_admin/public/m/.git/objects/b0/
+-r--r--r--   0 runner    (1001) docker     (123)     1821 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/.git/objects/b0/ecf609c3df960010b6f7877bc379ea45d1e9da
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.711468 domain-admin-1.5.9/domain_admin/public/m/.git/objects/c2/
+-r--r--r--   0 runner    (1001) docker     (123)      505 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/.git/objects/c2/c748e84bc4d5118b0e33d6e0073e315a36d034
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.711468 domain-admin-1.5.9/domain_admin/public/m/.git/objects/c7/
+-r--r--r--   0 runner    (1001) docker     (123)    31300 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/.git/objects/c7/ef9b19427f9af9e445bb5d63231ccd58ef5b28
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.711468 domain-admin-1.5.9/domain_admin/public/m/.git/objects/c8/
+-r--r--r--   0 runner    (1001) docker     (123)   143922 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/.git/objects/c8/bec3f3e9b26642a8221c20a5e422bc2cada687
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.711468 domain-admin-1.5.9/domain_admin/public/m/.git/objects/d9/
+-r--r--r--   0 runner    (1001) docker     (123)      119 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/.git/objects/d9/d9ca2809d6994fef91c1ee2d22bc7a54b8b4a5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.711468 domain-admin-1.5.9/domain_admin/public/m/.git/objects/ed/
+-r--r--r--   0 runner    (1001) docker     (123)      979 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/.git/objects/ed/50570bc6865f7dff2468d49072d7f4e4cb81d4
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.711468 domain-admin-1.5.9/domain_admin/public/m/.git/objects/f0/
+-r--r--r--   0 runner    (1001) docker     (123)      755 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/.git/objects/f0/a3f5a57d6bdb9961c3a56f4a992a08a0ecd671
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.711468 domain-admin-1.5.9/domain_admin/public/m/.git/objects/f8/
+-r--r--r--   0 runner    (1001) docker     (123)     1082 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/.git/objects/f8/0169320ed23edd9889e4de7631267635bfec27
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.711468 domain-admin-1.5.9/domain_admin/public/m/.git/objects/fd/
+-r--r--r--   0 runner    (1001) docker     (123)     5204 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/.git/objects/fd/bd32c675f85af4ed57021ac0638a21a3c6cad3
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.663468 domain-admin-1.5.9/domain_admin/public/m/.git/refs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.711468 domain-admin-1.5.9/domain_admin/public/m/.git/refs/heads/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/.git/refs/heads/dist
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.663468 domain-admin-1.5.9/domain_admin/public/m/.git/refs/remotes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.711468 domain-admin-1.5.9/domain_admin/public/m/.git/refs/remotes/origin/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/.git/refs/remotes/origin/dist
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/.git/shallow
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.719468 domain-admin-1.5.9/domain_admin/public/m/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/assets/common-c7dd5d89.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/assets/common.6194c42f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8065 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/assets/index-5eda257b.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/assets/index-958ae3a0.css
+-rw-r--r--   0 runner    (1001) docker     (123)   379599 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/assets/index-9c365a03.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/assets/index-ad047368.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5447 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/assets/index-e8224928.css
+-rw-r--r--   0 runner    (1001) docker     (123)    53115 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/assets/index-f79acb3d.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/assets/index.1a0d1182.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/assets/index.1d067866.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10416 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/assets/index.daaf9893.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/assets/index.feef7c0f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/assets/login-cb9f43ad.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/assets/pages-cert-list-cert-list.e9ecbf65.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/assets/pages-domain-list-domain-list.da5e6454.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10670 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/assets/pages-login-login.09426b90.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12225 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/assets/pages-user-index-user-index.d8efba8c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/assets/uni.06dd3c8e.css
+-rw-r--r--   0 runner    (1001) docker     (123)     9118 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/assets/user-index-be7005ab.css
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.719468 domain-admin-1.5.9/domain_admin/public/m/static/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6334 2023-07-30 05:37:40.000000 domain-admin-1.5.9/domain_admin/public/m/static/user-avatar.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.719468 domain-admin-1.5.9/domain_admin/public/svg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-30 05:37:39.000000 domain-admin-1.5.9/domain_admin/public/svg/logo.184a2d7d.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.719468 domain-admin-1.5.9/domain_admin/router/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/router/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8526 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/router/api_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/router/permission.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.723468 domain-admin-1.5.9/domain_admin/service/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/service/async_task_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/service/auth_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/service/common_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/service/domain_info_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12015 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/service/domain_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/service/file_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/service/group_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/service/group_user_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9139 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/service/issue_certificate_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11701 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/service/notify_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/service/operation_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/service/render_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/service/scheduler_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/service/system_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/service/token_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9186 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/service/version_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.723468 domain-admin-1.5.9/domain_admin/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    11659 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/templates/cert-email.html
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/templates/cert-export.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    10396 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/templates/domain-email.html
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/templates/domain-export.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.727468 domain-admin-1.5.9/domain_admin/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.727468 domain-admin-1.5.9/domain_admin/utils/acme_util/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/utils/acme_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8232 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/utils/acme_util/acme_v2_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/utils/acme_util/challenge_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/utils/bcrypt_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.727468 domain-admin-1.5.9/domain_admin/utils/cert_util/
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/utils/cert_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/utils/cert_util/cert_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/utils/cert_util/cert_consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/utils/cert_util/cert_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/utils/cert_util/cert_openssl_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/utils/cert_util/cert_socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/utils/cert_util/cert_socket_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/utils/datetime_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/utils/domain_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/utils/email_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/utils/fabric_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/utils/file_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.731468 domain-admin-1.5.9/domain_admin/utils/flask_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/utils/flask_ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/utils/flask_ext/api_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/utils/flask_ext/app_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/utils/flask_ext/flask_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/utils/flask_ext/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/utils/flask_ext/http_code_enum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.731468 domain-admin-1.5.9/domain_admin/utils/flask_ext/json/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/utils/flask_ext/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/utils/flask_ext/json/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/utils/flask_ext/json/json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/utils/flask_ext/json/json_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/utils/flask_ext/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/utils/flask_ext/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/utils/icp_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/utils/ip_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/utils/json_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/utils/md5_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.731468 domain-admin-1.5.9/domain_admin/utils/open_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/utils/open_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/utils/open_api/crtsh_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/utils/open_api/ding_talk_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/utils/open_api/feishu_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/utils/open_api/work_weixin_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.731468 domain-admin-1.5.9/domain_admin/utils/peewee_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/utils/peewee_ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/utils/peewee_ext/model_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/utils/secret_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/utils/text_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/utils/time_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.735468 domain-admin-1.5.9/domain_admin/utils/whois_util/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/utils/whois_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/utils/whois_util/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/utils/whois_util/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25912 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/utils/whois_util/whois-servers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/utils/whois_util/whois_util.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      236 2023-07-30 05:37:27.000000 domain-admin-1.5.9/domain_admin/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.667468 domain-admin-1.5.9/domain_admin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-07-30 05:37:42.000000 domain-admin-1.5.9/domain_admin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16456 2023-07-30 05:37:42.000000 domain-admin-1.5.9/domain_admin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 05:37:42.000000 domain-admin-1.5.9/domain_admin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-30 05:37:42.000000 domain-admin-1.5.9/domain_admin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-30 05:37:42.000000 domain-admin-1.5.9/domain_admin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 05:37:42.000000 domain-admin-1.5.9/domain_admin.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:37:42.735468 domain-admin-1.5.9/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-30 05:37:27.000000 domain-admin-1.5.9/requirements/production.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 05:37:42.735468 domain-admin-1.5.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3190 2023-07-30 05:37:27.000000 domain-admin-1.5.9/setup.py
```

### Comparing `domain-admin-1.5.8/LICENSE` & `domain-admin-1.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/api/address_api.py` & `domain-admin-1.5.9/domain_admin/api/address_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/api/auth_api.py` & `domain-admin-1.5.9/domain_admin/api/auth_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/api/cert_api.py` & `domain-admin-1.5.9/domain_admin/api/cert_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/api/domain_api.py` & `domain-admin-1.5.9/domain_admin/api/domain_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/api/domain_info_api.py` & `domain-admin-1.5.9/domain_admin/api/domain_info_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/api/group_api.py` & `domain-admin-1.5.9/domain_admin/api/group_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/api/group_user_api.py` & `domain-admin-1.5.9/domain_admin/api/group_user_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/api/log_async_task_api.py` & `domain-admin-1.5.9/domain_admin/api/log_async_task_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/api/log_operation_api.py` & `domain-admin-1.5.9/domain_admin/api/log_operation_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/api/log_scheduler_api.py` & `domain-admin-1.5.9/domain_admin/api/log_scheduler_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/api/notify_api.py` & `domain-admin-1.5.9/domain_admin/api/notify_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/api/prometheus_api.py` & `domain-admin-1.5.9/domain_admin/api/prometheus_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/api/system_api.py` & `domain-admin-1.5.9/domain_admin/api/system_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/api/user_api.py` & `domain-admin-1.5.9/domain_admin/api/user_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/api/whois_api.py` & `domain-admin-1.5.9/domain_admin/api/whois_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/compat.py` & `domain-admin-1.5.9/domain_admin/compat.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/config/default_config.py` & `domain-admin-1.5.9/domain_admin/config/default_config.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/config/env_config.py` & `domain-admin-1.5.9/domain_admin/config/env_config.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/config/runtime_config.py` & `domain-admin-1.5.9/domain_admin/config/runtime_config.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/enums/config_key_enum.py` & `domain-admin-1.5.9/domain_admin/enums/config_key_enum.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/enums/operation_enum.py` & `domain-admin-1.5.9/domain_admin/enums/operation_enum.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/enums/version_enum.py` & `domain-admin-1.5.9/domain_admin/enums/version_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,7 +117,11 @@
     Version_150 = '1.5.0'
     Version_151 = '1.5.1'
     Version_152 = '1.5.2'
 
     Version_153 = '1.5.3'
     Version_154 = '1.5.4'
     Version_155 = '1.5.5'
+    Version_156 = '1.5.6'
+    Version_157 = '1.5.7'
+    Version_158 = '1.5.8'
+    Version_159 = '1.5.9'
```

### Comparing `domain-admin-1.5.8/domain_admin/log.py` & `domain-admin-1.5.9/domain_admin/log.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/main.py` & `domain-admin-1.5.9/domain_admin/main.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/migrate/migrate_102_to_103.py` & `domain-admin-1.5.9/domain_admin/migrate/migrate_102_to_103.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/migrate/migrate_106_to_110.py` & `domain-admin-1.5.9/domain_admin/migrate/migrate_106_to_110.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/migrate/migrate_110_to_1212.py` & `domain-admin-1.5.9/domain_admin/migrate/migrate_110_to_1212.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/migrate/migrate_1212_to_1213.py` & `domain-admin-1.5.9/domain_admin/migrate/migrate_1212_to_1213.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/migrate/migrate_1213_to_131.py` & `domain-admin-1.5.9/domain_admin/migrate/migrate_1213_to_131.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/migrate/migrate_136_to_140_alpha.py` & `domain-admin-1.5.9/domain_admin/migrate/migrate_136_to_140_alpha.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/migrate/migrate_140_alpha_to_140.py` & `domain-admin-1.5.9/domain_admin/migrate/migrate_140_alpha_to_140.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/migrate/migrate_1413_to_1414.py` & `domain-admin-1.5.9/domain_admin/migrate/migrate_1413_to_1414.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/migrate/migrate_1422_to_1423.py` & `domain-admin-1.5.9/domain_admin/migrate/migrate_1422_to_1423.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/migrate/migrate_143_to_144.py` & `domain-admin-1.5.9/domain_admin/migrate/migrate_143_to_144.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/migrate/migrate_145_to_146.py` & `domain-admin-1.5.9/domain_admin/migrate/migrate_145_to_146.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/migrate/migrate_151_to_152.py` & `domain-admin-1.5.9/domain_admin/migrate/migrate_151_to_152.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/migrate/migrate_154_to_155.py` & `domain-admin-1.5.9/domain_admin/migrate/migrate_154_to_155.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/migrate/migrate_common.py` & `domain-admin-1.5.9/domain_admin/migrate/migrate_common.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/model/address_model.py` & `domain-admin-1.5.9/domain_admin/model/address_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/model/base_model.py` & `domain-admin-1.5.9/domain_admin/model/base_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/model/database.py` & `domain-admin-1.5.9/domain_admin/model/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # -*- coding: utf-8 -*-
 """
 database.py
 """
 from __future__ import print_function, unicode_literals, absolute_import, division
+
 from domain_admin.log import logger
 from domain_admin.model import address_model, log_operation_model, group_user_model, log_async_task_model, \
-    issue_certificate_model
+    issue_certificate_model, host_model
 from domain_admin.model import domain_info_model
 from domain_admin.model import domain_model
 from domain_admin.model import group_model
 from domain_admin.model import log_scheduler_model
 from domain_admin.model import notify_model
 from domain_admin.model import system_model
 from domain_admin.model import user_model
@@ -27,14 +28,15 @@
     (notify_model.NotifyModel, None),
     (address_model.AddressModel, None),
     (domain_info_model.DomainInfoModel, None),
     (log_operation_model.LogOperationModel, None),
     (group_user_model.GroupUserModel, None),
     (log_async_task_model.AsyncTaskModel, None),
     (issue_certificate_model.IssueCertificateModel, None),
+    (host_model.HostModel, None),
 ]
 
 
 def init_database():
     """
     初始化数据表
     :return:
```

### Comparing `domain-admin-1.5.8/domain_admin/model/domain_info_model.py` & `domain-admin-1.5.9/domain_admin/model/domain_info_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/model/domain_model.py` & `domain-admin-1.5.9/domain_admin/model/domain_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/model/group_model.py` & `domain-admin-1.5.9/domain_admin/model/group_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/model/group_user_model.py` & `domain-admin-1.5.9/domain_admin/model/group_user_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/model/issue_certificate_model.py` & `domain-admin-1.5.9/domain_admin/model/issue_certificate_model.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,59 +3,84 @@
 issue_certificate_model.py
 """
 from __future__ import print_function, unicode_literals, absolute_import, division
 
 import json
 from datetime import datetime
 
-from peewee import CharField, IntegerField, DateTimeField, BooleanField, AutoField, TextField
+from peewee import CharField, IntegerField, DateTimeField, AutoField, TextField, BooleanField
 
 from domain_admin.model.base_model import BaseModel
-from domain_admin.utils import datetime_util, time_util
+from domain_admin.utils import datetime_util
+from domain_admin.utils.acme_util.challenge_type import ChallengeType
 
 URI_ROOT_PATH = ".well-known/acme-challenge"
 
 
 class IssueCertificateModel(BaseModel):
     """
     申请证书
     @since v1.5.6
     """
     id = AutoField(primary_key=True)
 
     # 用户id
     user_id = IntegerField(default=0)
 
-    # 域名列表
-    domain_raw = TextField()
-
     # SSL证书
     ssl_certificate = TextField(default=None, null=True)
 
     # SSL证书私钥
     ssl_certificate_key = TextField(default=None, null=True)
 
+    # 域名列表
+    domain_raw = TextField(default='')
+
+    # 验证类型 http dns
+    challenge_type = CharField(default=ChallengeType.HTTP01, null=True)
+
     # 域名验证token
+    # @Deprecation @since v1.5.9
     token = CharField(default=None, null=True)
 
     # 域名验证数据
+    # @Deprecation @since v1.5.9
     validation = CharField(default=None, null=True)
 
     # 验证状态url
+    # @Deprecation @since v1.5.9
     status_url = CharField(default=None, null=True)
 
     # 验证状态 valid pending
-    status = CharField(default=None, null=True)
+    status = CharField(default='pending', null=True)
 
     # SSL签发时间
     start_time = DateTimeField(default=None, null=True)
 
     # SSL过期时间
     expire_time = DateTimeField(default=None, null=True)
 
+    # 部署机器
+    deploy_host_id = IntegerField(default=0)
+
+    # 验证文件部署目录
+    deploy_verify_path = CharField(default=None, null=True)
+
+    # key部署路径
+    deploy_key_file = CharField(default=None, null=True)
+
+    # pem部署路径
+    deploy_fullchain_file = CharField(default=None, null=True)
+
+    # 部署重启命令
+    deploy_reloadcmd = CharField(default=None, null=True)
+
+    # 自动续期
+    is_auto_renew = BooleanField(default=False)
+
     # 创建时间
     create_time = DateTimeField(default=datetime.now)
 
     # 更新时间
     update_time = DateTimeField(default=datetime.now)
 
     class Meta:
@@ -82,14 +107,18 @@
 
     @property
     def challenge_url(self):
         return '/.well-known/acme-challenge/{}'.format(self.token)
 
     @property
     def domains(self):
-        return json.loads(self.domain_raw)
+        if self.domain_raw:
+            return json.loads(self.domain_raw)
+        else:
+            return []
 
     @property
     def domain_validation_urls(self):
-        return [
-            "http://" + domain + '/' + URI_ROOT_PATH + '/' + self.token
-            for domain in self.domains]
+        return []
+
+        # ["http://" + domain + '/' + URI_ROOT_PATH + '/' + self.token
+        # for domain in self.domains]
```

### Comparing `domain-admin-1.5.8/domain_admin/model/log_async_task_model.py` & `domain-admin-1.5.9/domain_admin/model/log_async_task_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/model/log_operation_model.py` & `domain-admin-1.5.9/domain_admin/model/log_operation_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/model/log_scheduler_model.py` & `domain-admin-1.5.9/domain_admin/model/log_scheduler_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/model/notify_model.py` & `domain-admin-1.5.9/domain_admin/model/notify_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/model/system_model.py` & `domain-admin-1.5.9/domain_admin/model/system_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/model/user_model.py` & `domain-admin-1.5.9/domain_admin/model/user_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/model/version_model.py` & `domain-admin-1.5.9/domain_admin/model/version_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/.git/hooks/commit-msg.sample` & `domain-admin-1.5.9/domain_admin/public/.git/hooks/commit-msg.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/.git/hooks/fsmonitor-watchman.sample` & `domain-admin-1.5.9/domain_admin/public/.git/hooks/fsmonitor-watchman.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/.git/hooks/pre-commit.sample` & `domain-admin-1.5.9/domain_admin/public/.git/hooks/pre-commit.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/.git/hooks/pre-push.sample` & `domain-admin-1.5.9/domain_admin/public/.git/hooks/pre-push.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/.git/hooks/pre-rebase.sample` & `domain-admin-1.5.9/domain_admin/public/.git/hooks/pre-rebase.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/.git/hooks/pre-receive.sample` & `domain-admin-1.5.9/domain_admin/public/.git/hooks/pre-receive.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/.git/hooks/prepare-commit-msg.sample` & `domain-admin-1.5.9/domain_admin/public/.git/hooks/prepare-commit-msg.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/.git/hooks/push-to-checkout.sample` & `domain-admin-1.5.9/domain_admin/public/.git/hooks/push-to-checkout.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/.git/hooks/sendemail-validate.sample` & `domain-admin-1.5.9/domain_admin/public/.git/hooks/sendemail-validate.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/.git/hooks/update.sample` & `domain-admin-1.5.9/domain_admin/public/.git/hooks/update.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/.git/index` & `domain-admin-1.5.9/domain_admin/public/.git/index`

 * *Files 25% similar despite different names*

#### Comparing `/tmp/diffoscope_qbugsoku_/tmplj56_24m_TarContainer/0/97` & `/tmp/diffoscope_qbugsoku_/tmpxabcs3im_TarContainer/0/100`

```diff
@@ -5,452 +5,452 @@
 
 Path:      b'css/ConditionFilterGroup.a91875e6.css'
 SHA:       5fa7faf700c98850aa96022ab07af6a07b854f34
 Size:      1601
 Flags:     0b100101
 User ID:   1001
 Group ID:  123
-Created:   1690211711.837343906
-Modified:  1690211711.837343906
-Inode:     300730
+Created:   1690695459.891455610
+Modified:  1690695459.891455610
+Inode:     300565
 Device ID: (8, 1)
 
-Path:      b'css/index.302e10d7.css'
-SHA:       92cfface0a460c51331fb8f25083a09948e00cbf
+Path:      b'css/index.26827e91.css'
+SHA:       43cf76d02df6959240541fad0a582a256c9d1d9f
 Size:      301
 Flags:     0b10110
 User ID:   1001
 Group ID:  123
-Created:   1690211711.837343906
-Modified:  1690211711.837343906
-Inode:     300731
+Created:   1690695459.891455610
+Modified:  1690695459.891455610
+Inode:     300566
 Device ID: (8, 1)
 
 Path:      b'css/index.69a97337.css'
 SHA:       197f5cf73cf11d43d915904e0d8aad4736a77d63
 Size:      331526
 Flags:     0b10110
 User ID:   1001
 Group ID:  123
-Created:   1690211711.841344312
-Modified:  1690211711.841344312
-Inode:     300732
-Device ID: (8, 1)
-
-Path:      b'css/index.93c714bb.css'
-SHA:       716b5718c659ed5a85d4f93a2cf25fc5ff5031cb
-Size:      111
-Flags:     0b10110
-User ID:   1001
-Group ID:  123
-Created:   1690211711.841344312
-Modified:  1690211711.841344312
-Inode:     300733
+Created:   1690695459.895455628
+Modified:  1690695459.895455628
+Inode:     300567
 Device ID: (8, 1)
 
 Path:      b'css/index.a676cc2e.css'
 SHA:       551103b11c4b699a3b4107d3a2ab173dfe238556
 Size:      117
 Flags:     0b10110
 User ID:   1001
 Group ID:  123
-Created:   1690211711.841344312
-Modified:  1690211711.841344312
-Inode:     300734
+Created:   1690695459.895455628
+Modified:  1690695459.895455628
+Inode:     300568
 Device ID: (8, 1)
 
 Path:      b'css/index.b285e10a.css'
 SHA:       6c3e3059f9ec00c015681abca34b751c3439513d
 Size:      250
 Flags:     0b10110
 User ID:   1001
 Group ID:  123
-Created:   1690211711.841344312
-Modified:  1690211711.841344312
-Inode:     300735
+Created:   1690695459.895455628
+Modified:  1690695459.895455628
+Inode:     300569
 Device ID: (8, 1)
 
 Path:      b'css/index.cf805e1c.css'
 SHA:       95f07af46d709638b20c0b2c66cdf6de8e89a7e4
 Size:      117
 Flags:     0b10110
 User ID:   1001
 Group ID:  123
-Created:   1690211711.841344312
-Modified:  1690211711.841344312
-Inode:     300736
+Created:   1690695459.895455628
+Modified:  1690695459.895455628
+Inode:     300570
 Device ID: (8, 1)
 
 Path:      b'css/index.d028ae37.css'
 SHA:       c4c46ae2c464a49661d7793709077759039f0b5e
 Size:      45
 Flags:     0b10110
 User ID:   1001
 Group ID:  123
-Created:   1690211711.841344312
-Modified:  1690211711.841344312
-Inode:     300737
+Created:   1690695459.895455628
+Modified:  1690695459.895455628
+Inode:     300571
+Device ID: (8, 1)
+
+Path:      b'css/index.e21504c8.css'
+SHA:       6a6a1ab9b562bb27239abdcdf8e1a772761b4dee
+Size:      316
+Flags:     0b10110
+User ID:   1001
+Group ID:  123
+Created:   1690695459.895455628
+Modified:  1690695459.895455628
+Inode:     300572
 Device ID: (8, 1)
 
 Path:      b'favicon.ico'
 SHA:       3c0f2e923566dc74d04e67d46d8b722923ed1949
 Size:      15406
 Flags:     0b1011
 User ID:   1001
 Group ID:  123
-Created:   1690211711.841344312
-Modified:  1690211711.841344312
-Inode:     300738
+Created:   1690695459.895455628
+Modified:  1690695459.895455628
+Inode:     300573
 Device ID: (8, 1)
 
 Path:      b'gif/user-avatar.ea67286d.gif'
 SHA:       fdbd32c675f85af4ed57021ac0638a21a3c6cad3
 Size:      6334
 Flags:     0b11100
 User ID:   1001
 Group ID:  123
-Created:   1690211711.841344312
-Modified:  1690211711.841344312
-Inode:     300740
+Created:   1690695459.895455628
+Modified:  1690695459.895455628
+Inode:     300575
 Device ID: (8, 1)
 
 Path:      b'index.html'
-SHA:       60727d43f26f701780e7c55e90cb084973a1be9e
+SHA:       597a1712f21c02c83dc657e1eb2287fcbba0b692
 Size:      911
 Flags:     0b1010
 User ID:   1001
 Group ID:  123
-Created:   1690211711.841344312
-Modified:  1690211711.841344312
-Inode:     300741
+Created:   1690695459.895455628
+Modified:  1690695459.895455628
+Inode:     300576
 Device ID: (8, 1)
 
 Path:      b'jpg/chatpet-white.10f4f36c.jpg'
 SHA:       ff9c65dfdc7a16150c07745e0030a9d6373920cd
 Size:      14271
 Flags:     0b11110
 User ID:   1001
 Group ID:  123
-Created:   1690211711.841344312
-Modified:  1690211711.841344312
-Inode:     300743
+Created:   1690695459.895455628
+Modified:  1690695459.895455628
+Inode:     300578
 Device ID: (8, 1)
 
 Path:      b'jpg/chatpet.fce5580e.jpg'
 SHA:       e113bfd922675ce50e68cdf88cd94d16130ad58b
 Size:      24940
 Flags:     0b11000
 User ID:   1001
 Group ID:  123
-Created:   1690211711.841344312
-Modified:  1690211711.841344312
-Inode:     300744
+Created:   1690695459.895455628
+Modified:  1690695459.895455628
+Inode:     300579
 Device ID: (8, 1)
 
-Path:      b'js/ConditionFilterGroup.3c6ac067.js'
-SHA:       88eed16a647060a310c6f8fd8cbf109ad11d1211
+Path:      b'js/ConditionFilterGroup.8b8592a5.js'
+SHA:       9e16d5586b2b1ccd986fa841aadcf150ccf4ccf3
 Size:      18591
 Flags:     0b100011
 User ID:   1001
 Group ID:  123
-Created:   1690211711.841344312
-Modified:  1690211711.841344312
-Inode:     300746
+Created:   1690695459.895455628
+Modified:  1690695459.895455628
+Inode:     300581
 Device ID: (8, 1)
 
-Path:      b'js/ConnectStatus.a429b01b.js'
-SHA:       e98d4dd298d6c05d0bfa2fbe9182ec7cddde7926
+Path:      b'js/ConnectStatus.8f8cc994.js'
+SHA:       6ceb074240765b4f5dba74a28f57ff96fa54f33c
 Size:      953
 Flags:     0b11100
 User ID:   1001
 Group ID:  123
-Created:   1690211711.841344312
-Modified:  1690211711.841344312
-Inode:     300747
+Created:   1690695459.895455628
+Modified:  1690695459.895455628
+Inode:     300582
 Device ID: (8, 1)
 
-Path:      b'js/SearchUser.f8e52158.js'
-SHA:       e6e9c9b85a9477efa2c8f05874bd09fa93a6b34c
+Path:      b'js/SearchUser.8714bea9.js'
+SHA:       29a4c85c52713f69636b86696e2d2c46f10a6da0
 Size:      1105
 Flags:     0b11001
 User ID:   1001
 Group ID:  123
-Created:   1690211711.841344312
-Modified:  1690211711.841344312
-Inode:     300748
+Created:   1690695459.895455628
+Modified:  1690695459.895455628
+Inode:     300583
 Device ID: (8, 1)
 
-Path:      b'js/SelectGroup.53d83114.js'
-SHA:       f978f4b33c1fdc0cb74f1df45d0fc049f5da1c89
+Path:      b'js/SelectGroup.e46bb885.js'
+SHA:       6f0100c1cf8791c558a0116b7ca1e59de431ee28
 Size:      1257
 Flags:     0b11010
 User ID:   1001
 Group ID:  123
-Created:   1690211711.841344312
-Modified:  1690211711.841344312
-Inode:     300749
+Created:   1690695459.895455628
+Modified:  1690695459.895455628
+Inode:     300584
 Device ID: (8, 1)
 
 Path:      b'js/codemirror-lib.a3a39aa0.js'
 SHA:       3c2434ab20d756f0a95ad24f6a5adb7e1219a7d1
 Size:      390997
 Flags:     0b11101
 User ID:   1001
 Group ID:  123
-Created:   1690211711.845344719
-Modified:  1690211711.845344719
-Inode:     300750
+Created:   1690695459.899455645
+Modified:  1690695459.899455645
+Inode:     300585
 Device ID: (8, 1)
 
 Path:      b'js/element-icon.1ce1c350.js'
 SHA:       52c1926de72b181c9b7faf597fb8f71f48565462
 Size:      195335
 Flags:     0b11011
 User ID:   1001
 Group ID:  123
-Created:   1690211711.845344719
-Modified:  1690211711.845344719
-Inode:     300751
+Created:   1690695459.899455645
+Modified:  1690695459.899455645
+Inode:     300586
 Device ID: (8, 1)
 
 Path:      b'js/element-plus.30eb1cab.js'
 SHA:       69a9dda41cf39bb60d1dc5b1158ffba197580b6a
 Size:      749914
 Flags:     0b11011
 User ID:   1001
 Group ID:  123
-Created:   1690211711.849345125
-Modified:  1690211711.849345125
-Inode:     300752
+Created:   1690695459.903455663
+Modified:  1690695459.903455663
+Inode:     300587
 Device ID: (8, 1)
 
 Path:      b'js/event-enums.6c6f25e7.js'
 SHA:       7f64d8af0501887e805dc9ccf8228f4fb5e73fdb
 Size:      579
 Flags:     0b11010
 User ID:   1001
 Group ID:  123
-Created:   1690211711.849345125
-Modified:  1690211711.849345125
-Inode:     300753
+Created:   1690695459.903455663
+Modified:  1690695459.903455663
+Inode:     300588
 Device ID: (8, 1)
 
 Path:      b'js/highlight-lib.3654f6d3.js'
 SHA:       ccbfeaa0b21986ed309cbb83d17585b54f3b2fb9
 Size:      1058329
 Flags:     0b11100
 User ID:   1001
 Group ID:  123
-Created:   1690211711.857345938
-Modified:  1690211711.857345938
-Inode:     300754
+Created:   1690695459.911455699
+Modified:  1690695459.911455699
+Inode:     300589
 Device ID: (8, 1)
 
 Path:      b'js/highlight-util.a4f1867f.js'
 SHA:       9a4e8fcc1912f0c1af9a1836ebd9847d8b0e3118
 Size:      289
 Flags:     0b11101
 User ID:   1001
 Group ID:  123
-Created:   1690211711.857345938
-Modified:  1690211711.857345938
-Inode:     300755
+Created:   1690695459.911455699
+Modified:  1690695459.911455699
+Inode:     300590
 Device ID: (8, 1)
 
-Path:      b'js/index.0963ab53.js'
-SHA:       ae1c9a7def175d7a6389679bf822a6a9219c3ca3
-Size:      4603
+Path:      b'js/index.006f8a9f.js'
+SHA:       ad38c27c881e48722da8bb9bc7f410189a334108
+Size:      1818
 Flags:     0b10100
 User ID:   1001
 Group ID:  123
-Created:   1690211711.857345938
-Modified:  1690211711.857345938
-Inode:     300756
+Created:   1690695459.911455699
+Modified:  1690695459.911455699
+Inode:     300591
 Device ID: (8, 1)
 
-Path:      b'js/index.0d4c27ce.js'
-SHA:       57bd1a9bfce972b50e5efecf11f71a3f5b2ec3d3
-Size:      15553
+Path:      b'js/index.0bc39ff5.js'
+SHA:       8533870af4bccab767938338b23bf5d1ef5b3f3b
+Size:      39589
 Flags:     0b10100
 User ID:   1001
 Group ID:  123
-Created:   1690211711.857345938
-Modified:  1690211711.857345938
-Inode:     300757
+Created:   1690695459.911455699
+Modified:  1690695459.911455699
+Inode:     300592
 Device ID: (8, 1)
 
-Path:      b'js/index.165f9ce1.js'
-SHA:       7c7a565bed760068496030f030f2b05ede1bec4b
-Size:      64712
+Path:      b'js/index.1cd93e88.js'
+SHA:       28f9bf1d51da58ca27d653eb24726bf24710ad77
+Size:      4603
 Flags:     0b10100
 User ID:   1001
 Group ID:  123
-Created:   1690211711.857345938
-Modified:  1690211711.857345938
-Inode:     300758
+Created:   1690695459.911455699
+Modified:  1690695459.911455699
+Inode:     300593
 Device ID: (8, 1)
 
-Path:      b'js/index.24e255af.js'
-SHA:       fbac0b57e4138b4fca9c9f5babf558611a38e6d0
+Path:      b'js/index.22cdc255.js'
+SHA:       75d9dfaadcdfe57a016666775b36754ff77ec7d4
 Size:      28081
 Flags:     0b10100
 User ID:   1001
 Group ID:  123
-Created:   1690211711.857345938
-Modified:  1690211711.857345938
-Inode:     300759
+Created:   1690695459.911455699
+Modified:  1690695459.911455699
+Inode:     300594
 Device ID: (8, 1)
 
-Path:      b'js/index.2ab02c40.js'
-SHA:       32dd3b54be707f423bd7375381bbc2baede37f8c
-Size:      2691
+Path:      b'js/index.34d377d3.js'
+SHA:       f19692949226c296834afeb8669582e799d94a3f
+Size:      132683
 Flags:     0b10100
 User ID:   1001
 Group ID:  123
-Created:   1690211711.857345938
-Modified:  1690211711.857345938
-Inode:     300760
+Created:   1690695459.915455717
+Modified:  1690695459.915455717
+Inode:     300595
 Device ID: (8, 1)
 
-Path:      b'js/index.3b5a616c.js'
-SHA:       d25bbe60e329a2e662af042df10825c9dcdc3887
-Size:      1818
+Path:      b'js/index.435ed104.js'
+SHA:       9e0266769577ed8db9863f40a1ce18c97e9c85ca
+Size:      8982
 Flags:     0b10100
 User ID:   1001
 Group ID:  123
-Created:   1690211711.857345938
-Modified:  1690211711.857345938
-Inode:     300761
+Created:   1690695459.915455717
+Modified:  1690695459.915455717
+Inode:     300596
 Device ID: (8, 1)
 
-Path:      b'js/index.5b4cd516.js'
-SHA:       c93d3f53fd06fdbc8587e3a8f37876356c5cdb56
-Size:      8982
+Path:      b'js/index.47fd0142.js'
+SHA:       2d8a41ec985b9d8eae83de5d090acfcfc3c41242
+Size:      9882
 Flags:     0b10100
 User ID:   1001
 Group ID:  123
-Created:   1690211711.857345938
-Modified:  1690211711.857345938
-Inode:     300762
+Created:   1690695459.915455717
+Modified:  1690695459.915455717
+Inode:     300597
 Device ID: (8, 1)
 
-Path:      b'js/index.5f8ece3f.js'
-SHA:       3e24054f5e3a680f56b9276efe009e73b7133a99
-Size:      4248
+Path:      b'js/index.5c3a2f20.js'
+SHA:       9a395cf124caea477b9f8061fbf89228b989a948
+Size:      67289
 Flags:     0b10100
 User ID:   1001
 Group ID:  123
-Created:   1690211711.857345938
-Modified:  1690211711.857345938
-Inode:     300763
+Created:   1690695459.915455717
+Modified:  1690695459.915455717
+Inode:     300598
 Device ID: (8, 1)
 
-Path:      b'js/index.654f7830.js'
-SHA:       3711576f2b615224b9477da0a0a9a43c17539d12
-Size:      4147
+Path:      b'js/index.61002253.js'
+SHA:       c19a2a5676c89fe224b74ec4fb000399048d1a78
+Size:      21499
 Flags:     0b10100
 User ID:   1001
 Group ID:  123
-Created:   1690211711.857345938
-Modified:  1690211711.857345938
-Inode:     300764
+Created:   1690695459.915455717
+Modified:  1690695459.915455717
+Inode:     300599
 Device ID: (8, 1)
 
-Path:      b'js/index.8c31b31b.js'
-SHA:       a749320e6e50d7593d7d1d30ee0159023cd4e422
-Size:      9882
+Path:      b'js/index.8410f64d.js'
+SHA:       e6327e057f2a2d4a5a57f21379f407da0db060e2
+Size:      4248
 Flags:     0b10100
 User ID:   1001
 Group ID:  123
-Created:   1690211711.857345938
-Modified:  1690211711.857345938
-Inode:     300765
+Created:   1690695459.915455717
+Modified:  1690695459.915455717
+Inode:     300600
 Device ID: (8, 1)
 
-Path:      b'js/index.a8bb8abf.js'
-SHA:       a56b22c2eacca280122dde700a98068ebdd8c5af
-Size:      39363
+Path:      b'js/index.ab4c92d7.js'
+SHA:       8cc916b983bc8c1f7df16b9f5741cfad4d2a4fcc
+Size:      4147
 Flags:     0b10100
 User ID:   1001
 Group ID:  123
-Created:   1690211711.857345938
-Modified:  1690211711.857345938
-Inode:     300766
+Created:   1690695459.915455717
+Modified:  1690695459.915455717
+Inode:     300601
 Device ID: (8, 1)
 
-Path:      b'js/index.af06b2dc.js'
-SHA:       4bf6af202944cd3e22f8a375977737ce52b17763
-Size:      28958
+Path:      b'js/index.b9d6d972.js'
+SHA:       72d994916434598d7948b1adb0815369eccbd518
+Size:      2691
 Flags:     0b10100
 User ID:   1001
 Group ID:  123
-Created:   1690211711.857345938
-Modified:  1690211711.857345938
-Inode:     300767
+Created:   1690695459.915455717
+Modified:  1690695459.915455717
+Inode:     300602
 Device ID: (8, 1)
 
-Path:      b'js/index.c22f6489.js'
-SHA:       6cf21ee6e3a69b2e234f6012f1636e3621d25db8
-Size:      21499
+Path:      b'js/index.bc114a13.js'
+SHA:       2139b81dcd444515633d19490097a6b348cde5c5
+Size:      5241
 Flags:     0b10100
 User ID:   1001
 Group ID:  123
-Created:   1690211711.857345938
-Modified:  1690211711.857345938
-Inode:     300768
+Created:   1690695459.915455717
+Modified:  1690695459.915455717
+Inode:     300603
 Device ID: (8, 1)
 
-Path:      b'js/index.deff2c63.js'
-SHA:       9a44f010e55bd5cd3a7d60bcd86ee9b8e7ef2cef
-Size:      9652
+Path:      b'js/index.c1800b79.js'
+SHA:       00f7c6e2fba3e12bc14ab61c148b4ba2a64e38a3
+Size:      28958
 Flags:     0b10100
 User ID:   1001
 Group ID:  123
-Created:   1690211711.857345938
-Modified:  1690211711.857345938
-Inode:     300769
+Created:   1690695459.915455717
+Modified:  1690695459.915455717
+Inode:     300604
 Device ID: (8, 1)
 
-Path:      b'js/index.ef82c865.js'
-SHA:       8f3fc862ebdfdd80953e51ae5e44e7862b79ad63
-Size:      5241
+Path:      b'js/index.e0890673.js'
+SHA:       f3fe7436cf05ee53d3fe361b83e4e9d498a8c106
+Size:      9652
 Flags:     0b10100
 User ID:   1001
 Group ID:  123
-Created:   1690211711.861346345
-Modified:  1690211711.861346345
-Inode:     300770
+Created:   1690695459.915455717
+Modified:  1690695459.915455717
+Inode:     300605
 Device ID: (8, 1)
 
 Path:      b'js/vendor-lib.76301fc3.js'
 SHA:       79404c2464172f80b414d111f49718327b3ef93b
 Size:      312580
 Flags:     0b11001
 User ID:   1001
 Group ID:  123
-Created:   1690211711.861346345
-Modified:  1690211711.861346345
-Inode:     300771
+Created:   1690695459.919455734
+Modified:  1690695459.919455734
+Inode:     300606
 Device ID: (8, 1)
 
 Path:      b'js/vendor-vue.9e61e0af.js'
 SHA:       b31cb2667f48424e34cf9517362eadf899f704ad
 Size:      94202
 Flags:     0b11001
 User ID:   1001
 Group ID:  123
-Created:   1690211711.861346345
-Modified:  1690211711.861346345
-Inode:     300772
+Created:   1690695459.919455734
+Modified:  1690695459.919455734
+Inode:     300607
 Device ID: (8, 1)
 
 Path:      b'svg/logo.184a2d7d.svg'
 SHA:       6d15191314c9b832ac41056a30bf0bf6533a29dc
 Size:      1478
 Flags:     0b10101
 User ID:   1001
 Group ID:  123
-Created:   1690211711.861346345
-Modified:  1690211711.861346345
-Inode:     300774
+Created:   1690695459.919455734
+Modified:  1690695459.919455734
+Inode:     300609
 Device ID: (8, 1)
```

### Comparing `domain-admin-1.5.8/domain_admin/public/.git/objects/19/7f5cf73cf11d43d915904e0d8aad4736a77d63` & `domain-admin-1.5.9/domain_admin/public/.git/objects/19/7f5cf73cf11d43d915904e0d8aad4736a77d63`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/.git/objects/3c/0f2e923566dc74d04e67d46d8b722923ed1949` & `domain-admin-1.5.9/domain_admin/public/.git/objects/3c/0f2e923566dc74d04e67d46d8b722923ed1949`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/.git/objects/3c/2434ab20d756f0a95ad24f6a5adb7e1219a7d1` & `domain-admin-1.5.9/domain_admin/public/.git/objects/3c/2434ab20d756f0a95ad24f6a5adb7e1219a7d1`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/.git/objects/52/c1926de72b181c9b7faf597fb8f71f48565462` & `domain-admin-1.5.9/domain_admin/public/.git/objects/52/c1926de72b181c9b7faf597fb8f71f48565462`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/.git/objects/5f/a7faf700c98850aa96022ab07af6a07b854f34` & `domain-admin-1.5.9/domain_admin/public/.git/objects/5f/a7faf700c98850aa96022ab07af6a07b854f34`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/.git/objects/69/a9dda41cf39bb60d1dc5b1158ffba197580b6a` & `domain-admin-1.5.9/domain_admin/public/.git/objects/69/a9dda41cf39bb60d1dc5b1158ffba197580b6a`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/.git/objects/6d/15191314c9b832ac41056a30bf0bf6533a29dc` & `domain-admin-1.5.9/domain_admin/public/.git/objects/6d/15191314c9b832ac41056a30bf0bf6533a29dc`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/.git/objects/79/404c2464172f80b414d111f49718327b3ef93b` & `domain-admin-1.5.9/domain_admin/public/.git/objects/79/404c2464172f80b414d111f49718327b3ef93b`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/.git/objects/b3/1cb2667f48424e34cf9517362eadf899f704ad` & `domain-admin-1.5.9/domain_admin/public/.git/objects/b3/1cb2667f48424e34cf9517362eadf899f704ad`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/.git/objects/cc/bfeaa0b21986ed309cbb83d17585b54f3b2fb9` & `domain-admin-1.5.9/domain_admin/public/.git/objects/cc/bfeaa0b21986ed309cbb83d17585b54f3b2fb9`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/.git/objects/e1/13bfd922675ce50e68cdf88cd94d16130ad58b` & `domain-admin-1.5.9/domain_admin/public/.git/objects/e1/13bfd922675ce50e68cdf88cd94d16130ad58b`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/.git/objects/fb/ac0b57e4138b4fca9c9f5babf558611a38e6d0` & `domain-admin-1.5.9/domain_admin/public/.git/objects/75/d9dfaadcdfe57a016666775b36754ff77ec7d4`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 00000050: b2d4 e8d4 3af5 fff1 a7f3 304a 965e c98b  ....:.....0J.^..
 00000060: 4b7d fb92 2edf db43 babc b447 74f9 60f7  K}.....C...Gt.`.
 00000070: e9f2 83cd e8f2 d36a 1c85 53cb d961 d76c  .......j..S..a.l
 00000080: 9654 d96c 318d 9df6 b03d 6eb4 d89e f32e  .T.l1....=n.....
 00000090: b60e 6481 a794 faaf 7642 97bf d921 5d8e  ..d.....vB...!].
 000000a0: ec77 74f9 bb2a 6218 8ed8 d48f a230 aa06  .wt..*b......0..
 000000b0: fea5 e3ed 7abb fb9e 5733 4bb9 a00c 6f54  ....z...W3K...oT
-000000c0: 067f 3662 1f9d 7abb 35de 1fb2 ba99 ce9b  ..6b..z.5.......
-000000d0: 5042 5f7c e7d2 7e41 771f edbf d2e5 1fa2  PB_|..~Aw.......
-000000e0: 3527 f61b ba0b ed97 7499 d9bc c173 9b57  5'......t....s.W
-000000f0: f3da f622 7afa c2fe 1b5d 7eb6 0774 796b  ..."z....]~..tyk
-00000100: 7b1d babe b35f d1e5 9ff6 095d 0eed d774  {...._.....]...t
-00000110: 79af ea04 318c d080 eb05 73f6 59bb ce6a  y...1.....s.Y..j
-00000120: ded8 a818 092a 6053 1295 3f0c 674e 1df5  .....*`S..?.gN..
-00000130: 1eee b6cc 3622 892c 8384 b0d7 dead d5c7  ....6".,........
+000000c0: 067f 3662 1f9d d670 d76b 8c1b 9974 de84  ..6b...p.k...t..
+000000d0: 12fa e23b 97f6 0bba fb68 ff95 2eff 10ad  ...;.....h......
+000000e0: 39b1 dfd0 5d68 bfa4 cbcc e60d 9edb bc9a  9...]h..........
+000000f0: d7b6 17d1 d317 f6df e8f2 b33d a0cb 5bdb  ...........=..[.
+00000100: ebd0 f59d fd8a 2eff b44f e872 68bf a6cb  .........O.rh...
+00000110: 7b55 2788 6184 065c 2f98 b3cf da75 56f3  {U'.a..\/....uV.
+00000120: c646 0348 5001 9b92 a8fc 6138 73ea 4356  .F.HP.....a8s.CV
+00000130: 1fee b6cc ba23 892c 8384 b0d7 dead d5c7  .....#.,........
 00000140: c3dd fc32 e6c1 2276 766b ecb2 3ef4 2e79  ...2.."vvk..>..y
 00000150: 1214 1a27 25c6 bacb 38f1 9245 ec9e 2da7  ...'%...8..E..-.
 00000160: 2c8e bd2b e65a bf2c f61a 47ed 5f16 ed5a  ,..+.Z.,..G._..Z
 00000170: adfe cba2 d9af 1dff b2e8 d406 f8bf d9df  ................
 00000180: 3dc4 dbc3 bd43 cb8e d887 851f b191 fba8  =....C..........
 00000190: 6627 917f 75c5 22d7 ba0c 1691 b53a b7af  f'..u."......:..
 000001a0: bd60 c1b2 65ee d7ea 9477 afdf fa65 b15f  .`..e....w...e._
@@ -470,9 +470,9 @@
 00001d50: 193d 9ada 2865 b757 b141 13f9 9999 2aa5  .=..(e.W.A....*.
 00001d60: b550 2c5d 8dc9 51be 7ec9 df9a 1324 2f85  .P,]..Q.~....$/.
 00001d70: 1253 2980 4bf2 e80d 5fbd 8228 a5b1 3624  .S).K..._..(..6$
 00001d80: c8eb 0b11 521e 51e1 b58f 7320 6d16 23e6  ....R.Q...s m.#.
 00001d90: 7060 dd7b cde1 7abf 8c57 316b b278 5d37  p`.{..z..W1k.x]7
 00001da0: a76c a8aa ec55 a3c2 7abe 3614 8843 3519  .l...U..z.6..C5.
 00001db0: 972d 4930 533f cecc d43f d04c 7d00 4a07  .-I0S?...?.L}.J.
-00001dc0: ad58 26fc 4fa8 4998 b83a f8e6 5fbf c383  .X&.O.I..:.._...
-00001dd0: 38                                       8
+00001dc0: ad58 26fc 4fa8 4998 b83a f8e6 5fca a383  .X&.O.I..:.._...
+00001dd0: 2a                                       *
```

### Comparing `domain-admin-1.5.8/domain_admin/public/.git/objects/fd/bd32c675f85af4ed57021ac0638a21a3c6cad3` & `domain-admin-1.5.9/domain_admin/public/.git/objects/fd/bd32c675f85af4ed57021ac0638a21a3c6cad3`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/.git/objects/ff/9c65dfdc7a16150c07745e0030a9d6373920cd` & `domain-admin-1.5.9/domain_admin/public/.git/objects/ff/9c65dfdc7a16150c07745e0030a9d6373920cd`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/css/ConditionFilterGroup.a91875e6.css` & `domain-admin-1.5.9/domain_admin/public/css/ConditionFilterGroup.a91875e6.css`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/css/index.69a97337.css` & `domain-admin-1.5.9/domain_admin/public/css/index.69a97337.css`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/favicon.ico` & `domain-admin-1.5.9/domain_admin/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/gif/user-avatar.ea67286d.gif` & `domain-admin-1.5.9/domain_admin/public/gif/user-avatar.ea67286d.gif`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/jpg/chatpet-white.10f4f36c.jpg` & `domain-admin-1.5.9/domain_admin/public/jpg/chatpet-white.10f4f36c.jpg`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/jpg/chatpet.fce5580e.jpg` & `domain-admin-1.5.9/domain_admin/public/jpg/chatpet.fce5580e.jpg`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/js/ConditionFilterGroup.3c6ac067.js` & `domain-admin-1.5.9/domain_admin/public/js/ConditionFilterGroup.8b8592a5.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,14 @@
 import {
     d as O
 } from "./element-plus.30eb1cab.js";
 import {
     _ as D,
     R as E
-} from "./index.165f9ce1.js";
+} from "./index.5c3a2f20.js";
 import {
     o as d,
     c as u,
     J as I,
     U as w,
     ah as l,
     V as n,
```

### Comparing `domain-admin-1.5.8/domain_admin/public/js/ConnectStatus.a429b01b.js` & `domain-admin-1.5.9/domain_admin/public/js/ConnectStatus.8f8cc994.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 import {
     _
-} from "./index.165f9ce1.js";
+} from "./index.5c3a2f20.js";
 import {
     ah as n,
     o as a,
     O as s,
     P as e,
     V as l
 } from "./vendor-vue.9e61e0af.js";
```

### Comparing `domain-admin-1.5.8/domain_admin/public/js/SearchUser.f8e52158.js` & `domain-admin-1.5.9/domain_admin/public/js/SearchUser.8714bea9.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 import {
     _ as l
-} from "./index.165f9ce1.js";
+} from "./index.5c3a2f20.js";
 import {
     ah as c,
     o as d,
     O as i
 } from "./vendor-vue.9e61e0af.js";
 const u = {
     name: "SearchUser",
```

### Comparing `domain-admin-1.5.8/domain_admin/public/js/SelectGroup.53d83114.js` & `domain-admin-1.5.9/domain_admin/public/js/SelectGroup.e46bb885.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -9,15 +9,15 @@
     F as h,
     L as g,
     al as _
 } from "./vendor-vue.9e61e0af.js";
 import {
     H as f,
     _ as O
-} from "./index.165f9ce1.js";
+} from "./index.5c3a2f20.js";
 const S = u({
         id: "group-store",
         state: () => ({
             groupOptions: []
         }),
         getters: {
             getGroupOptions: e => e.groupOptions
```

### Comparing `domain-admin-1.5.8/domain_admin/public/js/codemirror-lib.a3a39aa0.js` & `domain-admin-1.5.9/domain_admin/public/js/codemirror-lib.a3a39aa0.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/js/element-icon.1ce1c350.js` & `domain-admin-1.5.9/domain_admin/public/js/element-icon.1ce1c350.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/js/element-plus.30eb1cab.js` & `domain-admin-1.5.9/domain_admin/public/js/element-plus.30eb1cab.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/js/event-enums.6c6f25e7.js` & `domain-admin-1.5.9/domain_admin/public/js/event-enums.6c6f25e7.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/js/highlight-lib.3654f6d3.js` & `domain-admin-1.5.9/domain_admin/public/js/highlight-lib.3654f6d3.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/js/index.0963ab53.js` & `domain-admin-1.5.9/domain_admin/public/js/index.1cd93e88.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 import {
     C as S
-} from "./ConnectStatus.a429b01b.js";
+} from "./ConnectStatus.8f8cc994.js";
 import {
     _ as m
-} from "./index.165f9ce1.js";
+} from "./index.5c3a2f20.js";
 import {
     ah as o,
     o as _,
     c as f,
     V as s,
     P as n,
     a as i,
```

### Comparing `domain-admin-1.5.8/domain_admin/public/js/index.165f9ce1.js` & `domain-admin-1.5.9/domain_admin/public/js/index.5c3a2f20.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,48 +1,48 @@
 import {
     aw as J,
-    ax as U,
+    ax as A,
     o as d,
     c as g,
-    U as x,
+    U as D,
     S as B,
     a as u,
     ay as F,
     ah as r,
     V as i,
     P as s,
-    F as C,
-    a8 as A,
+    F as x,
+    a8 as U,
     O as p,
-    R as j,
+    R as T,
     T as v,
-    Q as Qe,
-    W as Xe,
-    X as Ye,
-    a9 as Ze,
-    a3 as et,
-    az as tt,
-    aA as at,
-    aB as ot,
-    aC as it,
-    as as st,
-    aD as rt
+    Q as lt,
+    W as dt,
+    X as ut,
+    a9 as _t,
+    a3 as mt,
+    az as ct,
+    aA as pt,
+    aB as ft,
+    aC as gt,
+    as as ht,
+    aD as yt
 } from "./vendor-vue.9e61e0af.js";
 import {
-    Q as nt
+    Q as bt
 } from "./element-icon.1ce1c350.js";
 import {
     a as R,
-    b as lt,
-    N as z,
-    M as dt
+    b as vt,
+    N as H,
+    M as It
 } from "./vendor-lib.76301fc3.js";
 import {
     E as O,
-    i as ut
+    i as wt
 } from "./element-plus.30eb1cab.js";
 (function() {
     const t = document.createElement("link").relList;
     if (t && t.supports && t.supports("modulepreload")) return;
     for (const o of document.querySelectorAll('link[rel="modulepreload"]')) m(o);
     new MutationObserver(o => {
         for (const a of o)
@@ -61,15 +61,15 @@
     function m(o) {
         if (o.ep) return;
         o.ep = !0;
         const a = n(o);
         fetch(o.href, a)
     }
 })();
-var _t = {
+var Ct = {
     name: "zh-cn",
     el: {
         colorpicker: {
             confirm: "\u786E\u5B9A",
             clear: "\u6E05\u7A7A"
         },
         datepicker: {
@@ -188,15 +188,15 @@
         },
         popconfirm: {
             confirmButtonText: "\u786E\u5B9A",
             cancelButtonText: "\u53D6\u6D88"
         }
     }
 };
-const mt = {
+const Dt = {
         login: "/login",
         getDomainList: "/getDomainList",
         addDomain: "/addDomain",
         getDomainById: "/getDomainById",
         deleteDomainById: "/deleteDomainById",
         deleteDomainByIds: "/deleteDomainByIds",
         updateDomainById: "/updateDomainById",
@@ -277,65 +277,76 @@
         getCertInformation: "/getCertInformation",
         getAsyncTaskLogList: "/getAsyncTaskLogList",
         clearAsyncTaskLogList: "/clearAsyncTaskLogList",
         getCertificateList: "/getCertificateList",
         issueCertificate: "/issueCertificate",
         renewCertificate: "/renewCertificate",
         getIssueCertificateById: "/getIssueCertificateById",
-        verifyCertificateById: "/verifyCertificateById"
+        verifyCertificateById: "/verifyCertificateById",
+        getWaitVerifyDomainList: "/getWaitVerifyDomainList",
+        getDomainHost: "/getDomainHost",
+        deployVerifyFile: "/deployVerifyFile",
+        deployCertificateFile: "/deployCertificateFile",
+        getCertificateChallenges: "/getCertificateChallenges",
+        deleteCertificateById: "/deleteCertificateById",
+        deleteCertificateByBatch: "/deleteCertificateByBatch",
+        getHostList: "/getHostList",
+        addHost: "/addHost",
+        getHostById: "/getHostById",
+        updateHostById: "/updateHostById"
     },
     M = "token";
 
-function ct(e) {
+function xt(e) {
     R.set(M, e, {
         expires: 7
     })
 }
 
 function Q() {
     return R.get(M)
 }
 
-function pt() {
+function Et() {
     R.remove(M)
 }
 const X = "./api",
-    G = lt.create({
+    G = vt.create({
         baseURL: X
     });
 G.interceptors.request.use(e => {
     let t = Q();
     return t && (e.headers["X-Token"] = t), e
 }, e => {
     console.log(e)
 });
 G.interceptors.response.use(e => e.data, e => ({
     data: null,
     msg: e,
     code: -1
 }));
 
-function ft(e) {
+function kt(e) {
     return async function(t = {}, n) {
         const m = await G.post(e, t, n);
         return m.ok = !1, m.code == 0 ? m.ok = !0 : (O.closeAll(), O.error(m.msg)), m
     }
 }
 
-function gt() {
+function St() {
     let e = {};
-    for (let [t, n] of Object.entries(mt)) e[t] = ft(n);
+    for (let [t, n] of Object.entries(Dt)) e[t] = kt(n);
     return e
 }
-const N = gt();
+const N = St();
 
-function Bo(e) {
+function Qo(e) {
     return X + e
 }
-class ht {
+class Lt {
     static message(t) {
         return O.closeAll(), O(t)
     }
     static success(t) {
         return this.message({
             message: t,
             type: "success"
@@ -359,37 +370,37 @@
             type: "error"
         })
     }
     static closeAll() {
         O.closeAll()
     }
 }
-const yt = "modulepreload",
-    bt = function(e, t) {
+const Bt = "modulepreload",
+    $t = function(e, t) {
         return new URL(e, t).href
     },
-    H = {},
+    z = {},
     h = function(t, n, m) {
         return !n || n.length === 0 ? t() : Promise.all(n.map(o => {
-            if (o = bt(o, m), o in H) return;
-            H[o] = !0;
+            if (o = $t(o, m), o in z) return;
+            z[o] = !0;
             const a = o.endsWith(".css"),
                 l = a ? '[rel="stylesheet"]' : "";
             if (document.querySelector(`link[href="${o}"]${l}`)) return;
             const _ = document.createElement("link");
-            if (_.rel = a ? "stylesheet" : yt, a || (_.as = "script", _.crossOrigin = ""), _.href = o, document.head.appendChild(_), a) return new Promise((c, y) => {
+            if (_.rel = a ? "stylesheet" : Bt, a || (_.as = "script", _.crossOrigin = ""), _.href = o, document.head.appendChild(_), a) return new Promise((c, y) => {
                 _.addEventListener("load", c), _.addEventListener("error", () => y(new Error(`Unable to preload CSS for ${o}`)))
             })
         })).then(() => t())
     };
 
 function Y(e, t) {
     return e && e.length > 0 ? e.some(n => t.includes(n)) : !0
 }
-const D = {
+const C = {
         User: 1,
         Admin: 10
     },
     P = J({
         id: "user-store",
         state: () => ({
             _userInfo: null
@@ -399,15 +410,15 @@
                 return e._userInfo != null
             },
             isAdmin(e) {
                 if (e._userInfo) return e._userInfo.username == "admin"
             },
             userRoles(e) {
                 let t = [];
-                return this.isAdmin && t.push(D.Admin), t
+                return this.isAdmin && t.push(C.Admin), t
             },
             userInfo(e) {
                 return e._userInfo
             }
         },
         actions: {
             async updateUserInfo() {
@@ -442,86 +453,86 @@
             },
             async updateVersion() {
                 const e = await N.getSystemVersion();
                 e.code == 0 && (this._version = e.data.version)
             }
         }
     });
-const w = (e, t) => {
+const I = (e, t) => {
         const n = e.__vccOpts || e;
         for (const [m, o] of t) n[m] = o;
         return n
     },
-    vt = {
+    Ot = {
         name: "",
         props: [],
         components: {},
         data() {
             return {}
         },
         computed: {
-            ...U($, {
+            ...A($, {
                 version: "version"
             })
         },
         methods: {
             async getData() {}
         },
         created() {
             this.getData()
         }
     },
-    wt = {
+    At = {
         class: "sidebar-info"
     },
-    It = {
+    Ut = {
         key: 0
     },
-    Dt = u("a", {
+    Vt = u("a", {
         href: "https://pypi.org/project/domain-admin/",
         target: "_blank",
         class: "sidebar-info__box"
     }, [u("img", {
         alt: "Version",
         src: "https://img.shields.io/pypi/v/domain-admin.svg"
     })], -1),
-    xt = u("a", {
+    Ft = u("a", {
         href: "https://github.com/mouday/domain-admin",
         target: "_blank",
         class: "sidebar-info__box"
     }, [u("img", {
         alt: "GitHub stars",
         src: "https://img.shields.io/github/stars/mouday/domain-admin.svg?style=social"
     })], -1);
 
-function Ct(e, t, n, m, o, a) {
-    return d(), g("div", wt, [e.version ? (d(), g("div", It, x(e.version), 1)) : B("", !0), Dt, xt])
+function Pt(e, t, n, m, o, a) {
+    return d(), g("div", At, [e.version ? (d(), g("div", Ut, D(e.version), 1)) : B("", !0), Vt, Ft])
 }
-const Et = w(vt, [
-    ["render", Ct]
+const jt = I(Ot, [
+    ["render", Pt]
 ]);
-const kt = {
+const Tt = {
         name: "Menu",
         props: {},
         components: {
-            Info: Et
+            Info: jt
         },
         data() {
             return {
                 activeIndex: "",
                 routes: ee
             }
         },
         computed: {
-            ...U(P, {
+            ...A(P, {
                 userInfo: "userInfo",
                 isAdmin: "isAdmin",
                 userRoles: "userRoles"
             }),
-            ...U($, {
+            ...A($, {
                 isCollapse: "isCollapse"
             })
         },
         methods: {
             ...F($, {
                 toggleCollapse: "toggleCollapse"
             }),
@@ -539,157 +550,157 @@
                 return e.children.filter(t => this.hasRoutePermission(t)).length == 1
             }
         },
         created() {
             this.activeIndex = this.$route.name, console.log(this.activeIndex), this.getData()
         }
     },
-    St = {
+    Rt = {
         class: "layout-container"
     },
-    Lt = {
+    Mt = {
         class: "layout__menu-wrap"
     },
-    Bt = {
+    Gt = {
         class: "layout__menu__collapse-wrap"
     };
 
-function $t(e, t, n, m, o, a) {
+function Nt(e, t, n, m, o, a) {
     const l = r("el-icon"),
         _ = r("el-menu-item"),
         c = r("el-sub-menu"),
         y = r("Info"),
-        I = r("el-menu"),
-        T = r("CaretRight"),
+        w = r("el-menu"),
+        j = r("CaretRight"),
         E = r("el-link"),
         V = r("CaretLeft");
-    return d(), g("div", St, [u("div", Lt, [i(I, {
+    return d(), g("div", Rt, [u("div", Mt, [i(w, {
         "default-active": o.activeIndex,
         ellipsis: !1,
         class: "layout__menu",
         mode: "vertical",
         "menu-trigger": "click",
         "unique-opened": "",
         onSelect: a.handleSelect,
         collapse: e.isCollapse
     }, {
-        default: s(() => [(d(!0), g(C, null, A(o.routes, b => (d(), g(C, null, [a.hasRoutePermission(b) ? (d(), g(C, {
+        default: s(() => [(d(!0), g(x, null, U(o.routes, b => (d(), g(x, null, [a.hasRoutePermission(b) ? (d(), g(x, {
             key: 0
         }, [a.hasOnlyOneChildren(b) ? (d(), p(_, {
             key: 0,
             index: b.children[0].name,
             onClick: S => a.handleRouteClick(b.children[0])
         }, {
             default: s(() => [i(l, null, {
-                default: s(() => [(d(), p(j(b.children[0].meta.icon)))]),
+                default: s(() => [(d(), p(T(b.children[0].meta.icon)))]),
                 _: 2
-            }, 1024), u("span", null, x(b.children[0].meta.title), 1)]),
+            }, 1024), u("span", null, D(b.children[0].meta.title), 1)]),
             _: 2
         }, 1032, ["index", "onClick"])) : (d(), p(c, {
             key: 1,
             index: b.name
         }, {
             title: s(() => [i(l, null, {
-                default: s(() => [(d(), p(j(b.meta.icon)))]),
+                default: s(() => [(d(), p(T(b.meta.icon)))]),
                 _: 2
-            }, 1024), u("span", null, x(b.meta.title), 1)]),
-            default: s(() => [(d(!0), g(C, null, A(b.children, S => (d(), g(C, null, [a.hasRoutePermission(S) ? (d(), p(_, {
+            }, 1024), u("span", null, D(b.meta.title), 1)]),
+            default: s(() => [(d(!0), g(x, null, U(b.children, S => (d(), g(x, null, [a.hasRoutePermission(S) ? (d(), p(_, {
                 key: 0,
                 index: S.name,
                 onClick: q => a.handleRouteClick(S)
             }, {
-                default: s(() => [v(x(S.meta.title), 1)]),
+                default: s(() => [v(D(S.meta.title), 1)]),
                 _: 2
             }, 1032, ["index", "onClick"])) : B("", !0)], 64))), 256))]),
             _: 2
-        }, 1032, ["index"]))], 64)) : B("", !0)], 64))), 256)), Qe(i(y, {
+        }, 1032, ["index"]))], 64)) : B("", !0)], 64))), 256)), lt(i(y, {
             class: "menu-info"
         }, null, 512), [
-            [Xe, !e.isCollapse]
+            [dt, !e.isCollapse]
         ])]),
         _: 1
-    }, 8, ["default-active", "onSelect", "collapse"]), u("div", Bt, [u("div", {
+    }, 8, ["default-active", "onSelect", "collapse"]), u("div", Gt, [u("div", {
         class: "layout__menu__collapse",
         onClick: t[0] || (t[0] = (...b) => e.toggleCollapse && e.toggleCollapse(...b))
     }, [e.isCollapse ? (d(), p(E, {
         key: 0,
         underline: !1
     }, {
         default: s(() => [i(l, null, {
-            default: s(() => [i(T)]),
+            default: s(() => [i(j)]),
             _: 1
         })]),
         _: 1
     })) : (d(), p(E, {
         key: 1,
         underline: !1
     }, {
         default: s(() => [i(l, null, {
             default: s(() => [i(V)]),
             _: 1
         })]),
         _: 1
     }))])])])])
 }
-const Ot = w(kt, [
-        ["render", $t]
+const qt = I(Tt, [
+        ["render", Nt]
     ]),
-    Ut = {
+    Ht = {
         name: "Footer",
         props: {},
         components: {},
         data() {
             return {}
         },
         computed: {},
         methods: {
             async getData() {}
         },
         created() {
             this.getData()
         }
     },
-    At = {
+    zt = {
         class: "footer"
     };
 
-function Vt(e, t, n, m, o, a) {
-    return d(), g("div", At)
+function Wt(e, t, n, m, o, a) {
+    return d(), g("div", zt)
 }
-const Ft = w(Ut, [
-        ["render", Vt]
+const Kt = I(Ht, [
+        ["render", Wt]
     ]),
-    Pt = {
+    Jt = {
         password: [{
             message: "\u65E7\u5BC6\u7801\u4E0D\u80FD\u4E3A\u7A7A",
             required: !0,
             trigger: "blur"
         }],
         new_password: [{
             message: "\u65B0\u5BC6\u7801\u4E0D\u80FD\u4E3A\u7A7A",
             required: !0,
             trigger: "blur"
         }]
     },
-    Tt = {
+    Qt = {
         name: "",
         props: {
             row: {
                 type: Object,
                 default: null
             }
         },
         components: {},
         data() {
             return {
                 form: {
                     password: "",
                     new_password: ""
                 },
-                rules: Pt
+                rules: Jt
             }
         },
         computed: {},
         methods: {
             async getData() {
                 if (this.row) {
                     let e = {
@@ -724,19 +735,19 @@
                 })
             }
         },
         created() {
             this.getData()
         }
     },
-    jt = {
+    Xt = {
         class: "text-center"
     };
 
-function Rt(e, t, n, m, o, a) {
+function Yt(e, t, n, m, o, a) {
     const l = r("el-input"),
         _ = r("el-form-item"),
         c = r("el-form"),
         y = r("el-button");
     return d(), g("div", null, [i(c, {
         ref: "form",
         model: o.form,
@@ -746,62 +757,62 @@
         default: s(() => [i(_, {
             label: "\u65E7\u5BC6\u7801",
             prop: "password"
         }, {
             default: s(() => [i(l, {
                 type: "text",
                 modelValue: o.form.password,
-                "onUpdate:modelValue": t[0] || (t[0] = I => o.form.password = I),
+                "onUpdate:modelValue": t[0] || (t[0] = w => o.form.password = w),
                 placeholder: "\u8BF7\u8F93\u5165\u65E7\u5BC6\u7801"
             }, null, 8, ["modelValue"])]),
             _: 1
         }), i(_, {
             label: "\u65B0\u5BC6\u7801",
             prop: "new_password"
         }, {
             default: s(() => [i(l, {
                 type: "text",
                 modelValue: o.form.new_password,
-                "onUpdate:modelValue": t[1] || (t[1] = I => o.form.new_password = I),
+                "onUpdate:modelValue": t[1] || (t[1] = w => o.form.new_password = w),
                 placeholder: "\u8BF7\u8F93\u5165\u65B0\u5BC6\u7801"
             }, null, 8, ["modelValue"])]),
             _: 1
         })]),
         _: 1
-    }, 8, ["model", "rules"]), u("div", jt, [i(y, {
+    }, 8, ["model", "rules"]), u("div", Xt, [i(y, {
         onClick: a.handleCancel
     }, {
         default: s(() => [v("\u53D6 \u6D88")]),
         _: 1
     }, 8, ["onClick"]), i(y, {
         type: "primary",
         onClick: a.handleSubmit
     }, {
         default: s(() => [v("\u786E \u5B9A")]),
         _: 1
     }, 8, ["onClick"])])])
 }
-const Mt = w(Tt, [
-        ["render", Rt]
+const Zt = I(Qt, [
+        ["render", Yt]
     ]),
-    Gt = {
+    ea = {
         name: "",
         props: {
             row: {
                 type: Object,
                 default: null
             },
             visible: {
                 type: Boolean,
                 default: !1
             }
         },
         emits: ["update:visible"],
         components: {
-            DataForm: Mt
+            DataForm: Zt
         },
         data() {
             return {}
         },
         computed: {
             dialogTitle() {
                 return this.row ? "\u7F16\u8F91" : "\u6DFB\u52A0"
@@ -823,15 +834,15 @@
             handleSuccess() {
                 this.$emit("on-success")
             }
         },
         created() {}
     };
 
-function Nt(e, t, n, m, o, a) {
+function ta(e, t, n, m, o, a) {
     const l = r("DataForm"),
         _ = r("el-dialog");
     return d(), p(_, {
         title: "\u4FEE\u6539\u767B\u5F55\u5BC6\u7801",
         modelValue: a.dialogVisible,
         "onUpdate:modelValue": t[0] || (t[0] = c => a.dialogVisible = c),
         width: "400px",
@@ -844,18 +855,18 @@
             row: n.row,
             onOnCancel: a.handleClose,
             onOnSuccess: a.handleSuccess
         }, null, 8, ["row", "onOnCancel", "onOnSuccess"])) : B("", !0)]),
         _: 1
     }, 8, ["modelValue"])
 }
-const qt = w(Gt, [
-    ["render", Nt]
+const aa = I(ea, [
+    ["render", ta]
 ]);
-const zt = {
+const oa = {
         name: "",
         props: {},
         components: {},
         data() {
             return {
                 version: ""
             }
@@ -867,102 +878,102 @@
                 this.version = e.data.version
             }
         },
         created() {
             this.getData()
         }
     },
-    Ht = {
+    ia = {
         class: "mo-form-detail about-system"
     },
-    Wt = u("a", {
+    sa = u("a", {
         href: "https://pypi.org/project/domain-admin/",
         target: "_blank"
     }, [u("img", {
         alt: "Version",
         src: "https://img.shields.io/pypi/v/domain-admin.svg"
     })], -1),
-    Kt = u("a", {
+    ra = u("a", {
         class: "inline-block",
         href: "https://github.com/mouday/domain-admin/issues",
         target: "_blank"
     }, [u("img", {
         alt: "GitHub issues",
         src: "https://img.shields.io/github/issues/mouday/domain-admin"
     })], -1),
-    Jt = u("a", {
+    na = u("a", {
         class: "inline-block",
         href: "https://github.com/mouday/domain-admin",
         target: "_blank"
     }, [u("img", {
         alt: "GitHub stars",
         src: "https://img.shields.io/github/stars/mouday/domain-admin.svg?style=social"
     })], -1),
-    Qt = u("span", null, "731742868", -1);
+    la = u("span", null, "731742868", -1);
 
-function Xt(e, t, n, m, o, a) {
+function da(e, t, n, m, o, a) {
     const l = r("el-form-item"),
         _ = r("el-form");
-    return d(), g("div", Ht, [i(_, {
+    return d(), g("div", ia, [i(_, {
         ref: "form",
         model: e.form,
         "label-width": "130px"
     }, {
         default: s(() => [i(l, {
             label: "\u5F53\u524D\u7248\u672C",
             prop: "domain"
         }, {
-            default: s(() => [v(x(o.version), 1)]),
+            default: s(() => [v(D(o.version), 1)]),
             _: 1
         }), i(l, {
             label: "\u6700\u65B0\u7248\u672C",
             prop: "ip"
         }, {
-            default: s(() => [Wt]),
+            default: s(() => [sa]),
             _: 1
         }), i(l, {
             label: "\u95EE\u9898\u53CD\u9988",
             prop: "connect_status"
         }, {
-            default: s(() => [Kt]),
+            default: s(() => [ra]),
             _: 1
         }), i(l, {
             label: "\u7ED9\u6211\u4EEC\u70B9\u8D5E",
             prop: "connect_status"
         }, {
-            default: s(() => [Jt]),
+            default: s(() => [na]),
             _: 1
         }), i(l, {
             label: "QQ\u4EA4\u6D41\u7FA4",
             prop: "domain"
         }, {
-            default: s(() => [Qt]),
+            default: s(() => [la]),
             _: 1
         })]),
         _: 1
     }, 8, ["model"])])
 }
-const Yt = w(zt, [
-        ["render", Xt]
+const ua = I(oa, [
+        ["render", da]
     ]),
-    Zt = {
+    _a = {
         name: "",
         props: {
             row: {
                 type: Object,
                 default: null
             },
             visible: {
                 type: Boolean,
                 default: !1
             }
         },
         emits: ["update:visible"],
         components: {
-            DataForm: Yt
+            DataForm: ua
         },
         data() {
             return {}
         },
         computed: {
             dialogTitle() {
                 return this.row ? "\u7F16\u8F91" : "\u6DFB\u52A0"
@@ -986,15 +997,15 @@
             handleSuccess() {
                 this.handleClose(), this.$emit("on-success")
             }
         },
         created() {}
     };
 
-function ea(e, t, n, m, o, a) {
+function ma(e, t, n, m, o, a) {
     const l = r("DataForm"),
         _ = r("el-dialog");
     return d(), p(_, {
         title: "\u5173\u4E8E Domain Admin",
         modelValue: a.dialogVisible,
         "onUpdate:modelValue": t[0] || (t[0] = c => a.dialogVisible = c),
         width: "400px",
@@ -1007,42 +1018,42 @@
             row: n.row,
             onOnCancel: a.handleClose,
             onOnSuccess: a.handleSuccess
         }, null, 8, ["row", "onOnCancel", "onOnSuccess"])) : B("", !0)]),
         _: 1
     }, 8, ["modelValue"])
 }
-const ta = w(Zt, [
-        ["render", ea]
+const ca = I(_a, [
+        ["render", ma]
     ]),
-    aa = {};
+    pa = {};
 
-function oa() {
+function fa() {
     let e = URL.createObjectURL(new Blob),
         t = e.toString();
     return URL.revokeObjectURL(e), t.substring(t.lastIndexOf("/") + 1)
 }
-const ia = "mXMn18VQJxoH0P";
+const ga = "mXMn18VQJxoH0P";
 
-function sa() {
-    return `https://api.multiavatar.com/${oa()}.png?apikey=${ia}`
+function ha() {
+    return `https://api.multiavatar.com/${fa()}.png?apikey=${ga}`
 }
 const Z = "" + new URL("../gif/user-avatar.ea67286d.gif", import.meta.url).href,
-    ra = {
+    ya = {
         name: "",
         props: {
             row: {
                 type: Object,
                 default: null
             }
         },
         components: {},
         data() {
             return {
-                rules: aa,
+                rules: pa,
                 avatar: Z,
                 form: {
                     username: "",
                     avatar_url: "",
                     before_expire_days: 0
                 }
             }
@@ -1055,15 +1066,15 @@
                 let t = e.data;
                 this.form.username = t.username, this.form.avatar_url = t.avatar_url
             },
             handleCancel() {
                 this.$emit("on-cancel")
             },
             handleRandomAvatar() {
-                this.form.avatar_url = sa()
+                this.form.avatar_url = ha()
             },
             handleSubmit() {
                 this.$refs.form.validate(e => {
                     if (e) this.confirmSubmit();
                     else return !1
                 })
             },
@@ -1083,76 +1094,76 @@
                 })
             }
         },
         created() {
             this.getData()
         }
     },
-    na = {
+    ba = {
         class: "text-center"
     };
 
-function la(e, t, n, m, o, a) {
+function va(e, t, n, m, o, a) {
     const l = r("el-form-item"),
         _ = r("el-avatar"),
         c = r("el-form"),
         y = r("el-button");
     return d(), g("div", null, [i(c, {
         ref: "form",
         model: o.form,
         rules: o.rules,
         "label-width": "100px"
     }, {
         default: s(() => [i(l, {
             label: "\u7528\u6237\u540D",
             prop: "username"
         }, {
-            default: s(() => [u("span", null, x(o.form.username), 1)]),
+            default: s(() => [u("span", null, D(o.form.username), 1)]),
             _: 1
         }), i(l, {
             label: "\u5934\u50CF",
             prop: "avatar_url"
         }, {
             default: s(() => [i(_, {
                 src: o.avatar
             }, null, 8, ["src"])]),
             _: 1
         })]),
         _: 1
-    }, 8, ["model", "rules"]), u("div", na, [i(y, {
+    }, 8, ["model", "rules"]), u("div", ba, [i(y, {
         onClick: a.handleCancel
     }, {
         default: s(() => [v("\u53D6 \u6D88")]),
         _: 1
     }, 8, ["onClick"]), i(y, {
         type: "primary",
         onClick: a.handleSubmit
     }, {
         default: s(() => [v("\u786E \u5B9A")]),
         _: 1
     }, 8, ["onClick"])])])
 }
-const da = w(ra, [
-        ["render", la]
+const Ia = I(ya, [
+        ["render", va]
     ]),
-    ua = {
+    wa = {
         name: "",
         props: {
             row: {
                 type: Object,
                 default: null
             },
             visible: {
                 type: Boolean,
                 default: !1
             }
         },
         emits: ["update:visible"],
         components: {
-            DataForm: da
+            DataForm: Ia
         },
         data() {
             return {}
         },
         computed: {
             dialogTitle() {
                 return this.row ? "\u7F16\u8F91" : "\u6DFB\u52A0"
@@ -1176,15 +1187,15 @@
             handleSuccess() {
                 this.handleClose(), this.$emit("on-success")
             }
         },
         created() {}
     };
 
-function _a(e, t, n, m, o, a) {
+function Ca(e, t, n, m, o, a) {
     const l = r("DataForm"),
         _ = r("el-dialog");
     return d(), p(_, {
         title: "\u4E2A\u4EBA\u8BBE\u7F6E",
         modelValue: a.dialogVisible,
         "onUpdate:modelValue": t[0] || (t[0] = c => a.dialogVisible = c),
         width: "400px",
@@ -1197,18 +1208,18 @@
             row: n.row,
             onOnCancel: a.handleClose,
             onOnSuccess: a.handleSuccess
         }, null, 8, ["row", "onOnCancel", "onOnSuccess"])) : B("", !0)]),
         _: 1
     }, 8, ["modelValue"])
 }
-const ma = w(ua, [
-        ["render", _a]
+const Da = I(wa, [
+        ["render", Ca]
     ]),
-    ca = {
+    xa = {
         name: "Breadcrumb",
         props: {},
         components: {},
         data() {
             return {}
         },
         computed: {
@@ -1220,41 +1231,41 @@
             async getData() {}
         },
         created() {
             console.log(this.$route), this.getData()
         }
     };
 
-function pa(e, t, n, m, o, a) {
+function Ea(e, t, n, m, o, a) {
     const l = r("el-breadcrumb-item"),
         _ = r("el-breadcrumb");
     return d(), p(_, {
         separator: "/"
     }, {
-        default: s(() => [(d(!0), g(C, null, A(a.matchedRoutes, c => (d(), p(l, null, {
-            default: s(() => [v(x(c.meta.title), 1)]),
+        default: s(() => [(d(!0), g(x, null, U(a.matchedRoutes, c => (d(), p(l, null, {
+            default: s(() => [v(D(c.meta.title), 1)]),
             _: 2
         }, 1024))), 256))]),
         _: 1
     })
 }
-const fa = w(ca, [
-        ["render", pa]
+const ka = I(xa, [
+        ["render", Ea]
     ]),
-    ga = "" + new URL("../svg/logo.184a2d7d.svg", import.meta.url).href,
-    ha = "" + new URL("../jpg/chatpet.fce5580e.jpg", import.meta.url).href,
-    ya = "" + new URL("../jpg/chatpet-white.10f4f36c.jpg", import.meta.url).href;
-const ba = {
+    Sa = "" + new URL("../svg/logo.184a2d7d.svg", import.meta.url).href,
+    La = "" + new URL("../jpg/chatpet.fce5580e.jpg", import.meta.url).href,
+    Ba = "" + new URL("../jpg/chatpet-white.10f4f36c.jpg", import.meta.url).href;
+const $a = {
         name: "Header",
         props: {},
         components: {
-            UserPaswordEditDataFormDailog: qt,
-            AboutDataFormDailig: ta,
-            UserDataFormDailig: ma,
-            Breadcrumb: fa
+            UserPaswordEditDataFormDailog: aa,
+            AboutDataFormDailig: ca,
+            UserDataFormDailig: Da,
+            Breadcrumb: ka
         },
         data() {
             let e = [{
                 value: "theme--blue",
                 label: "\u7ECF\u5178"
             }, {
                 value: "theme--dark",
@@ -1298,19 +1309,19 @@
                 avatar: Z
             }
         },
         created() {
             this.getData()
         },
         computed: {
-            ...U(P, {
+            ...A(P, {
                 userInfo: "userInfo",
                 isAdmin: "isAdmin"
             }),
-            ...U($, {
+            ...A($, {
                 isCollapse: "isCollapse"
             }),
             username() {
                 return this.userInfo ? this.userInfo.username : ""
             }
         },
         methods: {
@@ -1318,15 +1329,15 @@
                 updateUserInfo: "updateUserInfo",
                 removeUserInfo: "removeUserInfo"
             }),
             ...F($, {
                 toggleCollapse: "toggleCollapse"
             }),
             handleLogoutClick(e) {
-                this.removeUserInfo(), pt(), this.$router.push({
+                this.removeUserInfo(), Et(), this.$router.push({
                     path: "/login"
                 })
             },
             handleUpdatePasswordClick() {
                 this.dialogVisible = !0
             },
             handleUserPaswordEditClose() {
@@ -1377,126 +1388,126 @@
                 })
             }
         },
         created() {
             this.theme = localStorage.getItem("theme") || this.theme, this.handleThemeChange(this.theme)
         }
     },
-    va = {
+    Oa = {
         class: "layout__header"
     },
-    wa = u("a", {
+    Aa = u("a", {
         class: "layout__header__logo__span",
         href: "#"
     }, [u("img", {
         class: "layout__header__logo",
-        src: ga,
+        src: Sa,
         alt: "",
         srcset: ""
     }), u("span", null, "Domain Admin")], -1),
-    Ia = {
+    Ua = {
         class: "header-breadcrumb"
     },
-    Da = {
+    Va = {
         class: "self-center margin-left--auto flex items-center"
     },
-    xa = u("a", {
-        href: "http://www.chatpet.top/",
+    Fa = u("a", {
+        href: "https://www.chatpet.top/",
         class: "ad-wrap mr-md",
         target: "_blank"
     }, [u("img", {
-        src: ha,
+        src: La,
         alt: "",
         class: "ad-img ad-img--blue"
     }), u("img", {
-        src: ya,
+        src: Ba,
         alt: "",
         class: "ad-img ad-img--white"
     })], -1),
-    Ca = {
+    Pa = {
         class: "header-tool-btn"
     },
-    Ea = u("span", {
+    ja = u("span", {
         class: "header-tool-btn__text"
     }, "\u5DE5\u5177\u7BB1", -1),
-    ka = {
+    Ta = {
         class: "avatar-group ml-sm"
     };
 
-function Sa(e, t, n, m, o, a) {
+function Ra(e, t, n, m, o, a) {
     const l = r("Menu"),
         _ = r("el-icon"),
         c = r("Breadcrumb"),
         y = r("Suitcase"),
-        I = r("arrow-down"),
-        T = r("Link"),
+        w = r("arrow-down"),
+        j = r("Link"),
         E = r("el-dropdown-item"),
         V = r("el-dropdown-menu"),
         b = r("el-dropdown"),
         S = r("el-radio-button"),
         q = r("el-radio-group"),
-        ze = r("el-avatar"),
-        He = r("UserPaswordEditDataFormDailog"),
-        We = r("UserDataFormDailig"),
-        Ke = r("AboutDataFormDailig");
-    return d(), g("div", va, [u("div", {
+        ot = r("el-avatar"),
+        it = r("UserPaswordEditDataFormDailog"),
+        st = r("UserDataFormDailig"),
+        rt = r("AboutDataFormDailig");
+    return d(), g("div", Oa, [u("div", {
         class: "menu__button",
         onClick: t[0] || (t[0] = (...f) => a.handleMenuClick && a.handleMenuClick(...f))
     }, [i(_, {
         style: {
             color: "#4f5a76",
             "font-size": "20px"
         }
     }, {
         default: s(() => [i(l)]),
         _: 1
-    })]), wa, u("div", Ia, [i(c)]), u("div", Da, [xa, i(b, {
+    })]), Aa, u("div", Ua, [i(c)]), u("div", Va, [Fa, i(b, {
         trigger: "hover"
     }, {
         dropdown: s(() => [i(V, null, {
-            default: s(() => [(d(!0), g(C, null, A(o.toolList, f => (d(), g(C, null, [f.type == "url" ? (d(), p(E, {
+            default: s(() => [(d(!0), g(x, null, U(o.toolList, f => (d(), g(x, null, [f.type == "url" ? (d(), p(E, {
                 key: 0,
-                onClick: Je => a.handleToolItemClick(f),
+                onClick: nt => a.handleToolItemClick(f),
                 class: "justify-center"
             }, {
-                default: s(() => [v(x(f.label), 1), i(_, null, {
-                    default: s(() => [i(T)]),
+                default: s(() => [v(D(f.label), 1), i(_, null, {
+                    default: s(() => [i(j)]),
                     _: 1
                 })]),
                 _: 2
             }, 1032, ["onClick"])) : (d(), p(E, {
                 key: 1,
-                onClick: Je => a.handleToolItemClick(f),
+                onClick: nt => a.handleToolItemClick(f),
                 class: "justify-center"
             }, {
-                default: s(() => [v(x(f.label), 1)]),
+                default: s(() => [v(D(f.label), 1)]),
                 _: 2
             }, 1032, ["onClick"]))], 64))), 256))]),
             _: 1
         })]),
-        default: s(() => [u("div", Ca, [i(_, null, {
+        default: s(() => [u("div", Pa, [i(_, null, {
             default: s(() => [i(y)]),
             _: 1
-        }), Ea, i(_, null, {
-            default: s(() => [i(I)]),
+        }), ja, i(_, null, {
+            default: s(() => [i(w)]),
             _: 1
         })])]),
         _: 1
     }), i(q, {
         modelValue: o.theme,
         "onUpdate:modelValue": t[1] || (t[1] = f => o.theme = f),
         size: "small",
         class: "ml-md",
         onChange: a.handleThemeChange
     }, {
-        default: s(() => [(d(!0), g(C, null, A(o.themeList, f => (d(), p(S, {
+        default: s(() => [(d(!0), g(x, null, U(o.themeList, f => (d(), p(S, {
             key: f.value,
             label: f.value
         }, {
-            default: s(() => [v(x(f.label), 1)]),
+            default: s(() => [v(D(f.label), 1)]),
             _: 2
         }, 1032, ["label"]))), 128))]),
         _: 1
     }, 8, ["modelValue", "onChange"]), i(b, {
         trigger: "hover"
     }, {
         dropdown: s(() => [i(V, null, {
@@ -1517,43 +1528,43 @@
                 class: "justify-center"
             }, {
                 default: s(() => [v("\u9000\u51FA")]),
                 _: 1
             }, 8, ["onClick"])]),
             _: 1
         })]),
-        default: s(() => [u("div", ka, [i(ze, {
+        default: s(() => [u("div", Ta, [i(ot, {
             src: o.avatar
-        }, null, 8, ["src"]), u("span", null, x(a.username), 1)])]),
+        }, null, 8, ["src"]), u("span", null, D(a.username), 1)])]),
         _: 1
-    })]), i(He, {
+    })]), i(it, {
         visible: o.dialogVisible,
         "onUpdate:visible": t[2] || (t[2] = f => o.dialogVisible = f),
         onOnSuccess: a.handleUserPaswordEditSuccess,
         onOnCancel: a.handleUserPaswordEditClose
-    }, null, 8, ["visible", "onOnSuccess", "onOnCancel"]), i(We, {
+    }, null, 8, ["visible", "onOnSuccess", "onOnCancel"]), i(st, {
         visible: o.userDialogVisible,
         "onUpdate:visible": t[3] || (t[3] = f => o.userDialogVisible = f),
         onOnSuccess: a.handleUserInfoEditClose,
         onOnCancel: a.handleUserInfoEditClose
-    }, null, 8, ["visible", "onOnSuccess", "onOnCancel"]), i(Ke, {
+    }, null, 8, ["visible", "onOnSuccess", "onOnCancel"]), i(rt, {
         visible: o.aboutDialogVisible,
         "onUpdate:visible": t[4] || (t[4] = f => o.aboutDialogVisible = f)
     }, null, 8, ["visible"])])
 }
-const La = w(ba, [
-    ["render", Sa]
+const Ma = I($a, [
+    ["render", Ra]
 ]);
-const Ba = {
+const Ga = {
         name: "index",
         props: {},
         components: {
-            Menu: Ot,
-            Footer: Ft,
-            Header: La
+            Menu: qt,
+            Footer: Kt,
+            Header: Ma
         },
         data() {
             return {}
         },
         computed: {
             currentPathName() {
                 return console.log(this.$route), this.$route.meta.title
@@ -1565,51 +1576,51 @@
         methods: {
             async getData() {}
         },
         created() {
             this.getData()
         }
     },
-    $a = {
+    Na = {
         class: "app-layout"
     },
-    Oa = {
+    qa = {
         class: "app-layout__main"
     },
-    Ua = {
+    Ha = {
         class: "app-layout__body"
     },
-    Aa = {
+    za = {
         class: "app-layout__view"
     };
 
-function Va(e, t, n, m, o, a) {
+function Wa(e, t, n, m, o, a) {
     const l = r("Header"),
         _ = r("Menu"),
         c = r("router-view"),
         y = r("Footer");
-    return d(), g("div", $a, [i(l), u("div", Oa, [i(_), u("div", Ua, [u("div", Aa, [i(c, null, {
+    return d(), g("div", Na, [i(l), u("div", qa, [i(_), u("div", Ha, [u("div", za, [i(c, null, {
         default: s(({
-            Component: I
-        }) => [i(Ye, {
+            Component: w
+        }) => [i(ut, {
             name: "fade-transform",
             mode: "out-in"
         }, {
-            default: s(() => [(d(), p(j(I), {
+            default: s(() => [(d(), p(T(w), {
                 key: a.key
             }))]),
             _: 2
         }, 1024)]),
         _: 1
     })])])]), i(y)])
 }
-const k = w(Ba, [
-    ["render", Va]
+const k = I(Ga, [
+    ["render", Wa]
 ]);
-const Fa = {
+const Ka = {
         name: "Login",
         props: {},
         components: {},
         data() {
             return {
                 form: {
                     username: "",
@@ -1640,92 +1651,92 @@
             },
             async confirmSubmit() {
                 const e = await this.$http.login({
                     username: this.form.username,
                     password: this.form.password
                 });
                 if (console.log(e), e.code == 0) {
-                    ct(e.data.token), this.$msg.success("\u767B\u5F55\u6210\u529F");
+                    xt(e.data.token), this.$msg.success("\u767B\u5F55\u6210\u529F");
                     let t = "/";
                     this.$route.query.redirect && (t = this.$route.query.redirect), this.$router.push({
                         path: t
                     })
                 }
             }
         },
         created() {
             this.getData()
         }
     },
-    Pa = e => (tt("data-v-ea6aa27d"), e = e(), at(), e),
-    Ta = {
+    Ja = e => (ct("data-v-ea6aa27d"), e = e(), pt(), e),
+    Qa = {
         class: "login-container-wrap"
     },
-    ja = {
+    Xa = {
         class: "login-container"
     },
-    Ra = Pa(() => u("h3", {
+    Ya = Ja(() => u("h3", {
         class: "title"
     }, "Domain Admin", -1));
 
-function Ma(e, t, n, m, o, a) {
+function Za(e, t, n, m, o, a) {
     const l = r("el-input"),
         _ = r("el-form-item"),
         c = r("el-form"),
         y = r("el-button");
-    return d(), g("div", Ta, [u("div", ja, [Ra, i(c, {
+    return d(), g("div", Qa, [u("div", Xa, [Ya, i(c, {
         class: "",
         ref: "form",
         model: o.form,
         rules: o.rules,
         "label-width": "auto"
     }, {
         default: s(() => [i(_, {
             label: "",
             prop: "username"
         }, {
             default: s(() => [i(l, {
                 modelValue: o.form.username,
-                "onUpdate:modelValue": t[0] || (t[0] = I => o.form.username = I),
+                "onUpdate:modelValue": t[0] || (t[0] = w => o.form.username = w),
                 "auto-complete": "off",
                 placeholder: "\u7528\u6237\u540D"
             }, null, 8, ["modelValue"])]),
             _: 1
         }), i(_, {
             label: "",
             prop: "password"
         }, {
             default: s(() => [i(l, {
                 modelValue: o.form.password,
-                "onUpdate:modelValue": t[1] || (t[1] = I => o.form.password = I),
+                "onUpdate:modelValue": t[1] || (t[1] = w => o.form.password = w),
                 type: "password",
                 "auto-complete": "off",
                 placeholder: "\u5BC6\u7801",
-                onKeypress: Ze(a.onSubmit, ["enter"])
+                onKeypress: _t(a.onSubmit, ["enter"])
             }, null, 8, ["modelValue", "onKeypress"])]),
             _: 1
         })]),
         _: 1
     }, 8, ["model", "rules"]), u("div", null, [i(y, {
         class: "w-full mt-md",
         type: "primary",
         size: "large",
-        onClick: et(a.onSubmit, ["prevent"])
+        onClick: mt(a.onSubmit, ["prevent"])
     }, {
         default: s(() => [v("\u767B \u5F55")]),
         _: 1
     }, 8, ["onClick"])])])])
 }
-const Ga = w(Fa, [
-        ["render", Ma],
+const eo = I(Ka, [
+        ["render", Za],
         ["__scopeId", "data-v-ea6aa27d"]
     ]),
     ee = [{
         path: "/login",
-        component: Ga,
+        component: eo,
         meta: {
             hidden: !0
         }
     }, {
         path: "/",
         redirect: {
             name: "cert-list"
@@ -1743,15 +1754,15 @@
         },
         redirect: {
             name: "cert-list"
         },
         children: [{
             path: "list",
             name: "cert-list",
-            component: () => h(() => import("./index.af06b2dc.js"), ["index.af06b2dc.js", "event-enums.6c6f25e7.js", "SelectGroup.53d83114.js", "vendor-vue.9e61e0af.js", "ConditionFilterGroup.3c6ac067.js", "../css/ConditionFilterGroup.a91875e6.css", "element-plus.30eb1cab.js", "element-icon.1ce1c350.js", "ConnectStatus.a429b01b.js", "vendor-lib.76301fc3.js"], import.meta.url),
+            component: () => h(() => import("./index.c1800b79.js"), ["index.c1800b79.js", "event-enums.6c6f25e7.js", "SelectGroup.e46bb885.js", "vendor-vue.9e61e0af.js", "ConditionFilterGroup.8b8592a5.js", "../css/ConditionFilterGroup.a91875e6.css", "element-plus.30eb1cab.js", "element-icon.1ce1c350.js", "ConnectStatus.8f8cc994.js", "vendor-lib.76301fc3.js"], import.meta.url),
             meta: {
                 title: "\u8BC1\u4E66\u5217\u8868",
                 icon: "Tickets"
             }
         }]
     }, {
         path: "/domain",
@@ -1763,15 +1774,15 @@
         },
         redirect: {
             name: "domain-list"
         },
         children: [{
             path: "list",
             name: "domain-list",
-            component: () => h(() => import("./index.a8bb8abf.js"), ["index.a8bb8abf.js", "../css/index.302e10d7.css", "event-enums.6c6f25e7.js", "SelectGroup.53d83114.js", "vendor-vue.9e61e0af.js", "SearchUser.f8e52158.js", "ConditionFilterGroup.3c6ac067.js", "../css/ConditionFilterGroup.a91875e6.css", "element-plus.30eb1cab.js", "element-icon.1ce1c350.js", "vendor-lib.76301fc3.js"], import.meta.url),
+            component: () => h(() => import("./index.0bc39ff5.js"), ["index.0bc39ff5.js", "../css/index.26827e91.css", "event-enums.6c6f25e7.js", "SelectGroup.e46bb885.js", "vendor-vue.9e61e0af.js", "SearchUser.8714bea9.js", "ConditionFilterGroup.8b8592a5.js", "../css/ConditionFilterGroup.a91875e6.css", "element-plus.30eb1cab.js", "element-icon.1ce1c350.js", "vendor-lib.76301fc3.js"], import.meta.url),
             meta: {
                 title: "\u57DF\u540D\u5217\u8868",
                 icon: "Coin"
             }
         }]
     }, {
         path: "/group",
@@ -1783,15 +1794,15 @@
         },
         redirect: {
             name: "group-list"
         },
         children: [{
             path: "list",
             name: "group-list",
-            component: () => h(() => import("./index.c22f6489.js"), ["index.c22f6489.js", "vendor-vue.9e61e0af.js", "SelectGroup.53d83114.js", "SearchUser.f8e52158.js", "element-icon.1ce1c350.js", "vendor-lib.76301fc3.js", "element-plus.30eb1cab.js"], import.meta.url),
+            component: () => h(() => import("./index.61002253.js"), ["index.61002253.js", "vendor-vue.9e61e0af.js", "SelectGroup.e46bb885.js", "SearchUser.8714bea9.js", "element-icon.1ce1c350.js", "vendor-lib.76301fc3.js", "element-plus.30eb1cab.js"], import.meta.url),
             meta: {
                 title: "\u5206\u7EC4\u7BA1\u7406",
                 icon: "Files"
             }
         }]
     }, {
         path: "/notify",
@@ -1803,15 +1814,15 @@
         },
         redirect: {
             name: "notify-list"
         },
         children: [{
             path: "edit",
             name: "notify-list",
-            component: () => h(() => import("./index.24e255af.js"), ["index.24e255af.js", "event-enums.6c6f25e7.js", "codemirror-lib.a3a39aa0.js", "vendor-vue.9e61e0af.js", "element-icon.1ce1c350.js", "vendor-lib.76301fc3.js", "element-plus.30eb1cab.js"], import.meta.url),
+            component: () => h(() => import("./index.22cdc255.js"), ["index.22cdc255.js", "event-enums.6c6f25e7.js", "codemirror-lib.a3a39aa0.js", "vendor-vue.9e61e0af.js", "element-icon.1ce1c350.js", "vendor-lib.76301fc3.js", "element-plus.30eb1cab.js"], import.meta.url),
             meta: {
                 title: "\u901A\u77E5\u5217\u8868",
                 icon: "Message"
             }
         }]
     }, {
         path: "/data",
@@ -1819,119 +1830,119 @@
         component: k,
         redirect: {
             name: "data-cert-list"
         },
         meta: {
             title: "\u6570\u636E\u7BA1\u7406",
             icon: "Box",
-            roles: [D.Admin]
+            roles: [C.Admin]
         },
         children: [{
             path: "cert-list",
             name: "data-cert-list",
-            component: () => h(() => import("./index.af06b2dc.js"), ["index.af06b2dc.js", "event-enums.6c6f25e7.js", "SelectGroup.53d83114.js", "vendor-vue.9e61e0af.js", "ConditionFilterGroup.3c6ac067.js", "../css/ConditionFilterGroup.a91875e6.css", "element-plus.30eb1cab.js", "element-icon.1ce1c350.js", "ConnectStatus.a429b01b.js", "vendor-lib.76301fc3.js"], import.meta.url),
+            component: () => h(() => import("./index.c1800b79.js"), ["index.c1800b79.js", "event-enums.6c6f25e7.js", "SelectGroup.e46bb885.js", "vendor-vue.9e61e0af.js", "ConditionFilterGroup.8b8592a5.js", "../css/ConditionFilterGroup.a91875e6.css", "element-plus.30eb1cab.js", "element-icon.1ce1c350.js", "ConnectStatus.8f8cc994.js", "vendor-lib.76301fc3.js"], import.meta.url),
             meta: {
                 title: "\u5168\u90E8\u8BC1\u4E66",
                 icon: "Tickets"
             },
             props: {
-                role: D.Admin
+                role: C.Admin
             }
         }, {
             path: "domain-list",
             name: "data-domain-list",
-            component: () => h(() => import("./index.a8bb8abf.js"), ["index.a8bb8abf.js", "../css/index.302e10d7.css", "event-enums.6c6f25e7.js", "SelectGroup.53d83114.js", "vendor-vue.9e61e0af.js", "SearchUser.f8e52158.js", "ConditionFilterGroup.3c6ac067.js", "../css/ConditionFilterGroup.a91875e6.css", "element-plus.30eb1cab.js", "element-icon.1ce1c350.js", "vendor-lib.76301fc3.js"], import.meta.url),
+            component: () => h(() => import("./index.0bc39ff5.js"), ["index.0bc39ff5.js", "../css/index.26827e91.css", "event-enums.6c6f25e7.js", "SelectGroup.e46bb885.js", "vendor-vue.9e61e0af.js", "SearchUser.8714bea9.js", "ConditionFilterGroup.8b8592a5.js", "../css/ConditionFilterGroup.a91875e6.css", "element-plus.30eb1cab.js", "element-icon.1ce1c350.js", "vendor-lib.76301fc3.js"], import.meta.url),
             meta: {
                 title: "\u5168\u90E8\u57DF\u540D",
                 icon: "Coin"
             },
             props: {
-                role: D.Admin
+                role: C.Admin
             }
         }, {
             path: "group-list",
             name: "data-group-list",
-            component: () => h(() => import("./index.c22f6489.js"), ["index.c22f6489.js", "vendor-vue.9e61e0af.js", "SelectGroup.53d83114.js", "SearchUser.f8e52158.js", "element-icon.1ce1c350.js", "vendor-lib.76301fc3.js", "element-plus.30eb1cab.js"], import.meta.url),
+            component: () => h(() => import("./index.61002253.js"), ["index.61002253.js", "vendor-vue.9e61e0af.js", "SelectGroup.e46bb885.js", "SearchUser.8714bea9.js", "element-icon.1ce1c350.js", "vendor-lib.76301fc3.js", "element-plus.30eb1cab.js"], import.meta.url),
             meta: {
                 title: "\u5168\u90E8\u5206\u7EC4",
                 icon: "Files"
             },
             props: {
-                role: D.Admin
+                role: C.Admin
             }
         }]
     }, {
         path: "/admin",
         name: "admin",
         component: k,
         redirect: {
             name: "admin-user-list"
         },
         meta: {
             title: "\u7CFB\u7EDF\u7BA1\u7406",
             icon: "Setting",
-            roles: [D.Admin]
+            roles: [C.Admin]
         },
         children: [{
             path: "user-list",
             name: "admin-user-list",
-            component: () => h(() => import("./index.deff2c63.js"), ["index.deff2c63.js", "vendor-vue.9e61e0af.js", "vendor-lib.76301fc3.js", "element-plus.30eb1cab.js", "element-icon.1ce1c350.js"], import.meta.url),
+            component: () => h(() => import("./index.e0890673.js"), ["index.e0890673.js", "vendor-vue.9e61e0af.js", "vendor-lib.76301fc3.js", "element-plus.30eb1cab.js", "element-icon.1ce1c350.js"], import.meta.url),
             meta: {
                 title: "\u7528\u6237\u7BA1\u7406",
                 icon: "User",
-                roles: [D.Admin]
+                roles: [C.Admin]
             }
         }, {
             path: "system-setup",
             name: "system-setup",
-            component: () => h(() => import("./index.5b4cd516.js"), ["index.5b4cd516.js", "../css/index.d028ae37.css", "vendor-vue.9e61e0af.js", "element-plus.30eb1cab.js", "element-icon.1ce1c350.js", "vendor-lib.76301fc3.js"], import.meta.url),
+            component: () => h(() => import("./index.435ed104.js"), ["index.435ed104.js", "../css/index.d028ae37.css", "vendor-vue.9e61e0af.js", "element-plus.30eb1cab.js", "element-icon.1ce1c350.js", "vendor-lib.76301fc3.js"], import.meta.url),
             meta: {
                 title: "\u7CFB\u7EDF\u8BBE\u7F6E",
                 icon: "Setting",
-                roles: [D.Admin]
+                roles: [C.Admin]
             }
         }]
     }, {
         path: "/log",
         name: "log",
         component: k,
         redirect: {
             name: "log-scheduler-list"
         },
         meta: {
             title: "\u7CFB\u7EDF\u65E5\u5FD7",
             icon: "Clock",
-            roles: [D.Admin]
+            roles: [C.Admin]
         },
         children: [{
             path: "log-scheduler-list",
             name: "log-scheduler-list",
-            component: () => h(() => import("./index.5f8ece3f.js"), ["index.5f8ece3f.js", "ConnectStatus.a429b01b.js", "vendor-vue.9e61e0af.js", "element-icon.1ce1c350.js", "vendor-lib.76301fc3.js", "element-plus.30eb1cab.js"], import.meta.url),
+            component: () => h(() => import("./index.8410f64d.js"), ["index.8410f64d.js", "ConnectStatus.8f8cc994.js", "vendor-vue.9e61e0af.js", "element-icon.1ce1c350.js", "vendor-lib.76301fc3.js", "element-plus.30eb1cab.js"], import.meta.url),
             meta: {
                 title: "\u76D1\u6D4B\u65E5\u5FD7",
                 icon: "Calendar",
-                roles: [D.Admin]
+                roles: [C.Admin]
             }
         }, {
             path: "log-operation-list",
             name: "log-operation-list",
-            component: () => h(() => import("./index.8c31b31b.js"), ["index.8c31b31b.js", "../css/index.b285e10a.css", "highlight-lib.3654f6d3.js", "vendor-vue.9e61e0af.js", "highlight-util.a4f1867f.js", "element-icon.1ce1c350.js", "vendor-lib.76301fc3.js", "element-plus.30eb1cab.js"], import.meta.url),
+            component: () => h(() => import("./index.47fd0142.js"), ["index.47fd0142.js", "../css/index.b285e10a.css", "highlight-lib.3654f6d3.js", "vendor-vue.9e61e0af.js", "highlight-util.a4f1867f.js", "element-icon.1ce1c350.js", "vendor-lib.76301fc3.js", "element-plus.30eb1cab.js"], import.meta.url),
             meta: {
                 title: "\u64CD\u4F5C\u65E5\u5FD7",
                 icon: "Compass",
-                roles: [D.Admin]
+                roles: [C.Admin]
             }
         }, {
             path: "log-async-task-list",
             name: "log-async-task-list",
-            component: () => h(() => import("./index.0963ab53.js"), ["index.0963ab53.js", "ConnectStatus.a429b01b.js", "vendor-vue.9e61e0af.js", "element-icon.1ce1c350.js", "vendor-lib.76301fc3.js", "element-plus.30eb1cab.js"], import.meta.url),
+            component: () => h(() => import("./index.1cd93e88.js"), ["index.1cd93e88.js", "ConnectStatus.8f8cc994.js", "vendor-vue.9e61e0af.js", "element-icon.1ce1c350.js", "vendor-lib.76301fc3.js", "element-plus.30eb1cab.js"], import.meta.url),
             meta: {
                 title: "\u5F02\u6B65\u4EFB\u52A1",
                 icon: "Compass",
-                roles: [D.Admin]
+                roles: [C.Admin]
             }
         }]
     }, {
         path: "/utils",
         name: "utils",
         component: k,
         redirect: {
@@ -1940,85 +1951,85 @@
         meta: {
             hidden: !0,
             title: "\u5DE5\u5177\u7BB1"
         },
         children: [{
             path: "lab",
             name: "lab",
-            component: () => h(() => import("./index.3b5a616c.js"), ["index.3b5a616c.js", "vendor-vue.9e61e0af.js", "element-icon.1ce1c350.js", "vendor-lib.76301fc3.js", "element-plus.30eb1cab.js"], import.meta.url),
+            component: () => h(() => import("./index.006f8a9f.js"), ["index.006f8a9f.js", "vendor-vue.9e61e0af.js", "element-icon.1ce1c350.js", "vendor-lib.76301fc3.js", "element-plus.30eb1cab.js"], import.meta.url),
             meta: {
                 title: "WHOIS\u67E5\u8BE2",
                 icon: "Box",
                 hidden: !0
             }
         }, {
             path: "domain-cert-list",
             name: "domain-cert-list",
-            component: () => h(() => import("./index.654f7830.js"), ["index.654f7830.js", "vendor-vue.9e61e0af.js", "element-icon.1ce1c350.js", "vendor-lib.76301fc3.js", "element-plus.30eb1cab.js"], import.meta.url),
+            component: () => h(() => import("./index.ab4c92d7.js"), ["index.ab4c92d7.js", "vendor-vue.9e61e0af.js", "element-icon.1ce1c350.js", "vendor-lib.76301fc3.js", "element-plus.30eb1cab.js"], import.meta.url),
             meta: {
                 title: "\u5B50\u57DF\u540D\u8BC1\u4E66\u67E5\u8BE2",
                 icon: "Box",
                 hidden: !0
             }
         }, {
             path: "cert-info",
             name: "cert-info",
-            component: () => h(() => import("./index.ef82c865.js"), ["index.ef82c865.js", "../css/index.a676cc2e.css", "vendor-vue.9e61e0af.js", "element-icon.1ce1c350.js", "vendor-lib.76301fc3.js", "element-plus.30eb1cab.js"], import.meta.url),
+            component: () => h(() => import("./index.bc114a13.js"), ["index.bc114a13.js", "../css/index.a676cc2e.css", "vendor-vue.9e61e0af.js", "element-icon.1ce1c350.js", "vendor-lib.76301fc3.js", "element-plus.30eb1cab.js"], import.meta.url),
             meta: {
                 title: "\u8BC1\u4E66\u4FE1\u606F\u67E5\u8BE2",
                 icon: "Box",
                 hidden: !0
             }
         }, {
             path: "icp-info",
             name: "icp-info",
-            component: () => h(() => import("./index.2ab02c40.js"), ["index.2ab02c40.js", "../css/index.cf805e1c.css", "vendor-vue.9e61e0af.js", "element-icon.1ce1c350.js", "vendor-lib.76301fc3.js", "element-plus.30eb1cab.js"], import.meta.url),
+            component: () => h(() => import("./index.b9d6d972.js"), ["index.b9d6d972.js", "../css/index.cf805e1c.css", "vendor-vue.9e61e0af.js", "element-icon.1ce1c350.js", "vendor-lib.76301fc3.js", "element-plus.30eb1cab.js"], import.meta.url),
             meta: {
                 title: "ICP\u5907\u6848\u67E5\u8BE2",
                 icon: "Box",
                 hidden: !0
             }
         }, {
             path: "issue-certificate-list",
             name: "issue-certificate-list",
-            component: () => h(() => import("./index.0d4c27ce.js"), ["index.0d4c27ce.js", "../css/index.93c714bb.css", "vendor-vue.9e61e0af.js", "vendor-lib.76301fc3.js", "element-plus.30eb1cab.js", "element-icon.1ce1c350.js", "highlight-lib.3654f6d3.js", "highlight-util.a4f1867f.js", "ConnectStatus.a429b01b.js"], import.meta.url),
+            component: () => h(() => import("./index.34d377d3.js"), ["index.34d377d3.js", "../css/index.e21504c8.css", "vendor-vue.9e61e0af.js", "vendor-lib.76301fc3.js", "element-plus.30eb1cab.js", "element-icon.1ce1c350.js", "highlight-lib.3654f6d3.js", "ConnectStatus.8f8cc994.js", "highlight-util.a4f1867f.js"], import.meta.url),
             meta: {
                 title: "SSL\u8BC1\u4E66\u7533\u8BF7",
                 icon: "Box",
                 hidden: !0
             }
         }]
     }];
-const Na = ["/login"];
+const to = ["/login"];
 
-function qa(e) {
+function ao(e) {
     e.beforeEach(async (t, n, m) => {
-        z.start();
+        H.start();
         let o = Q();
         const a = P();
         o && !a.hasUserInfo && await a.updateUserInfo(), !t.matched || t.matched.length == 0 ? m({
             path: "/"
-        }) : Na.includes(t.path) ? m() : a.hasUserInfo ? t.meta && t.meta.roles ? Y(t.meta.roles, a.userRoles) ? m() : m({
+        }) : to.includes(t.path) ? m() : a.hasUserInfo ? t.meta && t.meta.roles ? Y(t.meta.roles, a.userRoles) ? m() : m({
             path: "/"
         }) : m() : m({
             path: "/login",
             query: {
                 redirect: t.fullPath
             }
         })
     }), e.afterEach(() => {
-        z.done()
+        H.done()
     })
 }
-const te = ot({
-    history: it(),
+const te = ft({
+    history: gt(),
     routes: ee
 });
-qa(te);
-const za = te;
+ao(te);
+const oo = te;
 const ae = 0,
     oe = {
         list: [{
             create_time: "2023-05-30 15:42:07",
             id: 1,
             is_show_value: !0,
             key: "mail_host",
@@ -2080,30 +2091,134 @@
             placeholder: "Token\u6709\u6548\u671F\uFF08\u5929\uFF09",
             update_time: "2023-05-30 15:42:07",
             value: "7"
         }],
         total: 7
     },
     ie = "success",
-    Ha = {
+    io = {
         code: ae,
         data: oe,
         msg: ie
     },
-    Wa = Object.freeze(Object.defineProperty({
+    so = Object.freeze(Object.defineProperty({
         __proto__: null,
         code: ae,
         data: oe,
         msg: ie,
-        default: Ha
+        default: io
+    }, Symbol.toStringTag, {
+        value: "Module"
+    })),
+    se = {
+        list: [{
+            id: 3,
+            user_id: 1,
+            task_name: "\u8865\u5168\u57DF\u540DICP\u4FE1\u606F",
+            function_name: "domain_admin.service.domain_info_service.update_all_domain_icp_of_user",
+            status: !0,
+            result: "",
+            start_time: "2023-07-22 17:47:53",
+            end_time: "2023-07-22 17:48:28",
+            create_time: "2023-07-22 17:47:53",
+            update_time: "2023-07-22 17:48:28",
+            create_time_label: "2\u5929\u524D",
+            total_time_label: "35s",
+            total_time: 35,
+            user_name: "admin"
+        }, {
+            id: 2,
+            user_id: 1,
+            task_name: "\u8865\u5168\u57DF\u540DICP\u4FE1\u606F",
+            function_name: "domain_admin.service.domain_info_service.update_all_domain_icp_of_user",
+            status: !0,
+            result: "",
+            start_time: "2023-07-21 09:54:03",
+            end_time: "2023-07-21 09:54:09",
+            create_time: "2023-07-21 09:54:03",
+            update_time: "2023-07-21 09:54:09",
+            create_time_label: "4\u5929\u524D",
+            total_time_label: "6s",
+            total_time: 6,
+            user_name: "admin"
+        }, {
+            id: 1,
+            user_id: 1,
+            task_name: "\u8865\u5168\u57DF\u540DICP\u4FE1\u606F",
+            function_name: "domain_admin.service.domain_info_service.update_all_domain_icp_of_user",
+            status: !0,
+            result: "",
+            start_time: "2023-07-21 09:28:00",
+            end_time: "2023-07-21 09:28:19",
+            create_time: "2023-07-21 09:28:00",
+            update_time: "2023-07-21 09:28:19",
+            create_time_label: "4\u5929\u524D",
+            total_time_label: "19s",
+            total_time: 19,
+            user_name: "admin"
+        }],
+        total: 3
+    },
+    re = 0,
+    ne = "success",
+    ro = {
+        data: se,
+        code: re,
+        msg: ne
+    },
+    no = Object.freeze(Object.defineProperty({
+        __proto__: null,
+        data: se,
+        code: re,
+        msg: ne,
+        default: ro
+    }, Symbol.toStringTag, {
+        value: "Module"
+    })),
+    le = {
+        list: [],
+        total: 0
+    },
+    de = 0,
+    ue = "success",
+    lo = {
+        data: le,
+        code: de,
+        msg: ue
+    },
+    uo = Object.freeze(Object.defineProperty({
+        __proto__: null,
+        data: le,
+        code: de,
+        msg: ue,
+        default: lo
     }, Symbol.toStringTag, {
         value: "Module"
     })),
-    se = 0,
-    re = {
+    _e = {
+        scheduler_cron: "30 10 * * *"
+    },
+    me = 0,
+    ce = "success",
+    _o = {
+        data: _e,
+        code: me,
+        msg: ce
+    },
+    mo = Object.freeze(Object.defineProperty({
+        __proto__: null,
+        data: _e,
+        code: me,
+        msg: ce,
+        default: _o
+    }, Symbol.toStringTag, {
+        value: "Module"
+    })),
+    pe = 0,
+    fe = {
         list: [{
             cert_count: 18,
             create_time: "2023-06-04 17:45:58",
             id: 2,
             name: "\u817E\u8BAF\u7CFB",
             update_time: "2023-06-04 17:45:58",
             user_id: 1
@@ -2127,31 +2242,31 @@
             id: 5,
             name: "\u5934\u6761\u7CFB",
             update_time: "2023-06-22 13:49:43",
             user_id: 1
         }],
         total: 4
     },
-    ne = "success",
-    Ka = {
-        code: se,
-        data: re,
-        msg: ne
+    ge = "success",
+    co = {
+        code: pe,
+        data: fe,
+        msg: ge
     },
-    Ja = Object.freeze(Object.defineProperty({
+    po = Object.freeze(Object.defineProperty({
         __proto__: null,
-        code: se,
-        data: re,
-        msg: ne,
-        default: Ka
+        code: pe,
+        data: fe,
+        msg: ge,
+        default: co
     }, Symbol.toStringTag, {
         value: "Module"
     })),
-    le = 0,
-    de = {
+    he = 0,
+    ye = {
         list: [{
             domain_count: 7,
             id: 0,
             name: "\u672A\u5206\u7EC4"
         }, {
             create_time: "2023-06-04 17:45:58",
             domain_count: 6,
@@ -2179,31 +2294,31 @@
             id: 5,
             name: "\u5934\u6761\u7CFB",
             update_time: "2023-06-22 13:49:43",
             user_id: 1
         }],
         total: 5
     },
-    ue = "success",
-    Qa = {
-        code: le,
-        data: de,
-        msg: ue
+    be = "success",
+    fo = {
+        code: he,
+        data: ye,
+        msg: be
     },
-    Xa = Object.freeze(Object.defineProperty({
+    go = Object.freeze(Object.defineProperty({
         __proto__: null,
-        code: le,
-        data: de,
-        msg: ue,
-        default: Qa
+        code: he,
+        data: ye,
+        msg: be,
+        default: fo
     }, Symbol.toStringTag, {
         value: "Module"
     })),
-    _e = 0,
-    me = {
+    ve = 0,
+    Ie = {
         list: [{
             comment: "-",
             create_time: "2023-06-22 13:53:59",
             domain: "apple.com",
             domain_expire_days: 242,
             domain_expire_time: "2024-02-20 05:00:00",
             domain_start_time: "1987-02-19 05:00:00",
@@ -2391,31 +2506,31 @@
             ssl_count: 1,
             update_time: "2023-06-22 13:54:22",
             update_time_label: "1\u5206\u949F\u524D",
             user_id: 1
         }],
         total: 12
     },
-    ce = "success",
-    Ya = {
-        code: _e,
-        data: me,
-        msg: ce
+    we = "success",
+    ho = {
+        code: ve,
+        data: Ie,
+        msg: we
     },
-    Za = Object.freeze(Object.defineProperty({
+    yo = Object.freeze(Object.defineProperty({
         __proto__: null,
-        code: _e,
-        data: me,
-        msg: ce,
-        default: Ya
+        code: ve,
+        data: Ie,
+        msg: we,
+        default: ho
     }, Symbol.toStringTag, {
         value: "Module"
     })),
-    pe = 0,
-    fe = {
+    Ce = 0,
+    De = {
         list: [{
             address_count: 4,
             alias: "-",
             auto_update: !0,
             expire_status: !0,
             create_time: "2023-06-17 15:47:34",
             create_time_label: "2023-06-17",
@@ -2661,31 +2776,31 @@
             total_days: 0,
             update_time: "2023-06-22 10:34:29",
             update_time_label: "3\u5C0F\u65F6\u524D",
             user_id: 1
         }],
         total: 14
     },
-    ge = "success",
-    eo = {
-        code: pe,
-        data: fe,
-        msg: ge
+    xe = "success",
+    bo = {
+        code: Ce,
+        data: De,
+        msg: xe
     },
-    to = Object.freeze(Object.defineProperty({
+    vo = Object.freeze(Object.defineProperty({
         __proto__: null,
-        code: pe,
-        data: fe,
-        msg: ge,
-        default: eo
+        code: Ce,
+        data: De,
+        msg: xe,
+        default: bo
     }, Symbol.toStringTag, {
         value: "Module"
     })),
-    he = 0,
-    ye = {
+    Ee = 0,
+    ke = {
         list: [{
             cert_count: 6,
             create_time: "2023-06-04 17:45:58",
             domain_count: 0,
             id: 2,
             name: "\u817E\u8BAF\u7CFB",
             update_time: "2023-06-04 17:45:58",
@@ -2713,31 +2828,31 @@
             id: 5,
             name: "\u5934\u6761\u7CFB",
             update_time: "2023-06-22 13:49:43",
             user_id: 1
         }],
         total: 4
     },
-    be = "success",
-    ao = {
-        code: he,
-        data: ye,
-        msg: be
+    Se = "success",
+    Io = {
+        code: Ee,
+        data: ke,
+        msg: Se
     },
-    oo = Object.freeze(Object.defineProperty({
+    wo = Object.freeze(Object.defineProperty({
         __proto__: null,
-        code: he,
-        data: ye,
-        msg: be,
-        default: ao
+        code: Ee,
+        data: ke,
+        msg: Se,
+        default: Io
     }, Symbol.toStringTag, {
         value: "Module"
     })),
-    ve = 0,
-    we = {
+    Le = 0,
+    Be = {
         list: [{
             create_time: "2023-06-22 10:01:00",
             error_message: "",
             id: 38,
             status: !0,
             total_time: null,
             total_time_label: null,
@@ -2813,31 +2928,31 @@
             status: !0,
             total_time: 71,
             total_time_label: "1m 11s",
             update_time: "2023-06-17 10:56:11"
         }],
         total: 38
     },
-    Ie = "success",
-    io = {
-        code: ve,
-        data: we,
-        msg: Ie
+    $e = "success",
+    Co = {
+        code: Le,
+        data: Be,
+        msg: $e
     },
-    so = Object.freeze(Object.defineProperty({
+    Do = Object.freeze(Object.defineProperty({
         __proto__: null,
-        code: ve,
-        data: we,
-        msg: Ie,
-        default: io
+        code: Le,
+        data: Be,
+        msg: $e,
+        default: Co
     }, Symbol.toStringTag, {
         value: "Module"
     })),
-    De = 0,
-    xe = {
+    Oe = 0,
+    Ae = {
         list: [{
             create_time: "2023-06-22 09:40:36",
             event_id: 0,
             expire_days: 3,
             id: 14,
             status: !1,
             type_id: 1,
@@ -2902,57 +3017,57 @@
 }`,
                 corpid: "",
                 corpsecret: ""
             }
         }],
         total: 4
     },
-    Ce = "success",
-    ro = {
-        code: De,
-        data: xe,
-        msg: Ce
+    Ue = "success",
+    xo = {
+        code: Oe,
+        data: Ae,
+        msg: Ue
     },
-    no = Object.freeze(Object.defineProperty({
+    Eo = Object.freeze(Object.defineProperty({
         __proto__: null,
-        code: De,
-        data: xe,
-        msg: Ce,
-        default: ro
+        code: Oe,
+        data: Ae,
+        msg: Ue,
+        default: xo
     }, Symbol.toStringTag, {
         value: "Module"
     })),
-    Ee = 0,
-    ke = {
+    Ve = 0,
+    Fe = {
         create_time: "2022-10-14 18:15:21",
         id: 1,
         type_id: 1,
         update_time: "2022-10-14 18:15:21",
         user_id: 1,
         value: {
             email_list: ["123456@qq.com"]
         }
     },
-    Se = "success",
-    lo = {
-        code: Ee,
-        data: ke,
-        msg: Se
+    Pe = "success",
+    ko = {
+        code: Ve,
+        data: Fe,
+        msg: Pe
     },
-    uo = Object.freeze(Object.defineProperty({
+    So = Object.freeze(Object.defineProperty({
         __proto__: null,
-        code: Ee,
-        data: ke,
-        msg: Se,
-        default: lo
+        code: Ve,
+        data: Fe,
+        msg: Pe,
+        default: ko
     }, Symbol.toStringTag, {
         value: "Module"
     })),
-    Le = 0,
-    Be = {
+    je = 0,
+    Te = {
         list: [{
             after: '{"id": 2, "user_id": 1, "domain": "wenku.baidu.com", "root_domain": "baidu.com", "port": 443, "alias": "", "group_id": 0, "start_time": "2022-07-05 13:16:02", "expire_time": "2023-08-06 13:16:01", "expire_days": 32, "auto_update": true, "is_monitor": true, "is_dynamic_host": false, "connect_status": true, "total_days": 0, "create_time": "2023-06-29 17:32:01", "update_time": "2023-07-05 10:17:30"}',
             before: '{"id": 2, "user_id": 1, "domain": "zhidao.baidu.com", "root_domain": "baidu.com", "port": 443, "alias": "", "group_id": 0, "start_time": "2022-07-05 13:16:02", "expire_time": "2023-08-06 13:16:01", "expire_days": 32, "auto_update": true, "is_monitor": true, "is_dynamic_host": false, "connect_status": true, "total_days": 0, "create_time": "2023-06-29 17:32:01", "update_time": "2023-07-05 10:17:02"}',
             create_time: "2023-07-05 10:17:30",
             create_time_label: "4\u5C0F\u65F6\u524D",
             id: 19,
             table: "tb_domain",
@@ -3068,76 +3183,95 @@
             type_label: "\u5220\u9664",
             update_time: "2023-07-04 22:45:16",
             user_id: 1,
             user_name: "admin"
         }],
         total: 19
     },
-    $e = "success",
-    _o = {
-        code: Le,
-        data: Be,
-        msg: $e
+    Re = "success",
+    Lo = {
+        code: je,
+        data: Te,
+        msg: Re
     },
-    mo = Object.freeze(Object.defineProperty({
+    Bo = Object.freeze(Object.defineProperty({
         __proto__: null,
-        code: Le,
-        data: Be,
-        msg: $e,
-        default: _o
+        code: je,
+        data: Te,
+        msg: Re,
+        default: Lo
     }, Symbol.toStringTag, {
         value: "Module"
     })),
-    Oe = 0,
-    Ue = {
+    Me = {
+        prometheus_key: "x9ax6f1b59u0714c7c5e27fpx4902908"
+    },
+    Ge = 0,
+    Ne = "success",
+    $o = {
+        data: Me,
+        code: Ge,
+        msg: Ne
+    },
+    Oo = Object.freeze(Object.defineProperty({
+        __proto__: null,
+        data: Me,
+        code: Ge,
+        msg: Ne,
+        default: $o
+    }, Symbol.toStringTag, {
+        value: "Module"
+    })),
+    qe = 0,
+    He = {
         version: "latest"
     },
-    Ae = "success",
-    co = {
-        code: Oe,
-        data: Ue,
-        msg: Ae
+    ze = "success",
+    Ao = {
+        code: qe,
+        data: He,
+        msg: ze
     },
-    po = Object.freeze(Object.defineProperty({
+    Uo = Object.freeze(Object.defineProperty({
         __proto__: null,
-        code: Oe,
-        data: Ue,
-        msg: Ae,
-        default: co
+        code: qe,
+        data: He,
+        msg: ze,
+        default: Ao
     }, Symbol.toStringTag, {
         value: "Module"
     })),
-    Ve = 0,
-    Fe = {
+    We = 0,
+    Ke = {
         id: 1,
         username: "admin",
         avatar_url: "",
         before_expire_days: 3,
         email_list: ["email@qq.com"],
         status: !0,
         create_time: "2022-10-03 23:07:21",
         update_time: "2022-10-08 16:54:08"
     },
-    Pe = "success",
-    fo = {
-        code: Ve,
-        data: Fe,
-        msg: Pe
+    Je = "success",
+    Vo = {
+        code: We,
+        data: Ke,
+        msg: Je
     },
-    go = Object.freeze(Object.defineProperty({
+    Fo = Object.freeze(Object.defineProperty({
         __proto__: null,
-        code: Ve,
-        data: Fe,
-        msg: Pe,
-        default: fo
+        code: We,
+        data: Ke,
+        msg: Je,
+        default: Vo
     }, Symbol.toStringTag, {
         value: "Module"
     })),
-    Te = 0,
-    je = {
+    Qe = 0,
+    Xe = {
         list: [{
             avatar_url: "",
             cert_count: 0,
             create_time: "2023-06-04 11:10:09",
             domain_count: 0,
             id: 2,
             notify_count: 0,
@@ -3153,77 +3287,81 @@
             notify_count: 4,
             status: !0,
             update_time: "2023-06-15 22:33:35",
             username: "admin"
         }],
         total: 2
     },
-    Re = "success",
-    ho = {
-        code: Te,
-        data: je,
-        msg: Re
+    Ye = "success",
+    Po = {
+        code: Qe,
+        data: Xe,
+        msg: Ye
     },
-    yo = Object.freeze(Object.defineProperty({
+    jo = Object.freeze(Object.defineProperty({
         __proto__: null,
-        code: Te,
-        data: je,
-        msg: Re,
-        default: ho
+        code: Qe,
+        data: Xe,
+        msg: Ye,
+        default: Po
     }, Symbol.toStringTag, {
         value: "Module"
     })),
-    Me = 0,
-    Ge = {
+    Ze = 0,
+    et = {
         token: "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VyX2lkIjoyLCJleHAiOjE2NjUwNDQ5ODB9.4YnSKathN753sUp4a1njGsFUTanU-xEDoZflHprLYB0"
     },
-    Ne = "success",
-    bo = {
-        code: Me,
-        data: Ge,
-        msg: Ne
+    tt = "success",
+    To = {
+        code: Ze,
+        data: et,
+        msg: tt
     },
-    vo = Object.freeze(Object.defineProperty({
+    Ro = Object.freeze(Object.defineProperty({
         __proto__: null,
-        code: Me,
-        data: Ge,
-        msg: Ne,
-        default: bo
+        code: Ze,
+        data: et,
+        msg: tt,
+        default: To
     }, Symbol.toStringTag, {
         value: "Module"
     })),
     W = Object.assign({
-        "./api/getAllSystemConfig.json": Wa,
-        "./api/getDomainGroupFilter.json": Ja,
-        "./api/getDomainInfoGroupFilter.json": Xa,
-        "./api/getDomainInfoList.json": Za,
-        "./api/getDomainList.json": to,
-        "./api/getGroupList.json": oo,
-        "./api/getLogSchedulerList.json": so,
-        "./api/getNotifyListOfUser.json": no,
-        "./api/getNotifyOfUser.json": uo,
-        "./api/getOperationLogList.json": mo,
-        "./api/getSystemVersion.json": po,
-        "./api/getUserInfo.json": go,
-        "./api/getUserList.json": yo,
-        "./api/login.json": vo
+        "./api/getAllSystemConfig.json": so,
+        "./api/getAsyncTaskLogList.json": no,
+        "./api/getCertificateList.json": uo,
+        "./api/getCronConfig.json": mo,
+        "./api/getDomainGroupFilter.json": po,
+        "./api/getDomainInfoGroupFilter.json": go,
+        "./api/getDomainInfoList.json": yo,
+        "./api/getDomainList.json": vo,
+        "./api/getGroupList.json": wo,
+        "./api/getLogSchedulerList.json": Do,
+        "./api/getNotifyListOfUser.json": Eo,
+        "./api/getNotifyOfUser.json": So,
+        "./api/getOperationLogList.json": Bo,
+        "./api/getSystemEnvConfig.json": Oo,
+        "./api/getSystemVersion.json": Uo,
+        "./api/getUserInfo.json": Fo,
+        "./api/getUserList.json": jo,
+        "./api/login.json": Ro
     }),
-    qe = [];
+    at = [];
 for (let e in W) {
     const t = e.match(/\.(?<apiName>.*)\.json/);
-    qe.push({
+    at.push({
         url: t.groups.apiName,
         data: W[e]
     })
 }
 
-function wo() {
-    for (let e of qe) dt.mock(e.url, e.data)
+function Mo() {
+    for (let e of at) It.mock(e.url, e.data)
 }
-const Io = {
+const Go = {
     name: "app",
     props: {},
     components: {},
     data() {
         return {}
     },
     computed: {},
@@ -3235,39 +3373,39 @@
     },
     created() {
         let e = localStorage.getItem("isCollapse");
         this.setIsCollapse(e == "true"), this.updateVersion()
     }
 };
 
-function Do(e, t, n, m, o, a) {
+function No(e, t, n, m, o, a) {
     const l = r("router-view");
     return d(), p(l)
 }
-const xo = w(Io, [
-    ["render", Do]
+const qo = I(Go, [
+    ["render", No]
 ]);
 
 function K() {
     return window.screen.availWidth < 768
 }({
     VITE_APP_API: "./api",
     VITE_BASE_URL: "./",
     BASE_URL: "./",
     MODE: "production",
     DEV: !1,
     PROD: !0
-}).VITE_MODE == "preview" ? (wo(), K() && (window.location.href = "/domain-admin-mini")) : K() && (window.location.href = "./m");
-const L = st(xo);
+}).VITE_MODE == "preview" ? (Mo(), K() && (window.location.href = "/domain-admin-mini")) : K() && (window.location.href = "./m");
+const L = ht(qo);
 L.config.globalProperties.$http = N;
-L.config.globalProperties.$msg = ht;
-L.use(za);
-L.use(ut, {
-    locale: _t
+L.config.globalProperties.$msg = Lt;
+L.use(oo);
+L.use(wt, {
+    locale: Ct
 });
-for (const [e, t] of Object.entries(nt)) L.component(e, t);
-const Co = rt();
-L.use(Co);
+for (const [e, t] of Object.entries(bt)) L.component(e, t);
+const Ho = yt();
+L.use(Ho);
 L.mount("#app");
 export {
-    N as H, D as R, w as _, mt as d, Bo as r, P as u
+    N as H, C as R, I as _, Dt as d, Qo as r, P as u
 };
```

### Comparing `domain-admin-1.5.8/domain_admin/public/js/index.24e255af.js` & `domain-admin-1.5.9/domain_admin/public/js/index.22cdc255.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -10,15 +10,15 @@
     T as K,
     t as Q,
     o as B,
     j as X
 } from "./codemirror-lib.a3a39aa0.js";
 import {
     _ as V
-} from "./index.165f9ce1.js";
+} from "./index.5c3a2f20.js";
 import {
     ah as i,
     o as b,
     O as x,
     K as Y,
     c as S,
     V as o,
```

### Comparing `domain-admin-1.5.8/domain_admin/public/js/index.2ab02c40.js` & `domain-admin-1.5.9/domain_admin/public/js/index.b9d6d972.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -11,15 +11,15 @@
     T as f,
     U as u,
     az as I,
     aA as k
 } from "./vendor-vue.9e61e0af.js";
 import {
     _ as C
-} from "./index.165f9ce1.js";
+} from "./index.5c3a2f20.js";
 import "./element-icon.1ce1c350.js";
 import "./vendor-lib.76301fc3.js";
 import "./element-plus.30eb1cab.js";
 const V = {
         name: "index",
         props: {},
         components: {},
```

### Comparing `domain-admin-1.5.8/domain_admin/public/js/index.3b5a616c.js` & `domain-admin-1.5.9/domain_admin/public/js/index.006f8a9f.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -8,15 +8,15 @@
     a as i,
     U as w,
     a9 as S,
     T as b
 } from "./vendor-vue.9e61e0af.js";
 import {
     _ as V
-} from "./index.165f9ce1.js";
+} from "./index.5c3a2f20.js";
 import "./element-icon.1ce1c350.js";
 import "./vendor-lib.76301fc3.js";
 import "./element-plus.30eb1cab.js";
 const k = {
         name: "index",
         props: {},
         components: {},
```

### Comparing `domain-admin-1.5.8/domain_admin/public/js/index.5b4cd516.js` & `domain-admin-1.5.9/domain_admin/public/js/index.435ed104.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 import {
     _ as g
-} from "./index.165f9ce1.js";
+} from "./index.5c3a2f20.js";
 import {
     ah as a,
     o as u,
     c as d,
     V as r,
     P as l,
     a as f,
```

### Comparing `domain-admin-1.5.8/domain_admin/public/js/index.5f8ece3f.js` & `domain-admin-1.5.9/domain_admin/public/js/index.8410f64d.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 import {
     C as w
-} from "./ConnectStatus.a429b01b.js";
+} from "./ConnectStatus.8f8cc994.js";
 import {
     _ as m
-} from "./index.165f9ce1.js";
+} from "./index.5c3a2f20.js";
 import {
     ah as l,
     o as _,
     c as f,
     V as a,
     P as n,
     a as c,
```

### Comparing `domain-admin-1.5.8/domain_admin/public/js/index.654f7830.js` & `domain-admin-1.5.9/domain_admin/public/js/index.ab4c92d7.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 import {
     _ as u
-} from "./index.165f9ce1.js";
+} from "./index.5c3a2f20.js";
 import {
     ah as n,
     o as _,
     c as g,
     V as a,
     P as l,
     a as c,
```

### Comparing `domain-admin-1.5.8/domain_admin/public/js/index.8c31b31b.js` & `domain-admin-1.5.9/domain_admin/public/js/index.47fd0142.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 import {
     H as U
 } from "./highlight-lib.3654f6d3.js";
 import {
     _ as H
-} from "./index.165f9ce1.js";
+} from "./index.5c3a2f20.js";
 import {
     ah as m,
     o as b,
     c as O,
     V as f,
     P as h,
     a as w,
```

### Comparing `domain-admin-1.5.8/domain_admin/public/js/index.a8bb8abf.js` & `domain-admin-1.5.9/domain_admin/public/js/index.0bc39ff5.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,25 +1,25 @@
 import {
     i as X,
     E as Z
 } from "./event-enums.6c6f25e7.js";
 import {
     S as q,
     u as $
-} from "./SelectGroup.53d83114.js";
+} from "./SelectGroup.e46bb885.js";
 import {
     S as ee
-} from "./SearchUser.f8e52158.js";
+} from "./SearchUser.8714bea9.js";
 import {
     R as V,
     _ as v,
     u as te,
     d as j,
     r as oe
-} from "./index.165f9ce1.js";
+} from "./index.5c3a2f20.js";
 import {
     ax as G,
     ah as r,
     ar as P,
     Q as A,
     o as m,
     c as y,
@@ -32,23 +32,23 @@
     S as C,
     a9 as H,
     F as U,
     a8 as L,
     az as le,
     aA as ne,
     L as ie,
-    ay as se
+    ay as ae
 } from "./vendor-vue.9e61e0af.js";
 import {
     E as M,
-    A as ae,
+    A as se,
     a as re,
     b as de,
     C as ce
-} from "./ConditionFilterGroup.3c6ac067.js";
+} from "./ConditionFilterGroup.8b8592a5.js";
 import {
     F as me
 } from "./vendor-lib.76301fc3.js";
 import {
     b as ue
 } from "./element-plus.30eb1cab.js";
 import "./element-icon.1ce1c350.js";
@@ -202,15 +202,15 @@
     ye = {
         class: "grid grid-cols-2"
     },
     we = {
         class: "text-center"
     };
 
-function Ce(o, e, t, _, n, s) {
+function Ce(o, e, t, _, n, a) {
     const c = r("el-input"),
         d = r("el-form-item"),
         p = r("el-date-picker"),
         D = r("el-switch"),
         w = r("Warning"),
         x = r("el-icon"),
         k = r("el-link"),
@@ -230,36 +230,36 @@
         default: i(() => [l(d, {
             label: "\u57DF\u540D",
             prop: "domain"
         }, {
             default: i(() => [l(c, {
                 type: "text",
                 modelValue: n.form.domain,
-                "onUpdate:modelValue": e[0] || (e[0] = a => n.form.domain = a),
+                "onUpdate:modelValue": e[0] || (e[0] = s => n.form.domain = s),
                 placeholder: "\u8BF7\u8F93\u5165\u57DF\u540D",
-                onBlur: s.handleDomainChange
+                onBlur: a.handleDomainChange
             }, null, 8, ["modelValue", "onBlur"])]),
             _: 1
         }), l(d, {
             label: "\u57DF\u540D\u65F6\u95F4",
             prop: "start_time"
         }, {
             default: i(() => [u("div", fe, [l(p, {
                 modelValue: n.form.domain_start_time,
-                "onUpdate:modelValue": e[1] || (e[1] = a => n.form.domain_start_time = a),
+                "onUpdate:modelValue": e[1] || (e[1] = s => n.form.domain_start_time = s),
                 type: "date",
                 "value-format": "YYYY-MM-DD HH:mm:ss",
                 placeholder: "\u57DF\u540D\u6CE8\u518C\u65F6\u95F4",
                 disabled: n.form.is_auto_update,
                 style: {
                     width: "170px"
                 }
             }, null, 8, ["modelValue", "disabled"]), ge, l(p, {
                 modelValue: n.form.domain_expire_time,
-                "onUpdate:modelValue": e[2] || (e[2] = a => n.form.domain_expire_time = a),
+                "onUpdate:modelValue": e[2] || (e[2] = s => n.form.domain_expire_time = s),
                 type: "date",
                 "value-format": "YYYY-MM-DD HH:mm:ss",
                 placeholder: "\u57DF\u540D\u5230\u671F\u65F6\u95F4",
                 disabled: n.form.is_auto_update,
                 style: {
                     width: "170px"
                 }
@@ -267,15 +267,15 @@
             _: 1
         }), u("div", be, [l(d, {
             label: "\u81EA\u52A8\u66F4\u65B0",
             prop: "is_auto_update"
         }, {
             default: i(() => [l(D, {
                 modelValue: n.form.is_auto_update,
-                "onUpdate:modelValue": e[3] || (e[3] = a => n.form.is_auto_update = a)
+                "onUpdate:modelValue": e[3] || (e[3] = s => n.form.is_auto_update = s)
             }, null, 8, ["modelValue"]), l(S, {
                 effect: "dark",
                 content: "\u5982\u9700\u624B\u52A8\u8BBE\u7F6E\u8FC7\u671F\u65F6\u95F4\uFF0C\u9700\u5173\u95ED\u81EA\u52A8\u66F4\u65B0",
                 placement: "top-start",
                 "show-after": 500
             }, {
                 default: i(() => [l(k, {
@@ -294,15 +294,15 @@
             _: 1
         }), l(d, {
             label: "\u5B50\u57DF\u8BC1\u4E66",
             prop: "is_auto_subdomain"
         }, {
             default: i(() => [l(D, {
                 modelValue: n.form.is_auto_subdomain,
-                "onUpdate:modelValue": e[4] || (e[4] = a => n.form.is_auto_subdomain = a)
+                "onUpdate:modelValue": e[4] || (e[4] = s => n.form.is_auto_subdomain = s)
             }, null, 8, ["modelValue"]), l(S, {
                 effect: "dark",
                 content: "\u81EA\u52A8\u8BC6\u522B\u5B50\u57DF\u540D\uFF0C\u5E76\u6DFB\u52A0\u8BC1\u4E66\u76D1\u63A7\uFF0C\u4EC5\u672C\u6B21\u63D0\u4EA4\u6709\u6548",
                 placement: "top-start",
                 "show-after": 500
             }, {
                 default: i(() => [l(k, {
@@ -325,106 +325,106 @@
             style: {
                 "align-self": "flex-start"
             }
         }, {
             default: i(() => [l(T, {
                 class: "w-[150px]",
                 modelValue: n.form.group_id,
-                "onUpdate:modelValue": e[5] || (e[5] = a => n.form.group_id = a),
+                "onUpdate:modelValue": e[5] || (e[5] = s => n.form.group_id = s),
                 clearable: ""
             }, null, 8, ["modelValue"])]),
             _: 1
         }), t.role == n.RoleEnum.Admin ? (m(), f(d, {
             key: 0,
             label: "\u8D1F\u8D23\u4EBA",
             prop: "user_id",
             style: {
                 "align-self": "flex-start"
             }
         }, {
             default: i(() => [n.form.user_id ? (m(), f(O, {
                 key: 0,
                 closable: "",
-                onClose: s.handleRemoveUser
+                onClose: a.handleRemoveUser
             }, {
                 default: i(() => [b(h(n.form.user_name), 1)]),
                 _: 1
             }, 8, ["onClose"])) : (m(), f(F, {
                 key: 1,
                 keyword: n.keyword,
-                "onUpdate:keyword": e[6] || (e[6] = a => n.keyword = a),
-                onOnSelect: s.handleSelectUser
+                "onUpdate:keyword": e[6] || (e[6] = s => n.keyword = s),
+                onOnSelect: a.handleSelectUser
             }, null, 8, ["keyword", "onOnSelect"]))]),
             _: 1
         })) : C("", !0)]), l(d, {
             label: "\u6807\u7B7E",
             prop: "tags"
         }, {
             default: i(() => [u("div", null, [l(c, {
                 type: "text",
                 modelValue: n.tag,
-                "onUpdate:modelValue": e[7] || (e[7] = a => n.tag = a),
+                "onUpdate:modelValue": e[7] || (e[7] = s => n.tag = s),
                 placeholder: "\u6807\u7B7E\uFF0C\u56DE\u8F66\u786E\u8BA4",
-                onKeypress: H(s.handleAddTag, ["native", "enter"]),
+                onKeypress: H(a.handleAddTag, ["native", "enter"]),
                 style: {
                     width: "150px"
                 },
                 class: "mr-sm"
-            }, null, 8, ["modelValue", "onKeypress"]), u("div", null, [(m(!0), y(U, null, L(n.form.tags, (a, g) => (m(), f(O, {
+            }, null, 8, ["modelValue", "onKeypress"]), u("div", null, [(m(!0), y(U, null, L(n.form.tags, (s, g) => (m(), f(O, {
                 closable: "",
-                onClose: z => s.handleCloseTag(g)
+                onClose: z => a.handleCloseTag(g)
             }, {
-                default: i(() => [b(h(a), 1)]),
+                default: i(() => [b(h(s), 1)]),
                 _: 2
             }, 1032, ["onClose"]))), 256))])])]),
             _: 1
         }), l(d, {
             label: "\u4E3B\u529E\u5355\u4F4D",
             prop: "icp_company"
         }, {
             default: i(() => [l(c, {
                 type: "text",
                 modelValue: n.form.icp_company,
-                "onUpdate:modelValue": e[8] || (e[8] = a => n.form.icp_company = a),
+                "onUpdate:modelValue": e[8] || (e[8] = s => n.form.icp_company = s),
                 placeholder: "\u8BF7\u8F93\u5165\u4E3B\u529E\u5355\u4F4D\u540D\u79F0"
             }, null, 8, ["modelValue"])]),
             _: 1
         }), l(d, {
             label: "ICP\u5907\u6848",
             prop: "icp_licence"
         }, {
             default: i(() => [l(c, {
                 type: "text",
                 modelValue: n.form.icp_licence,
-                "onUpdate:modelValue": e[9] || (e[9] = a => n.form.icp_licence = a),
+                "onUpdate:modelValue": e[9] || (e[9] = s => n.form.icp_licence = s),
                 placeholder: "\u8BF7\u8F93\u5165ICP\u5907\u6848"
             }, null, 8, ["modelValue"])]),
             _: 1
         }), l(d, {
             label: "\u5907\u6CE8",
             prop: "comment"
         }, {
             default: i(() => [l(c, {
                 type: "textarea",
                 modelValue: n.form.comment,
-                "onUpdate:modelValue": e[10] || (e[10] = a => n.form.comment = a),
+                "onUpdate:modelValue": e[10] || (e[10] = s => n.form.comment = s),
                 rows: 3,
                 placeholder: "\u8BF7\u8F93\u5165\u5907\u6CE8"
             }, null, 8, ["modelValue"])]),
             _: 1
         })]),
         _: 1
     }, 8, ["model", "rules"]), u("div", we, [l(R, {
-        onClick: s.handleCancel
+        onClick: a.handleCancel
     }, {
         default: i(() => [b("\u53D6 \u6D88")]),
         _: 1
     }, 8, ["onClick"]), l(R, {
         type: "primary",
-        onClick: s.handleSubmit
+        onClick: a.handleSubmit
     }, {
         default: i(() => [b("\u786E \u5B9A")]),
         _: 1
     }, 8, ["onClick"])])])), [
         [E, n.loading]
     ])
 }
@@ -478,32 +478,32 @@
             handleSuccess() {
                 this.handleClose(), this.$emit("on-success")
             }
         },
         created() {}
     };
 
-function ve(o, e, t, _, n, s) {
+function ve(o, e, t, _, n, a) {
     const c = r("DataForm"),
         d = r("el-dialog");
     return m(), f(d, {
-        title: s.dialogTitle,
-        modelValue: s.dialogVisible,
-        "onUpdate:modelValue": e[0] || (e[0] = p => s.dialogVisible = p),
+        title: a.dialogTitle,
+        modelValue: a.dialogVisible,
+        "onUpdate:modelValue": e[0] || (e[0] = p => a.dialogVisible = p),
         width: "500px",
         center: "",
         "append-to-body": "",
         "lock-scroll": !1
     }, {
-        default: i(() => [s.dialogVisible ? (m(), f(c, {
+        default: i(() => [a.dialogVisible ? (m(), f(c, {
             key: 0,
             row: t.row,
             role: t.role,
-            onOnCancel: s.handleClose,
-            onOnSuccess: s.handleSuccess
+            onOnCancel: a.handleClose,
+            onOnSuccess: a.handleSuccess
         }, null, 8, ["row", "role", "onOnCancel", "onOnSuccess"])) : C("", !0)]),
         _: 1
     }, 8, ["title", "modelValue"])
 }
 const Y = v(ke, [
     ["render", ve]
 ]);
@@ -533,32 +533,32 @@
             }
             const e = this.$refs.ShowOverflowTooltip;
             console.log(e);
             const t = document.createRange();
             t.setStart(e, 0), t.setEnd(e, e.childNodes.length);
             const _ = t.getBoundingClientRect().width,
                 n = (parseInt(o(e, "paddingLeft"), 10) || 0) + (parseInt(o(e, "paddingRight"), 10) || 0);
-            let s = {
+            let a = {
                 rangeWidth: _,
                 padding: n,
                 "rangeWidth+padding": _ + n,
                 offsetWidth: e.offsetWidth,
                 scrollWidth: e.scrollWidth
             };
-            console.table(s), _ + n > e.offsetWidth || e.scrollWidth > e.offsetWidth ? (console.log("\u6709\u9690\u85CF\u6587\u5B57..."), this.content && this.content.length > 5 ? this.disabled = !1 : this.disabled = !0) : (console.log("\u6CA1\u6709\u9690\u85CF\u6587\u5B57"), this.disabled = !0)
+            console.table(a), _ + n > e.offsetWidth || e.scrollWidth > e.offsetWidth ? (console.log("\u6709\u9690\u85CF\u6587\u5B57..."), this.content && this.content.length > 5 ? this.disabled = !1 : this.disabled = !0) : (console.log("\u6CA1\u6709\u9690\u85CF\u6587\u5B57"), this.disabled = !0)
         }
     },
     mounted() {
         this.$nextTick(() => {
             this.handleInit()
         })
     }
 };
 
-function Se(o, e, t, _, n, s) {
+function Se(o, e, t, _, n, a) {
     const c = r("el-tooltip");
     return m(), f(c, {
         effect: "dark",
         disabled: n.disabled,
         content: t.content,
         placement: "top-start"
     }, {
@@ -579,15 +579,15 @@
             row: {
                 type: Object,
                 default: null
             }
         },
         components: {
             ExpireDays: M,
-            AddressList: ae,
+            AddressList: se,
             ShowOverflowTooltip: Ie
         },
         data() {
             return {
                 form: {
                     domain: "",
                     domain_url: "",
@@ -712,15 +712,15 @@
     $e = {
         class: "truncate"
     },
     Ne = {
         class: "text-center mt-md"
     };
 
-function Ge(o, e, t, _, n, s) {
+function Ge(o, e, t, _, n, a) {
     const c = r("el-link"),
         d = r("el-form-item"),
         p = r("ShowOverflowTooltip"),
         D = r("el-form"),
         w = r("ExpireDays"),
         x = r("Refresh"),
         k = r("el-icon"),
@@ -791,15 +791,15 @@
             label: "\u68C0\u67E5\u65F6\u95F4",
             prop: "isp"
         }, {
             default: i(() => [u("div", Te, [u("span", Fe, h(n.form.update_time_label || "-"), 1), l(c, {
                 underline: !1,
                 type: "primary",
                 class: "mr-sm",
-                onClick: s.handleUpdateRowDomainInfo
+                onClick: a.handleUpdateRowDomainInfo
             }, {
                 default: i(() => [l(k, null, {
                     default: i(() => [l(x)]),
                     _: 1
                 })]),
                 _: 1
             }, 8, ["onClick"])])]),
@@ -838,15 +838,15 @@
         }, {
             default: i(() => [u("span", $e, h(n.form.comment || "-"), 1)]),
             _: 1
         })]),
         _: 1
     })]), u("div", Ne, [l(S, {
         type: "primary",
-        onClick: s.handleCancel
+        onClick: a.handleCancel
     }, {
         default: i(() => [b("\u5173 \u95ED")]),
         _: 1
     }, 8, ["onClick"])])])
 }
 const Le = v(Ve, [
         ["render", Ge]
@@ -896,32 +896,32 @@
             handleDialogClose() {
                 this.$emit("on-success")
             }
         },
         created() {}
     };
 
-function je(o, e, t, _, n, s) {
+function je(o, e, t, _, n, a) {
     const c = r("DataForm"),
         d = r("el-dialog");
     return m(), f(d, {
         title: "\u57DF\u540D\u8BE6\u60C5",
-        modelValue: s.dialogVisible,
-        "onUpdate:modelValue": e[0] || (e[0] = p => s.dialogVisible = p),
+        modelValue: a.dialogVisible,
+        "onUpdate:modelValue": e[0] || (e[0] = p => a.dialogVisible = p),
         width: "800px",
         center: "",
         "append-to-body": "",
         "lock-scroll": !1,
-        onClose: s.handleDialogClose
+        onClose: a.handleDialogClose
     }, {
-        default: i(() => [s.dialogVisible ? (m(), f(c, {
+        default: i(() => [a.dialogVisible ? (m(), f(c, {
             key: 0,
             row: t.row,
-            onOnCancel: s.handleClose,
-            onOnSuccess: s.handleSuccess
+            onOnCancel: a.handleClose,
+            onOnSuccess: a.handleSuccess
         }, null, 8, ["row", "onOnCancel", "onOnSuccess"])) : C("", !0)]),
         _: 1
     }, 8, ["modelValue", "onClose"])
 }
 const qe = v(We, [
         ["render", je]
     ]),
@@ -1057,15 +1057,15 @@
     Ke = {
         class: "domain-info-list__table__tag"
     },
     Je = {
         key: 1
     };
 
-function Qe(o, e, t, _, n, s) {
+function Qe(o, e, t, _, n, a) {
     const c = r("el-table-column"),
         d = r("el-link"),
         p = r("ExpireDays"),
         D = r("el-tag"),
         w = r("Refresh"),
         x = r("el-icon"),
         k = r("el-switch"),
@@ -1076,140 +1076,140 @@
         B = r("DataFormDialog"),
         R = r("DataDetailDialog"),
         E = r("AddressListgDialog");
     return m(), y("div", null, [l(F, ie({
         stripe: "",
         border: ""
     }, o.$attrs, {
-        onSortChange: e[0] || (e[0] = a => o.$emit("sort-change", a)),
-        onSelectionChange: e[1] || (e[1] = a => o.$emit("selection-change", a))
+        onSortChange: e[0] || (e[0] = s => o.$emit("sort-change", s)),
+        onSelectionChange: e[1] || (e[1] = s => o.$emit("selection-change", s))
     }), {
         default: i(() => [t.role == n.RoleEnum.User ? (m(), f(c, {
             key: 0,
             type: "selection",
             "header-align": "center",
             align: "center",
             width: "40",
-            selectable: s.handleSelectable
+            selectable: a.handleSelectable
         }, null, 8, ["selectable"])) : C("", !0), l(c, {
             label: "\u57DF\u540D",
             "header-align": "center",
             align: "center",
             width: "250",
             "show-overflow-tooltip": "",
             prop: "domain"
         }, {
-            default: i(a => [l(d, {
+            default: i(s => [l(d, {
                 underline: !1,
-                onClick: g => s.handleShowDetail(a.row)
+                onClick: g => a.handleShowDetail(s.row)
             }, {
-                default: i(() => [b(h(a.row.domain), 1)]),
+                default: i(() => [b(h(s.row.domain), 1)]),
                 _: 2
             }, 1032, ["onClick"])]),
             _: 1
         }), l(c, {
             label: "\u57DF\u540D\u5929\u6570",
             "header-align": "center",
             align: "center",
             width: "90",
             sortable: "custom",
             prop: "domain_expire_days"
         }, {
-            default: i(a => [l(p, {
-                value: a.row.real_domain_expire_days
+            default: i(s => [l(p, {
+                value: s.row.real_domain_expire_days
             }, null, 8, ["value"])]),
             _: 1
         }), l(c, {
             label: "\u8BC1\u4E66\u6570\u91CF",
             "header-align": "center",
             align: "center",
             width: "100"
         }, {
-            default: i(a => [a.row.ssl_count && a.row.ssl_count > 0 ? (m(), f(d, {
+            default: i(s => [s.row.ssl_count && s.row.ssl_count > 0 ? (m(), f(d, {
                 key: 0,
                 underline: !1,
-                onClick: g => s.handleCertCountClick(a.row)
+                onClick: g => a.handleCertCountClick(s.row)
             }, {
-                default: i(() => [b(h(a.row.ssl_count), 1)]),
+                default: i(() => [b(h(s.row.ssl_count), 1)]),
                 _: 2
             }, 1032, ["onClick"])) : (m(), y("span", Ye, "-"))]),
             _: 1
         }), l(c, {
             label: "\u5206\u7EC4",
             "header-align": "center",
             align: "center",
             width: "100",
             sortable: "custom",
             prop: "group_name"
         }, {
-            default: i(a => [u("span", null, h(a.row.group_name || "-"), 1)]),
+            default: i(s => [u("span", null, h(s.row.group_name || "-"), 1)]),
             _: 1
         }), l(c, {
             label: "\u6807\u7B7E",
             "header-align": "center",
             align: "left",
             width: "100",
             prop: "tags",
             "show-overflow-tooltip": ""
         }, {
-            default: i(a => [a.row.tags && a.row.tags.length > 0 ? (m(!0), y(U, {
+            default: i(s => [s.row.tags && s.row.tags.length > 0 ? (m(!0), y(U, {
                 key: 0
-            }, L(a.row.tags, (g, z) => (m(), y("div", Ke, [l(D, {
-                onClick: W => s.handleTagClick(g),
+            }, L(s.row.tags, (g, z) => (m(), y("div", Ke, [l(D, {
+                onClick: W => a.handleTagClick(g),
                 class: "cursor-pointer"
             }, {
                 default: i(() => [b(h(g), 1)]),
                 _: 2
             }, 1032, ["onClick"])]))), 256)) : (m(), y("span", Je, "-"))]),
             _: 1
         }), l(c, {
             label: "\u5907\u6CE8",
             "header-align": "center",
             align: "left",
             prop: "comment",
             "show-overflow-tooltip": ""
         }, {
-            default: i(a => [u("span", null, h(a.row.comment || "-"), 1)]),
+            default: i(s => [u("span", null, h(s.row.comment || "-"), 1)]),
             _: 1
         }), t.tableColumns.includes("icp_company") ? (m(), f(c, {
             key: 1,
             label: "\u4E3B\u529E\u5355\u4F4D\u540D\u79F0",
             "header-align": "center",
             align: "left",
             width: "200",
             prop: "icp_company",
             "show-overflow-tooltip": ""
         }, {
-            default: i(a => [u("span", null, h(a.row.icp_company || "-"), 1)]),
+            default: i(s => [u("span", null, h(s.row.icp_company || "-"), 1)]),
             _: 1
         })) : C("", !0), t.tableColumns.includes("icp_licence") ? (m(), f(c, {
             key: 2,
             label: "ICP\u5907\u6848",
             "header-align": "center",
             align: "left",
             width: "200",
             prop: "icp_licence",
             "show-overflow-tooltip": ""
         }, {
-            default: i(a => [u("span", null, h(a.row.icp_licence || "-"), 1)]),
+            default: i(s => [u("span", null, h(s.row.icp_licence || "-"), 1)]),
             _: 1
         })) : C("", !0), t.tableColumns.includes("update_icp") ? (m(), f(c, {
             key: 3,
             label: "\u66F4\u65B0ICP",
             "header-align": "center",
             align: "center",
             width: "70",
             prop: "update_icp",
             "show-overflow-tooltip": ""
         }, {
-            default: i(a => [l(d, {
+            default: i(s => [l(d, {
                 underline: !1,
                 type: "primary",
                 class: "mr-sm",
-                onClick: g => s.handleUpdateRowICP(a.row)
+                onClick: g => a.handleUpdateRowICP(s.row)
             }, {
                 default: i(() => [l(x, null, {
                     default: i(() => [l(w)]),
                     _: 1
                 })]),
                 _: 2
             }, 1032, ["onClick"])]),
@@ -1219,122 +1219,133 @@
             label: "\u8D1F\u8D23\u4EBA",
             "header-align": "center",
             align: "center",
             width: "80",
             prop: "user_id",
             "show-overflow-tooltip": ""
         }, {
-            default: i(a => [u("span", null, h(a.row.user_name), 1)]),
+            default: i(s => [u("span", null, h(s.row.user_name), 1)]),
             _: 1
-        })) : C("", !0), t.role == n.RoleEnum.User ? (m(), y(U, {
+        })) : C("", !0), l(c, {
+            label: "\u66F4\u65B0\u65F6\u95F4",
+            "header-align": "center",
+            align: "center",
+            width: "110",
+            prop: "update_time",
+            sortable: "custom",
+            "show-overflow-tooltip": ""
+        }, {
+            default: i(s => [u("span", null, h(s.row.update_time_label || "-"), 1)]),
+            _: 1
+        }), t.role == n.RoleEnum.User ? (m(), y(U, {
             key: 5
         }, [l(c, {
             label: "\u81EA\u52A8\u66F4\u65B0",
             width: "90",
             "header-align": "center",
             align: "center",
             sortable: "custom",
             prop: "domain_expire_monitor"
         }, {
-            default: i(a => [l(k, {
-                modelValue: a.row.is_auto_update,
-                "onUpdate:modelValue": g => a.row.is_auto_update = g,
-                disabled: !a.row.has_edit_permission,
-                onChange: g => s.handleAutoUpdateStatusChange(a.row, g)
+            default: i(s => [l(k, {
+                modelValue: s.row.is_auto_update,
+                "onUpdate:modelValue": g => s.row.is_auto_update = g,
+                disabled: !s.row.has_edit_permission,
+                onChange: g => a.handleAutoUpdateStatusChange(s.row, g)
             }, null, 8, ["modelValue", "onUpdate:modelValue", "disabled", "onChange"])]),
             _: 1
         }), l(c, {
             label: "\u5230\u671F\u63D0\u9192",
             width: "90",
             "header-align": "center",
             align: "center",
             sortable: "custom",
             prop: "is_expire_monitor"
         }, {
-            default: i(a => [l(k, {
-                modelValue: a.row.is_expire_monitor,
-                "onUpdate:modelValue": g => a.row.is_expire_monitor = g,
-                disabled: !a.row.has_edit_permission,
-                onChange: g => s.handleMonitorStatusChange(a.row, g)
+            default: i(s => [l(k, {
+                modelValue: s.row.is_expire_monitor,
+                "onUpdate:modelValue": g => s.row.is_expire_monitor = g,
+                disabled: !s.row.has_edit_permission,
+                onChange: g => a.handleMonitorStatusChange(s.row, g)
             }, null, 8, ["modelValue", "onUpdate:modelValue", "disabled", "onChange"])]),
             _: 1
         })], 64)) : C("", !0), l(c, {
             label: "\u64CD\u4F5C",
             width: "100",
             "header-align": "center",
             align: "center"
         }, {
-            default: i(a => [l(d, {
+            default: i(s => [l(d, {
                 underline: !1,
                 type: "primary",
                 class: "mr-sm",
-                onClick: g => s.handleUpdateRowDomainInfo(a.row)
+                onClick: g => a.handleUpdateRowDomainInfo(s.row)
             }, {
                 default: i(() => [l(x, null, {
                     default: i(() => [l(w)]),
                     _: 1
                 })]),
                 _: 2
             }, 1032, ["onClick"]), l(d, {
                 underline: !1,
                 type: "primary",
                 class: "mr-sm",
-                disabled: !a.row.has_edit_permission,
-                onClick: g => s.handleEditRow(a.row)
+                disabled: !s.row.has_edit_permission,
+                onClick: g => a.handleEditRow(s.row)
             }, {
                 default: i(() => [l(x, null, {
                     default: i(() => [l(S)]),
                     _: 1
                 })]),
                 _: 2
             }, 1032, ["disabled", "onClick"]), l(O, {
                 title: "\u786E\u5B9A\u5220\u9664\uFF1F",
-                onConfirm: g => s.handleDeleteClick(a.row),
-                disabled: !a.row.has_edit_permission
+                onConfirm: g => a.handleDeleteClick(s.row),
+                disabled: !s.row.has_edit_permission
             }, {
                 reference: i(() => [l(d, {
                     underline: !1,
                     type: "danger",
-                    disabled: !a.row.has_edit_permission
+                    disabled: !s.row.has_edit_permission
                 }, {
                     default: i(() => [l(x, null, {
                         default: i(() => [l(T)]),
                         _: 1
                     })]),
                     _: 2
                 }, 1032, ["disabled"])]),
                 _: 2
             }, 1032, ["onConfirm", "disabled"])]),
             _: 1
         })]),
         _: 1
     }, 16), l(B, {
         visible: n.dialogVisible,
-        "onUpdate:visible": e[2] || (e[2] = a => n.dialogVisible = a),
+        "onUpdate:visible": e[2] || (e[2] = s => n.dialogVisible = s),
         row: n.currentRow,
         role: t.role,
-        onOnSuccess: e[3] || (e[3] = a => s.handleRefreshRow(n.currentRow))
+        onOnSuccess: e[3] || (e[3] = s => a.handleRefreshRow(n.currentRow))
     }, null, 8, ["visible", "row", "role"]), l(R, {
         row: n.currentRow,
         role: t.role,
         visible: n.dialogDetailVisible,
-        "onUpdate:visible": e[4] || (e[4] = a => n.dialogDetailVisible = a),
-        onOnSuccess: e[5] || (e[5] = a => s.handleRefreshRow(n.currentRow))
+        "onUpdate:visible": e[4] || (e[4] = s => n.dialogDetailVisible = s),
+        onOnSuccess: e[5] || (e[5] = s => a.handleRefreshRow(n.currentRow))
     }, null, 8, ["row", "role", "visible"]), n.currentRow ? (m(), f(E, {
         key: 0,
         domainId: n.currentRow.id,
         role: t.role,
         visible: n.AddressListgDialogVisible,
-        "onUpdate:visible": e[6] || (e[6] = a => n.AddressListgDialogVisible = a),
-        onOnSuccess: s.handleUpdateSuccess
+        "onUpdate:visible": e[6] || (e[6] = s => n.AddressListgDialogVisible = s),
+        onOnSuccess: a.handleUpdateSuccess
     }, null, 8, ["domainId", "role", "visible", "onOnSuccess"])) : C("", !0)])
 }
 const Xe = v(Me, [
         ["render", Qe],
-        ["__scopeId", "data-v-36c42171"]
+        ["__scopeId", "data-v-2a537759"]
     ]),
     Ze = {
         name: "updateDomainInfo",
         props: {},
         components: {},
         data() {
             return {
@@ -1356,28 +1367,28 @@
         },
         beforeUnmount() {
             clearInterval(this.updateTimer), this.updateTimer = null
         },
         created() {}
     };
 
-function et(o, e, t, _, n, s) {
+function et(o, e, t, _, n, a) {
     const c = r("Refresh"),
         d = r("el-icon"),
         p = r("el-link");
     return m(), f(p, {
         underline: !1,
         type: "primary",
-        onClick: s.updateAllDomainCertInfoOfUser,
-        disabled: s.disableUpdateButton
+        onClick: a.updateAllDomainCertInfoOfUser,
+        disabled: a.disableUpdateButton
     }, {
         default: i(() => [l(d, null, {
             default: i(() => [l(c)]),
             _: 1
-        }), b(h(s.updateText), 1)]),
+        }), b(h(a.updateText), 1)]),
         _: 1
     }, 8, ["onClick", "disabled"])
 }
 const tt = v(Ze, [
         ["render", et]
     ]),
     ot = {
@@ -1404,28 +1415,28 @@
         },
         beforeUnmount() {
             clearInterval(this.updateTimer), this.updateTimer = null
         },
         created() {}
     };
 
-function lt(o, e, t, _, n, s) {
+function lt(o, e, t, _, n, a) {
     const c = r("Refresh"),
         d = r("el-icon"),
         p = r("el-link");
     return m(), f(p, {
         underline: !1,
         type: "primary",
-        onClick: s.updateAllDomainCertInfoOfUser,
-        disabled: s.disableUpdateButton
+        onClick: a.updateAllDomainCertInfoOfUser,
+        disabled: a.disableUpdateButton
     }, {
         default: i(() => [l(d, null, {
             default: i(() => [l(c)]),
             _: 1
-        }), b(h(s.updateText), 1)]),
+        }), b(h(a.updateText), 1)]),
         _: 1
     }, 8, ["onClick", "disabled"])
 }
 const nt = v(ot, [
         ["render", lt]
     ]),
     it = {
@@ -1468,33 +1479,33 @@
         },
         beforeUnmount() {
             clearInterval(this.updateTimer), this.updateTimer = null
         },
         created() {}
     };
 
-function st(o, e, t, _, n, s) {
+function at(o, e, t, _, n, a) {
     const c = r("Position"),
         d = r("el-icon"),
         p = r("el-link");
     return m(), f(p, {
         underline: !1,
         type: "primary",
-        onClick: s.handleNotifyByEventId,
-        disabled: s.disableUpdateButton
+        onClick: a.handleNotifyByEventId,
+        disabled: a.disableUpdateButton
     }, {
         default: i(() => [l(d, null, {
             default: i(() => [l(c)]),
             _: 1
-        }), b(h(s.updateText), 1)]),
+        }), b(h(a.updateText), 1)]),
         _: 1
     }, 8, ["onClick", "disabled"])
 }
-const at = v(it, [
-        ["render", st]
+const st = v(it, [
+        ["render", at]
     ]),
     rt = {
         name: "ConditionFilter",
         props: {},
         components: {
             ConditionFilterGroup: ce
         },
@@ -1555,20 +1566,20 @@
             this.resetData()
         }
     },
     dt = {
         class: ""
     };
 
-function ct(o, e, t, _, n, s) {
+function ct(o, e, t, _, n, a) {
     const c = r("ConditionFilterGroup"),
         d = P("loading");
     return A((m(), y("div", dt, [l(c, {
         options: n.options,
-        onOnChange: s.handleChange
+        onOnChange: a.handleChange
     }, null, 8, ["options", "onOnChange"])])), [
         [d, n.loading]
     ])
 }
 const mt = v(rt, [
         ["render", ct]
     ]),
@@ -1607,15 +1618,15 @@
             this.form.fields = N()
         }
     },
     _t = {
         class: "text-center"
     };
 
-function pt(o, e, t, _, n, s) {
+function pt(o, e, t, _, n, a) {
     const c = r("el-checkbox"),
         d = r("el-checkbox-group"),
         p = r("el-form-item"),
         D = r("el-form"),
         w = r("el-button"),
         x = P("loading");
     return A((m(), y("div", null, [l(D, {
@@ -1640,21 +1651,21 @@
                 }, 1032, ["label"]))), 256))]),
                 _: 1
             }, 8, ["modelValue"])]),
             _: 1
         })]),
         _: 1
     }, 8, ["model", "rules"]), u("div", _t, [l(w, {
-        onClick: s.handleCancel
+        onClick: a.handleCancel
     }, {
         default: i(() => [b("\u53D6 \u6D88")]),
         _: 1
     }, 8, ["onClick"]), l(w, {
         type: "primary",
-        onClick: s.handleSubmit
+        onClick: a.handleSubmit
     }, {
         default: i(() => [b("\u786E \u5B9A")]),
         _: 1
     }, 8, ["onClick"])])])), [
         [x, o.loading]
     ])
 }
@@ -1700,31 +1711,31 @@
             handleSuccess() {
                 this.handleClose(), this.$emit("on-success")
             }
         },
         created() {}
     };
 
-function gt(o, e, t, _, n, s) {
+function gt(o, e, t, _, n, a) {
     const c = r("TableColumnSetForm"),
         d = r("el-dialog");
     return m(), f(d, {
         title: "\u8868\u683C\u8BBE\u7F6E",
-        modelValue: s.dialogVisible,
-        "onUpdate:modelValue": e[0] || (e[0] = p => s.dialogVisible = p),
+        modelValue: a.dialogVisible,
+        "onUpdate:modelValue": e[0] || (e[0] = p => a.dialogVisible = p),
         width: "500px",
         center: "",
         "append-to-body": "",
         "lock-scroll": !1
     }, {
-        default: i(() => [s.dialogVisible ? (m(), f(c, {
+        default: i(() => [a.dialogVisible ? (m(), f(c, {
             key: 0,
             row: t.row,
-            onOnCancel: s.handleClose,
-            onOnSuccess: s.handleSuccess
+            onOnCancel: a.handleClose,
+            onOnSuccess: a.handleSuccess
         }, null, 8, ["row", "onOnCancel", "onOnSuccess"])) : C("", !0)]),
         _: 1
     }, 8, ["modelValue"])
 }
 const bt = v(ft, [
         ["render", gt]
     ]),
@@ -1744,23 +1755,23 @@
             showDialog() {
                 this.visible = !0
             }
         },
         created() {}
     };
 
-function wt(o, e, t, _, n, s) {
+function wt(o, e, t, _, n, a) {
     const c = r("Setting"),
         d = r("el-icon"),
         p = r("el-link"),
         D = r("TableColumnSetDialog");
     return m(), y(U, null, [l(p, {
         underline: !1,
         type: "primary",
-        onClick: s.showDialog
+        onClick: a.showDialog
     }, {
         default: i(() => [l(d, null, {
             default: i(() => [l(c)]),
             _: 1
         }), b("\u8868\u683C\u8BBE\u7F6E")]),
         _: 1
     }, 8, ["onClick"]), l(D, {
@@ -1781,15 +1792,15 @@
             }
         },
         components: {
             DataFormDialog: Y,
             DataTable: Xe,
             SelectGroup: q,
             UpdateDomainInfo: tt,
-            CheckDomainInfo: at,
+            CheckDomainInfo: st,
             ConditionFilter: mt,
             UpdateDomainICP: nt,
             TableColumnSet: Ct
         },
         data() {
             return {
                 tableColumns: [],
@@ -1817,15 +1828,15 @@
                 groupOptions: "getGroupOptions"
             }),
             showBatchDeleteButton() {
                 return !!(this.selectedRows && this.selectedRows.length > 0)
             }
         },
         methods: {
-            ...se($, {
+            ...ae($, {
                 updateGroupOptions: "updateGroupOptions"
             }),
             resetData() {
                 this.page = 1, this.getData()
             },
             refreshData() {
                 this.getData()
@@ -1971,38 +1982,38 @@
             top: "0",
             left: "0",
             right: "0",
             bottom: "0"
         }
     }, null, -1);
 
-function Ut(o, e, t, _, n, s) {
+function Ut(o, e, t, _, n, a) {
     const c = r("Plus"),
         d = r("el-icon"),
         p = r("el-button"),
         D = r("Search"),
         w = r("el-input"),
         x = r("ConditionFilter"),
         k = r("Delete"),
         S = r("el-link"),
         T = r("el-popconfirm"),
         O = r("UpdateDomainInfo"),
         F = r("UpdateDomainICP"),
         B = r("CheckDomainInfo"),
         R = r("Upload"),
         E = r("el-upload"),
-        a = r("Download"),
+        s = r("Download"),
         g = r("TableColumnSet"),
         z = r("DataTable"),
         W = r("el-pagination"),
         J = r("DataFormDialog"),
         Q = P("loading");
     return m(), y("div", kt, [u("div", vt, [l(p, {
         type: "primary",
-        onClick: s.handleAddRow
+        onClick: a.handleAddRow
     }, {
         default: i(() => [l(d, null, {
             default: i(() => [l(c)]),
             _: 1
         }), b("\u6DFB\u52A0")]),
         _: 1
     }, 8, ["onClick"]), l(w, {
@@ -2010,61 +2021,61 @@
         style: {
             width: "260px"
         },
         modelValue: n.keyword,
         "onUpdate:modelValue": e[0] || (e[0] = I => n.keyword = I),
         placeholder: "\u641C\u7D22\u57DF\u540D\u3001\u6807\u7B7E",
         clearable: "",
-        onKeypress: H(s.handleSearch, ["enter"]),
-        onClear: s.handleSearch
+        onKeypress: H(a.handleSearch, ["enter"]),
+        onClear: a.handleSearch
     }, {
         append: i(() => [l(p, {
-            onClick: s.handleSearch
+            onClick: a.handleSearch
         }, {
             default: i(() => [l(d, null, {
                 default: i(() => [l(D)]),
                 _: 1
             })]),
             _: 1
         }, 8, ["onClick"])]),
         _: 1
     }, 8, ["modelValue", "onKeypress", "onClear"])]), t.role == n.RoleEnum.User ? (m(), y(U, {
         key: 0
     }, [n.hasInitData ? (m(), f(x, {
         key: 0,
         class: "mt-md",
         ref: "ConditionFilter",
-        onOnChange: s.handleConditionFilterChange
-    }, null, 8, ["onOnChange"])) : C("", !0)], 64)) : C("", !0), u("div", xt, [u("div", St, "\u5171\u8BA1 " + h(n.total) + " \u6761\u6570\u636E", 1), u("div", It, [s.showBatchDeleteButton ? (m(), f(T, {
+        onOnChange: a.handleConditionFilterChange
+    }, null, 8, ["onOnChange"])) : C("", !0)], 64)) : C("", !0), u("div", xt, [u("div", St, "\u5171\u8BA1 " + h(n.total) + " \u6761\u6570\u636E", 1), u("div", It, [a.showBatchDeleteButton ? (m(), f(T, {
         key: 0,
         title: "\u786E\u5B9A\u5220\u9664\u9009\u4E2D\uFF1F",
-        onConfirm: s.handleBatchDeleteConfirm
+        onConfirm: a.handleBatchDeleteConfirm
     }, {
         reference: i(() => [l(S, {
             underline: !1,
             type: "danger",
             class: "mr-sm"
         }, {
             default: i(() => [l(d, null, {
                 default: i(() => [l(k)]),
                 _: 1
             }), b("\u6279\u91CF\u5220\u9664")]),
             _: 1
         })]),
         _: 1
     }, 8, ["onConfirm"])) : C("", !0), l(O, {
-        onOnSuccess: s.resetData
+        onOnSuccess: a.resetData
     }, null, 8, ["onOnSuccess"]), t.role == n.RoleEnum.User ? (m(), y(U, {
         key: 1
     }, [l(F, {
         class: "ml-sm",
-        onOnSuccess: s.resetData
+        onOnSuccess: a.resetData
     }, null, 8, ["onOnSuccess"]), l(B, {
         class: "ml-sm",
-        onOnSuccess: s.resetData
+        onOnSuccess: a.resetData
     }, null, 8, ["onOnSuccess"]), l(S, {
         underline: !1,
         type: "primary",
         class: "ml-sm",
         style: {
             position: "relative"
         }
@@ -2073,63 +2084,63 @@
             default: i(() => [l(R)]),
             _: 1
         }), b("\u5BFC\u5165 "), l(E, {
             ref: "upload",
             action: "action",
             accept: ".txt",
             limit: 1,
-            "on-exceed": s.handleExceed,
+            "on-exceed": a.handleExceed,
             "show-file-list": !1,
-            "http-request": s.handleHttpRequest
+            "http-request": a.handleHttpRequest
         }, {
             default: i(() => [Vt]),
             _: 1
         }, 8, ["on-exceed", "http-request"])]),
         _: 1
     }), l(S, {
         underline: !1,
         type: "primary",
         class: "ml-sm mr-sm",
-        onClick: s.handleExportToFile
+        onClick: a.handleExportToFile
     }, {
         default: i(() => [l(d, null, {
-            default: i(() => [l(a)]),
+            default: i(() => [l(s)]),
             _: 1
         }), b("\u5BFC\u51FA")]),
         _: 1
     }, 8, ["onClick"]), l(g, {
-        onOnSuccess: s.handleTableColumnSuccess
+        onOnSuccess: a.handleTableColumnSuccess
     }, null, 8, ["onOnSuccess"])], 64)) : C("", !0)])]), A(l(z, {
         class: "mt-sm",
         tableColumns: n.tableColumns,
         data: n.list,
         role: t.role,
-        onOnSuccess: s.resetData,
-        onSortChange: s.handleSortChange,
-        onSelectionChange: s.handleSelectionChange,
-        onOnRefreshRow: s.handleRefreshRow,
-        onOnTagClick: s.handleTagClick
+        onOnSuccess: a.resetData,
+        onSortChange: a.handleSortChange,
+        onSelectionChange: a.handleSelectionChange,
+        onOnRefreshRow: a.handleRefreshRow,
+        onOnTagClick: a.handleTagClick
     }, null, 8, ["tableColumns", "data", "role", "onOnSuccess", "onSortChange", "onSelectionChange", "onOnRefreshRow", "onOnTagClick"]), [
         [Q, n.loading]
     ]), l(W, {
         class: "mt-md justify-center",
         background: "",
         layout: "total, sizes, prev, pager, next",
         total: n.total,
         "page-size": n.size,
         "onUpdate:pageSize": e[1] || (e[1] = I => n.size = I),
         "current-page": n.page,
         "onUpdate:currentPage": e[2] || (e[2] = I => n.page = I),
-        onCurrentChange: s.getData,
-        onSizeChange: s.handleSizeChange
+        onCurrentChange: a.getData,
+        onSizeChange: a.handleSizeChange
     }, null, 8, ["total", "page-size", "current-page", "onCurrentChange", "onSizeChange"]), l(J, {
         role: t.role,
         visible: n.dialogVisible,
         "onUpdate:visible": e[3] || (e[3] = I => n.dialogVisible = I),
-        onOnSuccess: s.handleAddSuccess
+        onOnSuccess: a.handleAddSuccess
     }, null, 8, ["role", "visible", "onOnSuccess"])])
 }
 const $t = v(Dt, [
     ["render", Ut]
 ]);
 export {
     $t as
```

### Comparing `domain-admin-1.5.8/domain_admin/public/js/index.af06b2dc.js` & `domain-admin-1.5.9/domain_admin/public/js/index.c1800b79.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,21 +1,21 @@
 import {
     i as Y,
     E as M
 } from "./event-enums.6c6f25e7.js";
 import {
     S as N,
     u as z
-} from "./SelectGroup.53d83114.js";
+} from "./SelectGroup.e46bb885.js";
 import {
     _ as v,
     R as $,
     d as L,
     r as W
-} from "./index.165f9ce1.js";
+} from "./index.5c3a2f20.js";
 import {
     ah as s,
     ar as P,
     Q as G,
     o as u,
     c as g,
     V as o,
@@ -33,18 +33,18 @@
 } from "./vendor-vue.9e61e0af.js";
 import {
     E as q,
     A as J,
     a as Z,
     b as ee,
     C as te
-} from "./ConditionFilterGroup.3c6ac067.js";
+} from "./ConditionFilterGroup.8b8592a5.js";
 import {
     C as oe
-} from "./ConnectStatus.a429b01b.js";
+} from "./ConnectStatus.8f8cc994.js";
 import {
     F as le
 } from "./vendor-lib.76301fc3.js";
 import {
     b as ie
 } from "./element-plus.30eb1cab.js";
 import "./element-icon.1ce1c350.js";
```

### Comparing `domain-admin-1.5.8/domain_admin/public/js/index.c22f6489.js` & `domain-admin-1.5.9/domain_admin/public/js/index.61002253.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 import {
     _ as C,
     R as O
-} from "./index.165f9ce1.js";
+} from "./index.5c3a2f20.js";
 import {
     ah as a,
     o as p,
     c as y,
     V as s,
     P as i,
     a as _,
@@ -21,18 +21,18 @@
     Q as T,
     F as A,
     ay as N
 } from "./vendor-vue.9e61e0af.js";
 import {
     S as j,
     u as B
-} from "./SelectGroup.53d83114.js";
+} from "./SelectGroup.e46bb885.js";
 import {
     S as F
-} from "./SearchUser.f8e52158.js";
+} from "./SearchUser.8714bea9.js";
 import "./element-icon.1ce1c350.js";
 import "./vendor-lib.76301fc3.js";
 import "./element-plus.30eb1cab.js";
 const P = {
         name: [{
             message: "\u540D\u79F0\u4E0D\u80FD\u4E3A\u7A7A",
             required: !0,
```

### Comparing `domain-admin-1.5.8/domain_admin/public/js/index.deff2c63.js` & `domain-admin-1.5.9/domain_admin/public/js/index.e0890673.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 import {
     _ as C
-} from "./index.165f9ce1.js";
+} from "./index.5c3a2f20.js";
 import {
     ah as i,
     o as b,
     c as k,
     V as t,
     P as l,
     a as h,
```

### Comparing `domain-admin-1.5.8/domain_admin/public/js/index.ef82c865.js` & `domain-admin-1.5.9/domain_admin/public/js/index.bc114a13.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -13,15 +13,15 @@
     F as k,
     a8 as N,
     az as w,
     aA as j
 } from "./vendor-vue.9e61e0af.js";
 import {
     _ as V
-} from "./index.165f9ce1.js";
+} from "./index.5c3a2f20.js";
 import "./element-icon.1ce1c350.js";
 import "./vendor-lib.76301fc3.js";
 import "./element-plus.30eb1cab.js";
 const A = {
         name: "index",
         props: {},
         components: {},
```

### Comparing `domain-admin-1.5.8/domain_admin/public/js/vendor-lib.76301fc3.js` & `domain-admin-1.5.9/domain_admin/public/js/vendor-lib.76301fc3.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/js/vendor-vue.9e61e0af.js` & `domain-admin-1.5.9/domain_admin/public/js/vendor-vue.9e61e0af.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/m/.git/hooks/commit-msg.sample` & `domain-admin-1.5.9/domain_admin/public/m/.git/hooks/commit-msg.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/m/.git/hooks/fsmonitor-watchman.sample` & `domain-admin-1.5.9/domain_admin/public/m/.git/hooks/fsmonitor-watchman.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/m/.git/hooks/pre-commit.sample` & `domain-admin-1.5.9/domain_admin/public/m/.git/hooks/pre-commit.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/m/.git/hooks/pre-push.sample` & `domain-admin-1.5.9/domain_admin/public/m/.git/hooks/pre-push.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/m/.git/hooks/pre-rebase.sample` & `domain-admin-1.5.9/domain_admin/public/m/.git/hooks/pre-rebase.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/m/.git/hooks/pre-receive.sample` & `domain-admin-1.5.9/domain_admin/public/m/.git/hooks/pre-receive.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/m/.git/hooks/prepare-commit-msg.sample` & `domain-admin-1.5.9/domain_admin/public/m/.git/hooks/prepare-commit-msg.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/m/.git/hooks/push-to-checkout.sample` & `domain-admin-1.5.9/domain_admin/public/m/.git/hooks/push-to-checkout.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/m/.git/hooks/sendemail-validate.sample` & `domain-admin-1.5.9/domain_admin/public/m/.git/hooks/sendemail-validate.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/m/.git/hooks/update.sample` & `domain-admin-1.5.9/domain_admin/public/m/.git/hooks/update.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/m/.git/objects/2d/7cec3e00ed3b3b835eb233ae4bb2ea21fb5a0b` & `domain-admin-1.5.9/domain_admin/public/m/.git/objects/2d/7cec3e00ed3b3b835eb233ae4bb2ea21fb5a0b`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/m/.git/objects/43/c4fcdf29fe10c6256aa4e9cf00f534e6933efc` & `domain-admin-1.5.9/domain_admin/public/m/.git/objects/43/c4fcdf29fe10c6256aa4e9cf00f534e6933efc`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/m/.git/objects/4b/63cfa29bd94b198d895f7a64e10c20f167e65b` & `domain-admin-1.5.9/domain_admin/public/m/.git/objects/4b/63cfa29bd94b198d895f7a64e10c20f167e65b`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/m/.git/objects/6f/9d23d38fd97c94c1dccf971fd7b7636cc075d2` & `domain-admin-1.5.9/domain_admin/public/m/.git/objects/6f/9d23d38fd97c94c1dccf971fd7b7636cc075d2`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/m/.git/objects/71/4dbccc412b153f5044c269745126581e3cf373` & `domain-admin-1.5.9/domain_admin/public/m/.git/objects/71/4dbccc412b153f5044c269745126581e3cf373`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/m/.git/objects/7a/694f3c8aca1586dc6f0e6e9e2773e207992329` & `domain-admin-1.5.9/domain_admin/public/m/.git/objects/7a/694f3c8aca1586dc6f0e6e9e2773e207992329`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/m/.git/objects/7a/c4cdd0b7c56c8fe9f98aaf044df58bef26b7a5` & `domain-admin-1.5.9/domain_admin/public/m/.git/objects/7a/c4cdd0b7c56c8fe9f98aaf044df58bef26b7a5`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/m/.git/objects/8e/ff5bef00cd2492d9b806988ea99996d636c126` & `domain-admin-1.5.9/domain_admin/public/m/.git/objects/8e/ff5bef00cd2492d9b806988ea99996d636c126`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/m/.git/objects/93/85587145f9afbabe2aa1a489d24fd1f489e5c6` & `domain-admin-1.5.9/domain_admin/public/m/.git/objects/93/85587145f9afbabe2aa1a489d24fd1f489e5c6`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/m/.git/objects/93/db3989e7874cd6b75bc0e984690ffa16666ea6` & `domain-admin-1.5.9/domain_admin/public/m/.git/objects/93/db3989e7874cd6b75bc0e984690ffa16666ea6`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/m/.git/objects/98/1e059e0de4604a5dec80930d8ff7cdf84e0006` & `domain-admin-1.5.9/domain_admin/public/m/.git/objects/98/1e059e0de4604a5dec80930d8ff7cdf84e0006`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/m/.git/objects/a9/a1035a25ce05f60741e3f70716a18d93322203` & `domain-admin-1.5.9/domain_admin/public/m/.git/objects/a9/a1035a25ce05f60741e3f70716a18d93322203`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/m/.git/objects/b0/ecf609c3df960010b6f7877bc379ea45d1e9da` & `domain-admin-1.5.9/domain_admin/public/m/.git/objects/b0/ecf609c3df960010b6f7877bc379ea45d1e9da`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/m/.git/objects/c7/ef9b19427f9af9e445bb5d63231ccd58ef5b28` & `domain-admin-1.5.9/domain_admin/public/m/.git/objects/c7/ef9b19427f9af9e445bb5d63231ccd58ef5b28`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/m/.git/objects/c8/bec3f3e9b26642a8221c20a5e422bc2cada687` & `domain-admin-1.5.9/domain_admin/public/m/.git/objects/c8/bec3f3e9b26642a8221c20a5e422bc2cada687`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/m/.git/objects/ed/50570bc6865f7dff2468d49072d7f4e4cb81d4` & `domain-admin-1.5.9/domain_admin/public/m/.git/objects/ed/50570bc6865f7dff2468d49072d7f4e4cb81d4`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/m/.git/objects/f0/a3f5a57d6bdb9961c3a56f4a992a08a0ecd671` & `domain-admin-1.5.9/domain_admin/public/m/.git/objects/f0/a3f5a57d6bdb9961c3a56f4a992a08a0ecd671`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/m/.git/objects/f8/0169320ed23edd9889e4de7631267635bfec27` & `domain-admin-1.5.9/domain_admin/public/m/.git/objects/f8/0169320ed23edd9889e4de7631267635bfec27`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/m/.git/objects/fd/bd32c675f85af4ed57021ac0638a21a3c6cad3` & `domain-admin-1.5.9/domain_admin/public/m/.git/objects/fd/bd32c675f85af4ed57021ac0638a21a3c6cad3`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/m/assets/common-c7dd5d89.css` & `domain-admin-1.5.9/domain_admin/public/m/assets/common-c7dd5d89.css`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/m/assets/common.6194c42f.js` & `domain-admin-1.5.9/domain_admin/public/m/assets/common.6194c42f.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/m/assets/index-5eda257b.css` & `domain-admin-1.5.9/domain_admin/public/m/assets/index-5eda257b.css`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/m/assets/index-958ae3a0.css` & `domain-admin-1.5.9/domain_admin/public/m/assets/index-958ae3a0.css`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/m/assets/index-9c365a03.js` & `domain-admin-1.5.9/domain_admin/public/m/assets/index-9c365a03.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/m/assets/index-ad047368.css` & `domain-admin-1.5.9/domain_admin/public/m/assets/index-ad047368.css`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/m/assets/index-e8224928.css` & `domain-admin-1.5.9/domain_admin/public/m/assets/index-e8224928.css`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/m/assets/index-f79acb3d.css` & `domain-admin-1.5.9/domain_admin/public/m/assets/index-f79acb3d.css`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/m/assets/index.1a0d1182.js` & `domain-admin-1.5.9/domain_admin/public/m/assets/index.1a0d1182.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/m/assets/index.1d067866.js` & `domain-admin-1.5.9/domain_admin/public/m/assets/index.1d067866.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/m/assets/index.daaf9893.js` & `domain-admin-1.5.9/domain_admin/public/m/assets/index.daaf9893.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/m/assets/index.feef7c0f.js` & `domain-admin-1.5.9/domain_admin/public/m/assets/index.feef7c0f.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/m/assets/login-cb9f43ad.css` & `domain-admin-1.5.9/domain_admin/public/m/assets/login-cb9f43ad.css`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/m/assets/pages-cert-list-cert-list.e9ecbf65.js` & `domain-admin-1.5.9/domain_admin/public/m/assets/pages-cert-list-cert-list.e9ecbf65.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/m/assets/pages-domain-list-domain-list.da5e6454.js` & `domain-admin-1.5.9/domain_admin/public/m/assets/pages-domain-list-domain-list.da5e6454.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/m/assets/pages-login-login.09426b90.js` & `domain-admin-1.5.9/domain_admin/public/m/assets/pages-login-login.09426b90.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/m/assets/pages-user-index-user-index.d8efba8c.js` & `domain-admin-1.5.9/domain_admin/public/m/assets/pages-user-index-user-index.d8efba8c.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/m/assets/uni.06dd3c8e.css` & `domain-admin-1.5.9/domain_admin/public/m/assets/uni.06dd3c8e.css`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/m/assets/user-index-be7005ab.css` & `domain-admin-1.5.9/domain_admin/public/m/assets/user-index-be7005ab.css`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/m/index.html` & `domain-admin-1.5.9/domain_admin/public/m/index.html`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/m/static/user-avatar.gif` & `domain-admin-1.5.9/domain_admin/public/m/static/user-avatar.gif`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/public/svg/logo.184a2d7d.svg` & `domain-admin-1.5.9/domain_admin/public/svg/logo.184a2d7d.svg`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/router/api_map.py` & `domain-admin-1.5.9/domain_admin/router/api_map.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 """
 from __future__ import print_function, unicode_literals, absolute_import, division
 from domain_admin.api import (
     cert_api, ip_api, notify_api,
     whois_api, address_api,
     domain_info_api, prometheus_api,
     log_operation_api, group_user_api,
-    log_async_task_api, issue_certificate_api)
+    log_async_task_api, issue_certificate_api, host_api)
 from domain_admin.api import domain_api
 from domain_admin.api import group_api
 from domain_admin.api import auth_api
 from domain_admin.api import system_api
 from domain_admin.api import user_api
 from domain_admin.api import log_scheduler_api
 
@@ -155,8 +155,22 @@
 
     # SSL证书
     '/api/getCertificateList': issue_certificate_api.get_certificate_list,
     '/api/issueCertificate': issue_certificate_api.issue_certificate,
     '/api/renewCertificate': issue_certificate_api.renew_certificate,
     '/api/getIssueCertificateById': issue_certificate_api.get_issue_certificate_by_id,
     '/api/verifyCertificateById': issue_certificate_api.verify_certificate,
+
+
+    '/api/getDomainHost': issue_certificate_api.get_domain_host,
+    '/api/deployVerifyFile': issue_certificate_api.deploy_verify_file,
+    '/api/deployCertificateFile': issue_certificate_api.deploy_certificate_file,
+    '/api/getCertificateChallenges': issue_certificate_api.get_certificate_challenges,
+    '/api/deleteCertificateById': issue_certificate_api.delete_certificate_by_id,
+    '/api/deleteCertificateByBatch': issue_certificate_api.delete_certificate_by_batch,
+
+    # 主机管理
+    '/api/addHost': host_api.add_host,
+    '/api/getHostById': host_api.get_host_by_id,
+    '/api/updateHostById': host_api.update_host_by_id,
+    '/api/getHostList': host_api.get_host_list,
 }
```

### Comparing `domain-admin-1.5.8/domain_admin/router/permission.py` & `domain-admin-1.5.9/domain_admin/router/permission.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/service/async_task_service.py` & `domain-admin-1.5.9/domain_admin/service/async_task_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/service/auth_service.py` & `domain-admin-1.5.9/domain_admin/service/auth_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/service/common_service.py` & `domain-admin-1.5.9/domain_admin/service/common_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/service/domain_info_service.py` & `domain-admin-1.5.9/domain_admin/service/domain_info_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/service/domain_service.py` & `domain-admin-1.5.9/domain_admin/service/domain_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/service/file_service.py` & `domain-admin-1.5.9/domain_admin/service/file_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/service/group_service.py` & `domain-admin-1.5.9/domain_admin/service/group_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/service/group_user_service.py` & `domain-admin-1.5.9/domain_admin/service/group_user_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/service/notify_service.py` & `domain-admin-1.5.9/domain_admin/service/notify_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/service/operation_service.py` & `domain-admin-1.5.9/domain_admin/service/operation_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/service/scheduler_service.py` & `domain-admin-1.5.9/domain_admin/service/scheduler_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 import warnings
 from logging.handlers import RotatingFileHandler
 
 from apscheduler.schedulers.background import BackgroundScheduler
 
 from domain_admin.enums.config_key_enum import ConfigKeyEnum
 from domain_admin.model.log_scheduler_model import LogSchedulerModel
-from domain_admin.service import system_service, domain_service, domain_info_service, notify_service
+from domain_admin.service import system_service, domain_service, domain_info_service, notify_service, \
+    issue_certificate_service
 from domain_admin.service.file_service import resolve_log_file
 from domain_admin.utils import datetime_util
 
 warnings.filterwarnings(action="ignore")
 
 apscheduler_logger = logging.getLogger('apscheduler')
 
@@ -84,14 +85,17 @@
 
     # 更新证书信息
     domain_service.update_all_domain_cert_info()
 
     # 更新域名信息
     domain_info_service.update_all_domain_info()
 
+    # 更新所有SSL证书
+    issue_certificate_service.renew_all_certificate()
+
     # 触发通知
     success = notify_service.notify_all_event()
 
     # 执行完毕
     LogSchedulerModel.update({
         'status': True,
         'error_message': '执行成功',
```

### Comparing `domain-admin-1.5.8/domain_admin/service/system_service.py` & `domain-admin-1.5.9/domain_admin/service/system_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/service/token_service.py` & `domain-admin-1.5.9/domain_admin/service/token_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/service/version_service.py` & `domain-admin-1.5.9/domain_admin/service/version_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     migrate_136_to_140_alpha,
     migrate_140_alpha_to_140,
     migrate_143_to_144,
     migrate_145_to_146,
     migrate_1413_to_1414,
     migrate_1422_to_1423,
     migrate_151_to_152,
-    migrate_154_to_155)
+    migrate_154_to_155, migrate_158_to_159)
 from domain_admin.model.version_model import VersionModel
 from domain_admin.version import VERSION
 
 
 def get_local_version():
     """
     获取本地最新版本号
@@ -264,14 +264,28 @@
             # 1.5.4 => 1.5.5
             logger.info('update version: %s => %s', local_version, VersionEnum.Version_155)
 
             migrate_154_to_155.execute_migrate()
 
             local_version = VersionEnum.Version_155
 
+        # 2023-07-22
+        if local_version in [
+            VersionEnum.Version_155,
+            VersionEnum.Version_156,
+            VersionEnum.Version_157,
+            VersionEnum.Version_158,
+        ]:
+            # 1.5.8 => 1.5.9
+            logger.info('update version: %s => %s', local_version, VersionEnum.Version_159)
+
+            migrate_158_to_159.execute_migrate()
+
+            local_version = VersionEnum.Version_159
+
     # 更新版本号
     # fix: 多实例同时启动版本号写入失败问题
     try:
         VersionModel.create(
             version=current_version
         )
     except IntegrityError:
```

### Comparing `domain-admin-1.5.8/domain_admin/templates/cert-email.html` & `domain-admin-1.5.9/domain_admin/templates/cert-email.html`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/templates/domain-email.html` & `domain-admin-1.5.9/domain_admin/templates/domain-email.html`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/utils/bcrypt_util.py` & `domain-admin-1.5.9/domain_admin/utils/bcrypt_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/utils/cert_util/cert_common.py` & `domain-admin-1.5.9/domain_admin/utils/cert_util/cert_common.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 """
 @File    : cert_common.py
 @Date    : 2022-11-08
 @Author  : Peng Shiyu
 """
 from __future__ import print_function, unicode_literals, absolute_import, division
 import socket
+from datetime import datetime
 
 import OpenSSL
 from dateutil import parser
 
 from domain_admin.utils import time_util
 from domain_admin.utils.cert_util import cert_consts
 
@@ -74,23 +75,14 @@
     dct = {}
     for key, value in name_map.items():
         dct[key] = data.get(value, '')
 
     return dct
 
 
-def get_domain_ip(domain):
-    """
-    获取ip地址
-    :param domain: str
-    :return: str
-    """
-    return socket.gethostbyname(domain)
-
-
 class X509Item(object):
     version = ''
     subject = dict()
     issuer = dict()
     notAfter = ''
     notBefore = ''
     serialNumber = ''
@@ -105,21 +97,26 @@
             'issuer': self.issuer,
             'notAfter': self.notAfter,
             'notBefore': self.notBefore,
             'serialNumber': self.serialNumber,
             'signatureAlgorithm': self.signatureAlgorithm,
             'subjectAltName': self.subjectAltName,
             'hasExpired': self.hasExpired,
+            'totalDays': self.totalDays,
             'expireDays': self.expireDays,
         }
 
     @property
-    def expireDays(self):
+    def totalDays(self):
         return time_util.get_diff_days(self.notBefore, self.notAfter)
 
+    @property
+    def expireDays(self):
+        return time_util.get_diff_days(datetime.now(), self.notAfter)
+
 
 def dump_certificate_to_text(ssl_cert):
     """
     将证书对象转为字符串text形式
     :param ssl_cert:
     :return: str
     """
```

### Comparing `domain-admin-1.5.8/domain_admin/utils/cert_util/cert_openssl_v2.py` & `domain-admin-1.5.9/domain_admin/utils/cert_util/cert_openssl_v2.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/utils/cert_util/cert_socket.py` & `domain-admin-1.5.9/domain_admin/utils/cert_util/cert_socket.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/utils/cert_util/cert_socket_v2.py` & `domain-admin-1.5.9/domain_admin/utils/cert_util/cert_socket_v2.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/utils/datetime_util.py` & `domain-admin-1.5.9/domain_admin/utils/datetime_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/utils/domain_util.py` & `domain-admin-1.5.9/domain_admin/utils/domain_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/utils/email_util.py` & `domain-admin-1.5.9/domain_admin/utils/email_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/utils/flask_ext/api_result.py` & `domain-admin-1.5.9/domain_admin/utils/flask_ext/api_result.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/utils/flask_ext/app_exception.py` & `domain-admin-1.5.9/domain_admin/utils/flask_ext/app_exception.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/utils/flask_ext/flask_app.py` & `domain-admin-1.5.9/domain_admin/utils/flask_ext/flask_app.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/utils/flask_ext/handler.py` & `domain-admin-1.5.9/domain_admin/utils/flask_ext/handler.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/utils/flask_ext/json/default.py` & `domain-admin-1.5.9/domain_admin/utils/flask_ext/json/default.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/utils/flask_ext/json/json_encoder.py` & `domain-admin-1.5.9/domain_admin/utils/flask_ext/json/json_encoder.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/utils/flask_ext/json/json_provider.py` & `domain-admin-1.5.9/domain_admin/utils/flask_ext/json/json_provider.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/utils/icp_util.py` & `domain-admin-1.5.9/domain_admin/utils/icp_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/utils/json_util.py` & `domain-admin-1.5.9/domain_admin/utils/json_util.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 @File    : json_util.py
 @Date    : 2023-04-16
 """
 from __future__ import print_function, unicode_literals, absolute_import, division
 import json
 from datetime import datetime
 
+from acme.messages import ChallengeBody
 from peewee import ModelSelect, Model
 from playhouse.shortcuts import model_to_dict
 
 DATETIME_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
 def default_json_encoder(o):
@@ -25,14 +26,17 @@
 
     if isinstance(o, Model):
         return model_to_dict(o)
 
     if isinstance(o, datetime):
         return o.strftime(DATETIME_FORMAT)
 
+    if isinstance(o, ChallengeBody):
+        return o.to_json()
+
     return o
 
 
 def json_encode(data, default=default_json_encoder, **kwargs):
     """
     json序列化
     :param data:
@@ -40,8 +44,8 @@
     :param kwargs:
     :return:
     """
     return json.dumps(data, default=default, **kwargs)
 
 
 def json_dump(obj):
-    print(json_encode(obj, ensure_ascii=False, indent=2))
+    return json_encode(obj, ensure_ascii=False, indent=2)
```

### Comparing `domain-admin-1.5.8/domain_admin/utils/open_api/crtsh_api.py` & `domain-admin-1.5.9/domain_admin/utils/open_api/crtsh_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/utils/open_api/ding_talk_api.py` & `domain-admin-1.5.9/domain_admin/utils/open_api/ding_talk_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/utils/open_api/feishu_api.py` & `domain-admin-1.5.9/domain_admin/utils/open_api/feishu_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/utils/open_api/work_weixin_api.py` & `domain-admin-1.5.9/domain_admin/utils/open_api/work_weixin_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/utils/peewee_ext/model_util.py` & `domain-admin-1.5.9/domain_admin/utils/peewee_ext/model_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/utils/secret_util.py` & `domain-admin-1.5.9/domain_admin/utils/secret_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/utils/text_util.py` & `domain-admin-1.5.9/domain_admin/utils/text_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/utils/time_util.py` & `domain-admin-1.5.9/domain_admin/utils/time_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/utils/whois_util/config.py` & `domain-admin-1.5.9/domain_admin/utils/whois_util/config.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/utils/whois_util/util.py` & `domain-admin-1.5.9/domain_admin/utils/whois_util/util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/utils/whois_util/whois-servers.txt` & `domain-admin-1.5.9/domain_admin/utils/whois_util/whois-servers.txt`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin/utils/whois_util/whois_util.py` & `domain-admin-1.5.9/domain_admin/utils/whois_util/whois_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.8/domain_admin.egg-info/SOURCES.txt` & `domain-admin-1.5.9/domain_admin.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 domain_admin/api/address_api.py
 domain_admin/api/auth_api.py
 domain_admin/api/cert_api.py
 domain_admin/api/domain_api.py
 domain_admin/api/domain_info_api.py
 domain_admin/api/group_api.py
 domain_admin/api/group_user_api.py
+domain_admin/api/host_api.py
 domain_admin/api/ip_api.py
 domain_admin/api/issue_certificate_api.py
 domain_admin/api/log_async_task_api.py
 domain_admin/api/log_operation_api.py
 domain_admin/api/log_scheduler_api.py
 domain_admin/api/notify_api.py
 domain_admin/api/prometheus_api.py
@@ -53,23 +54,25 @@
 domain_admin/migrate/migrate_140_alpha_to_140.py
 domain_admin/migrate/migrate_1413_to_1414.py
 domain_admin/migrate/migrate_1422_to_1423.py
 domain_admin/migrate/migrate_143_to_144.py
 domain_admin/migrate/migrate_145_to_146.py
 domain_admin/migrate/migrate_151_to_152.py
 domain_admin/migrate/migrate_154_to_155.py
+domain_admin/migrate/migrate_158_to_159.py
 domain_admin/migrate/migrate_common.py
 domain_admin/model/__init__.py
 domain_admin/model/address_model.py
 domain_admin/model/base_model.py
 domain_admin/model/database.py
 domain_admin/model/domain_info_model.py
 domain_admin/model/domain_model.py
 domain_admin/model/group_model.py
 domain_admin/model/group_user_model.py
+domain_admin/model/host_model.py
 domain_admin/model/issue_certificate_model.py
 domain_admin/model/log_async_task_model.py
 domain_admin/model/log_operation_model.py
 domain_admin/model/log_scheduler_model.py
 domain_admin/model/notify_model.py
 domain_admin/model/system_model.py
 domain_admin/model/user_model.py
@@ -96,100 +99,100 @@
 domain_admin/public/.git/hooks/push-to-checkout.sample
 domain_admin/public/.git/hooks/sendemail-validate.sample
 domain_admin/public/.git/hooks/update.sample
 domain_admin/public/.git/info/exclude
 domain_admin/public/.git/logs/HEAD
 domain_admin/public/.git/logs/refs/heads/dist
 domain_admin/public/.git/logs/refs/remotes/origin/dist
+domain_admin/public/.git/objects/00/f7c6e2fba3e12bc14ab61c148b4ba2a64e38a3
 domain_admin/public/.git/objects/19/7f5cf73cf11d43d915904e0d8aad4736a77d63
 domain_admin/public/.git/objects/21/00bd7d2219a26827cc80aa37fe72fcb303bb50
-domain_admin/public/.git/objects/2b/3195083ee5802a2c60fdb9919fbf35e18e6478
-domain_admin/public/.git/objects/32/dd3b54be707f423bd7375381bbc2baede37f8c
-domain_admin/public/.git/objects/37/11576f2b615224b9477da0a0a9a43c17539d12
+domain_admin/public/.git/objects/21/39b81dcd444515633d19490097a6b348cde5c5
+domain_admin/public/.git/objects/25/295734aef0855e20af49f3eeabf0b66868f6ba
+domain_admin/public/.git/objects/28/f9bf1d51da58ca27d653eb24726bf24710ad77
+domain_admin/public/.git/objects/29/a4c85c52713f69636b86696e2d2c46f10a6da0
+domain_admin/public/.git/objects/2d/8a41ec985b9d8eae83de5d090acfcfc3c41242
+domain_admin/public/.git/objects/2e/ae458563637ec44c6387b9169f3abfdb3e6c29
 domain_admin/public/.git/objects/3c/0f2e923566dc74d04e67d46d8b722923ed1949
 domain_admin/public/.git/objects/3c/2434ab20d756f0a95ad24f6a5adb7e1219a7d1
-domain_admin/public/.git/objects/3e/24054f5e3a680f56b9276efe009e73b7133a99
-domain_admin/public/.git/objects/4b/f6af202944cd3e22f8a375977737ce52b17763
+domain_admin/public/.git/objects/43/cf76d02df6959240541fad0a582a256c9d1d9f
 domain_admin/public/.git/objects/52/c1926de72b181c9b7faf597fb8f71f48565462
 domain_admin/public/.git/objects/55/1103b11c4b699a3b4107d3a2ab173dfe238556
-domain_admin/public/.git/objects/57/bd1a9bfce972b50e5efecf11f71a3f5b2ec3d3
+domain_admin/public/.git/objects/59/7a1712f21c02c83dc657e1eb2287fcbba0b692
 domain_admin/public/.git/objects/5f/a7faf700c98850aa96022ab07af6a07b854f34
-domain_admin/public/.git/objects/60/727d43f26f701780e7c55e90cb084973a1be9e
 domain_admin/public/.git/objects/69/a9dda41cf39bb60d1dc5b1158ffba197580b6a
+domain_admin/public/.git/objects/6a/6a1ab9b562bb27239abdcdf8e1a772761b4dee
 domain_admin/public/.git/objects/6c/3e3059f9ec00c015681abca34b751c3439513d
-domain_admin/public/.git/objects/6c/f21ee6e3a69b2e234f6012f1636e3621d25db8
+domain_admin/public/.git/objects/6c/eb074240765b4f5dba74a28f57ff96fa54f33c
 domain_admin/public/.git/objects/6d/15191314c9b832ac41056a30bf0bf6533a29dc
-domain_admin/public/.git/objects/71/6b5718c659ed5a85d4f93a2cf25fc5ff5031cb
+domain_admin/public/.git/objects/6f/0100c1cf8791c558a0116b7ca1e59de431ee28
+domain_admin/public/.git/objects/72/d994916434598d7948b1adb0815369eccbd518
+domain_admin/public/.git/objects/75/d9dfaadcdfe57a016666775b36754ff77ec7d4
 domain_admin/public/.git/objects/79/404c2464172f80b414d111f49718327b3ef93b
-domain_admin/public/.git/objects/7c/7a565bed760068496030f030f2b05ede1bec4b
 domain_admin/public/.git/objects/7f/64d8af0501887e805dc9ccf8228f4fb5e73fdb
-domain_admin/public/.git/objects/88/eed16a647060a310c6f8fd8cbf109ad11d1211
+domain_admin/public/.git/objects/85/33870af4bccab767938338b23bf5d1ef5b3f3b
 domain_admin/public/.git/objects/89/0f3ed83973272c63b56a722a88fe25160d11d2
+domain_admin/public/.git/objects/8c/c916b983bc8c1f7df16b9f5741cfad4d2a4fcc
 domain_admin/public/.git/objects/8c/f880f5a9481ef71cd22e08d59e7d366775b360
-domain_admin/public/.git/objects/8f/3fc862ebdfdd80953e51ae5e44e7862b79ad63
-domain_admin/public/.git/objects/92/cfface0a460c51331fb8f25083a09948e00cbf
+domain_admin/public/.git/objects/91/886bd903574b0bfe9b1ba9364bb716a6b8757b
 domain_admin/public/.git/objects/95/f07af46d709638b20c0b2c66cdf6de8e89a7e4
-domain_admin/public/.git/objects/9a/44f010e55bd5cd3a7d60bcd86ee9b8e7ef2cef
+domain_admin/public/.git/objects/9a/395cf124caea477b9f8061fbf89228b989a948
 domain_admin/public/.git/objects/9a/4e8fcc1912f0c1af9a1836ebd9847d8b0e3118
-domain_admin/public/.git/objects/a5/6b22c2eacca280122dde700a98068ebdd8c5af
-domain_admin/public/.git/objects/a7/49320e6e50d7593d7d1d30ee0159023cd4e422
-domain_admin/public/.git/objects/ae/1c9a7def175d7a6389679bf822a6a9219c3ca3
-domain_admin/public/.git/objects/b2/9b2820070fd0808f478afc2a5995aaee9cd79f
+domain_admin/public/.git/objects/9e/0266769577ed8db9863f40a1ce18c97e9c85ca
+domain_admin/public/.git/objects/9e/16d5586b2b1ccd986fa841aadcf150ccf4ccf3
+domain_admin/public/.git/objects/a1/13e44b9d9526cfc9b780807dbca0935bcbc9ad
+domain_admin/public/.git/objects/ad/38c27c881e48722da8bb9bc7f410189a334108
 domain_admin/public/.git/objects/b3/1cb2667f48424e34cf9517362eadf899f704ad
+domain_admin/public/.git/objects/c1/9a2a5676c89fe224b74ec4fb000399048d1a78
 domain_admin/public/.git/objects/c4/c46ae2c464a49661d7793709077759039f0b5e
-domain_admin/public/.git/objects/c9/3d3f53fd06fdbc8587e3a8f37876356c5cdb56
 domain_admin/public/.git/objects/cc/bfeaa0b21986ed309cbb83d17585b54f3b2fb9
-domain_admin/public/.git/objects/d2/5bbe60e329a2e662af042df10825c9dcdc3887
-domain_admin/public/.git/objects/e0/6f4cc670d4bb8f606c4edfb9d7aa51becaaf2a
 domain_admin/public/.git/objects/e1/13bfd922675ce50e68cdf88cd94d16130ad58b
-domain_admin/public/.git/objects/e6/8884f9d8cc37153041b8b82943d995c95ba1aa
-domain_admin/public/.git/objects/e6/e9c9b85a9477efa2c8f05874bd09fa93a6b34c
-domain_admin/public/.git/objects/e9/8d4dd298d6c05d0bfa2fbe9182ec7cddde7926
-domain_admin/public/.git/objects/f9/78f4b33c1fdc0cb74f1df45d0fc049f5da1c89
-domain_admin/public/.git/objects/fb/ac0b57e4138b4fca9c9f5babf558611a38e6d0
+domain_admin/public/.git/objects/e6/327e057f2a2d4a5a57f21379f407da0db060e2
+domain_admin/public/.git/objects/f1/9692949226c296834afeb8669582e799d94a3f
+domain_admin/public/.git/objects/f3/fe7436cf05ee53d3fe361b83e4e9d498a8c106
 domain_admin/public/.git/objects/fd/bd32c675f85af4ed57021ac0638a21a3c6cad3
 domain_admin/public/.git/objects/ff/9c65dfdc7a16150c07745e0030a9d6373920cd
 domain_admin/public/.git/refs/heads/dist
 domain_admin/public/.git/refs/remotes/origin/dist
 domain_admin/public/css/ConditionFilterGroup.a91875e6.css
-domain_admin/public/css/index.302e10d7.css
+domain_admin/public/css/index.26827e91.css
 domain_admin/public/css/index.69a97337.css
-domain_admin/public/css/index.93c714bb.css
 domain_admin/public/css/index.a676cc2e.css
 domain_admin/public/css/index.b285e10a.css
 domain_admin/public/css/index.cf805e1c.css
 domain_admin/public/css/index.d028ae37.css
+domain_admin/public/css/index.e21504c8.css
 domain_admin/public/gif/user-avatar.ea67286d.gif
 domain_admin/public/jpg/chatpet-white.10f4f36c.jpg
 domain_admin/public/jpg/chatpet.fce5580e.jpg
-domain_admin/public/js/ConditionFilterGroup.3c6ac067.js
-domain_admin/public/js/ConnectStatus.a429b01b.js
-domain_admin/public/js/SearchUser.f8e52158.js
-domain_admin/public/js/SelectGroup.53d83114.js
+domain_admin/public/js/ConditionFilterGroup.8b8592a5.js
+domain_admin/public/js/ConnectStatus.8f8cc994.js
+domain_admin/public/js/SearchUser.8714bea9.js
+domain_admin/public/js/SelectGroup.e46bb885.js
 domain_admin/public/js/codemirror-lib.a3a39aa0.js
 domain_admin/public/js/element-icon.1ce1c350.js
 domain_admin/public/js/element-plus.30eb1cab.js
 domain_admin/public/js/event-enums.6c6f25e7.js
 domain_admin/public/js/highlight-lib.3654f6d3.js
 domain_admin/public/js/highlight-util.a4f1867f.js
-domain_admin/public/js/index.0963ab53.js
-domain_admin/public/js/index.0d4c27ce.js
-domain_admin/public/js/index.165f9ce1.js
-domain_admin/public/js/index.24e255af.js
-domain_admin/public/js/index.2ab02c40.js
-domain_admin/public/js/index.3b5a616c.js
-domain_admin/public/js/index.5b4cd516.js
-domain_admin/public/js/index.5f8ece3f.js
-domain_admin/public/js/index.654f7830.js
-domain_admin/public/js/index.8c31b31b.js
-domain_admin/public/js/index.a8bb8abf.js
-domain_admin/public/js/index.af06b2dc.js
-domain_admin/public/js/index.c22f6489.js
-domain_admin/public/js/index.deff2c63.js
-domain_admin/public/js/index.ef82c865.js
+domain_admin/public/js/index.006f8a9f.js
+domain_admin/public/js/index.0bc39ff5.js
+domain_admin/public/js/index.1cd93e88.js
+domain_admin/public/js/index.22cdc255.js
+domain_admin/public/js/index.34d377d3.js
+domain_admin/public/js/index.435ed104.js
+domain_admin/public/js/index.47fd0142.js
+domain_admin/public/js/index.5c3a2f20.js
+domain_admin/public/js/index.61002253.js
+domain_admin/public/js/index.8410f64d.js
+domain_admin/public/js/index.ab4c92d7.js
+domain_admin/public/js/index.b9d6d972.js
+domain_admin/public/js/index.bc114a13.js
+domain_admin/public/js/index.c1800b79.js
+domain_admin/public/js/index.e0890673.js
 domain_admin/public/js/vendor-lib.76301fc3.js
 domain_admin/public/js/vendor-vue.9e61e0af.js
 domain_admin/public/m/index.html
 domain_admin/public/m/.git/FETCH_HEAD
 domain_admin/public/m/.git/HEAD
 domain_admin/public/m/.git/config
 domain_admin/public/m/.git/description
@@ -286,24 +289,26 @@
 domain_admin/templates/domain-email.html
 domain_admin/templates/domain-export.csv
 domain_admin/utils/__init__.py
 domain_admin/utils/bcrypt_util.py
 domain_admin/utils/datetime_util.py
 domain_admin/utils/domain_util.py
 domain_admin/utils/email_util.py
+domain_admin/utils/fabric_util.py
 domain_admin/utils/file_util.py
 domain_admin/utils/icp_util.py
 domain_admin/utils/ip_util.py
 domain_admin/utils/json_util.py
 domain_admin/utils/md5_util.py
 domain_admin/utils/secret_util.py
 domain_admin/utils/text_util.py
 domain_admin/utils/time_util.py
 domain_admin/utils/acme_util/__init__.py
 domain_admin/utils/acme_util/acme_v2_api.py
+domain_admin/utils/acme_util/challenge_type.py
 domain_admin/utils/cert_util/__init__.py
 domain_admin/utils/cert_util/cert_common.py
 domain_admin/utils/cert_util/cert_consts.py
 domain_admin/utils/cert_util/cert_info.py
 domain_admin/utils/cert_util/cert_openssl_v2.py
 domain_admin/utils/cert_util/cert_socket.py
 domain_admin/utils/cert_util/cert_socket_v2.py
```

### Comparing `domain-admin-1.5.8/setup.py` & `domain-admin-1.5.9/setup.py`

 * *Files identical despite different names*

