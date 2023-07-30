# Comparing `tmp/pdx-0.5.1.tar.gz` & `tmp/pdx-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdx-0.5.1.tar", max compression
+gzip compressed data, was "pdx-0.6.0.tar", max compression
```

## Comparing `pdx-0.5.1.tar` & `pdx-0.6.0.tar`

### file list

```diff
@@ -1,47 +1,51 @@
--rw-r--r--   0        0        0    11346 2023-06-17 05:57:05.771799 pdx-0.5.1/LICENSE
--rw-r--r--   0        0        0     1727 2023-07-27 12:59:32.744111 pdx-0.5.1/README.md
--rw-r--r--   0        0        0      832 2023-07-27 12:56:03.111928 pdx-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      249 2023-07-27 11:10:49.057117 pdx-0.5.1/src/pdx/__init__.py
--rw-r--r--   0        0        0     2881 2023-07-27 11:10:49.057347 pdx-0.5.1/src/pdx/agent/__init__.py
--rw-r--r--   0        0        0     1327 2023-07-27 11:10:49.057529 pdx-0.5.1/src/pdx/agent/config.py
--rw-r--r--   0        0        0     1898 2023-07-27 11:10:49.057733 pdx-0.5.1/src/pdx/agent/metadata.py
--rw-r--r--   0        0        0     1947 2023-07-27 11:10:49.057944 pdx-0.5.1/src/pdx/agent/tester.py
--rw-r--r--   0        0        0     1673 2023-07-27 12:55:20.723471 pdx-0.5.1/src/pdx/cli.py
--rw-r--r--   0        0        0        0 2023-06-28 14:39:53.768534 pdx-0.5.1/src/pdx/commands/__init__.py
--rw-r--r--   0        0        0     1317 2023-06-28 15:01:30.272225 pdx-0.5.1/src/pdx/commands/create.py
--rw-r--r--   0        0        0     1043 2023-06-17 06:02:47.694295 pdx-0.5.1/src/pdx/exceptions.py
--rw-r--r--   0        0        0     2172 2023-07-27 11:10:49.058505 pdx-0.5.1/src/pdx/logger.py
--rw-r--r--   0        0        0       93 2023-07-27 11:10:49.058639 pdx-0.5.1/src/pdx/metadata.py
--rw-r--r--   0        0        0        0 2023-07-27 11:10:49.058730 pdx-0.5.1/src/pdx/models/__init__.py
--rw-r--r--   0        0        0       59 2023-07-27 11:10:49.058958 pdx-0.5.1/src/pdx/models/anthropic/__init__.py
--rw-r--r--   0        0        0     3860 2023-07-27 11:10:49.059167 pdx-0.5.1/src/pdx/models/anthropic/client.py
--rw-r--r--   0        0        0     4400 2023-07-27 11:10:49.059316 pdx-0.5.1/src/pdx/models/anthropic/completion.py
--rw-r--r--   0        0        0       57 2023-06-17 06:00:09.710685 pdx-0.5.1/src/pdx/models/anthropic/constants.py
--rw-r--r--   0        0        0     1698 2023-06-17 06:01:13.890539 pdx-0.5.1/src/pdx/models/anthropic/exceptions.py
--rw-r--r--   0        0        0     3543 2023-06-17 06:01:20.740652 pdx-0.5.1/src/pdx/models/api_client.py
--rw-r--r--   0        0        0     2171 2023-07-27 11:10:49.059612 pdx-0.5.1/src/pdx/models/config.py
--rw-r--r--   0        0        0      462 2023-07-27 11:10:49.059806 pdx-0.5.1/src/pdx/models/metadata.py
--rw-r--r--   0        0        0     3764 2023-07-27 11:10:49.059941 pdx-0.5.1/src/pdx/models/model.py
--rw-r--r--   0        0        0       57 2023-07-27 11:10:49.060153 pdx-0.5.1/src/pdx/models/openai/__init__.py
--rw-r--r--   0        0        0     2165 2023-07-27 11:10:49.060479 pdx-0.5.1/src/pdx/models/openai/client.py
--rw-r--r--   0        0        0     5636 2023-07-27 11:10:49.060629 pdx-0.5.1/src/pdx/models/openai/completion.py
--rw-r--r--   0        0        0     1414 2023-06-17 06:01:07.686125 pdx-0.5.1/src/pdx/models/openai/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-17 06:00:09.713048 pdx-0.5.1/src/pdx/models/utils.py
--rw-r--r--   0        0        0     2413 2023-07-27 11:10:49.060795 pdx-0.5.1/src/pdx/prompt/__init__.py
--rw-r--r--   0        0        0     3081 2023-07-27 11:10:49.060934 pdx-0.5.1/src/pdx/prompt/config.py
--rw-r--r--   0        0        0     1244 2023-07-27 11:10:49.061217 pdx-0.5.1/src/pdx/prompt/prompt_chain.py
--rw-r--r--   0        0        0     1779 2023-07-27 11:10:49.061341 pdx-0.5.1/src/pdx/prompt/prompt_session.py
--rw-r--r--   0        0        0     2727 2023-07-27 11:10:49.061477 pdx-0.5.1/src/pdx/prompt/prompt_template.py
--rw-r--r--   0        0        0     5210 2023-07-27 11:10:49.061629 pdx-0.5.1/src/pdx/prompt/prompt_tree.py
--rw-r--r--   0        0        0      142 2023-07-27 12:57:35.646254 pdx-0.5.1/src/pdx/settings.py
--rw-r--r--   0        0        0       54 2023-06-28 14:16:27.138776 pdx-0.5.1/src/pdx/templates/__init__.py
--rw-r--r--   0        0        0        0 2023-06-28 14:38:23.123005 pdx-0.5.1/src/pdx/templates/simple/Readme.md
--rw-r--r--   0        0        0      405 2023-06-28 14:33:23.114668 pdx-0.5.1/src/pdx/templates/simple/__init__.py
--rw-r--r--   0        0        0      192 2023-06-28 14:54:47.892150 pdx-0.5.1/src/pdx/templates/simple/templates/1_prompt.defaults.yaml
--rw-r--r--   0        0        0      159 2023-06-28 14:27:03.141095 pdx-0.5.1/src/pdx/templates/simple/templates/1_prompt.jinja
--rw-r--r--   0        0        0      191 2023-06-28 14:54:26.649501 pdx-0.5.1/src/pdx/templates/simple/tests/test_1.yaml
--rw-r--r--   0        0        0        0 2023-06-17 06:00:09.713573 pdx-0.5.1/src/pdx/utils/__init__.py
--rw-r--r--   0        0        0      595 2023-06-17 06:00:09.714358 pdx-0.5.1/src/pdx/utils/rw.py
--rw-r--r--   0        0        0     2051 2023-07-27 11:10:49.062145 pdx-0.5.1/src/pdx/worker/__init__.py
--rw-r--r--   0        0        0     1905 2023-07-27 11:10:49.062500 pdx-0.5.1/src/pdx/worker/metadata.py
--rw-r--r--   0        0        0     2799 1970-01-01 00:00:00.000000 pdx-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0    11346 2023-06-17 05:57:05.771799 pdx-0.6.0/LICENSE
+-rw-r--r--   0        0        0     1727 2023-07-27 12:59:32.744111 pdx-0.6.0/README.md
+-rw-r--r--   0        0        0      831 2023-07-30 15:55:42.728662 pdx-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      249 2023-07-27 11:10:49.057117 pdx-0.6.0/src/pdx/__init__.py
+-rw-r--r--   0        0        0     3060 2023-07-29 16:39:10.239255 pdx-0.6.0/src/pdx/agent/__init__.py
+-rw-r--r--   0        0        0     1327 2023-07-27 11:10:49.057529 pdx-0.6.0/src/pdx/agent/config.py
+-rw-r--r--   0        0        0     1999 2023-07-29 16:39:10.239382 pdx-0.6.0/src/pdx/agent/metadata.py
+-rw-r--r--   0        0        0     1947 2023-07-27 11:10:49.057944 pdx-0.6.0/src/pdx/agent/tester.py
+-rw-r--r--   0        0        0     1949 2023-07-29 16:39:10.239496 pdx-0.6.0/src/pdx/cache/__init__.py
+-rw-r--r--   0        0        0      615 2023-07-29 16:39:10.239587 pdx-0.6.0/src/pdx/cache/cache.py
+-rw-r--r--   0        0        0     1037 2023-07-29 16:39:10.239680 pdx-0.6.0/src/pdx/cache/in_memory_cache.py
+-rw-r--r--   0        0        0      297 2023-07-29 16:39:10.239791 pdx-0.6.0/src/pdx/cache/utils.py
+-rw-r--r--   0        0        0     1673 2023-07-27 12:55:20.723471 pdx-0.6.0/src/pdx/cli.py
+-rw-r--r--   0        0        0        0 2023-06-28 14:39:53.768534 pdx-0.6.0/src/pdx/commands/__init__.py
+-rw-r--r--   0        0        0     1317 2023-06-28 15:01:30.272225 pdx-0.6.0/src/pdx/commands/create.py
+-rw-r--r--   0        0        0     1043 2023-06-17 06:02:47.694295 pdx-0.6.0/src/pdx/exceptions.py
+-rw-r--r--   0        0        0     2172 2023-07-27 11:10:49.058505 pdx-0.6.0/src/pdx/logger.py
+-rw-r--r--   0        0        0       90 2023-07-30 15:55:53.185728 pdx-0.6.0/src/pdx/metadata.py
+-rw-r--r--   0        0        0        0 2023-07-27 11:10:49.058730 pdx-0.6.0/src/pdx/models/__init__.py
+-rw-r--r--   0        0        0       59 2023-07-27 11:10:49.058958 pdx-0.6.0/src/pdx/models/anthropic/__init__.py
+-rw-r--r--   0        0        0     3860 2023-07-27 11:10:49.059167 pdx-0.6.0/src/pdx/models/anthropic/client.py
+-rw-r--r--   0        0        0     2751 2023-07-29 16:39:10.240085 pdx-0.6.0/src/pdx/models/anthropic/completion.py
+-rw-r--r--   0        0        0       57 2023-06-17 06:00:09.710685 pdx-0.6.0/src/pdx/models/anthropic/constants.py
+-rw-r--r--   0        0        0     1698 2023-06-17 06:01:13.890539 pdx-0.6.0/src/pdx/models/anthropic/exceptions.py
+-rw-r--r--   0        0        0     3543 2023-06-17 06:01:20.740652 pdx-0.6.0/src/pdx/models/api_client.py
+-rw-r--r--   0        0        0     2090 2023-07-29 16:39:10.240255 pdx-0.6.0/src/pdx/models/config.py
+-rw-r--r--   0        0        0      766 2023-07-29 16:39:10.240384 pdx-0.6.0/src/pdx/models/metadata.py
+-rw-r--r--   0        0        0     3764 2023-07-27 11:10:49.059941 pdx-0.6.0/src/pdx/models/model.py
+-rw-r--r--   0        0        0       57 2023-07-27 11:10:49.060153 pdx-0.6.0/src/pdx/models/openai/__init__.py
+-rw-r--r--   0        0        0     2165 2023-07-27 11:10:49.060479 pdx-0.6.0/src/pdx/models/openai/client.py
+-rw-r--r--   0        0        0     3988 2023-07-29 16:39:10.240529 pdx-0.6.0/src/pdx/models/openai/completion.py
+-rw-r--r--   0        0        0     1414 2023-06-17 06:01:07.686125 pdx-0.6.0/src/pdx/models/openai/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-17 06:00:09.713048 pdx-0.6.0/src/pdx/models/utils.py
+-rw-r--r--   0        0        0     2205 2023-07-29 16:39:10.240666 pdx-0.6.0/src/pdx/prompt/__init__.py
+-rw-r--r--   0        0        0     3081 2023-07-27 11:10:49.060934 pdx-0.6.0/src/pdx/prompt/config.py
+-rw-r--r--   0        0        0     1537 2023-07-29 16:39:10.240787 pdx-0.6.0/src/pdx/prompt/prompt_chain.py
+-rw-r--r--   0        0        0     1703 2023-07-29 16:39:10.240918 pdx-0.6.0/src/pdx/prompt/prompt_session.py
+-rw-r--r--   0        0        0     2727 2023-07-27 11:10:49.061477 pdx-0.6.0/src/pdx/prompt/prompt_template.py
+-rw-r--r--   0        0        0     5210 2023-07-27 11:10:49.061629 pdx-0.6.0/src/pdx/prompt/prompt_tree.py
+-rw-r--r--   0        0        0      128 2023-07-29 16:39:10.241044 pdx-0.6.0/src/pdx/settings.py
+-rw-r--r--   0        0        0       54 2023-06-28 14:16:27.138776 pdx-0.6.0/src/pdx/templates/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-28 14:38:23.123005 pdx-0.6.0/src/pdx/templates/simple/Readme.md
+-rw-r--r--   0        0        0      405 2023-06-28 14:33:23.114668 pdx-0.6.0/src/pdx/templates/simple/__init__.py
+-rw-r--r--   0        0        0      192 2023-06-28 14:54:47.892150 pdx-0.6.0/src/pdx/templates/simple/templates/1_prompt.defaults.yaml
+-rw-r--r--   0        0        0      159 2023-06-28 14:27:03.141095 pdx-0.6.0/src/pdx/templates/simple/templates/1_prompt.jinja
+-rw-r--r--   0        0        0      191 2023-06-28 14:54:26.649501 pdx-0.6.0/src/pdx/templates/simple/tests/test_1.yaml
+-rw-r--r--   0        0        0        0 2023-06-17 06:00:09.713573 pdx-0.6.0/src/pdx/utils/__init__.py
+-rw-r--r--   0        0        0      595 2023-06-17 06:00:09.714358 pdx-0.6.0/src/pdx/utils/rw.py
+-rw-r--r--   0        0        0     2051 2023-07-27 11:10:49.062145 pdx-0.6.0/src/pdx/worker/__init__.py
+-rw-r--r--   0        0        0     1905 2023-07-27 11:10:49.062500 pdx-0.6.0/src/pdx/worker/metadata.py
+-rw-r--r--   0        0        0     2798 1970-01-01 00:00:00.000000 pdx-0.6.0/PKG-INFO
```

### Comparing `pdx-0.5.1/LICENSE` & `pdx-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pdx-0.5.1/README.md` & `pdx-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pdx-0.5.1/pyproject.toml` & `pdx-0.6.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pdx"
-version = "0.5.1"
+version = "0.6.0"
 description = "Prompt Engineering and Dev-Ops toolkits. A faster way to build and manage applications powered by Language Models."
 keywords = ["prompt", "LLM", "prompt engineering", "dev-ops", "observability", "apps"]
 authors = ["Adithya Krishnan <krishsandeep@gmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 packages = [{include = "pdx", from = "src"}]
 
@@ -13,15 +13,15 @@
 
 [tool.poetry.dependencies]
 python = ">=3.7"
 click = "^8.1.3"
 jinja2 = "^3.1.2"
 pyyaml = "^6.0"
 jsonschema = "^4.17.3"
-pydantic = "^1.10.9"
+pydantic = "^2.1.1"
 regex = "^2023.6.3"
 aiohttp = "^3.8.4"
 requests = "^2.31.0"
 
 
 [tool.poetry.group.dev.dependencies]
 autopep8 = "^2.0.2"
```

### Comparing `pdx-0.5.1/src/pdx/agent/__init__.py` & `pdx-0.6.0/src/pdx/agent/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,19 +3,21 @@
 from pdx.agent.config import AgentConfig
 from pdx.prompt import Prompt
 from pdx.models.model import Model
 from pdx.prompt.prompt_chain import PromptChain
 from pdx.prompt.prompt_tree import PromptTree
 from pdx.prompt.prompt_session import PromptSession
 from pdx.models.metadata import ModelResponse
-from pdx.agent.metadata import AgentID, RequestMetadata, AgentResponse, AgentResponseMetadata
+from pdx.agent.metadata import AgentID, RequestMetadata, AgentResponse, AgentResponseMetadata, AgentRequest
+from pdx.cache.cache import Cache
+from pdx.cache import agent_cache, aagent_cache
 
 
 class Agent(object):
-    def __init__(self, path: str = None, prompt: Union[Prompt, PromptChain, PromptTree] = None, model: Model = None):
+    def __init__(self, path: str = None, prompt: Union[Prompt, PromptChain, PromptTree] = None, model: Model = None, cache: Cache = None):
         if path is not None:
             self._type = 'config'
             self._config: AgentConfig = AgentConfig(path)
             self._agent_id = AgentID(agent_name=self._config.name)
             if prompt is None:
                 self._prompt: PromptTree = PromptTree(
                     self._config.prompt_config)
@@ -29,15 +31,17 @@
         else:
             if prompt is None and model is None:
                 raise ValueError(
                     'Provide `Prompt` and `Model` if not providing Agent config path.')
             self._type = 'prompt-model'
             self._prompt = prompt
             self._model = model
-            self._agent_id = AgentID(agent_name='agent')
+            self._agent_id = AgentID()
+
+        self._cache = cache
 
     def _postprocess(self, response: ModelResponse, request: dict, prompt_session: PromptSession) -> AgentResponse:
         request_metadata = RequestMetadata(
             agent_id=self._agent_id,
             request_id=uuid4(),
             request_values=request,
             request_params=response.request_params,
@@ -49,22 +53,24 @@
         )
         agent_response = AgentResponse(
             data=response.data,
             metadata=metadata
         )
         return agent_response
 
-    async def aexecute(self, request: dict = {}, metadata: dict = {}):
+    @aagent_cache
+    async def aexecute(self, request: AgentRequest = {}, metadata: dict = {}):
         _prompt_session = self._prompt.execute(request)
         _model_response = await self._model.aexecute(_prompt_session)
         _agent_response = self._postprocess(
             _model_response, request, _prompt_session)
         _agent_response.metadata.add_custom(metadata=metadata)
         return _agent_response
 
-    def execute(self, request: dict = {}, metadata: dict = {}):
+    @agent_cache
+    def execute(self, request: AgentRequest = {}, metadata: dict = {}):
         _prompt_session = self._prompt.execute(request)
         _model_response = self._model.execute(_prompt_session)
         _agent_response = self._postprocess(
             _model_response, request, _prompt_session)
         _agent_response.metadata.add_custom(metadata=metadata)
         return _agent_response
```

### Comparing `pdx-0.5.1/src/pdx/agent/config.py` & `pdx-0.6.0/src/pdx/agent/config.py`

 * *Files identical despite different names*

### Comparing `pdx-0.5.1/src/pdx/agent/metadata.py` & `pdx-0.6.0/src/pdx/worker/metadata.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from dataclasses import dataclass, field
 from pdx.metadata import PDXMetadata
 from pdx.models.metadata import ResponseMetadata
 from pdx.logger import logger
 
 
 @dataclass
-class AgentID:
-    agent_name: str
+class WorkerID:
+    worker_name: str
     git_hash: str = None
     git_branch: str = None
 
     def __post_init__(self):
         if self.git_hash is None and self.git_branch is None:
             try:
                 subprocess.check_output(
@@ -28,37 +28,37 @@
                     'It is recommended to run `pdx` from a initialized git repository.', event='warning')
                 self.git_hash = 'not-git-repo'
                 self.git_branch = 'not-git-repo'
 
 
 @dataclass
 class RequestMetadata:
-    agent_id: AgentID
+    worker_id: WorkerID
     request_id: uuid.UUID = None
     request_values: dict = None
     request_params: dict = None
     prompt: list = None
 
     def __post_init__(self):
         if self.request_id is None:
             self.request_id = uuid.uuid4()
 
 
 @dataclass
-class AgentResponseMetadata:
+class WorkerResponseMetadata:
     request: RequestMetadata
     response: ResponseMetadata
     custom: dict = None
     pdx: PDXMetadata = None
 
     def __post_init__(self):
         if self.pdx is None:
             self.pdx = PDXMetadata()
 
     def add_custom(self, metadata: dict):
         self.custom = metadata
 
 
 @dataclass
-class AgentResponse:
+class WorkerResponse:
     data: str
-    metadata: AgentResponseMetadata
+    metadata: WorkerResponseMetadata
```

### Comparing `pdx-0.5.1/src/pdx/agent/tester.py` & `pdx-0.6.0/src/pdx/agent/tester.py`

 * *Files identical despite different names*

### Comparing `pdx-0.5.1/src/pdx/cli.py` & `pdx-0.6.0/src/pdx/cli.py`

 * *Files identical despite different names*

### Comparing `pdx-0.5.1/src/pdx/commands/create.py` & `pdx-0.6.0/src/pdx/commands/create.py`

 * *Files identical despite different names*

### Comparing `pdx-0.5.1/src/pdx/exceptions.py` & `pdx-0.6.0/src/pdx/exceptions.py`

 * *Files identical despite different names*

### Comparing `pdx-0.5.1/src/pdx/logger.py` & `pdx-0.6.0/src/pdx/logger.py`

 * *Files identical despite different names*

### Comparing `pdx-0.5.1/src/pdx/models/anthropic/client.py` & `pdx-0.6.0/src/pdx/models/anthropic/client.py`

 * *Files identical despite different names*

### Comparing `pdx-0.5.1/src/pdx/models/anthropic/completion.py` & `pdx-0.6.0/src/pdx/models/model.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,82 +1,68 @@
 from time import time
 from pdx.logger import logger
-from pdx.models.model import Model
 from pdx.prompt.prompt_session import PromptSession
-from pdx.models.anthropic.client import AnthropicClient
-import pdx.models.anthropic.constants as constants
-from pdx.models.anthropic.exceptions import handle_anthropic_prompt_validation
+from pdx.models.api_client import APIClient
 from pdx.models.metadata import ModelResponse, ResponseMetadata, ModelTokenUsage
 
 
-class CompletionModel(object):
+class Model:
     def __init__(self,
                  api_key: str,
                  model: str,
                  max_tokens: int = 1200,
                  stop: list = ["#", "---"],
                  temperature: float = 0,
-                 **kwargs,
+                 **kwargs
                  ):
 
-        self._api_url = "v1/complete"
-
-        self._provider = "anthropic"
-        self._client = AnthropicClient(api_key)
+        self._client = APIClient(api_key)
+        self._provider = "model_provider"
         self._model = model
-        self._max_tokens_to_sample = max_tokens
-        self._stop_sequences = stop
+        self._max_tokens = max_tokens
+        self._stop = stop
         self._temperature = temperature
-        self._top_p = kwargs.get('top_p', -1)
-        self._top_k = kwargs.get('top_k', -1)
         self._retries = kwargs.get('retries', 2)
 
-    def _preprocess(self, prompt: PromptSession):
-        if prompt.session_type == "chat":
-            _prompt = prompt.text_prompt({
-                'user': constants.HUMAN_PROMPT,
-                'assistant': constants.AI_PROMPT,
-                'system': constants.HUMAN_PROMPT,
-            })
-        else:
-            _content = prompt.text_prompt({})
-            _prompt = f"{constants.HUMAN_PROMPT} {_content}{constants.AI_PROMPT}"
+        self._api_url = "v1/completions"
 
-        handle_anthropic_prompt_validation(_prompt)
+    def _preprocess(self, prompt: PromptSession) -> dict:
         request_params = {
-            'prompt': _prompt,
-            'stop_sequences': self._stop_sequences,
-            'model': self._model,
-            'max_tokens_to_sample': self._max_tokens_to_sample,
-            'temperature': self._temperature,
-            'top_p': self._top_p,
-            'top_k': self._top_k,
+            "model": self._model,
+            "max_tokens": self._max_tokens,
+            "temperature": self._temperature,
+            "stop": self._stop
         }
 
+        _prompt = prompt.text_prompt({})
+
+        request_params['prompt'] = _prompt
+
         return request_params
 
-    def _postprocess(self, response: dict, request_params: dict, request_time) -> ModelResponse:
-        params = {key: value for key,
-                  value in request_params.items() if key != 'prompt'}
+    def _postprocess(self, response: dict, request_params: dict, request_time: float) -> ModelResponse:
         token_usage = ModelTokenUsage(
-            response=None,
-            prompt=None,
-            total=None)
+            response=response['usage']['completion_tokens'],
+            prompt=response['usage']['prompt_tokens'],
+            total=response['usage']['total_tokens']
+        )
         response_metadata = ResponseMetadata(
             model=response['model'],
-            api_log_id=response['log_id'],
-            stop=response['stop'],
-            stop_reason=response['stop'],
+            api_log_id=response['id'],
+            stop=response['choices'][0]['finish_reason'],
+            stop_reason=response['choices'][0]['finish_reason'],
             token_usage=token_usage,
             latency=request_time)
+
+        params = {key: value for key,
+                  value in request_params.items() if key != 'prompt'}
         model_response = ModelResponse(
             metadata=response_metadata,
             request_params=params,
-            data=response['completion'])
-
+            data=response['choices'][0]['text'])
         return model_response
 
     def execute(self, prompt: PromptSession) -> ModelResponse:
         start_time = time()
         request_params = self._preprocess(prompt)
 
         _try_count = 0
```

### Comparing `pdx-0.5.1/src/pdx/models/anthropic/exceptions.py` & `pdx-0.6.0/src/pdx/models/anthropic/exceptions.py`

 * *Files identical despite different names*

### Comparing `pdx-0.5.1/src/pdx/models/api_client.py` & `pdx-0.6.0/src/pdx/models/api_client.py`

 * *Files identical despite different names*

### Comparing `pdx-0.5.1/src/pdx/models/config.py` & `pdx-0.6.0/src/pdx/models/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,26 @@
-from pydantic import BaseSettings
-from dataclasses import dataclass, field
+import os
+from typing import Optional
+from pydantic import BaseModel, Field
 
 # Available LLM completion models
 OPENAI_COMPLETION_MODELS = ["text-davinci-003", "gpt-3.5-turbo", "gpt-4"]
 ANTHROPIC_COMPLETION_MODELS = ["claude-v1", "claude-v1-100k", "claude-instant-v1", "claude-instant-v1-100k",
                                "claude-v1.3", "claude-v1.3-100k", "claude-v1.2" "claude-v1.0", "claude-instant-v1.1",
                                "claude-instant-v1.1-100k", "claude-instant-v1.0"]
 
 
-class Keys(BaseSettings):
-    openai_key: str = None
-    anthropic_key: str = None
-    cohere_key: str = None
-
-
-@dataclass
-class ModelConfig:
+class ModelConfig(BaseModel):
     id: str
-    params: dict = field(default_factory=dict)
-    name: str = field(init=False)
-    provider: str = field(init=False)
-    api_key: str = field(init=False)
+    params: dict = Field(default_factory=dict)
+    name: Optional[str] = Field(default=None)
+    provider: Optional[str] = Field(default=None)
+    api_key: Optional[str] = Field(default=None)
 
-    def __post_init__(self):
+    def model_post_init(self, *args, **kwargs) -> None:
         self.name = self.id
 
         if self.id in [*OPENAI_COMPLETION_MODELS]:
             api_key_id = 'openai_key'
             self.provider = 'openai'
         elif self.id in [*ANTHROPIC_COMPLETION_MODELS]:
             api_key_id = 'anthropic_key'
@@ -34,20 +28,19 @@
         else:
             raise ValueError(f"Model: {self.id} not supported")
 
         self.api_key = self._get_api_key(api_key_id)
 
     @staticmethod
     def _get_api_key(api_key_id: str):
-        _keys = Keys()
-        _api_key = _keys.__dict__.get(api_key_id, None)
+        _api_key = os.environ[api_key_id.upper()]
 
         if _api_key is None:
             raise ValueError(
-                f"{api_key_id.capitalize()} API key not found. Make sure it is present as a environment variable.")
+                f"{api_key_id.upper()} API key not found. Make sure it is present as an environment variable.")
 
         return _api_key
 
     def build_model(self):
         if self.id in [*OPENAI_COMPLETION_MODELS]:
             from pdx.models.openai import CompletionModel as OpenAICompletionModel
             return OpenAICompletionModel(model=self.id, api_key=self.api_key, **self.params)
```

### Comparing `pdx-0.5.1/src/pdx/models/model.py` & `pdx-0.6.0/src/pdx/models/openai/completion.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,106 +1,99 @@
 from time import time
 from pdx.logger import logger
+from pdx.models.model import Model
 from pdx.prompt.prompt_session import PromptSession
-from pdx.models.api_client import APIClient
+from pdx.models.openai.client import OpenAIClient
 from pdx.models.metadata import ModelResponse, ResponseMetadata, ModelTokenUsage
 
 
-class Model:
+class CompletionModel(Model):
     def __init__(self,
                  api_key: str,
                  model: str,
                  max_tokens: int = 1200,
                  stop: list = ["#", "---"],
                  temperature: float = 0,
-                 **kwargs
+                 **kwargs,
                  ):
+        if model in ["gpt-3.5-turbo", "gpt-4"]:
+            self._client_type = "chat"
+        elif model in ["text-davinci-003", "text-davinci-002", "davinci", "curie", "babbage", "ada"]:
+            self._client_type = "text"
+        else:
+            raise Exception("Model not supported")
+
+        if self._client_type == "chat":
+            self._api_url = "v1/chat/completions"
+        else:  # self._client_type == "text"
+            self._api_url = "v1/completions"
 
-        self._client = APIClient(api_key)
-        self._provider = "model_provider"
+        self._provider = "openai"
+        self._client = OpenAIClient(api_key)
         self._model = model
         self._max_tokens = max_tokens
         self._stop = stop
         self._temperature = temperature
+        self._top_p = kwargs.get('top_p', 1)
+        self._best_of = kwargs.get('best_of', 1)
+        self._frequency_penalty = kwargs.get('frequency_penalty', 0)
+        self._presence_penalty = kwargs.get('presence_penalty', 0)
         self._retries = kwargs.get('retries', 2)
 
-        self._api_url = "v1/completions"
-
     def _preprocess(self, prompt: PromptSession) -> dict:
         request_params = {
             "model": self._model,
             "max_tokens": self._max_tokens,
             "temperature": self._temperature,
+            "top_p": self._top_p,
+            "frequency_penalty": self._frequency_penalty,
+            "presence_penalty": self._presence_penalty,
             "stop": self._stop
         }
-
-        _prompt = prompt.text_prompt({})
-
-        request_params['prompt'] = _prompt
+        if self._client_type == "chat":
+            if prompt.session_type == "text":
+                _content = prompt.text_prompt({})
+                _chat_prompt = [{"role": "user", "content": _content}]
+            else:
+                _chat_prompt = prompt.chat_prompt()
+            request_params['messages'] = _chat_prompt
+
+        if self._client_type == "text":
+            if prompt.session_type == "chat":
+                _text_prompt = prompt.text_prompt()
+            else:
+                _text_prompt = prompt.text_prompt({})
+            request_params['prompt'] = _text_prompt
+            request_params['best_of'] = self._best_of
 
         return request_params
 
     def _postprocess(self, response: dict, request_params: dict, request_time: float) -> ModelResponse:
         token_usage = ModelTokenUsage(
             response=response['usage']['completion_tokens'],
             prompt=response['usage']['prompt_tokens'],
-            total=response['usage']['total_tokens']
-        )
+            total=response['usage']['total_tokens'])
         response_metadata = ResponseMetadata(
             model=response['model'],
             api_log_id=response['id'],
             stop=response['choices'][0]['finish_reason'],
             stop_reason=response['choices'][0]['finish_reason'],
             token_usage=token_usage,
             latency=request_time)
 
-        params = {key: value for key,
-                  value in request_params.items() if key != 'prompt'}
-        model_response = ModelResponse(
-            metadata=response_metadata,
-            request_params=params,
-            data=response['choices'][0]['text'])
-        return model_response
-
-    def execute(self, prompt: PromptSession) -> ModelResponse:
-        start_time = time()
-        request_params = self._preprocess(prompt)
-
-        _try_count = 0
-        while (_try_count <= self._retries):
-            try:
-                _r = self._client.request(
-                    "post",
-                    self._api_url,
-                    params=request_params,
-                )
-                request_time = time() - start_time
-                return self._postprocess(_r, request_params, request_time)
-            except Exception as e:
-                logger.verbose(
-                    f"{self._provider} {self._model} model failed to run.\nReason: {e}")
-                _try_count += 1
-
-        raise ValueError(
-            f"{self._provider} {self._model} model failed to run successfully.")
-
-    async def aexecute(self, prompt: PromptSession) -> ModelResponse:
-        start_time = time()
-        request_params = self._preprocess(prompt)
-
-        _try_count = 0
-        while (_try_count <= self._retries):
-            try:
-                _r = await self._client.arequest(
-                    "post",
-                    self._api_url,
-                    params=request_params,
-                )
-                request_time = time() - start_time
-                return self._postprocess(_r, request_params, request_time)
-            except Exception as e:
-                logger.verbose(
-                    f"{self._provider} {self._model} model failed to run.\nReason: {e}")
-                _try_count += 1
-
-        raise ValueError(
-            f"{self._provider} {self._model} model failed to run successfully.")
+        if self._client_type == "chat":
+            params = {key: value for key,
+                      value in request_params.items() if key != 'messages'}
+            model_response = ModelResponse(
+                metadata=response_metadata,
+                request_params=params,
+                data=response['choices'][0]['message']['content'])
+            return model_response
+
+        if self._client_type == "text":
+            params = {key: value for key,
+                      value in request_params.items() if key != 'prompt'}
+            model_response = ModelResponse(
+                metadata=response_metadata,
+                request_params=params,
+                data=response['choices'][0]['text'])
+            return model_response
```

### Comparing `pdx-0.5.1/src/pdx/models/openai/client.py` & `pdx-0.6.0/src/pdx/models/openai/client.py`

 * *Files identical despite different names*

### Comparing `pdx-0.5.1/src/pdx/models/openai/exceptions.py` & `pdx-0.6.0/src/pdx/models/openai/exceptions.py`

 * *Files identical despite different names*

### Comparing `pdx-0.5.1/src/pdx/prompt/__init__.py` & `pdx-0.6.0/src/pdx/prompt/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,22 +16,18 @@
 
         if content != None:
             self._prompt = content
             self.pointer = pointer
         elif template != None:
             self._prompt = PromptTemplate(
                 template_string=template, name=pointer)
-            if pointer == None:
-                raise Exception('Prompt template must have a pointer.')
             self.pointer = pointer
         elif template_path != None:
             self._prompt = PromptTemplate(
                 template_path=template_path, name=pointer)
-            if pointer == None:
-                raise Exception('Prompt template must have a pointer.')
             self.pointer = pointer
 
         self.role = role
 
     def execute(self, values: dict = {}, _output_item=False, prompt_session: PromptSession = None) -> Union[PromptSession, PromptSessionItem]:
         _prompt_content = ''
         if isinstance(self._prompt, str):
```

### Comparing `pdx-0.5.1/src/pdx/prompt/config.py` & `pdx-0.6.0/src/pdx/prompt/config.py`

 * *Files identical despite different names*

### Comparing `pdx-0.5.1/src/pdx/prompt/prompt_chain.py` & `pdx-0.6.0/src/pdx/prompt/prompt_chain.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 from typing import List
 from pdx.prompt import Prompt
 from pdx.prompt.prompt_session import PromptSession, PromptSessionItem
 
 
 class PromptChain:
     def __init__(self, prompts: List[Prompt] = None):
+        for _prompt in prompts:
+            if _prompt.pointer == None:
+                raise ValueError(
+                    'Prompt Pointer missing.'
+                    'PromptChain must be initialized with a list of Prompt objects that have a unique `pointer` property.'
+                )
         self._chain = prompts
 
     def execute(self, values: dict = {}):
         _session_type = None
         _prompt_session = PromptSession()
         for _prompt in self._chain:
             prompt_pointer_request = values.get(_prompt.pointer, {})
```

### Comparing `pdx-0.5.1/src/pdx/prompt/prompt_session.py` & `pdx-0.6.0/src/pdx/prompt/prompt_session.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,15 @@
-from dataclasses import dataclass
-from typing import List, Union, Dict
-# from pdx.prompt import Prompt
-# from pdx.prompt.prompt_chain import PromptChain
-# from pdx.prompt.prompt_tree import PromptTree
+from typing import List, Union, Dict, Optional
+from pydantic import BaseModel, Field
 
 
-@dataclass
-class PromptSessionItem:
+class PromptSessionItem(BaseModel):
     content: str
-    content_type: str = 'text'
-    role: str = None
+    content_type: str = Field(default='text')
+    role: Optional[str] = Field(default=None)
 
 
 class PromptSession:
     def __init__(self):
         self.items: List[PromptSessionItem] = []
         self.session_type = 'text'  # text, chat
```

### Comparing `pdx-0.5.1/src/pdx/prompt/prompt_template.py` & `pdx-0.6.0/src/pdx/prompt/prompt_template.py`

 * *Files identical despite different names*

### Comparing `pdx-0.5.1/src/pdx/prompt/prompt_tree.py` & `pdx-0.6.0/src/pdx/prompt/prompt_tree.py`

 * *Files identical despite different names*

### Comparing `pdx-0.5.1/src/pdx/utils/rw.py` & `pdx-0.6.0/src/pdx/utils/rw.py`

 * *Files identical despite different names*

### Comparing `pdx-0.5.1/src/pdx/worker/__init__.py` & `pdx-0.6.0/src/pdx/worker/__init__.py`

 * *Files identical despite different names*

### Comparing `pdx-0.5.1/PKG-INFO` & `pdx-0.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdx
-Version: 0.5.1
+Version: 0.6.0
 Summary: Prompt Engineering and Dev-Ops toolkits. A faster way to build and manage applications powered by Language Models.
 License: Apache-2.0
 Keywords: prompt,LLM,prompt engineering,dev-ops,observability,apps
 Author: Adithya Krishnan
 Author-email: krishsandeep@gmail.com
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: Apache Software License
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: jsonschema (>=4.17.3,<5.0.0)
-Requires-Dist: pydantic (>=1.10.9,<2.0.0)
+Requires-Dist: pydantic (>=2.1.1,<3.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: regex (>=2023.6.3,<2024.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 <img src="./assets/pdx.png" height="40">
```

