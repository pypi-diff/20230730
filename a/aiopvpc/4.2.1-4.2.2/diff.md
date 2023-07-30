# Comparing `tmp/aiopvpc-4.2.1.tar.gz` & `tmp/aiopvpc-4.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiopvpc-4.2.1.tar", max compression
+gzip compressed data, was "aiopvpc-4.2.2.tar", max compression
```

## Comparing `aiopvpc-4.2.1.tar` & `aiopvpc-4.2.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1074 2023-05-29 10:24:28.495344 aiopvpc-4.2.1/LICENSE
--rw-r--r--   0        0        0     1714 2023-05-29 10:24:28.495344 aiopvpc-4.2.1/README.md
--rw-r--r--   0        0        0      382 2023-05-29 10:24:28.495344 aiopvpc-4.2.1/aiopvpc/__init__.py
--rw-r--r--   0        0        0     2612 2023-05-29 10:24:28.495344 aiopvpc-4.2.1/aiopvpc/const.py
--rw-r--r--   0        0        0     1360 2023-05-29 10:24:28.495344 aiopvpc-4.2.1/aiopvpc/ha_helpers.py
--rw-r--r--   0        0        0     4960 2023-05-29 10:24:28.495344 aiopvpc-4.2.1/aiopvpc/parser.py
--rw-r--r--   0        0        0     4380 2023-05-29 10:24:28.495344 aiopvpc-4.2.1/aiopvpc/prices.py
--rw-r--r--   0        0        0    15031 2023-05-29 10:24:28.495344 aiopvpc-4.2.1/aiopvpc/pvpc_data.py
--rw-r--r--   0        0        0     4803 2023-05-29 10:24:28.495344 aiopvpc-4.2.1/aiopvpc/pvpc_tariff.py
--rw-r--r--   0        0        0      401 2023-05-29 10:24:28.495344 aiopvpc-4.2.1/aiopvpc/utils.py
--rw-r--r--   0        0        0     1627 2023-05-29 10:24:28.495344 aiopvpc-4.2.1/pyproject.toml
--rw-r--r--   0        0        0     2461 1970-01-01 00:00:00.000000 aiopvpc-4.2.1/setup.py
--rw-r--r--   0        0        0     2411 1970-01-01 00:00:00.000000 aiopvpc-4.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-07-30 10:02:40.666650 aiopvpc-4.2.2/LICENSE
+-rw-r--r--   0        0        0     1714 2023-07-30 10:02:40.666650 aiopvpc-4.2.2/README.md
+-rw-r--r--   0        0        0      382 2023-07-30 10:02:40.666650 aiopvpc-4.2.2/aiopvpc/__init__.py
+-rw-r--r--   0        0        0     2612 2023-07-30 10:02:40.666650 aiopvpc-4.2.2/aiopvpc/const.py
+-rw-r--r--   0        0        0     1360 2023-07-30 10:02:40.666650 aiopvpc-4.2.2/aiopvpc/ha_helpers.py
+-rw-r--r--   0        0        0     4960 2023-07-30 10:02:40.666650 aiopvpc-4.2.2/aiopvpc/parser.py
+-rw-r--r--   0        0        0     4380 2023-07-30 10:02:40.666650 aiopvpc-4.2.2/aiopvpc/prices.py
+-rw-r--r--   0        0        0    15031 2023-07-30 10:02:40.666650 aiopvpc-4.2.2/aiopvpc/pvpc_data.py
+-rw-r--r--   0        0        0     4803 2023-07-30 10:02:40.666650 aiopvpc-4.2.2/aiopvpc/pvpc_tariff.py
+-rw-r--r--   0        0        0      401 2023-07-30 10:02:40.666650 aiopvpc-4.2.2/aiopvpc/utils.py
+-rw-r--r--   0        0        0     1621 2023-07-30 10:02:40.666650 aiopvpc-4.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2455 1970-01-01 00:00:00.000000 aiopvpc-4.2.2/setup.py
+-rw-r--r--   0        0        0     2405 1970-01-01 00:00:00.000000 aiopvpc-4.2.2/PKG-INFO
```

### Comparing `aiopvpc-4.2.1/LICENSE` & `aiopvpc-4.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aiopvpc-4.2.1/README.md` & `aiopvpc-4.2.2/README.md`

 * *Files identical despite different names*

### Comparing `aiopvpc-4.2.1/aiopvpc/const.py` & `aiopvpc-4.2.2/aiopvpc/const.py`

 * *Files identical despite different names*

### Comparing `aiopvpc-4.2.1/aiopvpc/ha_helpers.py` & `aiopvpc-4.2.2/aiopvpc/ha_helpers.py`

 * *Files identical despite different names*

### Comparing `aiopvpc-4.2.1/aiopvpc/parser.py` & `aiopvpc-4.2.2/aiopvpc/parser.py`

 * *Files identical despite different names*

### Comparing `aiopvpc-4.2.1/aiopvpc/prices.py` & `aiopvpc-4.2.2/aiopvpc/prices.py`

 * *Files identical despite different names*

### Comparing `aiopvpc-4.2.1/aiopvpc/pvpc_data.py` & `aiopvpc-4.2.2/aiopvpc/pvpc_data.py`

 * *Files identical despite different names*

### Comparing `aiopvpc-4.2.1/aiopvpc/pvpc_tariff.py` & `aiopvpc-4.2.2/aiopvpc/pvpc_tariff.py`

 * *Files identical despite different names*

### Comparing `aiopvpc-4.2.1/pyproject.toml` & `aiopvpc-4.2.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -36,23 +36,23 @@
 log_cli_date_format = "%H:%M:%S"
 markers = [
     "real_api_call: Tests making requests to api.esios.ree.es (deselected by default)",
 ]
 
 [tool.poetry]
 name = "aiopvpc"
-version = "4.2.1"
+version = "4.2.2"
 description = "Retrieval of Spanish Electricity hourly prices (PVPC)"
 authors = ["Eugenio Panadero <eugenio.panadero@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/azogue/aiopvpc"
 
 [tool.poetry.dependencies]
-python = ">=3.9,<3.12"
+python = ">=3.9"
 aiohttp = ">=3.7.4.post0"
 async_timeout = ">=3.0.1"
 
 [tool.poetry.dev-dependencies]
 pytest-sugar = ">=0.9.2"
 pytest = ">=5.3.5"
 pytest-cov = ">=2.8.1"
```

### Comparing `aiopvpc-4.2.1/setup.py` & `aiopvpc-4.2.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 {'': ['*']}
 
 install_requires = \
 ['aiohttp>=3.7.4.post0', 'async_timeout>=3.0.1']
 
 setup_kwargs = {
     'name': 'aiopvpc',
-    'version': '4.2.1',
+    'version': '4.2.2',
     'description': 'Retrieval of Spanish Electricity hourly prices (PVPC)',
     'long_description': '[![PyPI Version][pypi-image]][pypi-url]\n[![pre-commit.ci Status][pre-commit-ci-image]][pre-commit-ci-url]\n[![Build Status][build-image]][build-url]\n[![Code Coverage][coverage-image]][coverage-url]\n\n<!-- Badges -->\n\n[pypi-image]: https://img.shields.io/pypi/v/aiopvpc\n[pypi-url]: https://pypi.org/project/aiopvpc/\n[pre-commit-ci-image]: https://results.pre-commit.ci/badge/github/azogue/aiopvpc/master.svg\n[pre-commit-ci-url]: https://results.pre-commit.ci/latest/github/azogue/aiopvpc/master\n[build-image]: https://github.com/azogue/aiopvpc/actions/workflows/main.yml/badge.svg\n[build-url]: https://github.com/azogue/aiopvpc/actions/workflows/main.yml\n[coverage-image]: https://codecov.io/gh/azogue/aiopvpc/branch/master/graph/badge.svg\n[coverage-url]: https://codecov.io/gh/azogue/aiopvpc\n\n# aiopvpc\n\nSimple aio library to download Spanish electricity hourly prices.\n\nMade to support the [**`pvpc_hourly_pricing`** HomeAssistant integration](https://www.home-assistant.io/integrations/pvpc_hourly_pricing/).\n\n<span class="badge-buymeacoffee"><a href="https://www.buymeacoffee.com/azogue" title="Donate to this project using Buy Me A Coffee"><img src="https://img.shields.io/badge/buy%20me%20a%20coffee-donate-yellow.svg" alt="Buy Me A Coffee donate button" /></a></span>\n\n## Install\n\nInstall with `pip install aiopvpc` or clone it to run tests or anything else.\n\n## Usage\n\n```python\nimport aiohttp\nfrom datetime import datetime\nfrom aiopvpc import PVPCData\n\nasync with aiohttp.ClientSession() as session:\n    pvpc_handler = PVPCData(session=session, tariff="2.0TD")\n    esios_data = await pvpc_handler.async_update_all(\n        current_data=None, now=datetime.utcnow()\n    )\nprint(esios_data.sensors["PVPC"])\n```\n',
     'author': 'Eugenio Panadero',
     'author_email': 'eugenio.panadero@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/azogue/aiopvpc',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.9,<3.12',
+    'python_requires': '>=3.9',
 }
 
 
 setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['aiopvpc']
 package_data = \ {'': ['*']} install_requires = \ ['aiohttp>=3.7.4.post0',
-'async_timeout>=3.0.1'] setup_kwargs = { 'name': 'aiopvpc', 'version': '4.2.1',
+'async_timeout>=3.0.1'] setup_kwargs = { 'name': 'aiopvpc', 'version': '4.2.2',
 'description': 'Retrieval of Spanish Electricity hourly prices (PVPC)',
 'long_description': '[![PyPI Version][pypi-image]][pypi-url]\n[![pre-commit.ci
 Status][pre-commit-ci-image]][pre-commit-ci-url]\n[![Build Status][build-
 image]][build-url]\n[![Code Coverage][coverage-image]][coverage-url]\n\n\n\n
 [pypi-image]: https://img.shields.io/pypi/v/aiopvpc\n[pypi-url]: https://
 pypi.org/project/aiopvpc/\n[pre-commit-ci-image]: https://results.pre-
 commit.ci/badge/github/azogue/aiopvpc/master.svg\n[pre-commit-ci-url]: https://
@@ -22,8 +22,8 @@
 aiohttp.ClientSession() as session:\n pvpc_handler = PVPCData(session=session,
 tariff="2.0TD")\n esios_data = await pvpc_handler.async_update_all(\n
 current_data=None, now=datetime.utcnow()\n )\nprint(esios_data.sensors
 ["PVPC"])\n```\n', 'author': 'Eugenio Panadero', 'author_email':
 'eugenio.panadero@gmail.com', 'maintainer': 'None', 'maintainer_email': 'None',
 'url': 'https://github.com/azogue/aiopvpc', 'packages': packages,
 'package_data': package_data, 'install_requires': install_requires,
-'python_requires': '>=3.9,<3.12', } setup(**setup_kwargs)
+'python_requires': '>=3.9', } setup(**setup_kwargs)
```

### Comparing `aiopvpc-4.2.1/PKG-INFO` & `aiopvpc-4.2.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: aiopvpc
-Version: 4.2.1
+Version: 4.2.2
 Summary: Retrieval of Spanish Electricity hourly prices (PVPC)
 Home-page: https://github.com/azogue/aiopvpc
 License: MIT
 Author: Eugenio Panadero
 Author-email: eugenio.panadero@gmail.com
-Requires-Python: >=3.9,<3.12
+Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.7.4.post0)
 Requires-Dist: async_timeout (>=3.0.1)
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: aiopvpc Version: 4.2.1 Summary: Retrieval of
+Metadata-Version: 2.1 Name: aiopvpc Version: 4.2.2 Summary: Retrieval of
 Spanish Electricity hourly prices (PVPC) Home-page: https://github.com/azogue/
 aiopvpc License: MIT Author: Eugenio Panadero Author-email:
-eugenio.panadero@gmail.com Requires-Python: >=3.9,<3.12 Classifier: License ::
-OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
+eugenio.panadero@gmail.com Requires-Python: >=3.9 Classifier: License :: OSI
+Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.7.4.post0) Requires-Dist: async_timeout (>=3.0.1)
 Project-URL: Repository, https://github.com/azogue/aiopvpc Description-Content-
 Type: text/markdown [![PyPI Version][pypi-image]][pypi-url] [![pre-commit.ci
 Status][pre-commit-ci-image]][pre-commit-ci-url] [![Build Status][build-image]]
 [build-url] [![Code Coverage][coverage-image]][coverage-url]  [pypi-image]:
```

