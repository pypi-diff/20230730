# Comparing `tmp/examon-0.5.1.tar.gz` & `tmp/examon-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "examon-0.5.1.tar", max compression
+gzip compressed data, was "examon-0.5.4.tar", max compression
```

## Comparing `examon-0.5.1.tar` & `examon-0.5.4.tar`

### file list

```diff
@@ -1,25 +1,27 @@
--rw-r--r--   0        0        0      837 2023-07-11 11:00:43.648041 examon-0.5.1/README.md
--rwxr-xr-x   0        0        0        0 2023-01-06 12:36:14.367207 examon-0.5.1/examon/__init__.py
--rwxr-xr-x   0        0        0       24 2023-01-28 12:15:25.205762 examon-0.5.1/examon/lib/__init__.py
--rwxr-xr-x   0        0        0      468 2023-02-04 14:18:10.434445 examon-0.5.1/examon/lib/calc_stats.py
--rw-r--r--   0        0        0     1738 2023-07-12 20:04:21.589727 examon-0.5.1/examon/lib/quiz_engine.py
--rw-r--r--   0        0        0     1242 2023-07-12 20:04:21.584847 examon-0.5.1/examon/lib/quiz_engine_factory.py
--rw-r--r--   0        0        0     2389 2023-07-09 19:37:47.112886 examon-0.5.1/examon/lib/repo_manager.py
--rw-r--r--   0        0        0      366 2023-05-09 19:07:23.705779 examon-0.5.1/examon/lib/streak_tracker.py
--rwxr-xr-x   0        0        0       99 2023-07-12 20:13:15.318911 examon-0.5.1/examon/main.py
--rwxr-xr-x   0        0        0        0 2023-01-20 16:32:50.288125 examon-0.5.1/examon/view/__init__.py
--rw-r--r--   0        0        0        0 2023-07-09 19:56:53.890002 examon-0.5.1/examon/view/cli/__init__.py
--rwxr-xr-x   0        0        0     1711 2023-07-09 20:21:28.227289 examon-0.5.1/examon/view/cli/examon_arg_parse.py
--rwxr-xr-x   0        0        0      663 2023-07-12 17:14:39.575934 examon-0.5.1/examon/view/cli/main.py
--rw-r--r--   0        0        0      312 2023-07-12 17:16:53.877238 examon-0.5.1/examon/view/cli/overview.py
--rw-r--r--   0        0        0     1134 2023-07-11 10:42:41.187587 examon-0.5.1/examon/view/cli/repo.py
--rw-r--r--   0        0        0      488 2023-07-12 17:16:20.529570 examon-0.5.1/examon/view/cli/runner.py
--rwxr-xr-x   0        0        0      861 2023-04-12 17:42:31.225766 examon-0.5.1/examon/view/formatter_options.py
--rwxr-xr-x   0        0        0        0 2023-01-22 21:43:58.660247 examon-0.5.1/examon/view/input/__init__.py
--rwxr-xr-x   0        0        0      706 2023-07-08 09:55:03.400755 examon-0.5.1/examon/view/input/answer_question.py
--rwxr-xr-x   0        0        0        0 2023-01-22 21:44:07.847782 examon-0.5.1/examon/view/output/__init__.py
--rwxr-xr-x   0        0        0      187 2023-04-12 17:29:51.001345 examon-0.5.1/examon/view/output/display_stats.py
--rwxr-xr-x   0        0        0      335 2023-01-28 12:55:33.777034 examon-0.5.1/examon/view/output/functions.py
--rwxr-xr-x   0        0        0     1771 2023-06-03 10:59:00.541458 examon-0.5.1/examon/view/output/question.py
--rwxr-xr-x   0        0        0      532 2023-07-12 20:21:35.984248 examon-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     1436 1970-01-01 00:00:00.000000 examon-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0      820 2023-07-18 13:39:43.297716 examon-0.5.4/README.md
+-rwxr-xr-x   0        0        0        0 2023-01-06 12:36:14.367207 examon-0.5.4/examon/__init__.py
+-rwxr-xr-x   0        0        0       24 2023-01-28 12:15:25.205762 examon-0.5.4/examon/lib/__init__.py
+-rw-r--r--   0        0        0      536 2023-07-27 13:57:45.119515 examon-0.5.4/examon/lib/examon_config.py
+-rw-r--r--   0        0        0     1751 2023-07-15 11:53:35.970348 examon-0.5.4/examon/lib/examon_engine.py
+-rw-r--r--   0        0        0     1541 2023-07-15 12:06:34.065368 examon-0.5.4/examon/lib/examon_engine_factory.py
+-rw-r--r--   0        0        0     2382 2023-07-27 13:35:59.867607 examon-0.5.4/examon/lib/package_manager.py
+-rw-r--r--   0        0        0      820 2023-07-27 13:35:59.872649 examon-0.5.4/examon/lib/pip_installer.py
+-rw-r--r--   0        0        0     1116 2023-07-28 14:55:00.396350 examon-0.5.4/examon/lib/results_manager.py
+-rwxr-xr-x   0        0        0      606 2023-07-15 11:48:57.713181 examon-0.5.4/examon/lib/stats.py
+-rw-r--r--   0        0        0      367 2023-07-15 11:53:35.880898 examon-0.5.4/examon/lib/streak_tracker.py
+-rwxr-xr-x   0        0        0       99 2023-07-12 20:13:15.318911 examon-0.5.4/examon/main.py
+-rwxr-xr-x   0        0        0        0 2023-01-20 16:32:50.288125 examon-0.5.4/examon/view/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-09 19:56:53.890002 examon-0.5.4/examon/view/cli/__init__.py
+-rwxr-xr-x   0        0        0     1918 2023-07-25 06:03:38.544248 examon-0.5.4/examon/view/cli/examon_arg_parse.py
+-rw-r--r--   0        0        0     2600 2023-07-29 16:53:54.452624 examon-0.5.4/examon/view/cli/interactive.py
+-rwxr-xr-x   0        0        0      946 2023-07-23 10:24:31.594694 examon-0.5.4/examon/view/cli/main.py
+-rw-r--r--   0        0        0      301 2023-07-15 12:15:59.351678 examon-0.5.4/examon/view/cli/overview.py
+-rw-r--r--   0        0        0     1949 2023-07-27 13:41:27.906806 examon-0.5.4/examon/view/cli/package.py
+-rw-r--r--   0        0        0     1903 2023-07-28 14:55:00.383978 examon-0.5.4/examon/view/cli/runner.py
+-rwxr-xr-x   0        0        0      862 2023-07-15 11:53:35.671820 examon-0.5.4/examon/view/formatter_options.py
+-rwxr-xr-x   0        0        0        0 2023-01-22 21:43:58.660247 examon-0.5.4/examon/view/input/__init__.py
+-rwxr-xr-x   0        0        0      706 2023-07-08 09:55:03.400755 examon-0.5.4/examon/view/input/answer_question.py
+-rwxr-xr-x   0        0        0        0 2023-01-22 21:44:07.847782 examon-0.5.4/examon/view/output/__init__.py
+-rwxr-xr-x   0        0        0     2001 2023-07-29 20:47:42.245738 examon-0.5.4/examon/view/output/question.py
+-rwxr-xr-x   0        0        0      546 2023-07-30 18:42:22.446931 examon-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0     1433 1970-01-01 00:00:00.000000 examon-0.5.4/PKG-INFO
```

### Comparing `examon-0.5.1/README.md` & `examon-0.5.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -5,31 +5,31 @@
 * Python 3.9.15 or later
 * Pip
 
 ## Quick Start
 
 ```shell
 pip install examon
-examon repo add pcap1
-examon repo add_active pcap1
-examon repo install
-examon quiz 
+examon
 ```
 
 ### Customising Your Exam
 
 #### Set the active repos
 
-Examon will only use questions from repositories added which have been marked as active
+Examon will only use questions from repositories you have added which have been marked as active
 
 ```shell
 examon repos list
 examon repos add_active <repo name>
 ```
 * Use the tag filter
+```shell
+examon run --tag "<tag>"
+```
 
 ## Active Exam Repositories
 
 | Description | Pip Package |
 |-------------|-------------|
 | Beginners   ||
 | PCEP 1      ||
@@ -40,14 +40,16 @@
 
 ## Creating your own Exam
 
 ### Install from Pypi
 
 ### Install from GitHub
 
+## Security
+
 ## Roadmap
 
 ### V1.1
 
 * Filter questions by multiple tags
 * Filter questions by difficulty
 * Filter questions by LOC
```

### Comparing `examon-0.5.1/examon/lib/quiz_engine.py` & `examon-0.5.4/examon/lib/examon_engine.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from examon_core.question_response import QuestionResponse
 from examon.lib.streak_tracker import StreakTracker
 
 
-class QuizEngine:
+class ExamonEngine:
     def __init__(self, questions=None,
                  stats_outputter=None,
                  view_mappings=None):
         self.questions = questions
         self.correct_answers = 0
         self.responses = []
         self.__streak = StreakTracker()
 
         self.__view_mappings = view_mappings
         self.__stats_outputter = stats_outputter
 
-
     def run(self):
         for question in self.questions:
             lookup_key = question.__class__.__name__
             self.display(lookup_key, question)
             choice = self.get_user_input(lookup_key, question)
             correct = question.answer(choice)
             if correct:
@@ -27,20 +26,20 @@
             else:
                 self.__streak.reset()
 
             self.responses.append(QuestionResponse(question, choice, correct))
 
         self.final_summary()
 
-
     def get_user_input(self, lookup_key, question):
         return self.__view_mappings[lookup_key]['inputter'].prompt(question)
 
     def display(self, lookup, question):
-        self.__view_mappings[lookup]['outputter'].present_summary((self.summary()))
+        self.__view_mappings[lookup]['outputter'].present_summary(
+            (self.summary()))
         self.__view_mappings[lookup]['outputter'].present_question(question)
         return lookup
 
     def final_summary(self):
         correct, no = self.summary()
         print(f'You scored:\t{correct} / {no}')
         self.__streak.reset()
```

### Comparing `examon-0.5.1/examon/lib/quiz_engine_factory.py` & `examon-0.5.4/examon/lib/examon_engine_factory.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,37 @@
-from examon_core.question import *
-from examon_core.examon_item_registry import *
+from examon_core.question import BaseQuestion, ExpectedResultQuestion, \
+    InputParameterQuestion
+from examon_core.examon_item_registry import ExamonItemRegistry
 
-from examon.view.input.answer_question import AnswerInputter, FreeTextAnswerInputter
-from examon.view.output.question import *
-from .calc_stats import calc_stats
-from .quiz_engine import QuizEngine
+from examon.view.input.answer_question import AnswerInputter,\
+    FreeTextAnswerInputter
+from examon.view.output.question import ExpectedResultQuestionOutputter, \
+    InputParameterQuestionOutputter, FreeTextQuestionOutputter
+from .stats import Stats
+from .examon_engine import ExamonEngine
 
 
-class QuizEngineFactory:
+class ExamonEngineFactory:
     @staticmethod
     def build(tag, formatter_class, auto_answer=None):
+        def fetch_inputter(enabled, inputter):
+            return enabled if enabled else inputter
+
         registry = ExamonItemRegistry.registry(tag)
         view_mappings = {
             ExpectedResultQuestion.__name__: {
                 'outputter': ExpectedResultQuestionOutputter(formatter_class),
-                'inputter': auto_answer if auto_answer else AnswerInputter()
+                'inputter': fetch_inputter(auto_answer, AnswerInputter())
             },
             InputParameterQuestion.__name__: {
                 'outputter': InputParameterQuestionOutputter(formatter_class),
-                'inputter': auto_answer if auto_answer else AnswerInputter()
+                'inputter': fetch_inputter(auto_answer, AnswerInputter())
             }, BaseQuestion.__name__: {
                 'outputter': FreeTextQuestionOutputter(formatter_class),
-                'inputter': auto_answer if auto_answer else FreeTextAnswerInputter()
+                'inputter': fetch_inputter(
+                    auto_answer, FreeTextAnswerInputter())
             }
         }
-        return QuizEngine(
+        return ExamonEngine(
             questions=registry,
             view_mappings=view_mappings,
-            stats_outputter=calc_stats)
+            stats_outputter=Stats.calc_stats)
```

### Comparing `examon-0.5.1/examon/view/cli/examon_arg_parse.py` & `examon-0.5.4/examon/view/cli/examon_arg_parse.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,51 @@
 import argparse
 from examon.view.formatter_options import FormatterOptions
 
+
 class ExamonArgParse:
     def __init__(self, parser, formatter_options):
         self.__parser = parser
         self.__formatter_options = formatter_options
         self.__setup_args()
 
     def parse(self):
         return self.__parser.parse_args()
 
     def __setup_args(self):
-        subparsers = self.__parser.add_subparsers(help='Manage question repositories', dest='command')
-        repo_subparser = subparsers.add_parser('repo',
-                                               help='Manage question repositories',
-                                               aliases=['repos', 'repository', 'repositories'])
-        repo_subparser.add_argument('sub_command', help='[add|remove|list|init|help]')
-        repo_subparser.add_argument('--name', help='pip repository module name')
-        repo_subparser.add_argument('--pip-url', help='pip repository module name')
+        subparsers = self.__parser.add_subparsers(
+            help='Manage question repositories', dest='command')
+        package_subparser = subparsers.add_parser(
+            'package', help='Manage question packages', aliases=[
+                'packages'])
+        package_subparser.add_argument(
+            'sub_command', help='[add|remove|list|init|help]')
+        package_subparser.add_argument(
+            '--name', help='pip repository module name')
+        package_subparser.add_argument(
+            '--pip-url', help='pip repository module name')
 
         subparsers.add_parser('help', help='Print this message')
 
         run_subparser = subparsers.add_parser('run', help='Run the quiz')
         run_subparser.add_argument("--formatter", help='')
         run_subparser.add_argument("--tag", help='')
+        run_subparser.add_argument("--tags", help='')
+        run_subparser.add_argument("--tags-mandatory", help='')
+        run_subparser.add_argument("--max-questions", help='')
+        run_subparser.add_argument("--file", help='')
 
         subparsers.add_parser('tag',
                               help='Tag Information',
                               aliases=['tags'])
 
         subparsers.add_parser('overview',
                               help='Tag Information',
                               aliases=['tags'])
 
+
 class ExamonArgParseFactory:
     @staticmethod
     def build():
         parser = argparse.ArgumentParser(prog='Examon CLI')
         cli_args = ExamonArgParse(parser, FormatterOptions()).parse()
-        return (parser, cli_args)
+        return parser, cli_args
```

### Comparing `examon-0.5.1/examon/view/formatter_options.py` & `examon-0.5.4/examon/view/formatter_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     ('terminal256', Terminal256Formatter),
     ('terminal', TerminalFormatter),
     ('null', NullFormatter),
     ('true', TerminalTrueColorFormatter),
     ('raw', RawTokenFormatter)
 ]
 
+
 class FormatterOptions:
     def __init__(self):
         self.formatter_options = defaultdict(lambda: Terminal256Formatter)
         for option in OPTIONS:
             self.formatter_options[option[0]] = option[1]
 
     def __getitem__(self, item):
```

### Comparing `examon-0.5.1/examon/view/input/answer_question.py` & `examon-0.5.4/examon/view/input/answer_question.py`

 * *Files identical despite different names*

### Comparing `examon-0.5.1/examon/view/output/question.py` & `examon-0.5.4/examon/view/output/question.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 import os
 from pygments import highlight
 from pygments.lexers import PythonLexer
 
+
 class BaseQuestionOutputter():
     def __init__(self, formatter_class):
         self.formatter_class = formatter_class
 
+    def print_metrics(self, question):
+        print(f'Difficulty: {question.metrics.calc_difficulty()}')
+
     def present_summary(self, summary):
         os.system('clear')
         print(f'You are: {summary}')
 
     def present_question(self, question):
         print(
             highlight(
@@ -17,45 +21,48 @@
                 PythonLexer(),
                 self.formatter_class()))
 
     def display_print_logs(self, question):
         if len(question.print_logs) > 1:
             print('Print logs:')
             for log in question.print_logs:
-                print(f' - {log[0]}')
+                print(f' - {log.output}')
             print('')
 
 
 class InputParameterQuestionOutputter(BaseQuestionOutputter):
     def present_question(self, question):
         print('')
+        self.print_metrics(question)
         print('')
         super().present_question(question)
         print('')
-        print('What does the parameter need to be for the last print statement to return:')
+        test = 'What does the parameter need to be for' \
+               ' the last print statement to return:'
+        print(test)
         print(question.return_value)
         print('')
         print('')
         self.display_print_logs(question)
 
 
 class ExpectedResultQuestionOutputter(BaseQuestionOutputter):
     def present_question(self, question):
         print('')
-        print(question.metrics)
+        self.print_metrics(question)
         print('What is the result of the last print statement?')
         print('')
         super().present_question(question)
         print('')
         self.display_print_logs(question)
 
 
 class FreeTextQuestionOutputter(BaseQuestionOutputter):
     def present_question(self, question):
         print('')
+        self.print_metrics(question)
         print('')
         super().present_question(question)
         print('')
         print('What will this return?')
         print('')
         self.display_print_logs(question)
-
```

### Comparing `examon-0.5.1/PKG-INFO` & `examon-0.5.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: examon
-Version: 0.5.1
+Version: 0.5.4
 Summary: 
 Author: Jarrod Folino
 Author-email: jdfolino@icloud.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: consolemenu (>=1.0.1,<2.0.0)
-Requires-Dist: examon-core (==1.0.0)
+Requires-Dist: dataclasses-serialization (>=1.3.1,<2.0.0)
+Requires-Dist: examon-core (==1.1.0)
 Requires-Dist: inquirer (>=3.1.1,<4.0.0)
 Requires-Dist: pygments (>=2.13.0,<3.0.0)
 Requires-Dist: simple-term-menu (>=1.6.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 # ExamOn
 
@@ -23,31 +23,31 @@
 * Python 3.9.15 or later
 * Pip
 
 ## Quick Start
 
 ```shell
 pip install examon
-examon repo add pcap1
-examon repo add_active pcap1
-examon repo install
-examon quiz 
+examon
 ```
 
 ### Customising Your Exam
 
 #### Set the active repos
 
-Examon will only use questions from repositories added which have been marked as active
+Examon will only use questions from repositories you have added which have been marked as active
 
 ```shell
 examon repos list
 examon repos add_active <repo name>
 ```
 * Use the tag filter
+```shell
+examon run --tag "<tag>"
+```
 
 ## Active Exam Repositories
 
 | Description | Pip Package |
 |-------------|-------------|
 | Beginners   ||
 | PCEP 1      ||
@@ -58,14 +58,16 @@
 
 ## Creating your own Exam
 
 ### Install from Pypi
 
 ### Install from GitHub
 
+## Security
+
 ## Roadmap
 
 ### V1.1
 
 * Filter questions by multiple tags
 * Filter questions by difficulty
 * Filter questions by LOC
```

