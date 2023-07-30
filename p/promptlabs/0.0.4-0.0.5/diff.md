# Comparing `tmp/promptlabs-0.0.4.tar.gz` & `tmp/promptlabs-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptlabs-0.0.4.tar", last modified: Thu Jul 27 08:52:30 2023, max compression
+gzip compressed data, was "promptlabs-0.0.5.tar", last modified: Sun Jul 30 08:45:32 2023, max compression
```

## Comparing `promptlabs-0.0.4.tar` & `promptlabs-0.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 engineer_a  (1000) engineer_a  (1000)        0 2023-07-27 08:52:30.069518 promptlabs-0.0.4/
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)        0 2023-07-24 04:54:11.000000 promptlabs-0.0.4/LICENSE
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)      264 2023-07-27 08:52:30.065518 promptlabs-0.0.4/PKG-INFO
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)        0 2023-07-24 04:54:11.000000 promptlabs-0.0.4/README.md
-drwxrwxr-x   0 engineer_a  (1000) engineer_a  (1000)        0 2023-07-27 08:52:30.065518 promptlabs-0.0.4/promptlabs/
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)       75 2023-07-27 08:51:57.000000 promptlabs-0.0.4/promptlabs/__init__.py
-drwxrwxr-x   0 engineer_a  (1000) engineer_a  (1000)        0 2023-07-27 08:52:30.065518 promptlabs-0.0.4/promptlabs/chain/
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)      184 2023-07-27 05:23:57.000000 promptlabs-0.0.4/promptlabs/chain/__init__.py
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)     1816 2023-07-27 05:28:35.000000 promptlabs-0.0.4/promptlabs/chain/base_chain.py
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)     4455 2023-07-27 08:50:31.000000 promptlabs-0.0.4/promptlabs/chain/function_chain.py
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)     9908 2023-07-27 08:45:47.000000 promptlabs-0.0.4/promptlabs/chain/llm_chain.py
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)     2199 2023-07-27 05:36:18.000000 promptlabs-0.0.4/promptlabs/client.py
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)     5401 2023-07-27 05:21:53.000000 promptlabs-0.0.4/promptlabs/pipeline.py
-drwxrwxr-x   0 engineer_a  (1000) engineer_a  (1000)        0 2023-07-27 08:52:30.065518 promptlabs-0.0.4/promptlabs/scheme/
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)     3660 2023-07-26 10:58:35.000000 promptlabs-0.0.4/promptlabs/scheme/llm.py
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)      711 2023-07-26 09:36:55.000000 promptlabs-0.0.4/promptlabs/scheme/template.py
-drwxrwxr-x   0 engineer_a  (1000) engineer_a  (1000)        0 2023-07-27 08:52:30.065518 promptlabs-0.0.4/promptlabs.egg-info/
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)      264 2023-07-27 08:52:30.000000 promptlabs-0.0.4/promptlabs.egg-info/PKG-INFO
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)      442 2023-07-27 08:52:30.000000 promptlabs-0.0.4/promptlabs.egg-info/SOURCES.txt
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)        1 2023-07-27 08:52:30.000000 promptlabs-0.0.4/promptlabs.egg-info/dependency_links.txt
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)       25 2023-07-27 08:52:30.000000 promptlabs-0.0.4/promptlabs.egg-info/requires.txt
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)       11 2023-07-27 08:52:30.000000 promptlabs-0.0.4/promptlabs.egg-info/top_level.txt
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)       38 2023-07-27 08:52:30.069518 promptlabs-0.0.4/setup.cfg
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)      546 2023-07-27 08:51:53.000000 promptlabs-0.0.4/setup.py
+drwxrwxr-x   0 engineer_a  (1000) engineer_a  (1000)        0 2023-07-30 08:45:32.663154 promptlabs-0.0.5/
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)        0 2023-07-24 04:54:11.000000 promptlabs-0.0.5/LICENSE
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)      264 2023-07-30 08:45:32.663154 promptlabs-0.0.5/PKG-INFO
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)        0 2023-07-24 04:54:11.000000 promptlabs-0.0.5/README.md
+drwxrwxr-x   0 engineer_a  (1000) engineer_a  (1000)        0 2023-07-30 08:45:32.663154 promptlabs-0.0.5/promptlabs/
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)       75 2023-07-30 08:44:44.000000 promptlabs-0.0.5/promptlabs/__init__.py
+drwxrwxr-x   0 engineer_a  (1000) engineer_a  (1000)        0 2023-07-30 08:45:32.663154 promptlabs-0.0.5/promptlabs/chain/
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)      184 2023-07-27 05:23:57.000000 promptlabs-0.0.5/promptlabs/chain/__init__.py
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)     1602 2023-07-28 05:55:16.000000 promptlabs-0.0.5/promptlabs/chain/base_chain.py
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)     6269 2023-07-28 06:22:47.000000 promptlabs-0.0.5/promptlabs/chain/function_chain.py
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)    15272 2023-07-30 08:28:43.000000 promptlabs-0.0.5/promptlabs/chain/llm_chain.py
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)     2199 2023-07-27 05:36:18.000000 promptlabs-0.0.5/promptlabs/client.py
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)     8106 2023-07-28 06:23:34.000000 promptlabs-0.0.5/promptlabs/pipeline.py
+drwxrwxr-x   0 engineer_a  (1000) engineer_a  (1000)        0 2023-07-30 08:45:32.663154 promptlabs-0.0.5/promptlabs/scheme/
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)     4403 2023-07-28 01:47:35.000000 promptlabs-0.0.5/promptlabs/scheme/llm.py
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)      711 2023-07-26 09:36:55.000000 promptlabs-0.0.5/promptlabs/scheme/template.py
+drwxrwxr-x   0 engineer_a  (1000) engineer_a  (1000)        0 2023-07-30 08:45:32.663154 promptlabs-0.0.5/promptlabs.egg-info/
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)      264 2023-07-30 08:45:32.000000 promptlabs-0.0.5/promptlabs.egg-info/PKG-INFO
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)      442 2023-07-30 08:45:32.000000 promptlabs-0.0.5/promptlabs.egg-info/SOURCES.txt
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)        1 2023-07-30 08:45:32.000000 promptlabs-0.0.5/promptlabs.egg-info/dependency_links.txt
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)       25 2023-07-30 08:45:32.000000 promptlabs-0.0.5/promptlabs.egg-info/requires.txt
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)       11 2023-07-30 08:45:32.000000 promptlabs-0.0.5/promptlabs.egg-info/top_level.txt
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)       38 2023-07-30 08:45:32.663154 promptlabs-0.0.5/setup.cfg
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)      546 2023-07-30 08:44:45.000000 promptlabs-0.0.5/setup.py
```

### Comparing `promptlabs-0.0.4/promptlabs/chain/base_chain.py` & `promptlabs-0.0.5/promptlabs/chain/base_chain.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,34 +27,25 @@
         if missing_keys:
             raise ValueError(f"Missing some input keys: {missing_keys}")
 
     def _validate_outputs(self, outputs: Dict[str, Any]) -> None:
         missing_keys = set(self.output_keys).difference(outputs)
         if missing_keys:
             raise ValueError(f"Missing some output keys: {missing_keys}")
-        
-    # @abstractmethod
-    # def validate(
-    #     self,
-    #     inputs: Dict[str, Any],
-    #     outputs: Dict[str, Any] = {}
-    # ) -> Dict[str, Any]:
-    #     """Validate the chain."""
-    #     pass
-    
-    # @abstractmethod
-    # def test(
-    #     self,
-    #     inputs: Dict[str, Any],
-    #     outputs: Dict[str, Any] = {}
-    # ) -> Dict[str, Any]:
-    #     """Run the chain."""
-    #     pass
     
     @abstractmethod
     def run(
         self,
         inputs: Dict[str, Any],
         outputs: Dict[str, Any] = {}
     ) -> Tuple[ChainOutput, ChainLog]:
         """Run the chain."""
+        pass
+    
+    @abstractmethod
+    async def arun(
+        self,
+        inputs: Dict[str, Any],
+        outputs: Dict[str, Any] = {}
+    ) -> Tuple[ChainOutput, ChainLog]:
+        """Run the chain."""
         pass
```

### Comparing `promptlabs-0.0.4/promptlabs/client.py` & `promptlabs-0.0.5/promptlabs/client.py`

 * *Files identical despite different names*

### Comparing `promptlabs-0.0.4/promptlabs/pipeline.py` & `promptlabs-0.0.5/promptlabs/pipeline.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,29 +17,32 @@
         raise ValueError(f"Invalid chain type: {chain_config['type']}")
 class Pipeline:
     
     def __init__(self, config : Dict[str, Any]):
         self.config = config
         # add id to each chain_config from chain_id
         for chain_config in self.config["chain_configs"]:
-            print(chain_config)
+            # print(chain_config)
             chain_config['id'] = chain_config['chain_id']
         
         self.chains = [create_chain(chain_config) for chain_config in self.config["chain_configs"]]
     
+    def with_functions(self, inputs: Dict[str, Any]):
+        # TODO: add functions and llms into each chains. Input style is not decided yet
+        pass
+    
     @property
     def input_keys(self) -> List[str]:
         return self.config["input_keys"]
     
     @property
     def output_keys(self) -> List[str]:
         
         return self.config["output_keys"]
                 
-                
     @root_validator(pre=True)
     def validate_chains(cls, values: Dict) -> Dict:
         config = values["config"]
         chain_configs = config["chain_configs"]
         pipe_input_keys = config["input_keys"]
         
         known_variables = pipe_input_keys
@@ -105,15 +108,77 @@
                 pipeline_log.chain_outputs.append(chain_output)
                 
                 if chain_output.chain_success == False:
                     is_fail = True
                     error_message = "{chain_type} Chain Step#{i} failed. Error log: {error_log}".format(
                         chain_type=type(chain_in_pipe),
                         i=i+1, 
-                        error_log=chain_log.error_log)
+                        error_log=chain_log.logs["error_log"])
+                    pipeline_log.logs['error_log'] = error_message
+                else:
+                    outputs = chain_output.output_variables
+                    known_variables.update(outputs)
+            else:
+                pipeline_log.chain_logs.append(
+                    ChainLog(logs={"error_log" : "Error occurs before start this chain"})
+                )
+                pipeline_log.chain_outputs.append(
+                    ChainOutput(chain_success=False)
+                )
+        
+        if is_fail:
+
+            return (
+                PipelineOutput(pipeline_success=False),
+                pipeline_log
+            )
+        
+        output_variables = {key: val for key, val in known_variables.items() if key in self.output_keys}       
+
+        return (
+            PipelineOutput(pipeline_success=True, output_variables=output_variables),
+            pipeline_log
+        ) 
+
+    async def arun(self, inputs: Dict[str, Any]):
+        
+        # input validate
+        try:
+            self._validate_inputs(inputs)
+        except Exception as e:
+            return (
+                PipelineOutput(pipeline_success=False),
+                PipelineLog(logs={"error_log" : str(e)})
+            )
+            
+        # pipeline log
+        pipeline_log = PipelineLog()
+        
+        # run chains
+        known_variables = inputs
+        
+        is_fail = False
+        for i, chain_in_pipe in enumerate(self.chains):
+            chain_inputs = {key: val for key, val in known_variables.items() if key in chain_in_pipe.input_keys}
+            chain_outputs = {key: val for key, val in known_variables.items() if key in chain_in_pipe.output_keys}
+            if chain_in_pipe is not None and not is_fail:
+                if chain_in_pipe._chain_type == "FunctionChain" and chain_in_pipe._function is not None:
+                    chain_output, chain_log = await chain_in_pipe.arun(chain_inputs)
+                else:
+                    chain_output, chain_log = await chain_in_pipe.arun(chain_inputs,chain_outputs)
+                
+                pipeline_log.chain_logs.append(chain_log)
+                pipeline_log.chain_outputs.append(chain_output)
+                
+                if chain_output.chain_success == False:
+                    is_fail = True
+                    error_message = "{chain_type} Chain Step#{i} failed. Error log: {error_log}".format(
+                        chain_type=type(chain_in_pipe),
+                        i=i+1, 
+                        error_log=chain_log.logs['error_log'])
                     pipeline_log.logs['error_log'] = error_message
                 else:
                     outputs = chain_output.output_variables
                     known_variables.update(outputs)
             else:
                 pipeline_log.chain_logs.append(
                     ChainLog(logs={"error_log" : "Error occurs before start this chain"})
```

### Comparing `promptlabs-0.0.4/promptlabs/scheme/llm.py` & `promptlabs-0.0.5/promptlabs/scheme/llm.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,14 +31,22 @@
 class BaseLLM(BaseModel, ABC):
     @abstractmethod
     def generate(
         self,
         messages: List[Dict[str, Any]],
     ) -> Tuple[bool, Dict[str,Any]]:
         pass
+    
+    @abstractmethod
+    async def agenerate(
+        self,
+        messages: List[Dict[str, Any]],
+    ) -> Tuple[bool, Dict[str,Any]]:
+        pass
+
 
 class ChatOpenAI(BaseLLM):
     client: Any  #: :meta private:
     model_name: str = Field(default="gpt-3.5-turbo", alias="model")
     """Model name to use."""
     temperature: float = 0.7
     """What sampling temperature to use."""
@@ -82,14 +90,29 @@
         except Exception as e:
             return (False, {"error_log" : str(e)})
         try:
             if response['choices'][0]['finish_reason'] == 'stop':
                 return (True, {"response" : response})
         except Exception as e:
             return (False, {"error_log" : str(e), "response" : response})
+        
+    async def agenerate(
+        self,
+        messages: List[Dict[str, Any]],
+    ) -> Tuple[bool, Dict[str,Any]]:
+        openai_params = self._client_params
+        try:
+            response = await self.client.acreate(messages=messages, **openai_params)
+        except Exception as e:
+            return (False, {"error_log" : str(e)})
+        try:
+            if response['choices'][0]['finish_reason'] == 'stop':
+                return (True, {"response" : response})
+        except Exception as e:
+            return (False, {"error_log" : str(e), "response" : response})
     
     @property
     def _client_params(self) -> Mapping[str, Any]:
         """Get the parameters used for the openai client."""
         openai_creds: Dict[str, Any] = {
             "api_key": self.openai_api_key,
             "model": self.model_name,
```

### Comparing `promptlabs-0.0.4/promptlabs/scheme/template.py` & `promptlabs-0.0.5/promptlabs/scheme/template.py`

 * *Files identical despite different names*

### Comparing `promptlabs-0.0.4/setup.py` & `promptlabs-0.0.5/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 promptlabs: A Python package for PromptOps (versioning, logging, experimenting, etc.)
 """
 from setuptools import setup, find_namespace_packages
 
 setup(
     name="promptlabs",
-    version="0.0.4",
+    version="0.0.5",
     packages=find_namespace_packages(),
     description="promptlabs: A Python package for PromptOps (versioning, logging, experimenting, etc.)",
     auther="weavel",
     install_requires=['openai', 'pydantic', 'requests'],
     python_requires='>=3.7.1',
     keywords=['weavel', 'prompt', 'llm', 'promptops', 'promptlabs', 'prompt engineering']
 )
```

