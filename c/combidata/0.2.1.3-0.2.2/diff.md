# Comparing `tmp/combidata-0.2.1.3.tar.gz` & `tmp/combidata-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "combidata-0.2.1.3.tar", last modified: Fri Jul  7 17:26:10 2023, max compression
+gzip compressed data, was "combidata-0.2.2.tar", last modified: Sun Jul 30 14:50:50 2023, max compression
```

## Comparing `combidata-0.2.1.3.tar` & `combidata-0.2.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 17:26:10.940743 combidata-0.2.1.3/
--rw-rw-rw-   0        0        0     1083 2022-11-07 15:57:18.000000 combidata-0.2.1.3/LICENSE
--rw-rw-rw-   0        0        0    10467 2023-07-07 17:26:10.939745 combidata-0.2.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     9684 2023-06-30 14:16:48.000000 combidata-0.2.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-07 17:26:10.903745 combidata-0.2.1.3/combidata/
--rw-rw-rw-   0        0        0      395 2023-02-10 13:56:29.000000 combidata-0.2.1.3/combidata/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-07 17:26:10.931744 combidata-0.2.1.3/combidata/classes/
--rw-rw-rw-   0        0        0        0 2023-02-03 08:57:32.000000 combidata-0.2.1.3/combidata/classes/__init__.py
--rw-rw-rw-   0        0        0     2831 2023-04-01 06:03:08.000000 combidata-0.2.1.3/combidata/classes/case.py
--rw-rw-rw-   0        0        0     3071 2023-07-07 15:54:44.000000 combidata-0.2.1.3/combidata/classes/combination.py
--rw-rw-rw-   0        0        0     6255 2023-06-30 14:01:33.000000 combidata-0.2.1.3/combidata/classes/data_generator.py
--rw-rw-rw-   0        0        0      351 2023-03-02 16:58:22.000000 combidata-0.2.1.3/combidata/classes/process.py
-drwxrwxrwx   0        0        0        0 2023-07-07 17:26:10.936748 combidata-0.2.1.3/combidata/processes/
--rw-rw-rw-   0        0        0        0 2023-02-03 08:57:32.000000 combidata-0.2.1.3/combidata/processes/__init__.py
--rw-rw-rw-   0        0        0     5249 2023-04-01 05:47:28.000000 combidata-0.2.1.3/combidata/processes/combine.py
--rw-rw-rw-   0        0        0      655 2023-02-16 18:09:16.000000 combidata-0.2.1.3/combidata/processes/form.py
--rw-rw-rw-   0        0        0     1924 2023-04-01 06:30:40.000000 combidata-0.2.1.3/combidata/processes/genetate.py
-drwxrwxrwx   0        0        0        0 2023-07-07 17:26:10.924744 combidata-0.2.1.3/combidata.egg-info/
--rw-rw-rw-   0        0        0    10467 2023-07-07 17:26:10.000000 combidata-0.2.1.3/combidata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      496 2023-07-07 17:26:10.000000 combidata-0.2.1.3/combidata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 17:26:10.000000 combidata-0.2.1.3/combidata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-07 17:26:10.000000 combidata-0.2.1.3/combidata.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      555 2023-07-07 17:22:34.000000 combidata-0.2.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-07 17:26:10.940743 combidata-0.2.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1075 2023-07-07 17:22:34.000000 combidata-0.2.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-07 17:26:10.938744 combidata-0.2.1.3/tests/
--rw-rw-rw-   0        0        0     3511 2023-06-30 13:59:13.000000 combidata-0.2.1.3/tests/test_generator.py
+drwxrwxrwx   0        0        0        0 2023-07-30 14:50:50.320017 combidata-0.2.2/
+-rw-rw-rw-   0        0        0     1083 2022-11-07 15:57:18.000000 combidata-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0    10603 2023-07-30 14:50:50.319014 combidata-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     9822 2023-07-30 14:49:48.000000 combidata-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-30 14:50:50.218012 combidata-0.2.2/combidata/
+-rw-rw-rw-   0        0        0      395 2023-02-10 13:56:29.000000 combidata-0.2.2/combidata/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-30 14:50:50.276017 combidata-0.2.2/combidata/classes/
+-rw-rw-rw-   0        0        0        0 2023-02-03 08:57:32.000000 combidata-0.2.2/combidata/classes/__init__.py
+-rw-rw-rw-   0        0        0     2835 2023-07-29 20:41:49.000000 combidata-0.2.2/combidata/classes/case.py
+-rw-rw-rw-   0        0        0     3107 2023-07-30 08:57:21.000000 combidata-0.2.2/combidata/classes/combination.py
+-rw-rw-rw-   0        0        0    11849 2023-07-30 14:42:10.000000 combidata-0.2.2/combidata/classes/data_generator.py
+-rw-rw-rw-   0        0        0      351 2023-03-02 16:58:22.000000 combidata-0.2.2/combidata/classes/process.py
+drwxrwxrwx   0        0        0        0 2023-07-30 14:50:50.305014 combidata-0.2.2/combidata/processes/
+-rw-rw-rw-   0        0        0        0 2023-02-03 08:57:32.000000 combidata-0.2.2/combidata/processes/__init__.py
+-rw-rw-rw-   0        0        0     3516 2023-07-30 10:12:58.000000 combidata-0.2.2/combidata/processes/combine.py
+-rw-rw-rw-   0        0        0      655 2023-02-16 18:09:16.000000 combidata-0.2.2/combidata/processes/form.py
+-rw-rw-rw-   0        0        0     1924 2023-04-01 06:30:40.000000 combidata-0.2.2/combidata/processes/genetate.py
+drwxrwxrwx   0        0        0        0 2023-07-30 14:50:50.247015 combidata-0.2.2/combidata.egg-info/
+-rw-rw-rw-   0        0        0    10603 2023-07-30 14:50:50.000000 combidata-0.2.2/combidata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      496 2023-07-30 14:50:50.000000 combidata-0.2.2/combidata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 14:50:50.000000 combidata-0.2.2/combidata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-30 14:50:50.000000 combidata-0.2.2/combidata.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      553 2023-07-30 14:49:48.000000 combidata-0.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-30 14:50:50.321017 combidata-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1073 2023-07-30 14:49:48.000000 combidata-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 14:50:50.318015 combidata-0.2.2/tests/
+-rw-rw-rw-   0        0        0     3511 2023-06-30 13:59:13.000000 combidata-0.2.2/tests/test_generator.py
```

### Comparing `combidata-0.2.1.3/LICENSE` & `combidata-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `combidata-0.2.1.3/PKG-INFO` & `combidata-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: combidata
-Version: 0.2.1.3
+Version: 0.2.2
 Summary: Package for random data generation, combination and data prepare for tests
 Home-page: https://github.com/Warrfie/combidata
 Author: Kuklikov Maxim (Warrfie)
 Author-email: "MaximKuklikov(Warrfie)" <warrfie@gmail.com>
 Project-URL: Homepage, https://github.com/Warrfie/combidata
 Keywords: QA,SET,random data generation,testing API,testing,autotesting
 Classifier: Development Status :: 4 - Beta
@@ -27,14 +27,18 @@
 
 
 The core functionality of the Combidata library is provided by the `DataGenerator` class, which takes in test flags and a dictionary containing all cases, forms, and workflows. 
 The `DataGenerator` creates `Combination` instances from the possible cases. 
 The `run` function in each `Combination` instance processes all steps in the specified workflow.
 
 ## New features
+0.2.2:
+1) All combination problems was fixed by multidimensional graph (I will optimize algorithm in next realises)
+2) Added logger 
+
 0.2.1:
 1) So, we have greate problem with possible_modes and other parameters. I patched it but problem still here.
 2) Added logger begin
 3) And also fix bug with 'STOP' signal
 
 0.2.0:
 1) Ok, now its Beta ;)
```

### Comparing `combidata-0.2.1.3/README.md` & `combidata-0.2.2/combidata.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: combidata
+Version: 0.2.2
+Summary: Package for random data generation, combination and data prepare for tests
+Home-page: https://github.com/Warrfie/combidata
+Author: Kuklikov Maxim (Warrfie)
+Author-email: "MaximKuklikov(Warrfie)" <warrfie@gmail.com>
+Project-URL: Homepage, https://github.com/Warrfie/combidata
+Keywords: QA,SET,random data generation,testing API,testing,autotesting
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Information Technology
+Classifier: Topic :: Software Development :: Quality Assurance
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.10, <4
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![PyPi Package Version](https://img.shields.io/pypi/v/combidata.svg)](https://pypi.python.org/pypi/combidata)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/combidata.svg)](https://pypi.python.org/pypi/combidata)
 [![PyPi status](https://img.shields.io/pypi/status/combidata.svg?style=flat-square)](https://pypi.python.org/pypi/combidata)
 
 # <p align="center">Combidata
 
 Combidata is a flexible and powerful Python library designed for generating various combinations of test data based on defined cases and rules. 
@@ -9,14 +27,18 @@
 
 
 The core functionality of the Combidata library is provided by the `DataGenerator` class, which takes in test flags and a dictionary containing all cases, forms, and workflows. 
 The `DataGenerator` creates `Combination` instances from the possible cases. 
 The `run` function in each `Combination` instance processes all steps in the specified workflow.
 
 ## New features
+0.2.2:
+1) All combination problems was fixed by multidimensional graph (I will optimize algorithm in next realises)
+2) Added logger 
+
 0.2.1:
 1) So, we have greate problem with possible_modes and other parameters. I patched it but problem still here.
 2) Added logger begin
 3) And also fix bug with 'STOP' signal
 
 0.2.0:
 1) Ok, now its Beta ;)
@@ -286,8 +308,8 @@
 
 ## Acknowledgments
 A special thanks to the community for their support, contributions, and valuable feedback. Your input helps make Combidata a better tool for everyone! And a special thanks to JetBrains for their best software and License for Open Source Development.
 
 
 [![JetBrains Black Box Logo logo](https://resources.jetbrains.com/storage/products/company/brand/logos/jb_square.png)](https://jb.gg/OpenSourceSupport)
 
-With Combidata, you can easily generate test data for your applications and systems, ensuring that they are robust and reliable under various conditions. Start using Combidata today to improve the quality of your testing and development process!
+With Combidata, you can easily generate test data for your applications and systems, ensuring that they are robust and reliable under various conditions. Start using Combidata today to improve the quality of your testing and development process!
```

### Comparing `combidata-0.2.1.3/combidata/classes/case.py` & `combidata-0.2.2/combidata/classes/case.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,21 +33,21 @@
     def __init__(self, case: dict, field_name: str, field_mode: str):
         # TODO add additional checks
         self.field_name = field_name
         self.field_mode = field_mode
         self.case_name = case["name"]
 
         self.value = case.get("value", None)
-        self.type_of_case = case.get("type", None)
+        self.type_of_case = case.get("type", "standard")
         self.gen_func = case.get("gen_func", None)
         self.is_presented = case.get("is_presented", True)
         self.options = case.get("options", None)
 
         if "requirements" not in case.keys():
-            self.requirements = None
+            self.requirements = {}
         else:
             self.hand_requirements(case["requirements"])
 
         self.additional_fields = self.form_additional_fields(case)
```

### Comparing `combidata-0.2.1.3/combidata/classes/combination.py` & `combidata-0.2.2/combidata/classes/combination.py`

 * *Files 20% similar despite different names*

```diff
@@ -33,48 +33,50 @@
 
     """
     test_seed = None
     formed_data = None
 
     step_done = None  # last passed step
 
-    def __init__(self, case, workflow, init_lib, template, tools):
+    def __init__(self, case, workflow, init_lib, template, tools, logger, generator_id):
         self.init_lib = init_lib
         self.main_case = case
         self.template = template
         self.tools = tools
+        self.logger = logger
+        self.generator_id = generator_id
 
         self.generated_data = {}
         self.other_cases = {}
 
         self.cache = {}
 
         self.workflow = workflow
 
     def run(self):
         self.workflow = list(self.workflow) if isinstance(self.workflow, list) else self.workflow  # todo beautify
         workflow = self.workflow.pop(0) if isinstance(self.workflow, list) else self.workflow
         for current_step in workflow:
             while step_not_done(current_step.name, self):
                 if self.step_done != current_step.name:
-                    if start_step := self.tools.get("start_step"):
-                        start_step(self.tools.get("id"), current_step.name)
+                    if self.logger:
+                        self.logger.start_step(self.generator_id, current_step.name)
                     try:
                         current_step.activate(self)
                     except Exception as e:
                         self.step_done = "STOP"
-                        if end_step := self.tools.get("end_step"):
+                        if self.logger:
                             temp_exep = f"An exception occurred: {type(e).__name__}. "
                             temp_exep += f"Error message: {str(e)}. "
                             traceback_list = traceback.extract_tb(e.__traceback__)
                             if traceback_list:
                                 last_traceback = traceback_list[-1]
                                 file_name = last_traceback.filename
                                 line_number = last_traceback.lineno
                                 temp_exep += f"Occurred at: {file_name}:{line_number}. "
-                            end_step(self.tools.get("id"), temp_exep)
+                            self.logger.end_step(self.generator_id, temp_exep)
                         else:
                             raise e
                     else:
-                        if end_step := self.tools.get("end_step"):
-                            end_step(self.tools.get("id"))
+                        if self.logger:
+                            self.logger.end_step(self.generator_id)
```

### Comparing `combidata-0.2.1.3/combidata/processes/form.py` & `combidata-0.2.2/combidata/processes/form.py`

 * *Files identical despite different names*

### Comparing `combidata-0.2.1.3/combidata/processes/genetate.py` & `combidata-0.2.2/combidata/processes/genetate.py`

 * *Files identical despite different names*

### Comparing `combidata-0.2.1.3/combidata.egg-info/PKG-INFO` & `combidata-0.2.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: combidata
-Version: 0.2.1.3
-Summary: Package for random data generation, combination and data prepare for tests
-Home-page: https://github.com/Warrfie/combidata
-Author: Kuklikov Maxim (Warrfie)
-Author-email: "MaximKuklikov(Warrfie)" <warrfie@gmail.com>
-Project-URL: Homepage, https://github.com/Warrfie/combidata
-Keywords: QA,SET,random data generation,testing API,testing,autotesting
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Information Technology
-Classifier: Topic :: Software Development :: Quality Assurance
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10, <4
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![PyPi Package Version](https://img.shields.io/pypi/v/combidata.svg)](https://pypi.python.org/pypi/combidata)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/combidata.svg)](https://pypi.python.org/pypi/combidata)
 [![PyPi status](https://img.shields.io/pypi/status/combidata.svg?style=flat-square)](https://pypi.python.org/pypi/combidata)
 
 # <p align="center">Combidata
 
 Combidata is a flexible and powerful Python library designed for generating various combinations of test data based on defined cases and rules. 
@@ -27,14 +9,18 @@
 
 
 The core functionality of the Combidata library is provided by the `DataGenerator` class, which takes in test flags and a dictionary containing all cases, forms, and workflows. 
 The `DataGenerator` creates `Combination` instances from the possible cases. 
 The `run` function in each `Combination` instance processes all steps in the specified workflow.
 
 ## New features
+0.2.2:
+1) All combination problems was fixed by multidimensional graph (I will optimize algorithm in next realises)
+2) Added logger 
+
 0.2.1:
 1) So, we have greate problem with possible_modes and other parameters. I patched it but problem still here.
 2) Added logger begin
 3) And also fix bug with 'STOP' signal
 
 0.2.0:
 1) Ok, now its Beta ;)
@@ -304,8 +290,8 @@
 
 ## Acknowledgments
 A special thanks to the community for their support, contributions, and valuable feedback. Your input helps make Combidata a better tool for everyone! And a special thanks to JetBrains for their best software and License for Open Source Development.
 
 
 [![JetBrains Black Box Logo logo](https://resources.jetbrains.com/storage/products/company/brand/logos/jb_square.png)](https://jb.gg/OpenSourceSupport)
 
-With Combidata, you can easily generate test data for your applications and systems, ensuring that they are robust and reliable under various conditions. Start using Combidata today to improve the quality of your testing and development process!
+With Combidata, you can easily generate test data for your applications and systems, ensuring that they are robust and reliable under various conditions. Start using Combidata today to improve the quality of your testing and development process!
```

### Comparing `combidata-0.2.1.3/pyproject.toml` & `combidata-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -13,8 +13,8 @@
     "testing API",
     "testing",
     "autotesting"
 ]
 urls = {Homepage = "https://github.com/Warrfie/combidata"}
 authors = [{name = "MaximKuklikov(Warrfie)", email = "warrfie@gmail.com"}]
 requires-python = ">=3.10"
-version="0.2.1.3"
+version="0.2.2"
```

### Comparing `combidata-0.2.1.3/setup.py` & `combidata-0.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 
 setup(
     name="combidata",
-    version="0.2.1.3",
+    version="0.2.2",
     description="Package for random data generation and combination different cases",
     long_description=long_description,
     url="https://github.com/Warrfie/combidata",
     author="Kuklikov Maxim (Warrfie)",
     author_email="warrfie@gmail.com",
     classifiers=[
         "Development Status :: 4 - Beta",
```

### Comparing `combidata-0.2.1.3/tests/test_generator.py` & `combidata-0.2.2/tests/test_generator.py`

 * *Files identical despite different names*

