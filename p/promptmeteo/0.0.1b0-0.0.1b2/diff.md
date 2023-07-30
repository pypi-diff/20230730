# Comparing `tmp/promptmeteo-0.0.1b0.tar.gz` & `tmp/promptmeteo-0.0.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptmeteo-0.0.1b0.tar", last modified: Sun Jul 30 18:48:09 2023, max compression
+gzip compressed data, was "promptmeteo-0.0.1b2.tar", last modified: Sun Jul 30 18:54:51 2023, max compression
```

## Comparing `promptmeteo-0.0.1b0.tar` & `promptmeteo-0.0.1b2.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:48:09.460716 promptmeteo-0.0.1b0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:48:09.452716 promptmeteo-0.0.1b0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:48:09.456716 promptmeteo-0.0.1b0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/.github/workflows/code_lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/.github/workflows/code_testing.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/.github/workflows/publish_docker.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/.github/workflows/publish_package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-07-30 18:48:09.460716 promptmeteo-0.0.1b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:48:09.456716 promptmeteo-0.0.1b0/data/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/data/classification_data.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:48:09.456716 promptmeteo-0.0.1b0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/examples/01_minimal_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/examples/02_parametrization.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/examples/03_save_and_load.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/examples/04_command_example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:48:09.456716 promptmeteo-0.0.1b0/promptmeteo/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/promptmeteo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10878 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/promptmeteo/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:48:09.456716 promptmeteo-0.0.1b0/promptmeteo/models/
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/promptmeteo/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/promptmeteo/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/promptmeteo/models/fake_llm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/promptmeteo/models/hf_hub_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/promptmeteo/models/hf_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/promptmeteo/models/openai.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:48:09.456716 promptmeteo-0.0.1b0/promptmeteo/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/promptmeteo/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/promptmeteo/parsers/classification_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/promptmeteo/parsers/dummy_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:48:09.456716 promptmeteo-0.0.1b0/promptmeteo/promptmeteo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-07-30 18:48:09.000000 promptmeteo-0.0.1b0/promptmeteo/promptmeteo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-30 18:48:09.000000 promptmeteo-0.0.1b0/promptmeteo/promptmeteo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 18:48:09.000000 promptmeteo-0.0.1b0/promptmeteo/promptmeteo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-30 18:48:09.000000 promptmeteo-0.0.1b0/promptmeteo/promptmeteo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 18:48:09.000000 promptmeteo-0.0.1b0/promptmeteo/promptmeteo.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:48:09.456716 promptmeteo-0.0.1b0/promptmeteo/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/promptmeteo/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6906 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/promptmeteo/prompts/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/promptmeteo/prompts/classification_prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/promptmeteo/prompts/ner_prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:48:09.456716 promptmeteo-0.0.1b0/promptmeteo/prompts/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/promptmeteo/prompts/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:48:09.460716 promptmeteo-0.0.1b0/promptmeteo/prompts/templates/sp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/promptmeteo/prompts/templates/sp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/promptmeteo/prompts/templates/sp/classification_prompt.yml
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/promptmeteo/prompts/templates/sp/ner_prompt.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:48:09.460716 promptmeteo-0.0.1b0/promptmeteo/selector/
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/promptmeteo/selector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/promptmeteo/selector/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/promptmeteo/selector/marginal_relevance_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/promptmeteo/selector/semantic_similarity_selector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:48:09.460716 promptmeteo-0.0.1b0/promptmeteo/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/promptmeteo/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8067 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/promptmeteo/tasks/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/promptmeteo/tasks/classification_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/promptmeteo/tasks/ner_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     4739 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 18:48:09.460716 promptmeteo-0.0.1b0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:48:09.460716 promptmeteo-0.0.1b0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9283 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/tests/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/tests/test_prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/tests/test_selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-07-30 18:47:57.000000 promptmeteo-0.0.1b0/tests/test_task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:54:51.194786 promptmeteo-0.0.1b2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:54:51.186786 promptmeteo-0.0.1b2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:54:51.190786 promptmeteo-0.0.1b2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-30 18:54:40.000000 promptmeteo-0.0.1b2/.github/workflows/code_lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-30 18:54:40.000000 promptmeteo-0.0.1b2/.github/workflows/code_testing.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-07-30 18:54:40.000000 promptmeteo-0.0.1b2/.github/workflows/publish_docker.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-07-30 18:54:40.000000 promptmeteo-0.0.1b2/.github/workflows/publish_package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-30 18:54:40.000000 promptmeteo-0.0.1b2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-30 18:54:40.000000 promptmeteo-0.0.1b2/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-30 18:54:40.000000 promptmeteo-0.0.1b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-30 18:54:40.000000 promptmeteo-0.0.1b2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-07-30 18:54:51.194786 promptmeteo-0.0.1b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-07-30 18:54:40.000000 promptmeteo-0.0.1b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:54:51.190786 promptmeteo-0.0.1b2/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-30 18:54:40.000000 promptmeteo-0.0.1b2/data/classification_data.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:54:51.190786 promptmeteo-0.0.1b2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-30 18:54:40.000000 promptmeteo-0.0.1b2/examples/01_minimal_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-07-30 18:54:40.000000 promptmeteo-0.0.1b2/examples/02_parametrization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-30 18:54:40.000000 promptmeteo-0.0.1b2/examples/03_save_and_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-30 18:54:40.000000 promptmeteo-0.0.1b2/examples/04_command_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:54:51.190786 promptmeteo-0.0.1b2/promptmeteo/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-30 18:54:40.000000 promptmeteo-0.0.1b2/promptmeteo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10878 2023-07-30 18:54:40.000000 promptmeteo-0.0.1b2/promptmeteo/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:54:51.190786 promptmeteo-0.0.1b2/promptmeteo/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-07-30 18:54:40.000000 promptmeteo-0.0.1b2/promptmeteo/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-07-30 18:54:40.000000 promptmeteo-0.0.1b2/promptmeteo/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-07-30 18:54:40.000000 promptmeteo-0.0.1b2/promptmeteo/models/fake_llm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-30 18:54:40.000000 promptmeteo-0.0.1b2/promptmeteo/models/hf_hub_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-07-30 18:54:40.000000 promptmeteo-0.0.1b2/promptmeteo/models/hf_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-07-30 18:54:40.000000 promptmeteo-0.0.1b2/promptmeteo/models/openai.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:54:51.190786 promptmeteo-0.0.1b2/promptmeteo/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-07-30 18:54:40.000000 promptmeteo-0.0.1b2/promptmeteo/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-07-30 18:54:40.000000 promptmeteo-0.0.1b2/promptmeteo/parsers/classification_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-07-30 18:54:40.000000 promptmeteo-0.0.1b2/promptmeteo/parsers/dummy_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:54:51.190786 promptmeteo-0.0.1b2/promptmeteo/promptmeteo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-07-30 18:54:51.000000 promptmeteo-0.0.1b2/promptmeteo/promptmeteo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-30 18:54:51.000000 promptmeteo-0.0.1b2/promptmeteo/promptmeteo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 18:54:51.000000 promptmeteo-0.0.1b2/promptmeteo/promptmeteo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-30 18:54:51.000000 promptmeteo-0.0.1b2/promptmeteo/promptmeteo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 18:54:51.000000 promptmeteo-0.0.1b2/promptmeteo/promptmeteo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:54:51.190786 promptmeteo-0.0.1b2/promptmeteo/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-30 18:54:40.000000 promptmeteo-0.0.1b2/promptmeteo/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6906 2023-07-30 18:54:40.000000 promptmeteo-0.0.1b2/promptmeteo/prompts/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-30 18:54:40.000000 promptmeteo-0.0.1b2/promptmeteo/prompts/classification_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-07-30 18:54:40.000000 promptmeteo-0.0.1b2/promptmeteo/prompts/ner_prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:54:51.190786 promptmeteo-0.0.1b2/promptmeteo/prompts/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 18:54:40.000000 promptmeteo-0.0.1b2/promptmeteo/prompts/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:54:51.190786 promptmeteo-0.0.1b2/promptmeteo/prompts/templates/sp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 18:54:40.000000 promptmeteo-0.0.1b2/promptmeteo/prompts/templates/sp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-30 18:54:40.000000 promptmeteo-0.0.1b2/promptmeteo/prompts/templates/sp/classification_prompt.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-30 18:54:40.000000 promptmeteo-0.0.1b2/promptmeteo/prompts/templates/sp/ner_prompt.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:54:51.194786 promptmeteo-0.0.1b2/promptmeteo/selector/
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-07-30 18:54:40.000000 promptmeteo-0.0.1b2/promptmeteo/selector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-07-30 18:54:40.000000 promptmeteo-0.0.1b2/promptmeteo/selector/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-07-30 18:54:40.000000 promptmeteo-0.0.1b2/promptmeteo/selector/marginal_relevance_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-30 18:54:40.000000 promptmeteo-0.0.1b2/promptmeteo/selector/semantic_similarity_selector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:54:51.194786 promptmeteo-0.0.1b2/promptmeteo/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-30 18:54:40.000000 promptmeteo-0.0.1b2/promptmeteo/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8067 2023-07-30 18:54:40.000000 promptmeteo-0.0.1b2/promptmeteo/tasks/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-07-30 18:54:40.000000 promptmeteo-0.0.1b2/promptmeteo/tasks/classification_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-07-30 18:54:40.000000 promptmeteo-0.0.1b2/promptmeteo/tasks/ner_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-30 18:54:40.000000 promptmeteo-0.0.1b2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     4739 2023-07-30 18:54:40.000000 promptmeteo-0.0.1b2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 18:54:51.194786 promptmeteo-0.0.1b2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:54:51.194786 promptmeteo-0.0.1b2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9283 2023-07-30 18:54:40.000000 promptmeteo-0.0.1b2/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-07-30 18:54:40.000000 promptmeteo-0.0.1b2/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-30 18:54:40.000000 promptmeteo-0.0.1b2/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-30 18:54:40.000000 promptmeteo-0.0.1b2/tests/test_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-07-30 18:54:40.000000 promptmeteo-0.0.1b2/tests/test_selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-07-30 18:54:40.000000 promptmeteo-0.0.1b2/tests/test_task.py
```

### Comparing `promptmeteo-0.0.1b0/.github/workflows/code_lint.yml` & `promptmeteo-0.0.1b2/.github/workflows/code_lint.yml`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.1b0/.github/workflows/code_testing.yml` & `promptmeteo-0.0.1b2/.github/workflows/code_testing.yml`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.1b0/.github/workflows/publish_docker.yml` & `promptmeteo-0.0.1b2/.github/workflows/publish_docker.yml`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.1b0/.github/workflows/publish_package.yml` & `promptmeteo-0.0.1b2/.github/workflows/publish_package.yml`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.1b0/.gitignore` & `promptmeteo-0.0.1b2/.gitignore`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.1b0/Dockerfile` & `promptmeteo-0.0.1b2/Dockerfile`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.1b0/LICENSE` & `promptmeteo-0.0.1b2/LICENSE`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.1b0/PKG-INFO` & `promptmeteo-0.0.1b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptmeteo
-Version: 0.0.1b0
+Version: 0.0.1b2
 Summary: Enable the use of LLMs as a conventional ML model
 Author-email: Angel Delgado <adelgado@paradigmadigital.com>
 License: MIT License
         
         Copyright (c) 2023 Paradigma Digital S.L.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `promptmeteo-0.0.1b0/README.md` & `promptmeteo-0.0.1b2/README.md`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.1b0/examples/01_minimal_example.py` & `promptmeteo-0.0.1b2/examples/01_minimal_example.py`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.1b0/examples/02_parametrization.py` & `promptmeteo-0.0.1b2/examples/02_parametrization.py`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.1b0/examples/03_save_and_load.py` & `promptmeteo-0.0.1b2/examples/03_save_and_load.py`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.1b0/examples/04_command_example.py` & `promptmeteo-0.0.1b2/examples/04_command_example.py`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.1b0/promptmeteo/main.py` & `promptmeteo-0.0.1b2/promptmeteo/main.py`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.1b0/promptmeteo/models/__init__.py` & `promptmeteo-0.0.1b2/promptmeteo/models/__init__.py`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.1b0/promptmeteo/models/base.py` & `promptmeteo-0.0.1b2/promptmeteo/models/base.py`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.1b0/promptmeteo/models/fake_llm.py` & `promptmeteo-0.0.1b2/promptmeteo/models/fake_llm.py`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.1b0/promptmeteo/models/hf_hub_api.py` & `promptmeteo-0.0.1b2/promptmeteo/models/hf_hub_api.py`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.1b0/promptmeteo/models/hf_pipeline.py` & `promptmeteo-0.0.1b2/promptmeteo/models/hf_pipeline.py`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.1b0/promptmeteo/models/openai.py` & `promptmeteo-0.0.1b2/promptmeteo/models/openai.py`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.1b0/promptmeteo/parsers/__init__.py` & `promptmeteo-0.0.1b2/promptmeteo/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.1b0/promptmeteo/parsers/classification_parser.py` & `promptmeteo-0.0.1b2/promptmeteo/parsers/classification_parser.py`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.1b0/promptmeteo/parsers/dummy_parser.py` & `promptmeteo-0.0.1b2/promptmeteo/parsers/dummy_parser.py`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.1b0/promptmeteo/promptmeteo.egg-info/PKG-INFO` & `promptmeteo-0.0.1b2/promptmeteo/promptmeteo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptmeteo
-Version: 0.0.1b0
+Version: 0.0.1b2
 Summary: Enable the use of LLMs as a conventional ML model
 Author-email: Angel Delgado <adelgado@paradigmadigital.com>
 License: MIT License
         
         Copyright (c) 2023 Paradigma Digital S.L.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `promptmeteo-0.0.1b0/promptmeteo/promptmeteo.egg-info/SOURCES.txt` & `promptmeteo-0.0.1b2/promptmeteo/promptmeteo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.1b0/promptmeteo/prompts/base.py` & `promptmeteo-0.0.1b2/promptmeteo/prompts/base.py`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.1b0/promptmeteo/prompts/classification_prompt.py` & `promptmeteo-0.0.1b2/promptmeteo/prompts/classification_prompt.py`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.1b0/promptmeteo/prompts/ner_prompt.py` & `promptmeteo-0.0.1b2/promptmeteo/prompts/ner_prompt.py`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.1b0/promptmeteo/prompts/templates/sp/classification_prompt.yml` & `promptmeteo-0.0.1b2/promptmeteo/prompts/templates/sp/classification_prompt.yml`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.1b0/promptmeteo/prompts/templates/sp/ner_prompt.yml` & `promptmeteo-0.0.1b2/promptmeteo/prompts/templates/sp/ner_prompt.yml`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.1b0/promptmeteo/selector/__init__.py` & `promptmeteo-0.0.1b2/promptmeteo/selector/__init__.py`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.1b0/promptmeteo/selector/base.py` & `promptmeteo-0.0.1b2/promptmeteo/selector/base.py`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.1b0/promptmeteo/selector/marginal_relevance_selector.py` & `promptmeteo-0.0.1b2/promptmeteo/selector/marginal_relevance_selector.py`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.1b0/promptmeteo/selector/semantic_similarity_selector.py` & `promptmeteo-0.0.1b2/promptmeteo/selector/semantic_similarity_selector.py`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.1b0/promptmeteo/tasks/__init__.py` & `promptmeteo-0.0.1b2/promptmeteo/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.1b0/promptmeteo/tasks/base.py` & `promptmeteo-0.0.1b2/promptmeteo/tasks/base.py`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.1b0/promptmeteo/tasks/classification_task.py` & `promptmeteo-0.0.1b2/promptmeteo/tasks/classification_task.py`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.1b0/promptmeteo/tasks/ner_task.py` & `promptmeteo-0.0.1b2/promptmeteo/tasks/ner_task.py`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.1b0/pyproject.toml` & `promptmeteo-0.0.1b2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.1b0/requirements.txt` & `promptmeteo-0.0.1b2/requirements.txt`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.1b0/tests/test_main.py` & `promptmeteo-0.0.1b2/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.1b0/tests/test_models.py` & `promptmeteo-0.0.1b2/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.1b0/tests/test_parsers.py` & `promptmeteo-0.0.1b2/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.1b0/tests/test_prompts.py` & `promptmeteo-0.0.1b2/tests/test_prompts.py`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.1b0/tests/test_selectors.py` & `promptmeteo-0.0.1b2/tests/test_selectors.py`

 * *Files identical despite different names*

### Comparing `promptmeteo-0.0.1b0/tests/test_task.py` & `promptmeteo-0.0.1b2/tests/test_task.py`

 * *Files identical despite different names*

