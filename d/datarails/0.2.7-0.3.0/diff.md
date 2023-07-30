# Comparing `tmp/datarails-0.2.7.tar.gz` & `tmp/datarails-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datarails-0.2.7.tar", last modified: Sat Jul 29 18:32:25 2023, max compression
+gzip compressed data, was "datarails-0.3.0.tar", last modified: Sun Jul 30 06:15:36 2023, max compression
```

## Comparing `datarails-0.2.7.tar` & `datarails-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:32:25.108359 datarails-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-07-29 18:32:25.108359 datarails-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-07-29 18:32:15.000000 datarails-0.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:32:25.108359 datarails-0.2.7/datarails/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-29 18:32:15.000000 datarails-0.2.7/datarails/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-07-29 18:32:03.000000 datarails-0.2.7/datarails/contexts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-07-29 18:32:03.000000 datarails-0.2.7/datarails/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-07-29 18:32:03.000000 datarails-0.2.7/datarails/step.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-29 18:32:03.000000 datarails-0.2.7/datarails/type_vars.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:32:25.108359 datarails-0.2.7/datarails.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-07-29 18:32:25.000000 datarails-0.2.7/datarails.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-29 18:32:25.000000 datarails-0.2.7/datarails.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 18:32:25.000000 datarails-0.2.7/datarails.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-29 18:32:25.000000 datarails-0.2.7/datarails.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-29 18:32:25.000000 datarails-0.2.7/datarails.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-29 18:32:15.000000 datarails-0.2.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 18:32:25.108359 datarails-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-29 18:32:03.000000 datarails-0.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:32:25.108359 datarails-0.2.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-07-29 18:32:03.000000 datarails-0.2.7/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-29 18:32:03.000000 datarails-0.2.7/tests/test_databox.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-29 18:32:03.000000 datarails-0.2.7/tests/test_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-07-29 18:32:03.000000 datarails-0.2.7/tests/test_step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 06:15:36.851199 datarails-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5928 2023-07-30 06:15:36.851199 datarails-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-07-30 06:15:25.000000 datarails-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 06:15:36.847199 datarails-0.3.0/datarails/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-30 06:15:25.000000 datarails-0.3.0/datarails/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-07-30 06:15:11.000000 datarails-0.3.0/datarails/contexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-07-30 06:15:11.000000 datarails-0.3.0/datarails/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-07-30 06:15:11.000000 datarails-0.3.0/datarails/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-30 06:15:11.000000 datarails-0.3.0/datarails/type_vars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 06:15:36.851199 datarails-0.3.0/datarails.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5928 2023-07-30 06:15:36.000000 datarails-0.3.0/datarails.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-30 06:15:36.000000 datarails-0.3.0/datarails.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 06:15:36.000000 datarails-0.3.0/datarails.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-30 06:15:36.000000 datarails-0.3.0/datarails.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-30 06:15:36.000000 datarails-0.3.0/datarails.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-30 06:15:25.000000 datarails-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 06:15:36.851199 datarails-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-30 06:15:11.000000 datarails-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 06:15:36.851199 datarails-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-07-30 06:15:11.000000 datarails-0.3.0/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-30 06:15:11.000000 datarails-0.3.0/tests/test_databox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-30 06:15:11.000000 datarails-0.3.0/tests/test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-07-30 06:15:11.000000 datarails-0.3.0/tests/test_step.py
```

### Comparing `datarails-0.2.7/PKG-INFO` & `datarails-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: datarails
-Version: 0.2.7
+Version: 0.3.0
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 
+[![Release python package](https://github.com/JesseMaitland/datarails/actions/workflows/release.yml/badge.svg)](https://github.com/JesseMaitland/datarails/actions/workflows/release.yml)
 # datarails -- A Simple Framework for Dataframe ETL
-####  -- VERSION 0.2.7 --
+####  -- VERSION 0.3.0 --
+
 
 ## Official Documentation
 The official documentation is hosted on github pages at [jesse.maitland.github.io](https://jessemaitland.github.io/datarails/)
 
 ## Example Project
 There is an example repo containing some simple ETL jobs, notebooks and commands for building documentation at [jessemaitland/datarails-example](https://github.com/JesseMaitland/datarails_examples)
 
@@ -25,63 +27,63 @@
 Each step has access to a `DataBox` object that can be used to store dataframes and access them by name in downstream steps.
 
 In addition to the `DataBox` object, each step has access to a `DataRailsContext` object that can be used to store and access variables that are not dataframes.
 
 ```python
 import pandas as pd
 from datarails.step import DataRailsStep
-from datarails.runner import StepRunner
+from datarails.runner import DataRailsStepRunner
 
 
 class LoadDataFromCSV(DataRailsStep):
-    
+
     def step_load_csv(self) -> None:
         print('loading data from csv')
         df = pd.read_csv('data.csv')
-        self.dbx.put_df('data', df) # dbx now has an attribute called data that is a dataframe
+        self.dbx.put_df('data', df)  # dbx now has an attribute called data that is a dataframe
 
 
 class TransformData(DataRailsStep):
-    
+
     def step_add_new_column(self) -> None:
         print('adding new column')
         self.dbx.data['new_column'] = self.dbx.data['old_column'] * 2
-    
+
     def step_drop_all_null_rows(self) -> None:
         print('dropping null rows')
         self.dbx.data = self.dbx.data.dropna()
 
     def rename_columns(self) -> None:
         print('renaming columns')
         self.dbx.data = self.dbx.data.rename(columns={'new_column': 'blue_column'})
 
-        
+
 class SaveData(DataRailsStep):
-        
+
     def step_save_data(self) -> None:
         print('saving data')
         self.dbx.data.to_csv('new_data.csv')
 
 
 # gather your steps in a list of class definitions. The class instances will be created by the step runner
 # while the jobs is being executed.
 steps = [
     LoadDataFromCSV,
     TransformData,
     SaveData
-]        
+]
 
 # pass your steps to the step runner
-runner = StepRunner(steps=steps)
+runner = DataRailsStepRunner(steps=steps)
 
 # Run the job. The steps will be run in the order they are defined in the list. Each method declared in a step will be
 # executed in the order they are defined in the class.
 
 if __name__ == '__main__':
-    runner.run() 
+    runner.run()
 
 ```
 
 ## Why Use DataRails?
 
 `datarails` is intended to solve a few simple problems that I have encountered while working with small to medium sized etl scripts in python. It is a very
 simple framework for ETL job execution and nothing more. It is not a replacement for `airflow`, `luigi`, `dagster` or any other workflow management tool, but rather
```

### Comparing `datarails-0.2.7/README.md` & `datarails-0.3.0/datarails.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,19 @@
+Metadata-Version: 2.1
+Name: datarails
+Version: 0.3.0
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: docs
+
+[![Release python package](https://github.com/JesseMaitland/datarails/actions/workflows/release.yml/badge.svg)](https://github.com/JesseMaitland/datarails/actions/workflows/release.yml)
 # datarails -- A Simple Framework for Dataframe ETL
-####  -- VERSION 0.2.7 --
+####  -- VERSION 0.3.0 --
+
 
 ## Official Documentation
 The official documentation is hosted on github pages at [jesse.maitland.github.io](https://jessemaitland.github.io/datarails/)
 
 ## Example Project
 There is an example repo containing some simple ETL jobs, notebooks and commands for building documentation at [jessemaitland/datarails-example](https://github.com/JesseMaitland/datarails_examples)
 
@@ -17,63 +27,63 @@
 Each step has access to a `DataBox` object that can be used to store dataframes and access them by name in downstream steps.
 
 In addition to the `DataBox` object, each step has access to a `DataRailsContext` object that can be used to store and access variables that are not dataframes.
 
 ```python
 import pandas as pd
 from datarails.step import DataRailsStep
-from datarails.runner import StepRunner
+from datarails.runner import DataRailsStepRunner
 
 
 class LoadDataFromCSV(DataRailsStep):
-    
+
     def step_load_csv(self) -> None:
         print('loading data from csv')
         df = pd.read_csv('data.csv')
-        self.dbx.put_df('data', df) # dbx now has an attribute called data that is a dataframe
+        self.dbx.put_df('data', df)  # dbx now has an attribute called data that is a dataframe
 
 
 class TransformData(DataRailsStep):
-    
+
     def step_add_new_column(self) -> None:
         print('adding new column')
         self.dbx.data['new_column'] = self.dbx.data['old_column'] * 2
-    
+
     def step_drop_all_null_rows(self) -> None:
         print('dropping null rows')
         self.dbx.data = self.dbx.data.dropna()
 
     def rename_columns(self) -> None:
         print('renaming columns')
         self.dbx.data = self.dbx.data.rename(columns={'new_column': 'blue_column'})
 
-        
+
 class SaveData(DataRailsStep):
-        
+
     def step_save_data(self) -> None:
         print('saving data')
         self.dbx.data.to_csv('new_data.csv')
 
 
 # gather your steps in a list of class definitions. The class instances will be created by the step runner
 # while the jobs is being executed.
 steps = [
     LoadDataFromCSV,
     TransformData,
     SaveData
-]        
+]
 
 # pass your steps to the step runner
-runner = StepRunner(steps=steps)
+runner = DataRailsStepRunner(steps=steps)
 
 # Run the job. The steps will be run in the order they are defined in the list. Each method declared in a step will be
 # executed in the order they are defined in the class.
 
 if __name__ == '__main__':
-    runner.run() 
+    runner.run()
 
 ```
 
 ## Why Use DataRails?
 
 `datarails` is intended to solve a few simple problems that I have encountered while working with small to medium sized etl scripts in python. It is a very
 simple framework for ETL job execution and nothing more. It is not a replacement for `airflow`, `luigi`, `dagster` or any other workflow management tool, but rather
```

### Comparing `datarails-0.2.7/datarails/contexts.py` & `datarails-0.3.0/datarails/contexts.py`

 * *Files identical despite different names*

### Comparing `datarails-0.2.7/datarails.egg-info/PKG-INFO` & `datarails-0.3.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,11 @@
-Metadata-Version: 2.1
-Name: datarails
-Version: 0.2.7
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: docs
-
+[![Release python package](https://github.com/JesseMaitland/datarails/actions/workflows/release.yml/badge.svg)](https://github.com/JesseMaitland/datarails/actions/workflows/release.yml)
 # datarails -- A Simple Framework for Dataframe ETL
-####  -- VERSION 0.2.7 --
+####  -- VERSION 0.3.0 --
+
 
 ## Official Documentation
 The official documentation is hosted on github pages at [jesse.maitland.github.io](https://jessemaitland.github.io/datarails/)
 
 ## Example Project
 There is an example repo containing some simple ETL jobs, notebooks and commands for building documentation at [jessemaitland/datarails-example](https://github.com/JesseMaitland/datarails_examples)
 
@@ -25,63 +19,63 @@
 Each step has access to a `DataBox` object that can be used to store dataframes and access them by name in downstream steps.
 
 In addition to the `DataBox` object, each step has access to a `DataRailsContext` object that can be used to store and access variables that are not dataframes.
 
 ```python
 import pandas as pd
 from datarails.step import DataRailsStep
-from datarails.runner import StepRunner
+from datarails.runner import DataRailsStepRunner
 
 
 class LoadDataFromCSV(DataRailsStep):
-    
+
     def step_load_csv(self) -> None:
         print('loading data from csv')
         df = pd.read_csv('data.csv')
-        self.dbx.put_df('data', df) # dbx now has an attribute called data that is a dataframe
+        self.dbx.put_df('data', df)  # dbx now has an attribute called data that is a dataframe
 
 
 class TransformData(DataRailsStep):
-    
+
     def step_add_new_column(self) -> None:
         print('adding new column')
         self.dbx.data['new_column'] = self.dbx.data['old_column'] * 2
-    
+
     def step_drop_all_null_rows(self) -> None:
         print('dropping null rows')
         self.dbx.data = self.dbx.data.dropna()
 
     def rename_columns(self) -> None:
         print('renaming columns')
         self.dbx.data = self.dbx.data.rename(columns={'new_column': 'blue_column'})
 
-        
+
 class SaveData(DataRailsStep):
-        
+
     def step_save_data(self) -> None:
         print('saving data')
         self.dbx.data.to_csv('new_data.csv')
 
 
 # gather your steps in a list of class definitions. The class instances will be created by the step runner
 # while the jobs is being executed.
 steps = [
     LoadDataFromCSV,
     TransformData,
     SaveData
-]        
+]
 
 # pass your steps to the step runner
-runner = StepRunner(steps=steps)
+runner = DataRailsStepRunner(steps=steps)
 
 # Run the job. The steps will be run in the order they are defined in the list. Each method declared in a step will be
 # executed in the order they are defined in the class.
 
 if __name__ == '__main__':
-    runner.run() 
+    runner.run()
 
 ```
 
 ## Why Use DataRails?
 
 `datarails` is intended to solve a few simple problems that I have encountered while working with small to medium sized etl scripts in python. It is a very
 simple framework for ETL job execution and nothing more. It is not a replacement for `airflow`, `luigi`, `dagster` or any other workflow management tool, but rather
```

### Comparing `datarails-0.2.7/pyproject.toml` & `datarails-0.3.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "datarails"
-version = "0.2.7"
+version = "0.3.0"
 description = ""
 readme = "README.md"
 requires-python = ">=3.9"
 
 
 [project.optional-dependencies]
 dev = [
```

### Comparing `datarails-0.2.7/tests/test_context.py` & `datarails-0.3.0/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `datarails-0.2.7/tests/test_databox.py` & `datarails-0.3.0/tests/test_databox.py`

 * *Files identical despite different names*

### Comparing `datarails-0.2.7/tests/test_runner.py` & `datarails-0.3.0/tests/test_runner.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,50 +1,72 @@
 import pytest
 
 from datarails.contexts import DataBox
-from datarails.runner import (
-    StepRunner,  # Replace with actual module where StepRunner is defined
-)
+from datarails.runner import DataRailsStepRunner
 from datarails.step import DataRailsStep
 
 
 class MockStep(DataRailsStep):
     def step_one(self):
         pass
 
     def step_two(self):
         pass
 
 
+class MockAnotherStep(DataRailsStep):
+    def step_one(self):
+        pass
+
+    def step_two(self):
+        pass
+
+
 @pytest.fixture
 def test_runner_instance():
-    steps = [MockStep, MockStep]
-    return StepRunner(steps)
+    steps = [MockStep, MockAnotherStep]
+    return DataRailsStepRunner(steps)
 
 
 def test_constructor(test_runner_instance):
     assert isinstance(test_runner_instance.dbx, DataBox)
-    assert isinstance(test_runner_instance.steps_iterator, type(iter([])))
+    assert isinstance(test_runner_instance._i, int)
+    assert test_runner_instance._i == 0
     assert len(test_runner_instance.steps) == 2
 
 
 def test_reset(test_runner_instance):
-    iterator_before = test_runner_instance.steps_iterator
+    test_runner_instance._i = 1  # Modify the iterator index
     test_runner_instance.reset()
-    iterator_after = test_runner_instance.steps_iterator
-    assert iterator_before is not iterator_after
+    assert test_runner_instance._i == 0  # Iterator index should be reset to 0
 
 
-def test_advance(test_runner_instance):
-
-    # Test that advance raises StopIteration when no more steps
+def test_advance(test_runner_instance, capsys):
+    # Test that advance increments the _i attribute
     test_runner_instance.reset()
+    assert test_runner_instance._i == 0
     test_runner_instance.advance()  # Run first step
-    test_runner_instance.advance()  # Run second step
-    with pytest.raises(StopIteration):
-        test_runner_instance.advance(stepper=False)  # Should raise StopIteration
+    assert test_runner_instance._i == 1
 
+    # Test that advance prints "Running step: 0 : StepInstance" after first step
+    captured = capsys.readouterr()
+    assert "Running step: 0 : MockStep" in captured.out
+
+    # Test that advance prints "Running step: 1 : StepInstance" after second step
+    test_runner_instance.advance()  # Run second step
+    captured = capsys.readouterr()
+    assert "Running step: 1 : MockAnotherStep" in captured.out
 
-def test_run(test_runner_instance, capsys):
-    test_runner_instance.run()
+    # Test that advance prints "All Steps Completed." when no more steps
+    test_runner_instance.advance()  # Should print "All Steps Completed."
     captured = capsys.readouterr()
-    assert "No more steps to execute. Reset and try again." in captured.out
+    assert "All Steps Completed." in captured.out
+
+
+def test_get_current_step(test_runner_instance):
+    test_runner_instance.reset()
+    current_step = test_runner_instance.get_current_step()
+    assert isinstance(current_step, MockStep)
+
+    test_runner_instance.advance()
+    current_step = test_runner_instance.get_current_step()
+    assert isinstance(current_step, MockAnotherStep)
```

