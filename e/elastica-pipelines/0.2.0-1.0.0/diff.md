# Comparing `tmp/elastica_pipelines-0.2.0.tar.gz` & `tmp/elastica_pipelines-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elastica_pipelines-0.2.0.tar", max compression
+gzip compressed data, was "elastica_pipelines-1.0.0.tar", max compression
```

## Comparing `elastica_pipelines-0.2.0.tar` & `elastica_pipelines-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1067 2022-10-19 06:05:23.665684 elastica_pipelines-0.2.0/LICENSE
--rw-r--r--   0        0        0     3764 2022-10-19 06:05:23.665684 elastica_pipelines-0.2.0/README.md
--rw-r--r--   0        0        0     2040 2022-10-19 06:05:34.709857 elastica_pipelines-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       26 2022-10-19 06:05:23.669684 elastica_pipelines-0.2.0/src/elastica_pipelines/__init__.py
--rw-r--r--   0        0        0      226 2022-10-19 06:05:23.669684 elastica_pipelines-0.2.0/src/elastica_pipelines/__main__.py
--rw-r--r--   0        0        0      478 2022-10-19 06:05:23.669684 elastica_pipelines-0.2.0/src/elastica_pipelines/io/__init__.py
--rw-r--r--   0        0        0     1495 2022-10-19 06:05:23.669684 elastica_pipelines-0.2.0/src/elastica_pipelines/io/backends.py
--rw-r--r--   0        0        0     9753 2022-10-19 06:05:23.669684 elastica_pipelines-0.2.0/src/elastica_pipelines/io/core.py
--rw-r--r--   0        0        0     2846 2022-10-19 06:05:23.669684 elastica_pipelines-0.2.0/src/elastica_pipelines/io/entry.py
--rw-r--r--   0        0        0     5977 2022-10-19 06:05:23.669684 elastica_pipelines-0.2.0/src/elastica_pipelines/io/protocols.py
--rw-r--r--   0        0        0     5600 2022-10-19 06:05:23.669684 elastica_pipelines-0.2.0/src/elastica_pipelines/io/specialize.py
--rw-r--r--   0        0        0    16684 2022-10-19 06:05:23.669684 elastica_pipelines-0.2.0/src/elastica_pipelines/io/temporal.py
--rw-r--r--   0        0        0     1990 2022-10-19 06:05:23.669684 elastica_pipelines-0.2.0/src/elastica_pipelines/io/transforms.py
--rw-r--r--   0        0        0     1545 2022-10-19 06:05:23.669684 elastica_pipelines-0.2.0/src/elastica_pipelines/io/typing.py
--rw-r--r--   0        0        0        0 2022-10-19 06:05:23.669684 elastica_pipelines-0.2.0/src/elastica_pipelines/py.typed
--rw-r--r--   0        0        0     4817 1970-01-01 00:00:00.000000 elastica_pipelines-0.2.0/setup.py
--rw-r--r--   0        0        0     4803 1970-01-01 00:00:00.000000 elastica_pipelines-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-30 16:26:07.928515 elastica_pipelines-1.0.0/LICENSE
+-rw-r--r--   0        0        0     3764 2023-07-30 16:26:07.928515 elastica_pipelines-1.0.0/README.md
+-rw-r--r--   0        0        0     2037 2023-07-30 16:26:21.328548 elastica_pipelines-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0       26 2023-07-30 16:26:07.928515 elastica_pipelines-1.0.0/src/elastica_pipelines/__init__.py
+-rw-r--r--   0        0        0      226 2023-07-30 16:26:07.928515 elastica_pipelines-1.0.0/src/elastica_pipelines/__main__.py
+-rw-r--r--   0        0        0      478 2023-07-30 16:26:07.928515 elastica_pipelines-1.0.0/src/elastica_pipelines/io/__init__.py
+-rw-r--r--   0        0        0     1495 2023-07-30 16:26:07.928515 elastica_pipelines-1.0.0/src/elastica_pipelines/io/backends.py
+-rw-r--r--   0        0        0     9753 2023-07-30 16:26:07.928515 elastica_pipelines-1.0.0/src/elastica_pipelines/io/core.py
+-rw-r--r--   0        0        0     3138 2023-07-30 16:26:07.928515 elastica_pipelines-1.0.0/src/elastica_pipelines/io/entry.py
+-rw-r--r--   0        0        0     5977 2023-07-30 16:26:07.928515 elastica_pipelines-1.0.0/src/elastica_pipelines/io/protocols.py
+-rw-r--r--   0        0        0     5600 2023-07-30 16:26:07.928515 elastica_pipelines-1.0.0/src/elastica_pipelines/io/specialize.py
+-rw-r--r--   0        0        0    16684 2023-07-30 16:26:07.928515 elastica_pipelines-1.0.0/src/elastica_pipelines/io/temporal.py
+-rw-r--r--   0        0        0     1990 2023-07-30 16:26:07.928515 elastica_pipelines-1.0.0/src/elastica_pipelines/io/transforms.py
+-rw-r--r--   0        0        0     1545 2023-07-30 16:26:07.928515 elastica_pipelines-1.0.0/src/elastica_pipelines/io/typing.py
+-rw-r--r--   0        0        0        0 2023-07-30 16:26:07.928515 elastica_pipelines-1.0.0/src/elastica_pipelines/py.typed
+-rw-r--r--   0        0        0     4817 1970-01-01 00:00:00.000000 elastica_pipelines-1.0.0/setup.py
+-rw-r--r--   0        0        0     4753 1970-01-01 00:00:00.000000 elastica_pipelines-1.0.0/PKG-INFO
```

### Comparing `elastica_pipelines-0.2.0/LICENSE` & `elastica_pipelines-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `elastica_pipelines-0.2.0/README.md` & `elastica_pipelines-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `elastica_pipelines-0.2.0/pyproject.toml` & `elastica_pipelines-1.0.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "elastica-pipelines"
-version = "0.2.0"
+version = "1.0.0"
 description = "Elastica Pipelines"
 authors = ["ElasticaDev <tp5@illinois.edu>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/tp5uiuc/elastica-pipelines"
 repository = "https://github.com/tp5uiuc/elastica-pipelines"
 documentation = "https://elastica-pipelines.readthedocs.io"
@@ -12,15 +12,15 @@
     "Development Status :: 3 - Alpha",
 ]
 
 [tool.poetry.urls]
 Changelog = "https://github.com/tp5uiuc/elastica-pipelines/releases"
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 click = ">=8.0.1"
 numpy = ">=1.20.0"
 typing-extensions = ">=4.3.0"
 h5py = "^3.7.0"
 
 [tool.poetry.dev-dependencies]
 Pygments = ">=2.10.0"
@@ -42,15 +42,15 @@
 pre-commit-hooks = ">=4.1.0"
 pytest = ">=6.2.5"
 pyupgrade = ">=2.29.1"
 safety = ">=1.10.3"
 sphinx = ">=4.3.2"
 sphinx-autobuild = ">=2021.3.14"
 sphinx-click = ">=3.0.2"
-typeguard = ">=2.13.3"
+typeguard = "4.0.0"
 xdoctest = {extras = ["colors"], version = ">=0.15.10"}
 myst-parser = {version = ">=0.16.1"}
 
 [tool.poetry.scripts]
 elastica-pipelines = "elastica_pipelines.__main__:main"
 
 [tool.coverage.paths]
```

### Comparing `elastica_pipelines-0.2.0/src/elastica_pipelines/io/backends.py` & `elastica_pipelines-1.0.0/src/elastica_pipelines/io/backends.py`

 * *Files identical despite different names*

### Comparing `elastica_pipelines-0.2.0/src/elastica_pipelines/io/core.py` & `elastica_pipelines-1.0.0/src/elastica_pipelines/io/core.py`

 * *Files identical despite different names*

### Comparing `elastica_pipelines-0.2.0/src/elastica_pipelines/io/entry.py` & `elastica_pipelines-1.0.0/src/elastica_pipelines/io/entry.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,32 +7,47 @@
 from typing import Union
 
 from elastica_pipelines.io.backends import SupportedBackends
 from elastica_pipelines.io.temporal import Series
 from elastica_pipelines.io.typing import FuncType
 
 
+def _check_ok(p: pathlib.Path) -> None:
+    """Check if input path is okay to read from.
+
+    Args:
+        p(Path) : path of file to choose backend.
+
+    Raises:
+        FileNotFoundError: If p does not exist.
+        OSError: If p is not a file.
+    """
+    if not p.exists():
+        raise FileNotFoundError(f"File in path {p} not found.")
+
+    if not p.is_file():
+        raise OSError(f"Path {p} is not a valid file.")
+
+
 def _choose_backend(p: pathlib.Path) -> SupportedBackends:
     """Choose backend based on file name.
 
     Args:
         p(Path) : path of file to choose backend.
 
     Returns:
         Supported Backend
 
     Raises:
-        FileNotFoundError: If p does not exist.
         RuntimeError: If backend is unsupported.
     """
-    if not p.exists():
-        raise FileNotFoundError(f"File in path {p} not found.")
+    _check_ok(p)
 
     def match(suffix: str) -> bool:
-        return p.is_file() and p.suffix == suffix
+        return p.suffix == suffix
 
     if match(".h5"):
         return SupportedBackends.HDF5
     else:
         raise RuntimeError(f"Unsupported backend {p.suffix}")
```

### Comparing `elastica_pipelines-0.2.0/src/elastica_pipelines/io/protocols.py` & `elastica_pipelines-1.0.0/src/elastica_pipelines/io/protocols.py`

 * *Files identical despite different names*

### Comparing `elastica_pipelines-0.2.0/src/elastica_pipelines/io/specialize.py` & `elastica_pipelines-1.0.0/src/elastica_pipelines/io/specialize.py`

 * *Files identical despite different names*

### Comparing `elastica_pipelines-0.2.0/src/elastica_pipelines/io/temporal.py` & `elastica_pipelines-1.0.0/src/elastica_pipelines/io/temporal.py`

 * *Files identical despite different names*

### Comparing `elastica_pipelines-0.2.0/src/elastica_pipelines/io/transforms.py` & `elastica_pipelines-1.0.0/src/elastica_pipelines/io/transforms.py`

 * *Files identical despite different names*

### Comparing `elastica_pipelines-0.2.0/src/elastica_pipelines/io/typing.py` & `elastica_pipelines-1.0.0/src/elastica_pipelines/io/typing.py`

 * *Files identical despite different names*

### Comparing `elastica_pipelines-0.2.0/setup.py` & `elastica_pipelines-1.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,25 +17,25 @@
  'typing-extensions>=4.3.0']
 
 entry_points = \
 {'console_scripts': ['elastica-pipelines = elastica_pipelines.__main__:main']}
 
 setup_kwargs = {
     'name': 'elastica-pipelines',
-    'version': '0.2.0',
+    'version': '1.0.0',
     'description': 'Elastica Pipelines',
     'long_description': '# Elastica Pipelines\n\n[![PyPI](https://img.shields.io/pypi/v/elastica-pipelines.svg)][pypi_]\n[![Status](https://img.shields.io/pypi/status/elastica-pipelines.svg)][status]\n[![Python Version](https://img.shields.io/pypi/pyversions/elastica-pipelines)][python version]\n[![License](https://img.shields.io/pypi/l/elastica-pipelines)][license]\n\n[![Read the documentation at https://elastica-pipelines.readthedocs.io/](https://img.shields.io/readthedocs/elastica-pipelines/latest.svg?label=Read%20the%20Docs)][read the docs]\n[![Tests](https://github.com/tp5uiuc/elastica-pipelines/workflows/Tests/badge.svg)][tests]\n[![Codecov](https://codecov.io/gh/tp5uiuc/elastica-pipelines/branch/main/graph/badge.svg)][codecov]\n\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]\n[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]\n\n[pypi_]: https://pypi.org/project/elastica-pipelines/\n[status]: https://pypi.org/project/elastica-pipelines/\n[python version]: https://pypi.org/project/elastica-pipelines\n[read the docs]: https://elastica-pipelines.readthedocs.io/\n[tests]: https://github.com/tp5uiuc/elastica-pipelines/actions?workflow=Tests\n[codecov]: https://app.codecov.io/gh/tp5uiuc/elastica-pipelines\n[pre-commit]: https://github.com/pre-commit/pre-commit\n[black]: https://github.com/psf/black\n\n## Features\n\n### IO\n\n- Lazy loading of simulation time-series data generated by **Elastica++** applications\n- Track a single, or a subset, or whole group of rods, over time using familiar slicing API\n\n## Installation\n\nYou can install _Elastica Pipelines_ via [pip] from [PyPI]:\n\n```console\n$ pip install elastica-pipelines\n```\n\n## Usage\n\nPlease see the [Command-line Reference] for details.\n\n### IO\n\n[![Python3][api-py3]](https://www.python.org/) ![Python3 API: Alpha][dev-alpha]\n\n[api-py3]: https://img.shields.io/badge/language-Python3-yellowgreen "Python3 API"\n[dev-alpha]: https://img.shields.io/badge/phase-alpha-yellowgreen "Status: Alpha"\n\n```py\nfrom elastica_pipelines import io\n\n# ...\n\n# Read only access to data written by Elastica++\nseries = io.series(metadata="elastica_metadata.h5")\n\n# use series like a python Mapping\nfor t, snapshot in series.iterations():\n    print("Iteration: {0} at time {1}".format(t.iterate, t.time))\n\n    # Snapshot is a mapping contain system types such as CosseratRods & Spheres\n    # Here we access only cosserat rods\n    for rod_id, rod in snapshot.cosserat_rods().items(): # snapshot[\'CosseratRod\'] also works!\n        if rod_id == 0:\n            print("  Rod \'{0}\' attributes:".format(rod_id))\n            # even rod is a Mapping, get its keys\n            print("  {0}".format(list(rod.keys())))\n        print("  Rod \'{0}\' position:".format(rod_id), rod[\'Position\'])\n```\n\n## Contributing\n\nContributions are very welcome.\nTo learn more, see the [Contributor Guide].\n\n## License\n\nDistributed under the terms of the [MIT license][license],\n_Elastica Pipelines_ is free and open source software.\n\n## Issues\n\nIf you encounter any problems,\nplease [file an issue] along with a detailed description.\n\n## Credits\n\nThis project was generated from [@cjolowicz]\'s [Hypermodern Python Cookiecutter] template.\n\n[@cjolowicz]: https://github.com/cjolowicz\n[pypi]: https://pypi.org/\n[hypermodern python cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python\n[file an issue]: https://github.com/tp5uiuc/elastica-pipelines/issues\n[pip]: https://pip.pypa.io/\n\n<!-- github-only -->\n\n[license]: https://github.com/tp5uiuc/elastica-pipelines/blob/main/LICENSE\n[contributor guide]: https://github.com/tp5uiuc/elastica-pipelines/blob/main/CONTRIBUTING.md\n[command-line reference]: https://elastica-pipelines.readthedocs.io/en/latest/usage.html\n',
     'author': 'ElasticaDev',
     'author_email': 'tp5@illinois.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/tp5uiuc/elastica-pipelines',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `elastica_pipelines-0.2.0/PKG-INFO` & `elastica_pipelines-1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: elastica-pipelines
-Version: 0.2.0
+Version: 1.0.0
 Summary: Elastica Pipelines
 Home-page: https://github.com/tp5uiuc/elastica-pipelines
 License: MIT
 Author: ElasticaDev
 Author-email: tp5@illinois.edu
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.0.1)
 Requires-Dist: h5py (>=3.7.0,<4.0.0)
 Requires-Dist: numpy (>=1.20.0)
```

