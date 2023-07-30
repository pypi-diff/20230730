# Comparing `tmp/cli_command_parser-2023.7.29.tar.gz` & `tmp/cli_command_parser-2023.7.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cli_command_parser-2023.7.29.tar", last modified: Sat Jul 29 13:18:34 2023, max compression
+gzip compressed data, was "cli_command_parser-2023.7.30.tar", last modified: Sun Jul 30 20:03:19 2023, max compression
```

## Comparing `cli_command_parser-2023.7.29.tar` & `cli_command_parser-2023.7.30.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 13:18:34.900525 cli_command_parser-2023.7.29/
--rw-rw-rw-   0        0        0    11341 2022-09-17 20:57:36.000000 cli_command_parser-2023.7.29/LICENSE
--rw-rw-rw-   0        0        0       64 2022-09-17 20:57:36.000000 cli_command_parser-2023.7.29/MANIFEST.in
--rw-rw-rw-   0        0        0     5611 2023-07-29 13:18:34.901523 cli_command_parser-2023.7.29/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-29 13:18:34.694523 cli_command_parser-2023.7.29/lib/
-drwxrwxrwx   0        0        0        0 2023-07-29 13:18:34.778522 cli_command_parser-2023.7.29/lib/cli_command_parser/
--rw-rw-rw-   0        0        0     1158 2023-05-29 16:32:28.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/__init__.py
--rw-rw-rw-   0        0        0      114 2022-09-17 20:57:36.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/__main__.py
--rw-rw-rw-   0        0        0      295 2023-07-29 13:18:24.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/__version__.py
--rw-rw-rw-   0        0        0     2430 2023-06-14 11:32:55.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/annotations.py
--rw-rw-rw-   0        0        0    19228 2023-06-14 11:32:55.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/command_parameters.py
--rw-rw-rw-   0        0        0    12838 2023-07-29 13:17:30.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/commands.py
--rw-rw-rw-   0        0        0     5150 2023-05-02 11:35:36.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/compat.py
--rw-rw-rw-   0        0        0    18449 2023-05-20 18:50:11.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/config.py
--rw-rw-rw-   0        0        0    19091 2023-07-29 13:17:30.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/context.py
-drwxrwxrwx   0        0        0        0 2023-07-29 13:18:34.816522 cli_command_parser-2023.7.29/lib/cli_command_parser/conversion/
--rw-rw-rw-   0        0        0      234 2023-04-06 21:32:03.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/conversion/__init__.py
--rw-rw-rw-   0        0        0       54 2023-04-06 21:32:03.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/conversion/__main__.py
--rw-rw-rw-   0        0        0    12711 2023-05-08 11:55:32.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/conversion/argparse_ast.py
--rw-rw-rw-   0        0        0     1356 2023-04-06 21:32:03.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/conversion/argparse_utils.py
--rw-rw-rw-   0        0        0    24279 2023-05-08 11:55:32.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/conversion/command_builder.py
--rw-rw-rw-   0        0        0     1660 2023-04-06 21:32:03.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/conversion/utils.py
--rw-rw-rw-   0        0        0     7375 2023-05-08 11:55:32.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/conversion/visitor.py
--rw-rw-rw-   0        0        0    12518 2023-05-29 16:32:28.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/core.py
--rw-rw-rw-   0        0        0    15359 2023-05-13 19:45:03.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/documentation.py
--rw-rw-rw-   0        0        0     6787 2023-04-29 17:20:11.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/error_handling.py
--rw-rw-rw-   0        0        0     8297 2023-05-29 16:32:28.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-07-29 13:18:34.830522 cli_command_parser-2023.7.29/lib/cli_command_parser/formatting/
--rw-rw-rw-   0        0        0        0 2022-09-17 20:57:36.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/formatting/__init__.py
--rw-rw-rw-   0        0        0     9604 2023-07-29 13:17:30.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/formatting/commands.py
--rw-rw-rw-   0        0        0    20856 2023-07-29 13:17:30.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/formatting/params.py
--rw-rw-rw-   0        0        0     9377 2023-05-13 19:45:03.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/formatting/restructured_text.py
--rw-rw-rw-   0        0        0     5445 2023-05-13 19:45:03.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/formatting/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-29 13:18:34.863523 cli_command_parser-2023.7.29/lib/cli_command_parser/inputs/
--rw-rw-rw-   0        0        0     2591 2023-05-14 19:11:26.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/inputs/__init__.py
--rw-rw-rw-   0        0        0     1550 2023-05-20 18:50:11.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/inputs/base.py
--rw-rw-rw-   0        0        0     6582 2023-05-20 18:50:11.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/inputs/choices.py
--rw-rw-rw-   0        0        0     1113 2023-04-08 14:58:49.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/inputs/exceptions.py
--rw-rw-rw-   0        0        0     8897 2023-05-20 18:50:11.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/inputs/files.py
--rw-rw-rw-   0        0        0     8341 2023-05-20 18:50:11.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/inputs/numeric.py
--rw-rw-rw-   0        0        0     7601 2023-05-20 18:50:11.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/inputs/patterns.py
--rw-rw-rw-   0        0        0    22732 2023-05-20 18:50:11.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/inputs/time.py
--rw-rw-rw-   0        0        0     6523 2023-05-20 18:50:11.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/inputs/utils.py
--rw-rw-rw-   0        0        0    13618 2023-05-20 18:50:11.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/metadata.py
--rw-rw-rw-   0        0        0     8144 2023-05-29 16:32:28.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/nargs.py
-drwxrwxrwx   0        0        0        0 2023-07-29 13:18:34.900525 cli_command_parser-2023.7.29/lib/cli_command_parser/parameters/
--rw-rw-rw-   0        0        0      313 2023-06-14 11:32:55.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/parameters/__init__.py
--rw-rw-rw-   0        0        0    16944 2023-06-14 11:32:55.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/parameters/actions.py
--rw-rw-rw-   0        0        0    22558 2023-06-14 11:32:55.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/parameters/base.py
--rw-rw-rw-   0        0        0    16514 2023-06-14 11:32:55.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/parameters/choice_map.py
--rw-rw-rw-   0        0        0    10656 2023-05-13 19:45:03.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/parameters/groups.py
--rw-rw-rw-   0        0        0     8242 2023-05-21 20:53:58.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/parameters/option_strings.py
--rw-rw-rw-   0        0        0    24296 2023-06-14 11:32:55.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/parameters/options.py
--rw-rw-rw-   0        0        0      896 2023-05-29 16:32:28.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/parameters/pass_thru.py
--rw-rw-rw-   0        0        0     4422 2023-05-29 16:32:28.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/parameters/positionals.py
--rw-rw-rw-   0        0        0    11295 2023-05-21 20:53:58.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/parse_tree.py
--rw-rw-rw-   0        0        0    16701 2023-06-14 11:32:55.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/parser.py
--rw-rw-rw-   0        0        0    12301 2023-06-14 11:32:55.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/testing.py
--rw-rw-rw-   0        0        0     1882 2023-05-29 16:32:28.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/typing.py
--rw-rw-rw-   0        0        0     5216 2023-05-29 16:32:28.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-29 13:18:34.790524 cli_command_parser-2023.7.29/lib/cli_command_parser.egg-info/
--rw-rw-rw-   0        0        0     5611 2023-07-29 13:18:34.000000 cli_command_parser-2023.7.29/lib/cli_command_parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2367 2023-07-29 13:18:34.000000 cli_command_parser-2023.7.29/lib/cli_command_parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 13:18:34.000000 cli_command_parser-2023.7.29/lib/cli_command_parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       81 2023-07-29 13:18:34.000000 cli_command_parser-2023.7.29/lib/cli_command_parser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-07-29 13:18:34.000000 cli_command_parser-2023.7.29/lib/cli_command_parser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      316 2023-05-02 11:35:36.000000 cli_command_parser-2023.7.29/pyproject.toml
--rw-rw-rw-   0        0        0     4414 2023-05-02 11:35:36.000000 cli_command_parser-2023.7.29/readme.rst
--rw-rw-rw-   0        0        0      111 2023-04-10 12:30:46.000000 cli_command_parser-2023.7.29/requirements-dev.txt
--rw-rw-rw-   0        0        0     1293 2023-07-29 13:18:34.904523 cli_command_parser-2023.7.29/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-30 20:03:18.998197 cli_command_parser-2023.7.30/
+-rw-rw-rw-   0        0        0    11341 2022-09-17 20:57:36.000000 cli_command_parser-2023.7.30/LICENSE
+-rw-rw-rw-   0        0        0       64 2022-09-17 20:57:36.000000 cli_command_parser-2023.7.30/MANIFEST.in
+-rw-rw-rw-   0        0        0     5611 2023-07-30 20:03:18.998197 cli_command_parser-2023.7.30/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-30 20:03:18.844197 cli_command_parser-2023.7.30/lib/
+drwxrwxrwx   0        0        0        0 2023-07-30 20:03:18.905198 cli_command_parser-2023.7.30/lib/cli_command_parser/
+-rw-rw-rw-   0        0        0     1158 2023-05-29 16:32:28.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/__init__.py
+-rw-rw-rw-   0        0        0      114 2022-09-17 20:57:36.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/__main__.py
+-rw-rw-rw-   0        0        0      295 2023-07-30 20:03:08.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/__version__.py
+-rw-rw-rw-   0        0        0     2430 2023-06-14 11:32:55.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/annotations.py
+-rw-rw-rw-   0        0        0    19228 2023-06-14 11:32:55.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/command_parameters.py
+-rw-rw-rw-   0        0        0    12852 2023-07-30 20:03:01.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/commands.py
+-rw-rw-rw-   0        0        0     5101 2023-07-30 20:03:01.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/compat.py
+-rw-rw-rw-   0        0        0    18620 2023-07-30 20:03:01.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/config.py
+-rw-rw-rw-   0        0        0    19945 2023-07-30 20:03:01.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/context.py
+drwxrwxrwx   0        0        0        0 2023-07-30 20:03:18.943197 cli_command_parser-2023.7.30/lib/cli_command_parser/conversion/
+-rw-rw-rw-   0        0        0      234 2023-04-06 21:32:03.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/conversion/__init__.py
+-rw-rw-rw-   0        0        0       54 2023-04-06 21:32:03.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/conversion/__main__.py
+-rw-rw-rw-   0        0        0    12711 2023-05-08 11:55:32.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/conversion/argparse_ast.py
+-rw-rw-rw-   0        0        0     1356 2023-04-06 21:32:03.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/conversion/argparse_utils.py
+-rw-rw-rw-   0        0        0    24279 2023-05-08 11:55:32.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/conversion/command_builder.py
+-rw-rw-rw-   0        0        0     1660 2023-04-06 21:32:03.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/conversion/utils.py
+-rw-rw-rw-   0        0        0     7375 2023-05-08 11:55:32.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/conversion/visitor.py
+-rw-rw-rw-   0        0        0    12518 2023-05-29 16:32:28.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/core.py
+-rw-rw-rw-   0        0        0    15359 2023-05-13 19:45:03.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/documentation.py
+-rw-rw-rw-   0        0        0     6787 2023-04-29 17:20:11.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/error_handling.py
+-rw-rw-rw-   0        0        0     8297 2023-05-29 16:32:28.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-07-30 20:03:18.957196 cli_command_parser-2023.7.30/lib/cli_command_parser/formatting/
+-rw-rw-rw-   0        0        0        0 2022-09-17 20:57:36.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/formatting/__init__.py
+-rw-rw-rw-   0        0        0     9604 2023-07-29 13:17:30.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/formatting/commands.py
+-rw-rw-rw-   0        0        0    21721 2023-07-30 20:03:01.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/formatting/params.py
+-rw-rw-rw-   0        0        0     9377 2023-05-13 19:45:03.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/formatting/restructured_text.py
+-rw-rw-rw-   0        0        0     5306 2023-07-30 20:03:01.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/formatting/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-30 20:03:18.985197 cli_command_parser-2023.7.30/lib/cli_command_parser/inputs/
+-rw-rw-rw-   0        0        0     2591 2023-05-14 19:11:26.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/inputs/__init__.py
+-rw-rw-rw-   0        0        0     1550 2023-05-20 18:50:11.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/inputs/base.py
+-rw-rw-rw-   0        0        0     6582 2023-05-20 18:50:11.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/inputs/choices.py
+-rw-rw-rw-   0        0        0     1113 2023-04-08 14:58:49.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/inputs/exceptions.py
+-rw-rw-rw-   0        0        0     8897 2023-05-20 18:50:11.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/inputs/files.py
+-rw-rw-rw-   0        0        0     8341 2023-05-20 18:50:11.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/inputs/numeric.py
+-rw-rw-rw-   0        0        0     7601 2023-05-20 18:50:11.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/inputs/patterns.py
+-rw-rw-rw-   0        0        0    22732 2023-05-20 18:50:11.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/inputs/time.py
+-rw-rw-rw-   0        0        0     6523 2023-05-20 18:50:11.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/inputs/utils.py
+-rw-rw-rw-   0        0        0    13618 2023-05-20 18:50:11.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/metadata.py
+-rw-rw-rw-   0        0        0     8144 2023-05-29 16:32:28.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/nargs.py
+drwxrwxrwx   0        0        0        0 2023-07-30 20:03:18.998197 cli_command_parser-2023.7.30/lib/cli_command_parser/parameters/
+-rw-rw-rw-   0        0        0      313 2023-06-14 11:32:55.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/parameters/__init__.py
+-rw-rw-rw-   0        0        0    17329 2023-07-30 20:03:01.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/parameters/actions.py
+-rw-rw-rw-   0        0        0    25178 2023-07-30 20:03:01.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/parameters/base.py
+-rw-rw-rw-   0        0        0    16732 2023-07-30 20:03:01.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/parameters/choice_map.py
+-rw-rw-rw-   0        0        0    10656 2023-05-13 19:45:03.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/parameters/groups.py
+-rw-rw-rw-   0        0        0     8242 2023-05-21 20:53:58.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/parameters/option_strings.py
+-rw-rw-rw-   0        0        0    25683 2023-07-30 20:03:01.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/parameters/options.py
+-rw-rw-rw-   0        0        0      896 2023-05-29 16:32:28.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/parameters/pass_thru.py
+-rw-rw-rw-   0        0        0     4543 2023-07-30 20:03:01.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/parameters/positionals.py
+-rw-rw-rw-   0        0        0    11295 2023-05-21 20:53:58.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/parse_tree.py
+-rw-rw-rw-   0        0        0    16709 2023-07-30 20:03:01.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/parser.py
+-rw-rw-rw-   0        0        0    12348 2023-07-30 20:03:01.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/testing.py
+-rw-rw-rw-   0        0        0     1977 2023-07-30 20:03:01.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/typing.py
+-rw-rw-rw-   0        0        0     5695 2023-07-30 20:03:01.000000 cli_command_parser-2023.7.30/lib/cli_command_parser/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-30 20:03:18.917196 cli_command_parser-2023.7.30/lib/cli_command_parser.egg-info/
+-rw-rw-rw-   0        0        0     5611 2023-07-30 20:03:18.000000 cli_command_parser-2023.7.30/lib/cli_command_parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2367 2023-07-30 20:03:18.000000 cli_command_parser-2023.7.30/lib/cli_command_parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 20:03:18.000000 cli_command_parser-2023.7.30/lib/cli_command_parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       81 2023-07-30 20:03:18.000000 cli_command_parser-2023.7.30/lib/cli_command_parser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-07-30 20:03:18.000000 cli_command_parser-2023.7.30/lib/cli_command_parser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      316 2023-05-02 11:35:36.000000 cli_command_parser-2023.7.30/pyproject.toml
+-rw-rw-rw-   0        0        0     4414 2023-05-02 11:35:36.000000 cli_command_parser-2023.7.30/readme.rst
+-rw-rw-rw-   0        0        0      111 2023-04-10 12:30:46.000000 cli_command_parser-2023.7.30/requirements-dev.txt
+-rw-rw-rw-   0        0        0     1293 2023-07-30 20:03:18.999198 cli_command_parser-2023.7.30/setup.cfg
```

### Comparing `cli_command_parser-2023.7.29/LICENSE` & `cli_command_parser-2023.7.30/LICENSE`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.7.29/PKG-INFO` & `cli_command_parser-2023.7.30/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cli_command_parser
-Version: 2023.7.29
+Version: 2023.7.30
 Summary: CLI Command Parser
 Home-page: https://github.com/dskrypa/cli_command_parser
 Author: Doug Skrypa
 Author-email: dskrypa@gmail.com
 License: Apache 2.0
 Project-URL: Source, https://github.com/dskrypa/cli_command_parser
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cli_command_parser-2023.7.29/lib/cli_command_parser/__init__.py` & `cli_command_parser-2023.7.30/lib/cli_command_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.7.29/lib/cli_command_parser/annotations.py` & `cli_command_parser-2023.7.30/lib/cli_command_parser/annotations.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.7.29/lib/cli_command_parser/command_parameters.py` & `cli_command_parser-2023.7.30/lib/cli_command_parser/command_parameters.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.7.29/lib/cli_command_parser/commands.py` & `cli_command_parser-2023.7.30/lib/cli_command_parser/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     #: any CLI Command Parser internals, so it is safe for subclasses to redefine / overwrite it.
     ctx: Context
 
     def __new__(cls):
         # By storing the Context here instead of __init__, every single subclass won't need to
         # call super().__init__(...) from their own __init__ for this step
         self = super().__new__(cls)
-        self.__ctx = ctx = get_or_create_context(cls)
+        self.__ctx = ctx = get_or_create_context(cls, command=self)
         if not hasattr(self, 'ctx'):
             self.ctx: Context = ctx  # noqa  # PyCharm complains this is invalid, but doesn't understand it without it
         return self
 
     def __repr__(self) -> str:
         cls = self.__class__
         return f'<{cls.__name__} in prog={cls.__class__.meta(cls).prog!r}>'
```

### Comparing `cli_command_parser-2023.7.29/lib/cli_command_parser/compat.py` & `cli_command_parser-2023.7.30/lib/cli_command_parser/compat.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,18 +7,15 @@
 The :class:`WCTextWrapper` in this module extends the stdlib :class:`python:textwrap.TextWrapper` to support wide
 characters.
 """
 
 from textwrap import TextWrapper
 from typing import List
 
-try:
-    from wcwidth import wcswidth
-except ImportError:
-    wcswidth = len
+from .utils import wcswidth
 
 __all__ = ['WCTextWrapper']
 
 # region textwrap
 
 
 class WCTextWrapper(TextWrapper):
```

### Comparing `cli_command_parser-2023.7.29/lib/cli_command_parser/config.py` & `cli_command_parser-2023.7.30/lib/cli_command_parser/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -348,14 +348,17 @@
     #: Whether the metavar for Parameters that accept values should default to the name of the specified type
     #: (default: the name of the parameter)
     use_type_metavar: Bool = ConfigItem(False, bool)
 
     #: Whether the default value for Parameters should be shown in help text, and related behavior
     show_defaults: ShowDefaults = ConfigItem(ShowDefaults.MISSING | ShowDefaults.NON_EMPTY, ShowDefaults)
 
+    #: Whether Parameters that support reading their values from env variables should include the var names in help text
+    show_env_vars: Bool = ConfigItem(True, bool)
+
     @config_item(None)
     def cmd_alias_mode(self, value: CmdAliasMode) -> CmdAliasMode:
         """How subcommand aliases should be displayed in help text."""
         try:
             return SubcommandAliasHelpMode(value)
         except ValueError:
             return value
```

### Comparing `cli_command_parser-2023.7.29/lib/cli_command_parser/context.py` & `cli_command_parser-2023.7.30/lib/cli_command_parser/context.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,50 +22,56 @@
 from .exceptions import NoActiveContext
 from .utils import _NotSet, Terminal
 
 if TYPE_CHECKING:
     from .command_parameters import CommandParameters
     from .commands import Command
     from .parameters import Parameter, Option, ActionFlag
-    from .typing import Bool, ParamOrGroup, CommandType, AnyConfig, OptStr, PathLike
+    from .typing import Bool, ParamOrGroup, CommandType, CommandObj, AnyConfig, OptStr, StrSeq, PathLike  # noqa
 
 __all__ = ['Context', 'ctx', 'get_current_context', 'get_or_create_context', 'get_context', 'get_parsed', 'get_raw_arg']
 
 _context_stack = ContextVar('cli_command_parser.context.stack')
 _TERMINAL = Terminal()
 
+Argv = Optional['StrSeq']
+
 
 class Context(AbstractContextManager):  # Extending AbstractContextManager to make PyCharm's type checker happy
     """
     The parsing context.
 
     Holds user input while parsing, and holds the parsed values.  Handles config overrides / hierarchy for settings that
     affect parser behavior.
     """
 
     config: CommandConfig
     prog: OptStr = None
-    _terminal_width: Optional[int]
     allow_argv_prog: Bool = True
+    _command_obj: CommandObj = None
+    _terminal_width: Optional[int]
     _provided: Dict[ParamOrGroup, int]
 
     def __init__(
         self,
-        argv: Optional[Sequence[str]] = None,
-        command: Optional[CommandType] = None,
+        argv: Argv = None,
+        command_cls: Optional[CommandType] = None,
+        *,
         parent: Optional[Context] = None,
         config: AnyConfig = None,
         terminal_width: int = None,
         allow_argv_prog: Bool = None,
+        command: Optional[CommandObj] = None,
         **kwargs,
     ):
+        self.command_cls = command_cls
         self.command = command
         self.parent = parent
-        self.config = _normalize_config(config, kwargs, parent, command)
         self.actions_taken = 0
+        self.config = _normalize_config(config, kwargs, parent, command_cls)
         if parent:
             self._set_argv(parent.prog, argv)
             self._parsed = parent._parsed.copy()
             self._provided = parent._provided.copy()
             self._terminal_width = parent._terminal_width if terminal_width is None else terminal_width
             self.allow_argv_prog = parent.allow_argv_prog if allow_argv_prog is None else allow_argv_prog
         else:
@@ -80,31 +86,37 @@
 
     @classmethod
     def for_prog(cls, prog: PathLike, *args, **kwargs) -> Context:
         self = cls(*args, **kwargs)
         self.prog = getattr(prog, 'name', prog)
         return self
 
-    def _set_argv(self, prog: OptStr, argv: Optional[Sequence[str]]):
+    def _set_argv(self, prog: OptStr, argv: Argv):
         if prog:
             self.prog = prog
             self.argv = sys.argv[1:] if argv is None else argv
         elif argv is None:
             self.prog, *self.argv = sys.argv
         else:
             self.argv = argv
         self.remaining = list(self.argv)
 
-    def _sub_context(self, command: CommandType, argv: Optional[Sequence[str]] = None, **kwargs) -> Context:
-        if argv is None:
-            argv = self.remaining
-        return self.__class__(argv, command, parent=self, **kwargs)
+    def _sub_context(
+        self, command_cls: CommandType, argv: Argv = None, command: CommandObj = None, **kwargs
+    ) -> Context:
+        return self.__class__(
+            self.remaining if argv is None else argv,
+            command_cls,
+            parent=self,
+            command=self.command if command is None else command,
+            **kwargs,
+        )
 
     def __repr__(self) -> str:
-        command = getattr(self.command, '__name__', None)
+        command = getattr(self.command_cls, '__name__', None)
         prog, argv, allow_argv_prog = self.prog, self.argv, self.allow_argv_prog
         return f'<{self.__class__.__name__}[{command=!s}, {prog=}, {allow_argv_prog=}, {argv=}]>'
 
     def __enter__(self) -> Context:
         try:
             _context_stack.get().append(self)
         except LookupError:
@@ -136,56 +148,63 @@
         """Returns the current terminal width as the number of characters that fit on a single line."""
         if (width := self._terminal_width) is not None:
             return width
         return _TERMINAL.width
 
     def get_parsed(
         self,
+        command: Command = None,
+        *,
         exclude: Collection[Parameter] = (),
         recursive: Bool = True,
         default: Any = None,
         include_defaults: Bool = True,
     ) -> Dict[str, Any]:
         """
         Returns all of the parsed arguments as a dictionary.
 
         The :ref:`get_parsed() <advanced:Parsed Args as a Dictionary>` helper function provides an easier way to access
         this functionality.
 
+        :param command: An initialized Command object for which arguments were already parsed.
         :param exclude: Parameter objects that should be excluded from the returned results
         :param recursive: Whether parsed arguments should be recursively gathered from parent Commands
         :param default: The default value to use for parameters that raise :class:`.MissingArgument` when attempting to
           obtain their result values.
         :param include_defaults: Whether default values should be included in the returned results.  If False, only
           user-provided values will be included.
         :return: A dictionary containing all of the arguments that were parsed.  The keys in the returned dict match
           the names assigned to the Parameters in the Command associated with this Context.
         """
+        if command is None:
+            command = self.command
         with self:
             if recursive and (parent := self.parent):
-                parsed = parent.get_parsed(exclude, recursive, default, include_defaults)
+                parsed = parent.get_parsed(
+                    command, exclude=exclude, recursive=recursive, default=default, include_defaults=include_defaults
+                )
             else:
                 parsed = {}
 
             # TODO: Add way to get a nested dict with ParamGroup names as the keys of the nested sections?
             if params := self.params:
                 for param in params.iter_params(exclude):
                     if include_defaults or param in self._parsed:
-                        parsed[param.name] = param.result_value(default)
+                        parsed[param.name] = param.result_value(command, default)
 
         return parsed
 
     @cached_property
     def params(self) -> Optional[CommandParameters]:
         """
         The :class:`.CommandParameters` object that contains the categorized Parameters from the Command associated
         with this Context.
         """
-        if (command := self.command) is not None:
-            return command.__class__.params(command)
+        if self.command_cls is not None:
+            return self.command_cls.__class__.params(self.command_cls)
         return None
 
     def get_error_handler(self) -> Union[ErrorHandler, NullErrorHandler]:
         """Returns the :class:`.ErrorHandler` configured to be used."""
         if (error_handler := self.config.error_handler) is _NotSet:
             return extended_error_handler
         elif error_handler is None:
@@ -244,15 +263,15 @@
     def _parsed_action_flags(self) -> Tuple[int, List[ActionFlag], List[ActionFlag]]:
         """
         Not intended to be accessed by users.  Returns a tuple containing the total number of action flags provided, the
         action flags to run before main, and the action flags to run after main.
         """
         try:
             before_main, after_main = self.params.split_action_flags  # Each part is already sorted
-        except AttributeError:  # self.command is None
+        except AttributeError:  # self.command_cls is None
             return 0, [], []
 
         parsed = self._parsed
         before_main = [p for p in before_main if p in parsed] if before_main else []
         after_main = [p for p in after_main if p in parsed] if after_main else []
         return len(before_main) + len(after_main), before_main, after_main
 
@@ -298,15 +317,15 @@
             self.actions_taken += 1
             yield action_flag
 
     # endregion
 
 
 def _normalize_config(
-    config: AnyConfig, kwargs: Dict[str, Any], parent: Optional[Context], command: Optional[CommandType]
+    config: AnyConfig, kwargs: Dict[str, Any], parent: Context | None, command: CommandType | None
 ) -> CommandConfig:
     if config is not None:
         if kwargs:
             raise TypeError(f'Cannot combine {config=} with keyword config arguments={kwargs}')
         elif isinstance(config, CommandConfig):
             return config
         kwargs = config
@@ -418,25 +437,27 @@
         return _context_stack.get()[-1]
     except (LookupError, IndexError):
         if silent:
             return None
         raise NoActiveContext('There is no active context') from None
 
 
-def get_or_create_context(command_cls: CommandType, argv: Sequence[str] = None, **kwargs) -> Context:
+def get_or_create_context(
+    command_cls: CommandType, argv: Argv = None, *, command: CommandObj = None, **kwargs
+) -> Context:
     """
     Used internally by Commands to re-use an existing user-activated Context, or to create a new Context if there was
     no active Context.
     """
     if not (context := get_current_context(True)):
-        return Context(argv, command_cls, **kwargs)
-    elif argv is None and context.command is command_cls and not kwargs:
+        return Context(argv, command_cls, command=command, **kwargs)
+    elif argv is None and command is None and context.command_cls is command_cls and not kwargs:
         return context
     else:
-        return context._sub_context(command_cls, argv=argv, **kwargs)
+        return context._sub_context(command_cls, argv=argv, command=command, **kwargs)
 
 
 def get_context(command: Command) -> Context:
     """
     :param command: An initialized Command object
     :return: The Context associated with the given Command
     """
@@ -465,18 +486,20 @@
 
     :param command: An initialized Command object for which arguments were already parsed.
     :param to_call: A :class:`callable <python:collections.abc.Callable>` (function, method, class, etc.) that should
       be used to filter the parsed arguments.  If provided, then only the keys that match the callable's signature will
       be included in the returned dictionary of parsed arguments.
     :param default: The default value to use for parameters that raise :class:`.MissingArgument` when attempting to
       obtain their result values.
+    :param include_defaults: Whether default values should be included in the returned results.  If False, only
+      user-provided values will be included.
     :return: A dictionary containing all of the (optionally filtered) arguments that were parsed.  The keys in the
       returned dict match the names assigned to the Parameters in the given Command.
     """
-    parsed = get_context(command).get_parsed(default=default, include_defaults=include_defaults)
+    parsed = get_context(command).get_parsed(command, default=default, include_defaults=include_defaults)
     if to_call is not None:
         sig = Signature.from_callable(to_call)
         keys = {k for k, p in sig.parameters.items() if p.kind != _Parameter.VAR_KEYWORD}
         parsed = {k: v for k, v in parsed.items() if k in keys}
 
     return parsed
```

### Comparing `cli_command_parser-2023.7.29/lib/cli_command_parser/conversion/argparse_ast.py` & `cli_command_parser-2023.7.30/lib/cli_command_parser/conversion/argparse_ast.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.7.29/lib/cli_command_parser/conversion/argparse_utils.py` & `cli_command_parser-2023.7.30/lib/cli_command_parser/conversion/argparse_utils.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.7.29/lib/cli_command_parser/conversion/command_builder.py` & `cli_command_parser-2023.7.30/lib/cli_command_parser/conversion/command_builder.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.7.29/lib/cli_command_parser/conversion/utils.py` & `cli_command_parser-2023.7.30/lib/cli_command_parser/conversion/utils.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.7.29/lib/cli_command_parser/conversion/visitor.py` & `cli_command_parser-2023.7.30/lib/cli_command_parser/conversion/visitor.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.7.29/lib/cli_command_parser/core.py` & `cli_command_parser-2023.7.30/lib/cli_command_parser/core.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.7.29/lib/cli_command_parser/documentation.py` & `cli_command_parser-2023.7.30/lib/cli_command_parser/documentation.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.7.29/lib/cli_command_parser/error_handling.py` & `cli_command_parser-2023.7.30/lib/cli_command_parser/error_handling.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.7.29/lib/cli_command_parser/exceptions.py` & `cli_command_parser-2023.7.30/lib/cli_command_parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.7.29/lib/cli_command_parser/formatting/commands.py` & `cli_command_parser-2023.7.30/lib/cli_command_parser/formatting/commands.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.7.29/lib/cli_command_parser/formatting/params.py` & `cli_command_parser-2023.7.30/lib/cli_command_parser/formatting/params.py`

 * *Files 4% similar despite different names*

```diff
@@ -105,16 +105,15 @@
         yield self.format_usage(include_meta=include_meta, full=full)
 
     def format_description(self, rst: Bool = False, description: str = None) -> str:
         param = self.param
         if description is None:
             description = param.help or ''
         if _should_add_default(param.default, description, param.show_default):
-            pad = ' ' if description else ''
-            quote = '``' if rst else ''
+            pad, quote = _pad_and_quote(description, rst)
             description += f'{pad}(default: {quote}{param.default!r}{quote})'
 
         return description
 
     def format_help(self, prefix: str = '', tw_offset: int = 0) -> str:
         usage_iter = self.iter_usage_parts(include_meta=True, full=True)
         description = self.format_description()
@@ -158,14 +157,27 @@
         opts = param.option_strs
         if param.nargs == 0:
             yield from opts.option_strs()
         else:
             metavar = self._format_usage_metavar()
             yield from (f'{opt} {metavar}' for opt in opts.option_strs())
 
+    def format_description(self, rst: Bool = False, description: str = None) -> str:
+        description = super().format_description(rst, description)
+        param: BaseOption = self.param
+        if param.env_var and (param.show_env_var or (param.show_env_var is None and ctx.config.show_env_vars)):
+            pad, quote = _pad_and_quote(description, rst)
+            var_names = [f'{quote}{var_name}{quote}' for var_name in param.env_vars()]
+            if len(var_names) == 1:
+                description += f'{pad}(may be provided via env var: {var_names[0]})'
+            else:
+                description += f'{pad}(may be provided via any of the following env vars: {", ".join(var_names)})'
+
+        return description
+
     def format_usage(self, include_meta: Bool = False, full: Bool = False, delim: str = ', ') -> str:
         if full:
             return delim.join(self.iter_usage_parts())
 
         param: BaseOption = self.param
         opt = param.option_strs.get_usage_opt()
         if not include_meta or param.nargs == 0:
@@ -496,7 +508,13 @@
                     table.add_rows(formatter.rst_rows())
                     # table.add_row(*formatter.rst_row())
                 else:
                     sub_table.show_title = False
                     table.add_row(sub_table.title, str(sub_table))
 
         return table
+
+
+def _pad_and_quote(description: str, rst: bool) -> Tuple[str, str]:
+    pad = ' ' if description else ''
+    quote = '``' if rst else ''
+    return pad, quote
```

### Comparing `cli_command_parser-2023.7.29/lib/cli_command_parser/formatting/restructured_text.py` & `cli_command_parser-2023.7.30/lib/cli_command_parser/formatting/restructured_text.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.7.29/lib/cli_command_parser/formatting/utils.py` & `cli_command_parser-2023.7.30/lib/cli_command_parser/formatting/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,25 +2,20 @@
 Utils for usage / help text formatters
 
 :author: Doug Skrypa
 """
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Optional, Any, Collection, Sequence, Iterator, Iterable, Tuple, List
-
-try:
-    from wcwidth import wcswidth
-except ImportError:
-    wcswidth = len
+from typing import TYPE_CHECKING, Optional, Any, Collection, Sequence, Iterator, Iterable, List
 
 from ..compat import WCTextWrapper
 from ..config import ShowDefaults
 from ..context import ctx
-from ..utils import _NotSet
+from ..utils import _NotSet, wcswidth
 
 if TYPE_CHECKING:
     from ..typing import Bool, Strs, OptStrs
 
 __all__ = ['format_help_entry', 'line_iter']
 
 
@@ -39,16 +34,17 @@
     else:
         line_prefix = ' ' * lpad
 
     config = ctx.config
     term_width = ctx.terminal_width - tw_offset
     usage_width = max(config.min_usage_column_width, config.usage_column_width - tw_offset - 2)
     if not description:
-        usage_line_iter = combine_and_wrap(usage_parts, term_width, cont_indent, usage_delim)
-        return '\n'.join(line_prefix + line for line in usage_line_iter)
+        return '\n'.join(
+            line_prefix + line for line in combine_and_wrap(usage_parts, term_width, cont_indent, usage_delim)
+        )
 
     after_pad_width = usage_width - lpad
     usage_lines = tuple(combine_and_wrap(usage_parts, term_width, cont_indent, usage_delim))
     description_lines = [''] * _description_start_line(usage_lines, after_pad_width)
     description_lines.extend(_normalize_column_width(_single_line_strs(description), term_width - usage_width - 2))
     format_row = f'{line_prefix}{{:<{after_pad_width}s}}  {{}}'.format
     return '\n'.join(format_row(*row).rstrip() for row in line_iter(usage_lines, description_lines))
@@ -110,28 +106,24 @@
 
 def _single_line_strs(lines: Strs) -> List[str]:
     if isinstance(lines, str):
         lines = (lines,)
     return [line for full_line in lines for line in full_line.splitlines()]
 
 
-def _normalize_column_width(lines: Sequence[str], column_width: int, cont_indent: int = 0) -> Sequence[str]:
-    max_width = max(map(wcswidth, lines)) + cont_indent
-    if max_width <= column_width:
-        return lines
-
-    tw = WCTextWrapper(column_width, break_long_words=True, break_on_hyphens=True)
-    fixed = []
-    for line in lines:
-        if wcswidth(line) + cont_indent >= column_width:
-            fixed.extend(tw.wrap(line))
-        else:
-            fixed.append(line)
-
-    return fixed
+def _normalize_column_width(lines: Sequence[str], column_width: int, cont_indent: int = 0) -> Iterator[str]:
+    if max(map(wcswidth, lines)) + cont_indent <= column_width:
+        yield from lines
+    else:
+        tw = WCTextWrapper(column_width, break_long_words=True, break_on_hyphens=True)
+        for line in lines:
+            if wcswidth(line) + cont_indent >= column_width:
+                yield from tw.wrap(line)
+            else:
+                yield line
 
 
 def _should_add_default(default: Any, help_text: Optional[str], param_show_default: Optional[Bool]) -> bool:
     if default is _NotSet:
         return False
     elif param_show_default is not None:
         return param_show_default
@@ -142,25 +134,25 @@
         return True
     elif sd & ShowDefaults.NON_EMPTY:
         return bool(default) or not (default is None or isinstance(default, Collection))
     else:
         return bool(default)
 
 
-def line_iter(*columns: Strs) -> Iterator[Tuple[str, ...]]:
+def line_iter(*columns: Strs) -> Iterator[List[str, ...]]:
     """More complicated than what would be necessary for just 2 columns, but this will scale to handle 3+"""
     exhausted = 0
     column_count = len(columns)
 
     def _iter(column: Strs) -> Iterator[str]:
         nonlocal exhausted
         yield from column.splitlines() if isinstance(column, str) else column
         exhausted += 1
         while True:
             yield ''
 
-    column_iters = tuple(_iter(c) for c in columns)
+    column_iters = [_iter(c) for c in columns]
     while True:
-        row = tuple(next(ci) for ci in column_iters)  # pylint: disable=R1708
+        row = [next(ci) for ci in column_iters]  # pylint: disable=R1708
         if exhausted == column_count:  # `while exhausted < column_count:` always results in 1 extra row
             break
         yield row
```

### Comparing `cli_command_parser-2023.7.29/lib/cli_command_parser/inputs/__init__.py` & `cli_command_parser-2023.7.30/lib/cli_command_parser/inputs/__init__.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.7.29/lib/cli_command_parser/inputs/base.py` & `cli_command_parser-2023.7.30/lib/cli_command_parser/inputs/base.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.7.29/lib/cli_command_parser/inputs/choices.py` & `cli_command_parser-2023.7.30/lib/cli_command_parser/inputs/choices.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.7.29/lib/cli_command_parser/inputs/exceptions.py` & `cli_command_parser-2023.7.30/lib/cli_command_parser/inputs/exceptions.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.7.29/lib/cli_command_parser/inputs/files.py` & `cli_command_parser-2023.7.30/lib/cli_command_parser/inputs/files.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.7.29/lib/cli_command_parser/inputs/numeric.py` & `cli_command_parser-2023.7.30/lib/cli_command_parser/inputs/numeric.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.7.29/lib/cli_command_parser/inputs/patterns.py` & `cli_command_parser-2023.7.30/lib/cli_command_parser/inputs/patterns.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.7.29/lib/cli_command_parser/inputs/time.py` & `cli_command_parser-2023.7.30/lib/cli_command_parser/inputs/time.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.7.29/lib/cli_command_parser/inputs/utils.py` & `cli_command_parser-2023.7.30/lib/cli_command_parser/inputs/utils.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.7.29/lib/cli_command_parser/metadata.py` & `cli_command_parser-2023.7.30/lib/cli_command_parser/metadata.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.7.29/lib/cli_command_parser/nargs.py` & `cli_command_parser-2023.7.30/lib/cli_command_parser/nargs.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.7.29/lib/cli_command_parser/parameters/actions.py` & `cli_command_parser-2023.7.30/lib/cli_command_parser/parameters/actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from ..context import ctx
 from ..exceptions import BadArgument, MissingArgument, InvalidChoice, TooManyArguments, ParamUsageError, ParamConflict
 from ..inputs import InputType
 from ..nargs import Nargs
 from ..utils import _NotSet, camel_to_snake_case
 
 if TYPE_CHECKING:
-    from ..typing import OptStr, Param, Bool, T_co
+    from ..typing import CommandObj, Param, Bool, T_co
 
 __all__ = [
     'ParamAction',
     'Store',
     'Append',
     'StoreConst',
     'AppendConst',
@@ -133,17 +133,19 @@
     def can_reset(self) -> bool:
         return False
 
     # endregion
 
     # region Parsed Value / Default Finalization
 
-    def get_default(self, missing_default=_NotSet):
+    def get_default(self, command: CommandObj | None = None, missing_default=_NotSet):
         if (default := self.param.default) is not _NotSet:
             return self.finalize_default(default)
+        elif (default_cb := self.param.default_cb) and command is not None:
+            return self.finalize_default(default_cb(command))
         return self.default
 
     def finalize_default(self, value):
         if (type_func := self.param.type) and isinstance(type_func, InputType):
             return type_func.fix_default(value)
         return value
 
@@ -335,17 +337,19 @@
             return False
         return ctx.has_parsed_value(self.param)
 
     # endregion
 
     # region Parsed Value / Default Finalization
 
-    def get_default(self, missing_default=_NotSet):
+    def get_default(self, command: CommandObj | None = None, missing_default=_NotSet):
         if (default := self.param.default) is not _NotSet:
             return self.finalize_default(default)
+        elif (default_cb := self.param.default_cb) and command is not None:
+            return self.finalize_default(default_cb(command))
         return []
 
     def finalize_default(self, value):
         if self.param.strict_default:
             return value
 
         if (type_func := self.param.type) and isinstance(type_func, InputType):
@@ -419,15 +423,15 @@
         self.append_const(self.param.get_const(opt))
         return 1
 
     # endregion
 
     # region Parsed Value / Default Finalization
 
-    def get_default(self, missing_default=_NotSet):
+    def get_default(self, command: CommandObj | None = None, missing_default=_NotSet):
         return []
 
     # endregion
 
 
 # class StoreValueOrConst(ConstMixin, Store, accepts_values=True, accepts_consts=True):
 #     __slots__ = ()
```

### Comparing `cli_command_parser-2023.7.29/lib/cli_command_parser/parameters/base.py` & `cli_command_parser-2023.7.30/lib/cli_command_parser/parameters/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from ..config import CommandConfig, OptionNameMode, AllowLeadingDash, DEFAULT_CONFIG
 from ..context import Context, ctx, get_current_context
 from ..exceptions import ParameterDefinitionError, BadArgument, MissingArgument, InvalidChoice
 from ..inputs import InputType, normalize_input_type
 from ..inputs.choices import _ChoicesBase
 from ..inputs.exceptions import InputValidationError, InvalidChoiceError
 from ..nargs import Nargs, REMAINDER
-from ..typing import T_co
+from ..typing import T_co, DefaultFunc, CommandMethod
 from ..utils import _NotSet
 from .option_strings import OptionStrings
 
 if TYPE_CHECKING:
     from ..formatting.params import ParamHelpFormatter
     from ..typing import OptStr, OptStrs, Strings, Bool, CommandCls, CommandObj, CommandAny, Param, LeadingDash
     from .actions import ParamAction
@@ -170,16 +170,18 @@
     # Class attributes
     _action_map: Dict[str, Type[ParamAction]] = {}
     _repr_attrs: Optional[Strings] = None           #: Attributes to include in ``repr()`` output
     # Instance attributes with class defaults
     metavar: str = None
     nargs: Nargs                                    # Expected to be set in subclasses
     type: Optional[Callable[[str], T_co]] = None    # Expected to be set in subclasses
-    show_default: Bool = None
     allow_leading_dash: AllowLeadingDash = AllowLeadingDash.NUMERIC  # Set in some subclasses
+    default = _NotSet
+    default_cb: DefaultCallback | None = None
+    show_default: Bool = None
     strict_default: Bool = False
 
     def __init_subclass__(cls, repr_attrs: Strings = None, actions: Collection[Type[ParamAction]] = None, **kwargs):
         """
         :param repr_attrs: Additional attributes to include in the repr.
         :param actions: Collection of ParamAction classes that this type of Parameter supports
         """
@@ -190,36 +192,45 @@
             action_map.update((action.name, action) for action in actions)
         if repr_attrs:
             cls._repr_attrs = repr_attrs
 
     def __init__(  # pylint: disable=R0913
         self,
         action: str,
-        name: str = None,
-        default: Any = _NotSet,
-        required: Bool = False,
-        metavar: str = None,
+        *,
         help: str = None,  # noqa
         hide: Bool = False,
+        metavar: str = None,
+        name: str = None,
+        required: Bool = False,
+        default: Any = _NotSet,
+        default_cb: DefaultFunc = None,
         show_default: Bool = None,
         strict_default: Bool = False,
     ):
         if not (param_action := self._action_map.get(action)):
             self._handle_bad_action(action)
         if required and default is not _NotSet:
             # TODO: For required mutually dependent groups, or a required group with all params having a default,
             #  is another check needed, or does this check make sense, or should this check be removed?
             raise ParameterDefinitionError(
                 f'Invalid combination of required=True with {default=} for {self.__class__.__name__} -'
                 ' required Parameters cannot have a default value'
             )
         super().__init__(name=name, required=required, help=help, hide=hide)
         self.action = param_action(self)
-        self.default = default
         self.metavar = metavar
+        if default is not _NotSet:
+            if default_cb is not None:
+                raise ParameterDefinitionError(
+                    f'{self.__class__.__name__}s can only have a {default=} xor {default_cb=}, not both'
+                )
+            self.default = default
+        elif default_cb is not None:
+            self.default_cb = DefaultCallback(default_cb)
         self.strict_default = strict_default
         if show_default is not None:
             self.show_default = show_default
 
     def _handle_bad_action(self, action: str) -> NoReturn:
         """
         Called when an action not supported by this type of Parameter was provided.  May be overwritten in subclasses
@@ -250,18 +261,42 @@
 
     @property
     def has_choices(self) -> bool:
         if type_attr := self.type:
             return isinstance(type_attr, _ChoicesBase) and type_attr.choices
         return False
 
+    def register_default_cb(self, method: CommandMethod) -> CommandMethod:
+        """
+        Intended to be used as a decorator to register a method in a Command to be used as the default callback for
+        this Parameter.  The method will only be called during parsing if no value was explicitly provided for this
+        Parameter.  The decorated method is returned unchanged, so it can still be called directly if necessary.
+
+        :param method: A method that does not accept any arguments (except ``self``), and returns the value that should
+          be used for this Parameter.
+        :return: The method, unchanged.
+        """
+        if self.default is not _NotSet:
+            problem = f'default={self.default!r}'
+        elif self.default_cb:
+            problem = f'default_cb={self.default_cb!r}'
+        else:
+            problem = None
+
+        if problem:
+            raise ParameterDefinitionError(
+                f'Cannot register a default callback method for {self} because it already has {problem}'
+            )
+        self.default_cb = DefaultCallback(method, True)
+        return method
+
     # endregion
 
     def __repr__(self) -> str:
-        names = ('action', 'const', 'default', 'type', 'choices', 'required', 'hide', 'help')
+        names = ('action', 'const', 'default', 'default_cb', 'type', 'choices', 'required', 'hide', 'help')
         if extra_attrs := self._repr_attrs:
             names = chain(names, extra_attrs)
 
         skip = (None, _NotSet)
         attrs = (
             (a, str(v) if a == 'action' else v)
             for a in names
@@ -323,29 +358,29 @@
         ...
 
     def __get__(self, command, owner):
         if command is None:
             return self
 
         with self._ctx(command):
-            value = self.result()
+            value = self.result(command)
 
-        if (name := self._attr_name) is not None:
-            command.__dict__[name] = value  # Skip __get__ on subsequent accesses
+        if self._attr_name:
+            command.__dict__[self._attr_name] = value  # Skip __get__ on subsequent accesses
         return value
 
-    def result_value(self, missing_default: TD = _NotSet) -> Union[T_co, TD, None]:
+    def result_value(self, command: CommandObj | None = None, missing_default: TD = _NotSet) -> Union[T_co, TD, None]:
         value = ctx.get_parsed_value(self)
         if value is _NotSet:
             if self.required:
                 if missing_default is _NotSet:
                     raise MissingArgument(self)
                 return missing_default
             else:
-                return self.action.get_default(missing_default)
+                return self.action.get_default(command, missing_default)
 
         return self.action.finalize_value(value)
 
     result = result_value
 
     # endregion
 
@@ -384,23 +419,25 @@
         :param default_ok: Whether default values are supported for this Parameter type
         :param kwargs: Additional keyword arguments to pass to :meth:`.Parameter.__init_subclass__`.
         """
         super().__init_subclass__(**kwargs)
         if default_ok is not None:
             cls._default_ok = default_ok
 
-    def __init__(self, action: str, *, required: Bool = True, default: Any = _NotSet, **kwargs):
+    def __init__(
+        self, action: str, *, required: Bool = True, default: Any = _NotSet, default_cb: DefaultFunc = None, **kwargs
+    ):
         if not (self._default_ok and 0 in self.nargs):  # Indicates that having a default is bad
             if not required:
                 cls_name = self.__class__.__name__
                 raise ParameterDefinitionError(f'All {cls_name} parameters must be required - invalid {required=}')
-            elif default is not _NotSet:
+            elif kw := ('default' if default is not _NotSet else 'default_cb' if default_cb is not None else None):
                 cls_name = self.__class__.__name__
-                raise ParameterDefinitionError(f"The 'default' arg is not supported for {cls_name} parameters")
-        super().__init__(action, default=default, required=required, **kwargs)
+                raise ParameterDefinitionError(f'The {kw!r} arg is not supported for {cls_name} parameters')
+        super().__init__(action, default=default, required=required, default_cb=default_cb, **kwargs)
 
 
 class BaseOption(Parameter[T_co], ABC):
     """
     Base class for :class:`.Option`, :class:`.Flag`, :class:`.Counter`, and any other keyword-like parameters that have
     ``--long`` and ``-short`` prefixes before values.
 
@@ -430,35 +467,39 @@
       taken as if it was specified as a CLI flag (e.g., ``--foo`` with no value).
     :param kwargs: Additional keyword arguments to pass to :class:`Parameter`.
     """
 
     _opt_str_cls: Type[OptionStrings] = OptionStrings
     option_strs: OptionStrings
     env_var: OptStrs = None
+    show_env_var: Bool = None
     strict_env: Bool
     use_env_value: Bool
     const = _NotSet
 
     def __init__(
         self,
         *option_strs: str,
         action: str,
         name_mode: Union[OptionNameMode, str, None] = _NotSet,
         env_var: OptStrs = None,
         strict_env: bool = True,
         use_env_value: Bool = None,
+        show_env_var: Bool = None,
         **kwargs,
     ):
         super().__init__(action, **kwargs)
         self.option_strs = self._opt_str_cls(option_strs, name_mode)
         self.strict_env = strict_env
         if env_var:
             self.env_var = env_var
         if use_env_value is not None:
             self.use_env_value = use_env_value
+        if show_env_var is not None:
+            self.show_env_var = show_env_var
 
     def _handle_bad_action(self, action: str) -> NoReturn:
         if action in ('store', 'append') and (fixed := f'{action}_const') in self._action_map:
             raise ParameterDefinitionError(f'Invalid {action=} for {self.__class__.__name__} - did you mean {fixed!r}?')
         super()._handle_bad_action(action)
 
     def __set_name__(self, command: CommandCls, name: str):
@@ -508,7 +549,23 @@
                 raise ParameterDefinitionError(
                     f'With {nargs=}, only allow_leading_dash=AllowLeadingDash.ALWAYS is supported - found: {value!r}'
                 )
             value = AllowLeadingDash.ALWAYS
 
         if value is not None:
             instance.__dict__[self.name] = value
+
+
+class DefaultCallback:
+    __slots__ = ('func', 'is_method')
+
+    def __init__(self, func: CommandMethod | DefaultFunc, is_method: bool = False):
+        self.func = func
+        self.is_method = is_method
+
+    def __repr__(self) -> str:
+        return f'<{self.__class__.__name__}({self.func!r}, is_method={self.is_method})>'
+
+    def __call__(self, command: CommandObj | None) -> T_co:
+        # If the func is not a method, then `command` must not be None, but the default callback is intentionally
+        # not called by ParamAction.get_default (and its subclasses) when command is None.
+        return self.func(command) if self.is_method else self.func()
```

### Comparing `cli_command_parser-2023.7.29/lib/cli_command_parser/parameters/choice_map.py` & `cli_command_parser-2023.7.30/lib/cli_command_parser/parameters/choice_map.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from typing import Type, TypeVar, Generic, Optional, Callable, Union, Collection, Mapping, NoReturn, Dict
 from types import MethodType
 
 from ..context import ctx
 from ..exceptions import ParameterDefinitionError, BadArgument, InvalidChoice, CommandDefinitionError
 from ..formatting.utils import format_help_entry
 from ..nargs import Nargs
-from ..typing import Bool, CommandCls
+from ..typing import Bool, CommandCls, CommandObj
 from ..utils import _NotSet, camel_to_snake_case, short_repr
 from .actions import Concatenate
 from .base import BasePositional
 
 __all__ = ['SubCommand', 'Action', 'Choice', 'ChoiceMap']
 
 T = TypeVar('T')
@@ -98,14 +98,17 @@
 
     def __init__(self, *, action: str = 'concatenate', title: str = None, description: str = None, **kwargs):
         super().__init__(action=action, **kwargs)
         self.title = title
         self.description = description
         self.choices = {}
 
+    def register_default_cb(self, method):
+        raise ParameterDefinitionError(f'{self.__class__.__name__}s do not support default callback methods')
+
     # region Choice Registration
 
     @property
     def has_choices(self) -> bool:
         return bool(self.choices)
 
     def _update_nargs(self):
@@ -160,23 +163,23 @@
             return
         elif len(values) > self.nargs.max:
             raise BadArgument(self, 'too many values')
         prefix = choice + ' '
         if not any(c.startswith(prefix) for c in choices if c):
             raise InvalidChoice(self, prefix[:-1], choices)
 
-    def result_value(self, missing_default: TD = _NotSet) -> Union[OptStr, TD]:
+    def result_value(self, command: CommandObj | None = None, missing_default: TD = _NotSet) -> Union[OptStr, TD]:
         if not self.choices:
             self._no_choices_error()
-        return super().result_value(missing_default)
+        return super().result_value(command, missing_default)
 
     result = result_value
 
     def target(self) -> T:
-        return self.choices[self.result_value()].target
+        return self.choices[self.result_value(None)].target
 
     # endregion
 
     # region Usage / Help Text
 
     @property
     def show_in_help(self) -> bool:
@@ -278,15 +281,15 @@
             if choice is not None:
                 raise CommandDefinitionError(f'Cannot combine a positional {command_or_choice=} choice with {choice=}')
             return partial(self.register_command, command_or_choice, help=help)
         else:
             return self.register_command(choice, command_or_choice, help=help)  # noqa
 
     def _no_choices_error(self) -> NoReturn:
-        raise CommandDefinitionError(f'{ctx.command}.{self.name} = {self} has no sub Commands')
+        raise CommandDefinitionError(f'{ctx.command_cls}.{self.name} = {self} has no sub Commands')
 
 
 class Action(ChoiceMap[MethodType], title='Actions'):
     """
     Actions are similar to :class:`.SubCommand` parameters, but allow methods in :class:`.Command` classes to
     be registered as a callable to be executed based on a user's choice instead of separate sub Commands.
```

### Comparing `cli_command_parser-2023.7.29/lib/cli_command_parser/parameters/groups.py` & `cli_command_parser-2023.7.30/lib/cli_command_parser/parameters/groups.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.7.29/lib/cli_command_parser/parameters/option_strings.py` & `cli_command_parser-2023.7.30/lib/cli_command_parser/parameters/option_strings.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.7.29/lib/cli_command_parser/parameters/options.py` & `cli_command_parser-2023.7.30/lib/cli_command_parser/parameters/options.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from ..typing import T_co, TypeFunc
 from ..utils import _NotSet, str_to_bool
 from .actions import Store, StoreConst, Append, AppendConst, Count
 from .base import BaseOption, AllowLeadingDashProperty
 from .option_strings import TriFlagOptionStrings
 
 if TYPE_CHECKING:
-    from ..typing import Bool, ChoicesType, InputTypeFunc, CommandCls, CommandObj, OptStr, LeadingDash
+    from ..typing import Bool, ChoicesType, InputTypeFunc, CommandCls, CommandObj, OptStr, LeadingDash, CommandMethod
 
 __all__ = [
     'Option',
     'Flag',
     'TriFlag',
     'ActionFlag',
     'Counter',
@@ -157,34 +157,41 @@
     const: TC
 
     def __init__(
         self,
         *option_strs: str,
         action: ConstAct = 'store_const',
         default: TD = _NotSet,
+        default_cb=_NotSet,
         const: TC = _NotSet,
         type: TypeFunc = None,  # noqa
         **kwargs,
     ):
         if const is _NotSet:
             try:
                 const = self.__default_const_map[default]
             except KeyError as e:
                 raise ParameterDefinitionError(
                     f"A 'const' value is required for {self.__class__.__name__} since {default=} is not True or False"
                 ) from e
+        if default_cb is not _NotSet:
+            cls_name = self.__class__.__name__
+            raise ParameterDefinitionError(f"The 'default_cb' arg is not supported for {cls_name} parameters")
         if default is _NotSet:
             default = self.__default_const_map.get(const, _NotSet)  # will be True or False
         if default is False:  # Avoid surprises for custom non-truthy values
             kwargs.setdefault('show_default', False)
         super().__init__(*option_strs, action=action, default=default, **kwargs)
         self.const = const
         if type is not None:
             self.type = type
 
+    def register_default_cb(self, method):
+        raise ParameterDefinitionError(f'{self.__class__.__name__}s do not support default callback methods')
+
     def get_env_const(self, value: str, env_var: str) -> Tuple[Union[TC, TD], bool]:
         try:
             parsed = self.type(value)
         except Exception as e:
             raise ParamUsageError(self, f'unable to parse {value=} from {env_var=}: {e}') from e
         if self.use_env_value and parsed != self.const and parsed != self.default:
             raise BadArgument(self, f'invalid value={parsed!r} from {env_var=}')
@@ -225,14 +232,15 @@
       whether this TriFlag's normal action should be taken as if it was specified via a CLI argument.
     :param kwargs: Additional keyword arguments to pass to :class:`.BaseOption`.
     """
 
     nargs = Nargs(0)
     type = staticmethod(str_to_bool)  # Without staticmethod, this would be interpreted as a normal method
     use_env_value: bool = False
+    _default_cb_ok = True
     _opt_str_cls = TriFlagOptionStrings
     option_strs: TriFlagOptionStrings
     alt_help: OptStr = None
     default: TD
     consts: Tuple[TC, TA]
 
     def __init__(
@@ -241,14 +249,15 @@
         consts: Tuple[TC, TA] = (True, False),
         alt_prefix: str = None,
         alt_long: str = None,
         alt_short: str = None,
         alt_help: str = None,
         action: ConstAct = 'store_const',
         default: TD = _NotSet,
+        default_cb: Callable[[], TD] = None,
         type: TypeFunc = None,  # noqa
         **kwargs,
     ):
         if alt_short and '-' in alt_short[1:]:
             raise ParameterDefinitionError(f"Bad alt_short option - may not contain '-': {alt_short}")
         elif alt_prefix and ('=' in alt_prefix or alt_prefix.startswith('-')):
             raise ParameterDefinitionError(f"Bad alt_prefix - may not contain '=' or start with '-': {alt_prefix}")
@@ -257,34 +266,42 @@
 
         try:
             _pos, _neg = consts
         except (ValueError, TypeError) as e:
             msg = f'Invalid {consts=} - expected a 2-tuple of (positive, negative) constants to store'
             raise ParameterDefinitionError(msg) from e
 
-        if default is _NotSet and not kwargs.get('required', False):
-            default = None
+        if default is _NotSet and default_cb is None:
+            if not kwargs.get('required', False):
+                default = None
+        else:
+            self._default_cb_ok = False
         if default in consts:
             raise ParameterDefinitionError(
                 f'Invalid {default=} with {consts=} - the default must not match either value'
             )
 
         alt_opt_strs = (opt for opt in (alt_short, alt_long) if opt)
-        super().__init__(*option_strs, *alt_opt_strs, action=action, default=default, **kwargs)
+        super().__init__(*option_strs, *alt_opt_strs, action=action, default=default, default_cb=default_cb, **kwargs)
         self.consts = consts
         self.option_strs.add_alts(alt_prefix, alt_long, alt_short)
         if alt_help:
             self.alt_help = alt_help
         if type is not None:
             self.type = type
 
     def __set_name__(self, command: CommandCls, name: str):
         super().__set_name__(command, name)
         self.option_strs.update_alts(name)
 
+    def register_default_cb(self, method: CommandMethod) -> CommandMethod:
+        if self._default_cb_ok and self.default is not _NotSet:
+            self.default = _NotSet  # The default was set by __init__ - remove it so the method can be registered
+        return super().register_default_cb(method)
+
     def get_const(self, opt_str: OptStr = None) -> Union[TC, TA]:
         if opt_str in self.option_strs.alt_allowed:
             return self.consts[1]
         else:
             return self.consts[0]
 
     def get_env_const(self, value: str, env_var: str) -> Tuple[Union[TC, TA, TD], bool]:
@@ -388,18 +405,18 @@
 
     def __get__(self, command: Optional[CommandObj], owner: CommandCls) -> Union[ActionFlag, Callable]:
         # Allow the method to be called, regardless of whether it was specified
         if command is None:
             return self
         return partial(self.func, command)  # imitates a bound method
 
-    def result(self) -> Optional[Callable]:
-        if self.result_value():
-            if func := self.func:
-                return func
+    def result(self, command: CommandObj | None = None) -> Optional[Callable]:
+        if self.result_value(command):
+            if self.func:
+                return self.func
             raise ParameterDefinitionError(f'No function was registered for {self}')
         return None
 
 
 #: Alias for :class:`ActionFlag`
 action_flag = ActionFlag  # pylint: disable=C0103
 
@@ -454,28 +471,36 @@
     def __init__(
         self,
         *option_strs: str,
         action: str = 'count',
         init: int = 0,
         const: int = 1,
         default: int = _NotSet,
+        default_cb: Callable[[], int] = None,
         required: bool = False,
         **kwargs,
     ):
         type_check_vals = {'const': const, 'init': init}
         if default is not _NotSet:
             type_check_vals['default'] = default
-        elif not required:
-            default = 0
+        elif not required and default_cb is None:
+            default_cb = _counter_default  # This makes it easier to allow a method to override it
         if bad_types := ', '.join(f'{k}={v!r}' for k, v in type_check_vals.items() if not isinstance(v, self.type)):
             raise ParameterDefinitionError(f'Invalid type for parameters (expected int): {bad_types}')
-        super().__init__(*option_strs, action=action, default=default, required=required, **kwargs)
+        super().__init__(
+            *option_strs, action=action, default=default, default_cb=default_cb, required=required, **kwargs
+        )
         self.init = init
         self.const = const
 
+    def register_default_cb(self, method: CommandMethod) -> CommandMethod:
+        if self.default_cb and self.default_cb.func is _counter_default:
+            self.default_cb = None
+        return super().register_default_cb(method)
+
     def prepare_value(self, value: Optional[str], short_combo: bool = False, pre_action: bool = False) -> int:
         try:
             return self.type(value)
         except (ValueError, TypeError) as e:
             combinable = self.option_strs.combinable
             if short_combo and combinable and all(c in combinable for c in value):
                 return len(value) + 1  # +1 for the -short that preceded this value
@@ -486,7 +511,11 @@
             return
         try:
             value = self.type(value)
         except (ValueError, TypeError) as e:
             raise BadArgument(self, f'invalid {value=} (expected an integer)') from e
         else:
             return
+
+
+def _counter_default():
+    return 0
```

### Comparing `cli_command_parser-2023.7.29/lib/cli_command_parser/parameters/pass_thru.py` & `cli_command_parser-2023.7.30/lib/cli_command_parser/parameters/pass_thru.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.7.29/lib/cli_command_parser/parameters/positionals.py` & `cli_command_parser-2023.7.30/lib/cli_command_parser/parameters/positionals.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from ..inputs import normalize_input_type
 from ..nargs import Nargs, NargsValue
 from ..utils import _NotSet
 from .actions import Store, Append
 from .base import BasePositional, AllowLeadingDashProperty
 
 if TYPE_CHECKING:
-    from ..typing import InputTypeFunc, ChoicesType, LeadingDash
+    from ..typing import InputTypeFunc, ChoicesType, LeadingDash, DefaultFunc
 
 __all__ = ['Positional']
 
 
 class Positional(BasePositional, default_ok=True, actions=(Store, Append)):
     """
     A parameter that must be provided positionally.
@@ -55,14 +55,15 @@
     def __init__(
         self,
         nargs: NargsValue = None,
         action: Literal['store', 'append'] = None,
         type: InputTypeFunc = None,  # noqa
         default: Any = _NotSet,
         *,
+        default_cb: DefaultFunc = None,
         choices: ChoicesType = None,
         allow_leading_dash: LeadingDash = None,
         **kwargs,
     ):
         if nargs_provided := nargs is not None:
             self.nargs = nargs = Nargs(nargs)
             if nargs == 0:
@@ -76,15 +77,15 @@
             if nargs_provided:
                 action = 'store' if nargs == 1 or nargs == Nargs('?') else 'append'
             else:
                 action = 'store'
         elif nargs_provided and action == 'store' and nargs.max != 1:
             raise ParameterDefinitionError(f'Invalid {action=} for {nargs=}')
 
-        if (required := 0 not in nargs) and default is not _NotSet:
+        if (required := 0 not in nargs) and (default is not _NotSet or default_cb is not None):
             raise ParameterDefinitionError(
-                f'Invalid {default=} - only allowed for Positional parameters when nargs=? or nargs=*'
+                f'Invalid {default=} or {default_cb=} - only allowed for Positional parameters when nargs=? or nargs=*'
             )
         kwargs.setdefault('required', required)
-        super().__init__(action=action, default=default, **kwargs)
+        super().__init__(action=action, default=default, default_cb=default_cb, **kwargs)
         self.type = normalize_input_type(type, choices)
         self.allow_leading_dash = allow_leading_dash
```

### Comparing `cli_command_parser-2023.7.29/lib/cli_command_parser/parse_tree.py` & `cli_command_parser-2023.7.30/lib/cli_command_parser/parse_tree.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.7.29/lib/cli_command_parser/parser.py` & `cli_command_parser-2023.7.30/lib/cli_command_parser/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     def __init__(self, ctx: Context, params: CommandParameters, config: CommandConfig):
         self._last = None
         self.ctx = ctx
         self.params = params
         self.positionals = params.get_positionals_to_parse(ctx)
         self.config = config
         if config.reject_ambiguous_pos_combos:
-            PosNode.build_tree(ctx.command)
+            PosNode.build_tree(ctx.command_cls)
 
     @classmethod
     def parse_args_and_get_next_cmd(cls, ctx: Context) -> Optional[CommandType]:
         try:
             return cls(ctx, ctx.params, ctx.config).get_next_cmd(ctx)
         except UsageError:
             if not ctx.categorized_action_flags[_PRE_INIT]:
@@ -61,15 +61,15 @@
             return None
 
     def get_next_cmd(self, ctx: Context) -> Optional[CommandType]:
         self._parse_args(ctx)
         self._validate_groups()
         missing = ctx.get_missing()
         if (sub_cmd_param := self.params.sub_command) and (next_cmd := sub_cmd_param.target()) is not None:
-            if missing and not ctx.categorized_action_flags[_PRE_INIT] and get_parent(next_cmd) is not ctx.command:
+            if missing and not ctx.categorized_action_flags[_PRE_INIT] and get_parent(next_cmd) is not ctx.command_cls:
                 raise ParamsMissing(missing)
             return next_cmd
         elif missing and not ctx.config.allow_missing and (not self.params.action or self.params.action not in missing):
             if not ctx.categorized_action_flags[_PRE_INIT]:  # No pre-init action was triggered
                 raise ParamsMissing(missing)
         elif ctx.remaining and not ctx.config.ignore_unknown:  # Note: ctx.remaining is self.deferred at this point
             raise NoSuchOption(f'unrecognized arguments: {" ".join(ctx.remaining)}') from None
```

### Comparing `cli_command_parser-2023.7.29/lib/cli_command_parser/testing.py` & `cli_command_parser-2023.7.30/lib/cli_command_parser/testing.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 ExcType = Type[Exception]
 ExceptionCase = Union[Argv, Tuple[Argv, ExcType], Tuple[Argv, ExcType, str]]
 ExcCases = Iterable[ExceptionCase]
 CallExceptionCase = Union[Tuple[Kwargs, ExcType], Tuple[Kwargs, ExcType, str]]
 CallExceptionCases = Iterable[CallExceptionCase]
 
 OPT_ENV_MOD = 'cli_command_parser.parser.environ'
+EXCLUDE_ACTIONS = (help_action,)
 
 
 class AssertRaisesWithStringContext:
     """
     Simplified version of the stdlib ``_AssertRaisesContext`` that tests whether the raised exception's string contains
     the given text rather than matching it against a regex pattern.  This avoids the regex overhead when it isn't
     necessary, which is the majority of the time for such checks in this project.
@@ -97,15 +98,15 @@
             self.fail(self._formatMessage(msg, f'{d1} != {d2}\n{format_dict_diff(d1, d2)}'))
 
     def assert_raises_contains_str(self, expected_exc: Type[BaseException], expected_text: str, msg: str = None):
         return AssertRaisesWithStringContext(self, expected_exc, expected_text, msg)
 
     def assert_parse_results(self, cmd_cls: CommandCls, argv: Argv, expected: Expected, msg: str = None) -> Command:
         cmd = cmd_cls.parse(argv)
-        parsed = cmd.ctx.get_parsed((help_action,))
+        parsed = cmd.ctx.get_parsed(cmd, exclude=EXCLUDE_ACTIONS)
         self.assert_dict_equal(expected, parsed, msg)
         return cmd
 
     def assert_parse_results_cases(self, cmd_cls: CommandCls, cases: Iterable[Case], msg: str = None):
         for argv, expected in cases:
             with self.subTest(expected='results', argv=argv):
                 self.assert_parse_results(cmd_cls, argv, expected, msg)
```

### Comparing `cli_command_parser-2023.7.29/lib/cli_command_parser/typing.py` & `cli_command_parser-2023.7.30/lib/cli_command_parser/typing.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,16 @@
 NumType = Callable[[Union[str, float, int]], NT]
 RngType = Union[range, int, Sequence[int]]
 
 InputTypeFunc = Union[None, TypeFunc, 'InputType', range, Type['Enum'], Pattern]
 ChoicesType = Optional[Collection[Any]]
 
 Bool = Union[bool, Any]
-Strs = Union[str, Sequence[str]]
+StrSeq = Sequence[str]
+Strs = Union[str, StrSeq]
 OptStr = Optional[str]
 OptStrs = Optional[Strs]
 Strings = Collection[str]
 PathLike = Union[str, 'Path']
 
 Locale = Union[str, Tuple[Optional[str], Optional[str]]]
 TimeBound = Union['datetime', 'date', 'time', 'timedelta', None]
@@ -54,7 +55,10 @@
 ParamList = List[Param]
 ParamOrGroup = Union[Param, 'ParamGroup']
 
 CommandObj = TypeVar('CommandObj', bound='Command')
 CommandType = TypeVar('CommandType', bound='CommandMeta')
 CommandCls = Union[CommandType, Type[CommandObj]]
 CommandAny = Union[CommandCls, CommandObj]
+
+DefaultFunc = Callable[[], T_co]
+CommandMethod = Callable[[CommandObj], T_co]
```

### Comparing `cli_command_parser-2023.7.29/lib/cli_command_parser/utils.py` & `cli_command_parser-2023.7.30/lib/cli_command_parser/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,14 +12,19 @@
 from typing import Any, Callable, TypeVar, List
 
 try:
     from enum import CONFORM
 except ImportError:
     CONFORM = None
 
+try:
+    from wcwidth import wcwidth
+except ImportError:
+    wcwidth = len
+
 FlagEnum = TypeVar('FlagEnum', bound='FixedFlag')
 _NotSet = object()
 
 # region Text Processing / Formatting
 
 
 def camel_to_snake_case(text: str, delim: str = '_') -> str:
@@ -37,14 +42,28 @@
 def _parse_tree_target_repr(target) -> str:
     try:
         return target.__name__
     except AttributeError:
         return repr(target)
 
 
+if wcwidth is len:
+    wcswidth = len
+else:
+
+    def wcswidth(text: str, unicode_version: str = 'auto') -> int:
+        """A version of wcswidth from the wcwidth library, optimized for how it is used in this repo."""
+        width = 0
+        for c in text:
+            if (char_width := wcwidth(c, unicode_version)) < 0:
+                return -1
+            width += char_width
+        return width
+
+
 # endregion
 
 
 class MissingMixin:
     @classmethod
     def _missing_(cls, value):
         if isinstance(value, str):
```

### Comparing `cli_command_parser-2023.7.29/lib/cli_command_parser.egg-info/PKG-INFO` & `cli_command_parser-2023.7.30/lib/cli_command_parser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cli-command-parser
-Version: 2023.7.29
+Version: 2023.7.30
 Summary: CLI Command Parser
 Home-page: https://github.com/dskrypa/cli_command_parser
 Author: Doug Skrypa
 Author-email: dskrypa@gmail.com
 License: Apache 2.0
 Project-URL: Source, https://github.com/dskrypa/cli_command_parser
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cli_command_parser-2023.7.29/lib/cli_command_parser.egg-info/SOURCES.txt` & `cli_command_parser-2023.7.30/lib/cli_command_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.7.29/readme.rst` & `cli_command_parser-2023.7.30/readme.rst`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.7.29/setup.cfg` & `cli_command_parser-2023.7.30/setup.cfg`

 * *Files identical despite different names*

