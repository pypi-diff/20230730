# Comparing `tmp/examon_core-1.0.9.tar.gz` & `tmp/examon_core-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "examon_core-1.0.9.tar", max compression
+gzip compressed data, was "examon_core-1.1.0.tar", max compression
```

## Comparing `examon_core-1.0.9.tar` & `examon_core-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0      199 2023-05-28 20:39:21.972747 examon_core-1.0.9/examon_core/__init__.py
--rw-r--r--   0        0        0     1039 2023-07-16 08:19:13.878728 examon_core-1.0.9/examon_core/code_metrics.py
--rwxr-xr-x   0        0        0      574 2023-07-17 15:50:11.694400 examon_core-1.0.9/examon_core/examon_item.py
--rwxr-xr-x   0        0        0     1606 2023-07-21 16:14:24.632842 examon_core-1.0.9/examon_core/examon_item_registry.py
--rwxr-xr-x   0        0        0     1697 2023-07-16 08:20:56.019327 examon_core-1.0.9/examon_core/function_raw_code.py
--rw-r--r--   0        0        0      408 2023-07-16 08:19:13.774401 examon_core-1.0.9/examon_core/multi_choice_factory.py
--rw-r--r--   0        0        0      980 2023-07-16 08:19:13.846489 examon_core-1.0.9/examon_core/print_ext.py
--rwxr-xr-x   0        0        0      620 2023-07-16 08:19:13.933636 examon_core-1.0.9/examon_core/question.py
--rw-r--r--   0        0        0     2632 2023-07-23 11:03:35.138786 examon_core-1.0.9/examon_core/question_factory.py
--rwxr-xr-x   0        0        0      201 2023-07-15 15:48:50.722464 examon_core-1.0.9/examon_core/question_response.py
--rw-r--r--   0        0        0      107 2023-07-17 15:48:04.895960 examon_core-1.0.9/examon_core/todo.md
--rw-r--r--   0        0        0      517 2023-07-23 11:07:34.365034 examon_core-1.0.9/pyproject.toml
--rw-r--r--   0        0        0      461 1970-01-01 00:00:00.000000 examon_core-1.0.9/PKG-INFO
+-rw-r--r--   0        0        0      225 2023-07-28 15:55:25.250080 examon_core-1.1.0/examon_core/__init__.py
+-rwxr-xr-x   0        0        0     1908 2023-07-30 15:28:57.756531 examon_core-1.1.0/examon_core/code_as_string_factory.py
+-rw-r--r--   0        0        0     1301 2023-07-30 18:35:51.460062 examon_core-1.1.0/examon_core/code_execution_sandbox.py
+-rw-r--r--   0        0        0     1671 2023-07-30 08:22:25.918054 examon_core-1.1.0/examon_core/code_metrics.py
+-rwxr-xr-x   0        0        0      574 2023-07-17 15:50:11.694400 examon_core-1.1.0/examon_core/examon_item.py
+-rwxr-xr-x   0        0        0     2085 2023-07-30 15:20:51.926942 examon_core-1.1.0/examon_core/examon_item_registry.py
+-rw-r--r--   0        0        0      408 2023-07-16 08:19:13.774401 examon_core-1.1.0/examon_core/multi_choice_factory.py
+-rwxr-xr-x   0        0        0      617 2023-07-30 15:10:40.198476 examon_core-1.1.0/examon_core/question.py
+-rw-r--r--   0        0        0     3000 2023-07-30 18:20:40.962231 examon_core-1.1.0/examon_core/question_factory.py
+-rwxr-xr-x   0        0        0      201 2023-07-15 15:48:50.722464 examon_core-1.1.0/examon_core/question_response.py
+-rw-r--r--   0        0        0      550 2023-07-30 18:39:40.266777 examon_core-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      507 1970-01-01 00:00:00.000000 examon_core-1.1.0/PKG-INFO
```

### Comparing `examon_core-1.0.9/examon_core/examon_item.py` & `examon_core-1.1.0/examon_core/examon_item.py`

 * *Files identical despite different names*

### Comparing `examon_core-1.0.9/examon_core/examon_item_registry.py` & `examon_core-1.1.0/examon_core/examon_item_registry.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from dataclasses import dataclass
 import logging
 
 
 @dataclass
 class ItemRegistryFilter:
     tags_any: list = None
-    difficulty: str = None
+    difficulty_category: str = None
     tags_all: list = None
     max_questions: int = None
 
 
 class ExamonItemRegistry:
     __registry = []
     __tags = []
@@ -25,32 +25,46 @@
     @classmethod
     def reset(cls):
         cls.__registry = []
         cls.__filter = None
 
     @classmethod
     def registry(cls, examon_filter=None):
-        def intersection(lst1, lst2):
-            return list(set(lst1) & set(lst2))
-
         results = cls.__registry
         if examon_filter is None:
             return results
-        elif examon_filter.tags_any is not None:
+
+        def intersection(lst1, lst2):
+            return list(set(lst1) & set(lst2))
+
+        def array_contains_any(array, has_one):
+            return len(intersection(array, has_one)) > 0
+
+        def array_contains_all(array, has_one):
+            return len(intersection(array, has_one)) == len(has_one)
+
+        if examon_filter.tags_any is not None:
             results = [
                 py_quiz_data
                 for py_quiz_data in cls.__registry
-                if len(intersection(examon_filter.tags_any, py_quiz_data.tags)) > 0
+                if array_contains_any(examon_filter.tags_any, py_quiz_data.tags)
             ]
-        elif examon_filter.tags_all is not None:
+        if examon_filter.tags_all is not None:
             results = [
                 py_quiz_data
                 for py_quiz_data in cls.__registry
-                if len(intersection(examon_filter.tags_all, py_quiz_data.tags)) == len(py_quiz_data.tags)
+                if array_contains_all(examon_filter.tags_all, py_quiz_data.tags)
             ]
+        if examon_filter.difficulty_category is not None:
+            results = [
+                py_quiz_data
+                for py_quiz_data in cls.__registry
+                if examon_filter.difficulty_category == py_quiz_data.metrics.categorised_difficulty
+            ]
+
         if examon_filter.max_questions is not None:
             return results[0:examon_filter.max_questions]
         else:
             return results
 
     @classmethod
     def unique_tags(cls):
```

### Comparing `examon_core-1.0.9/examon_core/function_raw_code.py` & `examon_core-1.1.0/examon_core/code_as_string_factory.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import inspect
 import re
 import logging
 
 
-class RawCodeFactory:
+class CodeAsStringFactory:
     @staticmethod
     def build(function, decorators=[]):
-        src_code = RawCodeFactory.function_src(function)
+        src_code = CodeAsStringFactory.function_src(function)
         for decorator in decorators:
-            logging.debug(f'RawCodeFactory.build: {decorator}')
+            logging.debug(f'CodeAsStringFactory.build: {decorator}')
             src_code = decorator.decorate(src_code)
-            logging.debug(f'RawCodeFactory.build: {src_code}')
+            logging.debug(f'CodeAsStringFactory.build: {src_code}')
 
-        logging.debug(f'RawCodeFactory.build: {src_code}')
+        logging.debug(f'CodeAsStringFactory.build: {src_code}')
         return src_code
 
     @staticmethod
     def function_src(function):
-        logging.debug(f'RawCodeFactory.function_src: {function}')
+        logging.debug(f'CodeAsStringFactory.function_src: {function}')
         return inspect.getsource(function).strip()
 
 
 class SourceCodeCommentsDecorator:
     def __init__(self, hints):
         self.hints = hints
 
@@ -38,20 +38,23 @@
 
 class RemoveQuizItemDecorator:
     def decorate(self, src_code):
         return re.sub('@examon\\_item\\(.*\\)', '', src_code)
 
 
 class AppendPrintDecorator:
-    def __init__(self, function_name):
+    def __init__(self, function_name, param=''):
         self.function_name = function_name
+        self.param = param
 
     def decorate(self, src_code):
-        println = f'\n\nprint({self.function_name}())'
+        if isinstance(self.param, str) and self.param != '':
+            self.param = f"'{self.param}'"
+        println = f'\n\nprint({self.function_name}({self.param}))'
         return src_code + println
 
 
-def function_raw_code(function, hints):
-    append_print_decorator = AppendPrintDecorator(function.__name__)
+def default_code_as_string_factory(function, param=''):
+    append_print_decorator = AppendPrintDecorator(function.__name__, param)
     remove_quiz_item_decorator = RemoveQuizItemDecorator()
     decorators = [remove_quiz_item_decorator, append_print_decorator]
-    return RawCodeFactory.build(function, decorators)
+    return CodeAsStringFactory.build(function, decorators)
```

### Comparing `examon_core-1.0.9/examon_core/question.py` & `examon_core-1.1.0/examon_core/question.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     metrics: Any = None
 
     def answer(self, given_answer):
         return str(self.correct_answer) == str(given_answer)
 
 
 @dataclass
-class ExpectedResultQuestion(BaseQuestion):
+class MultiChoiceQuestion(BaseQuestion):
     correct_answer: str = None
 
 
 @dataclass
 class InputParameterQuestion(BaseQuestion):
     return_value: str = None
     selected_param: str = None
```

### Comparing `examon_core-1.0.9/examon_core/question_factory.py` & `examon_core-1.1.0/examon_core/question_factory.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,80 +1,81 @@
-from .question import ExpectedResultQuestion, InputParameterQuestion, BaseQuestion
+from .question import MultiChoiceQuestion, InputParameterQuestion, BaseQuestion
 from .multi_choice_factory import MultiChoiceFactory
-from .function_raw_code import function_raw_code
-from .print_ext import PrintLog
+from .code_as_string_factory import default_code_as_string_factory
 from .code_metrics import CodeMetricsFactory
-
+from .code_execution_sandbox import CodeExecutionSandbox
 import random
 import logging
 
 
+class InvalidAnswerException(Exception):
+    pass
+
+
 class QuestionFactory:
     @staticmethod
     def build(**kwargs):
         function = kwargs['function']
         tags = kwargs['tags']
         hints = kwargs['hints'] if 'hints' in kwargs.keys() else []
         param1 = kwargs['param1'] if 'param1' in kwargs else None
-        choice_list = kwargs['choice_list']
-        fn_string = function_raw_code(function, hints)
-        first_line_no = function.__code__.co_firstlineno
-
-        # Code Metrics
-        metrics = CodeMetricsFactory.build(fn_string)
+        choice_list = []
+        if 'choice_list' in kwargs and kwargs['choice_list'] is not None:
+            choice_list = list(map(lambda x: str(x), kwargs['choice_list']))
 
         # Build
         if param1 is not None:
-            selected_input_param = random.choice(param1)
-            PrintLog.reset()
-            return_value = QuestionFactory.run_function_with_param(
-                function, selected_input_param
-            )
-            PrintLog.apply_offset(first_line_no)
-            print_logs = PrintLog.logs()
-            PrintLog.reset()
-
-            question = InputParameterQuestion(
-                selected_param=selected_input_param,
-                choices=param1
-            )
-            question.return_value = return_value
+            fn_string, metrics, question = QuestionFactory.build_input_param_question(function, param1)
         else:
-            # Print Logs
-            PrintLog.reset()
-            correct_answer = QuestionFactory.run_function(function=function)
-            PrintLog.apply_offset(first_line_no)
-            print_logs = PrintLog.logs()
-            PrintLog.reset()
-
-            if choice_list is not None:
-                question = ExpectedResultQuestion(
-                    choices=(
-                        MultiChoiceFactory.build(
-                            correct_answer,
-                            choice_list)))
-            else:
-                question = BaseQuestion()
-            question.correct_answer = correct_answer
+            fn_string, metrics, question = QuestionFactory.method_name1(choice_list, function)
 
         question.metrics = metrics
         question.hints = hints
         question.tags = tags
-        question.print_logs = print_logs
         question.function_src = fn_string
         logging.debug(f'QuestionFactory.build: {question}')
         return question
 
     @staticmethod
-    def run_function(function):
-        try:
-            result = function()
-            return result
-        except Exception as e:
-            return repr(e)
+    def method_name1(choice_list, function):
+        function_src = default_code_as_string_factory(function)
+        metrics = CodeMetricsFactory.build(function_src)
+        print_logs = QuestionFactory.run_function(function_src)
+        if choice_list is not None:
+            question = MultiChoiceQuestion(
+                correct_answer=print_logs[-1],
+                print_logs=print_logs,
+                choices=(
+                    MultiChoiceFactory.build(
+                        print_logs[-1],
+                        choice_list
+                    )
+                )
+            )
+        else:
+            question = BaseQuestion(function_src=function_src,
+                                    print_logs=print_logs,
+                                    correct_answer=print_logs[-1])
+        return function_src, metrics, question
 
     @staticmethod
-    def run_function_with_param(function, param):
-        try:
-            return str(function(param))
-        except Exception as e:
-            return repr(e)
+    def build_input_param_question(function, param1):
+        selected_input_param = random.choice(param1)
+        function_src = default_code_as_string_factory(function, selected_input_param)
+        print_logs = QuestionFactory.run_function(function_src)
+        metrics = CodeMetricsFactory.build(function_src)
+        return_value = print_logs[-1]
+        question = InputParameterQuestion(
+            selected_param=selected_input_param,
+            choices=param1,
+            function_src=function_src,
+            print_logs=print_logs
+        )
+        question.return_value = return_value
+        return function_src, metrics, question
+
+    @staticmethod
+    def run_function(source_code):
+        ces = CodeExecutionSandbox(source_code)
+        ces.execute()
+
+        return ces.print_logs
```

