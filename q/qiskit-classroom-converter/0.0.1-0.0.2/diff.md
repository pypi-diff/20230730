# Comparing `tmp/qiskit-classroom-converter-0.0.1.tar.gz` & `tmp/qiskit-classroom-converter-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit-classroom-converter-0.0.1.tar", last modified: Fri Jul 28 06:14:54 2023, max compression
+gzip compressed data, was "qiskit-classroom-converter-0.0.2.tar", last modified: Sun Jul 30 00:20:44 2023, max compression
```

## Comparing `qiskit-classroom-converter-0.0.1.tar` & `qiskit-classroom-converter-0.0.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-07-28 06:14:54.475848 qiskit-classroom-converter-0.0.1/
--rw-r--r--   0 minwook-shin   (501) staff       (20)    11350 2023-07-28 05:38:56.000000 qiskit-classroom-converter-0.0.1/LICENSE
--rw-r--r--   0 minwook-shin   (501) staff       (20)       24 2023-06-25 02:07:36.000000 qiskit-classroom-converter-0.0.1/MANIFEST.in
--rw-r--r--   0 minwook-shin   (501) staff       (20)     2455 2023-07-28 06:14:54.476022 qiskit-classroom-converter-0.0.1/PKG-INFO
--rw-r--r--   0 minwook-shin   (501) staff       (20)     1848 2023-07-28 05:39:05.000000 qiskit-classroom-converter-0.0.1/README.md
--rw-r--r--   0 minwook-shin   (501) staff       (20)      951 2023-07-28 05:38:56.000000 qiskit-classroom-converter-0.0.1/pyproject.toml
-drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-07-28 06:14:54.464255 qiskit-classroom-converter-0.0.1/qiskit_class_converter/
--rw-r--r--   0 minwook-shin   (501) staff       (20)     1649 2023-07-28 06:11:36.000000 qiskit-classroom-converter-0.0.1/qiskit_class_converter/__init__.py
-drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-07-28 06:14:54.468917 qiskit-classroom-converter-0.0.1/qiskit_class_converter/converters/
--rw-r--r--   0 minwook-shin   (501) staff       (20)        0 2023-05-26 12:59:36.000000 qiskit-classroom-converter-0.0.1/qiskit_class_converter/converters/__init__.py
--rw-r--r--   0 minwook-shin   (501) staff       (20)     1629 2023-07-28 05:38:56.000000 qiskit-classroom-converter-0.0.1/qiskit_class_converter/converters/base.py
--rw-r--r--   0 minwook-shin   (501) staff       (20)     3710 2023-07-28 05:39:05.000000 qiskit-classroom-converter-0.0.1/qiskit_class_converter/converters/braket_notation_to_matrix.py
--rw-r--r--   0 minwook-shin   (501) staff       (20)     1401 2023-07-28 05:39:05.000000 qiskit-classroom-converter-0.0.1/qiskit_class_converter/converters/matrix_to_quantum_circuit.py
--rw-r--r--   0 minwook-shin   (501) staff       (20)     2440 2023-07-28 05:38:56.000000 qiskit-classroom-converter-0.0.1/qiskit_class_converter/converters/quantum_circuit_to_braket_notation.py
--rw-r--r--   0 minwook-shin   (501) staff       (20)     1526 2023-07-28 05:38:56.000000 qiskit-classroom-converter-0.0.1/qiskit_class_converter/converters/quantum_circuit_to_matrix.py
-drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-07-28 06:14:54.470583 qiskit-classroom-converter-0.0.1/qiskit_class_converter/services/
--rw-r--r--   0 minwook-shin   (501) staff       (20)        0 2023-05-26 12:59:36.000000 qiskit-classroom-converter-0.0.1/qiskit_class_converter/services/__init__.py
--rw-r--r--   0 minwook-shin   (501) staff       (20)     4325 2023-07-28 06:11:36.000000 qiskit-classroom-converter-0.0.1/qiskit_class_converter/services/converter_service.py
-drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-07-28 06:14:54.473835 qiskit-classroom-converter-0.0.1/qiskit_classroom_converter.egg-info/
--rw-r--r--   0 minwook-shin   (501) staff       (20)     2455 2023-07-28 06:14:54.000000 qiskit-classroom-converter-0.0.1/qiskit_classroom_converter.egg-info/PKG-INFO
--rw-r--r--   0 minwook-shin   (501) staff       (20)      861 2023-07-28 06:14:54.000000 qiskit-classroom-converter-0.0.1/qiskit_classroom_converter.egg-info/SOURCES.txt
--rw-r--r--   0 minwook-shin   (501) staff       (20)        1 2023-07-28 06:14:54.000000 qiskit-classroom-converter-0.0.1/qiskit_classroom_converter.egg-info/dependency_links.txt
--rw-r--r--   0 minwook-shin   (501) staff       (20)      165 2023-07-28 06:14:54.000000 qiskit-classroom-converter-0.0.1/qiskit_classroom_converter.egg-info/requires.txt
--rw-r--r--   0 minwook-shin   (501) staff       (20)       23 2023-07-28 06:14:54.000000 qiskit-classroom-converter-0.0.1/qiskit_classroom_converter.egg-info/top_level.txt
--rw-r--r--   0 minwook-shin   (501) staff       (20)       69 2023-06-30 23:31:50.000000 qiskit-classroom-converter-0.0.1/requirements.txt
--rw-r--r--   0 minwook-shin   (501) staff       (20)       79 2023-07-28 06:14:54.476610 qiskit-classroom-converter-0.0.1/setup.cfg
-drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-07-28 06:14:54.475122 qiskit-classroom-converter-0.0.1/tests/
--rw-r--r--   0 minwook-shin   (501) staff       (20)     3812 2023-07-28 06:03:19.000000 qiskit-classroom-converter-0.0.1/tests/test_convert_class.py
--rw-r--r--   0 minwook-shin   (501) staff       (20)     5698 2023-07-28 06:03:19.000000 qiskit-classroom-converter-0.0.1/tests/test_converter_service.py
+drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-07-30 00:20:44.058942 qiskit-classroom-converter-0.0.2/
+-rw-r--r--   0 minwook-shin   (501) staff       (20)    11350 2023-07-28 05:38:56.000000 qiskit-classroom-converter-0.0.2/LICENSE
+-rw-r--r--   0 minwook-shin   (501) staff       (20)       24 2023-06-25 02:07:36.000000 qiskit-classroom-converter-0.0.2/MANIFEST.in
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     2565 2023-07-30 00:20:44.059136 qiskit-classroom-converter-0.0.2/PKG-INFO
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     1958 2023-07-28 06:54:58.000000 qiskit-classroom-converter-0.0.2/README.md
+-rw-r--r--   0 minwook-shin   (501) staff       (20)      951 2023-07-30 00:19:08.000000 qiskit-classroom-converter-0.0.2/pyproject.toml
+drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-07-30 00:20:44.048997 qiskit-classroom-converter-0.0.2/qiskit_class_converter/
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     1653 2023-07-28 06:43:21.000000 qiskit-classroom-converter-0.0.2/qiskit_class_converter/__init__.py
+drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-07-30 00:20:44.053207 qiskit-classroom-converter-0.0.2/qiskit_class_converter/converters/
+-rw-r--r--   0 minwook-shin   (501) staff       (20)        0 2023-05-26 12:59:36.000000 qiskit-classroom-converter-0.0.2/qiskit_class_converter/converters/__init__.py
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     1629 2023-07-28 05:38:56.000000 qiskit-classroom-converter-0.0.2/qiskit_class_converter/converters/base.py
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     3710 2023-07-28 05:39:05.000000 qiskit-classroom-converter-0.0.2/qiskit_class_converter/converters/braket_notation_to_matrix.py
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     1409 2023-07-28 06:43:21.000000 qiskit-classroom-converter-0.0.2/qiskit_class_converter/converters/matrix_to_quantum_circuit.py
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     2440 2023-07-28 05:38:56.000000 qiskit-classroom-converter-0.0.2/qiskit_class_converter/converters/quantum_circuit_to_braket_notation.py
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     1526 2023-07-28 05:38:56.000000 qiskit-classroom-converter-0.0.2/qiskit_class_converter/converters/quantum_circuit_to_matrix.py
+drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-07-30 00:20:44.054452 qiskit-classroom-converter-0.0.2/qiskit_class_converter/services/
+-rw-r--r--   0 minwook-shin   (501) staff       (20)        0 2023-05-26 12:59:36.000000 qiskit-classroom-converter-0.0.2/qiskit_class_converter/services/__init__.py
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     4310 2023-07-28 06:43:21.000000 qiskit-classroom-converter-0.0.2/qiskit_class_converter/services/converter_service.py
+drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-07-30 00:20:44.057050 qiskit-classroom-converter-0.0.2/qiskit_classroom_converter.egg-info/
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     2565 2023-07-30 00:20:44.000000 qiskit-classroom-converter-0.0.2/qiskit_classroom_converter.egg-info/PKG-INFO
+-rw-r--r--   0 minwook-shin   (501) staff       (20)      861 2023-07-30 00:20:44.000000 qiskit-classroom-converter-0.0.2/qiskit_classroom_converter.egg-info/SOURCES.txt
+-rw-r--r--   0 minwook-shin   (501) staff       (20)        1 2023-07-30 00:20:44.000000 qiskit-classroom-converter-0.0.2/qiskit_classroom_converter.egg-info/dependency_links.txt
+-rw-r--r--   0 minwook-shin   (501) staff       (20)      165 2023-07-30 00:20:44.000000 qiskit-classroom-converter-0.0.2/qiskit_classroom_converter.egg-info/requires.txt
+-rw-r--r--   0 minwook-shin   (501) staff       (20)       23 2023-07-30 00:20:44.000000 qiskit-classroom-converter-0.0.2/qiskit_classroom_converter.egg-info/top_level.txt
+-rw-r--r--   0 minwook-shin   (501) staff       (20)       88 2023-07-30 00:19:08.000000 qiskit-classroom-converter-0.0.2/requirements.txt
+-rw-r--r--   0 minwook-shin   (501) staff       (20)       79 2023-07-30 00:20:44.059740 qiskit-classroom-converter-0.0.2/setup.cfg
+drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-07-30 00:20:44.058252 qiskit-classroom-converter-0.0.2/tests/
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     3813 2023-07-28 06:43:21.000000 qiskit-classroom-converter-0.0.2/tests/test_convert_class.py
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     5698 2023-07-28 06:03:19.000000 qiskit-classroom-converter-0.0.2/tests/test_converter_service.py
```

### Comparing `qiskit-classroom-converter-0.0.1/LICENSE` & `qiskit-classroom-converter-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qiskit-classroom-converter-0.0.1/PKG-INFO` & `qiskit-classroom-converter-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-classroom-converter
-Version: 0.0.1
+Version: 0.0.2
 Summary: extend the Qiskit classroom applications.
 Author: KMU-quantum-classroom
 Project-URL: Homepage, https://github.com/KMU-quantum-classroom/qiskit-classroom-converter
 Project-URL: Bug Tracker, https://github.com/KMU-quantum-classroom/qiskit-classroom-converter/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -12,14 +12,18 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # qiskit-classroom-converter
 Qiskit classroom Converter
 
+## Documents
+
+https://kmu-quantum-classroom.github.io/qiskit-classroom-converter/qiskit_class_converter.html
+
 ## Support convert method
 
 * quantum circuit to bra-ket notation
 * quantum circuit to matrix
 * matrix to quantum circuit
 * bra-ket notation to matrix
```

### Comparing `qiskit-classroom-converter-0.0.1/README.md` & `qiskit-classroom-converter-0.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 # qiskit-classroom-converter
 Qiskit classroom Converter
 
+## Documents
+
+https://kmu-quantum-classroom.github.io/qiskit-classroom-converter/qiskit_class_converter.html
+
 ## Support convert method
 
 * quantum circuit to bra-ket notation
 * quantum circuit to matrix
 * matrix to quantum circuit
 * bra-ket notation to matrix
```

### Comparing `qiskit-classroom-converter-0.0.1/pyproject.toml` & `qiskit-classroom-converter-0.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 [build-system]
 requires = ["setuptools>=68.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qiskit-classroom-converter"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     { name = "KMU-quantum-classroom" },
 ]
 description = "extend the Qiskit classroom applications."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "qiskit==0.43.2",
+    "qiskit==0.44.0",
+    "qiskit-aer==0.12.2",
     "loguru==0.7.0",
     "sympy==1.12",
     "antlr4-python3-runtime==4.11"
 ]
 
 [project.optional-dependencies]
 dev = [
-    "qiskit-aer==0.12.1",
     "coverage==7.2.7",
-    "pylint==2.17.4",
-    "tox==4.6.3",
+    "pylint==2.17.5",
+    "tox==4.6.4",
     "build==0.10.0",
     "pdoc==14.0.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/KMU-quantum-classroom/qiskit-classroom-converter"
 "Bug Tracker" = "https://github.com/KMU-quantum-classroom/qiskit-classroom-converter/issues"
```

### Comparing `qiskit-classroom-converter-0.0.1/qiskit_class_converter/__init__.py` & `qiskit-classroom-converter-0.0.2/qiskit_class_converter/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,8 +41,8 @@
 #  "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 #  KIND, either express or implied.  See the License for the
 #  specific language governing permissions and limitations
 #  under the License.
 
 from .services.converter_service import ConversionService, ConversionType
 
-__all__ = [ConversionService, ConversionType]
+__all__ = ["ConversionService", "ConversionType"]
```

### Comparing `qiskit-classroom-converter-0.0.1/qiskit_class_converter/converters/base.py` & `qiskit-classroom-converter-0.0.2/qiskit_class_converter/converters/base.py`

 * *Files identical despite different names*

### Comparing `qiskit-classroom-converter-0.0.1/qiskit_class_converter/converters/braket_notation_to_matrix.py` & `qiskit-classroom-converter-0.0.2/qiskit_class_converter/converters/braket_notation_to_matrix.py`

 * *Files identical despite different names*

### Comparing `qiskit-classroom-converter-0.0.1/qiskit_class_converter/converters/matrix_to_quantum_circuit.py` & `qiskit-classroom-converter-0.0.2/qiskit_class_converter/converters/matrix_to_quantum_circuit.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,13 +24,14 @@
 class MatrixToQuantumCircuitConverter(BaseConverter):
     """
     Converter class
     """
 
     def actual_convert_action(self):
         self.logger.debug("matrix to quantum circuit")
-        gate = self.qiskit.extensions.UnitaryGate(self.input_value) # parse by unitary circuit. can't describe what circuit is.
+        gate = self.qiskit.extensions.UnitaryGate(self.input_value)
+        # parse by unitary circuit. can't describe what circuit is.
         if self.option.get("label", False):
             gate.label = self.option.get("label", "")
         else:
             gate.label = str(self.input_value)
         return gate
```

### Comparing `qiskit-classroom-converter-0.0.1/qiskit_class_converter/converters/quantum_circuit_to_braket_notation.py` & `qiskit-classroom-converter-0.0.2/qiskit_class_converter/converters/quantum_circuit_to_braket_notation.py`

 * *Files identical despite different names*

### Comparing `qiskit-classroom-converter-0.0.1/qiskit_class_converter/converters/quantum_circuit_to_matrix.py` & `qiskit-classroom-converter-0.0.2/qiskit_class_converter/converters/quantum_circuit_to_matrix.py`

 * *Files identical despite different names*

### Comparing `qiskit-classroom-converter-0.0.1/qiskit_class_converter/services/converter_service.py` & `qiskit-classroom-converter-0.0.2/qiskit_class_converter/services/converter_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 ConversionService(conversion_type="QC_TO_BRA_KET", option={"expression": "simplify"})
 ```
     """
 
     def __init__(self, conversion_type: typing.Union[str, ConversionType], option=None):
         """
         init function
-        :param conversion_type:  QC_TO_BRA_KET, QC_TO_MATRIX, MATRIX_TO_QC, BRA_KET_TO_MATRIX, BRA_KET_TO_QC
+        :param conversion_type:  QC_TO_BRA_KET, QC_TO_MATRIX, MATRIX_TO_QC, BRA_KET_TO_MATRIX
         :param option: See the Options table in this article.
         """
         if option is None:
             self.option = {}
         self.option = option
         if isinstance(conversion_type, str):
             self.__conversion_object = ConversionType[conversion_type.upper()].value
```

### Comparing `qiskit-classroom-converter-0.0.1/qiskit_classroom_converter.egg-info/PKG-INFO` & `qiskit-classroom-converter-0.0.2/qiskit_classroom_converter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-classroom-converter
-Version: 0.0.1
+Version: 0.0.2
 Summary: extend the Qiskit classroom applications.
 Author: KMU-quantum-classroom
 Project-URL: Homepage, https://github.com/KMU-quantum-classroom/qiskit-classroom-converter
 Project-URL: Bug Tracker, https://github.com/KMU-quantum-classroom/qiskit-classroom-converter/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -12,14 +12,18 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # qiskit-classroom-converter
 Qiskit classroom Converter
 
+## Documents
+
+https://kmu-quantum-classroom.github.io/qiskit-classroom-converter/qiskit_class_converter.html
+
 ## Support convert method
 
 * quantum circuit to bra-ket notation
 * quantum circuit to matrix
 * matrix to quantum circuit
 * bra-ket notation to matrix
```

### Comparing `qiskit-classroom-converter-0.0.1/qiskit_classroom_converter.egg-info/SOURCES.txt` & `qiskit-classroom-converter-0.0.2/qiskit_classroom_converter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qiskit-classroom-converter-0.0.1/tests/test_convert_class.py` & `qiskit-classroom-converter-0.0.2/tests/test_convert_class.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -87,8 +87,8 @@
         result = main.convert(input_value=quantum_circuit)
         expect_value = array([
             [1, 0, 0, 0],
             [0, 0, 0, 1],
             [0, 0, 1, 0],
             [0, 1, 0, 0]
         ])
-        self.assertTrue((result["result"].astype(int) & expect_value).any())
+        self.assertTrue((result["result"].astype(int) & expect_value).any())
```

### Comparing `qiskit-classroom-converter-0.0.1/tests/test_converter_service.py` & `qiskit-classroom-converter-0.0.2/tests/test_converter_service.py`

 * *Files identical despite different names*

