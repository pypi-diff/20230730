# Comparing `tmp/langchain_experimental-0.0.7.tar.gz` & `tmp/langchain_experimental-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_experimental-0.0.7.tar", max compression
+gzip compressed data, was "langchain_experimental-0.0.8.tar", max compression
```

## Comparing `langchain_experimental-0.0.7.tar` & `langchain_experimental-0.0.8.tar`

### file list

```diff
@@ -1,64 +1,65 @@
--rw-r--r--   0        0        0       93 2023-07-29 00:17:08.308358 langchain_experimental-0.0.7/README.md
--rw-r--r--   0        0        0        0 2023-07-29 00:17:08.308358 langchain_experimental-0.0.7/langchain_experimental/__init__.py
--rw-r--r--   0        0        0      288 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/autonomous_agents/__init__.py
--rw-r--r--   0        0        0        0 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/autonomous_agents/autogpt/__init__.py
--rw-r--r--   0        0        0     5244 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/autonomous_agents/autogpt/agent.py
--rw-r--r--   0        0        0     1103 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/autonomous_agents/autogpt/memory.py
--rw-r--r--   0        0        0     1882 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/autonomous_agents/autogpt/output_parser.py
--rw-r--r--   0        0        0     3305 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/autonomous_agents/autogpt/prompt.py
--rw-r--r--   0        0        0     6573 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/autonomous_agents/autogpt/prompt_generator.py
--rw-r--r--   0        0        0      514 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/autonomous_agents/baby_agi/__init__.py
--rw-r--r--   0        0        0     7469 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/autonomous_agents/baby_agi/baby_agi.py
--rw-r--r--   0        0        0     1282 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/autonomous_agents/baby_agi/task_creation.py
--rw-r--r--   0        0        0      835 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/autonomous_agents/baby_agi/task_execution.py
--rw-r--r--   0        0        0     1076 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/autonomous_agents/baby_agi/task_prioritization.py
--rw-r--r--   0        0        0        0 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/autonomous_agents/hugginggpt/__init__.py
--rw-r--r--   0        0        0     1083 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/autonomous_agents/hugginggpt/hugginggpt.py
--rw-r--r--   0        0        0     1450 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/autonomous_agents/hugginggpt/repsonse_generator.py
--rw-r--r--   0        0        0     4551 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/autonomous_agents/hugginggpt/task_executor.py
--rw-r--r--   0        0        0     6439 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/autonomous_agents/hugginggpt/task_planner.py
--rw-r--r--   0        0        0      100 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/cpal/README.md
--rw-r--r--   0        0        0        0 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/cpal/__init__.py
--rw-r--r--   0        0        0     9041 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/cpal/base.py
--rw-r--r--   0        0        0      246 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/cpal/constants.py
--rw-r--r--   0        0        0     8322 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/cpal/models.py
--rw-r--r--   0        0        0        0 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/cpal/templates/__init__.py
--rw-r--r--   0        0        0        0 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/cpal/templates/univariate/__init__.py
--rw-r--r--   0        0        0     2175 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/cpal/templates/univariate/causal.py
--rw-r--r--   0        0        0      706 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/cpal/templates/univariate/intervention.py
--rw-r--r--   0        0        0     1750 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/cpal/templates/univariate/narrative.py
--rw-r--r--   0        0        0     4503 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/cpal/templates/univariate/query.py
--rw-r--r--   0        0        0      260 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/generative_agents/__init__.py
--rw-r--r--   0        0        0    10158 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/generative_agents/generative_agent.py
--rw-r--r--   0        0        0    12500 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/generative_agents/memory.py
--rw-r--r--   0        0        0      277 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/llms/__init__.py
--rw-r--r--   0        0        0     1965 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/llms/jsonformer_decoder.py
--rw-r--r--   0        0        0     4279 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/llms/llamaapi.py
--rw-r--r--   0        0        0     2089 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/llms/rellm_decoder.py
--rw-r--r--   0        0        0      277 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/pal_chain/__init__.py
--rw-r--r--   0        0        0    11672 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/pal_chain/base.py
--rw-r--r--   0        0        0     2645 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/pal_chain/colored_object_prompt.py
--rw-r--r--   0        0        0     4301 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/pal_chain/math_prompt.py
--rw-r--r--   0        0        0      363 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/plan_and_execute/__init__.py
--rw-r--r--   0        0        0     3544 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/plan_and_execute/agent_executor.py
--rw-r--r--   0        0        0        0 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/plan_and_execute/executors/__init__.py
--rw-r--r--   0        0        0     1464 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/plan_and_execute/executors/agent_executor.py
--rw-r--r--   0        0        0     1243 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/plan_and_execute/executors/base.py
--rw-r--r--   0        0        0        0 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/plan_and_execute/planners/__init__.py
--rw-r--r--   0        0        0     1541 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/plan_and_execute/planners/base.py
--rw-r--r--   0        0        0     1836 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/plan_and_execute/planners/chat_planner.py
--rw-r--r--   0        0        0     1391 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/plan_and_execute/schema.py
--rw-r--r--   0        0        0       87 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/prompts/__init__.py
--rw-r--r--   0        0        0     1873 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/prompts/load.py
--rw-r--r--   0        0        0      140 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/sql/__init__.py
--rw-r--r--   0        0        0    11413 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/sql/base.py
--rw-r--r--   0        0        0      149 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/tot/__init__.py
--rw-r--r--   0        0        0     5087 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/tot/base.py
--rw-r--r--   0        0        0     1405 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/tot/checker.py
--rw-r--r--   0        0        0     1666 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/tot/controller.py
--rw-r--r--   0        0        0     1456 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/tot/memory.py
--rw-r--r--   0        0        0     3534 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/tot/prompts.py
--rw-r--r--   0        0        0      398 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/tot/thought.py
--rw-r--r--   0        0        0     3026 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/tot/thought_generation.py
--rw-r--r--   0        0        0     1904 2023-07-29 00:17:08.328358 langchain_experimental-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      717 1970-01-01 00:00:00.000000 langchain_experimental-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0       93 2023-07-30 14:28:35.264821 langchain_experimental-0.0.8/README.md
+-rw-r--r--   0        0        0        0 2023-07-30 14:28:35.264821 langchain_experimental-0.0.8/langchain_experimental/__init__.py
+-rw-r--r--   0        0        0      288 2023-07-30 14:28:35.264821 langchain_experimental-0.0.8/langchain_experimental/autonomous_agents/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-30 14:28:35.264821 langchain_experimental-0.0.8/langchain_experimental/autonomous_agents/autogpt/__init__.py
+-rw-r--r--   0        0        0     5244 2023-07-30 14:28:35.264821 langchain_experimental-0.0.8/langchain_experimental/autonomous_agents/autogpt/agent.py
+-rw-r--r--   0        0        0     1103 2023-07-30 14:28:35.264821 langchain_experimental-0.0.8/langchain_experimental/autonomous_agents/autogpt/memory.py
+-rw-r--r--   0        0        0     1882 2023-07-30 14:28:35.264821 langchain_experimental-0.0.8/langchain_experimental/autonomous_agents/autogpt/output_parser.py
+-rw-r--r--   0        0        0     3305 2023-07-30 14:28:35.264821 langchain_experimental-0.0.8/langchain_experimental/autonomous_agents/autogpt/prompt.py
+-rw-r--r--   0        0        0     6573 2023-07-30 14:28:35.264821 langchain_experimental-0.0.8/langchain_experimental/autonomous_agents/autogpt/prompt_generator.py
+-rw-r--r--   0        0        0      514 2023-07-30 14:28:35.264821 langchain_experimental-0.0.8/langchain_experimental/autonomous_agents/baby_agi/__init__.py
+-rw-r--r--   0        0        0     7469 2023-07-30 14:28:35.264821 langchain_experimental-0.0.8/langchain_experimental/autonomous_agents/baby_agi/baby_agi.py
+-rw-r--r--   0        0        0     1282 2023-07-30 14:28:35.264821 langchain_experimental-0.0.8/langchain_experimental/autonomous_agents/baby_agi/task_creation.py
+-rw-r--r--   0        0        0      835 2023-07-30 14:28:35.264821 langchain_experimental-0.0.8/langchain_experimental/autonomous_agents/baby_agi/task_execution.py
+-rw-r--r--   0        0        0     1076 2023-07-30 14:28:35.264821 langchain_experimental-0.0.8/langchain_experimental/autonomous_agents/baby_agi/task_prioritization.py
+-rw-r--r--   0        0        0        0 2023-07-30 14:28:35.264821 langchain_experimental-0.0.8/langchain_experimental/autonomous_agents/hugginggpt/__init__.py
+-rw-r--r--   0        0        0     1083 2023-07-30 14:28:35.264821 langchain_experimental-0.0.8/langchain_experimental/autonomous_agents/hugginggpt/hugginggpt.py
+-rw-r--r--   0        0        0     1450 2023-07-30 14:28:35.264821 langchain_experimental-0.0.8/langchain_experimental/autonomous_agents/hugginggpt/repsonse_generator.py
+-rw-r--r--   0        0        0     4551 2023-07-30 14:28:35.264821 langchain_experimental-0.0.8/langchain_experimental/autonomous_agents/hugginggpt/task_executor.py
+-rw-r--r--   0        0        0     6439 2023-07-30 14:28:35.264821 langchain_experimental-0.0.8/langchain_experimental/autonomous_agents/hugginggpt/task_planner.py
+-rw-r--r--   0        0        0      100 2023-07-30 14:28:35.264821 langchain_experimental-0.0.8/langchain_experimental/cpal/README.md
+-rw-r--r--   0        0        0        0 2023-07-30 14:28:35.264821 langchain_experimental-0.0.8/langchain_experimental/cpal/__init__.py
+-rw-r--r--   0        0        0     9041 2023-07-30 14:28:35.264821 langchain_experimental-0.0.8/langchain_experimental/cpal/base.py
+-rw-r--r--   0        0        0      246 2023-07-30 14:28:35.264821 langchain_experimental-0.0.8/langchain_experimental/cpal/constants.py
+-rw-r--r--   0        0        0     8322 2023-07-30 14:28:35.264821 langchain_experimental-0.0.8/langchain_experimental/cpal/models.py
+-rw-r--r--   0        0        0        0 2023-07-30 14:28:35.264821 langchain_experimental-0.0.8/langchain_experimental/cpal/templates/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-30 14:28:35.264821 langchain_experimental-0.0.8/langchain_experimental/cpal/templates/univariate/__init__.py
+-rw-r--r--   0        0        0     2175 2023-07-30 14:28:35.264821 langchain_experimental-0.0.8/langchain_experimental/cpal/templates/univariate/causal.py
+-rw-r--r--   0        0        0      706 2023-07-30 14:28:35.264821 langchain_experimental-0.0.8/langchain_experimental/cpal/templates/univariate/intervention.py
+-rw-r--r--   0        0        0     1750 2023-07-30 14:28:35.264821 langchain_experimental-0.0.8/langchain_experimental/cpal/templates/univariate/narrative.py
+-rw-r--r--   0        0        0     4503 2023-07-30 14:28:35.264821 langchain_experimental-0.0.8/langchain_experimental/cpal/templates/univariate/query.py
+-rw-r--r--   0        0        0      260 2023-07-30 14:28:35.264821 langchain_experimental-0.0.8/langchain_experimental/generative_agents/__init__.py
+-rw-r--r--   0        0        0    10158 2023-07-30 14:28:35.264821 langchain_experimental-0.0.8/langchain_experimental/generative_agents/generative_agent.py
+-rw-r--r--   0        0        0    12500 2023-07-30 14:28:35.264821 langchain_experimental-0.0.8/langchain_experimental/generative_agents/memory.py
+-rw-r--r--   0        0        0      277 2023-07-30 14:28:35.264821 langchain_experimental-0.0.8/langchain_experimental/llms/__init__.py
+-rw-r--r--   0        0        0     7520 2023-07-30 14:28:35.264821 langchain_experimental-0.0.8/langchain_experimental/llms/anthropic_functions.py
+-rw-r--r--   0        0        0     1965 2023-07-30 14:28:35.264821 langchain_experimental-0.0.8/langchain_experimental/llms/jsonformer_decoder.py
+-rw-r--r--   0        0        0     4279 2023-07-30 14:28:35.264821 langchain_experimental-0.0.8/langchain_experimental/llms/llamaapi.py
+-rw-r--r--   0        0        0     2089 2023-07-30 14:28:35.264821 langchain_experimental-0.0.8/langchain_experimental/llms/rellm_decoder.py
+-rw-r--r--   0        0        0      277 2023-07-30 14:28:35.264821 langchain_experimental-0.0.8/langchain_experimental/pal_chain/__init__.py
+-rw-r--r--   0        0        0    11672 2023-07-30 14:28:35.264821 langchain_experimental-0.0.8/langchain_experimental/pal_chain/base.py
+-rw-r--r--   0        0        0     2645 2023-07-30 14:28:35.264821 langchain_experimental-0.0.8/langchain_experimental/pal_chain/colored_object_prompt.py
+-rw-r--r--   0        0        0     4301 2023-07-30 14:28:35.264821 langchain_experimental-0.0.8/langchain_experimental/pal_chain/math_prompt.py
+-rw-r--r--   0        0        0      363 2023-07-30 14:28:35.264821 langchain_experimental-0.0.8/langchain_experimental/plan_and_execute/__init__.py
+-rw-r--r--   0        0        0     3544 2023-07-30 14:28:35.264821 langchain_experimental-0.0.8/langchain_experimental/plan_and_execute/agent_executor.py
+-rw-r--r--   0        0        0        0 2023-07-30 14:28:35.264821 langchain_experimental-0.0.8/langchain_experimental/plan_and_execute/executors/__init__.py
+-rw-r--r--   0        0        0     1464 2023-07-30 14:28:35.264821 langchain_experimental-0.0.8/langchain_experimental/plan_and_execute/executors/agent_executor.py
+-rw-r--r--   0        0        0     1243 2023-07-30 14:28:35.264821 langchain_experimental-0.0.8/langchain_experimental/plan_and_execute/executors/base.py
+-rw-r--r--   0        0        0        0 2023-07-30 14:28:35.264821 langchain_experimental-0.0.8/langchain_experimental/plan_and_execute/planners/__init__.py
+-rw-r--r--   0        0        0     1541 2023-07-30 14:28:35.264821 langchain_experimental-0.0.8/langchain_experimental/plan_and_execute/planners/base.py
+-rw-r--r--   0        0        0     1836 2023-07-30 14:28:35.264821 langchain_experimental-0.0.8/langchain_experimental/plan_and_execute/planners/chat_planner.py
+-rw-r--r--   0        0        0     1391 2023-07-30 14:28:35.264821 langchain_experimental-0.0.8/langchain_experimental/plan_and_execute/schema.py
+-rw-r--r--   0        0        0       87 2023-07-30 14:28:35.268821 langchain_experimental-0.0.8/langchain_experimental/prompts/__init__.py
+-rw-r--r--   0        0        0     1873 2023-07-30 14:28:35.268821 langchain_experimental-0.0.8/langchain_experimental/prompts/load.py
+-rw-r--r--   0        0        0      140 2023-07-30 14:28:35.268821 langchain_experimental-0.0.8/langchain_experimental/sql/__init__.py
+-rw-r--r--   0        0        0    11413 2023-07-30 14:28:35.268821 langchain_experimental-0.0.8/langchain_experimental/sql/base.py
+-rw-r--r--   0        0        0      149 2023-07-30 14:28:35.268821 langchain_experimental-0.0.8/langchain_experimental/tot/__init__.py
+-rw-r--r--   0        0        0     5087 2023-07-30 14:28:35.268821 langchain_experimental-0.0.8/langchain_experimental/tot/base.py
+-rw-r--r--   0        0        0     1405 2023-07-30 14:28:35.268821 langchain_experimental-0.0.8/langchain_experimental/tot/checker.py
+-rw-r--r--   0        0        0     1666 2023-07-30 14:28:35.268821 langchain_experimental-0.0.8/langchain_experimental/tot/controller.py
+-rw-r--r--   0        0        0     1456 2023-07-30 14:28:35.268821 langchain_experimental-0.0.8/langchain_experimental/tot/memory.py
+-rw-r--r--   0        0        0     3534 2023-07-30 14:28:35.268821 langchain_experimental-0.0.8/langchain_experimental/tot/prompts.py
+-rw-r--r--   0        0        0      398 2023-07-30 14:28:35.268821 langchain_experimental-0.0.8/langchain_experimental/tot/thought.py
+-rw-r--r--   0        0        0     3026 2023-07-30 14:28:35.268821 langchain_experimental-0.0.8/langchain_experimental/tot/thought_generation.py
+-rw-r--r--   0        0        0     1904 2023-07-30 14:28:35.272822 langchain_experimental-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      717 1970-01-01 00:00:00.000000 langchain_experimental-0.0.8/PKG-INFO
```

### Comparing `langchain_experimental-0.0.7/langchain_experimental/autonomous_agents/autogpt/agent.py` & `langchain_experimental-0.0.8/langchain_experimental/autonomous_agents/autogpt/agent.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.7/langchain_experimental/autonomous_agents/autogpt/memory.py` & `langchain_experimental-0.0.8/langchain_experimental/autonomous_agents/autogpt/memory.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.7/langchain_experimental/autonomous_agents/autogpt/output_parser.py` & `langchain_experimental-0.0.8/langchain_experimental/autonomous_agents/autogpt/output_parser.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.7/langchain_experimental/autonomous_agents/autogpt/prompt.py` & `langchain_experimental-0.0.8/langchain_experimental/autonomous_agents/autogpt/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.7/langchain_experimental/autonomous_agents/autogpt/prompt_generator.py` & `langchain_experimental-0.0.8/langchain_experimental/autonomous_agents/autogpt/prompt_generator.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.7/langchain_experimental/autonomous_agents/baby_agi/__init__.py` & `langchain_experimental-0.0.8/langchain_experimental/autonomous_agents/baby_agi/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.7/langchain_experimental/autonomous_agents/baby_agi/baby_agi.py` & `langchain_experimental-0.0.8/langchain_experimental/autonomous_agents/baby_agi/baby_agi.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.7/langchain_experimental/autonomous_agents/baby_agi/task_creation.py` & `langchain_experimental-0.0.8/langchain_experimental/autonomous_agents/baby_agi/task_creation.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.7/langchain_experimental/autonomous_agents/baby_agi/task_execution.py` & `langchain_experimental-0.0.8/langchain_experimental/autonomous_agents/baby_agi/task_execution.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.7/langchain_experimental/autonomous_agents/baby_agi/task_prioritization.py` & `langchain_experimental-0.0.8/langchain_experimental/autonomous_agents/baby_agi/task_prioritization.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.7/langchain_experimental/autonomous_agents/hugginggpt/hugginggpt.py` & `langchain_experimental-0.0.8/langchain_experimental/autonomous_agents/hugginggpt/hugginggpt.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.7/langchain_experimental/autonomous_agents/hugginggpt/repsonse_generator.py` & `langchain_experimental-0.0.8/langchain_experimental/autonomous_agents/hugginggpt/repsonse_generator.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.7/langchain_experimental/autonomous_agents/hugginggpt/task_executor.py` & `langchain_experimental-0.0.8/langchain_experimental/autonomous_agents/hugginggpt/task_executor.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.7/langchain_experimental/autonomous_agents/hugginggpt/task_planner.py` & `langchain_experimental-0.0.8/langchain_experimental/autonomous_agents/hugginggpt/task_planner.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.7/langchain_experimental/cpal/base.py` & `langchain_experimental-0.0.8/langchain_experimental/cpal/base.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.7/langchain_experimental/cpal/models.py` & `langchain_experimental-0.0.8/langchain_experimental/cpal/models.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.7/langchain_experimental/cpal/templates/univariate/causal.py` & `langchain_experimental-0.0.8/langchain_experimental/cpal/templates/univariate/causal.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.7/langchain_experimental/cpal/templates/univariate/intervention.py` & `langchain_experimental-0.0.8/langchain_experimental/cpal/templates/univariate/intervention.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.7/langchain_experimental/cpal/templates/univariate/narrative.py` & `langchain_experimental-0.0.8/langchain_experimental/cpal/templates/univariate/narrative.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.7/langchain_experimental/cpal/templates/univariate/query.py` & `langchain_experimental-0.0.8/langchain_experimental/cpal/templates/univariate/query.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.7/langchain_experimental/generative_agents/generative_agent.py` & `langchain_experimental-0.0.8/langchain_experimental/generative_agents/generative_agent.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.7/langchain_experimental/generative_agents/memory.py` & `langchain_experimental-0.0.8/langchain_experimental/generative_agents/memory.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.7/langchain_experimental/llms/jsonformer_decoder.py` & `langchain_experimental-0.0.8/langchain_experimental/llms/jsonformer_decoder.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.7/langchain_experimental/llms/llamaapi.py` & `langchain_experimental-0.0.8/langchain_experimental/llms/llamaapi.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.7/langchain_experimental/llms/rellm_decoder.py` & `langchain_experimental-0.0.8/langchain_experimental/llms/rellm_decoder.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.7/langchain_experimental/pal_chain/base.py` & `langchain_experimental-0.0.8/langchain_experimental/pal_chain/base.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.7/langchain_experimental/pal_chain/colored_object_prompt.py` & `langchain_experimental-0.0.8/langchain_experimental/pal_chain/colored_object_prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.7/langchain_experimental/pal_chain/math_prompt.py` & `langchain_experimental-0.0.8/langchain_experimental/pal_chain/math_prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.7/langchain_experimental/plan_and_execute/agent_executor.py` & `langchain_experimental-0.0.8/langchain_experimental/plan_and_execute/agent_executor.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.7/langchain_experimental/plan_and_execute/executors/agent_executor.py` & `langchain_experimental-0.0.8/langchain_experimental/plan_and_execute/executors/agent_executor.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.7/langchain_experimental/plan_and_execute/executors/base.py` & `langchain_experimental-0.0.8/langchain_experimental/plan_and_execute/executors/base.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.7/langchain_experimental/plan_and_execute/planners/base.py` & `langchain_experimental-0.0.8/langchain_experimental/plan_and_execute/planners/base.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.7/langchain_experimental/plan_and_execute/planners/chat_planner.py` & `langchain_experimental-0.0.8/langchain_experimental/plan_and_execute/planners/chat_planner.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.7/langchain_experimental/plan_and_execute/schema.py` & `langchain_experimental-0.0.8/langchain_experimental/plan_and_execute/schema.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.7/langchain_experimental/prompts/load.py` & `langchain_experimental-0.0.8/langchain_experimental/prompts/load.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.7/langchain_experimental/sql/base.py` & `langchain_experimental-0.0.8/langchain_experimental/sql/base.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.7/langchain_experimental/tot/base.py` & `langchain_experimental-0.0.8/langchain_experimental/tot/base.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.7/langchain_experimental/tot/checker.py` & `langchain_experimental-0.0.8/langchain_experimental/tot/checker.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.7/langchain_experimental/tot/controller.py` & `langchain_experimental-0.0.8/langchain_experimental/tot/controller.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.7/langchain_experimental/tot/memory.py` & `langchain_experimental-0.0.8/langchain_experimental/tot/memory.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.7/langchain_experimental/tot/prompts.py` & `langchain_experimental-0.0.8/langchain_experimental/tot/prompts.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.7/langchain_experimental/tot/thought_generation.py` & `langchain_experimental-0.0.8/langchain_experimental/tot/thought_generation.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.7/pyproject.toml` & `langchain_experimental-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchain-experimental"
-version = "0.0.7"
+version = "0.0.8"
 description = "Building applications with LLMs through composability"
 authors = []
 license = "MIT"
 readme = "README.md"
 repository = "https://www.github.com/hwchase17/langchain"
```

### Comparing `langchain_experimental-0.0.7/PKG-INFO` & `langchain_experimental-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-experimental
-Version: 0.0.7
+Version: 0.0.8
 Summary: Building applications with LLMs through composability
 Home-page: https://www.github.com/hwchase17/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

