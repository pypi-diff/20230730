# Comparing `tmp/cycode-0.2.6.dev9.tar.gz` & `tmp/cycode-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cycode-0.2.6.dev9.tar", max compression
+gzip compressed data, was "cycode-1.0.0.tar", max compression
```

## Comparing `cycode-0.2.6.dev9.tar` & `cycode-1.0.0.tar`

### file list

```diff
@@ -1,66 +1,65 @@
--rw-r--r--   0        0        0    32549 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/README.md
--rw-r--r--   0        0        0      760 2023-07-06 08:23:21.437194 cycode-0.2.6.dev9/cycode/__init__.py
--rw-r--r--   0        0        0        0 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/auth/__init__.py
--rw-r--r--   0        0        0     2777 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/auth/auth_command.py
--rw-r--r--   0        0        0     4742 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/auth/auth_manager.py
--rw-r--r--   0        0        0     1560 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/ci_integrations.py
--rw-r--r--   0        0        0    53335 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/code_scanner.py
--rw-r--r--   0        0        0      466 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/config.py
--rw-r--r--   0        0        0      387 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/config.yaml
--rw-r--r--   0        0        0     5705 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/consts.py
--rw-r--r--   0        0        0        0 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/exceptions/__init__.py
--rw-r--r--   0        0        0     1717 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/exceptions/custom_exceptions.py
--rw-r--r--   0        0        0        0 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/helpers/__init__.py
--rw-r--r--   0        0        0        0 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/helpers/maven/__init__.py
--rw-r--r--   0        0        0     2041 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/helpers/maven/base_restore_maven_dependencies.py
--rw-r--r--   0        0        0      975 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/helpers/maven/restore_gradle_dependencies.py
--rw-r--r--   0        0        0     2888 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/helpers/maven/restore_maven_dependencies.py
--rw-r--r--   0        0        0     5626 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/helpers/sca_code_scanner.py
--rw-r--r--   0        0        0     7940 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/main.py
--rw-r--r--   0        0        0     1554 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/models.py
--rw-r--r--   0        0        0       93 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/printers/__init__.py
--rw-r--r--   0        0        0      700 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/printers/base_printer.py
--rw-r--r--   0        0        0     1378 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/printers/base_table_printer.py
--rw-r--r--   0        0        0     1963 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/printers/console_printer.py
--rw-r--r--   0        0        0     1603 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/printers/json_printer.py
--rw-r--r--   0        0        0     5809 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/printers/sca_table_printer.py
--rw-r--r--   0        0        0     2266 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/printers/table.py
--rw-r--r--   0        0        0      477 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/printers/table_models.py
--rw-r--r--   0        0        0     5409 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/printers/table_printer.py
--rw-r--r--   0        0        0     9539 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/printers/text_printer.py
--rw-r--r--   0        0        0        0 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/user_settings/__init__.py
--rw-r--r--   0        0        0      533 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/user_settings/base_file_manager.py
--rw-r--r--   0        0        0     4485 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/user_settings/config_file_manager.py
--rw-r--r--   0        0        0     7054 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/user_settings/configuration_manager.py
--rw-r--r--   0        0        0     1862 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/user_settings/credentials_manager.py
--rw-r--r--   0        0        0     6548 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/user_settings/user_settings_commands.py
--rw-r--r--   0        0        0        0 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/utils/__init__.py
--rw-r--r--   0        0        0      154 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/utils/enum_utils.py
--rw-r--r--   0        0        0     2170 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/utils/path_utils.py
--rw-r--r--   0        0        0     7572 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/utils/progress_bar.py
--rw-r--r--   0        0        0     2751 2023-07-06 08:22:35.488955 cycode-0.2.6.dev9/cycode/cli/utils/scan_batch.py
--rw-r--r--   0        0        0      334 2023-07-06 08:22:35.488955 cycode-0.2.6.dev9/cycode/cli/utils/scan_utils.py
--rw-r--r--   0        0        0      970 2023-07-06 08:22:35.488955 cycode-0.2.6.dev9/cycode/cli/utils/shell_executor.py
--rw-r--r--   0        0        0     2004 2023-07-06 08:22:35.488955 cycode-0.2.6.dev9/cycode/cli/utils/string_utils.py
--rw-r--r--   0        0        0     2684 2023-07-06 08:22:35.488955 cycode-0.2.6.dev9/cycode/cli/utils/task_timer.py
--rw-r--r--   0        0        0      816 2023-07-06 08:22:35.488955 cycode-0.2.6.dev9/cycode/cli/utils/yaml_utils.py
--rw-r--r--   0        0        0      930 2023-07-06 08:22:35.488955 cycode-0.2.6.dev9/cycode/cli/zip_file.py
--rw-r--r--   0        0        0       56 2023-07-06 08:22:35.488955 cycode-0.2.6.dev9/cycode/cyclient/__init__.py
--rw-r--r--   0        0        0     1709 2023-07-06 08:22:35.488955 cycode-0.2.6.dev9/cycode/cyclient/auth_client.py
--rw-r--r--   0        0        0     2543 2023-07-06 08:22:35.488955 cycode-0.2.6.dev9/cycode/cyclient/config.py
--rw-r--r--   0        0        0      126 2023-07-06 08:22:35.488955 cycode-0.2.6.dev9/cycode/cyclient/config.yaml
--rw-r--r--   0        0        0      120 2023-07-06 08:22:35.488955 cycode-0.2.6.dev9/cycode/cyclient/config_dev.py
--rw-r--r--   0        0        0      220 2023-07-06 08:22:35.488955 cycode-0.2.6.dev9/cycode/cyclient/cycode_client.py
--rw-r--r--   0        0        0     3757 2023-07-06 08:22:35.488955 cycode-0.2.6.dev9/cycode/cyclient/cycode_client_base.py
--rw-r--r--   0        0        0      581 2023-07-06 08:22:35.488955 cycode-0.2.6.dev9/cycode/cyclient/cycode_dev_based_client.py
--rw-r--r--   0        0        0     1788 2023-07-06 08:22:35.488955 cycode-0.2.6.dev9/cycode/cyclient/cycode_token_based_client.py
--rw-r--r--   0        0        0     9412 2023-07-06 08:22:35.488955 cycode-0.2.6.dev9/cycode/cyclient/models.py
--rw-r--r--   0        0        0     6400 2023-07-06 08:22:35.488955 cycode-0.2.6.dev9/cycode/cyclient/scan_client.py
--rw-r--r--   0        0        0        0 2023-07-06 08:22:35.488955 cycode-0.2.6.dev9/cycode/cyclient/scan_config/__init__.py
--rw-r--r--   0        0        0     1165 2023-07-06 08:22:35.488955 cycode-0.2.6.dev9/cycode/cyclient/scan_config/scan_config_base.py
--rw-r--r--   0        0        0     1241 2023-07-06 08:22:35.488955 cycode-0.2.6.dev9/cycode/cyclient/scan_config/scan_config_creator.py
--rw-r--r--   0        0        0      199 2023-07-06 08:22:35.488955 cycode-0.2.6.dev9/cycode/cyclient/utils.py
--rw-r--r--   0        0        0       16 2023-07-06 08:22:35.488955 cycode-0.2.6.dev9/cycode/pre-commit-hook-version
--rw-r--r--   0        0        0     3138 2023-07-06 08:23:21.433194 cycode-0.2.6.dev9/pyproject.toml
--rw-r--r--   0        0        0    34044 1970-01-01 00:00:00.000000 cycode-0.2.6.dev9/PKG-INFO
+-rw-r--r--   0        0        0    33099 2023-07-30 08:05:46.108893 cycode-1.0.0/README.md
+-rw-r--r--   0        0        0      109 2023-07-30 08:06:03.940979 cycode-1.0.0/cycode/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-30 08:05:46.108893 cycode-1.0.0/cycode/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-30 08:05:46.108893 cycode-1.0.0/cycode/cli/auth/__init__.py
+-rw-r--r--   0        0        0     3003 2023-07-30 08:05:46.108893 cycode-1.0.0/cycode/cli/auth/auth_command.py
+-rw-r--r--   0        0        0     4727 2023-07-30 08:05:46.108893 cycode-1.0.0/cycode/cli/auth/auth_manager.py
+-rw-r--r--   0        0        0     1588 2023-07-30 08:05:46.108893 cycode-1.0.0/cycode/cli/ci_integrations.py
+-rw-r--r--   0        0        0    54675 2023-07-30 08:05:46.108893 cycode-1.0.0/cycode/cli/code_scanner.py
+-rw-r--r--   0        0        0      466 2023-07-30 08:05:46.108893 cycode-1.0.0/cycode/cli/config.py
+-rw-r--r--   0        0        0      387 2023-07-30 08:05:46.108893 cycode-1.0.0/cycode/cli/config.yaml
+-rw-r--r--   0        0        0     5819 2023-07-30 08:05:46.108893 cycode-1.0.0/cycode/cli/consts.py
+-rw-r--r--   0        0        0        0 2023-07-30 08:05:46.108893 cycode-1.0.0/cycode/cli/exceptions/__init__.py
+-rw-r--r--   0        0        0     1792 2023-07-30 08:05:46.108893 cycode-1.0.0/cycode/cli/exceptions/custom_exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-30 08:05:46.108893 cycode-1.0.0/cycode/cli/helpers/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-30 08:05:46.108893 cycode-1.0.0/cycode/cli/helpers/maven/__init__.py
+-rw-r--r--   0        0        0     2042 2023-07-30 08:05:46.108893 cycode-1.0.0/cycode/cli/helpers/maven/base_restore_maven_dependencies.py
+-rw-r--r--   0        0        0      983 2023-07-30 08:05:46.108893 cycode-1.0.0/cycode/cli/helpers/maven/restore_gradle_dependencies.py
+-rw-r--r--   0        0        0     3004 2023-07-30 08:05:46.108893 cycode-1.0.0/cycode/cli/helpers/maven/restore_maven_dependencies.py
+-rw-r--r--   0        0        0     5927 2023-07-30 08:05:46.108893 cycode-1.0.0/cycode/cli/helpers/sca_code_scanner.py
+-rw-r--r--   0        0        0     7805 2023-07-30 08:05:46.108893 cycode-1.0.0/cycode/cli/main.py
+-rw-r--r--   0        0        0     1584 2023-07-30 08:05:46.108893 cycode-1.0.0/cycode/cli/models.py
+-rw-r--r--   0        0        0       93 2023-07-30 08:05:46.108893 cycode-1.0.0/cycode/cli/printers/__init__.py
+-rw-r--r--   0        0        0     2078 2023-07-30 08:05:46.108893 cycode-1.0.0/cycode/cli/printers/console_printer.py
+-rw-r--r--   0        0        0     1973 2023-07-30 08:05:46.108893 cycode-1.0.0/cycode/cli/printers/json_printer.py
+-rw-r--r--   0        0        0      786 2023-07-30 08:05:46.108893 cycode-1.0.0/cycode/cli/printers/printer_base.py
+-rw-r--r--   0        0        0        0 2023-07-30 08:05:46.108893 cycode-1.0.0/cycode/cli/printers/tables/__init__.py
+-rw-r--r--   0        0        0     5853 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cli/printers/tables/sca_table_printer.py
+-rw-r--r--   0        0        0     2281 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cli/printers/tables/table.py
+-rw-r--r--   0        0        0      480 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cli/printers/tables/table_models.py
+-rw-r--r--   0        0        0     5471 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cli/printers/tables/table_printer.py
+-rw-r--r--   0        0        0     2025 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cli/printers/tables/table_printer_base.py
+-rw-r--r--   0        0        0    10099 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cli/printers/text_printer.py
+-rw-r--r--   0        0        0        0 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cli/user_settings/__init__.py
+-rw-r--r--   0        0        0      630 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cli/user_settings/base_file_manager.py
+-rw-r--r--   0        0        0     4741 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cli/user_settings/config_file_manager.py
+-rw-r--r--   0        0        0     7202 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cli/user_settings/configuration_manager.py
+-rw-r--r--   0        0        0     1954 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cli/user_settings/credentials_manager.py
+-rw-r--r--   0        0        0     6687 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cli/user_settings/user_settings_commands.py
+-rw-r--r--   0        0        0        0 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cli/utils/__init__.py
+-rw-r--r--   0        0        0      211 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cli/utils/enum_utils.py
+-rw-r--r--   0        0        0     2339 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cli/utils/path_utils.py
+-rw-r--r--   0        0        0     7619 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cli/utils/progress_bar.py
+-rw-r--r--   0        0        0     2782 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cli/utils/scan_batch.py
+-rw-r--r--   0        0        0      334 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cli/utils/scan_utils.py
+-rw-r--r--   0        0        0      978 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cli/utils/shell_executor.py
+-rw-r--r--   0        0        0     2034 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cli/utils/string_utils.py
+-rw-r--r--   0        0        0     2748 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cli/utils/task_timer.py
+-rw-r--r--   0        0        0      934 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cli/utils/yaml_utils.py
+-rw-r--r--   0        0        0     1011 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cli/zip_file.py
+-rw-r--r--   0        0        0       56 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cyclient/__init__.py
+-rw-r--r--   0        0        0     1749 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cyclient/auth_client.py
+-rw-r--r--   0        0        0     2664 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cyclient/config.py
+-rw-r--r--   0        0        0      126 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cyclient/config.yaml
+-rw-r--r--   0        0        0      120 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cyclient/config_dev.py
+-rw-r--r--   0        0        0      228 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cyclient/cycode_client.py
+-rw-r--r--   0        0        0     3954 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cyclient/cycode_client_base.py
+-rw-r--r--   0        0        0      640 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cyclient/cycode_dev_based_client.py
+-rw-r--r--   0        0        0     1848 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cyclient/cycode_token_based_client.py
+-rw-r--r--   0        0        0    10005 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cyclient/models.py
+-rw-r--r--   0        0        0     6407 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cyclient/scan_client.py
+-rw-r--r--   0        0        0        0 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cyclient/scan_config/__init__.py
+-rw-r--r--   0        0        0     1086 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cyclient/scan_config/scan_config_base.py
+-rw-r--r--   0        0        0     1254 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cyclient/scan_config/scan_config_creator.py
+-rw-r--r--   0        0        0     3476 2023-07-30 08:06:03.936979 cycode-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0    34635 1970-01-01 00:00:00.000000 cycode-1.0.0/PKG-INFO
```

### Comparing `cycode-0.2.6.dev9/README.md` & `cycode-1.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -209,27 +209,27 @@
 > A successful hook installation will result in the message:<br/>
 `Pre-commit installed at .git/hooks/pre-commit`
 
 # Cycode CLI Commands
 
 The following are the options and commands available with the Cycode CLI application:
 
-| Option                         | Description                                                       |
-|--------------------------------|-------------------------------------------------------------------|
-| `--output [text\|json\|table]` | Specify the output (`text`/`json`/`table`). The default is `text` |
-| `-v`, `--verbose`              | Show detailed logs                                                |
-| `--version`                    | Show the version and exit.                                        |
-| `--help`                       | Show options for given command.                                   |
-
-| Command                             | Description |
-|-------------------------------------|-------------|
-| [auth](#use-auth-command)           | Authenticates your machine to associate CLI with your Cycode account. |
-| [configure](#use-configure-command) | Initial command to authenticate your CLI client with Cycode using client ID and client secret. |
-| [ignore](#ingoring-scan-results)    | Ignore a specific value, path or rule ID |
-| [scan](#running-a-scan)             | Scan content for secrets/IaC/SCA/SAST violations. You need to specify which scan type: `ci`/`commit_history`/`path`/`repository`/etc |
+| Option                               | Description                                                        |
+|--------------------------------------|--------------------------------------------------------------------|
+| `-o`, `--output [text\|json\|table]` | Specify the output (`text`/`json`/`table`). The default is `text`. |
+| `-v`, `--verbose`                    | Show detailed logs.                                                |
+| `--help`                             | Show options for given command.                                    |
+
+| Command                             | Description                                                                                                                           |
+|-------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------|
+| [auth](#use-auth-command)           | Authenticates your machine to associate CLI with your Cycode account.                                                                 |
+| [configure](#use-configure-command) | Initial command to authenticate your CLI client with Cycode using client ID and client secret.                                        |
+| [ignore](#ingoring-scan-results)    | Ignore a specific value, path or rule ID.                                                                                             |
+| [scan](#running-a-scan)             | Scan content for secrets/IaC/SCA/SAST violations. You need to specify which scan type: `ci`/`commit_history`/`path`/`repository`/etc. |
+| version                             | Show the version and exit.                                                                                                            |
 
 # Running a Scan
 
 The Cycode CLI application offers several types of scans so that you can choose the option that best fits your case. The following are the current options and commands available:
 
 | Option                               | Description                                                                |
 |--------------------------------------|----------------------------------------------------------------------------|
@@ -551,14 +551,15 @@
 
 # Ignoring Scan Results
 
 Ignore rules can be added to ignore specific secret values, specific SHA512 values, specific paths, and specific Cycode secret and IaC rule IDs. This will cause the scan to not alert these values. The ignore rules are written and saved locally in the `./.cycode/config.yaml` file.
 
 > :warning: **Warning**<br/>
 > Adding values to be ignored should be done with careful consideration of the values, paths, and policies to ensure that the scans will pick up true positives.
+
 The following are the options available for the `cycode ignore` command:
 
 | Option                          | Description |
 |---------------------------------|-------------|
 | `--by-value TEXT`               | Ignore a specific value while scanning for secrets. See [Ignoring a Secret Value](#ignoring-a-secret-value) for more details. |
 | `--by-sha TEXT`                 | Ignore a specific SHA512 representation of a string while scanning for secrets. See [Ignoring a Secret SHA Value](#ignoring-a-secret-sha-value) for more details. |
 | `--by-path TEXT`                | Avoid scanning a specific path. Need to specify scan type. See [Ignoring a Path](#ignoring-a-path) for more details. |
```

### Comparing `cycode-0.2.6.dev9/cycode/cli/auth/auth_command.py` & `cycode-1.0.0/cycode/cli/auth/auth_command.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,18 +8,19 @@
 from cycode.cli.printers import ConsolePrinter
 from cycode.cli.user_settings.credentials_manager import CredentialsManager
 from cycode.cyclient import logger
 from cycode.cyclient.cycode_token_based_client import CycodeTokenBasedClient
 
 
 @click.group(
-    invoke_without_command=True, short_help='Authenticates your machine to associate CLI with your cycode account'
+    invoke_without_command=True, short_help='Authenticate your machine to associate the CLI with your Cycode account.'
 )
 @click.pass_context
-def authenticate(context: click.Context):
+def authenticate(context: click.Context) -> None:
+    """Authenticates your machine."""
     if context.invoked_subcommand is not None:
         # if it is a subcommand, do nothing
         return
 
     try:
         logger.debug('Starting authentication process')
 
@@ -28,51 +29,57 @@
 
         result = CliResult(success=True, message='Successfully logged into cycode')
         ConsolePrinter(context).print_result(result)
     except Exception as e:
         _handle_exception(context, e)
 
 
-@authenticate.command(name='check')
+@authenticate.command(
+    name='check', short_help='Checks that your machine is associating the CLI with your Cycode account.'
+)
 @click.pass_context
-def authorization_check(context: click.Context):
-    """Check your machine associating CLI with your cycode account"""
+def authorization_check(context: click.Context) -> None:
+    """Validates that your Cycode account has permission to work with the CLI."""
     printer = ConsolePrinter(context)
 
-    passed_auth_check_res = CliResult(success=True, message='You are authorized')
-    failed_auth_check_res = CliResult(success=False, message='You are not authorized')
+    passed_auth_check_res = CliResult(success=True, message='Cycode authentication verified')
+    failed_auth_check_res = CliResult(success=False, message='Cycode authentication failed')
 
     client_id, client_secret = CredentialsManager().get_credentials()
     if not client_id or not client_secret:
-        return printer.print_result(failed_auth_check_res)
+        printer.print_result(failed_auth_check_res)
+        return
 
     try:
         if CycodeTokenBasedClient(client_id, client_secret).api_token:
-            return printer.print_result(passed_auth_check_res)
+            printer.print_result(passed_auth_check_res)
+            return
     except (NetworkError, HttpUnauthorizedError):
         if context.obj['verbose']:
             click.secho(f'Error: {traceback.format_exc()}', fg='red')
 
-        return printer.print_result(failed_auth_check_res)
+        printer.print_result(failed_auth_check_res)
+        return
 
 
-def _handle_exception(context: click.Context, e: Exception):
+def _handle_exception(context: click.Context, e: Exception) -> None:
     if context.obj['verbose']:
         click.secho(f'Error: {traceback.format_exc()}', fg='red')
 
     errors: CliErrors = {
         AuthProcessError: CliError(
             code='auth_error', message='Authentication failed. Please try again later using the command `cycode auth`'
         ),
         NetworkError: CliError(
             code='cycode_error', message='Authentication failed. Please try again later using the command `cycode auth`'
         ),
     }
 
     error = errors.get(type(e))
     if error:
-        return ConsolePrinter(context).print_error(error)
+        ConsolePrinter(context).print_error(error)
+        return
 
     if isinstance(e, click.ClickException):
         raise e
 
     raise click.ClickException(str(e))
```

### Comparing `cycode-0.2.6.dev9/cycode/cli/auth/auth_manager.py` & `cycode-1.0.0/cycode/cli/auth/auth_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 import time
 import webbrowser
-from typing import Optional
+from typing import TYPE_CHECKING, Tuple
 
 from requests import Request
 
 from cycode.cli.exceptions.custom_exceptions import AuthProcessError
 from cycode.cli.user_settings.configuration_manager import ConfigurationManager
 from cycode.cli.user_settings.credentials_manager import CredentialsManager
 from cycode.cli.utils.string_utils import generate_random_string, hash_string_to_sha256
 from cycode.cyclient import logger
 from cycode.cyclient.auth_client import AuthClient
-from cycode.cyclient.models import ApiToken, ApiTokenGenerationPollingResponse
+from cycode.cyclient.models import ApiTokenGenerationPollingResponse
+
+if TYPE_CHECKING:
+    from cycode.cyclient.models import ApiToken
 
 
 class AuthManager:
     CODE_VERIFIER_LENGTH = 101
     POLLING_WAIT_INTERVAL_IN_SECONDS = 3
     POLLING_TIMEOUT_IN_SECONDS = 180
     FAILED_POLLING_STATUS = 'Error'
     COMPLETED_POLLING_STATUS = 'Completed'
 
-    configuration_manager: ConfigurationManager
-    credentials_manager: CredentialsManager
-    auth_client: AuthClient
-
-    def __init__(self):
+    def __init__(self) -> None:
         self.configuration_manager = ConfigurationManager()
         self.credentials_manager = CredentialsManager()
         self.auth_client = AuthClient()
 
-    def authenticate(self):
+    def authenticate(self) -> None:
         logger.debug('generating pkce code pair')
         code_challenge, code_verifier = self._generate_pkce_code_pair()
 
         logger.debug('starting authentication session')
         session_id = self.start_session(code_challenge)
         logger.debug('authentication session created, %s', {'session_id': session_id})
 
@@ -42,55 +41,55 @@
 
         logger.debug('starting get api token process')
         api_token = self.get_api_token(session_id, code_verifier)
 
         logger.debug('saving get api token')
         self.save_api_token(api_token)
 
-    def start_session(self, code_challenge: str):
+    def start_session(self, code_challenge: str) -> str:
         auth_session = self.auth_client.start_session(code_challenge)
         return auth_session.session_id
 
-    def redirect_to_login_page(self, code_challenge: str, session_id: str):
+    def redirect_to_login_page(self, code_challenge: str, session_id: str) -> None:
         login_url = self._build_login_url(code_challenge, session_id)
         webbrowser.open(login_url)
 
-    def get_api_token(self, session_id: str, code_verifier: str) -> Optional[ApiToken]:
+    def get_api_token(self, session_id: str, code_verifier: str) -> 'ApiToken':
         api_token = self.get_api_token_polling(session_id, code_verifier)
         if api_token is None:
             raise AuthProcessError('getting api token is completed, but the token is missing')
         return api_token
 
-    def get_api_token_polling(self, session_id: str, code_verifier: str) -> Optional[ApiToken]:
+    def get_api_token_polling(self, session_id: str, code_verifier: str) -> 'ApiToken':
         end_polling_time = time.time() + self.POLLING_TIMEOUT_IN_SECONDS
         while time.time() < end_polling_time:
             logger.debug('trying to get api token...')
             api_token_polling_response = self.auth_client.get_api_token(session_id, code_verifier)
             if self._is_api_token_process_completed(api_token_polling_response):
                 logger.debug('get api token process completed')
                 return api_token_polling_response.api_token
             if self._is_api_token_process_failed(api_token_polling_response):
                 logger.debug('get api token process failed')
                 raise AuthProcessError('error during getting api token')
             time.sleep(self.POLLING_WAIT_INTERVAL_IN_SECONDS)
 
         raise AuthProcessError('session expired')
 
-    def save_api_token(self, api_token: ApiToken):
+    def save_api_token(self, api_token: 'ApiToken') -> None:
         self.credentials_manager.update_credentials_file(api_token.client_id, api_token.secret)
 
-    def _build_login_url(self, code_challenge: str, session_id: str):
+    def _build_login_url(self, code_challenge: str, session_id: str) -> str:
         app_url = self.configuration_manager.get_cycode_app_url()
         login_url = f'{app_url}/account/sign-in'
         query_params = {'source': 'cycode_cli', 'code_challenge': code_challenge, 'session_id': session_id}
         # TODO(MarshalX). Use auth_client instead and don't depend on "requests" lib here
         request = Request(url=login_url, params=query_params)
         return request.prepare().url
 
-    def _generate_pkce_code_pair(self) -> (str, str):
+    def _generate_pkce_code_pair(self) -> Tuple[str, str]:
         code_verifier = generate_random_string(self.CODE_VERIFIER_LENGTH)
         code_challenge = hash_string_to_sha256(code_verifier)
         return code_challenge, code_verifier
 
     def _is_api_token_process_completed(self, api_token_polling_response: ApiTokenGenerationPollingResponse) -> bool:
         return (
             api_token_polling_response is not None
```

### Comparing `cycode-0.2.6.dev9/cycode/cli/ci_integrations.py` & `cycode-1.0.0/cycode/cli/ci_integrations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 
 import click
 
 
-def github_action_range():
+def github_action_range() -> str:
     before_sha = os.getenv('BEFORE_SHA')
     push_base_sha = os.getenv('BASE_SHA')
     pr_base_sha = os.getenv('PR_BASE_SHA')
     default_branch = os.getenv('DEFAULT_BRANCH')
     head_sha = os.getenv('GITHUB_SHA')
     ref = os.getenv('GITHUB_REF')
 
@@ -18,39 +18,39 @@
     return '...'
 
     # if pr_base_sha and pr_base_sha != FIRST_COMMIT:
     #
     # if push_base_sha and push_base_sha != "null":
 
 
-def circleci_range():
+def circleci_range() -> str:
     before_sha = os.getenv('BEFORE_SHA')
     current_sha = os.getenv('CURRENT_SHA')
     commit_range = f'{before_sha}...{current_sha}'
     click.echo(f'commit range: {commit_range}')
 
     if not commit_range.startswith('...'):
         return commit_range
 
     commit_sha = os.getenv('CIRCLE_SHA1', 'HEAD')
 
     return f'{commit_sha}~1...'
 
 
-def gitlab_range():
+def gitlab_range() -> str:
     before_sha = os.getenv('CI_COMMIT_BEFORE_SHA')
     commit_sha = os.getenv('CI_COMMIT_SHA', 'HEAD')
 
     if before_sha and before_sha != NO_COMMITS:
         return f'{before_sha}...'
 
     return f'{commit_sha}'
 
 
-def get_commit_range():
+def get_commit_range() -> str:
     if os.getenv('GITHUB_ACTIONS'):
         return github_action_range()
     if os.getenv('CIRCLECI'):
         return circleci_range()
     if os.getenv('GITLAB_CI'):
         return gitlab_range()
```

### Comparing `cycode-0.2.6.dev9/cycode/cli/code_scanner.py` & `cycode-1.0.0/cycode/cli/code_scanner.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import logging
 import os
 import sys
 import time
 import traceback
 from platform import platform
 from sys import getsizeof
-from typing import TYPE_CHECKING, Callable, Dict, List, Optional, Tuple
+from typing import TYPE_CHECKING, Callable, Dict, Iterator, List, Optional, Tuple, Union
 from uuid import UUID, uuid4
 
 import click
 from git import NULL_TREE, InvalidGitRepositoryError, Repo
 
 from cycode.cli import consts
 from cycode.cli.ci_integrations import get_commit_range
@@ -36,88 +36,97 @@
 from cycode.cli.utils.string_utils import get_content_size, is_binary_content
 from cycode.cli.utils.task_timer import TimeoutAfter
 from cycode.cli.zip_file import InMemoryZip
 from cycode.cyclient import logger
 from cycode.cyclient.models import Detection, DetectionSchema, DetectionsPerFile, ZippedFileScanResult
 
 if TYPE_CHECKING:
+    from git import Blob, Diff
+    from git.objects.base import IndexObjUnion
+    from git.objects.tree import TraversedTreeTup
+
     from cycode.cli.utils.progress_bar import BaseProgressBar
     from cycode.cyclient.models import ScanDetailsResponse
     from cycode.cyclient.scan_client import ScanClient
 
 start_scan_time = time.time()
 
 
-@click.command(short_help='Scan git repository including its history')
-@click.argument('path', nargs=1, type=click.STRING, required=True)
+@click.command(short_help='Scan the git repository including its history.')
+@click.argument('path', nargs=1, type=click.Path(exists=True, resolve_path=True), required=True)
 @click.option(
     '--branch',
     '-b',
     default=None,
     help='Branch to scan, if not set scanning the default branch',
     type=str,
     required=False,
 )
 @click.pass_context
-def scan_repository(context: click.Context, path: str, branch: str):
+def scan_repository(context: click.Context, path: str, branch: str) -> None:
     try:
         logger.debug('Starting repository scan process, %s', {'path': path, 'branch': branch})
 
         scan_type = context.obj['scan_type']
         monitor = context.obj.get('monitor')
         if monitor and scan_type != consts.SCA_SCAN_TYPE:
             raise click.ClickException('Monitor flag is currently supported for SCA scan type only')
 
         progress_bar = context.obj['progress_bar']
+        progress_bar.start()
 
         file_entries = list(get_git_repository_tree_file_entries(path, branch))
         progress_bar.set_section_length(ProgressBarSection.PREPARE_LOCAL_FILES, len(file_entries))
 
         documents_to_scan = []
         for file in file_entries:
+            # FIXME(MarshalX): probably file could be tree or submodule too. we expect blob only
             progress_bar.update(ProgressBarSection.PREPARE_LOCAL_FILES)
 
-            path = file.path if monitor else get_path_by_os(os.path.join(path, file.path))
-
-            documents_to_scan.append(Document(path, file.data_stream.read().decode('UTF-8', errors='replace')))
+            file_path = file.path if monitor else get_path_by_os(os.path.join(path, file.path))
+            documents_to_scan.append(Document(file_path, file.data_stream.read().decode('UTF-8', errors='replace')))
 
         documents_to_scan = exclude_irrelevant_documents_to_scan(context, documents_to_scan)
 
         perform_pre_scan_documents_actions(context, scan_type, documents_to_scan, is_git_diff=False)
 
         logger.debug('Found all relevant files for scanning %s', {'path': path, 'branch': branch})
-        return scan_documents(
+        scan_documents(
             context, documents_to_scan, is_git_diff=False, scan_parameters=get_scan_parameters(context, path)
         )
     except Exception as e:
         _handle_exception(context, e)
 
 
-@click.command(short_help='Scan all the commits history in this git repository')
-@click.argument('path', nargs=1, type=click.STRING, required=True)
+@click.command(short_help='Scan all the commits history in this git repository.')
+@click.argument('path', nargs=1, type=click.Path(exists=True, resolve_path=True), required=True)
 @click.option(
     '--commit_range',
     '-r',
     help='Scan a commit range in this git repository, by default cycode scans all commit history (example: HEAD~1)',
     type=click.STRING,
     default='--all',
     required=False,
 )
 @click.pass_context
-def scan_repository_commit_history(context: click.Context, path: str, commit_range: str):
+def scan_repository_commit_history(context: click.Context, path: str, commit_range: str) -> None:
     try:
         logger.debug('Starting commit history scan process, %s', {'path': path, 'commit_range': commit_range})
-        return scan_commit_range(context, path=path, commit_range=commit_range)
+        scan_commit_range(context, path=path, commit_range=commit_range)
     except Exception as e:
         _handle_exception(context, e)
 
 
-def scan_commit_range(context: click.Context, path: str, commit_range: str, max_commits_count: Optional[int] = None):
+def scan_commit_range(
+    context: click.Context, path: str, commit_range: str, max_commits_count: Optional[int] = None
+) -> None:
     scan_type = context.obj['scan_type']
+
     progress_bar = context.obj['progress_bar']
+    progress_bar.start()
 
     if scan_type not in consts.COMMIT_RANGE_SCAN_SUPPORTED_SCAN_TYPES:
         raise click.ClickException(f'Commit range scanning for {str.upper(scan_type)} is not supported')
 
     if scan_type == consts.SCA_SCAN_TYPE:
         return scan_sca_commit_range(context, path, commit_range)
 
@@ -162,64 +171,91 @@
 
         documents_to_scan.extend(exclude_irrelevant_documents_to_scan(context, commit_documents_to_scan))
         scanned_commits_count += 1
 
     logger.debug('List of commit ids to scan, %s', {'commit_ids': commit_ids_to_scan})
     logger.debug('Starting to scan commit range (It may take a few minutes)')
 
-    return scan_documents(context, documents_to_scan, is_git_diff=True, is_commit_range=True)
+    scan_documents(context, documents_to_scan, is_git_diff=True, is_commit_range=True)
+    return None
 
 
 @click.command(
     short_help='Execute scan in a CI environment which relies on the '
     'CYCODE_TOKEN and CYCODE_REPO_LOCATION environment variables'
 )
 @click.pass_context
-def scan_ci(context: click.Context):
-    return scan_commit_range(context, path=os.getcwd(), commit_range=get_commit_range())
+def scan_ci(context: click.Context) -> None:
+    scan_commit_range(context, path=os.getcwd(), commit_range=get_commit_range())
 
 
-@click.command(short_help='Scan the files in the path supplied in the command')
-@click.argument('path', nargs=1, type=click.STRING, required=True)
+@click.command(short_help='Scan the files in the path provided in the command.')
+@click.argument('path', nargs=1, type=click.Path(exists=True, resolve_path=True), required=True)
 @click.pass_context
-def scan_path(context: click.Context, path):
+def scan_path(context: click.Context, path: str) -> None:
+    progress_bar = context.obj['progress_bar']
+    progress_bar.start()
+
     logger.debug('Starting path scan process, %s', {'path': path})
-    files_to_scan = get_relevant_files_in_path(path=path, exclude_patterns=['**/.git/**', '**/.cycode/**'])
-    files_to_scan = exclude_irrelevant_files(context, files_to_scan)
-    logger.debug('Found all relevant files for scanning %s', {'path': path, 'file_to_scan_count': len(files_to_scan)})
-    return scan_disk_files(context, path, files_to_scan)
+
+    all_files_to_scan = get_relevant_files_in_path(path=path, exclude_patterns=['**/.git/**', '**/.cycode/**'])
+
+    # we are double the progress bar section length because we are going to process the files twice
+    # first time to get the file list with respect of excluded patterns (excluding takes seconds to execute)
+    # second time to get the files content
+    progress_bar_section_len = len(all_files_to_scan) * 2
+    progress_bar.set_section_length(ProgressBarSection.PREPARE_LOCAL_FILES, progress_bar_section_len)
+
+    relevant_files_to_scan = exclude_irrelevant_files(context, all_files_to_scan)
+
+    # after finishing the first processing (excluding),
+    # we must update the progress bar stage with respect of excluded files.
+    # now it's possible that we will not process x2 of the files count
+    # because some of them were excluded, we should subtract the excluded files count
+    # from the progress bar section length
+    excluded_files_count = len(all_files_to_scan) - len(relevant_files_to_scan)
+    progress_bar_section_len = progress_bar_section_len - excluded_files_count
+    progress_bar.set_section_length(ProgressBarSection.PREPARE_LOCAL_FILES, progress_bar_section_len)
+
+    logger.debug(
+        'Found all relevant files for scanning %s', {'path': path, 'file_to_scan_count': len(relevant_files_to_scan)}
+    )
+    scan_disk_files(context, path, relevant_files_to_scan)
 
 
-@click.command(short_help='Use this command to scan the content that was not committed yet')
+@click.command(short_help='Use this command to scan any content that was not committed yet.')
 @click.argument('ignored_args', nargs=-1, type=click.UNPROCESSED)
 @click.pass_context
-def pre_commit_scan(context: click.Context, ignored_args: List[str]):
+def pre_commit_scan(context: click.Context, ignored_args: List[str]) -> None:
     scan_type = context.obj['scan_type']
+
     progress_bar = context.obj['progress_bar']
+    progress_bar.start()
 
     if scan_type == consts.SCA_SCAN_TYPE:
-        return scan_sca_pre_commit(context)
+        scan_sca_pre_commit(context)
+        return
 
     diff_files = Repo(os.getcwd()).index.diff('HEAD', create_patch=True, R=True)
 
     progress_bar.set_section_length(ProgressBarSection.PREPARE_LOCAL_FILES, len(diff_files))
 
     documents_to_scan = []
     for file in diff_files:
         progress_bar.update(ProgressBarSection.PREPARE_LOCAL_FILES)
         documents_to_scan.append(Document(get_path_by_os(get_diff_file_path(file)), get_diff_file_content(file)))
 
     documents_to_scan = exclude_irrelevant_documents_to_scan(context, documents_to_scan)
-    return scan_documents(context, documents_to_scan, is_git_diff=True)
+    scan_documents(context, documents_to_scan, is_git_diff=True)
 
 
-@click.command(short_help='Use this command to scan commits on the server side before pushing them to the repository')
+@click.command(short_help='Use this command to scan commits on the server side before pushing them to the repository.')
 @click.argument('ignored_args', nargs=-1, type=click.UNPROCESSED)
 @click.pass_context
-def pre_receive_scan(context: click.Context, ignored_args: List[str]):
+def pre_receive_scan(context: click.Context, ignored_args: List[str]) -> None:
     try:
         scan_type = context.obj['scan_type']
         if scan_type != consts.SECRET_SCAN_TYPE:
             raise click.ClickException(f'Commit range scanning for {scan_type.upper()} is not supported')
 
         if should_skip_pre_receive_scan():
             logger.info(
@@ -249,69 +285,65 @@
             max_commits_to_scan = configuration_manager.get_pre_receive_max_commits_to_scan_count(command_scan_type)
             scan_commit_range(context, os.getcwd(), commit_range, max_commits_count=max_commits_to_scan)
             perform_post_pre_receive_scan_actions(context)
     except Exception as e:
         _handle_exception(context, e)
 
 
-def scan_sca_pre_commit(context: click.Context):
+def scan_sca_pre_commit(context: click.Context) -> None:
     scan_parameters = get_default_scan_parameters(context)
     git_head_documents, pre_committed_documents = get_pre_commit_modified_documents(context.obj['progress_bar'])
     git_head_documents = exclude_irrelevant_documents_to_scan(context, git_head_documents)
     pre_committed_documents = exclude_irrelevant_documents_to_scan(context, pre_committed_documents)
     sca_code_scanner.perform_pre_hook_range_scan_actions(git_head_documents, pre_committed_documents)
-    return scan_commit_range_documents(
+    scan_commit_range_documents(
         context,
         git_head_documents,
         pre_committed_documents,
         scan_parameters,
         configuration_manager.get_sca_pre_commit_timeout_in_seconds(),
     )
 
 
-def scan_sca_commit_range(context: click.Context, path: str, commit_range: str):
+def scan_sca_commit_range(context: click.Context, path: str, commit_range: str) -> None:
     progress_bar = context.obj['progress_bar']
 
     scan_parameters = get_scan_parameters(context, path)
     from_commit_rev, to_commit_rev = parse_commit_range(commit_range, path)
     from_commit_documents, to_commit_documents = get_commit_range_modified_documents(
         progress_bar, path, from_commit_rev, to_commit_rev
     )
     from_commit_documents = exclude_irrelevant_documents_to_scan(context, from_commit_documents)
     to_commit_documents = exclude_irrelevant_documents_to_scan(context, to_commit_documents)
     sca_code_scanner.perform_pre_commit_range_scan_actions(
         path, from_commit_documents, from_commit_rev, to_commit_documents, to_commit_rev
     )
 
-    return scan_commit_range_documents(
-        context, from_commit_documents, to_commit_documents, scan_parameters=scan_parameters
-    )
+    scan_commit_range_documents(context, from_commit_documents, to_commit_documents, scan_parameters=scan_parameters)
 
 
-def scan_disk_files(context: click.Context, path: str, files_to_scan: List[str]):
+def scan_disk_files(context: click.Context, path: str, files_to_scan: List[str]) -> None:
     scan_parameters = get_scan_parameters(context, path)
     scan_type = context.obj['scan_type']
     progress_bar = context.obj['progress_bar']
 
     is_git_diff = False
 
-    progress_bar.set_section_length(ProgressBarSection.PREPARE_LOCAL_FILES, len(files_to_scan))
-
     documents: List[Document] = []
     for file in files_to_scan:
         progress_bar.update(ProgressBarSection.PREPARE_LOCAL_FILES)
 
-        with open(file, 'r', encoding='UTF-8') as f:
-            try:
-                documents.append(Document(file, f.read(), is_git_diff))
-            except UnicodeDecodeError:
-                continue
+        content = get_file_content(file)
+        if not content:
+            continue
+
+        documents.append(Document(file, content, is_git_diff))
 
     perform_pre_scan_documents_actions(context, scan_type, documents, is_git_diff)
-    return scan_documents(context, documents, is_git_diff=is_git_diff, scan_parameters=scan_parameters)
+    scan_documents(context, documents, is_git_diff=is_git_diff, scan_parameters=scan_parameters)
 
 
 def set_issue_detected_by_scan_results(context: click.Context, scan_results: List[LocalScanResult]) -> None:
     set_issue_detected(context, any(scan_result.issue_detected for scan_result in scan_results))
 
 
 def _get_scan_documents_thread_func(
@@ -384,43 +416,35 @@
     documents_to_scan: List[Document],
     is_git_diff: bool = False,
     is_commit_range: bool = False,
     scan_parameters: Optional[dict] = None,
 ) -> None:
     progress_bar = context.obj['progress_bar']
 
+    if not documents_to_scan:
+        progress_bar.stop()
+        ConsolePrinter(context).print_error(
+            CliError(
+                code='no_relevant_files',
+                message='Error: The scan could not be completed - relevant files to scan are not found.',
+            )
+        )
+        return
+
     scan_batch_thread_func = _get_scan_documents_thread_func(context, is_git_diff, is_commit_range, scan_parameters)
     errors, local_scan_results = run_parallel_batched_scan(
         scan_batch_thread_func, documents_to_scan, progress_bar=progress_bar
     )
 
     progress_bar.set_section_length(ProgressBarSection.GENERATE_REPORT, 1)
     progress_bar.update(ProgressBarSection.GENERATE_REPORT)
     progress_bar.stop()
 
     set_issue_detected_by_scan_results(context, local_scan_results)
-    print_results(context, local_scan_results)
-
-    if not errors:
-        return
-
-    if context.obj['output'] == 'json':
-        # TODO(MarshalX): we can't just print JSON formatted errors here
-        #  because we should return only one root json structure per scan
-        #  could be added later to "print_results" function if we wish to display detailed errors in UI
-        return
-
-    click.secho(
-        'Unfortunately, Cycode was unable to complete the full scan. '
-        'Please note that not all results may be available:',
-        fg='red',
-    )
-    for scan_id, error in errors.items():
-        click.echo(f'- {scan_id}: ', nl=False)
-        ConsolePrinter(context).print_error(error)
+    print_results(context, local_scan_results, errors)
 
 
 def scan_commit_range_documents(
     context: click.Context,
     from_documents_to_scan: List[Document],
     to_documents_to_scan: List[Document],
     scan_parameters: Optional[dict] = None,
@@ -470,14 +494,15 @@
             scan_result, to_documents_to_scan, scan_command_type, scan_type, severity_threshold
         )
         set_issue_detected_by_scan_results(context, [local_scan_result])
 
         progress_bar.update(ProgressBarSection.GENERATE_REPORT)
         progress_bar.stop()
 
+        # errors will be handled with try-except block; printing will not occur on errors
         print_results(context, [local_scan_result])
 
         scan_completed = True
     except Exception as e:
         _handle_exception(context, e)
         error_message = str(e)
 
@@ -657,17 +682,19 @@
     logger.debug(f'Scan update: (scan_id: {scan_details_response.id})')
     logger.debug(f'Scan status: {scan_details_response.scan_status}')
 
     if scan_details_response.message:
         logger.debug(f'Scan message: {scan_details_response.message}')
 
 
-def print_results(context: click.Context, local_scan_results: List[LocalScanResult]) -> None:
+def print_results(
+    context: click.Context, local_scan_results: List[LocalScanResult], errors: Optional[Dict[str, 'CliError']] = None
+) -> None:
     printer = ConsolePrinter(context)
-    printer.print_scan_results(local_scan_results)
+    printer.print_scan_results(local_scan_results, errors)
 
 
 def get_document_detections(
     scan_result: ZippedFileScanResult, documents_to_scan: List[Document]
 ) -> List[DocumentDetections]:
     logger.debug('Get document detections')
 
@@ -753,27 +780,29 @@
     not_updated_commits = Repo(os.getcwd()).git.rev_list(commit, '--topo-order', '--reverse', '--not', '--all')
     commits = not_updated_commits.splitlines()
     if not commits:
         return None
     return commits[0]
 
 
-def get_diff_file_path(file):
+def get_diff_file_path(file: 'Diff') -> Optional[str]:
     return file.b_path if file.b_path else file.a_path
 
 
-def get_diff_file_content(file):
+def get_diff_file_content(file: 'Diff') -> str:
     return file.diff.decode('UTF-8', errors='replace')
 
 
-def should_process_git_object(obj, _: int) -> bool:
+def should_process_git_object(obj: 'Blob', _: int) -> bool:
     return obj.type == 'blob' and obj.size > 0
 
 
-def get_git_repository_tree_file_entries(path: str, branch: str):
+def get_git_repository_tree_file_entries(
+    path: str, branch: str
+) -> Union[Iterator['IndexObjUnion'], Iterator['TraversedTreeTup']]:
     return Repo(path).tree(branch).traverse(predicate=should_process_git_object)
 
 
 def get_default_scan_parameters(context: click.Context) -> dict:
     return {
         'monitor': context.obj.get('monitor'),
         'report': context.obj.get('report'),
@@ -814,20 +843,24 @@
             relevant_documents.append(document)
 
     return relevant_documents
 
 
 def exclude_irrelevant_files(context: click.Context, filenames: List[str]) -> List[str]:
     scan_type = context.obj['scan_type']
+    progress_bar = context.obj['progress_bar']
 
     relevant_files = []
     for filename in filenames:
+        progress_bar.update(ProgressBarSection.PREPARE_LOCAL_FILES)
         if _is_relevant_file_to_scan(scan_type, filename):
             relevant_files.append(filename)
 
+    is_sub_path.cache_clear()  # free up memory
+
     return relevant_files
 
 
 def exclude_irrelevant_detections(
     detections: List[Detection], scan_type: str, command_scan_type: str, severity_threshold: str
 ) -> List[Detection]:
     relevant_detections = _exclude_detections_by_exclusions_configuration(detections, scan_type)
@@ -863,15 +896,15 @@
         and exclude_in_deleted_lines
     ):
         return exclude_detections_in_deleted_lines(detections)
 
     return detections
 
 
-def exclude_detections_in_deleted_lines(detections) -> List:
+def exclude_detections_in_deleted_lines(detections: List[Detection]) -> List[Detection]:
     return [detection for detection in detections if detection.detection_details.get('line_type') != 'Removed']
 
 
 def _exclude_detections_by_exclusions_configuration(detections: List[Detection], scan_type: str) -> List[Detection]:
     exclusions = configuration_manager.get_exclusions_by_scan_type(scan_type)
     return [detection for detection in detections if not _should_exclude_detection(detection, exclusions)]
 
@@ -965,15 +998,15 @@
                 'Going to ignore violations because is in the packages to ignore list, %s', {'package': package}
             )
             return True
 
     return False
 
 
-def _is_detection_sha_configured_in_exclusions(detection, exclusions: List[str]) -> bool:
+def _is_detection_sha_configured_in_exclusions(detection: Detection, exclusions: List[str]) -> bool:
     detection_sha = detection.detection_details.get('sha512', '')
     return detection_sha in exclusions
 
 
 def _is_path_configured_in_exclusions(scan_type: str, file_path: str) -> bool:
     exclusions_by_path = configuration_manager.get_exclusions_by_scan_type(scan_type).get(
         consts.EXCLUSIONS_BY_PATH_SECTION_NAME, []
@@ -1054,28 +1087,20 @@
     return True
 
 
 def _is_file_extension_supported(scan_type: str, filename: str) -> bool:
     filename = filename.lower()
 
     if scan_type == consts.INFRA_CONFIGURATION_SCAN_TYPE:
-        return any(
-            filename.endswith(supported_file_extension)
-            for supported_file_extension in consts.INFRA_CONFIGURATION_SCAN_SUPPORTED_FILES
-        )
+        return filename.endswith(consts.INFRA_CONFIGURATION_SCAN_SUPPORTED_FILES)
 
     if scan_type == consts.SCA_SCAN_TYPE:
-        return any(
-            filename.endswith(supported_file) for supported_file in consts.SCA_CONFIGURATION_SCAN_SUPPORTED_FILES
-        )
+        return filename.endswith(consts.SCA_CONFIGURATION_SCAN_SUPPORTED_FILES)
 
-    return all(
-        not filename.endswith(file_extension_to_ignore)
-        for file_extension_to_ignore in consts.SECRET_SCAN_FILE_EXTENSIONS_TO_IGNORE
-    )
+    return not filename.endswith(consts.SECRET_SCAN_FILE_EXTENSIONS_TO_IGNORE)
 
 
 def _does_file_exceed_max_size_limit(filename: str) -> bool:
     return get_file_size(filename) > consts.FILE_MAX_SIZE_LIMIT_IN_BYTES
 
 
 def _does_document_exceed_max_size_limit(content: str) -> bool:
@@ -1132,15 +1157,15 @@
             'Please try ignoring irrelevant paths using the `cycode ignore --by-path` command '
             'and execute the scan again',
         ),
         InvalidGitRepositoryError: CliError(
             soft_fail=False,
             code='invalid_git_error',
             message='The path you supplied does not correlate to a git repository. '
-            'Should you still wish to scan this path, use: `cycode scan path <path>`',
+            'If you still wish to scan this path, use: `cycode scan path <path>`',
         ),
     }
 
     if type(e) in errors:
         error = errors[type(e)]
 
         if error.soft_fail is True:
```

### Comparing `cycode-0.2.6.dev9/cycode/cli/consts.py` & `cycode-1.0.0/cycode/cli/consts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,25 @@
+PROGRAM_NAME = 'cycode'
+CLI_CONTEXT_SETTINGS = {
+    'terminal_width': 10**9,
+    'max_content_width': 10**9,
+}
+
 PRE_COMMIT_COMMAND_SCAN_TYPE = 'pre_commit'
 PRE_RECEIVE_COMMAND_SCAN_TYPE = 'pre_receive'
 COMMIT_HISTORY_COMMAND_SCAN_TYPE = 'commit_history'
 
 SECRET_SCAN_TYPE = 'secret'  # noqa: S105
 INFRA_CONFIGURATION_SCAN_TYPE = 'iac'
 SCA_SCAN_TYPE = 'sca'
 SAST_SCAN_TYPE = 'sast'
 
-INFRA_CONFIGURATION_SCAN_SUPPORTED_FILES = ['.tf', '.tf.json', '.json', '.yaml', '.yml', 'dockerfile']
+INFRA_CONFIGURATION_SCAN_SUPPORTED_FILES = ('.tf', '.tf.json', '.json', '.yaml', '.yml', 'dockerfile')
 
-SECRET_SCAN_FILE_EXTENSIONS_TO_IGNORE = [
+SECRET_SCAN_FILE_EXTENSIONS_TO_IGNORE = (
     '.7z',
     '.bmp',
     '.bz2',
     '.dmg',
     '.exe',
     '.gif',
     '.gz',
@@ -35,17 +41,17 @@
     '.css',
     '.less',
     '.dll',
     '.enc',
     '.deb',
     '.obj',
     '.model',
-]
+)
 
-SCA_CONFIGURATION_SCAN_SUPPORTED_FILES = [
+SCA_CONFIGURATION_SCAN_SUPPORTED_FILES = (
     'cargo.lock',
     'cargo.toml',
     'composer.json',
     'composer.lock',
     'go.sum',
     'go.mod',
     'gopkg.lock',
@@ -69,17 +75,17 @@
     'build.sbt.lock',
     'pyproject.toml',
     'poetry.lock',
     'pipfile',
     'pipfile.lock',
     'requirements.txt',
     'setup.py',
-]
+)
 
-SCA_EXCLUDED_PATHS = ['node_modules']
+SCA_EXCLUDED_PATHS = ('node_modules',)
 
 PROJECT_FILES_BY_ECOSYSTEM_MAP = {
     'crates': ['Cargo.lock', 'Cargo.toml'],
     'composer': ['composer.json', 'composer.lock'],
     'go': ['go.sum', 'go.mod', 'Gopkg.lock'],
     'maven_pom': ['pom.xml'],
     'maven_gradle': ['build.gradle', 'build.gradle.kts', 'gradle.lockfile'],
```

### Comparing `cycode-0.2.6.dev9/cycode/cli/exceptions/custom_exceptions.py` & `cycode-1.0.0/cycode/cli/exceptions/custom_exceptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,56 +2,56 @@
 
 
 class CycodeError(Exception):
     """Base class for all custom exceptions"""
 
 
 class NetworkError(CycodeError):
-    def __init__(self, status_code: int, error_message: str, response: Response):
+    def __init__(self, status_code: int, error_message: str, response: Response) -> None:
         self.status_code = status_code
         self.error_message = error_message
         self.response = response
         super().__init__(self.error_message)
 
-    def __str__(self):
+    def __str__(self) -> str:
         return (
             f'error occurred during the request. status code: {self.status_code}, error message: '
             f'{self.error_message}'
         )
 
 
 class ScanAsyncError(CycodeError):
-    def __init__(self, error_message: str):
+    def __init__(self, error_message: str) -> None:
         self.error_message = error_message
         super().__init__(self.error_message)
 
-    def __str__(self):
+    def __str__(self) -> str:
         return f'error occurred during the scan. error message: {self.error_message}'
 
 
 class HttpUnauthorizedError(CycodeError):
-    def __init__(self, error_message: str, response: Response):
+    def __init__(self, error_message: str, response: Response) -> None:
         self.status_code = 401
         self.error_message = error_message
         self.response = response
         super().__init__(self.error_message)
 
-    def __str__(self):
+    def __str__(self) -> str:
         return 'Http Unauthorized Error'
 
 
 class ZipTooLargeError(CycodeError):
-    def __init__(self, size_limit: int):
+    def __init__(self, size_limit: int) -> None:
         self.size_limit = size_limit
         super().__init__()
 
-    def __str__(self):
+    def __str__(self) -> str:
         return f'The size of zip to scan is too large, size limit: {self.size_limit}'
 
 
 class AuthProcessError(CycodeError):
-    def __init__(self, error_message: str):
+    def __init__(self, error_message: str) -> None:
         self.error_message = error_message
         super().__init__()
 
-    def __str__(self):
+    def __str__(self) -> str:
         return f'Something went wrong during the authentication process, error message: {self.error_message}'
```

### Comparing `cycode-0.2.6.dev9/cycode/cli/helpers/maven/base_restore_maven_dependencies.py` & `cycode-1.0.0/cycode/cli/helpers/maven/base_restore_maven_dependencies.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from abc import ABC, abstractmethod
-from typing import Dict, List, Optional
+from typing import List, Optional
 
 import click
 
 from cycode.cli.models import Document
 from cycode.cli.utils.path_utils import get_file_dir, join_paths
 from cycode.cli.utils.shell_executor import shell
 from cycode.cyclient import logger
 
 
 def build_dep_tree_path(path: str, generated_file_name: str) -> str:
     return join_paths(get_file_dir(path), generated_file_name)
 
 
-def execute_command(command: List[str], file_name: str, command_timeout: int) -> Optional[Dict]:
+def execute_command(command: List[str], file_name: str, command_timeout: int) -> Optional[str]:
     try:
         dependencies = shell(command, command_timeout)
     except Exception as e:
         logger.debug('Failed to restore dependencies shell comment. %s', {'filename': file_name, 'exception': str(e)})
         return None
 
     return dependencies
 
 
 class BaseRestoreMavenDependencies(ABC):
-    def __init__(self, context: click.Context, is_git_diff: bool, command_timeout: int):
+    def __init__(self, context: click.Context, is_git_diff: bool, command_timeout: int) -> None:
         self.context = context
         self.is_git_diff = is_git_diff
         self.command_timeout = command_timeout
 
     def restore(self, document: Document) -> Optional[Document]:
         return self.try_restore_dependencies(document)
```

### Comparing `cycode-0.2.6.dev9/cycode/cli/helpers/maven/restore_gradle_dependencies.py` & `cycode-1.0.0/cycode/cli/helpers/maven/restore_gradle_dependencies.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 BUILD_GRADLE_FILE_NAME = 'build.gradle'
 BUILD_GRADLE_KTS_FILE_NAME = 'build.gradle.kts'
 BUILD_GRADLE_DEP_TREE_FILE_NAME = 'gradle-dependencies-generated.txt'
 
 
 class RestoreGradleDependencies(BaseRestoreMavenDependencies):
-    def __init__(self, context: click.Context, is_git_diff: bool, command_timeout: int):
+    def __init__(self, context: click.Context, is_git_diff: bool, command_timeout: int) -> None:
         super().__init__(context, is_git_diff, command_timeout)
 
     def is_project(self, document: Document) -> bool:
         return document.path.endswith(BUILD_GRADLE_FILE_NAME) or document.path.endswith(BUILD_GRADLE_KTS_FILE_NAME)
 
     def get_command(self, manifest_file_path: str) -> List[str]:
         return ['gradle', 'dependencies', '-b', manifest_file_path, '-q', '--console', 'plain']
```

### Comparing `cycode-0.2.6.dev9/cycode/cli/helpers/maven/restore_maven_dependencies.py` & `cycode-1.0.0/cycode/cli/helpers/maven/restore_maven_dependencies.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 BUILD_MAVEN_FILE_NAME = 'pom.xml'
 MAVEN_CYCLONE_DEP_TREE_FILE_NAME = 'bom.json'
 MAVEN_DEP_TREE_FILE_NAME = 'bcde.mvndeps'
 
 
 class RestoreMavenDependencies(BaseRestoreMavenDependencies):
-    def __init__(self, context: click.Context, is_git_diff: bool, command_timeout: int):
+    def __init__(self, context: click.Context, is_git_diff: bool, command_timeout: int) -> None:
         super().__init__(context, is_git_diff, command_timeout)
 
     def is_project(self, document: Document) -> bool:
         return path.basename(document.path).split('/')[-1] == BUILD_MAVEN_FILE_NAME
 
     def get_command(self, manifest_file_path: str) -> List[str]:
         return ['mvn', 'org.cyclonedx:cyclonedx-maven-plugin:2.7.4:makeAggregateBom', '-f', manifest_file_path]
@@ -39,30 +39,32 @@
         else:
             restore_dependencies_document.content = get_file_content(
                 join_paths(get_file_dir(manifest_file_path), self.get_lock_file_name())
             )
 
         return restore_dependencies_document
 
-    def restore_from_secondary_command(self, document, manifest_file_path, restore_dependencies_document):
-        # TODO(MarshalX): does it even work? Missing argument
+    def restore_from_secondary_command(
+        self, document: Document, manifest_file_path: str, restore_dependencies_document: Optional[Document]
+    ) -> Optional[Document]:
+        # TODO(MarshalX): does it even work? Ignored restore_dependencies_document arg
         secondary_restore_command = create_secondary_restore_command(manifest_file_path)
         backup_restore_content = execute_command(secondary_restore_command, manifest_file_path, self.command_timeout)
         restore_dependencies_document = Document(
             build_dep_tree_path(document.path, MAVEN_DEP_TREE_FILE_NAME), backup_restore_content, self.is_git_diff
         )
         restore_dependencies = None
         if restore_dependencies_document.content is not None:
             restore_dependencies = restore_dependencies_document
             restore_dependencies.content = get_file_content(MAVEN_DEP_TREE_FILE_NAME)
 
         return restore_dependencies
 
 
-def create_secondary_restore_command(self, manifest_file_path):
+def create_secondary_restore_command(manifest_file_path: str) -> List[str]:
     return [
         'mvn',
         'dependency:tree',
         '-B',
         '-DoutputType=text',
         '-f',
         manifest_file_path,
```

### Comparing `cycode-0.2.6.dev9/cycode/cli/helpers/sca_code_scanner.py` & `cycode-1.0.0/cycode/cli/helpers/sca_code_scanner.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 import os
-from typing import Dict, List, Optional
+from typing import TYPE_CHECKING, Dict, List, Optional
 
 import click
 from git import GitCommandError, Repo
 
 from cycode.cli import consts
 from cycode.cli.helpers.maven.restore_gradle_dependencies import RestoreGradleDependencies
 from cycode.cli.helpers.maven.restore_maven_dependencies import RestoreMavenDependencies
 from cycode.cli.models import Document
 from cycode.cli.utils.path_utils import get_file_content, get_file_dir, join_paths
 from cycode.cyclient import logger
 
+if TYPE_CHECKING:
+    from cycode.cli.helpers.maven.base_restore_maven_dependencies import BaseRestoreMavenDependencies
+
 BUILD_GRADLE_FILE_NAME = 'build.gradle'
 BUILD_GRADLE_KTS_FILE_NAME = 'build.gradle.kts'
 BUILD_GRADLE_DEP_TREE_FILE_NAME = 'gradle-dependencies-generated.txt'
 BUILD_GRADLE_DEP_TREE_TIMEOUT = 180
 
 
 def perform_pre_commit_range_scan_actions(
@@ -35,36 +38,38 @@
     repo = Repo(os.getcwd())
     add_ecosystem_related_files_if_exists(git_head_documents, repo, consts.GIT_HEAD_COMMIT_REV)
     add_ecosystem_related_files_if_exists(pre_committed_documents)
 
 
 def add_ecosystem_related_files_if_exists(
     documents: List[Document], repo: Optional[Repo] = None, commit_rev: Optional[str] = None
-):
+) -> None:
+    documents_to_add: List[Document] = []
     for doc in documents:
         ecosystem = get_project_file_ecosystem(doc)
         if ecosystem is None:
             logger.debug('failed to resolve project file ecosystem: %s', doc.path)
             continue
-        documents_to_add = get_doc_ecosystem_related_project_files(doc, documents, ecosystem, commit_rev, repo)
-        documents.extend(documents_to_add)
+
+        documents_to_add.extend(get_doc_ecosystem_related_project_files(doc, documents, ecosystem, commit_rev, repo))
+
+    documents.extend(documents_to_add)
 
 
 def get_doc_ecosystem_related_project_files(
     doc: Document, documents: List[Document], ecosystem: str, commit_rev: Optional[str], repo: Optional[Repo]
 ) -> List[Document]:
     documents_to_add: List[Document] = []
     for ecosystem_project_file in consts.PROJECT_FILES_BY_ECOSYSTEM_MAP.get(ecosystem):
         file_to_search = join_paths(get_file_dir(doc.path), ecosystem_project_file)
         if not is_project_file_exists_in_documents(documents, file_to_search):
-            file_content = (
-                get_file_content_from_commit(repo, commit_rev, file_to_search)
-                if repo
-                else get_file_content(file_to_search)
-            )
+            if repo:
+                file_content = get_file_content_from_commit(repo, commit_rev, file_to_search)
+            else:
+                file_content = get_file_content(file_to_search)
 
             if file_content is not None:
                 documents_to_add.append(Document(file_to_search, file_content))
 
     return documents_to_add
 
 
@@ -77,16 +82,19 @@
         for project_file in project_files:
             if document.path.endswith(project_file):
                 return ecosystem
     return None
 
 
 def try_restore_dependencies(
-    context: click.Context, documents_to_add: List[Document], restore_dependencies, document: Document
-):
+    context: click.Context,
+    documents_to_add: Dict[str, Document],
+    restore_dependencies: 'BaseRestoreMavenDependencies',
+    document: Document,
+) -> None:
     if restore_dependencies.is_project(document):
         restore_dependencies_document = restore_dependencies.restore(document)
         if restore_dependencies_document is None:
             logger.warning('Error occurred while trying to generate dependencies tree. %s', {'filename': document.path})
             return
 
         if restore_dependencies_document.content is None:
@@ -113,15 +121,15 @@
     for restore_dependencies in restore_dependencies_list:
         for document in documents_to_scan:
             try_restore_dependencies(context, documents_to_add, restore_dependencies, document)
 
     documents_to_scan.extend(list(documents_to_add.values()))
 
 
-def restore_handlers(context, is_git_diff):
+def restore_handlers(context: click.Context, is_git_diff: bool) -> List[RestoreGradleDependencies]:
     return [
         RestoreGradleDependencies(context, is_git_diff, BUILD_GRADLE_DEP_TREE_TIMEOUT),
         RestoreMavenDependencies(context, is_git_diff, BUILD_GRADLE_DEP_TREE_TIMEOUT),
     ]
 
 
 def get_manifest_file_path(document: Document, is_monitor_action: bool, project_path: str) -> str:
```

### Comparing `cycode-0.2.6.dev9/cycode/cli/main.py` & `cycode-1.0.0/cycode/cli/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
+import json
 import logging
 import sys
-from typing import TYPE_CHECKING, List, Optional
+from typing import TYPE_CHECKING, List, Optional, Tuple
 
 import click
 
 from cycode import __version__
 from cycode.cli import code_scanner
 from cycode.cli.auth.auth_command import authenticate
 from cycode.cli.config import config
-from cycode.cli.consts import ISSUE_DETECTED_STATUS_CODE, NO_ISSUES_STATUS_CODE
+from cycode.cli.consts import CLI_CONTEXT_SETTINGS, ISSUE_DETECTED_STATUS_CODE, NO_ISSUES_STATUS_CODE, PROGRAM_NAME
 from cycode.cli.models import Severity
 from cycode.cli.user_settings.configuration_manager import ConfigurationManager
 from cycode.cli.user_settings.credentials_manager import CredentialsManager
 from cycode.cli.user_settings.user_settings_commands import add_exclusions, set_credentials
 from cycode.cli.utils import scan_utils
 from cycode.cli.utils.progress_bar import get_progress_bar
 from cycode.cli.utils.progress_bar import logger as progress_bar_logger
@@ -20,242 +21,237 @@
 from cycode.cyclient.cycode_client_base import CycodeClientBase
 from cycode.cyclient.models import UserAgentOptionScheme
 from cycode.cyclient.scan_config.scan_config_creator import create_scan_client
 
 if TYPE_CHECKING:
     from cycode.cyclient.scan_client import ScanClient
 
-CONTEXT = {}
-
 
 @click.group(
     commands={
         'repository': code_scanner.scan_repository,
         'commit_history': code_scanner.scan_repository_commit_history,
         'path': code_scanner.scan_path,
         'pre_commit': code_scanner.pre_commit_scan,
         'pre_receive': code_scanner.pre_receive_scan,
     },
-    short_help='Scan content for secrets/IaC/sca/SAST violations. '
-    'You need to specify which scan type: ci/commit_history/path/repository/etc',
+    short_help='Scan the content for Secrets/IaC/SCA/SAST violations. '
+    'You`ll need to specify which scan type to perform: ci/commit_history/path/repository/etc.',
 )
 @click.option(
     '--scan-type',
     '-t',
     default='secret',
-    help="""
-              \b
-              Specify the scan you wish to execute (secret/iac/sca),
-              the default is secret
-              """,
+    help='Specify the type of scan you wish to execute (the default is Secrets)',
     type=click.Choice(config['scans']['supported_scans']),
 )
 @click.option(
     '--secret',
     default=None,
-    help='Specify a Cycode client secret for this specific scan execution',
+    help='Specify a Cycode client secret for this specific scan execution.',
     type=str,
     required=False,
 )
 @click.option(
     '--client-id',
     default=None,
-    help='Specify a Cycode client ID for this specific scan execution',
+    help='Specify a Cycode client ID for this specific scan execution.',
     type=str,
     required=False,
 )
 @click.option(
-    '--show-secret', is_flag=True, default=False, help='Show secrets in plain text', type=bool, required=False
+    '--show-secret', is_flag=True, default=False, help='Show Secrets in plain text.', type=bool, required=False
 )
 @click.option(
     '--soft-fail',
     is_flag=True,
     default=False,
-    help='Run scan without failing, always return a non-error status code',
+    help='Run the scan without failing; always return a non-error status code.',
     type=bool,
     required=False,
 )
 @click.option(
-    '--output',
-    default=None,
-    help="""
-              \b
-              Specify the results output (text/json/table),
-              the default is text
-              """,
-    type=click.Choice(['text', 'json', 'table']),
-)
-@click.option(
     '--severity-threshold',
     default=None,
-    help='Show only violations at the specified level or higher (supported for SCA scan type only).',
+    help='Show violations only for the specified level or higher (supported for SCA scan types only).',
     type=click.Choice([e.name for e in Severity]),
     required=False,
 )
 @click.option(
     '--sca-scan',
     default=None,
-    help='Specify the sca scan you wish to execute (package-vulnerabilities/license-compliance), the default is both',
+    help='Specify the type of SCA scan you wish to execute (the default is both).',
     multiple=True,
     type=click.Choice(config['scans']['supported_sca_scans']),
 )
 @click.option(
     '--monitor',
     is_flag=True,
     default=False,
-    help="When specified, the scan results will be recorded in the knowledge graph. "
-    "Please note that when working in 'monitor' mode, the knowledge graph "
-    "will not be updated as a result of SCM events (Push, Repo creation).(supported for SCA scan type only).",
+    help='Used for SCA scan types only; when specified, the scan results are recorded in the Discovery module.',
     type=bool,
     required=False,
 )
 @click.option(
     '--report',
     is_flag=True,
     default=False,
-    help='When specified, a violations report will be generated. '
-    'A URL link to the report will be printed as an output to the command execution',
+    help='When specified, generates a violations report. A link to the report will be displayed in the console output.',
     type=bool,
     required=False,
 )
 @click.pass_context
 def code_scan(
     context: click.Context,
-    scan_type,
-    client_id,
-    secret,
-    show_secret,
-    soft_fail,
-    output,
-    severity_threshold,
+    scan_type: str,
+    secret: str,
+    client_id: str,
+    show_secret: bool,
+    soft_fail: bool,
+    severity_threshold: str,
     sca_scan: List[str],
-    monitor,
-    report,
-):
+    monitor: bool,
+    report: bool,
+) -> int:
+    """Scans for Secrets, IaC, SCA or SAST violations."""
     if show_secret:
         context.obj['show_secret'] = show_secret
     else:
         context.obj['show_secret'] = config['result_printer']['default']['show_secret']
 
     if soft_fail:
         context.obj['soft_fail'] = soft_fail
     else:
         context.obj['soft_fail'] = config['soft_fail']
 
+    context.obj['client'] = get_cycode_client(client_id, secret, not context.obj['show_secret'])
     context.obj['scan_type'] = scan_type
-
-    # save backward compatability with old style command
-    if output is not None:
-        context.obj['output'] = output
-        if output == 'json':
-            context.obj['no_progress_meter'] = True
-
-    context.obj['client'] = get_cycode_client(client_id, secret)
     context.obj['severity_threshold'] = severity_threshold
     context.obj['monitor'] = monitor
     context.obj['report'] = report
 
     _sca_scan_to_context(context, sca_scan)
 
-    context.obj['progress_bar'] = get_progress_bar(hidden=context.obj['no_progress_meter'])
-    context.obj['progress_bar'].start()
-
     return 1
 
 
 @code_scan.result_callback()
 @click.pass_context
-def finalize(context: click.Context, *_, **__):
+def finalize(context: click.Context, *_, **__) -> None:
     progress_bar = context.obj.get('progress_bar')
     if progress_bar:
         progress_bar.stop()
 
     if context.obj['soft_fail']:
         sys.exit(0)
 
     exit_code = NO_ISSUES_STATUS_CODE
     if _should_fail_scan(context):
         exit_code = ISSUE_DETECTED_STATUS_CODE
 
     sys.exit(exit_code)
 
 
+@click.command(short_help='Show the CLI version and exit.')
+@click.pass_context
+def version(context: click.Context) -> None:
+    output = context.obj['output']
+
+    prog = PROGRAM_NAME
+    ver = __version__
+
+    message = f'{prog}, version {ver}'
+    if output == 'json':
+        message = json.dumps({'name': prog, 'version': ver})
+
+    click.echo(message, color=context.color)
+    context.exit()
+
+
 @click.group(
-    commands={'scan': code_scan, 'configure': set_credentials, 'ignore': add_exclusions, 'auth': authenticate},
-    context_settings=CONTEXT,
+    commands={
+        'scan': code_scan,
+        'configure': set_credentials,
+        'ignore': add_exclusions,
+        'auth': authenticate,
+        'version': version,
+    },
+    context_settings=CLI_CONTEXT_SETTINGS,
 )
 @click.option(
     '--verbose',
     '-v',
     is_flag=True,
     default=False,
-    help='Show detailed logs',
+    help='Show detailed logs.',
 )
 @click.option(
     '--no-progress-meter',
     is_flag=True,
     default=False,
-    help='Do not show the progress meter',
+    help='Do not show the progress meter.',
 )
 @click.option(
     '--output',
+    '-o',
     default='text',
-    help='Specify the output (text/json/table), the default is text',
+    help='Specify the output type (the default is text).',
     type=click.Choice(['text', 'json', 'table']),
 )
 @click.option(
     '--user-agent',
     default=None,
-    help='Characteristic JSON object that lets servers identify the application',
+    help='Characteristic JSON object that lets servers identify the application.',
     type=str,
 )
-@click.version_option(__version__, prog_name='cycode')
 @click.pass_context
-def main_cli(context: click.Context, verbose: bool, no_progress_meter: bool, output: str, user_agent: Optional[str]):
+def main_cli(
+    context: click.Context, verbose: bool, no_progress_meter: bool, output: str, user_agent: Optional[str]
+) -> None:
     context.ensure_object(dict)
     configuration_manager = ConfigurationManager()
 
     verbose = verbose or configuration_manager.get_verbose_flag()
     context.obj['verbose'] = verbose
     # TODO(MarshalX): rework setting the log level for loggers
     log_level = logging.DEBUG if verbose else logging.INFO
     logger.setLevel(log_level)
     progress_bar_logger.setLevel(log_level)
 
     context.obj['output'] = output
     if output == 'json':
         no_progress_meter = True
 
-    context.obj['no_progress_meter'] = no_progress_meter
+    context.obj['progress_bar'] = get_progress_bar(hidden=no_progress_meter)
 
     if user_agent:
         user_agent_option = UserAgentOptionScheme().loads(user_agent)
         CycodeClientBase.enrich_user_agent(user_agent_option.user_agent_suffix)
 
 
-def get_cycode_client(client_id: str, client_secret: str) -> 'ScanClient':
+def get_cycode_client(client_id: str, client_secret: str, hide_response_log: bool) -> 'ScanClient':
     if not client_id or not client_secret:
         client_id, client_secret = _get_configured_credentials()
         if not client_id:
             raise click.ClickException('Cycode client id needed.')
         if not client_secret:
             raise click.ClickException('Cycode client secret is needed.')
 
-    return create_scan_client(client_id, client_secret)
+    return create_scan_client(client_id, client_secret, hide_response_log)
 
 
-def _get_configured_credentials():
+def _get_configured_credentials() -> Tuple[str, str]:
     credentials_manager = CredentialsManager()
     return credentials_manager.get_credentials()
 
 
-def _should_fail_scan(context: click.Context):
+def _should_fail_scan(context: click.Context) -> bool:
     return scan_utils.is_scan_failed(context)
 
 
-def _sca_scan_to_context(context: click.Context, sca_scan_user_selected: List[str]):
+def _sca_scan_to_context(context: click.Context, sca_scan_user_selected: List[str]) -> None:
     for sca_scan_option_selected in sca_scan_user_selected:
         context.obj[sca_scan_option_selected] = True
 
 
 if __name__ == '__main__':
     main_cli()
```

### Comparing `cycode-0.2.6.dev9/cycode/cli/models.py` & `cycode-1.0.0/cycode/cli/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from enum import Enum
 from typing import Dict, List, NamedTuple, Optional, Type
 
 from cycode.cyclient.models import Detection
 
 
 class Document:
-    def __init__(self, path: str, content: str, is_git_diff_format: bool = False, unique_id: Optional[str] = None):
+    def __init__(
+        self, path: str, content: str, is_git_diff_format: bool = False, unique_id: Optional[str] = None
+    ) -> None:
         self.path = path
         self.content = content
         self.is_git_diff_format = is_git_diff_format
         self.unique_id = unique_id
 
     def __repr__(self) -> str:
         return 'path:{0}, content:{1}'.format(self.path, self.content)
 
 
 class DocumentDetections:
-    def __init__(self, document: Document, detections: List[Detection]):
+    def __init__(self, document: Document, detections: List[Detection]) -> None:
         self.document = document
         self.detections = detections
 
     def __repr__(self) -> str:
         return 'document:{0}, detections:{1}'.format(self.document, self.detections)
```

### Comparing `cycode-0.2.6.dev9/cycode/cli/printers/base_printer.py` & `cycode-1.0.0/cycode/cli/printers/printer_base.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 from abc import ABC, abstractmethod
-from typing import TYPE_CHECKING, List
+from typing import TYPE_CHECKING, Dict, List, Optional
 
 import click
 
 from cycode.cli.models import CliError, CliResult
 
 if TYPE_CHECKING:
     from cycode.cli.models import LocalScanResult
 
 
-class BasePrinter(ABC):
+class PrinterBase(ABC):
     RED_COLOR_NAME = 'red'
     WHITE_COLOR_NAME = 'white'
     GREEN_COLOR_NAME = 'green'
 
-    def __init__(self, context: click.Context):
+    def __init__(self, context: click.Context) -> None:
         self.context = context
 
     @abstractmethod
-    def print_scan_results(self, local_scan_results: List['LocalScanResult']) -> None:
+    def print_scan_results(
+        self, local_scan_results: List['LocalScanResult'], errors: Optional[Dict[str, 'CliError']] = None
+    ) -> None:
         pass
 
     @abstractmethod
     def print_result(self, result: CliResult) -> None:
         pass
 
     @abstractmethod
```

### Comparing `cycode-0.2.6.dev9/cycode/cli/printers/console_printer.py` & `cycode-1.0.0/cycode/cli/printers/console_printer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,49 @@
-from typing import TYPE_CHECKING, ClassVar, Dict, List
+from typing import TYPE_CHECKING, ClassVar, Dict, List, Optional
 
 import click
 
 from cycode.cli.exceptions.custom_exceptions import CycodeError
 from cycode.cli.models import CliError, CliResult
 from cycode.cli.printers.json_printer import JsonPrinter
-from cycode.cli.printers.sca_table_printer import SCATablePrinter
-from cycode.cli.printers.table_printer import TablePrinter
+from cycode.cli.printers.tables.sca_table_printer import ScaTablePrinter
+from cycode.cli.printers.tables.table_printer import TablePrinter
 from cycode.cli.printers.text_printer import TextPrinter
 
 if TYPE_CHECKING:
     from cycode.cli.models import LocalScanResult
-    from cycode.cli.printers.base_printer import BasePrinter
+    from cycode.cli.printers.tables.table_printer_base import PrinterBase
 
 
 class ConsolePrinter:
-    _AVAILABLE_PRINTERS: ClassVar[Dict[str, 'BasePrinter']] = {
+    _AVAILABLE_PRINTERS: ClassVar[Dict[str, 'PrinterBase']] = {
         'text': TextPrinter,
         'json': JsonPrinter,
         'table': TablePrinter,
         # overrides
-        'table_sca': SCATablePrinter,
-        'text_sca': SCATablePrinter,
+        'table_sca': ScaTablePrinter,
+        'text_sca': ScaTablePrinter,
     }
 
-    def __init__(self, context: click.Context):
+    def __init__(self, context: click.Context) -> None:
         self.context = context
         self.scan_type = self.context.obj.get('scan_type')
         self.output_type = self.context.obj.get('output')
 
         self._printer_class = self._AVAILABLE_PRINTERS.get(self.output_type)
         if self._printer_class is None:
             raise CycodeError(f'"{self.output_type}" output type is not supported.')
 
-    def print_scan_results(self, local_scan_results: List['LocalScanResult']) -> None:
+    def print_scan_results(
+        self, local_scan_results: List['LocalScanResult'], errors: Optional[Dict[str, 'CliError']] = None
+    ) -> None:
         printer = self._get_scan_printer()
-        printer.print_scan_results(local_scan_results)
+        printer.print_scan_results(local_scan_results, errors)
 
-    def _get_scan_printer(self) -> 'BasePrinter':
+    def _get_scan_printer(self) -> 'PrinterBase':
         printer_class = self._printer_class
 
         composite_printer = self._AVAILABLE_PRINTERS.get(f'{self.output_type}_{self.scan_type}')
         if composite_printer:
             printer_class = composite_printer
 
         return printer_class(self.context)
```

### Comparing `cycode-0.2.6.dev9/cycode/cli/printers/json_printer.py` & `cycode-1.0.0/cycode/cli/printers/json_printer.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,45 +1,53 @@
 import json
-from typing import TYPE_CHECKING, List
+from typing import TYPE_CHECKING, Dict, List, Optional
 
 import click
 
 from cycode.cli.models import CliError, CliResult
-from cycode.cli.printers.base_printer import BasePrinter
+from cycode.cli.printers.printer_base import PrinterBase
 from cycode.cyclient.models import DetectionSchema
 
 if TYPE_CHECKING:
     from cycode.cli.models import LocalScanResult
 
 
-class JsonPrinter(BasePrinter):
+class JsonPrinter(PrinterBase):
     def print_result(self, result: CliResult) -> None:
         result = {'result': result.success, 'message': result.message}
 
-        click.secho(self.get_data_json(result))
+        click.echo(self.get_data_json(result))
 
     def print_error(self, error: CliError) -> None:
         result = {'error': error.code, 'message': error.message}
 
-        click.secho(self.get_data_json(result))
+        click.echo(self.get_data_json(result))
 
-    def print_scan_results(self, local_scan_results: List['LocalScanResult']) -> None:
+    def print_scan_results(
+        self, local_scan_results: List['LocalScanResult'], errors: Optional[Dict[str, 'CliError']] = None
+    ) -> None:
         detections = []
         for local_scan_result in local_scan_results:
             for document_detections in local_scan_result.document_detections:
                 detections.extend(document_detections.detections)
 
         detections_dict = DetectionSchema(many=True).dump(detections)
 
-        click.secho(self._get_json_scan_result(detections_dict))
+        inlined_errors = []
+        if errors:
+            # FIXME(MarshalX): we don't care about scan IDs in JSON output due to clumsy JSON root structure
+            inlined_errors = [err._asdict() for err in errors.values()]
 
-    def _get_json_scan_result(self, detections: dict) -> str:
+        click.echo(self._get_json_scan_result(detections_dict, inlined_errors))
+
+    def _get_json_scan_result(self, detections: dict, errors: List[dict]) -> str:
         result = {
             'scan_id': 'DEPRECATED',  # FIXME(MarshalX): we need change JSON struct to support multiple scan results
             'detections': detections,
+            'errors': errors,
         }
 
         return self.get_data_json(result)
 
     @staticmethod
     def get_data_json(data: dict) -> str:
         # ensure_ascii is disabled for symbols like "`". Eg: `cycode scan`
```

### Comparing `cycode-0.2.6.dev9/cycode/cli/printers/sca_table_printer.py` & `cycode-1.0.0/cycode/cli/printers/tables/table_printer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,154 +1,134 @@
-from collections import defaultdict
-from typing import TYPE_CHECKING, Dict, List
+from typing import TYPE_CHECKING, List
 
 import click
-from texttable import Texttable
 
-from cycode.cli.consts import LICENSE_COMPLIANCE_POLICY_ID, PACKAGE_VULNERABILITY_POLICY_ID
-from cycode.cli.models import Detection
-from cycode.cli.printers.base_table_printer import BaseTablePrinter
-from cycode.cli.utils.string_utils import shortcut_dependency_paths
+from cycode.cli.consts import INFRA_CONFIGURATION_SCAN_TYPE, SAST_SCAN_TYPE, SECRET_SCAN_TYPE
+from cycode.cli.models import Detection, Document
+from cycode.cli.printers.tables.table import Table
+from cycode.cli.printers.tables.table_models import ColumnInfoBuilder, ColumnWidthsConfig
+from cycode.cli.printers.tables.table_printer_base import TablePrinterBase
+from cycode.cli.utils.string_utils import get_position_in_line, obfuscate_text
 
 if TYPE_CHECKING:
     from cycode.cli.models import LocalScanResult
 
-SEVERITY_COLUMN = 'Severity'
-LICENSE_COLUMN = 'License'
-UPGRADE_COLUMN = 'Upgrade'
-REPOSITORY_COLUMN = 'Repository'
-CVE_COLUMN = 'CVE'
-
-PREVIEW_DETECTIONS_COMMON_HEADERS = [
-    'File Path',
-    'Ecosystem',
-    'Dependency Name',
-    'Direct Dependency',
-    'Development Dependency',
-    'Dependency Paths',
-]
+column_builder = ColumnInfoBuilder()
 
+# Building must have strict order. Represents the order of the columns in the table (from left to right)
+ISSUE_TYPE_COLUMN = column_builder.build(name='Issue Type')
+RULE_ID_COLUMN = column_builder.build(name='Rule ID')
+FILE_PATH_COLUMN = column_builder.build(name='File Path')
+SECRET_SHA_COLUMN = column_builder.build(name='Secret SHA')
+COMMIT_SHA_COLUMN = column_builder.build(name='Commit SHA')
+LINE_NUMBER_COLUMN = column_builder.build(name='Line Number')
+COLUMN_NUMBER_COLUMN = column_builder.build(name='Column Number')
+VIOLATION_LENGTH_COLUMN = column_builder.build(name='Violation Length')
+VIOLATION_COLUMN = column_builder.build(name='Violation')
+SCAN_ID_COLUMN = column_builder.build(name='Scan ID')
+REPORT_URL_COLUMN = column_builder.build(name='Report URL')
+
+COLUMN_WIDTHS_CONFIG: ColumnWidthsConfig = {
+    SECRET_SCAN_TYPE: {
+        ISSUE_TYPE_COLUMN: 2,
+        RULE_ID_COLUMN: 2,
+        FILE_PATH_COLUMN: 2,
+        SECRET_SHA_COLUMN: 2,
+        VIOLATION_COLUMN: 2,
+        SCAN_ID_COLUMN: 2,
+    },
+    INFRA_CONFIGURATION_SCAN_TYPE: {
+        ISSUE_TYPE_COLUMN: 4,
+        RULE_ID_COLUMN: 3,
+        FILE_PATH_COLUMN: 3,
+        SCAN_ID_COLUMN: 2,
+    },
+    SAST_SCAN_TYPE: {
+        ISSUE_TYPE_COLUMN: 7,
+        RULE_ID_COLUMN: 2,
+        FILE_PATH_COLUMN: 3,
+        SCAN_ID_COLUMN: 2,
+    },
+}
 
-class SCATablePrinter(BaseTablePrinter):
-    def _print_results(self, local_scan_results: List['LocalScanResult']) -> None:
-        detections_per_detection_type_id = self._extract_detections_per_detection_type_id(local_scan_results)
-        self._print_detection_per_detection_type_id(detections_per_detection_type_id)
 
-    @staticmethod
-    def _extract_detections_per_detection_type_id(
-        local_scan_results: List['LocalScanResult'],
-    ) -> Dict[str, List[Detection]]:
-        detections_per_detection_type_id = defaultdict(list)
+class TablePrinter(TablePrinterBase):
+    def _print_results(self, local_scan_results: List['LocalScanResult']) -> None:
+        table = self._get_table()
+        if self.scan_type in COLUMN_WIDTHS_CONFIG:
+            table.set_cols_width(COLUMN_WIDTHS_CONFIG[self.scan_type])
 
         for local_scan_result in local_scan_results:
-            for document_detection in local_scan_result.document_detections:
-                for detection in document_detection.detections:
-                    detections_per_detection_type_id[detection.detection_type_id].append(detection)
-
-        return detections_per_detection_type_id
-
-    def _print_detection_per_detection_type_id(
-        self, detections_per_detection_type_id: Dict[str, List[Detection]]
-    ) -> None:
-        for detection_type_id in detections_per_detection_type_id:
-            detections = detections_per_detection_type_id[detection_type_id]
-            headers = self._get_table_headers()
-
-            title = None
-            rows = []
-
-            if detection_type_id == PACKAGE_VULNERABILITY_POLICY_ID:
-                title = 'Dependencies Vulnerabilities'
-
-                headers = [SEVERITY_COLUMN, *headers]
-                headers.extend(PREVIEW_DETECTIONS_COMMON_HEADERS)
-                headers.append(CVE_COLUMN)
-                headers.append(UPGRADE_COLUMN)
+            for document_detections in local_scan_result.document_detections:
+                report_url = local_scan_result.report_url if local_scan_result.report_url else 'N/A'
+                for detection in document_detections.detections:
+                    table.set(REPORT_URL_COLUMN, report_url)
+                    table.set(SCAN_ID_COLUMN, local_scan_result.scan_id)
+                    self._enrich_table_with_values(table, detection, document_detections.document)
+
+        self._print_table(table)
+
+    def _get_table(self) -> Table:
+        table = Table()
+
+        table.add(ISSUE_TYPE_COLUMN)
+        table.add(RULE_ID_COLUMN)
+        table.add(FILE_PATH_COLUMN)
+        table.add(LINE_NUMBER_COLUMN)
+        table.add(COLUMN_NUMBER_COLUMN)
+        table.add(SCAN_ID_COLUMN)
 
-                for detection in detections:
-                    rows.append(self._get_upgrade_package_vulnerability(detection))
-            elif detection_type_id == LICENSE_COMPLIANCE_POLICY_ID:
-                title = 'License Compliance'
-
-                headers.extend(PREVIEW_DETECTIONS_COMMON_HEADERS)
-                headers.append(LICENSE_COLUMN)
-
-                for detection in detections:
-                    rows.append(self._get_license(detection))
+        if self._is_git_repository():
+            table.add(COMMIT_SHA_COLUMN)
 
-            if rows:
-                self._print_table_detections(detections, headers, rows, title)
+        if self.scan_type == SECRET_SCAN_TYPE:
+            table.add(SECRET_SHA_COLUMN)
+            table.add(VIOLATION_LENGTH_COLUMN)
+            table.add(VIOLATION_COLUMN)
 
-    def _get_table_headers(self) -> list:
-        if self._is_git_repository():
-            return [REPOSITORY_COLUMN]
+        if self.context.obj.get('report'):
+            table.add(REPORT_URL_COLUMN)
 
-        return []
+        return table
 
-    def _print_table_detections(self, detections: List[Detection], headers: List[str], rows, title: str) -> None:
-        self._print_summary_issues(detections, title)
-        text_table = Texttable()
-        text_table.header(headers)
-
-        self.set_table_width(headers, text_table)
-
-        for row in rows:
-            text_table.add_row(row)
-
-        click.echo(text_table.draw())
-
-    @staticmethod
-    def set_table_width(headers: List[str], text_table: Texttable) -> None:
-        header_width_size_cols = []
-        for header in headers:
-            header_len = len(header)
-            if header == CVE_COLUMN:
-                header_width_size_cols.append(header_len * 5)
-            elif header == UPGRADE_COLUMN:
-                header_width_size_cols.append(header_len * 2)
-            else:
-                header_width_size_cols.append(header_len)
-        text_table.set_cols_width(header_width_size_cols)
-
-    @staticmethod
-    def _print_summary_issues(detections: List, title: str) -> None:
-        click.echo(f'⛔ Found {len(detections)} issues of type: {click.style(title, bold=True)}')
-
-    def _get_common_detection_fields(self, detection: Detection) -> List[str]:
-        dependency_paths = 'N/A'
-        dependency_paths_raw = detection.detection_details.get('dependency_paths')
-        if dependency_paths_raw:
-            dependency_paths = shortcut_dependency_paths(dependency_paths_raw)
-
-        row = [
-            detection.detection_details.get('file_name'),
-            detection.detection_details.get('ecosystem'),
-            detection.detection_details.get('package_name'),
-            detection.detection_details.get('is_direct_dependency_str'),
-            detection.detection_details.get('is_dev_dependency_str'),
-            dependency_paths,
-        ]
+    def _enrich_table_with_values(self, table: Table, detection: Detection, document: Document) -> None:
+        self._enrich_table_with_detection_summary_values(table, detection, document)
+        self._enrich_table_with_detection_code_segment_values(table, detection, document)
 
-        if self._is_git_repository():
-            row = [detection.detection_details.get('repository_name'), *row]
+    def _enrich_table_with_detection_summary_values(
+        self, table: Table, detection: Detection, document: Document
+    ) -> None:
+        issue_type = detection.message
+        if self.scan_type == SECRET_SCAN_TYPE:
+            issue_type = detection.type
+
+        table.set(ISSUE_TYPE_COLUMN, issue_type)
+        table.set(RULE_ID_COLUMN, detection.detection_rule_id)
+        table.set(FILE_PATH_COLUMN, click.format_filename(document.path))
+        table.set(SECRET_SHA_COLUMN, detection.detection_details.get('sha512', ''))
+        table.set(COMMIT_SHA_COLUMN, detection.detection_details.get('commit_id', ''))
 
-        return row
+    def _enrich_table_with_detection_code_segment_values(
+        self, table: Table, detection: Detection, document: Document
+    ) -> None:
+        detection_details = detection.detection_details
 
-    def _get_upgrade_package_vulnerability(self, detection: Detection) -> List[str]:
-        alert = detection.detection_details.get('alert')
-        row = [
-            detection.detection_details.get('advisory_severity'),
-            *self._get_common_detection_fields(detection),
-            detection.detection_details.get('vulnerability_id'),
-        ]
-
-        upgrade = ''
-        if alert.get('first_patched_version'):
-            upgrade = f'{alert.get("vulnerable_requirements")} -> {alert.get("first_patched_version")}'
-        row.append(upgrade)
-
-        return row
-
-    def _get_license(self, detection: Detection) -> List[str]:
-        row = self._get_common_detection_fields(detection)
-        row.append(f'{detection.detection_details.get("license")}')
-        return row
+        detection_line = detection_details.get('line_in_file', -1)
+        if self.scan_type == SECRET_SCAN_TYPE:
+            detection_line = detection_details.get('line', -1)
+
+        detection_column = get_position_in_line(document.content, detection_details.get('start_position', -1))
+        violation_length = detection_details.get('length', -1)
+
+        violation = ''
+        file_content_lines = document.content.splitlines()
+        if detection_line < len(file_content_lines):
+            line = file_content_lines[detection_line]
+            violation = line[detection_column : detection_column + violation_length]
+
+            if not self.show_secret:
+                violation = obfuscate_text(violation)
+
+        table.set(LINE_NUMBER_COLUMN, str(detection_line))
+        table.set(COLUMN_NUMBER_COLUMN, str(detection_column))
+        table.set(VIOLATION_LENGTH_COLUMN, f'{violation_length} chars')
+        table.set(VIOLATION_COLUMN, violation)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `cycode-0.2.6.dev9/cycode/cli/printers/table.py` & `cycode-1.0.0/cycode/cli/printers/tables/table.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from typing import TYPE_CHECKING, Dict, List, Optional
 
 from texttable import Texttable
 
 if TYPE_CHECKING:
-    from cycode.cli.printers.table_models import ColumnInfo, ColumnWidths
+    from cycode.cli.printers.tables.table_models import ColumnInfo, ColumnWidths
 
 
 class Table:
     """Helper class to manage columns and their values in the right order and only if the column should be presented."""
 
-    def __init__(self, column_infos: Optional[List['ColumnInfo']] = None):
+    def __init__(self, column_infos: Optional[List['ColumnInfo']] = None) -> None:
         self._column_widths = None
 
         self._columns: Dict['ColumnInfo', List[str]] = {}
         if column_infos:
             self._columns: Dict['ColumnInfo', List[str]] = {columns: [] for columns in column_infos}
 
     def add(self, column: 'ColumnInfo') -> None:
```

### Comparing `cycode-0.2.6.dev9/cycode/cli/printers/table_printer.py` & `cycode-1.0.0/cycode/cli/printers/tables/sca_table_printer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,130 +1,143 @@
-from typing import TYPE_CHECKING, List
+from collections import defaultdict
+from typing import TYPE_CHECKING, Dict, List
 
 import click
 
-from cycode.cli.consts import INFRA_CONFIGURATION_SCAN_TYPE, SAST_SCAN_TYPE, SECRET_SCAN_TYPE
-from cycode.cli.models import Detection, Document
-from cycode.cli.printers.base_table_printer import BaseTablePrinter
-from cycode.cli.printers.table import Table
-from cycode.cli.printers.table_models import ColumnInfoBuilder, ColumnWidthsConfig
-from cycode.cli.utils.string_utils import get_position_in_line, obfuscate_text
+from cycode.cli.consts import LICENSE_COMPLIANCE_POLICY_ID, PACKAGE_VULNERABILITY_POLICY_ID
+from cycode.cli.models import Detection
+from cycode.cli.printers.tables.table import Table
+from cycode.cli.printers.tables.table_models import ColumnInfoBuilder, ColumnWidths
+from cycode.cli.printers.tables.table_printer_base import TablePrinterBase
+from cycode.cli.utils.string_utils import shortcut_dependency_paths
 
 if TYPE_CHECKING:
     from cycode.cli.models import LocalScanResult
 
-# Creation must have strict order. Represents the order of the columns in the table (from left to right)
-ISSUE_TYPE_COLUMN = ColumnInfoBuilder.build(name='Issue Type')
-RULE_ID_COLUMN = ColumnInfoBuilder.build(name='Rule ID')
-FILE_PATH_COLUMN = ColumnInfoBuilder.build(name='File Path')
-SECRET_SHA_COLUMN = ColumnInfoBuilder.build(name='Secret SHA')
-COMMIT_SHA_COLUMN = ColumnInfoBuilder.build(name='Commit SHA')
-LINE_NUMBER_COLUMN = ColumnInfoBuilder.build(name='Line Number')
-COLUMN_NUMBER_COLUMN = ColumnInfoBuilder.build(name='Column Number')
-VIOLATION_LENGTH_COLUMN = ColumnInfoBuilder.build(name='Violation Length')
-VIOLATION_COLUMN = ColumnInfoBuilder.build(name='Violation')
-SCAN_ID_COLUMN = ColumnInfoBuilder.build(name='Scan ID')
-REPORT_URL_COLUMN = ColumnInfoBuilder.build(name='Report URL')
-
-COLUMN_WIDTHS_CONFIG: ColumnWidthsConfig = {
-    SECRET_SCAN_TYPE: {
-        ISSUE_TYPE_COLUMN: 2,
-        RULE_ID_COLUMN: 2,
-        FILE_PATH_COLUMN: 2,
-        SECRET_SHA_COLUMN: 2,
-        VIOLATION_COLUMN: 2,
-        SCAN_ID_COLUMN: 2,
-    },
-    INFRA_CONFIGURATION_SCAN_TYPE: {
-        ISSUE_TYPE_COLUMN: 4,
-        RULE_ID_COLUMN: 3,
-        FILE_PATH_COLUMN: 3,
-        SCAN_ID_COLUMN: 2,
-    },
-    SAST_SCAN_TYPE: {
-        ISSUE_TYPE_COLUMN: 7,
-        RULE_ID_COLUMN: 2,
-        FILE_PATH_COLUMN: 3,
-        SCAN_ID_COLUMN: 2,
-    },
+
+column_builder = ColumnInfoBuilder()
+
+# Building must have strict order. Represents the order of the columns in the table (from left to right)
+SEVERITY_COLUMN = column_builder.build(name='Severity')
+REPOSITORY_COLUMN = column_builder.build(name='Repository')
+
+FILE_PATH_COLUMN = column_builder.build(name='File Path')
+ECOSYSTEM_COLUMN = column_builder.build(name='Ecosystem')
+DEPENDENCY_NAME_COLUMN = column_builder.build(name='Dependency Name')
+DIRECT_DEPENDENCY_COLUMN = column_builder.build(name='Direct Dependency')
+DEVELOPMENT_DEPENDENCY_COLUMN = column_builder.build(name='Development Dependency')
+DEPENDENCY_PATHS_COLUMN = column_builder.build(name='Dependency Paths')
+
+CVE_COLUMNS = column_builder.build(name='CVE')
+UPGRADE_COLUMN = column_builder.build(name='Upgrade')
+LICENSE_COLUMN = column_builder.build(name='License')
+
+COLUMN_WIDTHS_CONFIG: ColumnWidths = {
+    REPOSITORY_COLUMN: 2,
+    FILE_PATH_COLUMN: 3,
+    CVE_COLUMNS: 5,
+    UPGRADE_COLUMN: 3,
+    LICENSE_COLUMN: 2,
 }
 
 
-class TablePrinter(BaseTablePrinter):
+class ScaTablePrinter(TablePrinterBase):
     def _print_results(self, local_scan_results: List['LocalScanResult']) -> None:
-        table = self._get_table()
-        if self.scan_type in COLUMN_WIDTHS_CONFIG:
-            table.set_cols_width(COLUMN_WIDTHS_CONFIG[self.scan_type])
+        detections_per_policy_id = self._extract_detections_per_policy_id(local_scan_results)
+        for policy_id, detections in detections_per_policy_id.items():
+            table = self._get_table(policy_id)
+            table.set_cols_width(COLUMN_WIDTHS_CONFIG)
 
-        for local_scan_result in local_scan_results:
-            for document_detections in local_scan_result.document_detections:
-                report_url = local_scan_result.report_url if local_scan_result.report_url else 'N/A'
-                for detection in document_detections.detections:
-                    table.set(REPORT_URL_COLUMN, report_url)
-                    table.set(SCAN_ID_COLUMN, local_scan_result.scan_id)
-                    self._enrich_table_with_values(table, detection, document_detections.document)
+            for detection in detections:
+                self._enrich_table_with_values(table, detection)
+
+            self._print_summary_issues(len(detections), self._get_title(policy_id))
+            self._print_table(table)
+
+        self._print_report_urls(local_scan_results)
+
+    @staticmethod
+    def _get_title(policy_id: str) -> str:
+        if policy_id == PACKAGE_VULNERABILITY_POLICY_ID:
+            return 'Dependency Vulnerabilities'
+        if policy_id == LICENSE_COMPLIANCE_POLICY_ID:
+            return 'License Compliance'
 
-        click.echo(table.get_table().draw())
+        return 'Unknown'
 
-    def _get_table(self) -> Table:
+    def _get_table(self, policy_id: str) -> Table:
         table = Table()
 
-        table.add(ISSUE_TYPE_COLUMN)
-        table.add(RULE_ID_COLUMN)
-        table.add(FILE_PATH_COLUMN)
-        table.add(LINE_NUMBER_COLUMN)
-        table.add(COLUMN_NUMBER_COLUMN)
-        table.add(SCAN_ID_COLUMN)
-        table.add(REPORT_URL_COLUMN)
+        if policy_id == PACKAGE_VULNERABILITY_POLICY_ID:
+            table.add(SEVERITY_COLUMN)
+            table.add(CVE_COLUMNS)
+            table.add(UPGRADE_COLUMN)
+        elif policy_id == LICENSE_COMPLIANCE_POLICY_ID:
+            table.add(LICENSE_COLUMN)
 
         if self._is_git_repository():
-            table.add(COMMIT_SHA_COLUMN)
+            table.add(REPOSITORY_COLUMN)
 
-        if self.scan_type == SECRET_SCAN_TYPE:
-            table.add(SECRET_SHA_COLUMN)
-            table.add(VIOLATION_LENGTH_COLUMN)
-            table.add(VIOLATION_COLUMN)
+        table.add(FILE_PATH_COLUMN)
+        table.add(ECOSYSTEM_COLUMN)
+        table.add(DEPENDENCY_NAME_COLUMN)
+        table.add(DIRECT_DEPENDENCY_COLUMN)
+        table.add(DEVELOPMENT_DEPENDENCY_COLUMN)
+        table.add(DEPENDENCY_PATHS_COLUMN)
 
         return table
 
-    def _enrich_table_with_values(self, table: Table, detection: Detection, document: Document) -> None:
-        self._enrich_table_with_detection_summary_values(table, detection, document)
-        self._enrich_table_with_detection_code_segment_values(table, detection, document)
-
-    def _enrich_table_with_detection_summary_values(
-        self, table: Table, detection: Detection, document: Document
-    ) -> None:
-        issue_type = detection.message
-        if self.scan_type == SECRET_SCAN_TYPE:
-            issue_type = detection.type
-
-        table.set(ISSUE_TYPE_COLUMN, issue_type)
-        table.set(RULE_ID_COLUMN, detection.detection_rule_id)
-        table.set(FILE_PATH_COLUMN, click.format_filename(document.path))
-        table.set(SECRET_SHA_COLUMN, detection.detection_details.get('sha512', ''))
-        table.set(COMMIT_SHA_COLUMN, detection.detection_details.get('commit_id', ''))
-
-    def _enrich_table_with_detection_code_segment_values(
-        self, table: Table, detection: Detection, document: Document
-    ) -> None:
+    @staticmethod
+    def _enrich_table_with_values(table: Table, detection: Detection) -> None:
         detection_details = detection.detection_details
 
-        detection_line = detection_details.get('line_in_file', -1)
-        if self.scan_type == SECRET_SCAN_TYPE:
-            detection_line = detection_details.get('line', -1)
-
-        detection_column = get_position_in_line(document.content, detection_details.get('start_position', -1))
-        violation_length = detection_details.get('length', -1)
-
-        violation = ''
-        file_content_lines = document.content.splitlines()
-        if detection_line < len(file_content_lines):
-            line = file_content_lines[detection_line]
-            violation = line[detection_column : detection_column + violation_length]
-
-            if not self.show_secret:
-                violation = obfuscate_text(violation)
-
-        table.set(LINE_NUMBER_COLUMN, str(detection_line))
-        table.set(COLUMN_NUMBER_COLUMN, str(detection_column))
-        table.set(VIOLATION_LENGTH_COLUMN, f'{violation_length} chars')
-        table.set(VIOLATION_COLUMN, violation)
+        table.set(SEVERITY_COLUMN, detection_details.get('advisory_severity'))
+        table.set(REPOSITORY_COLUMN, detection_details.get('repository_name'))
+
+        table.set(FILE_PATH_COLUMN, detection_details.get('file_name'))
+        table.set(ECOSYSTEM_COLUMN, detection_details.get('ecosystem'))
+        table.set(DEPENDENCY_NAME_COLUMN, detection_details.get('package_name'))
+        table.set(DIRECT_DEPENDENCY_COLUMN, detection_details.get('is_direct_dependency_str'))
+        table.set(DEVELOPMENT_DEPENDENCY_COLUMN, detection_details.get('is_dev_dependency_str'))
+
+        dependency_paths = 'N/A'
+        dependency_paths_raw = detection_details.get('dependency_paths')
+        if dependency_paths_raw:
+            dependency_paths = shortcut_dependency_paths(dependency_paths_raw)
+        table.set(DEPENDENCY_PATHS_COLUMN, dependency_paths)
+
+        upgrade = ''
+        alert = detection_details.get('alert')
+        if alert and alert.get('first_patched_version'):
+            upgrade = f'{alert.get("vulnerable_requirements")} -> {alert.get("first_patched_version")}'
+        table.set(UPGRADE_COLUMN, upgrade)
+
+        table.set(CVE_COLUMNS, detection_details.get('vulnerability_id'))
+        table.set(LICENSE_COLUMN, detection_details.get('license'))
+
+    @staticmethod
+    def _print_report_urls(local_scan_results: List['LocalScanResult']) -> None:
+        report_urls = [scan_result.report_url for scan_result in local_scan_results if scan_result.report_url]
+        if not report_urls:
+            return
+
+        click.echo('Report URLs:')
+        for report_url in report_urls:
+            click.echo(f'- {report_url}')
+
+    @staticmethod
+    def _print_summary_issues(detections_count: int, title: str) -> None:
+        click.echo(f'⛔ Found {detections_count} issues of type: {click.style(title, bold=True)}')
+
+    @staticmethod
+    def _extract_detections_per_policy_id(
+        local_scan_results: List['LocalScanResult'],
+    ) -> Dict[str, List[Detection]]:
+        detections_to_policy_id = defaultdict(list)
+
+        for local_scan_result in local_scan_results:
+            for document_detection in local_scan_result.document_detections:
+                for detection in document_detection.detections:
+                    detections_to_policy_id[detection.detection_type_id].append(detection)
+
+        # sort dict by keys (policy id) to make persist output order
+        return dict(sorted(detections_to_policy_id.items(), reverse=True))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cycode-0.2.6.dev9/cycode/cli/printers/text_printer.py` & `cycode-1.0.0/cycode/cli/printers/text_printer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import math
-from typing import TYPE_CHECKING, List, Optional
+from typing import TYPE_CHECKING, Dict, List, Optional
 
 import click
 
 from cycode.cli.config import config
 from cycode.cli.consts import COMMIT_RANGE_BASED_COMMAND_SCAN_TYPES, SECRET_SCAN_TYPE
 from cycode.cli.models import CliError, CliResult, Detection, Document, DocumentDetections
-from cycode.cli.printers.base_printer import BasePrinter
+from cycode.cli.printers.printer_base import PrinterBase
 from cycode.cli.utils.string_utils import get_position_in_line, obfuscate_text
 
 if TYPE_CHECKING:
     from cycode.cli.models import LocalScanResult
 
 
-class TextPrinter(BasePrinter):
-    def __init__(self, context: click.Context):
+class TextPrinter(PrinterBase):
+    def __init__(self, context: click.Context) -> None:
         super().__init__(context)
         self.scan_type: str = context.obj.get('scan_type')
         self.command_scan_type: str = context.info_name
         self.show_secret: bool = context.obj.get('show_secret', False)
 
     def print_result(self, result: CliResult) -> None:
         color = None
@@ -26,37 +26,51 @@
             color = self.RED_COLOR_NAME
 
         click.secho(result.message, fg=color)
 
     def print_error(self, error: CliError) -> None:
         click.secho(error.message, fg=self.RED_COLOR_NAME)
 
-    def print_scan_results(self, local_scan_results: List['LocalScanResult']):
-        if all(result.issue_detected == 0 for result in local_scan_results):
+    def print_scan_results(
+        self, local_scan_results: List['LocalScanResult'], errors: Optional[Dict[str, 'CliError']] = None
+    ) -> None:
+        if not errors and all(result.issue_detected == 0 for result in local_scan_results):
             click.secho('Good job! No issues were found!!! 👏👏👏', fg=self.GREEN_COLOR_NAME)
             return
 
         for local_scan_result in local_scan_results:
             for document_detections in local_scan_result.document_detections:
                 self._print_document_detections(
                     document_detections, local_scan_result.scan_id, local_scan_result.report_url
                 )
 
+        if not errors:
+            return
+
+        click.secho(
+            'Unfortunately, Cycode was unable to complete the full scan. '
+            'Please note that not all results may be available:',
+            fg='red',
+        )
+        for scan_id, error in errors.items():
+            click.echo(f'- {scan_id}: ', nl=False)
+            self.print_error(error)
+
     def _print_document_detections(
         self, document_detections: DocumentDetections, scan_id: str, report_url: Optional[str]
-    ):
+    ) -> None:
         document = document_detections.document
         lines_to_display = self._get_lines_to_display_count()
         for detection in document_detections.detections:
             self._print_detection_summary(detection, document.path, scan_id, report_url)
             self._print_detection_code_segment(detection, document, lines_to_display)
 
     def _print_detection_summary(
         self, detection: Detection, document_path: str, scan_id: str, report_url: Optional[str]
-    ):
+    ) -> None:
         detection_name = detection.type if self.scan_type == SECRET_SCAN_TYPE else detection.message
 
         detection_sha = detection.detection_details.get('sha512')
         detection_sha_message = f'\nSecret SHA: {detection_sha}' if detection_sha else ''
 
         scan_id_message = f'\nScan ID: {scan_id}'
         report_url_message = f'\nReport URL: {report_url}' if report_url else ''
@@ -66,49 +80,50 @@
 
         click.echo(
             f'⛔  Found issue of type: {click.style(detection_name, fg="bright_red", bold=True)} '
             f'(rule ID: {detection.detection_rule_id}) in file: {click.format_filename(document_path)} '
             f'{detection_sha_message}{scan_id_message}{report_url_message}{detection_commit_id_message}  ⛔'
         )
 
-    def _print_detection_code_segment(self, detection: Detection, document: Document, code_segment_size: int):
+    def _print_detection_code_segment(self, detection: Detection, document: Document, code_segment_size: int) -> None:
         if self._is_git_diff_based_scan():
             self._print_detection_from_git_diff(detection, document)
             return
 
         self._print_detection_from_file(detection, document, code_segment_size)
 
-    def _get_code_segment_start_line(self, detection_line: int, code_segment_size: int):
+    @staticmethod
+    def _get_code_segment_start_line(detection_line: int, code_segment_size: int) -> int:
         start_line = detection_line - math.ceil(code_segment_size / 2)
         return 0 if start_line < 0 else start_line
 
     def _print_line_of_code_segment(
         self,
         document: Document,
         line: str,
         line_number: int,
         detection_position_in_line: int,
         violation_length: int,
         is_detection_line: bool,
-    ):
+    ) -> None:
         if is_detection_line:
             self._print_detection_line(document, line, line_number, detection_position_in_line, violation_length)
         else:
             self._print_line(document, line, line_number)
 
     def _print_detection_line(
         self, document: Document, line: str, line_number: int, detection_position_in_line: int, violation_length: int
     ) -> None:
         detection_line = self._get_detection_line_style(
             line, document.is_git_diff_format, detection_position_in_line, violation_length
         )
 
         click.echo(f'{self._get_line_number_style(line_number)} {detection_line}')
 
-    def _print_line(self, document: Document, line: str, line_number: int):
+    def _print_line(self, document: Document, line: str, line_number: int) -> None:
         line_no = self._get_line_number_style(line_number)
         line = self._get_line_style(line, document.is_git_diff_format)
 
         click.echo(f'{line_no} {line}')
 
     def _get_detection_line_style(self, line: str, is_git_diff: bool, start_position: int, length: int) -> str:
         line_color = self._get_line_color(line, is_git_diff)
@@ -144,15 +159,15 @@
             return self.GREEN_COLOR_NAME
 
         if line.startswith('-'):
             return self.RED_COLOR_NAME
 
         return self.WHITE_COLOR_NAME
 
-    def _get_line_number_style(self, line_number: int):
+    def _get_line_number_style(self, line_number: int) -> str:
         return (
             f'{click.style(str(line_number), fg=self.WHITE_COLOR_NAME, bold=False)} '
             f'{click.style("|", fg=self.RED_COLOR_NAME, bold=False)}'
         )
 
     def _get_lines_to_display_count(self) -> int:
         result_printer_configuration = config.get('result_printer')
@@ -160,15 +175,15 @@
             result_printer_configuration.get(self.scan_type, {}).get(self.command_scan_type, {}).get('lines_to_display')
         )
         if lines_to_display_of_scan:
             return lines_to_display_of_scan
 
         return result_printer_configuration.get('default').get('lines_to_display')
 
-    def _print_detection_from_file(self, detection: Detection, document: Document, code_segment_size: int):
+    def _print_detection_from_file(self, detection: Detection, document: Document, code_segment_size: int) -> None:
         detection_details = detection.detection_details
         detection_line = (
             detection_details.get('line', -1)
             if self.scan_type == SECRET_SCAN_TYPE
             else detection_details.get('line_in_file', -1)
         )
         detection_position = detection_details.get('start_position', -1)
@@ -193,15 +208,15 @@
                 current_line_index + 1,
                 detection_position_in_line,
                 violation_length,
                 is_detection_line,
             )
         click.echo()
 
-    def _print_detection_from_git_diff(self, detection: Detection, document: Document):
+    def _print_detection_from_git_diff(self, detection: Detection, document: Document) -> None:
         detection_details = detection.detection_details
         detection_line_number = detection_details.get('line', -1)
         detection_line_number_in_original_file = detection_details.get('line_in_file', -1)
         detection_position = detection_details.get('start_position', -1)
         violation_length = detection_details.get('length', -1)
 
         git_diff_content = document.content
@@ -215,9 +230,9 @@
             detection_line,
             detection_line_number_in_original_file,
             detection_position_in_line,
             violation_length,
         )
         click.echo()
 
-    def _is_git_diff_based_scan(self):
+    def _is_git_diff_based_scan(self) -> bool:
         return self.command_scan_type in COMMIT_RANGE_BASED_COMMAND_SCAN_TYPES and self.scan_type == SECRET_SCAN_TYPE
```

### Comparing `cycode-0.2.6.dev9/cycode/cli/user_settings/config_file_manager.py` & `cycode-1.0.0/cycode/cli/user_settings/config_file_manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import os
-from typing import Dict, List, Optional
+from typing import TYPE_CHECKING, Any, Dict, Hashable, List, Optional, Union
 
 from cycode.cli.consts import CYCODE_CONFIGURATION_DIRECTORY
 from cycode.cli.user_settings.base_file_manager import BaseFileManager
 
+if TYPE_CHECKING:
+    from pathlib import Path
+
 
 class ConfigFileManager(BaseFileManager):
     CYCODE_HIDDEN_DIRECTORY: str = CYCODE_CONFIGURATION_DIRECTORY
     FILE_NAME: str = 'config.yaml'
 
     ENVIRONMENT_SECTION_NAME: str = 'environment'
     EXCLUSIONS_SECTION_NAME: str = 'exclusions'
@@ -18,53 +21,53 @@
     APP_URL_FIELD_NAME: str = 'cycode_app_url'
     VERBOSE_FIELD_NAME: str = 'verbose'
 
     MAX_COMMITS_FIELD_NAME: str = 'max_commits'
     COMMAND_TIMEOUT_FIELD_NAME: str = 'command_timeout'
     EXCLUDE_DETECTIONS_IN_DELETED_LINES: str = 'exclude_detections_in_deleted_lines'
 
-    def __init__(self, path):
+    def __init__(self, path: Union['Path', str]) -> None:
         self.path = path
 
-    def get_api_url(self) -> Optional[str]:
+    def get_api_url(self) -> Optional[Any]:
         return self._get_value_from_environment_section(self.API_URL_FIELD_NAME)
 
-    def get_app_url(self) -> Optional[str]:
+    def get_app_url(self) -> Optional[Any]:
         return self._get_value_from_environment_section(self.APP_URL_FIELD_NAME)
 
-    def get_verbose_flag(self) -> Optional[bool]:
+    def get_verbose_flag(self) -> Optional[Any]:
         return self._get_value_from_environment_section(self.VERBOSE_FIELD_NAME)
 
-    def get_exclusions_by_scan_type(self, scan_type) -> Dict:
+    def get_exclusions_by_scan_type(self, scan_type: str) -> Dict[Hashable, Any]:
         exclusions_section = self._get_section(self.EXCLUSIONS_SECTION_NAME)
         return exclusions_section.get(scan_type, {})
 
-    def get_max_commits(self, command_scan_type) -> Optional[int]:
+    def get_max_commits(self, command_scan_type: str) -> Optional[Any]:
         return self._get_value_from_command_scan_type_configuration(command_scan_type, self.MAX_COMMITS_FIELD_NAME)
 
-    def get_command_timeout(self, command_scan_type) -> Optional[int]:
+    def get_command_timeout(self, command_scan_type: str) -> Optional[Any]:
         return self._get_value_from_command_scan_type_configuration(command_scan_type, self.COMMAND_TIMEOUT_FIELD_NAME)
 
-    def get_exclude_detections_in_deleted_lines(self, command_scan_type) -> Optional[bool]:
+    def get_exclude_detections_in_deleted_lines(self, command_scan_type: str) -> Optional[Any]:
         return self._get_value_from_command_scan_type_configuration(
             command_scan_type, self.EXCLUDE_DETECTIONS_IN_DELETED_LINES
         )
 
-    def update_base_url(self, base_url: str):
+    def update_base_url(self, base_url: str) -> None:
         update_data = {self.ENVIRONMENT_SECTION_NAME: {self.API_URL_FIELD_NAME: base_url}}
         self.write_content_to_file(update_data)
 
     def get_installation_id(self) -> Optional[str]:
         return self._get_value_from_environment_section(self.INSTALLATION_ID_FIELD_NAME)
 
     def update_installation_id(self, installation_id: str) -> None:
         update_data = {self.ENVIRONMENT_SECTION_NAME: {self.INSTALLATION_ID_FIELD_NAME: installation_id}}
         self.write_content_to_file(update_data)
 
-    def add_exclusion(self, scan_type, exclusion_type, new_exclusion):
+    def add_exclusion(self, scan_type: str, exclusion_type: str, new_exclusion: str) -> None:
         exclusions = self._get_exclusions_by_exclusion_type(scan_type, exclusion_type)
         if new_exclusion in exclusions:
             return
 
         exclusions.append(new_exclusion)
 
         update_data = {self.EXCLUSIONS_SECTION_NAME: {scan_type: {exclusion_type: exclusions}}}
@@ -76,26 +79,26 @@
     def get_filename(self) -> str:
         return os.path.join(self.get_config_directory_path(), self.FILE_NAME)
 
     @staticmethod
     def get_config_file_route() -> str:
         return os.path.join(ConfigFileManager.CYCODE_HIDDEN_DIRECTORY, ConfigFileManager.FILE_NAME)
 
-    def _get_exclusions_by_exclusion_type(self, scan_type, exclusion_type) -> List:
+    def _get_exclusions_by_exclusion_type(self, scan_type: str, exclusion_type: str) -> List[Any]:
         scan_type_exclusions = self.get_exclusions_by_scan_type(scan_type)
         return scan_type_exclusions.get(exclusion_type, [])
 
-    def _get_value_from_environment_section(self, field_name: str):
+    def _get_value_from_environment_section(self, field_name: str) -> Optional[Any]:
         environment_section = self._get_section(self.ENVIRONMENT_SECTION_NAME)
         return environment_section.get(field_name)
 
-    def _get_scan_configuration_by_scan_type(self, command_scan_type: str) -> Dict:
+    def _get_scan_configuration_by_scan_type(self, command_scan_type: str) -> Dict[Hashable, Any]:
         scan_section = self._get_section(self.SCAN_SECTION_NAME)
         return scan_section.get(command_scan_type, {})
 
-    def _get_value_from_command_scan_type_configuration(self, command_scan_type: str, field_name: str):
+    def _get_value_from_command_scan_type_configuration(self, command_scan_type: str, field_name: str) -> Optional[Any]:
         command_scan_type_configuration = self._get_scan_configuration_by_scan_type(command_scan_type)
         return command_scan_type_configuration.get(field_name)
 
-    def _get_section(self, section_name: str) -> Dict:
+    def _get_section(self, section_name: str) -> Dict[Hashable, Any]:
         file_content = self.read_file()
         return file_content.get(section_name, {})
```

### Comparing `cycode-0.2.6.dev9/cycode/cli/user_settings/configuration_manager.py` & `cycode-1.0.0/cycode/cli/user_settings/configuration_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import os
+from functools import lru_cache
 from pathlib import Path
-from typing import Dict, Optional
+from typing import Any, Dict, Optional
 from uuid import uuid4
 
 from cycode.cli import consts
 from cycode.cli.user_settings.config_file_manager import ConfigFileManager
 
 
 class ConfigurationManager:
     global_config_file_manager: ConfigFileManager
     local_config_file_manager: ConfigFileManager
 
-    def __init__(self):
+    def __init__(self) -> None:
         self.global_config_file_manager = ConfigFileManager(Path.home())
         self.local_config_file_manager = ConfigFileManager(os.getcwd())
 
     def get_cycode_api_url(self) -> str:
         api_url = self.get_api_url_from_environment_variables()
         if api_url is not None:
             return api_url
@@ -57,28 +58,29 @@
     def get_app_url_from_environment_variables(self) -> Optional[str]:
         return self._get_value_from_environment_variables(consts.CYCODE_APP_URL_ENV_VAR_NAME)
 
     def get_verbose_flag_from_environment_variables(self) -> bool:
         value = self._get_value_from_environment_variables(consts.VERBOSE_ENV_VAR_NAME, '')
         return value.lower() in ('true', '1')
 
-    def get_exclusions_by_scan_type(self, scan_type) -> Dict:
+    @lru_cache(maxsize=None)  # noqa: B019
+    def get_exclusions_by_scan_type(self, scan_type: str) -> Dict:
         local_exclusions = self.local_config_file_manager.get_exclusions_by_scan_type(scan_type)
         global_exclusions = self.global_config_file_manager.get_exclusions_by_scan_type(scan_type)
         return self._merge_exclusions(local_exclusions, global_exclusions)
 
-    def add_exclusion(self, scope: str, scan_type: str, exclusion_type: str, value: str):
+    def add_exclusion(self, scope: str, scan_type: str, exclusion_type: str, value: str) -> None:
         config_file_manager = self.get_config_file_manager(scope)
         config_file_manager.add_exclusion(scan_type, exclusion_type, value)
 
     def _merge_exclusions(self, local_exclusions: Dict, global_exclusions: Dict) -> Dict:
         keys = set(list(local_exclusions.keys()) + list(global_exclusions.keys()))
         return {key: local_exclusions.get(key, []) + global_exclusions.get(key, []) for key in keys}
 
-    def update_base_url(self, base_url: str, scope: str = 'local'):
+    def update_base_url(self, base_url: str, scope: str = 'local') -> None:
         config_file_manager = self.get_config_file_manager(scope)
         config_file_manager.update_base_url(base_url)
 
     def get_or_create_installation_id(self) -> str:
         config_file_manager = self.get_config_file_manager()
 
         installation_id = config_file_manager.get_installation_id()
@@ -158,9 +160,9 @@
         )
         if exclude_detections_in_deleted_lines is not None:
             return exclude_detections_in_deleted_lines
 
         return consts.DEFAULT_EXCLUDE_DETECTIONS_IN_DELETED_LINES
 
     @staticmethod
-    def _get_value_from_environment_variables(env_var_name, default=None):
+    def _get_value_from_environment_variables(env_var_name: str, default: Optional[Any] = None) -> Optional[Any]:
         return os.getenv(env_var_name, default)
```

### Comparing `cycode-0.2.6.dev9/cycode/cli/user_settings/credentials_manager.py` & `cycode-1.0.0/cycode/cli/user_settings/credentials_manager.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,48 @@
 import os
 from pathlib import Path
+from typing import Optional, Tuple
 
 from cycode.cli.config import CYCODE_CLIENT_ID_ENV_VAR_NAME, CYCODE_CLIENT_SECRET_ENV_VAR_NAME
 from cycode.cli.user_settings.base_file_manager import BaseFileManager
 from cycode.cli.utils.yaml_utils import read_file
 
 
 class CredentialsManager(BaseFileManager):
     HOME_PATH: str = Path.home()
     CYCODE_HIDDEN_DIRECTORY: str = '.cycode'
     FILE_NAME: str = 'credentials.yaml'
     CLIENT_ID_FIELD_NAME: str = 'cycode_client_id'
     CLIENT_SECRET_FIELD_NAME: str = 'cycode_client_secret'
 
-    def get_credentials(self) -> (str, str):
+    def get_credentials(self) -> Tuple[str, str]:
         client_id, client_secret = self.get_credentials_from_environment_variables()
         if client_id is not None and client_secret is not None:
             return client_id, client_secret
 
         return self.get_credentials_from_file()
 
-    def get_credentials_from_environment_variables(self) -> (str, str):
+    @staticmethod
+    def get_credentials_from_environment_variables() -> Tuple[str, str]:
         client_id = os.getenv(CYCODE_CLIENT_ID_ENV_VAR_NAME)
         client_secret = os.getenv(CYCODE_CLIENT_SECRET_ENV_VAR_NAME)
         return client_id, client_secret
 
-    def get_credentials_from_file(self) -> (str, str):
+    def get_credentials_from_file(self) -> Tuple[Optional[str], Optional[str]]:
         credentials_filename = self.get_filename()
         try:
             file_content = read_file(credentials_filename)
         except FileNotFoundError:
             return None, None
 
         client_id = file_content.get(self.CLIENT_ID_FIELD_NAME)
         client_secret = file_content.get(self.CLIENT_SECRET_FIELD_NAME)
         return client_id, client_secret
 
-    def update_credentials_file(self, client_id: str, client_secret: str):
+    def update_credentials_file(self, client_id: str, client_secret: str) -> None:
         credentials = {self.CLIENT_ID_FIELD_NAME: client_id, self.CLIENT_SECRET_FIELD_NAME: client_secret}
 
         self.get_filename()
         self.write_content_to_file(credentials)
 
     def get_filename(self) -> str:
         return os.path.join(self.HOME_PATH, self.CYCODE_HIDDEN_DIRECTORY, self.FILE_NAME)
```

### Comparing `cycode-0.2.6.dev9/cycode/cli/user_settings/user_settings_commands.py` & `cycode-1.0.0/cycode/cli/user_settings/user_settings_commands.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,79 +18,79 @@
     ' precedent over these credentials; either update or remove '
     'the environment variables.'
 )
 credentials_manager = CredentialsManager()
 
 
 @click.command(
-    short_help='Initial command to authenticate your CLI client with Cycode using client ID and client secret'
+    short_help='Initial command to authenticate your CLI client with Cycode using a client ID and client secret.'
 )
-def set_credentials():
+def set_credentials() -> None:
+    """Authenticates your CLI client with Cycode manually by using a client ID and client secret."""
     click.echo(f'Update credentials in file ({credentials_manager.get_filename()})')
     current_client_id, current_client_secret = credentials_manager.get_credentials_from_file()
     client_id = _get_client_id_input(current_client_id)
     client_secret = _get_client_secret_input(current_client_secret)
 
     if not _should_update_credentials(current_client_id, current_client_secret, client_id, client_secret):
         return
 
     credentials_manager.update_credentials_file(client_id, client_secret)
     click.echo(_get_credentials_update_result_message())
 
 
-@click.command()
+@click.command(short_help='Ignores a specific value, path or rule ID.')
 @click.option(
-    '--by-value', type=click.STRING, required=False, help='Ignore a specific value while scanning for secrets'
+    '--by-value', type=click.STRING, required=False, help='Ignore a specific value while scanning for Secrets.'
 )
 @click.option(
     '--by-sha',
     type=click.STRING,
     required=False,
-    help='Ignore a specific SHA512 representation of a string while scanning for secrets',
+    help='Ignore a specific SHA512 representation of a string while scanning for Secrets.',
 )
 @click.option(
-    '--by-path', type=click.STRING, required=False, help='Avoid scanning a specific path. Need to specify scan type '
+    '--by-path',
+    type=click.STRING,
+    required=False,
+    help='Avoid scanning a specific path. You`ll need to specify the scan type.',
 )
 @click.option(
     '--by-rule',
     type=click.STRING,
     required=False,
-    help='Ignore scanning a specific secret rule ID/IaC rule ID. Need to specify scan type.',
+    help='Ignore scanning a specific secret rule ID or IaC rule ID. You`ll to specify the scan type.',
 )
 @click.option(
     '--by-package',
     type=click.STRING,
     required=False,
-    help='Ignore scanning a specific package version while running SCA scan. expected pattern - name@version',
+    help='Ignore scanning a specific package version while running an SCA scan. Expected pattern: name@version.',
 )
 @click.option(
     '--scan-type',
     '-t',
     default='secret',
-    help="""
-              \b
-              Specify the scan you wish to execute (secrets/iac),
-              the default is secrets
-              """,
+    help='Specify the type of scan you wish to execute (the default is Secrets).',
     type=click.Choice(config['scans']['supported_scans']),
     required=False,
 )
 @click.option(
     '--global',
     '-g',
     'is_global',
     is_flag=True,
     default=False,
     required=False,
-    help='Add an ignore rule and update it in the global .cycode config file',
+    help='Add an ignore rule to the global CLI config.',
 )
 def add_exclusions(
     by_value: str, by_sha: str, by_path: str, by_rule: str, by_package: str, scan_type: str, is_global: bool
-):
-    """Ignore a specific value, path or rule ID"""
+) -> None:
+    """Ignores a specific value, path or rule ID."""
     if not by_value and not by_sha and not by_path and not by_rule and not by_package:
         raise click.ClickException('ignore by type is missing')
 
     if any(by is not None for by in [by_value, by_sha]) and scan_type != consts.SECRET_SCAN_TYPE:
         raise click.ClickException('this exclude is supported only for secret scan type')
 
     if by_value is not None:
@@ -139,22 +139,22 @@
 def _get_client_secret_input(current_client_secret: str) -> str:
     new_client_secret = click.prompt(
         f'cycode client secret [{_obfuscate_credential(current_client_secret)}]', default='', show_default=False
     )
     return new_client_secret if new_client_secret else current_client_secret
 
 
-def _get_credentials_update_result_message():
+def _get_credentials_update_result_message() -> str:
     if not _are_credentials_exist_in_environment_variables():
         return CREDENTIALS_UPDATED_SUCCESSFULLY_MESSAGE
 
     return CREDENTIALS_UPDATED_SUCCESSFULLY_MESSAGE + ' ' + CREDENTIALS_ARE_SET_IN_ENVIRONMENT_VARIABLES_MESSAGE
 
 
-def _are_credentials_exist_in_environment_variables():
+def _are_credentials_exist_in_environment_variables() -> bool:
     client_id, client_secret = credentials_manager.get_credentials_from_environment_variables()
     return client_id is not None or client_secret is not None
 
 
 def _should_update_credentials(
     current_client_id: str, current_client_secret: str, new_client_id: str, new_client_secret: str
 ) -> bool:
```

### Comparing `cycode-0.2.6.dev9/cycode/cli/utils/path_utils.py` & `cycode-1.0.0/cycode/cli/utils/path_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 import os
-from pathlib import Path
+from functools import lru_cache
 from typing import AnyStr, Iterable, List, Optional
 
 import pathspec
 from binaryornot.check import is_binary
 
 
 def get_relevant_files_in_path(path: str, exclude_patterns: Iterable[str]) -> List[str]:
     absolute_path = get_absolute_path(path)
+
     if not os.path.isfile(absolute_path) and not os.path.isdir(absolute_path):
-        raise FileNotFoundError(f'the specified path was not found, path: {path}')
+        raise FileNotFoundError(f'the specified path was not found, path: {absolute_path}')
 
     if os.path.isfile(absolute_path):
         return [absolute_path]
 
-    directory_files_paths = _get_all_existing_files_in_directory(absolute_path)
-    file_paths = set({str(file_path) for file_path in directory_files_paths})
-    spec = pathspec.PathSpec.from_lines(pathspec.patterns.GitWildMatchPattern, exclude_patterns)
-    exclude_file_paths = set(spec.match_files(file_paths))
+    all_file_paths = set(_get_all_existing_files_in_directory(absolute_path))
+
+    path_spec = pathspec.PathSpec.from_lines(pathspec.patterns.GitWildMatchPattern, exclude_patterns)
+    excluded_file_paths = set(path_spec.match_files(all_file_paths))
+
+    relevant_file_paths = all_file_paths - excluded_file_paths
 
-    return [file_path for file_path in (file_paths - exclude_file_paths) if os.path.isfile(file_path)]
+    return [file_path for file_path in relevant_file_paths if os.path.isfile(file_path)]
 
 
+@lru_cache(maxsize=None)
 def is_sub_path(path: str, sub_path: str) -> bool:
     try:
         common_path = os.path.commonpath([get_absolute_path(path), get_absolute_path(sub_path)])
         return path == common_path
     except ValueError:
         # if paths are on the different drives
         return False
@@ -45,20 +49,25 @@
     return os.path.getsize(filename)
 
 
 def get_path_by_os(filename: str) -> str:
     return filename.replace('/', os.sep)
 
 
-def _get_all_existing_files_in_directory(path: str):
-    directory = Path(path)
-    return directory.rglob(r'*')
+def _get_all_existing_files_in_directory(path: str) -> List[str]:
+    files: List[str] = []
+
+    for root, _, filenames in os.walk(path):
+        for filename in filenames:
+            files.append(os.path.join(root, filename))
+
+    return files
 
 
-def is_path_exists(path: str):
+def is_path_exists(path: str) -> bool:
     return os.path.exists(path)
 
 
 def get_file_dir(path: str) -> str:
     return os.path.dirname(path)
```

### Comparing `cycode-0.2.6.dev9/cycode/cli/utils/progress_bar.py` & `cycode-1.0.0/cycode/cli/utils/progress_bar.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import click
 
 from cycode.cli.utils.enum_utils import AutoCountEnum
 from cycode.cyclient.config import get_logger
 
 if TYPE_CHECKING:
     from click._termui_impl import ProgressBar
+    from click.termui import V as ProgressBarValue
 
 
 logger = get_logger('progress bar')
 
 
 class ProgressBarSection(AutoCountEnum):
     PREPARE_LOCAL_FILES = auto()
@@ -35,17 +36,14 @@
 
 _PROGRESS_BAR_LENGTH = 100
 
 _PROGRESS_BAR_SECTIONS = {
     ProgressBarSection.PREPARE_LOCAL_FILES: ProgressBarSectionInfo(
         ProgressBarSection.PREPARE_LOCAL_FILES, 'Prepare local files', start_percent=0, stop_percent=5
     ),
-    # TODO(MarshalX): could be added in the future
-    # ProgressBarSection.UPLOAD_FILES: ProgressBarSectionInfo(
-    # ),
     ProgressBarSection.SCAN: ProgressBarSectionInfo(
         ProgressBarSection.SCAN, 'Scan in progress', start_percent=5, stop_percent=95
     ),
     ProgressBarSection.GENERATE_REPORT: ProgressBarSectionInfo(
         ProgressBarSection.GENERATE_REPORT, 'Generate report', start_percent=95, stop_percent=100
     ),
 }
@@ -53,15 +51,15 @@
 
 def _get_section_length(section: 'ProgressBarSection') -> int:
     return _PROGRESS_BAR_SECTIONS[section].stop_percent - _PROGRESS_BAR_SECTIONS[section].start_percent
 
 
 class BaseProgressBar(ABC):
     @abstractmethod
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, **kwargs) -> None:
         pass
 
     @abstractmethod
     def __enter__(self) -> 'BaseProgressBar':
         ...
 
     @abstractmethod
@@ -82,15 +80,15 @@
 
     @abstractmethod
     def update(self, section: 'ProgressBarSection') -> None:
         ...
 
 
 class DummyProgressBar(BaseProgressBar):
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
 
     def __enter__(self) -> 'DummyProgressBar':
         return self
 
     def __exit__(self, *args, **kwargs) -> None:
         pass
@@ -105,15 +103,15 @@
         pass
 
     def update(self, section: 'ProgressBarSection') -> None:
         pass
 
 
 class CompositeProgressBar(BaseProgressBar):
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__()
         self._progress_bar_context_manager = click.progressbar(
             length=_PROGRESS_BAR_LENGTH,
             item_show_func=self._progress_bar_item_show_func,
             update_min_steps=0,
         )
         self._progress_bar: Optional['ProgressBar'] = None
@@ -144,14 +142,16 @@
 
     def set_section_length(self, section: 'ProgressBarSection', length: int) -> None:
         logger.debug(f'set_section_length: {section} {length}')
         self._section_lengths[section] = length
 
         if length == 0:
             self._skip_section(section)
+        else:
+            self._maybe_update_current_section()
 
     def _skip_section(self, section: 'ProgressBarSection') -> None:
         self._progress_bar.update(_get_section_length(section))
         self._maybe_update_current_section()
 
     def _increment_section_value(self, section: 'ProgressBarSection', value: int) -> None:
         self._section_values[section] = self._section_values.get(section, 0) + value
@@ -188,15 +188,15 @@
         max_val = self._section_lengths[section]
         cur_val = self._section_values[section]
 
         expected_value = round(_get_section_length(section) * (cur_val / max_val))
 
         return expected_value - self._current_section_value
 
-    def _progress_bar_item_show_func(self, _=None) -> str:
+    def _progress_bar_item_show_func(self, _: Optional['ProgressBarValue'] = None) -> str:
         return self._current_section.label
 
     def update(self, section: 'ProgressBarSection', value: int = 1) -> None:
         if not self._progress_bar:
             raise ValueError('Progress bar is not initialized. Call start() first or use "with" statement.')
 
         if section not in self._section_lengths:
```

### Comparing `cycode-0.2.6.dev9/cycode/cli/utils/scan_batch.py` & `cycode-1.0.0/cycode/cli/utils/scan_batch.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,16 @@
     if current_batch:
         batches.append(current_batch)
 
     return batches
 
 
 def _get_threads_count() -> int:
-    return min(os.cpu_count() * SCAN_BATCH_SCANS_PER_CPU, SCAN_BATCH_MAX_PARALLEL_SCANS)
+    cpu_count = os.cpu_count() or 1
+    return min(cpu_count * SCAN_BATCH_SCANS_PER_CPU, SCAN_BATCH_MAX_PARALLEL_SCANS)
 
 
 def run_parallel_batched_scan(
     scan_function: Callable[[List[Document]], Tuple[str, 'CliError', 'LocalScanResult']],
     documents: List[Document],
     progress_bar: 'BaseProgressBar',
     max_size_mb: int = SCAN_BATCH_MAX_SIZE_IN_BYTES,
```

### Comparing `cycode-0.2.6.dev9/cycode/cli/utils/shell_executor.py` & `cycode-1.0.0/cycode/cli/utils/shell_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from cycode.cyclient import logger
 
 _SUBPROCESS_DEFAULT_TIMEOUT_SEC = 60
 
 
 def shell(
-    command: Union[str, List[str]], timeout: int = _SUBPROCESS_DEFAULT_TIMEOUT_SEC, execute_in_shell=False
+    command: Union[str, List[str]], timeout: int = _SUBPROCESS_DEFAULT_TIMEOUT_SEC, execute_in_shell: bool = False
 ) -> Optional[str]:
     logger.debug(f'Executing shell command: {command}')
 
     try:
         result = subprocess.run(
             command,
             timeout=timeout,
```

### Comparing `cycode-0.2.6.dev9/cycode/cli/utils/string_utils.py` & `cycode-1.0.0/cycode/cli/utils/string_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,27 +26,27 @@
 def is_binary_content(content: str) -> bool:
     """Get the first 1024 chars and check if it's binary or not."""
     chunk = content[:1024]
     chunk_bytes = convert_string_to_bytes(chunk)
     return is_binary_string(chunk_bytes)
 
 
-def get_content_size(content: str):
+def get_content_size(content: str) -> int:
     return getsizeof(content)
 
 
-def convert_string_to_bytes(content: str):
+def convert_string_to_bytes(content: str) -> bytes:
     return bytes(content, 'UTF-8')
 
 
-def hash_string_to_sha256(content: str):
+def hash_string_to_sha256(content: str) -> str:
     return hashlib.sha256(content.encode()).hexdigest()
 
 
-def generate_random_string(string_len: int):
+def generate_random_string(string_len: int) -> str:
     # letters, digits, and symbols
     characters = string.ascii_letters + string.digits + string.punctuation
     return ''.join(random.choice(characters) for _ in range(string_len))  # noqa: S311
 
 
 def get_position_in_line(text: str, position: int) -> int:
     return position - text.rfind('\n', 0, position) - 1
```

### Comparing `cycode-0.2.6.dev9/cycode/cli/utils/task_timer.py` & `cycode-1.0.0/cycode/cli/utils/task_timer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 from _thread import interrupt_main
 from threading import Event, Thread
 from types import TracebackType
 from typing import Callable, Dict, List, Optional, Type
 
 
 class FunctionContext:
-    def __init__(self, function: Callable, args: Optional[List] = None, kwargs: Optional[Dict] = None):
+    def __init__(self, function: Callable, args: Optional[List] = None, kwargs: Optional[Dict] = None) -> None:
         self.function = function
         self.args = args or []
         self.kwargs = kwargs or {}
 
 
 class TimerThread(Thread):
     """
     Custom thread class for executing timer in the background
 
     Members:
         timeout - the amount of time to count until timeout in seconds
         quit_function (Mandatory) - function to perform when reaching to timeout
     """
 
-    def __init__(self, timeout: int, quit_function: FunctionContext):
+    def __init__(self, timeout: int, quit_function: FunctionContext) -> None:
         Thread.__init__(self)
         self._timeout = timeout
         self._quit_function = quit_function
         self.event = Event()
 
-    def run(self):
+    def run(self) -> None:
         self._run_quit_function_on_timeout()
 
-    def stop(self):
+    def stop(self) -> None:
         self.event.set()
 
-    def _run_quit_function_on_timeout(self):
+    def _run_quit_function_on_timeout(self) -> None:
         self.event.wait(self._timeout)
         if not self.event.is_set():
             self._call_quit_function()
         self.stop()
 
-    def _call_quit_function(self):
+    def _call_quit_function(self) -> None:
         self._quit_function.function(*self._quit_function.args, **self._quit_function.kwargs)
 
 
 class TimeoutAfter:
     """
     A task wrapper for controlling how much time a task should be run before timing out
 
@@ -52,15 +52,15 @@
 
     Members:
         timeout - the amount of time to count until timeout in seconds
         quit_function (Optional) - function to perform when reaching to timeout,
                                    the default option is to interrupt main thread
     """
 
-    def __init__(self, timeout: int, quit_function: Optional[FunctionContext] = None):
+    def __init__(self, timeout: int, quit_function: Optional[FunctionContext] = None) -> None:
         self.timeout = timeout
         self._quit_function = quit_function or FunctionContext(function=self.timeout_function)
         self.timer = TimerThread(timeout, quit_function=self._quit_function)
 
     def __enter__(self) -> None:
         if self.timeout:
             self.timer.start()
@@ -72,9 +72,9 @@
             self.timer.stop()
 
         # catch the exception of interrupt_main before exiting
         # the with statement and throw timeout error instead
         if exc_type == KeyboardInterrupt:
             raise TimeoutError(f'Task timed out after {self.timeout} seconds')
 
-    def timeout_function(self):
+    def timeout_function(self) -> None:
         interrupt_main()
```

### Comparing `cycode-0.2.6.dev9/cycode/cli/utils/yaml_utils.py` & `cycode-1.0.0/cycode/cli/utils/yaml_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-from typing import Dict
+from typing import Any, Dict, Hashable
 
 import yaml
 
 
-def read_file(filename: str) -> Dict:
+def read_file(filename: str) -> Dict[Hashable, Any]:
     with open(filename, 'r', encoding='UTF-8') as file:
         return yaml.safe_load(file)
 
 
-def update_file(filename: str, content: Dict):
+def update_file(filename: str, content: Dict[Hashable, Any]) -> None:
     try:
         with open(filename, 'r', encoding='UTF-8') as file:
             file_content = yaml.safe_load(file)
     except FileNotFoundError:
         file_content = {}
 
     with open(filename, 'w', encoding='UTF-8') as file:
         file_content = _deep_update(file_content, content)
         yaml.safe_dump(file_content, file)
 
 
-def _deep_update(source, overrides):
+def _deep_update(source: Dict[Hashable, Any], overrides: Dict[Hashable, Any]) -> Dict[Hashable, Any]:
     for key, value in overrides.items():
         if isinstance(value, dict) and value:
             source[key] = _deep_update(source.get(key, {}), value)
         else:
             source[key] = overrides[key]
     return source
```

### Comparing `cycode-0.2.6.dev9/cycode/cli/zip_file.py` & `cycode-1.0.0/cycode/cli/zip_file.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 import os.path
 from io import BytesIO
+from typing import Optional
 from zipfile import ZIP_DEFLATED, ZipFile
 
 
 class InMemoryZip(object):
-    def __init__(self):
+    def __init__(self) -> None:
         # Create the in-memory file-like object
         self.in_memory_zip = BytesIO()
         self.zip = ZipFile(self.in_memory_zip, 'a', ZIP_DEFLATED, False)
 
-    def append(self, filename, unique_id, content):
+    def append(self, filename: str, unique_id: Optional[str], content: str) -> None:
         # Write the file to the in-memory zip
         if unique_id:
             filename = concat_unique_id(filename, unique_id)
 
         self.zip.writestr(filename, content)
 
-    def close(self):
+    def close(self) -> None:
         self.zip.close()
 
     # to bytes
     def read(self) -> bytes:
         self.in_memory_zip.seek(0)
         return self.in_memory_zip.read()
 
 
 def concat_unique_id(filename: str, unique_id: str) -> str:
     if filename.startswith(os.sep):
-        # remove leading slash to join path correctly
+        # remove leading slash to join the path correctly
         filename = filename[len(os.sep) :]
 
     return os.path.join(unique_id, filename)
```

### Comparing `cycode-0.2.6.dev9/cycode/cyclient/auth_client.py` & `cycode-1.0.0/cycode/cyclient/auth_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,28 +7,28 @@
 from . import models
 from .cycode_client import CycodeClient
 
 
 class AuthClient:
     AUTH_CONTROLLER_PATH = 'api/v1/device-auth'
 
-    def __init__(self):
+    def __init__(self) -> None:
         self.cycode_client = CycodeClient()
 
     def start_session(self, code_challenge: str) -> models.AuthenticationSession:
         path = f'{self.AUTH_CONTROLLER_PATH}/start'
         body = {'code_challenge': code_challenge}
         response = self.cycode_client.post(url_path=path, body=body)
         return self.parse_start_session_response(response)
 
     def get_api_token(self, session_id: str, code_verifier: str) -> Optional[models.ApiTokenGenerationPollingResponse]:
         path = f'{self.AUTH_CONTROLLER_PATH}/token'
         body = {'session_id': session_id, 'code_verifier': code_verifier}
         try:
-            response = self.cycode_client.post(url_path=path, body=body)
+            response = self.cycode_client.post(url_path=path, body=body, hide_response_content_log=True)
             return self.parse_api_token_polling_response(response)
         except (NetworkError, HttpUnauthorizedError) as e:
             return self.parse_api_token_polling_response(e.response)
         except Exception:
             return None
 
     @staticmethod
```

### Comparing `cycode-0.2.6.dev9/cycode/cyclient/config.py` & `cycode-1.0.0/cycode/cyclient/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 import os
 import sys
+from typing import Optional
 from urllib.parse import urlparse
 
 from cycode.cli import consts
 from cycode.cli.user_settings.configuration_manager import ConfigurationManager
 
 # set io encoding (for windows)
 from .config_dev import DEV_MODE_ENV_VAR_NAME, DEV_TENANT_ID_ENV_VAR_NAME
@@ -35,35 +36,38 @@
     DEV_MODE_ENV_VAR_NAME: 'False',
     consts.BATCH_SIZE_ENV_VAR_NAME: 20,
 }
 
 configuration = dict(DEFAULT_CONFIGURATION, **os.environ)
 
 
-def get_logger(logger_name=None):
+def get_logger(logger_name: Optional[str] = None) -> logging.Logger:
     logger = logging.getLogger(logger_name)
     level = _get_val_as_string(consts.LOGGING_LEVEL_ENV_VAR_NAME)
     level = level if level in logging._nameToLevel else int(level)
     logger.setLevel(level)
 
     return logger
 
 
-def _get_val_as_string(key):
+def _get_val_as_string(key: str) -> str:
     return configuration.get(key)
 
 
-def _get_val_as_bool(key, default=''):
+def _get_val_as_bool(key: str, default: str = '') -> bool:
     val = configuration.get(key, default)
     return val.lower() in ('true', '1')
 
 
-def _get_val_as_int(key):
+def _get_val_as_int(key: str) -> Optional[int]:
     val = configuration.get(key)
-    return int(val) if val is not None else None
+    if val:
+        return int(val)
+
+    return None
 
 
 logger = get_logger('cycode cli')
 
 configuration_manager = ConfigurationManager()
 
 cycode_api_url = configuration_manager.get_cycode_api_url()
```

### Comparing `cycode-0.2.6.dev9/cycode/cyclient/cycode_client_base.py` & `cycode-1.0.0/cycode/cyclient/cycode_client_base.py`

 * *Files 23% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
     return f'{app_name}/{version} (OS: {os}; Arch: {arch}; Python: {python_version}; InstallID: {install_id})'
 
 
 class CycodeClientBase:
     MANDATORY_HEADERS: ClassVar[Dict[str, str]] = {'User-Agent': get_cli_user_agent()}
 
-    def __init__(self, api_url: str):
+    def __init__(self, api_url: str) -> None:
         self.timeout = config.timeout
         self.api_url = api_url
 
     @staticmethod
     def reset_user_agent() -> None:
         CycodeClientBase.MANDATORY_HEADERS['User-Agent'] = get_cli_user_agent()
 
@@ -49,48 +49,55 @@
     def put(self, url_path: str, body: Optional[dict] = None, headers: Optional[dict] = None, **kwargs) -> Response:
         return self._execute(method='put', endpoint=url_path, json=body, headers=headers, **kwargs)
 
     def get(self, url_path: str, headers: Optional[dict] = None, **kwargs) -> Response:
         return self._execute(method='get', endpoint=url_path, headers=headers, **kwargs)
 
     def _execute(
-        self, method: str, endpoint: str, headers: Optional[dict] = None, without_auth: bool = False, **kwargs
+        self,
+        method: str,
+        endpoint: str,
+        headers: Optional[dict] = None,
+        without_auth: bool = False,
+        hide_response_content_log: bool = False,
+        **kwargs,
     ) -> Response:
         url = self.build_full_url(self.api_url, endpoint)
         logger.debug(f'Executing {method.upper()} request to {url}')
 
         try:
             headers = self.get_request_headers(headers, without_auth=without_auth)
             response = request(method=method, url=url, timeout=self.timeout, headers=headers, **kwargs)
 
-            logger.debug(f'Response {response.status_code} from {url}. Content: {response.text}')
+            content = 'HIDDEN' if hide_response_content_log else response.text
+            logger.debug(f'Response {response.status_code} from {url}. Content: {content}')
 
             response.raise_for_status()
             return response
         except Exception as e:
             self._handle_exception(e)
 
-    def get_request_headers(self, additional_headers: Optional[dict] = None, **kwargs) -> dict:
+    def get_request_headers(self, additional_headers: Optional[dict] = None, **kwargs) -> Dict[str, str]:
         if additional_headers is None:
             return self.MANDATORY_HEADERS.copy()
         return {**self.MANDATORY_HEADERS, **additional_headers}
 
     def build_full_url(self, url: str, endpoint: str) -> str:
         return f'{url}/{endpoint}'
 
-    def _handle_exception(self, e: Exception):
+    def _handle_exception(self, e: Exception) -> None:
         if isinstance(e, exceptions.Timeout):
             raise NetworkError(504, 'Timeout Error', e.response)
 
         if isinstance(e, exceptions.HTTPError):
             self._handle_http_exception(e)
         elif isinstance(e, exceptions.ConnectionError):
             raise NetworkError(502, 'Connection Error', e.response)
         else:
             raise e
 
     @staticmethod
-    def _handle_http_exception(e: exceptions.HTTPError):
+    def _handle_http_exception(e: exceptions.HTTPError) -> None:
         if e.response.status_code == 401:
             raise HttpUnauthorizedError(e.response.text, e.response)
 
         raise NetworkError(e.response.status_code, e.response.text, e.response)
```

### Comparing `cycode-0.2.6.dev9/cycode/cyclient/cycode_token_based_client.py` & `cycode-1.0.0/cycode/cyclient/cycode_token_based_client.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from .cycode_client import CycodeClient
 
 
 class CycodeTokenBasedClient(CycodeClient):
     """Send requests with api token"""
 
-    def __init__(self, client_id: str, client_secret: str):
+    def __init__(self, client_id: str, client_secret: str) -> None:
         super().__init__()
         self.client_secret = client_secret
         self.client_id = client_id
 
         self._api_token = None
         self._expires_in = None
 
@@ -31,21 +31,22 @@
             self.refresh_api_token()
 
     def refresh_api_token(self) -> None:
         auth_response = self.post(
             url_path='api/v1/auth/api-token',
             body={'clientId': self.client_id, 'secret': self.client_secret},
             without_auth=True,
+            hide_response_content_log=True,
         )
         auth_response_data = auth_response.json()
 
         self._api_token = auth_response_data['token']
         self._expires_in = arrow.utcnow().shift(seconds=auth_response_data['expires_in'] * 0.8)
 
-    def get_request_headers(self, additional_headers: Optional[dict] = None, without_auth=False) -> dict:
+    def get_request_headers(self, additional_headers: Optional[dict] = None, without_auth: bool = False) -> dict:
         headers = super().get_request_headers(additional_headers=additional_headers)
 
         if not without_auth:
             headers = self._add_auth_header(headers)
 
         return headers
```

### Comparing `cycode-0.2.6.dev9/cycode/cyclient/models.py` & `cycode-1.0.0/cycode/cyclient/models.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from dataclasses import dataclass
-from typing import Dict, List, Optional
+from typing import Any, Dict, List, Optional
 
 from marshmallow import EXCLUDE, Schema, fields, post_load
 
 
 class Detection(Schema):
     def __init__(
         self,
         detection_type_id: str,
         type: str,
         message: str,
         detection_details: dict,
         detection_rule_id: str,
         severity: Optional[str] = None,
-    ):
+    ) -> None:
         super().__init__()
         self.message = message
         self.type = type
         self.severity = severity
         self.detection_type_id = detection_type_id
         self.detection_details = detection_details
         self.detection_rule_id = detection_rule_id
@@ -41,20 +41,20 @@
     severity = fields.String(missing='High')
     # TODO(MarshalX): Remove "missing" arg when IaC and Secrets scans will have classifications
     detection_type_id = fields.String()
     detection_details = fields.Dict()
     detection_rule_id = fields.String()
 
     @post_load
-    def build_dto(self, data, **kwargs):
+    def build_dto(self, data: Dict[str, Any], **_) -> Detection:
         return Detection(**data)
 
 
 class DetectionsPerFile(Schema):
-    def __init__(self, file_name: str, detections: List[Detection], commit_id: Optional[str] = None):
+    def __init__(self, file_name: str, detections: List[Detection], commit_id: Optional[str] = None) -> None:
         super().__init__()
         self.file_name = file_name
         self.detections = detections
         self.commit_id = commit_id
 
 
 class DetectionsPerFileSchema(Schema):
@@ -62,27 +62,27 @@
         unknown = EXCLUDE
 
     file_name = fields.String()
     detections = fields.List(fields.Nested(DetectionSchema))
     commit_id = fields.String(allow_none=True)
 
     @post_load
-    def build_dto(self, data, **kwargs):
+    def build_dto(self, data: Dict[str, Any], **_) -> 'DetectionsPerFile':
         return DetectionsPerFile(**data)
 
 
 class ZippedFileScanResult(Schema):
     def __init__(
         self,
         did_detect: bool,
         detections_per_file: List[DetectionsPerFile],
         report_url: Optional[str] = None,
         scan_id: Optional[str] = None,
         err: Optional[str] = None,
-    ):
+    ) -> None:
         super().__init__()
         self.did_detect = did_detect
         self.detections_per_file = detections_per_file
         self.scan_id = scan_id
         self.report_url = report_url
         self.err = err
 
@@ -94,26 +94,26 @@
     did_detect = fields.Boolean()
     scan_id = fields.String()
     report_url = fields.String(allow_none=True)
     detections_per_file = fields.List(fields.Nested(DetectionsPerFileSchema))
     err = fields.String()
 
     @post_load
-    def build_dto(self, data, **kwargs):
+    def build_dto(self, data: Dict[str, Any], **_) -> 'ZippedFileScanResult':
         return ZippedFileScanResult(**data)
 
 
 class ScanResult(Schema):
     def __init__(
         self,
         did_detect: bool,
         scan_id: Optional[str] = None,
         detections: Optional[List[Detection]] = None,
         err: Optional[str] = None,
-    ):
+    ) -> None:
         super().__init__()
         self.did_detect = did_detect
         self.scan_id = scan_id
         self.detections = detections
         self.err = err
 
 
@@ -123,48 +123,48 @@
 
     did_detect = fields.Boolean()
     scan_id = fields.String()
     detections = fields.List(fields.Nested(DetectionSchema), required=False, allow_none=True)
     err = fields.String()
 
     @post_load
-    def build_dto(self, data, **kwargs):
+    def build_dto(self, data: Dict[str, Any], **_) -> 'ScanResult':
         return ScanResult(**data)
 
 
 class ScanInitializationResponse(Schema):
-    def __init__(self, scan_id: Optional[str] = None, err: Optional[str] = None):
+    def __init__(self, scan_id: Optional[str] = None, err: Optional[str] = None) -> None:
         super().__init__()
         self.scan_id = scan_id
         self.err = err
 
 
 class ScanInitializationResponseSchema(Schema):
     class Meta:
         unknown = EXCLUDE
 
     scan_id = fields.String()
     err = fields.String()
 
     @post_load
-    def build_dto(self, data, **kwargs):
+    def build_dto(self, data: Dict[str, Any], **_) -> 'ScanInitializationResponse':
         return ScanInitializationResponse(**data)
 
 
 class ScanDetailsResponse(Schema):
     def __init__(
         self,
         id: Optional[str] = None,
         scan_status: Optional[str] = None,
         results_count: Optional[int] = None,
         metadata: Optional[str] = None,
         message: Optional[str] = None,
         scan_update_at: Optional[str] = None,
         err: Optional[str] = None,
-    ):
+    ) -> None:
         super().__init__()
         self.id = id
         self.scan_status = scan_status
         self.detections_count = results_count
         self.metadata = metadata
         self.message = message
         self.scan_update_at = scan_update_at
@@ -180,53 +180,53 @@
     results_count = fields.Integer(allow_none=True)
     metadata = fields.String(allow_none=True)
     message = fields.String(allow_none=True)
     scan_update_at = fields.String(allow_none=True)
     err = fields.String()
 
     @post_load
-    def build_dto(self, data, **kwargs):
+    def build_dto(self, data: Dict[str, Any], **_) -> 'ScanDetailsResponse':
         return ScanDetailsResponse(**data)
 
 
 class K8SResource:
-    def __init__(self, name: str, resource_type: str, namespace: str, content: Dict):
+    def __init__(self, name: str, resource_type: str, namespace: str, content: Dict) -> None:
         super().__init__()
         self.name = name
         self.type = resource_type
         self.namespace = namespace
         self.content = content
         self.internal_metadata = None
         self.schema = K8SResourceSchema()
 
-    def to_json(self):
+    def to_json(self) -> dict:  # FIXME(MarshalX): rename to to_dict?
         return self.schema.dump(self)
 
 
 class InternalMetadata:
-    def __init__(self, root_entity_name: str, root_entity_type: str):
+    def __init__(self, root_entity_name: str, root_entity_type: str) -> None:
         super().__init__()
         self.root_entity_name = root_entity_name
         self.root_entity_type = root_entity_type
         self.schema = InternalMetadataSchema()
 
-    def to_json(self):
+    def to_json(self) -> dict:  # FIXME(MarshalX): rename to to_dict?
         return self.schema.dump(self)
 
 
 class ResourcesCollection:
-    def __init__(self, resource_type: str, namespace: str, resources: List[K8SResource], total_count: int):
+    def __init__(self, resource_type: str, namespace: str, resources: List[K8SResource], total_count: int) -> None:
         super().__init__()
         self.type = resource_type
         self.namespace = namespace
         self.resources = resources
         self.total_count = total_count
         self.schema = ResourcesCollectionSchema()
 
-    def to_json(self):
+    def to_json(self) -> dict:  # FIXME(MarshalX): rename to to_dict?
         return self.schema.dump(self)
 
 
 class InternalMetadataSchema(Schema):
     root_entity_name = fields.String()
     root_entity_type = fields.String()
 
@@ -243,42 +243,42 @@
     type = fields.String()
     namespace = fields.String()
     resources = fields.List(fields.Nested(K8SResourceSchema))
     total_count = fields.Integer()
 
 
 class OwnerReference:
-    def __init__(self, name: str, kind: str):
+    def __init__(self, name: str, kind: str) -> None:
         super().__init__()
         self.name = name
         self.kind = kind
 
-    def __str__(self):
+    def __str__(self) -> str:
         return 'Name: {0}, Kind: {1}'.format(self.name, self.kind)
 
 
 class AuthenticationSession(Schema):
-    def __init__(self, session_id: str):
+    def __init__(self, session_id: str) -> None:
         super().__init__()
         self.session_id = session_id
 
 
 class AuthenticationSessionSchema(Schema):
     class Meta:
         unknown = EXCLUDE
 
     session_id = fields.String()
 
     @post_load
-    def build_dto(self, data, **kwargs):
+    def build_dto(self, data: Dict[str, Any], **_) -> 'AuthenticationSession':
         return AuthenticationSession(**data)
 
 
 class ApiToken(Schema):
-    def __init__(self, client_id: str, secret: str, description: str):
+    def __init__(self, client_id: str, secret: str, description: str) -> None:
         super().__init__()
         self.client_id = client_id
         self.secret = secret
         self.description = description
 
 
 class ApiTokenSchema(Schema):
@@ -286,45 +286,45 @@
         unknown = EXCLUDE
 
     client_id = fields.String(data_key='clientId')
     secret = fields.String()
     description = fields.String()
 
     @post_load
-    def build_dto(self, data, **kwargs):
+    def build_dto(self, data: Dict[str, Any], **_) -> 'ApiToken':
         return ApiToken(**data)
 
 
 class ApiTokenGenerationPollingResponse(Schema):
-    def __init__(self, status: str, api_token):
+    def __init__(self, status: str, api_token: 'ApiToken') -> None:
         super().__init__()
         self.status = status
         self.api_token = api_token
 
 
 class ApiTokenGenerationPollingResponseSchema(Schema):
     class Meta:
         unknown = EXCLUDE
 
     status = fields.String()
     api_token = fields.Nested(ApiTokenSchema, allow_none=True)
 
     @post_load
-    def build_dto(self, data, **kwargs):
+    def build_dto(self, data: Dict[str, Any], **_) -> 'ApiTokenGenerationPollingResponse':
         return ApiTokenGenerationPollingResponse(**data)
 
 
 class UserAgentOptionScheme(Schema):
     app_name = fields.String(required=True)  # ex. vscode_extension
     app_version = fields.String(required=True)  # ex. 0.2.3
     env_name = fields.String(required=True)  # ex.: Visual Studio Code
     env_version = fields.String(required=True)  # ex. 1.78.2
 
     @post_load
-    def build_dto(self, data: dict, **_) -> 'UserAgentOption':
+    def build_dto(self, data: Dict[str, Any], **_) -> 'UserAgentOption':
         return UserAgentOption(**data)
 
 
 @dataclass
 class UserAgentOption:
     app_name: str
     app_version: str
```

### Comparing `cycode-0.2.6.dev9/cycode/cyclient/scan_client.py` & `cycode-1.0.0/cycode/cyclient/scan_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,42 +7,44 @@
 
 from . import models
 from .cycode_client_base import CycodeClientBase
 from .scan_config.scan_config_base import ScanConfigBase
 
 
 class ScanClient:
-    def __init__(self, scan_cycode_client: CycodeClientBase, scan_config: ScanConfigBase):
+    def __init__(
+        self, scan_cycode_client: CycodeClientBase, scan_config: ScanConfigBase, hide_response_log: bool = True
+    ) -> None:
         self.scan_cycode_client = scan_cycode_client
         self.scan_config = scan_config
+
         self.SCAN_CONTROLLER_PATH = 'api/v1/scan'
         self.DETECTIONS_SERVICE_CONTROLLER_PATH = 'api/v1/detections'
 
+        self._hide_response_log = hide_response_log
+
     def content_scan(self, scan_type: str, file_name: str, content: str, is_git_diff: bool = True) -> models.ScanResult:
         path = f'{self.scan_config.get_service_name(scan_type)}/{self.SCAN_CONTROLLER_PATH}/content'
         body = {'name': file_name, 'content': content, 'is_git_diff': is_git_diff}
-        response = self.scan_cycode_client.post(url_path=path, body=body)
-        return self.parse_scan_response(response)
-
-    def file_scan(self, scan_type: str, path: str) -> models.ScanResult:
-        url_path = f'{self.scan_config.get_service_name(scan_type)}/{self.SCAN_CONTROLLER_PATH}'
-        files = {'file': open(path, 'rb')}  # noqa: SIM115 requests lib should care about closing
-        response = self.scan_cycode_client.post(url_path=url_path, files=files)
+        response = self.scan_cycode_client.post(
+            url_path=path, body=body, hide_response_content_log=self._hide_response_log
+        )
         return self.parse_scan_response(response)
 
     def zipped_file_scan(
         self, scan_type: str, zip_file: InMemoryZip, scan_id: str, scan_parameters: dict, is_git_diff: bool = False
     ) -> models.ZippedFileScanResult:
         url_path = f'{self.scan_config.get_service_name(scan_type)}/{self.SCAN_CONTROLLER_PATH}/zipped-file'
         files = {'file': ('multiple_files_scan.zip', zip_file.read())}
 
         response = self.scan_cycode_client.post(
             url_path=url_path,
             data={'scan_id': scan_id, 'is_git_diff': is_git_diff, 'scan_parameters': json.dumps(scan_parameters)},
             files=files,
+            hide_response_content_log=self._hide_response_log,
         )
 
         return self.parse_zipped_file_scan_response(response)
 
     def zipped_file_scan_async(
         self, zip_file: InMemoryZip, scan_type: str, scan_parameters: dict, is_git_diff: bool = False
     ) -> models.ScanInitializationResponse:
@@ -92,15 +94,17 @@
 
         page_number = 0
         last_response_size = 0
         while page_number == 0 or last_response_size == page_size:
             params['page_size'] = page_size
             params['page_number'] = page_number
 
-            response = self.scan_cycode_client.get(url_path=url_path, params=params).json()
+            response = self.scan_cycode_client.get(
+                url_path=url_path, params=params, hide_response_content_log=self._hide_response_log
+            ).json()
             detections.extend(response)
 
             page_number += 1
             last_response_size = len(response)
 
         return detections
 
@@ -112,18 +116,20 @@
     def commit_range_zipped_file_scan(
         self, scan_type: str, zip_file: InMemoryZip, scan_id: str
     ) -> models.ZippedFileScanResult:
         url_path = (
             f'{self.scan_config.get_service_name(scan_type)}/{self.SCAN_CONTROLLER_PATH}/commit-range-zipped-file'
         )
         files = {'file': ('multiple_files_scan.zip', zip_file.read())}
-        response = self.scan_cycode_client.post(url_path=url_path, data={'scan_id': scan_id}, files=files)
+        response = self.scan_cycode_client.post(
+            url_path=url_path, data={'scan_id': scan_id}, files=files, hide_response_content_log=self._hide_response_log
+        )
         return self.parse_zipped_file_scan_response(response)
 
-    def report_scan_status(self, scan_type: str, scan_id: str, scan_status: dict):
+    def report_scan_status(self, scan_type: str, scan_id: str, scan_status: dict) -> None:
         url_path = f'{self.scan_config.get_service_name(scan_type)}/{self.SCAN_CONTROLLER_PATH}/{scan_id}/status'
         self.scan_cycode_client.post(url_path=url_path, body=scan_status)
 
     @staticmethod
     def parse_scan_response(response: Response) -> models.ScanResult:
         return models.ScanResultSchema().load(response.json())
```

### Comparing `cycode-0.2.6.dev9/cycode/cyclient/scan_config/scan_config_creator.py` & `cycode-1.0.0/cycode/cyclient/scan_config/scan_config_creator.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 from cycode.cyclient.config_dev import DEV_CYCODE_API_URL
 from cycode.cyclient.cycode_dev_based_client import CycodeDevBasedClient
 from cycode.cyclient.cycode_token_based_client import CycodeTokenBasedClient
 from cycode.cyclient.scan_client import ScanClient
 from cycode.cyclient.scan_config.scan_config_base import DefaultScanConfig, DevScanConfig
 
 
-def create_scan_client(client_id: str, client_secret: str) -> ScanClient:
+def create_scan_client(client_id: str, client_secret: str, hide_response_log: bool) -> ScanClient:
     if dev_mode:
         scan_cycode_client, scan_config = create_scan_for_dev_env()
     else:
         scan_cycode_client, scan_config = create_scan(client_id, client_secret)
 
-    return ScanClient(scan_cycode_client=scan_cycode_client, scan_config=scan_config)
+    return ScanClient(scan_cycode_client, scan_config, hide_response_log)
 
 
 def create_scan(client_id: str, client_secret: str) -> Tuple[CycodeTokenBasedClient, DefaultScanConfig]:
     scan_cycode_client = CycodeTokenBasedClient(client_id, client_secret)
     scan_config = DefaultScanConfig()
     return scan_cycode_client, scan_config
```

### Comparing `cycode-0.2.6.dev9/PKG-INFO` & `cycode-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: cycode
-Version: 0.2.6.dev9
-Summary: Perform secrets/iac scans for your sources using Cycode's engine
+Version: 1.0.0
+Summary: Boost security in your dev lifecycle via SAST, SCA, Secrets & IaC scanning.
 Home-page: https://github.com/cycodehq-public/cycode-cli
 License: MIT
 Keywords: secret-scan,cycode,devops,token,secret,security,cycode,code
 Author: Cycode
 Author-email: support@cycode.com
 Requires-Python: >=3.7,<3.12
 Classifier: Development Status :: 5 - Production/Stable
@@ -27,14 +27,15 @@
 Requires-Dist: colorama (>=0.4.3,<0.5.0)
 Requires-Dist: gitpython (>=3.1.30,<3.2.0)
 Requires-Dist: marshmallow (>=3.8.0,<3.9.0)
 Requires-Dist: pathspec (>=0.11.1,<0.12.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.24,<3.0)
 Requires-Dist: texttable (>=1.6.7,<1.7.0)
+Requires-Dist: urllib3 (==1.26.16)
 Project-URL: Repository, https://github.com/cycodehq-public/cycode-cli
 Description-Content-Type: text/markdown
 
 # Cycode CLI User Guide
 
 The Cycode Command Line Interface (CLI) is an application you can install on your local machine which can scan your locally stored repositories for any secrets or infrastructure as code misconfigurations.
 
@@ -245,27 +246,27 @@
 > A successful hook installation will result in the message:<br/>
 `Pre-commit installed at .git/hooks/pre-commit`
 
 # Cycode CLI Commands
 
 The following are the options and commands available with the Cycode CLI application:
 
-| Option                         | Description                                                       |
-|--------------------------------|-------------------------------------------------------------------|
-| `--output [text\|json\|table]` | Specify the output (`text`/`json`/`table`). The default is `text` |
-| `-v`, `--verbose`              | Show detailed logs                                                |
-| `--version`                    | Show the version and exit.                                        |
-| `--help`                       | Show options for given command.                                   |
-
-| Command                             | Description |
-|-------------------------------------|-------------|
-| [auth](#use-auth-command)           | Authenticates your machine to associate CLI with your Cycode account. |
-| [configure](#use-configure-command) | Initial command to authenticate your CLI client with Cycode using client ID and client secret. |
-| [ignore](#ingoring-scan-results)    | Ignore a specific value, path or rule ID |
-| [scan](#running-a-scan)             | Scan content for secrets/IaC/SCA/SAST violations. You need to specify which scan type: `ci`/`commit_history`/`path`/`repository`/etc |
+| Option                               | Description                                                        |
+|--------------------------------------|--------------------------------------------------------------------|
+| `-o`, `--output [text\|json\|table]` | Specify the output (`text`/`json`/`table`). The default is `text`. |
+| `-v`, `--verbose`                    | Show detailed logs.                                                |
+| `--help`                             | Show options for given command.                                    |
+
+| Command                             | Description                                                                                                                           |
+|-------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------|
+| [auth](#use-auth-command)           | Authenticates your machine to associate CLI with your Cycode account.                                                                 |
+| [configure](#use-configure-command) | Initial command to authenticate your CLI client with Cycode using client ID and client secret.                                        |
+| [ignore](#ingoring-scan-results)    | Ignore a specific value, path or rule ID.                                                                                             |
+| [scan](#running-a-scan)             | Scan content for secrets/IaC/SCA/SAST violations. You need to specify which scan type: `ci`/`commit_history`/`path`/`repository`/etc. |
+| version                             | Show the version and exit.                                                                                                            |
 
 # Running a Scan
 
 The Cycode CLI application offers several types of scans so that you can choose the option that best fits your case. The following are the current options and commands available:
 
 | Option                               | Description                                                                |
 |--------------------------------------|----------------------------------------------------------------------------|
@@ -587,14 +588,15 @@
 
 # Ignoring Scan Results
 
 Ignore rules can be added to ignore specific secret values, specific SHA512 values, specific paths, and specific Cycode secret and IaC rule IDs. This will cause the scan to not alert these values. The ignore rules are written and saved locally in the `./.cycode/config.yaml` file.
 
 > :warning: **Warning**<br/>
 > Adding values to be ignored should be done with careful consideration of the values, paths, and policies to ensure that the scans will pick up true positives.
+
 The following are the options available for the `cycode ignore` command:
 
 | Option                          | Description |
 |---------------------------------|-------------|
 | `--by-value TEXT`               | Ignore a specific value while scanning for secrets. See [Ignoring a Secret Value](#ignoring-a-secret-value) for more details. |
 | `--by-sha TEXT`                 | Ignore a specific SHA512 representation of a string while scanning for secrets. See [Ignoring a Secret SHA Value](#ignoring-a-secret-sha-value) for more details. |
 | `--by-path TEXT`                | Avoid scanning a specific path. Need to specify scan type. See [Ignoring a Path](#ignoring-a-path) for more details. |
```

