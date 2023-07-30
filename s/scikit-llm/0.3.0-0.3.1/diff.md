# Comparing `tmp/scikit-llm-0.3.0.tar.gz` & `tmp/scikit-llm-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit-llm-0.3.0.tar", last modified: Tue Jul  4 20:13:20 2023, max compression
+gzip compressed data, was "scikit-llm-0.3.1.tar", last modified: Sun Jul 30 11:22:37 2023, max compression
```

## Comparing `scikit-llm-0.3.0.tar` & `scikit-llm-0.3.1.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-04 20:13:20.026403 scikit-llm-0.3.0/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     1077 2023-06-17 15:57:54.000000 scikit-llm-0.3.0/LICENSE
--rw-rw-r--   0 oleg      (1000) oleg      (1000)    12301 2023-07-04 20:13:20.026403 scikit-llm-0.3.0/PKG-INFO
--rw-rw-r--   0 oleg      (1000) oleg      (1000)    11747 2023-07-04 20:09:01.000000 scikit-llm-0.3.0/README.md
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     1983 2023-07-04 20:12:37.000000 scikit-llm-0.3.0/pyproject.toml
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-04 20:13:20.022403 scikit-llm-0.3.0/scikit_llm.egg-info/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)    12301 2023-07-04 20:13:20.000000 scikit-llm-0.3.0/scikit_llm.egg-info/PKG-INFO
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     1231 2023-07-04 20:13:20.000000 scikit-llm-0.3.0/scikit_llm.egg-info/SOURCES.txt
--rw-rw-r--   0 oleg      (1000) oleg      (1000)        1 2023-07-04 20:13:20.000000 scikit-llm-0.3.0/scikit_llm.egg-info/dependency_links.txt
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      149 2023-07-04 20:13:20.000000 scikit-llm-0.3.0/scikit_llm.egg-info/requires.txt
--rw-rw-r--   0 oleg      (1000) oleg      (1000)        6 2023-07-04 20:13:20.000000 scikit-llm-0.3.0/scikit_llm.egg-info/top_level.txt
--rw-rw-r--   0 oleg      (1000) oleg      (1000)       38 2023-07-04 20:13:20.026403 scikit-llm-0.3.0/setup.cfg
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-04 20:13:20.022403 scikit-llm-0.3.0/skllm/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      317 2023-07-04 20:07:18.000000 scikit-llm-0.3.0/skllm/__init__.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      740 2023-07-04 20:07:18.000000 scikit-llm-0.3.0/skllm/completions.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     2960 2023-07-04 20:07:18.000000 scikit-llm-0.3.0/skllm/config.py
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-04 20:13:20.022403 scikit-llm-0.3.0/skllm/datasets/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      273 2023-06-17 15:57:54.000000 scikit-llm-0.3.0/skllm/datasets/__init__.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     5870 2023-06-17 15:57:54.000000 scikit-llm-0.3.0/skllm/datasets/multi_class.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     1438 2023-06-17 15:57:54.000000 scikit-llm-0.3.0/skllm/datasets/multi_label.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     2729 2023-06-17 15:57:54.000000 scikit-llm-0.3.0/skllm/datasets/summarization.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      818 2023-06-17 15:57:54.000000 scikit-llm-0.3.0/skllm/datasets/translation.py
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-04 20:13:20.022403 scikit-llm-0.3.0/skllm/google/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     1403 2023-07-04 20:07:18.000000 scikit-llm-0.3.0/skllm/google/completions.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      507 2023-07-04 20:07:18.000000 scikit-llm-0.3.0/skllm/google/tuning.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      992 2023-06-17 15:57:54.000000 scikit-llm-0.3.0/skllm/gpt4all_client.py
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-04 20:13:20.022403 scikit-llm-0.3.0/skllm/memory/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)       49 2023-06-17 15:57:54.000000 scikit-llm-0.3.0/skllm/memory/__init__.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     3269 2023-06-17 15:57:54.000000 scikit-llm-0.3.0/skllm/memory/_annoy.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     1027 2023-06-17 15:57:54.000000 scikit-llm-0.3.0/skllm/memory/base.py
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-04 20:13:20.022403 scikit-llm-0.3.0/skllm/models/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     5956 2023-07-04 20:07:18.000000 scikit-llm-0.3.0/skllm/models/_base.py
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-04 20:13:20.026403 scikit-llm-0.3.0/skllm/models/gpt/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      260 2023-07-04 20:07:18.000000 scikit-llm-0.3.0/skllm/models/gpt/__init__.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     4049 2023-07-04 20:07:18.000000 scikit-llm-0.3.0/skllm/models/gpt/gpt_dyn_few_shot_clf.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     1827 2023-07-04 20:07:18.000000 scikit-llm-0.3.0/skllm/models/gpt/gpt_few_shot_clf.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     5829 2023-07-04 20:07:18.000000 scikit-llm-0.3.0/skllm/models/gpt/gpt_zero_shot_clf.py
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-04 20:13:20.026403 scikit-llm-0.3.0/skllm/models/palm/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      122 2023-07-04 20:07:18.000000 scikit-llm-0.3.0/skllm/models/palm/__init__.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     4854 2023-07-04 20:07:18.000000 scikit-llm-0.3.0/skllm/models/palm/palm_clf.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     2313 2023-07-04 20:07:18.000000 scikit-llm-0.3.0/skllm/models/palm/palm_est.py
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-04 20:13:20.026403 scikit-llm-0.3.0/skllm/openai/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     2829 2023-07-04 20:07:18.000000 scikit-llm-0.3.0/skllm/openai/base_gpt.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     2074 2023-07-04 20:07:18.000000 scikit-llm-0.3.0/skllm/openai/chatgpt.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      730 2023-07-04 20:07:18.000000 scikit-llm-0.3.0/skllm/openai/credentials.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     1441 2023-06-17 15:57:54.000000 scikit-llm-0.3.0/skllm/openai/embeddings.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     1200 2023-06-17 21:25:38.000000 scikit-llm-0.3.0/skllm/openai/mixin.py
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-04 20:13:20.026403 scikit-llm-0.3.0/skllm/preprocessing/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      183 2023-06-17 15:57:54.000000 scikit-llm-0.3.0/skllm/preprocessing/__init__.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     2237 2023-06-17 15:57:54.000000 scikit-llm-0.3.0/skllm/preprocessing/gpt_summarizer.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     1400 2023-07-04 20:07:18.000000 scikit-llm-0.3.0/skllm/preprocessing/gpt_translator.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     3044 2023-06-17 15:57:54.000000 scikit-llm-0.3.0/skllm/preprocessing/gpt_vectorizer.py
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-04 20:13:20.026403 scikit-llm-0.3.0/skllm/prompts/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     4130 2023-06-17 15:57:54.000000 scikit-llm-0.3.0/skllm/prompts/builders.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     4310 2023-07-04 20:07:18.000000 scikit-llm-0.3.0/skllm/prompts/templates.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     1697 2023-07-04 20:07:18.000000 scikit-llm-0.3.0/skllm/utils.py
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-04 20:13:20.026403 scikit-llm-0.3.0/tests/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     1763 2023-06-17 15:57:54.000000 scikit-llm-0.3.0/tests/test_chatgpt.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     1821 2023-06-17 15:57:54.000000 scikit-llm-0.3.0/tests/test_gpt_few_shot_clf.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     4376 2023-07-04 20:07:18.000000 scikit-llm-0.3.0/tests/test_gpt_zero_shot_clf.py
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-30 11:22:37.318195 scikit-llm-0.3.1/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     1077 2023-06-17 15:57:54.000000 scikit-llm-0.3.1/LICENSE
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)    12363 2023-07-30 11:22:37.318195 scikit-llm-0.3.1/PKG-INFO
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)    11809 2023-07-30 11:20:35.000000 scikit-llm-0.3.1/README.md
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     1983 2023-07-30 11:21:11.000000 scikit-llm-0.3.1/pyproject.toml
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-30 11:22:37.314195 scikit-llm-0.3.1/scikit_llm.egg-info/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)    12363 2023-07-30 11:22:37.000000 scikit-llm-0.3.1/scikit_llm.egg-info/PKG-INFO
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     1231 2023-07-30 11:22:37.000000 scikit-llm-0.3.1/scikit_llm.egg-info/SOURCES.txt
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)        1 2023-07-30 11:22:37.000000 scikit-llm-0.3.1/scikit_llm.egg-info/dependency_links.txt
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      149 2023-07-30 11:22:37.000000 scikit-llm-0.3.1/scikit_llm.egg-info/requires.txt
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)        6 2023-07-30 11:22:37.000000 scikit-llm-0.3.1/scikit_llm.egg-info/top_level.txt
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)       38 2023-07-30 11:22:37.318195 scikit-llm-0.3.1/setup.cfg
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-30 11:22:37.314195 scikit-llm-0.3.1/skllm/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      317 2023-07-30 11:21:07.000000 scikit-llm-0.3.1/skllm/__init__.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      740 2023-07-04 20:07:18.000000 scikit-llm-0.3.1/skllm/completions.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     2960 2023-07-04 20:07:18.000000 scikit-llm-0.3.1/skllm/config.py
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-30 11:22:37.314195 scikit-llm-0.3.1/skllm/datasets/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      273 2023-06-17 15:57:54.000000 scikit-llm-0.3.1/skllm/datasets/__init__.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     5870 2023-06-17 15:57:54.000000 scikit-llm-0.3.1/skllm/datasets/multi_class.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     1438 2023-06-17 15:57:54.000000 scikit-llm-0.3.1/skllm/datasets/multi_label.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     2729 2023-06-17 15:57:54.000000 scikit-llm-0.3.1/skllm/datasets/summarization.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      818 2023-06-17 15:57:54.000000 scikit-llm-0.3.1/skllm/datasets/translation.py
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-30 11:22:37.314195 scikit-llm-0.3.1/skllm/google/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     1403 2023-07-04 20:07:18.000000 scikit-llm-0.3.1/skllm/google/completions.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      507 2023-07-04 20:07:18.000000 scikit-llm-0.3.1/skllm/google/tuning.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     1441 2023-07-30 11:20:35.000000 scikit-llm-0.3.1/skllm/gpt4all_client.py
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-30 11:22:37.314195 scikit-llm-0.3.1/skllm/memory/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)       49 2023-06-17 15:57:54.000000 scikit-llm-0.3.1/skllm/memory/__init__.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     3269 2023-06-17 15:57:54.000000 scikit-llm-0.3.1/skllm/memory/_annoy.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     1027 2023-06-17 15:57:54.000000 scikit-llm-0.3.1/skllm/memory/base.py
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-30 11:22:37.314195 scikit-llm-0.3.1/skllm/models/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     5956 2023-07-04 20:07:18.000000 scikit-llm-0.3.1/skllm/models/_base.py
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-30 11:22:37.314195 scikit-llm-0.3.1/skllm/models/gpt/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      260 2023-07-04 20:07:18.000000 scikit-llm-0.3.1/skllm/models/gpt/__init__.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     4049 2023-07-04 20:07:18.000000 scikit-llm-0.3.1/skllm/models/gpt/gpt_dyn_few_shot_clf.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     1827 2023-07-04 20:07:18.000000 scikit-llm-0.3.1/skllm/models/gpt/gpt_few_shot_clf.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     5829 2023-07-04 20:07:18.000000 scikit-llm-0.3.1/skllm/models/gpt/gpt_zero_shot_clf.py
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-30 11:22:37.314195 scikit-llm-0.3.1/skllm/models/palm/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      122 2023-07-04 20:07:18.000000 scikit-llm-0.3.1/skllm/models/palm/__init__.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     4854 2023-07-04 20:07:18.000000 scikit-llm-0.3.1/skllm/models/palm/palm_clf.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     2313 2023-07-04 20:07:18.000000 scikit-llm-0.3.1/skllm/models/palm/palm_est.py
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-30 11:22:37.314195 scikit-llm-0.3.1/skllm/openai/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     2829 2023-07-04 20:07:18.000000 scikit-llm-0.3.1/skllm/openai/base_gpt.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     2074 2023-07-04 20:07:18.000000 scikit-llm-0.3.1/skllm/openai/chatgpt.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      730 2023-07-04 20:07:18.000000 scikit-llm-0.3.1/skllm/openai/credentials.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     1441 2023-06-17 15:57:54.000000 scikit-llm-0.3.1/skllm/openai/embeddings.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     1200 2023-06-17 21:25:38.000000 scikit-llm-0.3.1/skllm/openai/mixin.py
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-30 11:22:37.314195 scikit-llm-0.3.1/skllm/preprocessing/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      183 2023-06-17 15:57:54.000000 scikit-llm-0.3.1/skllm/preprocessing/__init__.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     2237 2023-06-17 15:57:54.000000 scikit-llm-0.3.1/skllm/preprocessing/gpt_summarizer.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     1400 2023-07-04 20:07:18.000000 scikit-llm-0.3.1/skllm/preprocessing/gpt_translator.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     3044 2023-06-17 15:57:54.000000 scikit-llm-0.3.1/skllm/preprocessing/gpt_vectorizer.py
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-30 11:22:37.314195 scikit-llm-0.3.1/skllm/prompts/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     4130 2023-06-17 15:57:54.000000 scikit-llm-0.3.1/skllm/prompts/builders.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     4310 2023-07-23 17:33:46.000000 scikit-llm-0.3.1/skllm/prompts/templates.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     1697 2023-07-04 20:07:18.000000 scikit-llm-0.3.1/skllm/utils.py
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-30 11:22:37.314195 scikit-llm-0.3.1/tests/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     1763 2023-06-17 15:57:54.000000 scikit-llm-0.3.1/tests/test_chatgpt.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     1821 2023-06-17 15:57:54.000000 scikit-llm-0.3.1/tests/test_gpt_few_shot_clf.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     4376 2023-07-04 20:07:18.000000 scikit-llm-0.3.1/tests/test_gpt_zero_shot_clf.py
```

### Comparing `scikit-llm-0.3.0/LICENSE` & `scikit-llm-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.3.0/PKG-INFO` & `scikit-llm-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-llm
-Version: 0.3.0
+Version: 0.3.1
 Summary: Scikit-LLM: Seamlessly integrate powerful language models like ChatGPT into scikit-learn for enhanced text analysis tasks.
 Author-email: Oleg Kostromin <kostromin97@gmail.com>, Iryna Kondrashchenko <iryna230520@gmail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -32,16 +32,16 @@
 
 - ⭐ Star Scikit-LLM on GitHub (click the star button in the top right corner)
 - 💡 Provide your feedback or propose ideas in the [issues](https://github.com/iryna-kondr/scikit-llm/issues) section or [Discord](https://discord.gg/YDAbwuWK7V)
 - 📰 Post about Scikit-LLM on LinkedIn or other platforms
 
 ## Our Related Projects 🔗
 
-<a href="https://github.com/OKUA1/falcon"><img src="https://raw.githubusercontent.com/gist/OKUA1/6264a95a8abd225c74411a2b707b0242/raw/3cedb53538cb04656cd9d7d07e697e726896ce9f/falcon_light.svg"/></a> <br>
-<a href="https://github.com/OKUA1/agent_dingo"><img src="https://gist.githubusercontent.com/OKUA1/6264a95a8abd225c74411a2b707b0242/raw/1b231aab718fcab624faa33d9c10d0eee17ca160/dingo_light.svg"/></a>
+<a href="https://github.com/OKUA1/agent_dingo"><img src="https://gist.githubusercontent.com/OKUA1/6264a95a8abd225c74411a2b707b0242/raw/1b231aab718fcab624faa33d9c10d0eee17ca160/dingo_light.svg"/></a> <br>
+<a href="https://github.com/OKUA1/falcon"><img src="https://raw.githubusercontent.com/gist/OKUA1/6264a95a8abd225c74411a2b707b0242/raw/3cedb53538cb04656cd9d7d07e697e726896ce9f/falcon_light.svg"/></a>
 
 ## Documentation 📚
 
 ### Configuring OpenAI API Key
 
 At the moment the majority of the Scikit-LLM estimators are only compatible with some of the OpenAI models. Hence, a user-provided OpenAI API key is required.
 
@@ -58,15 +58,15 @@
 - When calling `SKLLMConfig.set_openai_org`, you have to provide your organization ID and **NOT** the name. You can find your ID [here](https://platform.openai.com/account/org-settings).
 
 ### Using Azure OpenAI
 
 ```python
 from skllm.config import SKLLMConfig
 
-SKLLMConfig.set_openai_key("<YOUR_KEY>") #use azure key instead
+SKLLMConfig.set_openai_key("<YOUR_KEY>")  # use azure key instead
 SKLLMConfig.set_azure_api_base("<API_BASE>")
 
 # start with "azure::" prefix when setting the model name
 model_name = "azure::<model_name>"
 # e.g. ZeroShotGPTClassifier(openai_model="azure::gpt-3.5-turbo")
 ```
 
@@ -86,15 +86,15 @@
 
 In order to switch from OpenAI to GPT4ALL model, simply provide a string of the format `gpt4all::<model_name>` as an argument. While the model runs completely locally, the estimator still treats it as an OpenAI endpoint and will try to check that the API key is present. You can provide any string as a key.
 
 ```python
 SKLLMConfig.set_openai_key("any string")
 SKLLMConfig.set_openai_org("any string")
 
-ZeroShotGPTClassifier(openai_model="gpt4all::ggml-gpt4all-j-v1.3-groovy")
+ZeroShotGPTClassifier(openai_model="gpt4all::ggml-model-gpt4all-falcon-q4_0.bin")
 ```
 
 When running for the first time, the model file will be downloaded automatially.
 
 When using gpt4all please keep the following in mind:
 
 1. Not all gpt4all models are commercially licensable, please consult gpt4all website for more details.
@@ -235,32 +235,33 @@
 clf.fit(X, y)
 labels = clf.predict(X)
 ```
 
 ### Text Classification with Google PaLM 2
 
 At the moment 3 PaLM based models are available in test mode:
+
 - `ZeroShotPaLMClassifier` - zero-shot text classification with PaLM 2;
 - `PaLMClassifier` - fine-tunable text classifier with PaLM 2;
 - `PaLM` - fine-tunable estimator that can be trained on arbitrary text input-output pairs.
 
-Example: 
+Example:
 
 ```python
 from skllm.models.palm import PaLMClassifier
 from skllm.datasets import get_classification_dataset
 
 X, y = get_classification_dataset()
 
 clf = PaLMClassifier(n_update_steps=100)
 clf.fit(X, y)
 labels = clf.predict(X)
 ```
 
-A more detailed documentation will follow soon. For now, please refer to our [official guide on Medium](https://medium.com/@iryna230520).
+A more detailed documentation will follow soon. For now, please refer to our [official guide on Medium](https://medium.com/@iryna230520/fine-tune-google-palm-2-with-scikit-llm-d41b0aa673a5).
 
 ### Text Vectorization
 
 As an alternative to using GPT as a classifier, it can be used solely for data preprocessing. `GPTVectorizer` allows to embed a chunk of text of arbitrary length to a fixed-dimensional vector, that can be used with virtually any classification or regression model.
 
 Example 1: Embedding the text
 
@@ -321,8 +322,7 @@
 from skllm.preprocessing import GPTTranslator
 from skllm.datasets import get_translation_dataset
 
 X = get_translation_dataset()
 t = GPTTranslator(openai_model="gpt-3.5-turbo", output_language="English")
 translated_text = t.fit_transform(X)
 ```
-
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: scikit-llm Version: 0.3.0 Summary: Scikit-LLM:
+Metadata-Version: 2.1 Name: scikit-llm Version: 0.3.1 Summary: Scikit-LLM:
 Seamlessly integrate powerful language models like ChatGPT into scikit-learn
 for enhanced text analysis tasks. Author-email: Oleg Kostromin
 gmail.com>, Iryna Kondrashchenko
 gmail.com> License: MIT Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.8 Description-Content-Type: text/
 markdown Provides-Extra: gpt4all License-File: LICENSE
@@ -11,71 +11,71 @@
 language models like ChatGPT into scikit-learn for enhanced text analysis
 tasks. ## Installation ð¾ ```bash pip install scikit-llm ``` ## Support us
 ð¤ You can support the project in the following ways: - â­ Star Scikit-LLM
 on GitHub (click the star button in the top right corner) - ð¡ Provide your
 feedback or propose ideas in the [issues](https://github.com/iryna-kondr/
 scikit-llm/issues) section or [Discord](https://discord.gg/YDAbwuWK7V) - ð°
 Post about Scikit-LLM on LinkedIn or other platforms ## Our Related Projects
-ð [https://raw.githubusercontent.com/gist/OKUA1/
-6264a95a8abd225c74411a2b707b0242/raw/3cedb53538cb04656cd9d7d07e697e726896ce9f/
-falcon_light.svg]
-[https://gist.githubusercontent.com/OKUA1/6264a95a8abd225c74411a2b707b0242/raw/
-1b231aab718fcab624faa33d9c10d0eee17ca160/dingo_light.svg] ## Documentation ð
-### Configuring OpenAI API Key At the moment the majority of the Scikit-LLM
-estimators are only compatible with some of the OpenAI models. Hence, a user-
-provided OpenAI API key is required. ```python from skllm.config import
+ð [https://gist.githubusercontent.com/OKUA1/
+6264a95a8abd225c74411a2b707b0242/raw/1b231aab718fcab624faa33d9c10d0eee17ca160/
+dingo_light.svg]
+[https://raw.githubusercontent.com/gist/OKUA1/6264a95a8abd225c74411a2b707b0242/
+raw/3cedb53538cb04656cd9d7d07e697e726896ce9f/falcon_light.svg] ## Documentation
+ð ### Configuring OpenAI API Key At the moment the majority of the Scikit-
+LLM estimators are only compatible with some of the OpenAI models. Hence, a
+user-provided OpenAI API key is required. ```python from skllm.config import
 SKLLMConfig SKLLMConfig.set_openai_key("") SKLLMConfig.set_openai_org("") ```
 **Important notice:** - If you have a free trial OpenAI account, the [rate
 limits](https://platform.openai.com/docs/guides/rate-limits/overview) are not
 sufficient (specifically 3 requests per minute). Please switch to the "pay as
 you go" plan first. - When calling `SKLLMConfig.set_openai_org`, you have to
 provide your organization ID and **NOT** the name. You can find your ID [here]
 (https://platform.openai.com/account/org-settings). ### Using Azure OpenAI
-```python from skllm.config import SKLLMConfig SKLLMConfig.set_openai_key("")
-#use azure key instead SKLLMConfig.set_azure_api_base("") # start with "azure::
+```python from skllm.config import SKLLMConfig SKLLMConfig.set_openai_key("") #
+use azure key instead SKLLMConfig.set_azure_api_base("") # start with "azure::
 " prefix when setting the model name model_name = "azure::" # e.g.
 ZeroShotGPTClassifier(openai_model="azure::gpt-3.5-turbo") ``` Note: Azure
 OpenAI is not supported by the preprocessors at the moment. ### Using GPT4ALL
 In addition to OpenAI, some of the models can use [gpt4all](https://gpt4all.io/
 index.html) as a backend. **This feature is considered higly experimental!** In
 order to use gpt4all, you need to install the corresponding submodule: ```bash
 pip install "scikit-llm[gpt4all]" ``` In order to switch from OpenAI to GPT4ALL
 model, simply provide a string of the format `gpt4all::` as an argument. While
 the model runs completely locally, the estimator still treats it as an OpenAI
 endpoint and will try to check that the API key is present. You can provide any
 string as a key. ```python SKLLMConfig.set_openai_key("any string")
 SKLLMConfig.set_openai_org("any string") ZeroShotGPTClassifier
-(openai_model="gpt4all::ggml-gpt4all-j-v1.3-groovy") ``` When running for the
-first time, the model file will be downloaded automatially. When using gpt4all
-please keep the following in mind: 1. Not all gpt4all models are commercially
-licensable, please consult gpt4all website for more details. 2. The accuracy of
-the models may be much lower compared to ones provided by OpenAI (especially
-gpt-4). 3. Not all of the available models were tested, some may not work with
-scikit-llm at all. ### Supported models by a non-standard backend At the moment
-only the following estimators support non-standard backends (gpt4all, azure): -
-`ZeroShotGPTClassifier` - `MultiLabelZeroShotGPTClassifier` -
-`FewShotGPTClassifier` ### Zero-Shot Text Classification One of the powerful
-ChatGPT features is the ability to perform text classification without being
-re-trained. For that, the only requirement is that the labels must be
-descriptive. We provide a class `ZeroShotGPTClassifier` that allows to create
-such a model as a regular scikit-learn classifier. Example 1: Training as a
-regular classifier ```python from skllm import ZeroShotGPTClassifier from
-skllm.datasets import get_classification_dataset # demo sentiment analysis
-dataset # labels: positive, negative, neutral X, y = get_classification_dataset
-() clf = ZeroShotGPTClassifier(openai_model="gpt-3.5-turbo") clf.fit(X, y)
-labels = clf.predict(X) ``` Scikit-LLM will automatically query the OpenAI API
-and transform the response into a regular list of labels. Additionally, Scikit-
-LLM will ensure that the obtained response contains a valid label. If this is
-not the case, a label will be selected randomly (label probabilities are
-proportional to label occurrences in the training set). Example 2: Training
-without labeled data Since the training data is not strictly required, it can
-be fully ommited. The only thing that has to be provided is the list of
-candidate labels. ```python from skllm import ZeroShotGPTClassifier from
-skllm.datasets import get_classification_dataset X, _ =
-get_classification_dataset() clf = ZeroShotGPTClassifier() clf.fit(None,
+(openai_model="gpt4all::ggml-model-gpt4all-falcon-q4_0.bin") ``` When running
+for the first time, the model file will be downloaded automatially. When using
+gpt4all please keep the following in mind: 1. Not all gpt4all models are
+commercially licensable, please consult gpt4all website for more details. 2.
+The accuracy of the models may be much lower compared to ones provided by
+OpenAI (especially gpt-4). 3. Not all of the available models were tested, some
+may not work with scikit-llm at all. ### Supported models by a non-standard
+backend At the moment only the following estimators support non-standard
+backends (gpt4all, azure): - `ZeroShotGPTClassifier` -
+`MultiLabelZeroShotGPTClassifier` - `FewShotGPTClassifier` ### Zero-Shot Text
+Classification One of the powerful ChatGPT features is the ability to perform
+text classification without being re-trained. For that, the only requirement is
+that the labels must be descriptive. We provide a class `ZeroShotGPTClassifier`
+that allows to create such a model as a regular scikit-learn classifier.
+Example 1: Training as a regular classifier ```python from skllm import
+ZeroShotGPTClassifier from skllm.datasets import get_classification_dataset #
+demo sentiment analysis dataset # labels: positive, negative, neutral X, y =
+get_classification_dataset() clf = ZeroShotGPTClassifier(openai_model="gpt-3.5-
+turbo") clf.fit(X, y) labels = clf.predict(X) ``` Scikit-LLM will automatically
+query the OpenAI API and transform the response into a regular list of labels.
+Additionally, Scikit-LLM will ensure that the obtained response contains a
+valid label. If this is not the case, a label will be selected randomly (label
+probabilities are proportional to label occurrences in the training set).
+Example 2: Training without labeled data Since the training data is not
+strictly required, it can be fully ommited. The only thing that has to be
+provided is the list of candidate labels. ```python from skllm import
+ZeroShotGPTClassifier from skllm.datasets import get_classification_dataset X,
+_ = get_classification_dataset() clf = ZeroShotGPTClassifier() clf.fit(None,
 ["positive", "negative", "neutral"]) labels = clf.predict(X) ``` **Note:**
 unlike in a typical supervised setting, the performance of a zero-shot
 classifier greatly depends on how the label itself is structured. It has to be
 expressed in natural language, be descriptive and self-explanatory. For
 example, in the previous semantic classification task, it could be beneficial
 to transform a label from `""` to `"the semantics of the provided text is "`.
 ### Multi-Label Zero-Shot Text Classification With a class
@@ -123,39 +123,39 @@
 `PaLMClassifier` - fine-tunable text classifier with PaLM 2; - `PaLM` - fine-
 tunable estimator that can be trained on arbitrary text input-output pairs.
 Example: ```python from skllm.models.palm import PaLMClassifier from
 skllm.datasets import get_classification_dataset X, y =
 get_classification_dataset() clf = PaLMClassifier(n_update_steps=100) clf.fit
 (X, y) labels = clf.predict(X) ``` A more detailed documentation will follow
 soon. For now, please refer to our [official guide on Medium](https://
-medium.com/@iryna230520). ### Text Vectorization As an alternative to using GPT
-as a classifier, it can be used solely for data preprocessing. `GPTVectorizer`
-allows to embed a chunk of text of arbitrary length to a fixed-dimensional
-vector, that can be used with virtually any classification or regression model.
-Example 1: Embedding the text ```python from skllm.preprocessing import
-GPTVectorizer model = GPTVectorizer() vectors = model.fit_transform(X) ```
-Example 2: Combining the Vectorizer with the XGBoost Classifier in a Sklearn
-Pipeline ```python from sklearn.pipeline import Pipeline from
-sklearn.preprocessing import LabelEncoder from xgboost import XGBClassifier le
-= LabelEncoder() y_train_encoded = le.fit_transform(y_train) y_test_encoded =
-le.transform(y_test) steps = [("GPT", GPTVectorizer()), ("Clf", XGBClassifier
-())] clf = Pipeline(steps) clf.fit(X_train, y_train_encoded) yh = clf.predict
-(X_test) ``` ### Text Summarization GPT excels at performing summarization
-tasks. Therefore, we provide `GPTSummarizer` that can be used both as stand-
-alone estimator, or as a preprocessor (in this case we can make an analogy with
-a dimensionality reduction preprocessor). Example: ```python from
-skllm.preprocessing import GPTSummarizer from skllm.datasets import
-get_summarization_dataset X = get_summarization_dataset() s = GPTSummarizer
-(openai_model="gpt-3.5-turbo", max_words=15) summaries = s.fit_transform(X) ```
-Please be aware that the `max_words` hyperparameter sets a soft limit, which is
-not strictly enforced outside of the prompt. Therefore, in some cases, the
-actual number of words might be slightly higher. It is possible to generate a
-summary, emphasizing a specific concept, by providing an optional parameter
-`focus`: ```python s = GPTSummarizer(openai_model="gpt-3.5-turbo",
-max_words=15, focus="apples") ``` ### Text Translation GPT models have
-demonstrated their effectiveness in translation tasks by generating accurate
-translations across various languages. Thus, we added `GPTTranslator` that
-allows translating an arbitraty text into a language of interest. Example:
-```python from skllm.preprocessing import GPTTranslator from skllm.datasets
-import get_translation_dataset X = get_translation_dataset() t = GPTTranslator
-(openai_model="gpt-3.5-turbo", output_language="English") translated_text =
-t.fit_transform(X) ```
+medium.com/@iryna230520/fine-tune-google-palm-2-with-scikit-llm-d41b0aa673a5).
+### Text Vectorization As an alternative to using GPT as a classifier, it can
+be used solely for data preprocessing. `GPTVectorizer` allows to embed a chunk
+of text of arbitrary length to a fixed-dimensional vector, that can be used
+with virtually any classification or regression model. Example 1: Embedding the
+text ```python from skllm.preprocessing import GPTVectorizer model =
+GPTVectorizer() vectors = model.fit_transform(X) ``` Example 2: Combining the
+Vectorizer with the XGBoost Classifier in a Sklearn Pipeline ```python from
+sklearn.pipeline import Pipeline from sklearn.preprocessing import LabelEncoder
+from xgboost import XGBClassifier le = LabelEncoder() y_train_encoded =
+le.fit_transform(y_train) y_test_encoded = le.transform(y_test) steps = [
+("GPT", GPTVectorizer()), ("Clf", XGBClassifier())] clf = Pipeline(steps)
+clf.fit(X_train, y_train_encoded) yh = clf.predict(X_test) ``` ### Text
+Summarization GPT excels at performing summarization tasks. Therefore, we
+provide `GPTSummarizer` that can be used both as stand-alone estimator, or as a
+preprocessor (in this case we can make an analogy with a dimensionality
+reduction preprocessor). Example: ```python from skllm.preprocessing import
+GPTSummarizer from skllm.datasets import get_summarization_dataset X =
+get_summarization_dataset() s = GPTSummarizer(openai_model="gpt-3.5-turbo",
+max_words=15) summaries = s.fit_transform(X) ``` Please be aware that the
+`max_words` hyperparameter sets a soft limit, which is not strictly enforced
+outside of the prompt. Therefore, in some cases, the actual number of words
+might be slightly higher. It is possible to generate a summary, emphasizing a
+specific concept, by providing an optional parameter `focus`: ```python s =
+GPTSummarizer(openai_model="gpt-3.5-turbo", max_words=15, focus="apples") ```
+### Text Translation GPT models have demonstrated their effectiveness in
+translation tasks by generating accurate translations across various languages.
+Thus, we added `GPTTranslator` that allows translating an arbitraty text into a
+language of interest. Example: ```python from skllm.preprocessing import
+GPTTranslator from skllm.datasets import get_translation_dataset X =
+get_translation_dataset() t = GPTTranslator(openai_model="gpt-3.5-turbo",
+output_language="English") translated_text = t.fit_transform(X) ```
```

### Comparing `scikit-llm-0.3.0/README.md` & `scikit-llm-0.3.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 
 - ⭐ Star Scikit-LLM on GitHub (click the star button in the top right corner)
 - 💡 Provide your feedback or propose ideas in the [issues](https://github.com/iryna-kondr/scikit-llm/issues) section or [Discord](https://discord.gg/YDAbwuWK7V)
 - 📰 Post about Scikit-LLM on LinkedIn or other platforms
 
 ## Our Related Projects 🔗
 
-<a href="https://github.com/OKUA1/falcon"><img src="https://raw.githubusercontent.com/gist/OKUA1/6264a95a8abd225c74411a2b707b0242/raw/3cedb53538cb04656cd9d7d07e697e726896ce9f/falcon_light.svg"/></a> <br>
-<a href="https://github.com/OKUA1/agent_dingo"><img src="https://gist.githubusercontent.com/OKUA1/6264a95a8abd225c74411a2b707b0242/raw/1b231aab718fcab624faa33d9c10d0eee17ca160/dingo_light.svg"/></a>
+<a href="https://github.com/OKUA1/agent_dingo"><img src="https://gist.githubusercontent.com/OKUA1/6264a95a8abd225c74411a2b707b0242/raw/1b231aab718fcab624faa33d9c10d0eee17ca160/dingo_light.svg"/></a> <br>
+<a href="https://github.com/OKUA1/falcon"><img src="https://raw.githubusercontent.com/gist/OKUA1/6264a95a8abd225c74411a2b707b0242/raw/3cedb53538cb04656cd9d7d07e697e726896ce9f/falcon_light.svg"/></a>
 
 ## Documentation 📚
 
 ### Configuring OpenAI API Key
 
 At the moment the majority of the Scikit-LLM estimators are only compatible with some of the OpenAI models. Hence, a user-provided OpenAI API key is required.
 
@@ -44,15 +44,15 @@
 - When calling `SKLLMConfig.set_openai_org`, you have to provide your organization ID and **NOT** the name. You can find your ID [here](https://platform.openai.com/account/org-settings).
 
 ### Using Azure OpenAI
 
 ```python
 from skllm.config import SKLLMConfig
 
-SKLLMConfig.set_openai_key("<YOUR_KEY>") #use azure key instead
+SKLLMConfig.set_openai_key("<YOUR_KEY>")  # use azure key instead
 SKLLMConfig.set_azure_api_base("<API_BASE>")
 
 # start with "azure::" prefix when setting the model name
 model_name = "azure::<model_name>"
 # e.g. ZeroShotGPTClassifier(openai_model="azure::gpt-3.5-turbo")
 ```
 
@@ -72,15 +72,15 @@
 
 In order to switch from OpenAI to GPT4ALL model, simply provide a string of the format `gpt4all::<model_name>` as an argument. While the model runs completely locally, the estimator still treats it as an OpenAI endpoint and will try to check that the API key is present. You can provide any string as a key.
 
 ```python
 SKLLMConfig.set_openai_key("any string")
 SKLLMConfig.set_openai_org("any string")
 
-ZeroShotGPTClassifier(openai_model="gpt4all::ggml-gpt4all-j-v1.3-groovy")
+ZeroShotGPTClassifier(openai_model="gpt4all::ggml-model-gpt4all-falcon-q4_0.bin")
 ```
 
 When running for the first time, the model file will be downloaded automatially.
 
 When using gpt4all please keep the following in mind:
 
 1. Not all gpt4all models are commercially licensable, please consult gpt4all website for more details.
@@ -221,32 +221,33 @@
 clf.fit(X, y)
 labels = clf.predict(X)
 ```
 
 ### Text Classification with Google PaLM 2
 
 At the moment 3 PaLM based models are available in test mode:
+
 - `ZeroShotPaLMClassifier` - zero-shot text classification with PaLM 2;
 - `PaLMClassifier` - fine-tunable text classifier with PaLM 2;
 - `PaLM` - fine-tunable estimator that can be trained on arbitrary text input-output pairs.
 
-Example: 
+Example:
 
 ```python
 from skllm.models.palm import PaLMClassifier
 from skllm.datasets import get_classification_dataset
 
 X, y = get_classification_dataset()
 
 clf = PaLMClassifier(n_update_steps=100)
 clf.fit(X, y)
 labels = clf.predict(X)
 ```
 
-A more detailed documentation will follow soon. For now, please refer to our [official guide on Medium](https://medium.com/@iryna230520).
+A more detailed documentation will follow soon. For now, please refer to our [official guide on Medium](https://medium.com/@iryna230520/fine-tune-google-palm-2-with-scikit-llm-d41b0aa673a5).
 
 ### Text Vectorization
 
 As an alternative to using GPT as a classifier, it can be used solely for data preprocessing. `GPTVectorizer` allows to embed a chunk of text of arbitrary length to a fixed-dimensional vector, that can be used with virtually any classification or regression model.
 
 Example 1: Embedding the text
 
@@ -307,8 +308,7 @@
 from skllm.preprocessing import GPTTranslator
 from skllm.datasets import get_translation_dataset
 
 X = get_translation_dataset()
 t = GPTTranslator(openai_model="gpt-3.5-turbo", output_language="English")
 translated_text = t.fit_transform(X)
 ```
-
```

#### html2text {}

```diff
@@ -3,71 +3,71 @@
 language models like ChatGPT into scikit-learn for enhanced text analysis
 tasks. ## Installation ð¾ ```bash pip install scikit-llm ``` ## Support us
 ð¤ You can support the project in the following ways: - â­ Star Scikit-LLM
 on GitHub (click the star button in the top right corner) - ð¡ Provide your
 feedback or propose ideas in the [issues](https://github.com/iryna-kondr/
 scikit-llm/issues) section or [Discord](https://discord.gg/YDAbwuWK7V) - ð°
 Post about Scikit-LLM on LinkedIn or other platforms ## Our Related Projects
-ð [https://raw.githubusercontent.com/gist/OKUA1/
-6264a95a8abd225c74411a2b707b0242/raw/3cedb53538cb04656cd9d7d07e697e726896ce9f/
-falcon_light.svg]
-[https://gist.githubusercontent.com/OKUA1/6264a95a8abd225c74411a2b707b0242/raw/
-1b231aab718fcab624faa33d9c10d0eee17ca160/dingo_light.svg] ## Documentation ð
-### Configuring OpenAI API Key At the moment the majority of the Scikit-LLM
-estimators are only compatible with some of the OpenAI models. Hence, a user-
-provided OpenAI API key is required. ```python from skllm.config import
+ð [https://gist.githubusercontent.com/OKUA1/
+6264a95a8abd225c74411a2b707b0242/raw/1b231aab718fcab624faa33d9c10d0eee17ca160/
+dingo_light.svg]
+[https://raw.githubusercontent.com/gist/OKUA1/6264a95a8abd225c74411a2b707b0242/
+raw/3cedb53538cb04656cd9d7d07e697e726896ce9f/falcon_light.svg] ## Documentation
+ð ### Configuring OpenAI API Key At the moment the majority of the Scikit-
+LLM estimators are only compatible with some of the OpenAI models. Hence, a
+user-provided OpenAI API key is required. ```python from skllm.config import
 SKLLMConfig SKLLMConfig.set_openai_key("") SKLLMConfig.set_openai_org("") ```
 **Important notice:** - If you have a free trial OpenAI account, the [rate
 limits](https://platform.openai.com/docs/guides/rate-limits/overview) are not
 sufficient (specifically 3 requests per minute). Please switch to the "pay as
 you go" plan first. - When calling `SKLLMConfig.set_openai_org`, you have to
 provide your organization ID and **NOT** the name. You can find your ID [here]
 (https://platform.openai.com/account/org-settings). ### Using Azure OpenAI
-```python from skllm.config import SKLLMConfig SKLLMConfig.set_openai_key("")
-#use azure key instead SKLLMConfig.set_azure_api_base("") # start with "azure::
+```python from skllm.config import SKLLMConfig SKLLMConfig.set_openai_key("") #
+use azure key instead SKLLMConfig.set_azure_api_base("") # start with "azure::
 " prefix when setting the model name model_name = "azure::" # e.g.
 ZeroShotGPTClassifier(openai_model="azure::gpt-3.5-turbo") ``` Note: Azure
 OpenAI is not supported by the preprocessors at the moment. ### Using GPT4ALL
 In addition to OpenAI, some of the models can use [gpt4all](https://gpt4all.io/
 index.html) as a backend. **This feature is considered higly experimental!** In
 order to use gpt4all, you need to install the corresponding submodule: ```bash
 pip install "scikit-llm[gpt4all]" ``` In order to switch from OpenAI to GPT4ALL
 model, simply provide a string of the format `gpt4all::` as an argument. While
 the model runs completely locally, the estimator still treats it as an OpenAI
 endpoint and will try to check that the API key is present. You can provide any
 string as a key. ```python SKLLMConfig.set_openai_key("any string")
 SKLLMConfig.set_openai_org("any string") ZeroShotGPTClassifier
-(openai_model="gpt4all::ggml-gpt4all-j-v1.3-groovy") ``` When running for the
-first time, the model file will be downloaded automatially. When using gpt4all
-please keep the following in mind: 1. Not all gpt4all models are commercially
-licensable, please consult gpt4all website for more details. 2. The accuracy of
-the models may be much lower compared to ones provided by OpenAI (especially
-gpt-4). 3. Not all of the available models were tested, some may not work with
-scikit-llm at all. ### Supported models by a non-standard backend At the moment
-only the following estimators support non-standard backends (gpt4all, azure): -
-`ZeroShotGPTClassifier` - `MultiLabelZeroShotGPTClassifier` -
-`FewShotGPTClassifier` ### Zero-Shot Text Classification One of the powerful
-ChatGPT features is the ability to perform text classification without being
-re-trained. For that, the only requirement is that the labels must be
-descriptive. We provide a class `ZeroShotGPTClassifier` that allows to create
-such a model as a regular scikit-learn classifier. Example 1: Training as a
-regular classifier ```python from skllm import ZeroShotGPTClassifier from
-skllm.datasets import get_classification_dataset # demo sentiment analysis
-dataset # labels: positive, negative, neutral X, y = get_classification_dataset
-() clf = ZeroShotGPTClassifier(openai_model="gpt-3.5-turbo") clf.fit(X, y)
-labels = clf.predict(X) ``` Scikit-LLM will automatically query the OpenAI API
-and transform the response into a regular list of labels. Additionally, Scikit-
-LLM will ensure that the obtained response contains a valid label. If this is
-not the case, a label will be selected randomly (label probabilities are
-proportional to label occurrences in the training set). Example 2: Training
-without labeled data Since the training data is not strictly required, it can
-be fully ommited. The only thing that has to be provided is the list of
-candidate labels. ```python from skllm import ZeroShotGPTClassifier from
-skllm.datasets import get_classification_dataset X, _ =
-get_classification_dataset() clf = ZeroShotGPTClassifier() clf.fit(None,
+(openai_model="gpt4all::ggml-model-gpt4all-falcon-q4_0.bin") ``` When running
+for the first time, the model file will be downloaded automatially. When using
+gpt4all please keep the following in mind: 1. Not all gpt4all models are
+commercially licensable, please consult gpt4all website for more details. 2.
+The accuracy of the models may be much lower compared to ones provided by
+OpenAI (especially gpt-4). 3. Not all of the available models were tested, some
+may not work with scikit-llm at all. ### Supported models by a non-standard
+backend At the moment only the following estimators support non-standard
+backends (gpt4all, azure): - `ZeroShotGPTClassifier` -
+`MultiLabelZeroShotGPTClassifier` - `FewShotGPTClassifier` ### Zero-Shot Text
+Classification One of the powerful ChatGPT features is the ability to perform
+text classification without being re-trained. For that, the only requirement is
+that the labels must be descriptive. We provide a class `ZeroShotGPTClassifier`
+that allows to create such a model as a regular scikit-learn classifier.
+Example 1: Training as a regular classifier ```python from skllm import
+ZeroShotGPTClassifier from skllm.datasets import get_classification_dataset #
+demo sentiment analysis dataset # labels: positive, negative, neutral X, y =
+get_classification_dataset() clf = ZeroShotGPTClassifier(openai_model="gpt-3.5-
+turbo") clf.fit(X, y) labels = clf.predict(X) ``` Scikit-LLM will automatically
+query the OpenAI API and transform the response into a regular list of labels.
+Additionally, Scikit-LLM will ensure that the obtained response contains a
+valid label. If this is not the case, a label will be selected randomly (label
+probabilities are proportional to label occurrences in the training set).
+Example 2: Training without labeled data Since the training data is not
+strictly required, it can be fully ommited. The only thing that has to be
+provided is the list of candidate labels. ```python from skllm import
+ZeroShotGPTClassifier from skllm.datasets import get_classification_dataset X,
+_ = get_classification_dataset() clf = ZeroShotGPTClassifier() clf.fit(None,
 ["positive", "negative", "neutral"]) labels = clf.predict(X) ``` **Note:**
 unlike in a typical supervised setting, the performance of a zero-shot
 classifier greatly depends on how the label itself is structured. It has to be
 expressed in natural language, be descriptive and self-explanatory. For
 example, in the previous semantic classification task, it could be beneficial
 to transform a label from `""` to `"the semantics of the provided text is "`.
 ### Multi-Label Zero-Shot Text Classification With a class
@@ -115,39 +115,39 @@
 `PaLMClassifier` - fine-tunable text classifier with PaLM 2; - `PaLM` - fine-
 tunable estimator that can be trained on arbitrary text input-output pairs.
 Example: ```python from skllm.models.palm import PaLMClassifier from
 skllm.datasets import get_classification_dataset X, y =
 get_classification_dataset() clf = PaLMClassifier(n_update_steps=100) clf.fit
 (X, y) labels = clf.predict(X) ``` A more detailed documentation will follow
 soon. For now, please refer to our [official guide on Medium](https://
-medium.com/@iryna230520). ### Text Vectorization As an alternative to using GPT
-as a classifier, it can be used solely for data preprocessing. `GPTVectorizer`
-allows to embed a chunk of text of arbitrary length to a fixed-dimensional
-vector, that can be used with virtually any classification or regression model.
-Example 1: Embedding the text ```python from skllm.preprocessing import
-GPTVectorizer model = GPTVectorizer() vectors = model.fit_transform(X) ```
-Example 2: Combining the Vectorizer with the XGBoost Classifier in a Sklearn
-Pipeline ```python from sklearn.pipeline import Pipeline from
-sklearn.preprocessing import LabelEncoder from xgboost import XGBClassifier le
-= LabelEncoder() y_train_encoded = le.fit_transform(y_train) y_test_encoded =
-le.transform(y_test) steps = [("GPT", GPTVectorizer()), ("Clf", XGBClassifier
-())] clf = Pipeline(steps) clf.fit(X_train, y_train_encoded) yh = clf.predict
-(X_test) ``` ### Text Summarization GPT excels at performing summarization
-tasks. Therefore, we provide `GPTSummarizer` that can be used both as stand-
-alone estimator, or as a preprocessor (in this case we can make an analogy with
-a dimensionality reduction preprocessor). Example: ```python from
-skllm.preprocessing import GPTSummarizer from skllm.datasets import
-get_summarization_dataset X = get_summarization_dataset() s = GPTSummarizer
-(openai_model="gpt-3.5-turbo", max_words=15) summaries = s.fit_transform(X) ```
-Please be aware that the `max_words` hyperparameter sets a soft limit, which is
-not strictly enforced outside of the prompt. Therefore, in some cases, the
-actual number of words might be slightly higher. It is possible to generate a
-summary, emphasizing a specific concept, by providing an optional parameter
-`focus`: ```python s = GPTSummarizer(openai_model="gpt-3.5-turbo",
-max_words=15, focus="apples") ``` ### Text Translation GPT models have
-demonstrated their effectiveness in translation tasks by generating accurate
-translations across various languages. Thus, we added `GPTTranslator` that
-allows translating an arbitraty text into a language of interest. Example:
-```python from skllm.preprocessing import GPTTranslator from skllm.datasets
-import get_translation_dataset X = get_translation_dataset() t = GPTTranslator
-(openai_model="gpt-3.5-turbo", output_language="English") translated_text =
-t.fit_transform(X) ```
+medium.com/@iryna230520/fine-tune-google-palm-2-with-scikit-llm-d41b0aa673a5).
+### Text Vectorization As an alternative to using GPT as a classifier, it can
+be used solely for data preprocessing. `GPTVectorizer` allows to embed a chunk
+of text of arbitrary length to a fixed-dimensional vector, that can be used
+with virtually any classification or regression model. Example 1: Embedding the
+text ```python from skllm.preprocessing import GPTVectorizer model =
+GPTVectorizer() vectors = model.fit_transform(X) ``` Example 2: Combining the
+Vectorizer with the XGBoost Classifier in a Sklearn Pipeline ```python from
+sklearn.pipeline import Pipeline from sklearn.preprocessing import LabelEncoder
+from xgboost import XGBClassifier le = LabelEncoder() y_train_encoded =
+le.fit_transform(y_train) y_test_encoded = le.transform(y_test) steps = [
+("GPT", GPTVectorizer()), ("Clf", XGBClassifier())] clf = Pipeline(steps)
+clf.fit(X_train, y_train_encoded) yh = clf.predict(X_test) ``` ### Text
+Summarization GPT excels at performing summarization tasks. Therefore, we
+provide `GPTSummarizer` that can be used both as stand-alone estimator, or as a
+preprocessor (in this case we can make an analogy with a dimensionality
+reduction preprocessor). Example: ```python from skllm.preprocessing import
+GPTSummarizer from skllm.datasets import get_summarization_dataset X =
+get_summarization_dataset() s = GPTSummarizer(openai_model="gpt-3.5-turbo",
+max_words=15) summaries = s.fit_transform(X) ``` Please be aware that the
+`max_words` hyperparameter sets a soft limit, which is not strictly enforced
+outside of the prompt. Therefore, in some cases, the actual number of words
+might be slightly higher. It is possible to generate a summary, emphasizing a
+specific concept, by providing an optional parameter `focus`: ```python s =
+GPTSummarizer(openai_model="gpt-3.5-turbo", max_words=15, focus="apples") ```
+### Text Translation GPT models have demonstrated their effectiveness in
+translation tasks by generating accurate translations across various languages.
+Thus, we added `GPTTranslator` that allows translating an arbitraty text into a
+language of interest. Example: ```python from skllm.preprocessing import
+GPTTranslator from skllm.datasets import get_translation_dataset X =
+get_translation_dataset() t = GPTTranslator(openai_model="gpt-3.5-turbo",
+output_language="English") translated_text = t.fit_transform(X) ```
```

### Comparing `scikit-llm-0.3.0/pyproject.toml` & `scikit-llm-0.3.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   "openai>=0.27.0",
   "tqdm>=4.60.0",
   "annoy>=1.17.2",
   "google-cloud-aiplatform>=1.27.0",
   "vertexai<0.1.0"
 ]
 name = "scikit-llm"
-version = "0.3.0"
+version = "0.3.1"
 authors = [
   { name="Oleg Kostromin", email="kostromin97@gmail.com" },
   { name="Iryna Kondrashchenko", email="iryna230520@gmail.com" },
 ]
 description = "Scikit-LLM: Seamlessly integrate powerful language models like ChatGPT into scikit-learn for enhanced text analysis tasks."
 readme = "README.md"
 license = {text = "MIT"}
@@ -25,15 +25,15 @@
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.optional-dependencies]
-gpt4all = ["gpt4all>=0.2.0"]
+gpt4all = ["gpt4all>=1.0.0"]
 
 [tool.ruff]
 select = [
     # pycodestyle
     "E",
     # pyflakes
     "F",
```

### Comparing `scikit-llm-0.3.0/scikit_llm.egg-info/PKG-INFO` & `scikit-llm-0.3.1/scikit_llm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-llm
-Version: 0.3.0
+Version: 0.3.1
 Summary: Scikit-LLM: Seamlessly integrate powerful language models like ChatGPT into scikit-learn for enhanced text analysis tasks.
 Author-email: Oleg Kostromin <kostromin97@gmail.com>, Iryna Kondrashchenko <iryna230520@gmail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -32,16 +32,16 @@
 
 - ⭐ Star Scikit-LLM on GitHub (click the star button in the top right corner)
 - 💡 Provide your feedback or propose ideas in the [issues](https://github.com/iryna-kondr/scikit-llm/issues) section or [Discord](https://discord.gg/YDAbwuWK7V)
 - 📰 Post about Scikit-LLM on LinkedIn or other platforms
 
 ## Our Related Projects 🔗
 
-<a href="https://github.com/OKUA1/falcon"><img src="https://raw.githubusercontent.com/gist/OKUA1/6264a95a8abd225c74411a2b707b0242/raw/3cedb53538cb04656cd9d7d07e697e726896ce9f/falcon_light.svg"/></a> <br>
-<a href="https://github.com/OKUA1/agent_dingo"><img src="https://gist.githubusercontent.com/OKUA1/6264a95a8abd225c74411a2b707b0242/raw/1b231aab718fcab624faa33d9c10d0eee17ca160/dingo_light.svg"/></a>
+<a href="https://github.com/OKUA1/agent_dingo"><img src="https://gist.githubusercontent.com/OKUA1/6264a95a8abd225c74411a2b707b0242/raw/1b231aab718fcab624faa33d9c10d0eee17ca160/dingo_light.svg"/></a> <br>
+<a href="https://github.com/OKUA1/falcon"><img src="https://raw.githubusercontent.com/gist/OKUA1/6264a95a8abd225c74411a2b707b0242/raw/3cedb53538cb04656cd9d7d07e697e726896ce9f/falcon_light.svg"/></a>
 
 ## Documentation 📚
 
 ### Configuring OpenAI API Key
 
 At the moment the majority of the Scikit-LLM estimators are only compatible with some of the OpenAI models. Hence, a user-provided OpenAI API key is required.
 
@@ -58,15 +58,15 @@
 - When calling `SKLLMConfig.set_openai_org`, you have to provide your organization ID and **NOT** the name. You can find your ID [here](https://platform.openai.com/account/org-settings).
 
 ### Using Azure OpenAI
 
 ```python
 from skllm.config import SKLLMConfig
 
-SKLLMConfig.set_openai_key("<YOUR_KEY>") #use azure key instead
+SKLLMConfig.set_openai_key("<YOUR_KEY>")  # use azure key instead
 SKLLMConfig.set_azure_api_base("<API_BASE>")
 
 # start with "azure::" prefix when setting the model name
 model_name = "azure::<model_name>"
 # e.g. ZeroShotGPTClassifier(openai_model="azure::gpt-3.5-turbo")
 ```
 
@@ -86,15 +86,15 @@
 
 In order to switch from OpenAI to GPT4ALL model, simply provide a string of the format `gpt4all::<model_name>` as an argument. While the model runs completely locally, the estimator still treats it as an OpenAI endpoint and will try to check that the API key is present. You can provide any string as a key.
 
 ```python
 SKLLMConfig.set_openai_key("any string")
 SKLLMConfig.set_openai_org("any string")
 
-ZeroShotGPTClassifier(openai_model="gpt4all::ggml-gpt4all-j-v1.3-groovy")
+ZeroShotGPTClassifier(openai_model="gpt4all::ggml-model-gpt4all-falcon-q4_0.bin")
 ```
 
 When running for the first time, the model file will be downloaded automatially.
 
 When using gpt4all please keep the following in mind:
 
 1. Not all gpt4all models are commercially licensable, please consult gpt4all website for more details.
@@ -235,32 +235,33 @@
 clf.fit(X, y)
 labels = clf.predict(X)
 ```
 
 ### Text Classification with Google PaLM 2
 
 At the moment 3 PaLM based models are available in test mode:
+
 - `ZeroShotPaLMClassifier` - zero-shot text classification with PaLM 2;
 - `PaLMClassifier` - fine-tunable text classifier with PaLM 2;
 - `PaLM` - fine-tunable estimator that can be trained on arbitrary text input-output pairs.
 
-Example: 
+Example:
 
 ```python
 from skllm.models.palm import PaLMClassifier
 from skllm.datasets import get_classification_dataset
 
 X, y = get_classification_dataset()
 
 clf = PaLMClassifier(n_update_steps=100)
 clf.fit(X, y)
 labels = clf.predict(X)
 ```
 
-A more detailed documentation will follow soon. For now, please refer to our [official guide on Medium](https://medium.com/@iryna230520).
+A more detailed documentation will follow soon. For now, please refer to our [official guide on Medium](https://medium.com/@iryna230520/fine-tune-google-palm-2-with-scikit-llm-d41b0aa673a5).
 
 ### Text Vectorization
 
 As an alternative to using GPT as a classifier, it can be used solely for data preprocessing. `GPTVectorizer` allows to embed a chunk of text of arbitrary length to a fixed-dimensional vector, that can be used with virtually any classification or regression model.
 
 Example 1: Embedding the text
 
@@ -321,8 +322,7 @@
 from skllm.preprocessing import GPTTranslator
 from skllm.datasets import get_translation_dataset
 
 X = get_translation_dataset()
 t = GPTTranslator(openai_model="gpt-3.5-turbo", output_language="English")
 translated_text = t.fit_transform(X)
 ```
-
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: scikit-llm Version: 0.3.0 Summary: Scikit-LLM:
+Metadata-Version: 2.1 Name: scikit-llm Version: 0.3.1 Summary: Scikit-LLM:
 Seamlessly integrate powerful language models like ChatGPT into scikit-learn
 for enhanced text analysis tasks. Author-email: Oleg Kostromin
 gmail.com>, Iryna Kondrashchenko
 gmail.com> License: MIT Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.8 Description-Content-Type: text/
 markdown Provides-Extra: gpt4all License-File: LICENSE
@@ -11,71 +11,71 @@
 language models like ChatGPT into scikit-learn for enhanced text analysis
 tasks. ## Installation ð¾ ```bash pip install scikit-llm ``` ## Support us
 ð¤ You can support the project in the following ways: - â­ Star Scikit-LLM
 on GitHub (click the star button in the top right corner) - ð¡ Provide your
 feedback or propose ideas in the [issues](https://github.com/iryna-kondr/
 scikit-llm/issues) section or [Discord](https://discord.gg/YDAbwuWK7V) - ð°
 Post about Scikit-LLM on LinkedIn or other platforms ## Our Related Projects
-ð [https://raw.githubusercontent.com/gist/OKUA1/
-6264a95a8abd225c74411a2b707b0242/raw/3cedb53538cb04656cd9d7d07e697e726896ce9f/
-falcon_light.svg]
-[https://gist.githubusercontent.com/OKUA1/6264a95a8abd225c74411a2b707b0242/raw/
-1b231aab718fcab624faa33d9c10d0eee17ca160/dingo_light.svg] ## Documentation ð
-### Configuring OpenAI API Key At the moment the majority of the Scikit-LLM
-estimators are only compatible with some of the OpenAI models. Hence, a user-
-provided OpenAI API key is required. ```python from skllm.config import
+ð [https://gist.githubusercontent.com/OKUA1/
+6264a95a8abd225c74411a2b707b0242/raw/1b231aab718fcab624faa33d9c10d0eee17ca160/
+dingo_light.svg]
+[https://raw.githubusercontent.com/gist/OKUA1/6264a95a8abd225c74411a2b707b0242/
+raw/3cedb53538cb04656cd9d7d07e697e726896ce9f/falcon_light.svg] ## Documentation
+ð ### Configuring OpenAI API Key At the moment the majority of the Scikit-
+LLM estimators are only compatible with some of the OpenAI models. Hence, a
+user-provided OpenAI API key is required. ```python from skllm.config import
 SKLLMConfig SKLLMConfig.set_openai_key("") SKLLMConfig.set_openai_org("") ```
 **Important notice:** - If you have a free trial OpenAI account, the [rate
 limits](https://platform.openai.com/docs/guides/rate-limits/overview) are not
 sufficient (specifically 3 requests per minute). Please switch to the "pay as
 you go" plan first. - When calling `SKLLMConfig.set_openai_org`, you have to
 provide your organization ID and **NOT** the name. You can find your ID [here]
 (https://platform.openai.com/account/org-settings). ### Using Azure OpenAI
-```python from skllm.config import SKLLMConfig SKLLMConfig.set_openai_key("")
-#use azure key instead SKLLMConfig.set_azure_api_base("") # start with "azure::
+```python from skllm.config import SKLLMConfig SKLLMConfig.set_openai_key("") #
+use azure key instead SKLLMConfig.set_azure_api_base("") # start with "azure::
 " prefix when setting the model name model_name = "azure::" # e.g.
 ZeroShotGPTClassifier(openai_model="azure::gpt-3.5-turbo") ``` Note: Azure
 OpenAI is not supported by the preprocessors at the moment. ### Using GPT4ALL
 In addition to OpenAI, some of the models can use [gpt4all](https://gpt4all.io/
 index.html) as a backend. **This feature is considered higly experimental!** In
 order to use gpt4all, you need to install the corresponding submodule: ```bash
 pip install "scikit-llm[gpt4all]" ``` In order to switch from OpenAI to GPT4ALL
 model, simply provide a string of the format `gpt4all::` as an argument. While
 the model runs completely locally, the estimator still treats it as an OpenAI
 endpoint and will try to check that the API key is present. You can provide any
 string as a key. ```python SKLLMConfig.set_openai_key("any string")
 SKLLMConfig.set_openai_org("any string") ZeroShotGPTClassifier
-(openai_model="gpt4all::ggml-gpt4all-j-v1.3-groovy") ``` When running for the
-first time, the model file will be downloaded automatially. When using gpt4all
-please keep the following in mind: 1. Not all gpt4all models are commercially
-licensable, please consult gpt4all website for more details. 2. The accuracy of
-the models may be much lower compared to ones provided by OpenAI (especially
-gpt-4). 3. Not all of the available models were tested, some may not work with
-scikit-llm at all. ### Supported models by a non-standard backend At the moment
-only the following estimators support non-standard backends (gpt4all, azure): -
-`ZeroShotGPTClassifier` - `MultiLabelZeroShotGPTClassifier` -
-`FewShotGPTClassifier` ### Zero-Shot Text Classification One of the powerful
-ChatGPT features is the ability to perform text classification without being
-re-trained. For that, the only requirement is that the labels must be
-descriptive. We provide a class `ZeroShotGPTClassifier` that allows to create
-such a model as a regular scikit-learn classifier. Example 1: Training as a
-regular classifier ```python from skllm import ZeroShotGPTClassifier from
-skllm.datasets import get_classification_dataset # demo sentiment analysis
-dataset # labels: positive, negative, neutral X, y = get_classification_dataset
-() clf = ZeroShotGPTClassifier(openai_model="gpt-3.5-turbo") clf.fit(X, y)
-labels = clf.predict(X) ``` Scikit-LLM will automatically query the OpenAI API
-and transform the response into a regular list of labels. Additionally, Scikit-
-LLM will ensure that the obtained response contains a valid label. If this is
-not the case, a label will be selected randomly (label probabilities are
-proportional to label occurrences in the training set). Example 2: Training
-without labeled data Since the training data is not strictly required, it can
-be fully ommited. The only thing that has to be provided is the list of
-candidate labels. ```python from skllm import ZeroShotGPTClassifier from
-skllm.datasets import get_classification_dataset X, _ =
-get_classification_dataset() clf = ZeroShotGPTClassifier() clf.fit(None,
+(openai_model="gpt4all::ggml-model-gpt4all-falcon-q4_0.bin") ``` When running
+for the first time, the model file will be downloaded automatially. When using
+gpt4all please keep the following in mind: 1. Not all gpt4all models are
+commercially licensable, please consult gpt4all website for more details. 2.
+The accuracy of the models may be much lower compared to ones provided by
+OpenAI (especially gpt-4). 3. Not all of the available models were tested, some
+may not work with scikit-llm at all. ### Supported models by a non-standard
+backend At the moment only the following estimators support non-standard
+backends (gpt4all, azure): - `ZeroShotGPTClassifier` -
+`MultiLabelZeroShotGPTClassifier` - `FewShotGPTClassifier` ### Zero-Shot Text
+Classification One of the powerful ChatGPT features is the ability to perform
+text classification without being re-trained. For that, the only requirement is
+that the labels must be descriptive. We provide a class `ZeroShotGPTClassifier`
+that allows to create such a model as a regular scikit-learn classifier.
+Example 1: Training as a regular classifier ```python from skllm import
+ZeroShotGPTClassifier from skllm.datasets import get_classification_dataset #
+demo sentiment analysis dataset # labels: positive, negative, neutral X, y =
+get_classification_dataset() clf = ZeroShotGPTClassifier(openai_model="gpt-3.5-
+turbo") clf.fit(X, y) labels = clf.predict(X) ``` Scikit-LLM will automatically
+query the OpenAI API and transform the response into a regular list of labels.
+Additionally, Scikit-LLM will ensure that the obtained response contains a
+valid label. If this is not the case, a label will be selected randomly (label
+probabilities are proportional to label occurrences in the training set).
+Example 2: Training without labeled data Since the training data is not
+strictly required, it can be fully ommited. The only thing that has to be
+provided is the list of candidate labels. ```python from skllm import
+ZeroShotGPTClassifier from skllm.datasets import get_classification_dataset X,
+_ = get_classification_dataset() clf = ZeroShotGPTClassifier() clf.fit(None,
 ["positive", "negative", "neutral"]) labels = clf.predict(X) ``` **Note:**
 unlike in a typical supervised setting, the performance of a zero-shot
 classifier greatly depends on how the label itself is structured. It has to be
 expressed in natural language, be descriptive and self-explanatory. For
 example, in the previous semantic classification task, it could be beneficial
 to transform a label from `""` to `"the semantics of the provided text is "`.
 ### Multi-Label Zero-Shot Text Classification With a class
@@ -123,39 +123,39 @@
 `PaLMClassifier` - fine-tunable text classifier with PaLM 2; - `PaLM` - fine-
 tunable estimator that can be trained on arbitrary text input-output pairs.
 Example: ```python from skllm.models.palm import PaLMClassifier from
 skllm.datasets import get_classification_dataset X, y =
 get_classification_dataset() clf = PaLMClassifier(n_update_steps=100) clf.fit
 (X, y) labels = clf.predict(X) ``` A more detailed documentation will follow
 soon. For now, please refer to our [official guide on Medium](https://
-medium.com/@iryna230520). ### Text Vectorization As an alternative to using GPT
-as a classifier, it can be used solely for data preprocessing. `GPTVectorizer`
-allows to embed a chunk of text of arbitrary length to a fixed-dimensional
-vector, that can be used with virtually any classification or regression model.
-Example 1: Embedding the text ```python from skllm.preprocessing import
-GPTVectorizer model = GPTVectorizer() vectors = model.fit_transform(X) ```
-Example 2: Combining the Vectorizer with the XGBoost Classifier in a Sklearn
-Pipeline ```python from sklearn.pipeline import Pipeline from
-sklearn.preprocessing import LabelEncoder from xgboost import XGBClassifier le
-= LabelEncoder() y_train_encoded = le.fit_transform(y_train) y_test_encoded =
-le.transform(y_test) steps = [("GPT", GPTVectorizer()), ("Clf", XGBClassifier
-())] clf = Pipeline(steps) clf.fit(X_train, y_train_encoded) yh = clf.predict
-(X_test) ``` ### Text Summarization GPT excels at performing summarization
-tasks. Therefore, we provide `GPTSummarizer` that can be used both as stand-
-alone estimator, or as a preprocessor (in this case we can make an analogy with
-a dimensionality reduction preprocessor). Example: ```python from
-skllm.preprocessing import GPTSummarizer from skllm.datasets import
-get_summarization_dataset X = get_summarization_dataset() s = GPTSummarizer
-(openai_model="gpt-3.5-turbo", max_words=15) summaries = s.fit_transform(X) ```
-Please be aware that the `max_words` hyperparameter sets a soft limit, which is
-not strictly enforced outside of the prompt. Therefore, in some cases, the
-actual number of words might be slightly higher. It is possible to generate a
-summary, emphasizing a specific concept, by providing an optional parameter
-`focus`: ```python s = GPTSummarizer(openai_model="gpt-3.5-turbo",
-max_words=15, focus="apples") ``` ### Text Translation GPT models have
-demonstrated their effectiveness in translation tasks by generating accurate
-translations across various languages. Thus, we added `GPTTranslator` that
-allows translating an arbitraty text into a language of interest. Example:
-```python from skllm.preprocessing import GPTTranslator from skllm.datasets
-import get_translation_dataset X = get_translation_dataset() t = GPTTranslator
-(openai_model="gpt-3.5-turbo", output_language="English") translated_text =
-t.fit_transform(X) ```
+medium.com/@iryna230520/fine-tune-google-palm-2-with-scikit-llm-d41b0aa673a5).
+### Text Vectorization As an alternative to using GPT as a classifier, it can
+be used solely for data preprocessing. `GPTVectorizer` allows to embed a chunk
+of text of arbitrary length to a fixed-dimensional vector, that can be used
+with virtually any classification or regression model. Example 1: Embedding the
+text ```python from skllm.preprocessing import GPTVectorizer model =
+GPTVectorizer() vectors = model.fit_transform(X) ``` Example 2: Combining the
+Vectorizer with the XGBoost Classifier in a Sklearn Pipeline ```python from
+sklearn.pipeline import Pipeline from sklearn.preprocessing import LabelEncoder
+from xgboost import XGBClassifier le = LabelEncoder() y_train_encoded =
+le.fit_transform(y_train) y_test_encoded = le.transform(y_test) steps = [
+("GPT", GPTVectorizer()), ("Clf", XGBClassifier())] clf = Pipeline(steps)
+clf.fit(X_train, y_train_encoded) yh = clf.predict(X_test) ``` ### Text
+Summarization GPT excels at performing summarization tasks. Therefore, we
+provide `GPTSummarizer` that can be used both as stand-alone estimator, or as a
+preprocessor (in this case we can make an analogy with a dimensionality
+reduction preprocessor). Example: ```python from skllm.preprocessing import
+GPTSummarizer from skllm.datasets import get_summarization_dataset X =
+get_summarization_dataset() s = GPTSummarizer(openai_model="gpt-3.5-turbo",
+max_words=15) summaries = s.fit_transform(X) ``` Please be aware that the
+`max_words` hyperparameter sets a soft limit, which is not strictly enforced
+outside of the prompt. Therefore, in some cases, the actual number of words
+might be slightly higher. It is possible to generate a summary, emphasizing a
+specific concept, by providing an optional parameter `focus`: ```python s =
+GPTSummarizer(openai_model="gpt-3.5-turbo", max_words=15, focus="apples") ```
+### Text Translation GPT models have demonstrated their effectiveness in
+translation tasks by generating accurate translations across various languages.
+Thus, we added `GPTTranslator` that allows translating an arbitraty text into a
+language of interest. Example: ```python from skllm.preprocessing import
+GPTTranslator from skllm.datasets import get_translation_dataset X =
+get_translation_dataset() t = GPTTranslator(openai_model="gpt-3.5-turbo",
+output_language="English") translated_text = t.fit_transform(X) ```
```

### Comparing `scikit-llm-0.3.0/scikit_llm.egg-info/SOURCES.txt` & `scikit-llm-0.3.1/scikit_llm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.3.0/skllm/completions.py` & `scikit-llm-0.3.1/skllm/completions.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.3.0/skllm/config.py` & `scikit-llm-0.3.1/skllm/config.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.3.0/skllm/datasets/multi_class.py` & `scikit-llm-0.3.1/skllm/datasets/multi_class.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.3.0/skllm/datasets/multi_label.py` & `scikit-llm-0.3.1/skllm/datasets/multi_label.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.3.0/skllm/datasets/summarization.py` & `scikit-llm-0.3.1/skllm/datasets/summarization.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.3.0/skllm/datasets/translation.py` & `scikit-llm-0.3.1/skllm/datasets/translation.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.3.0/skllm/google/completions.py` & `scikit-llm-0.3.1/skllm/google/completions.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.3.0/skllm/gpt4all_client.py` & `scikit-llm-0.3.1/skllm/gpt4all_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,17 +4,22 @@
     from gpt4all import GPT4All
 except (ImportError, ModuleNotFoundError):
     GPT4All = None
 
 _loaded_models = {}
 
 
-def get_chat_completion(messages: Dict, model: str="ggml-gpt4all-j-v1.3-groovy") -> Dict:
-    """
-    Gets a chat completion from GPT4All
+def _make_openai_compatabile(message: str) -> Dict:
+    return {"choices": [{"message": {"content": message, "role": "assistant"}}]}
+
+
+def get_chat_completion(
+    messages: Dict, model: str = "ggml-model-gpt4all-falcon-q4_0.bin"
+) -> Dict:
+    """Gets a chat completion from GPT4All.
 
     Parameters
     ----------
     messages : Dict
         The messages to use as a prompt for the chat completion.
     model : str
         The model to use for the chat completion. Defaults to "ggml-gpt4all-j-v1.3-groovy".
@@ -24,17 +29,26 @@
     completion : Dict
     """
     if GPT4All is None:
         raise ImportError(
             "gpt4all is not installed, try `pip install scikit-llm[gpt4all]`"
         )
     if model not in _loaded_models.keys():
-        _loaded_models[model] = GPT4All(model)
+        loaded_model = GPT4All(model)
+        _loaded_models[model] = loaded_model
+        loaded_model._current_prompt_template = loaded_model.config["promptTemplate"]
 
-    return _loaded_models[model].chat_completion(
-        messages, verbose=False, streaming=False, temp=1e-10
+    prompt = _loaded_models[model]._format_chat_prompt_template(
+        messages, _loaded_models[model].config["systemPrompt"]
     )
+    generated = _loaded_models[model].generate(
+        prompt,
+        streaming=False,
+        temp=1e-10,
+    )
+
+    return _make_openai_compatabile(generated)
 
 
 def unload_models() -> None:
     global _loaded_models
     _loaded_models = {}
```

### Comparing `scikit-llm-0.3.0/skllm/memory/_annoy.py` & `scikit-llm-0.3.1/skllm/memory/_annoy.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.3.0/skllm/memory/base.py` & `scikit-llm-0.3.1/skllm/memory/base.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.3.0/skllm/models/_base.py` & `scikit-llm-0.3.1/skllm/models/_base.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.3.0/skllm/models/gpt/gpt_dyn_few_shot_clf.py` & `scikit-llm-0.3.1/skllm/models/gpt/gpt_dyn_few_shot_clf.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.3.0/skllm/models/gpt/gpt_few_shot_clf.py` & `scikit-llm-0.3.1/skllm/models/gpt/gpt_few_shot_clf.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.3.0/skllm/models/gpt/gpt_zero_shot_clf.py` & `scikit-llm-0.3.1/skllm/models/gpt/gpt_zero_shot_clf.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.3.0/skllm/models/palm/palm_clf.py` & `scikit-llm-0.3.1/skllm/models/palm/palm_clf.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.3.0/skllm/models/palm/palm_est.py` & `scikit-llm-0.3.1/skllm/models/palm/palm_est.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.3.0/skllm/openai/base_gpt.py` & `scikit-llm-0.3.1/skllm/openai/base_gpt.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.3.0/skllm/openai/chatgpt.py` & `scikit-llm-0.3.1/skllm/openai/chatgpt.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.3.0/skllm/openai/credentials.py` & `scikit-llm-0.3.1/skllm/openai/credentials.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.3.0/skllm/openai/embeddings.py` & `scikit-llm-0.3.1/skllm/openai/embeddings.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.3.0/skllm/openai/mixin.py` & `scikit-llm-0.3.1/skllm/openai/mixin.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.3.0/skllm/preprocessing/gpt_summarizer.py` & `scikit-llm-0.3.1/skllm/preprocessing/gpt_summarizer.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.3.0/skllm/preprocessing/gpt_translator.py` & `scikit-llm-0.3.1/skllm/preprocessing/gpt_translator.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.3.0/skllm/preprocessing/gpt_vectorizer.py` & `scikit-llm-0.3.1/skllm/preprocessing/gpt_vectorizer.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.3.0/skllm/prompts/builders.py` & `scikit-llm-0.3.1/skllm/prompts/builders.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.3.0/skllm/prompts/templates.py` & `scikit-llm-0.3.1/skllm/prompts/templates.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.3.0/skllm/utils.py` & `scikit-llm-0.3.1/skllm/utils.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.3.0/tests/test_chatgpt.py` & `scikit-llm-0.3.1/tests/test_chatgpt.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.3.0/tests/test_gpt_few_shot_clf.py` & `scikit-llm-0.3.1/tests/test_gpt_few_shot_clf.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.3.0/tests/test_gpt_zero_shot_clf.py` & `scikit-llm-0.3.1/tests/test_gpt_zero_shot_clf.py`

 * *Files identical despite different names*

