# Comparing `tmp/fastllm-0.1.3.tar.gz` & `tmp/fastllm-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastllm-0.1.3.tar", max compression
+gzip compressed data, was "fastllm-0.1.4.tar", max compression
```

## Comparing `fastllm-0.1.3.tar` & `fastllm-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,8 @@
--rw-r--r--   0        0        0    11357 2023-07-24 18:01:27.056723 fastllm-0.1.3/LICENSE
--rw-r--r--   0        0        0     4374 2023-07-25 19:28:31.313986 fastllm-0.1.3/README.md
--rw-r--r--   0        0        0      137 2023-07-24 18:01:27.056723 fastllm-0.1.3/fastllm/__init__.py
--rw-r--r--   0        0        0    19838 2023-07-25 19:28:19.493990 fastllm-0.1.3/fastllm/base.py
--rw-r--r--   0        0        0     1539 2023-07-25 19:28:04.093995 fastllm-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     5260 1970-01-01 00:00:00.000000 fastllm-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-16 18:54:36.878631 fastllm-0.1.4/LICENSE
+-rw-r--r--   0        0        0     5353 2023-07-30 20:01:21.676030 fastllm-0.1.4/README.md
+-rw-r--r--   0        0        0      137 2023-07-23 15:51:19.906944 fastllm-0.1.4/fastllm/__init__.py
+-rw-r--r--   0        0        0    22275 2023-07-30 20:05:18.654169 fastllm-0.1.4/fastllm/base.py
+-rw-r--r--   0        0        0     1173 2023-07-30 20:00:28.975555 fastllm-0.1.4/fastllm/utils.py
+-rw-r--r--   0        0        0     1577 2023-07-30 20:01:57.104350 fastllm-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     6375 1970-01-01 00:00:00.000000 fastllm-0.1.4/setup.py
+-rw-r--r--   0        0        0     6470 1970-01-01 00:00:00.000000 fastllm-0.1.4/PKG-INFO
```

### Comparing `fastllm-0.1.3/LICENSE` & `fastllm-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fastllm-0.1.3/README.md` & `fastllm-0.1.4/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -82,52 +82,105 @@
         case _:
             raise ValueError(f"Unknown operator {operator}")
 
 
 result = calculator_agent(task="give the final result for (11 + 14) * (6 - 2)")
 
 print(result)
+```
+
+```bash
+100
+```
 
+```python
 another_result = calculator_agent(
     task="If I have 114 apples and 3 elephants, how many apples will each elephant get?"
 )
 
 print(another_result)
 ```
 
 ```bash
-100
 38
 ```
 
+#### Avoid and Prefer
+
+Guide completion by prefer or avoid certain words or phrases. Supports regex patterns. For avoiding/banning words typically it is advised to put a [blank space](https://community.openai.com/t/reproducible-gpt-3-5-turbo-logit-bias-100-not-functioning/88293/8) in front of the word.
+
+```python
+cat = Agent(
+    Prompt("Say Cat!"),
+)
+
+print(cat())
+```
+
+```bash
+Cat!
+```
+
+```python
+not_cat = Agent(
+    Prompt("Say Cat!", avoid=r"[ ]?Cat"),
+)
+
+print(not_cat())
+```
+
+OpenAI is making fun of us (that really happened!) and writes "Cat" with a lower case "c". 
+
+```bash
+Dog! Just kidding, cat!
+```
+
+Ok let's try again.
+
+```python
+seriously_not_a_cat = Agent(
+    Prompt("Say Cat!, PLEEASSEE", avoid=r"[ ]?[Cc][aA][tT]]"),
+)
+```
+
+Well no cat but kudos for the effort.
+
+```bash
+Sure, here you go: "Meow! "
+```
+
+
+
 ## Roadmap
 
 ### Features
 
 - [x] Prompts using jinja2 templates
 - [x] LLM calling with backoff and retry
 - [x] Able to register functions to agents, models and prompts using decorators
 - [x] Possible to register functions on multiple levels (agent, model, prompt). The function call is only available on the level it was registered.
 - [x] Conversation history. The Model class keeps track of the conversation history.
 - [x] Function schema is inferred from python function type hints, documentation and name
 - [x] Function calling is handled by the Model class itself. Meaning if a LLM response indicate a function call, the Model class will call the function and return the result back to the LLM
+- [x] Streaming with function calling
 - [ ] Function calling can result in an infinite loop if LLM can not provide function name or arguments properly. This needs to be handled by the Model class.
-- [ ] Streaming with function calling
+- [ ] Force particular function call by providing function call argument
 - [ ] Option to "smartly forget" conversation history in case context length is too long.
-- [ ] Prompts with pattern using logit bias to guide LLM completion.
+- [x] Prompts with pattern using logit bias to guide LLM completion.
 - [ ] Able to switch between models (e.g. 3.5 and 4) within one agent over different prompts.
 - [ ] Handling of multiple response messages from LLMs in a single call. At the moment only the first response is kept.
 - [ ] Supporting non chat based LLMs (e.g. OpenAI's completion LLMs).
 - [ ] Supporting other LLMs over APIs except OpenAI's. (e.g. Google etc.)
 - [ ] Supporting local LLMs (e.g. llama-1, llama-2, etc.)
 
 ### Package
 
 - [x] Basic package structure and functionality
 - [x] Test cases and high test coverage
+- [ ] Mock implementation of OpenAI's API for tests
 - [ ] Tests against multiple python versions
 - [ ] 100% test coverage (at the moment around 90%)
 - [ ] Better documentation including readthedocs site.
 - [ ] Better error handling and logging
 - [ ] Better samples using jupyter notebooks
 - [ ] Set up of pre-commit
 - [ ] CI using github actions
```

### Comparing `fastllm-0.1.3/fastllm/base.py` & `fastllm-0.1.4/fastllm/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 
 import backoff
 import openai
 from jinja2 import Template
 from jsonschema import ValidationError, validate
 from openai.error import RateLimitError, ServiceUnavailableError
 
+from fastllm.utils import get_logit_bias
+
 logger = logging.getLogger(__name__)
 
 
 P = ParamSpec("P")
 R = TypeVar("R")
 
 
@@ -269,31 +271,51 @@
                 else:
                     return function(**kwargs)
 
         raise ValueError(f"Function {name} not available. ")
 
 
 @dataclass
+class FunctionCall:
+    """Represents a function call in a message."""
+
+    name: str
+    arguments: str
+
+    def __add__(self, other: FunctionCall):
+        """Implements the + operator."""
+
+        if isinstance(other, FunctionCall):
+            return FunctionCall(
+                self.name,
+                self.arguments + other.arguments,
+            )
+        else:
+            raise TypeError(f"Cannot add FunctionCall and {type(other)}.")
+
+
+@dataclass
 class Message:
     """Represents a message when interacting with a chat model."""
 
     seed: InitVar[Message | dict | str]
     role: Role = Role.USER
     name: str | None = None
-    function_call: dict[str, str] | None = None
+    function_call: FunctionCall | None = None
     content: str = field(init=False, default="")
 
     def __post_init__(self, seed: Message | dict | str):
         """Initializes the message content."""
 
         if isinstance(seed, str):
             self.content = seed
         elif isinstance(seed, Message):
             self.content = seed.content
             self.role = seed.role
+            self.function_call = seed.function_call
         elif isinstance(seed, dict):
             _seed = self.from_response(seed)
 
             if len(_seed) > 1:
                 logger.warning(
                     "More than one message in response. Using first message."
                 )
@@ -307,37 +329,37 @@
     @classmethod
     def from_response(cls, response: dict) -> list[Message]:
         """Returns a message or a list of messages from a openai response dict."""
 
         messages = []
         for choice in response["choices"]:
             if "message" in choice:
-                message = choice["message"]
+                data = choice["message"]
 
-                content = "" if message["content"] is None else message["content"]
-                role = Role(message["role"])
+                content = "" if data["content"] is None else data["content"]
+                role = Role(data["role"])
 
-                if "function_call" in message:
-                    function_call = {
-                        "name": message["function_call"]["name"],
-                        "arguments": message["function_call"]["arguments"],
-                    }
-                    messages.append(Message(content, role, function_call=function_call))
-                else:
-                    messages.append(Message(content, role))
             elif "delta" in choice:
-                content = (
-                    choice["delta"]["content"] if "content" in choice["delta"] else ""
-                )
-                role = (
-                    Role(choice["delta"]["role"])
-                    if "role" in choice["delta"]
-                    else Role.ASSISTANT
-                )
+                data = choice["delta"]
+
+                content = data["content"] if "content" in data else ""
+                content = content or ""
 
+                role = Role(data["role"]) if "role" in data else Role.ASSISTANT
+            else:
+                raise ValueError("Cannot parse response.")
+
+            if "function_call" in data:
+                function_call = data["function_call"]
+
+                name = function_call["name"] if "name" in function_call else ""
+                function_call = FunctionCall(name, function_call["arguments"])
+
+                messages.append(Message(content, role, function_call=function_call))
+            else:
                 messages.append(Message(content, role))
 
         if len(messages) == 0:
             raise ValueError("No messages in response.")
 
         return messages
 
@@ -352,15 +374,27 @@
         return f"{self.role.value}: {self.content}"
 
     def __add__(self, other: Message | str) -> Message:
         """Implements the + operator."""
 
         if isinstance(other, Message):
             if self.role == other.role:
-                return Message(self.content + other.content, self.role)
+                function_call = None
+                if self.function_call and other.function_call:
+                    function_call = self.function_call + other.function_call
+                elif self.function_call:
+                    function_call = self.function_call
+                elif other.function_call:
+                    function_call = other.function_call
+
+                return Message(
+                    self.content + other.content,
+                    self.role,
+                    function_call=function_call,
+                )
             else:
                 raise ValueError("Cannot add messages with different roles.")
         elif isinstance(other, str):
             return Message(self.content + other, self.role)
         else:
             raise TypeError(f"Cannot add Message and {type(other)}.")
 
@@ -372,15 +406,18 @@
             "content": self.content if self.content else None,
         }
 
         if self.name:
             message["name"] = self.name
 
         if self.function_call:
-            message["function_call"] = self.function_call
+            message["function_call"] = {
+                "name": self.function_call.name,
+                "arguments": self.function_call.arguments,
+            }
 
         return message
 
 
 @dataclass
 class Conversation:
     """Represents a ordered list of messages."""
@@ -436,29 +473,35 @@
 
 @dataclass
 class Prompt(Functions):
     """Represents a prompt."""
 
     template: Template = field(init=False)
     role: Role = field(init=False, default=Role.USER)
+    prefer: list[str] | str | None = None
+    avoid: list[str] | str | None = None
     model_params: dict[str, Any] = field(default_factory=dict)
 
     def __init__(
         self,
         template: str,
         role: Role = Role.USER,
+        prefer: list[str] | str | None = None,
+        avoid: list[str] | str | None = None,
         functions: list[Callable[..., Any]] | None = None,
         **model_params,
     ):
         """Initializes the prompt."""
 
         super().__init__(functions=functions)
 
         self.template = Template(template)
         self.role = role
+        self.prefer = prefer
+        self.avoid = avoid
         self.model_params = model_params
 
     def __call__(self, **kwargs) -> Message:
         """Returns the message from the prompt."""
 
         return Message(self.template.render(**kwargs), self.role)
 
@@ -470,23 +513,23 @@
     seed: InitVar[Conversation | Message | str | None] = None
     name: str = "gpt-3.5-turbo-0613"
     stream_callback: Callable[[str], Any] | None = None
     conversation: Conversation = field(init=False, default_factory=Conversation)
 
     def __post_init__(
         self,
-        available_functions: list[Callable[..., Any]] | None = None,
+        functions: list[Callable[..., Any]] | None = None,
         seed: Conversation | Message | str | None = None,
     ):
         """Initializes the model.
 
         Optionally pass a seed as conversation, message or string.
         """
 
-        super().__post_init__(available_functions)
+        super().__post_init__(functions)
 
         if seed is None:
             self.conversation = Conversation()
         elif isinstance(seed, str):
             self.conversation = Conversation(Message(seed, Role.SYSTEM))
         elif isinstance(seed, Message):
             self.conversation = Conversation(seed)
@@ -495,14 +538,16 @@
         else:
             raise TypeError(f"Cannot create Model from {type(seed)}.")
 
     def __call__(
         self,
         *args: Conversation | Message | str,
         functions: list[Callable[..., Any]] | list[Function] | None = None,
+        prefer: list[str] | str | None = None,
+        avoid: list[str] | str | None = None,
         stream_callback: Callable[[str], Any] | None = None,
         **kwargs,
     ) -> str:
         """Returns the response of the model."""
 
         self.update(*args)
 
@@ -510,37 +555,41 @@
 
         if _functions:
             kwargs["functions"] = [function.schema for function in _functions]
             # kwargs["function_call"] = "auto"
 
         stream_callback = stream_callback or self.stream_callback
 
+        response = None
         if stream_callback:
-            response = Message("", Role.ASSISTANT)
-
-            for chunk in self.completion(stream=True, **kwargs):
+            for chunk in self.completion(
+                stream=True, prefer=prefer, avoid=avoid, **kwargs
+            ):
                 chunk = Message(chunk)
                 stream_callback(chunk.content)
 
-                response += chunk
+                response = chunk if response is None else response + chunk
         else:
-            response = next(self.completion(**kwargs))
+            response = next(self.completion(prefer=prefer, avoid=avoid, **kwargs))
+
+        if response is None:
+            raise ValueError("No response from model.")
 
         message = Message(response)
         if message.function_call:
             self.update(message)
 
             function_output = self.function_call(
-                message.function_call["name"],
-                message.function_call["arguments"],
+                message.function_call.name,
+                message.function_call.arguments,
                 functions=_functions,
             )
 
             function_message = Message(
-                str(function_output), Role.FUNCTION, message.function_call["name"]
+                str(function_output), Role.FUNCTION, message.function_call.name
             )
 
             kwargs.pop("functions", None)
 
             # TODO might result in an infinite loop - fix this!
             self(
                 function_message,
@@ -555,20 +604,48 @@
 
     @backoff.on_exception(
         backoff.expo,
         [RateLimitError, ServiceUnavailableError],
         max_time=60,
         logger=logger,
     )
-    def completion(self, stream: bool = False, **kwargs) -> Generator[dict, None, None]:
+    def completion(
+        self,
+        stream: bool = False,
+        prefer: list[str] | str | None = None,
+        avoid: list[str] | str | None = None,
+        **kwargs,
+    ) -> Generator[dict, None, None]:
         """Calls the model, retries on RateLimitError."""
 
+        name = kwargs.pop("name", self.name)
+        logit_bias = kwargs.get("logit_bias", {})
+
+        if prefer:
+            _logit_bias, _ = get_logit_bias(name, prefer)
+
+            logit_bias.update(_logit_bias)
+        if avoid:
+            _logit_bias, _ = get_logit_bias(name, avoid, bias=-100)
+
+            logit_bias.update(_logit_bias)
+
+        if logit_bias:
+            kwargs["logit_bias"] = logit_bias
+
+            # this is a hard limit by OpenAI for tokens with a logit bias
+            if len(kwargs["logit_bias"]) > 300:
+                raise ValueError(
+                    f'Too many tokens ({len(kwargs["logit_bias"])}) in logit bias \
+for model {name}.'
+                )
+
         if len(self.conversation) > 0:
             response = openai.ChatCompletion.create(
-                model=self.name,
+                model=name,
                 messages=self.conversation.to_list(),
                 stream=stream,
                 **kwargs,
             )
         else:
             raise ValueError("Cannot create completion from empty conversation.")
 
@@ -650,14 +727,16 @@
         for step in self.playbook:
             if isinstance(step, Prompt):
                 prompt = step
 
                 yield self.model(
                     *steps,
                     prompt(**inputs),
+                    prefer=prompt.prefer,
+                    avoid=prompt.avoid,
                     functions=prompt._functions + self._functions,
                     **prompt.model_params,
                 )
 
                 steps = []
             elif isinstance(step, Agent):
                 agent = step
```

### Comparing `fastllm-0.1.3/pyproject.toml` & `fastllm-0.1.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastllm"
-version = "0.1.3"
+version = "0.1.4"
 description = "Fast and easy wrapper around LLMs."
 authors = ["Clemens Kriechbaumer <clemens.kriechbaumer@gmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/clemens33/fastllm"
 repository = "https://github.com/clemens33/fastllm"
 keywords = ["agents", "chatbots", "openai", "llm", "ai"]
@@ -20,14 +20,16 @@
 
 [tool.poetry.dependencies]
 python = "^3.10"
 jinja2 = "^3.1.2"
 backoff = "^2.2.1"
 openai = "^0.27.8"
 jsonschema = "^4.18.4"
+tiktoken = "^0.4.0"
+exrex = "^0.11.0"
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.0.278"
 black = "^23.7.0"
 pyright = "^1.1.317"
 pytest = "^7.4.0"
 pytest-cov = "^4.1.0"
```

### Comparing `fastllm-0.1.3/PKG-INFO` & `fastllm-0.1.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 Metadata-Version: 2.1
 Name: fastllm
-Version: 0.1.3
+Version: 0.1.4
 Summary: Fast and easy wrapper around LLMs.
 Home-page: https://github.com/clemens33/fastllm
 License: Apache-2.0
 Keywords: agents,chatbots,openai,llm,ai
 Author: Clemens Kriechbaumer
 Author-email: clemens.kriechbaumer@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: backoff (>=2.2.1,<3.0.0)
+Requires-Dist: exrex (>=0.11.0,<0.12.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: jsonschema (>=4.18.4,<5.0.0)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
+Requires-Dist: tiktoken (>=0.4.0,<0.5.0)
 Project-URL: Repository, https://github.com/clemens33/fastllm
 Description-Content-Type: text/markdown
 
 # FastLLM
 
 Fast and simple wrapper around LLMs. The package aims to be simply, precise and allows for fast prototyping of agents and applications around LLMs. At the moment focus around OpenAI's chat models.
 
@@ -105,52 +110,105 @@
         case _:
             raise ValueError(f"Unknown operator {operator}")
 
 
 result = calculator_agent(task="give the final result for (11 + 14) * (6 - 2)")
 
 print(result)
+```
+
+```bash
+100
+```
 
+```python
 another_result = calculator_agent(
     task="If I have 114 apples and 3 elephants, how many apples will each elephant get?"
 )
 
 print(another_result)
 ```
 
 ```bash
-100
 38
 ```
 
+#### Avoid and Prefer
+
+Guide completion by prefer or avoid certain words or phrases. Supports regex patterns. For avoiding/banning words typically it is advised to put a [blank space](https://community.openai.com/t/reproducible-gpt-3-5-turbo-logit-bias-100-not-functioning/88293/8) in front of the word.
+
+```python
+cat = Agent(
+    Prompt("Say Cat!"),
+)
+
+print(cat())
+```
+
+```bash
+Cat!
+```
+
+```python
+not_cat = Agent(
+    Prompt("Say Cat!", avoid=r"[ ]?Cat"),
+)
+
+print(not_cat())
+```
+
+OpenAI is making fun of us (that really happened!) and writes "Cat" with a lower case "c". 
+
+```bash
+Dog! Just kidding, cat!
+```
+
+Ok let's try again.
+
+```python
+seriously_not_a_cat = Agent(
+    Prompt("Say Cat!, PLEEASSEE", avoid=r"[ ]?[Cc][aA][tT]]"),
+)
+```
+
+Well no cat but kudos for the effort.
+
+```bash
+Sure, here you go: "Meow! "
+```
+
+
+
 ## Roadmap
 
 ### Features
 
 - [x] Prompts using jinja2 templates
 - [x] LLM calling with backoff and retry
 - [x] Able to register functions to agents, models and prompts using decorators
 - [x] Possible to register functions on multiple levels (agent, model, prompt). The function call is only available on the level it was registered.
 - [x] Conversation history. The Model class keeps track of the conversation history.
 - [x] Function schema is inferred from python function type hints, documentation and name
 - [x] Function calling is handled by the Model class itself. Meaning if a LLM response indicate a function call, the Model class will call the function and return the result back to the LLM
+- [x] Streaming with function calling
 - [ ] Function calling can result in an infinite loop if LLM can not provide function name or arguments properly. This needs to be handled by the Model class.
-- [ ] Streaming with function calling
+- [ ] Force particular function call by providing function call argument
 - [ ] Option to "smartly forget" conversation history in case context length is too long.
-- [ ] Prompts with pattern using logit bias to guide LLM completion.
+- [x] Prompts with pattern using logit bias to guide LLM completion.
 - [ ] Able to switch between models (e.g. 3.5 and 4) within one agent over different prompts.
 - [ ] Handling of multiple response messages from LLMs in a single call. At the moment only the first response is kept.
 - [ ] Supporting non chat based LLMs (e.g. OpenAI's completion LLMs).
 - [ ] Supporting other LLMs over APIs except OpenAI's. (e.g. Google etc.)
 - [ ] Supporting local LLMs (e.g. llama-1, llama-2, etc.)
 
 ### Package
 
 - [x] Basic package structure and functionality
 - [x] Test cases and high test coverage
+- [ ] Mock implementation of OpenAI's API for tests
 - [ ] Tests against multiple python versions
 - [ ] 100% test coverage (at the moment around 90%)
 - [ ] Better documentation including readthedocs site.
 - [ ] Better error handling and logging
 - [ ] Better samples using jupyter notebooks
 - [ ] Set up of pre-commit
 - [ ] CI using github actions
```

