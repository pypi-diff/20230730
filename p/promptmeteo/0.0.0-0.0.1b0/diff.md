# Comparing `tmp/promptmeteo-0.0.0.tar.gz` & `tmp/promptmeteo-0.0.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptmeteo-0.0.0.tar", last modified: Sat Jul 29 23:56:20 2023, max compression
+gzip compressed data, was "promptmeteo-0.0.1b0.tar", last modified: Sun Jul 30 18:48:09 2023, max compression
```

## Comparing `promptmeteo-0.0.0.tar` & `promptmeteo-0.0.1b0.tar`

### file list

```diff
@@ -1,55 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 23:56:20.962172 promptmeteo-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-29 23:56:06.000000 promptmeteo-0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-07-29 23:56:20.962172 promptmeteo-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-07-29 23:56:06.000000 promptmeteo-0.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-07-29 23:56:06.000000 promptmeteo-0.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 23:56:20.962172 promptmeteo-0.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 23:56:20.950172 promptmeteo-0.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 23:56:20.954172 promptmeteo-0.0.0/src/promptmeteo/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-29 23:56:06.000000 promptmeteo-0.0.0/src/promptmeteo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10882 2023-07-29 23:56:06.000000 promptmeteo-0.0.0/src/promptmeteo/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 23:56:20.958172 promptmeteo-0.0.0/src/promptmeteo/models/
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-07-29 23:56:06.000000 promptmeteo-0.0.0/src/promptmeteo/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-07-29 23:56:06.000000 promptmeteo-0.0.0/src/promptmeteo/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-07-29 23:56:06.000000 promptmeteo-0.0.0/src/promptmeteo/models/fake_llm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-29 23:56:06.000000 promptmeteo-0.0.0/src/promptmeteo/models/hf_hub_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-07-29 23:56:06.000000 promptmeteo-0.0.0/src/promptmeteo/models/hf_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-07-29 23:56:06.000000 promptmeteo-0.0.0/src/promptmeteo/models/openai.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 23:56:20.958172 promptmeteo-0.0.0/src/promptmeteo/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-07-29 23:56:06.000000 promptmeteo-0.0.0/src/promptmeteo/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-07-29 23:56:06.000000 promptmeteo-0.0.0/src/promptmeteo/parsers/classification_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-07-29 23:56:06.000000 promptmeteo-0.0.0/src/promptmeteo/parsers/dummy_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 23:56:20.958172 promptmeteo-0.0.0/src/promptmeteo/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-29 23:56:06.000000 promptmeteo-0.0.0/src/promptmeteo/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6859 2023-07-29 23:56:06.000000 promptmeteo-0.0.0/src/promptmeteo/prompts/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-29 23:56:06.000000 promptmeteo-0.0.0/src/promptmeteo/prompts/classification_prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-07-29 23:56:06.000000 promptmeteo-0.0.0/src/promptmeteo/prompts/ner_prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 23:56:20.958172 promptmeteo-0.0.0/src/promptmeteo/prompts/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 23:56:06.000000 promptmeteo-0.0.0/src/promptmeteo/prompts/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 23:56:20.958172 promptmeteo-0.0.0/src/promptmeteo/prompts/templates/sp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 23:56:06.000000 promptmeteo-0.0.0/src/promptmeteo/prompts/templates/sp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-29 23:56:06.000000 promptmeteo-0.0.0/src/promptmeteo/prompts/templates/sp/classification_prompt.yml
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-29 23:56:06.000000 promptmeteo-0.0.0/src/promptmeteo/prompts/templates/sp/ner_prompt.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 23:56:20.962172 promptmeteo-0.0.0/src/promptmeteo/selector/
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-07-29 23:56:06.000000 promptmeteo-0.0.0/src/promptmeteo/selector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-07-29 23:56:06.000000 promptmeteo-0.0.0/src/promptmeteo/selector/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-07-29 23:56:06.000000 promptmeteo-0.0.0/src/promptmeteo/selector/marginal_relevance_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-29 23:56:06.000000 promptmeteo-0.0.0/src/promptmeteo/selector/semantic_similarity_selector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 23:56:20.962172 promptmeteo-0.0.0/src/promptmeteo/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-29 23:56:06.000000 promptmeteo-0.0.0/src/promptmeteo/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8067 2023-07-29 23:56:06.000000 promptmeteo-0.0.0/src/promptmeteo/tasks/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-07-29 23:56:06.000000 promptmeteo-0.0.0/src/promptmeteo/tasks/classification_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-07-29 23:56:06.000000 promptmeteo-0.0.0/src/promptmeteo/tasks/ner_task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 23:56:20.954172 promptmeteo-0.0.0/src/promptmeteo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-07-29 23:56:20.000000 promptmeteo-0.0.0/src/promptmeteo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-29 23:56:20.000000 promptmeteo-0.0.0/src/promptmeteo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 23:56:20.000000 promptmeteo-0.0.0/src/promptmeteo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-29 23:56:20.000000 promptmeteo-0.0.0/src/promptmeteo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-29 23:56:20.000000 promptmeteo-0.0.0/src/promptmeteo.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 23:56:20.962172 promptmeteo-0.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9283 2023-07-29 23:56:06.000000 promptmeteo-0.0.0/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-07-29 23:56:06.000000 promptmeteo-0.0.0/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-29 23:56:06.000000 promptmeteo-0.0.0/tests/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-29 23:56:06.000000 promptmeteo-0.0.0/tests/test_prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-07-29 23:56:06.000000 promptmeteo-0.0.0/tests/test_selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-07-29 23:56:06.000000 promptmeteo-0.0.0/tests/test_task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:48:09.460716 promptmeteo-0.0.1b0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:48:09.452716 promptmeteo-0.0.1b0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:48:09.456716 promptmeteo-0.0.1b0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/.github/workflows/code_lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/.github/workflows/code_testing.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/.github/workflows/publish_docker.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/.github/workflows/publish_package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-07-30 18:48:09.460716 promptmeteo-0.0.1b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:48:09.456716 promptmeteo-0.0.1b0/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/data/classification_data.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:48:09.456716 promptmeteo-0.0.1b0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/examples/01_minimal_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/examples/02_parametrization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/examples/03_save_and_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/examples/04_command_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:48:09.456716 promptmeteo-0.0.1b0/promptmeteo/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/promptmeteo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10878 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/promptmeteo/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:48:09.456716 promptmeteo-0.0.1b0/promptmeteo/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/promptmeteo/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/promptmeteo/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/promptmeteo/models/fake_llm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/promptmeteo/models/hf_hub_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/promptmeteo/models/hf_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/promptmeteo/models/openai.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:48:09.456716 promptmeteo-0.0.1b0/promptmeteo/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/promptmeteo/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/promptmeteo/parsers/classification_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/promptmeteo/parsers/dummy_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:48:09.456716 promptmeteo-0.0.1b0/promptmeteo/promptmeteo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-07-30 18:48:09.000000 promptmeteo-0.0.1b0/promptmeteo/promptmeteo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-30 18:48:09.000000 promptmeteo-0.0.1b0/promptmeteo/promptmeteo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 18:48:09.000000 promptmeteo-0.0.1b0/promptmeteo/promptmeteo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-30 18:48:09.000000 promptmeteo-0.0.1b0/promptmeteo/promptmeteo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 18:48:09.000000 promptmeteo-0.0.1b0/promptmeteo/promptmeteo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:48:09.456716 promptmeteo-0.0.1b0/promptmeteo/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/promptmeteo/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6906 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/promptmeteo/prompts/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/promptmeteo/prompts/classification_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/promptmeteo/prompts/ner_prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:48:09.456716 promptmeteo-0.0.1b0/promptmeteo/prompts/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/promptmeteo/prompts/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:48:09.460716 promptmeteo-0.0.1b0/promptmeteo/prompts/templates/sp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/promptmeteo/prompts/templates/sp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/promptmeteo/prompts/templates/sp/classification_prompt.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/promptmeteo/prompts/templates/sp/ner_prompt.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:48:09.460716 promptmeteo-0.0.1b0/promptmeteo/selector/
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/promptmeteo/selector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/promptmeteo/selector/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/promptmeteo/selector/marginal_relevance_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/promptmeteo/selector/semantic_similarity_selector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:48:09.460716 promptmeteo-0.0.1b0/promptmeteo/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/promptmeteo/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8067 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/promptmeteo/tasks/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/promptmeteo/tasks/classification_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/promptmeteo/tasks/ner_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     4739 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 18:48:09.460716 promptmeteo-0.0.1b0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:48:09.460716 promptmeteo-0.0.1b0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9283 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/tests/test_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/tests/test_selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/tests/test_task.py
```

### Comparing `promptmeteo-0.0.0/LICENSE` & `promptmeteo-0.0.1b0/LICENSE`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.0/pyproject.toml` & `promptmeteo-0.0.1b0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,48 @@
 [build-system]
-requires = ["setuptools>=65.0.0", "wheel >= 0.38"]
+requires = ["setuptools>=65.0.0", "wheel >= 0.38", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "promptmeteo"
-version = "0.0.0"
-description = "Label, clean and enrich text datasets with LLMs"
+dynamic = ["version"]
+description = "Enable the use of LLMs as a conventional ML model"
 readme = "README.md"
 authors = [{ name = "Angel Delgado", email = "adelgado@paradigmadigital.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
-requires-python = ">=3.10"
+requires-python = ">=3.8"
 dependencies = [
     "langchain == 0.0.234",
     "torch == 2.0.1",
     "pydantic == 1.10.11",
     "faiss-cpu == 1.7.4",
     "transformers ==4.31.0",
     "openai==0.27.8",
     "sentence-transformers==2.2.2"
 ]
 
+[tool.setuptools_scm]
 
 [tool.setuptools.packages.find]
-where = ["src"]
+where = ["promptmeteo"]
 
 [tool.setuptools.package-data]
 "promptmeteo.prompts.templates.sp" = ["*.yml"]
-#"*" = ["*.yml"]
 
 [project.optional-dependencies]
 all = [
     "black",
+    "coverage",
     "bumpver",
     "pip-tools",
+    "pylint",
     "pytest",
+    "pytest-cov",
     "pytest-mock",
-    "openai >= 0.27.4",
-    "tiktoken >= 0.3.3",
-    "transformers >= 4.25.0",
-    "google-cloud-aiplatform>=1.25.0",
 ]
```

### Comparing `promptmeteo-0.0.0/src/promptmeteo/main.py` & `promptmeteo-0.0.1b0/promptmeteo/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 import sys
 import tarfile
 import tempfile
 from typing import List
 from typing import Dict
 from typing import Optional
 
-from langchain.schema import LLMResult
 from promptmeteo.tasks import TaskBuilderFactory
 
 
 class Promptmeteo():
 
 
     def __init__(
@@ -171,14 +170,16 @@
 
     def read_prompt_file(
         self,
         prompt_text : str
     ) -> None:
 
         self.task.prompt.read_prompt_file(prompt_text)
+        self.task.prompt.__init__()
+
         return self
 
 
     def predict(
         self,
         examples : List[str],
     ):
@@ -322,15 +323,15 @@
             raise ValueError(
                 f'{self.__class__.__name__} error in `save_model()`. '
                 f'directory {model_dir} does not exists.'
             )
 
         with tempfile.TemporaryDirectory() as tmp:
 
-            tmp_path = os.path.join(tmp,model_name.removesuffix('.meteo'))
+            tmp_path = os.path.join(tmp,model_name.replace('.meteo',''))
             self.task.selector.vectorstore.save_local(tmp_path)
 
             with tarfile.open(model_path, mode="w:gz") as tar:
                 tar.add(tmp_path, arcname=model_name)
 
         return self
```

### Comparing `promptmeteo-0.0.0/src/promptmeteo/models/__init__.py` & `promptmeteo-0.0.1b0/promptmeteo/models/__init__.py`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.0/src/promptmeteo/models/base.py` & `promptmeteo-0.0.1b0/promptmeteo/models/base.py`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.0/src/promptmeteo/models/fake_llm.py` & `promptmeteo-0.0.1b0/promptmeteo/models/fake_llm.py`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.0/src/promptmeteo/models/hf_hub_api.py` & `promptmeteo-0.0.1b0/promptmeteo/models/hf_hub_api.py`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.0/src/promptmeteo/models/hf_pipeline.py` & `promptmeteo-0.0.1b0/promptmeteo/models/hf_pipeline.py`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.0/src/promptmeteo/models/openai.py` & `promptmeteo-0.0.1b0/promptmeteo/models/openai.py`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.0/src/promptmeteo/parsers/__init__.py` & `promptmeteo-0.0.1b0/promptmeteo/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.0/src/promptmeteo/parsers/classification_parser.py` & `promptmeteo-0.0.1b0/promptmeteo/parsers/classification_parser.py`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.0/src/promptmeteo/parsers/dummy_parser.py` & `promptmeteo-0.0.1b0/promptmeteo/parsers/dummy_parser.py`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.0/src/promptmeteo/prompts/base.py` & `promptmeteo-0.0.1b0/promptmeteo/prompts/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -116,21 +116,22 @@
         --------
 
         prompt : Prompt
             Text with the reasulting prompt.
 
         Example
         -------
-        >>> from promptmeteo.prompts.sp import BasePrompt as CP
-        >>>
-        >>> CP(
-        >>>     prompt_labels            = CP.PROMPT_LABELS,
-        >>>     prompt_task_info         = CP.PROMPT_TASK_INFO,
-        >>>     prompt_answer_format     = CP.PROMPT_ANSWER_FORMAT,
-        >>>     prompt_chain_of_thoughts = CP.PROMPT_CHAIN_OF_THOUGHTS,
+        ```
+        >>> from promptmeteo.prompts.sp import BasePrompt
+
+        >>> BasePrompt(
+        >>>     prompt_labels            = BasePrompt.PROMPT_LABELS,
+        >>>     prompt_task_info         = BasePrompt.PROMPT_TASK_INFO,
+        >>>     prompt_answer_format     = BasePrompt.PROMPT_ANSWER_FORMAT,
+        >>>     prompt_chain_of_thoughts = BasePrompt.PROMPT_CHAIN_OF_THOUGHTS,
         >>> ).build()
 
         Clasifica el siguiente texto en una de las siguientes clases:
 
         positivo, negativo, neutro.
 
         Asume que estamos usando estas categorías con su significado subjetivo
@@ -145,14 +146,15 @@
 
         Por favor argumenta tu respuesta paso a paso, explica por qué crees
         que está justificada tu elección final, y por favor asegúrate de que
         acabas tu explicación con el nombre de la clase que has escogido como
         la correcta, en minúscula y sin puntuación.
 
         Éste es el texto que debes clasificar: "{__INPUT__}"
+        ```
         """
 
         self._labels = prompt_labels
 
         prompt_labels = PromptTemplate.from_template(_format(
             ', '.join(prompt_labels)))
```

### Comparing `promptmeteo-0.0.0/src/promptmeteo/prompts/classification_prompt.py` & `promptmeteo-0.0.1b0/promptmeteo/prompts/classification_prompt.py`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.0/src/promptmeteo/prompts/ner_prompt.py` & `promptmeteo-0.0.1b0/promptmeteo/prompts/ner_prompt.py`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.0/src/promptmeteo/prompts/templates/sp/classification_prompt.yml` & `promptmeteo-0.0.1b0/promptmeteo/prompts/templates/sp/classification_prompt.yml`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.0/src/promptmeteo/prompts/templates/sp/ner_prompt.yml` & `promptmeteo-0.0.1b0/promptmeteo/prompts/templates/sp/ner_prompt.yml`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.0/src/promptmeteo/selector/__init__.py` & `promptmeteo-0.0.1b0/promptmeteo/selector/__init__.py`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.0/src/promptmeteo/selector/base.py` & `promptmeteo-0.0.1b0/promptmeteo/selector/base.py`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.0/src/promptmeteo/selector/marginal_relevance_selector.py` & `promptmeteo-0.0.1b0/promptmeteo/selector/marginal_relevance_selector.py`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.0/src/promptmeteo/selector/semantic_similarity_selector.py` & `promptmeteo-0.0.1b0/promptmeteo/selector/semantic_similarity_selector.py`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.0/src/promptmeteo/tasks/__init__.py` & `promptmeteo-0.0.1b0/promptmeteo/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.0/src/promptmeteo/tasks/base.py` & `promptmeteo-0.0.1b0/promptmeteo/tasks/base.py`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.0/src/promptmeteo/tasks/classification_task.py` & `promptmeteo-0.0.1b0/promptmeteo/tasks/classification_task.py`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.0/src/promptmeteo/tasks/ner_task.py` & `promptmeteo-0.0.1b0/promptmeteo/tasks/ner_task.py`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.0/tests/test_main.py` & `promptmeteo-0.0.1b0/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.0/tests/test_models.py` & `promptmeteo-0.0.1b0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.0/tests/test_parsers.py` & `promptmeteo-0.0.1b0/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.0/tests/test_prompts.py` & `promptmeteo-0.0.1b0/tests/test_prompts.py`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.0/tests/test_selectors.py` & `promptmeteo-0.0.1b0/tests/test_selectors.py`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.0/tests/test_task.py` & `promptmeteo-0.0.1b0/tests/test_task.py`

 * *Files identical despite different names*

