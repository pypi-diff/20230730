# Comparing `tmp/iso18245-1.2.0.tar.gz` & `tmp/iso18245-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iso18245-1.2.0.tar", max compression
+gzip compressed data, was "iso18245-1.3.0.tar", max compression
```

## Comparing `iso18245-1.2.0.tar` & `iso18245-1.3.0.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0     1073 2022-05-12 22:10:38.319936 iso18245-1.2.0/LICENSE
--rw-r--r--   0        0        0     1554 2022-05-12 22:10:38.319936 iso18245-1.2.0/README.md
--rw-r--r--   0        0        0     3519 2022-05-12 22:11:52.095439 iso18245-1.2.0/iso18245/__init__.py
--rw-r--r--   0        0        0    11368 2022-05-12 22:10:38.319936 iso18245-1.2.0/iso18245/data/alipay_list.csv
--rw-r--r--   0        0        0    12525 2022-05-12 22:10:38.323270 iso18245-1.2.0/iso18245/data/iso18245_official_list.csv
--rw-r--r--   0        0        0      552 2022-05-12 22:10:38.323270 iso18245-1.2.0/iso18245/data/iso18245_ranges.csv
--rw-r--r--   0        0        0       88 2022-05-12 22:10:38.323270 iso18245-1.2.0/iso18245/data/private_ranges.csv
--rw-r--r--   0        0        0    17546 2022-05-12 22:10:38.323270 iso18245-1.2.0/iso18245/data/stripe_list.csv
--rw-r--r--   0        0        0    21892 2022-05-12 22:10:38.323270 iso18245-1.2.0/iso18245/data/usda_list.csv
--rw-r--r--   0        0        0    29154 2022-05-12 22:10:38.323270 iso18245-1.2.0/iso18245/data/visa_list.csv
--rw-r--r--   0        0        0        0 2022-05-12 22:11:52.095439 iso18245-1.2.0/iso18245/py.typed
--rw-r--r--   0        0        0      815 2022-05-12 22:15:37.065384 iso18245-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     2237 1970-01-01 00:00:00.000000 iso18245-1.2.0/setup.py
--rw-r--r--   0        0        0     2566 1970-01-01 00:00:00.000000 iso18245-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-30 00:11:13.939806 iso18245-1.3.0/LICENSE
+-rw-r--r--   0        0        0     1554 2023-07-30 00:11:13.939806 iso18245-1.3.0/README.md
+-rw-r--r--   0        0        0     3536 2023-07-30 00:11:13.939806 iso18245-1.3.0/iso18245/__init__.py
+-rw-r--r--   0        0        0    11368 2023-07-30 00:11:13.939806 iso18245-1.3.0/iso18245/data/alipay_list.csv
+-rw-r--r--   0        0        0    12525 2023-07-30 00:11:13.939806 iso18245-1.3.0/iso18245/data/iso18245_official_list.csv
+-rw-r--r--   0        0        0      552 2023-07-30 00:11:13.939806 iso18245-1.3.0/iso18245/data/iso18245_ranges.csv
+-rw-r--r--   0        0        0       88 2023-07-30 00:11:13.939806 iso18245-1.3.0/iso18245/data/private_ranges.csv
+-rw-r--r--   0        0        0    17546 2023-07-30 00:11:13.939806 iso18245-1.3.0/iso18245/data/stripe_list.csv
+-rw-r--r--   0        0        0    21892 2023-07-30 00:11:13.939806 iso18245-1.3.0/iso18245/data/usda_list.csv
+-rw-r--r--   0        0        0    29154 2023-07-30 00:11:13.939806 iso18245-1.3.0/iso18245/data/visa_list.csv
+-rw-r--r--   0        0        0        0 2023-07-30 00:11:13.939806 iso18245-1.3.0/iso18245/py.typed
+-rw-r--r--   0        0        0      849 2023-07-30 00:11:31.536653 iso18245-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2517 1970-01-01 00:00:00.000000 iso18245-1.3.0/PKG-INFO
```

### Comparing `iso18245-1.2.0/LICENSE` & `iso18245-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iso18245-1.2.0/README.md` & `iso18245-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `iso18245-1.2.0/iso18245/__init__.py` & `iso18245-1.3.0/iso18245/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,49 @@
 import csv
 import os.path
-from collections import namedtuple
-from typing import Dict, List
+from typing import Dict, List, NamedTuple
 
 from pkg_resources import resource_filename
 
 ISO_VERSION_YEAR = 2003
 
 
 class MCCNotFound(KeyError):
 	pass
 
 
 class InvalidMCC(ValueError):
 	pass
 
 
-MCC = namedtuple(
-	"MCC",
-	(
-		"mcc",
-		"range",
-		"iso_description",
-		"usda_description",
-		"stripe_description",
-		"stripe_code",
-		"visa_description",
-		"visa_req_clearing_name",
-		"alipay_description",
-	),
-)
-MCCRange = namedtuple("MCCRange", ("start", "end", "description", "reserved"))
+class MCCRange(NamedTuple):
+	start: str
+	end: str
+	description: str
+	reserved: bool
+
+
+class MCC(NamedTuple):
+	mcc: str
+	range: MCCRange
+	iso_description: str
+	usda_description: str
+	stripe_description: str
+	stripe_code: str
+	visa_description: str
+	visa_req_clearing_name: str
+	alipay_description: str
+
 
 _cached_csv: Dict[str, List[List[str]]] = {}
 
 
 def _load_csv(path: str) -> List[List[str]]:
-	full_path = resource_filename("iso18245", os.path.join("data", path))
 	if path not in _cached_csv:
+		full_path = resource_filename("iso18245", os.path.join("data", path))
 		with open(full_path, "r") as f:
 			reader = csv.reader(f)
 			_cached_csv[path] = list(reader)[1:]
 
 	return _cached_csv[path]
 
 
@@ -78,15 +80,19 @@
 
 	usda_data = _find_mcc_in_csv(mcc, "usda_list.csv")
 	if usda_data:
 		usda_description, found = usda_data[0], True
 
 	visa_info = _find_mcc_in_csv(mcc, "visa_list.csv")
 	if visa_info:
-		visa_description, visa_req_clearing_name, found = visa_info[0], visa_info[1], True
+		visa_description, visa_req_clearing_name, found = (
+			visa_info[0],
+			visa_info[1],
+			True,
+		)
 
 	stripe_info = _find_mcc_in_csv(mcc, "stripe_list.csv")
 	if stripe_info:
 		stripe_description, stripe_code, found = stripe_info[0], stripe_info[1], True
 
 	alipay_info = _find_mcc_in_csv(mcc, "alipay_list.csv")
 	if alipay_info:
@@ -111,15 +117,18 @@
 def get_mcc_range(mcc: str) -> MCCRange:
 	mcc_as_num = validate_mcc(mcc)
 	range_data = _load_csv("iso18245_ranges.csv")
 	for range_start, range_end, description in range_data:
 		start_num, end_num = int(range_start), int(range_end)
 		if start_num <= mcc_as_num <= end_num:
 			return MCCRange(
-				range_start, range_end, description, reserved=description.startswith("Reserved")
+				range_start,
+				range_end,
+				description,
+				reserved=description.startswith("Reserved"),
 			)
 
 		if end_num > mcc_as_num:
 			break
 
 	raise RuntimeError(f"Could not find correct MCC range for {mcc} (likely a bug)")
```

### Comparing `iso18245-1.2.0/iso18245/data/alipay_list.csv` & `iso18245-1.3.0/iso18245/data/alipay_list.csv`

 * *Files identical despite different names*

### Comparing `iso18245-1.2.0/iso18245/data/iso18245_official_list.csv` & `iso18245-1.3.0/iso18245/data/iso18245_official_list.csv`

 * *Files identical despite different names*

### Comparing `iso18245-1.2.0/iso18245/data/iso18245_ranges.csv` & `iso18245-1.3.0/iso18245/data/iso18245_ranges.csv`

 * *Files identical despite different names*

### Comparing `iso18245-1.2.0/iso18245/data/stripe_list.csv` & `iso18245-1.3.0/iso18245/data/stripe_list.csv`

 * *Files identical despite different names*

### Comparing `iso18245-1.2.0/iso18245/data/usda_list.csv` & `iso18245-1.3.0/iso18245/data/usda_list.csv`

 * *Files identical despite different names*

### Comparing `iso18245-1.2.0/iso18245/data/visa_list.csv` & `iso18245-1.3.0/iso18245/data/visa_list.csv`

 * *Files identical despite different names*

### Comparing `iso18245-1.2.0/pyproject.toml` & `iso18245-1.3.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iso18245"
-version = "1.2.0"
+version = "1.3.0"
 description = "The ISO 18245 Merchant Category Codes database"
 authors = ["Jerome Leclanche <jerome@leclan.ch>"]
 readme = "README.md"
 repository = "https://github.com/jleclanche/python-iso18245"
 license = "MIT"
 classifiers = [
 	"Development Status :: 5 - Production/Stable",
@@ -12,24 +12,24 @@
 	"Topic :: Office/Business :: Financial",
 	"Topic :: Office/Business :: Financial :: Accounting",
 	"Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
 
 [tool.poetry.dependencies]
-python = "^3.6"
+python = "^3.8"
 
-[tool.poetry.dev-dependencies]
-mypy = "^0.950"
-types-setuptools = "^57.4.14"
+[tool.poetry.group.dev.dependencies]
+mypy = "^1.2.0"
+pre-commit = "^3.2.2"
+types-setuptools = "^68.0.0.3"
 
 [build-system]
-requires = ["poetry>=0.12"]
+requires = ["poetry_core>=1.5.0"]
 build-backend = "poetry.masonry.api"
 
 [tool.black]
 use-tabs = true
 
 [tool.mypy]
 strict = true
 warn_unused_configs = true
-
```

### Comparing `iso18245-1.2.0/PKG-INFO` & `iso18245-1.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: iso18245
-Version: 1.2.0
+Version: 1.3.0
 Summary: The ISO 18245 Merchant Category Codes database
 Home-page: https://github.com/jleclanche/python-iso18245
 License: MIT
 Author: Jerome Leclanche
 Author-email: jerome@leclan.ch
-Requires-Python: >=3.6,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Office/Business :: Financial
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Project-URL: Repository, https://github.com/jleclanche/python-iso18245
 Description-Content-Type: text/markdown
 
 # python-iso18245
```

