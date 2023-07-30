# Comparing `tmp/jaraco.home-3.4.0.tar.gz` & `tmp/jaraco.home-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaraco.home-3.4.0.tar", last modified: Sat Aug 21 00:36:20 2021, max compression
+gzip compressed data, was "jaraco.home-3.5.0.tar", last modified: Sun Jul 30 00:40:29 2023, max compression
```

## Comparing `jaraco.home-3.4.0.tar` & `jaraco.home-3.5.0.tar`

### file list

```diff
@@ -1,39 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-21 00:36:20.720147 jaraco.home-3.4.0/
--rw-r--r--   0 runner    (1001) docker     (121)       99 2021-08-21 00:35:56.000000 jaraco.home-3.4.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (121)      195 2021-08-21 00:35:56.000000 jaraco.home-3.4.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (121)      136 2021-08-21 00:35:56.000000 jaraco.home-3.4.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-21 00:36:20.720147 jaraco.home-3.4.0/.github/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2021-08-21 00:35:56.000000 jaraco.home-3.4.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-21 00:36:20.720147 jaraco.home-3.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1104 2021-08-21 00:35:56.000000 jaraco.home-3.4.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (121)       81 2021-08-21 00:35:56.000000 jaraco.home-3.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       79 2021-08-21 00:35:56.000000 jaraco.home-3.4.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)      974 2021-08-21 00:35:56.000000 jaraco.home-3.4.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1050 2021-08-21 00:35:56.000000 jaraco.home-3.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1415 2021-08-21 00:36:20.720147 jaraco.home-3.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      808 2021-08-21 00:35:56.000000 jaraco.home-3.4.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      684 2021-08-21 00:35:56.000000 jaraco.home-3.4.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-21 00:36:20.720147 jaraco.home-3.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      814 2021-08-21 00:35:56.000000 jaraco.home-3.4.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       81 2021-08-21 00:35:56.000000 jaraco.home-3.4.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (121)      292 2021-08-21 00:35:56.000000 jaraco.home-3.4.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-21 00:36:20.716146 jaraco.home-3.4.0/jaraco/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-21 00:36:20.720147 jaraco.home-3.4.0/jaraco/home/
--rw-r--r--   0 runner    (1001) docker     (121)      652 2021-08-21 00:35:56.000000 jaraco.home-3.4.0/jaraco/home/Gather HDHomeRun Stats.plist
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-21 00:35:56.000000 jaraco.home-3.4.0/jaraco/home/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3831 2021-08-21 00:35:56.000000 jaraco.home-3.4.0/jaraco/home/hdhomerun.py
--rw-r--r--   0 runner    (1001) docker     (121)      244 2021-08-21 00:35:56.000000 jaraco.home-3.4.0/jaraco/home/mock hdhomerun.py
--rw-r--r--   0 runner    (1001) docker     (121)      666 2021-08-21 00:35:56.000000 jaraco.home-3.4.0/jaraco/home/relay.py
--rw-r--r--   0 runner    (1001) docker     (121)     2742 2021-08-21 00:35:56.000000 jaraco.home-3.4.0/jaraco/home/thermostat.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-21 00:36:20.720147 jaraco.home-3.4.0/jaraco.home.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1415 2021-08-21 00:36:20.000000 jaraco.home-3.4.0/jaraco.home.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      615 2021-08-21 00:36:20.000000 jaraco.home-3.4.0/jaraco.home.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-21 00:36:20.000000 jaraco.home-3.4.0/jaraco.home.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      351 2021-08-21 00:36:20.000000 jaraco.home-3.4.0/jaraco.home.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-08-21 00:36:20.000000 jaraco.home-3.4.0/jaraco.home.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       37 2021-08-21 00:35:56.000000 jaraco.home-3.4.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (121)      367 2021-08-21 00:35:56.000000 jaraco.home-3.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      416 2021-08-21 00:35:56.000000 jaraco.home-3.4.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (121)     1121 2021-08-21 00:36:20.720147 jaraco.home-3.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       92 2021-08-21 00:35:56.000000 jaraco.home-3.4.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)      732 2021-08-21 00:35:56.000000 jaraco.home-3.4.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 00:40:29.786366 jaraco.home-3.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-30 00:40:01.000000 jaraco.home-3.5.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-30 00:40:01.000000 jaraco.home-3.5.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 00:40:29.778366 jaraco.home-3.5.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-30 00:40:01.000000 jaraco.home-3.5.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 00:40:29.778366 jaraco.home-3.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-07-30 00:40:01.000000 jaraco.home-3.5.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-30 00:40:01.000000 jaraco.home-3.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-30 00:40:01.000000 jaraco.home-3.5.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-30 00:40:01.000000 jaraco.home-3.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-30 00:40:01.000000 jaraco.home-3.5.0/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-07-30 00:40:29.786366 jaraco.home-3.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-30 00:40:01.000000 jaraco.home-3.5.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-30 00:40:01.000000 jaraco.home-3.5.0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 00:40:29.782366 jaraco.home-3.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-30 00:40:01.000000 jaraco.home-3.5.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-30 00:40:01.000000 jaraco.home-3.5.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-30 00:40:01.000000 jaraco.home-3.5.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 00:40:29.774366 jaraco.home-3.5.0/jaraco/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 00:40:29.786366 jaraco.home-3.5.0/jaraco/home/
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-30 00:40:01.000000 jaraco.home-3.5.0/jaraco/home/Gather HDHomeRun Stats.plist
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 00:40:01.000000 jaraco.home-3.5.0/jaraco/home/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-07-30 00:40:01.000000 jaraco.home-3.5.0/jaraco/home/hdhomerun.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-30 00:40:01.000000 jaraco.home-3.5.0/jaraco/home/mock hdhomerun.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-30 00:40:01.000000 jaraco.home-3.5.0/jaraco/home/relay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-07-30 00:40:01.000000 jaraco.home-3.5.0/jaraco/home/thermostat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 00:40:29.782366 jaraco.home-3.5.0/jaraco.home.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-07-30 00:40:29.000000 jaraco.home-3.5.0/jaraco.home.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-30 00:40:29.000000 jaraco.home-3.5.0/jaraco.home.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 00:40:29.000000 jaraco.home-3.5.0/jaraco.home.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-30 00:40:29.000000 jaraco.home-3.5.0/jaraco.home.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-30 00:40:29.000000 jaraco.home-3.5.0/jaraco.home.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-30 00:40:01.000000 jaraco.home-3.5.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-30 00:40:01.000000 jaraco.home-3.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-30 00:40:01.000000 jaraco.home-3.5.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-30 00:40:29.786366 jaraco.home-3.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-30 00:40:01.000000 jaraco.home-3.5.0/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-30 00:40:01.000000 jaraco.home-3.5.0/tox.ini
```

### Comparing `jaraco.home-3.4.0/CHANGES.rst` & `jaraco.home-3.5.0/NEWS.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v3.5.0
+======
+
+Features
+--------
+
+- Require Python 3.8 or later.
+
+
 v3.4.0
 ======
 
 In HDHomeRun utility, now include device ID in the data.
 
 v3.3.1
 ======
```

### Comparing `jaraco.home-3.4.0/LICENSE` & `jaraco.home-3.5.0/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-Copyright Jason R. Coombs
-
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to
 deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
 sell copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `jaraco.home-3.4.0/PKG-INFO` & `jaraco.home-3.5.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,42 +1,39 @@
 Metadata-Version: 2.1
 Name: jaraco.home
-Version: 3.4.0
+Version: 3.5.0
 Summary: Some functions supporting the devices in jaraco's home
 Home-page: https://github.com/jaraco/jaraco.home
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.9
 Provides-Extra: testing
 Provides-Extra: docs
 License-File: LICENSE
 
 .. image:: https://img.shields.io/pypi/v/jaraco.home.svg
-   :target: `PyPI link`_
+   :target: https://pypi.org/project/jaraco.home
 
 .. image:: https://img.shields.io/pypi/pyversions/jaraco.home.svg
-   :target: `PyPI link`_
-
-.. _PyPI link: https://pypi.org/project/jaraco.home
 
 .. image:: https://github.com/jaraco/jaraco.home/workflows/tests/badge.svg
    :target: https://github.com/jaraco/jaraco.home/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
-.. .. image:: https://readthedocs.org/projects/skeleton/badge/?version=latest
-..    :target: https://skeleton.readthedocs.io/en/latest/?badge=latest
+.. .. image:: https://readthedocs.org/projects/PROJECT_RTD/badge/?version=latest
+..    :target: https://PROJECT_RTD.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2021-informational
+.. image:: https://img.shields.io/badge/skeleton-2023-informational
    :target: https://blog.jaraco.com/skeleton
-
-
```

### Comparing `jaraco.home-3.4.0/README.rst` & `jaraco.home-3.5.0/README.rst`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 .. image:: https://img.shields.io/pypi/v/jaraco.home.svg
-   :target: `PyPI link`_
+   :target: https://pypi.org/project/jaraco.home
 
 .. image:: https://img.shields.io/pypi/pyversions/jaraco.home.svg
-   :target: `PyPI link`_
-
-.. _PyPI link: https://pypi.org/project/jaraco.home
 
 .. image:: https://github.com/jaraco/jaraco.home/workflows/tests/badge.svg
    :target: https://github.com/jaraco/jaraco.home/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
-.. .. image:: https://readthedocs.org/projects/skeleton/badge/?version=latest
-..    :target: https://skeleton.readthedocs.io/en/latest/?badge=latest
+.. .. image:: https://readthedocs.org/projects/PROJECT_RTD/badge/?version=latest
+..    :target: https://PROJECT_RTD.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2021-informational
+.. image:: https://img.shields.io/badge/skeleton-2023-informational
    :target: https://blog.jaraco.com/skeleton
```

### Comparing `jaraco.home-3.4.0/conftest.py` & `jaraco.home-3.5.0/conftest.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,16 +12,17 @@
 collect_ignore = [
     'jaraco/home/relay.py',
 ] + win_ignore
 
 
 @pytest.fixture(scope='session', autouse=True)
 def hdhomerun_config_mocked():
-    # todo: should be jaraco.home.homerun, but for pytest bug
-    import home.hdhomerun as hd
+    import jaraco.home.hdhomerun as hd
 
     hd.hdhomerun_config = 'hdhomerun_config'
     scripts = mockprocess.MockProc()
-    script = files('jaraco.home').joinpath('mock hdhomerun.py').read_text()
+    script = (
+        files('jaraco.home').joinpath('mock hdhomerun.py').read_text(encoding='utf-8')
+    )
     scripts.append('hdhomerun_config', returncode=0, script=script)
     with scripts:
         yield
```

### Comparing `jaraco.home-3.4.0/docs/conf.py` & `jaraco.home-3.5.0/docs/conf.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,42 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-
-extensions = ['sphinx.ext.autodoc', 'jaraco.packaging.sphinx', 'rst.linker']
+extensions = [
+    'sphinx.ext.autodoc',
+    'jaraco.packaging.sphinx',
+]
 
 master_doc = "index"
+html_theme = "furo"
 
+# Link dates and other references in the changelog
+extensions += ['rst.linker']
 link_files = {
-    '../CHANGES.rst': dict(
+    '../NEWS.rst': dict(
         using=dict(GH='https://github.com'),
         replace=[
             dict(
                 pattern=r'(Issue #|\B#)(?P<issue>\d+)',
                 url='{package_url}/issues/{issue}',
             ),
             dict(
                 pattern=r'(?m:^((?P<scm_version>v?\d+(\.\d+){1,2}))\n[-=]+\n)',
                 with_scm='{text}\n{rev[timestamp]:%d %b %Y}\n',
             ),
             dict(
                 pattern=r'PEP[- ](?P<pep_number>\d+)',
-                url='https://www.python.org/dev/peps/pep-{pep_number:0>4}/',
+                url='https://peps.python.org/pep-{pep_number:0>4}/',
             ),
         ],
     )
 }
 
-# Be strict about any broken references:
+# Be strict about any broken references
 nitpicky = True
+
+# Include Python intersphinx mapping to prevent failures
+# jaraco/skeleton#51
+extensions += ['sphinx.ext.intersphinx']
+intersphinx_mapping = {
+    'python': ('https://docs.python.org/3', None),
+}
+
+# Preserve authored syntax for defaults
+autodoc_preserve_defaults = True
```

### Comparing `jaraco.home-3.4.0/jaraco/home/Gather HDHomeRun Stats.plist` & `jaraco.home-3.5.0/jaraco/home/Gather HDHomeRun Stats.plist`

 * *Files identical despite different names*

### Comparing `jaraco.home-3.4.0/jaraco/home/hdhomerun.py` & `jaraco.home-3.5.0/jaraco/home/hdhomerun.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,25 +39,25 @@
     ['1072F92A', '1072F92A']
     """
     return (match.group(1) for match in re.finditer(r'device (\w+)', res))
 
 
 def discover():
     cmd = [hdhomerun_config, 'discover']
-    return parse_devices(subprocess.check_output(cmd, text=True))
+    return parse_devices(subprocess.check_output(cmd, text=True, encoding='utf-8'))
 
 
 @retry(retries=5, cleanup=sleep_2, trap=Exception)
 def get_status(tuner_id, device_id='FFFFFFFF'):
     """
     >>> get_status(0)
     {'ch': None, 'ss': 80}
     """
     cmd = [hdhomerun_config, device_id, 'get', f'/tuner{tuner_id}/status']
-    line = subprocess.check_output(cmd, text=True)
+    line = subprocess.check_output(cmd, text=True, encoding='utf-8')
     return parse_status(line)
 
 
 @retry(retries=5, cleanup=sleep_2, trap=Exception)
 def set_channel(tuner_id, channel, device_id='FFFFFFFF'):
     channel_str = str(channel) if channel else 'none'
     cmd = [
```

### Comparing `jaraco.home-3.4.0/jaraco/home/relay.py` & `jaraco.home-3.5.0/jaraco/home/relay.py`

 * *Files identical despite different names*

### Comparing `jaraco.home-3.4.0/jaraco/home/thermostat.py` & `jaraco.home-3.5.0/jaraco/home/thermostat.py`

 * *Files identical despite different names*

### Comparing `jaraco.home-3.4.0/jaraco.home.egg-info/PKG-INFO` & `jaraco.home-3.5.0/jaraco.home.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,42 +1,39 @@
 Metadata-Version: 2.1
 Name: jaraco.home
-Version: 3.4.0
+Version: 3.5.0
 Summary: Some functions supporting the devices in jaraco's home
 Home-page: https://github.com/jaraco/jaraco.home
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.9
 Provides-Extra: testing
 Provides-Extra: docs
 License-File: LICENSE
 
 .. image:: https://img.shields.io/pypi/v/jaraco.home.svg
-   :target: `PyPI link`_
+   :target: https://pypi.org/project/jaraco.home
 
 .. image:: https://img.shields.io/pypi/pyversions/jaraco.home.svg
-   :target: `PyPI link`_
-
-.. _PyPI link: https://pypi.org/project/jaraco.home
 
 .. image:: https://github.com/jaraco/jaraco.home/workflows/tests/badge.svg
    :target: https://github.com/jaraco/jaraco.home/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
-.. .. image:: https://readthedocs.org/projects/skeleton/badge/?version=latest
-..    :target: https://skeleton.readthedocs.io/en/latest/?badge=latest
+.. .. image:: https://readthedocs.org/projects/PROJECT_RTD/badge/?version=latest
+..    :target: https://PROJECT_RTD.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2021-informational
+.. image:: https://img.shields.io/badge/skeleton-2023-informational
    :target: https://blog.jaraco.com/skeleton
-
-
```

### Comparing `jaraco.home-3.4.0/jaraco.home.egg-info/SOURCES.txt` & `jaraco.home-3.5.0/jaraco.home.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 .coveragerc
 .editorconfig
-.flake8
 .pre-commit-config.yaml
-.readthedocs.yml
-CHANGES.rst
+.readthedocs.yaml
 LICENSE
+NEWS.rst
 README.rst
 conftest.py
 mypy.ini
 pyproject.toml
 pytest.ini
 setup.cfg
-setup.py
+towncrier.toml
 tox.ini
 .github/dependabot.yml
 .github/workflows/main.yml
 docs/conf.py
 docs/history.rst
 docs/index.rst
 jaraco.home.egg-info/PKG-INFO
```

### Comparing `jaraco.home-3.4.0/setup.cfg` & `jaraco.home-3.5.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -31,30 +31,32 @@
 	build*
 	dist*
 	docs*
 	tests*
 
 [options.extras_require]
 testing = 
-	pytest >= 4.6
+	pytest >= 6
 	pytest-checkdocs >= 2.4
-	pytest-flake8
 	pytest-black >= 0.3.7; \
 	python_implementation != "PyPy"
 	pytest-cov
-	pytest-mypy; \
+	pytest-mypy >= 0.9.1; \
 	python_implementation != "PyPy"
-	pytest-enabler >= 1.0.1
+	pytest-enabler >= 2.2
+	pytest-ruff
 	
 	types-requests
 	mockproc
 docs = 
-	sphinx
-	jaraco.packaging >= 8.2
+	sphinx >= 3.5
+	jaraco.packaging >= 9.3
 	rst.linker >= 1.9
+	furo
+	sphinx-lint
 
 [options.entry_points]
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

