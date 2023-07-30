# Comparing `tmp/simple_dag-0.1.0.tar.gz` & `tmp/simple_dag-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_dag-0.1.0.tar", last modified: Thu Jun  1 14:46:40 2023, max compression
+gzip compressed data, was "simple_dag-0.1.1.tar", last modified: Sun Jul 30 16:14:11 2023, max compression
```

## Comparing `simple_dag-0.1.0.tar` & `simple_dag-0.1.1.tar`

### file list

```diff
@@ -1,39 +1,65 @@
-drwxr-xr-x   0 tim        (501) staff       (20)        0 2023-06-01 14:46:40.415904 simple_dag-0.1.0/
--rw-r--r--   0 tim        (501) staff       (20)      153 2023-05-18 10:24:17.000000 simple_dag-0.1.0/AUTHORS.rst
--rw-r--r--   0 tim        (501) staff       (20)     3544 2023-06-01 14:45:37.000000 simple_dag-0.1.0/CONTRIBUTING.rst
--rw-r--r--   0 tim        (501) staff       (20)       89 2023-05-18 10:24:17.000000 simple_dag-0.1.0/HISTORY.rst
--rw-r--r--   0 tim        (501) staff       (20)     1069 2023-05-18 10:24:17.000000 simple_dag-0.1.0/LICENSE
--rw-r--r--   0 tim        (501) staff       (20)      262 2023-05-18 10:24:17.000000 simple_dag-0.1.0/MANIFEST.in
--rw-r--r--   0 tim        (501) staff       (20)     2822 2023-06-01 14:46:40.415239 simple_dag-0.1.0/PKG-INFO
--rw-r--r--   0 tim        (501) staff       (20)      855 2023-06-01 14:45:37.000000 simple_dag-0.1.0/README.rst
-drwxr-xr-x   0 tim        (501) staff       (20)        0 2023-06-01 14:46:40.405973 simple_dag-0.1.0/docs/
--rw-r--r--   0 tim        (501) staff       (20)      611 2023-06-01 14:45:37.000000 simple_dag-0.1.0/docs/Makefile
-drwxr-xr-x   0 tim        (501) staff       (20)        0 2023-06-01 14:46:40.390275 simple_dag-0.1.0/docs/_build/
-drwxr-xr-x   0 tim        (501) staff       (20)        0 2023-06-01 14:46:40.390415 simple_dag-0.1.0/docs/_build/html/
-drwxr-xr-x   0 tim        (501) staff       (20)        0 2023-06-01 14:46:40.408451 simple_dag-0.1.0/docs/_build/html/_static/
--rw-r--r--   0 tim        (501) staff       (20)      286 2023-05-18 11:15:25.000000 simple_dag-0.1.0/docs/_build/html/_static/file.png
--rw-r--r--   0 tim        (501) staff       (20)       90 2023-05-18 11:15:25.000000 simple_dag-0.1.0/docs/_build/html/_static/minus.png
--rw-r--r--   0 tim        (501) staff       (20)       90 2023-05-18 11:15:25.000000 simple_dag-0.1.0/docs/_build/html/_static/plus.png
--rw-r--r--   0 tim        (501) staff       (20)       28 2023-05-18 10:24:17.000000 simple_dag-0.1.0/docs/authors.rst
--rwxr-xr-x   0 tim        (501) staff       (20)     4818 2023-06-01 14:45:37.000000 simple_dag-0.1.0/docs/conf.py
--rw-r--r--   0 tim        (501) staff       (20)       33 2023-05-18 10:24:17.000000 simple_dag-0.1.0/docs/contributing.rst
--rw-r--r--   0 tim        (501) staff       (20)       28 2023-05-18 10:24:17.000000 simple_dag-0.1.0/docs/history.rst
--rw-r--r--   0 tim        (501) staff       (20)      302 2023-06-01 14:45:37.000000 simple_dag-0.1.0/docs/index.rst
--rw-r--r--   0 tim        (501) staff       (20)     1138 2023-06-01 14:45:37.000000 simple_dag-0.1.0/docs/installation.rst
--rw-r--r--   0 tim        (501) staff       (20)      808 2023-06-01 14:45:37.000000 simple_dag-0.1.0/docs/make.bat
--rw-r--r--   0 tim        (501) staff       (20)       72 2023-06-01 14:45:37.000000 simple_dag-0.1.0/docs/modules.rst
--rw-r--r--   0 tim        (501) staff       (20)       27 2023-05-18 10:24:17.000000 simple_dag-0.1.0/docs/readme.rst
--rw-r--r--   0 tim        (501) staff       (20)      650 2023-06-01 14:45:37.000000 simple_dag-0.1.0/docs/simple_pipeline.rst
--rw-r--r--   0 tim        (501) staff       (20)       75 2023-06-01 14:45:37.000000 simple_dag-0.1.0/docs/usage.rst
--rw-r--r--   0 tim        (501) staff       (20)     1609 2023-06-01 14:45:37.000000 simple_dag-0.1.0/pyproject.toml
--rw-r--r--   0 tim        (501) staff       (20)       38 2023-06-01 14:46:40.416067 simple_dag-0.1.0/setup.cfg
-drwxr-xr-x   0 tim        (501) staff       (20)        0 2023-06-01 14:46:40.413187 simple_dag-0.1.0/simple_dag.egg-info/
--rw-r--r--   0 tim        (501) staff       (20)     2822 2023-06-01 14:46:40.000000 simple_dag-0.1.0/simple_dag.egg-info/PKG-INFO
--rw-r--r--   0 tim        (501) staff       (20)      650 2023-06-01 14:46:40.000000 simple_dag-0.1.0/simple_dag.egg-info/SOURCES.txt
--rw-r--r--   0 tim        (501) staff       (20)        1 2023-06-01 14:46:40.000000 simple_dag-0.1.0/simple_dag.egg-info/dependency_links.txt
--rw-r--r--   0 tim        (501) staff       (20)       51 2023-06-01 14:46:40.000000 simple_dag-0.1.0/simple_dag.egg-info/entry_points.txt
--rw-r--r--   0 tim        (501) staff       (20)      383 2023-06-01 14:46:40.000000 simple_dag-0.1.0/simple_dag.egg-info/requires.txt
--rw-r--r--   0 tim        (501) staff       (20)        1 2023-06-01 14:46:40.000000 simple_dag-0.1.0/simple_dag.egg-info/top_level.txt
-drwxr-xr-x   0 tim        (501) staff       (20)        0 2023-06-01 14:46:40.414608 simple_dag-0.1.0/tests/
--rw-r--r--   0 tim        (501) staff       (20)       40 2023-06-01 14:45:37.000000 simple_dag-0.1.0/tests/__init__.py
--rw-r--r--   0 tim        (501) staff       (20)      994 2023-06-01 14:45:37.000000 simple_dag-0.1.0/tests/test_simple_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:14:11.520607 simple_dag-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-30 16:13:08.000000 simple_dag-0.1.1/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:14:11.512606 simple_dag-0.1.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-30 16:13:08.000000 simple_dag-0.1.1/.github/ISSUE_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:14:11.512606 simple_dag-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-30 16:13:08.000000 simple_dag-0.1.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-30 16:13:08.000000 simple_dag-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-30 16:13:08.000000 simple_dag-0.1.1/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-30 16:13:08.000000 simple_dag-0.1.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-07-30 16:13:08.000000 simple_dag-0.1.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-30 16:13:08.000000 simple_dag-0.1.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-30 16:13:08.000000 simple_dag-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-30 16:13:08.000000 simple_dag-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-07-30 16:13:08.000000 simple_dag-0.1.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-07-30 16:14:11.516606 simple_dag-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-07-30 16:13:08.000000 simple_dag-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:14:11.512606 simple_dag-0.1.1/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)  1142998 2023-07-30 16:13:08.000000 simple_dag-0.1.1/assets/dagster.png
+-rw-r--r--   0 runner    (1001) docker     (123)   377331 2023-07-30 16:13:08.000000 simple_dag-0.1.1/assets/example.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:14:11.516606 simple_dag-0.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-30 16:13:08.000000 simple_dag-0.1.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:14:11.516606 simple_dag-0.1.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 16:13:08.000000 simple_dag-0.1.1/docs/_static/.gitkeep
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4880 2023-07-30 16:13:08.000000 simple_dag-0.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 16:13:08.000000 simple_dag-0.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-30 16:13:08.000000 simple_dag-0.1.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-30 16:13:08.000000 simple_dag-0.1.1/docs/simple_dag.datahandlers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-30 16:13:08.000000 simple_dag-0.1.1/docs/simple_dag.orchestrators.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-30 16:13:08.000000 simple_dag-0.1.1/docs/simple_dag.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-30 16:13:08.000000 simple_dag-0.1.1/docs/simple_dag.transforms.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-30 16:13:08.000000 simple_dag-0.1.1/docs/toc.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-30 16:13:08.000000 simple_dag-0.1.1/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:14:11.516606 simple_dag-0.1.1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:14:11.516606 simple_dag-0.1.1/examples/airports/
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-07-30 16:13:08.000000 simple_dag-0.1.1/examples/airports/airport.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-30 16:13:08.000000 simple_dag-0.1.1/examples/dag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:14:11.516606 simple_dag-0.1.1/examples/ds_salaries/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:14:11.508607 simple_dag-0.1.1/examples/ds_salaries/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:14:11.516606 simple_dag-0.1.1/examples/ds_salaries/data/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)   210076 2023-07-30 16:13:08.000000 simple_dag-0.1.1/examples/ds_salaries/data/raw/ds_salaries.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-07-30 16:13:08.000000 simple_dag-0.1.1/examples/ds_salaries/ds_salaries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-07-30 16:13:08.000000 simple_dag-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 16:14:11.520607 simple_dag-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:14:11.516606 simple_dag-0.1.1/simple_dag/
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-30 16:13:08.000000 simple_dag-0.1.1/simple_dag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-30 16:14:11.000000 simple_dag-0.1.1/simple_dag/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:14:11.516606 simple_dag-0.1.1/simple_dag/datahandlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-30 16:13:08.000000 simple_dag-0.1.1/simple_dag/datahandlers/base_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-30 16:13:08.000000 simple_dag-0.1.1/simple_dag/datahandlers/binary_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-07-30 16:13:08.000000 simple_dag-0.1.1/simple_dag/datahandlers/pandas_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-30 16:13:08.000000 simple_dag-0.1.1/simple_dag/datahandlers/spark_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:14:11.516606 simple_dag-0.1.1/simple_dag/orchestrators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 16:13:08.000000 simple_dag-0.1.1/simple_dag/orchestrators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-07-30 16:13:08.000000 simple_dag-0.1.1/simple_dag/orchestrators/dagster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-07-30 16:13:08.000000 simple_dag-0.1.1/simple_dag/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:14:11.516606 simple_dag-0.1.1/simple_dag.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-07-30 16:14:11.000000 simple_dag-0.1.1/simple_dag.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-07-30 16:14:11.000000 simple_dag-0.1.1/simple_dag.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 16:14:11.000000 simple_dag-0.1.1/simple_dag.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-30 16:14:11.000000 simple_dag-0.1.1/simple_dag.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-30 16:14:11.000000 simple_dag-0.1.1/simple_dag.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-30 16:14:11.000000 simple_dag-0.1.1/simple_dag.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:14:11.516606 simple_dag-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-30 16:13:08.000000 simple_dag-0.1.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-30 16:13:08.000000 simple_dag-0.1.1/tox.ini
```

### Comparing `simple_dag-0.1.0/CONTRIBUTING.rst` & `simple_dag-0.1.1/CONTRIBUTING.rst`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 -----------------------
 
 Before you submit a pull request, check that it meets these guidelines:
 
 1. The pull request should include tests.
 2. If the pull request adds functionality, the docs should be updated. Put
    your new functionality into a function with a docstring, and add the
-   feature to the list in README.rst.
+   feature to the list in README.md.
 3. The pull request should work for Python 3.5, 3.6, 3.7 and 3.8, and for PyPy. Check
    https://travis-ci.com/leokster/simple_dag/pull_requests
    and make sure that the tests pass for all supported Python versions.
 
 Tips
 ----
```

### Comparing `simple_dag-0.1.0/LICENSE` & `simple_dag-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_dag-0.1.0/docs/Makefile` & `simple_dag-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `simple_dag-0.1.0/docs/conf.py` & `simple_dag-0.1.1/docs/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,27 +27,32 @@
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
-extensions = ['sphinx.ext.autodoc', 'sphinx.ext.viewcode']
+extensions = [
+    "sphinx.ext.autodoc",
+    "sphinx.ext.viewcode",
+    "sphinx.ext.napoleon",
+    "sphinx.ext.doctest",
+]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 #
 # source_suffix = ['.rst', '.md']
 source_suffix = '.rst'
 
 # The master toctree document.
-master_doc = 'index'
+master_doc = 'toc'
 
 # General information about the project.
 project = 'simple_dag'
 copyright = "2023, Tim Rohner"
 author = "Tim Rohner"
 
 # The version info for the project you're documenting, acts as replacement
@@ -60,15 +65,15 @@
 release = simple_dag.__version__
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = "en"
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
 exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
 
 # The name of the Pygments (syntax highlighting) style to use.
```

### Comparing `simple_dag-0.1.0/docs/make.bat` & `simple_dag-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `simple_dag-0.1.0/pyproject.toml` & `simple_dag-0.1.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 [build-system]
-requires = ["setuptools", "wheel"]
+requires = ["setuptools>=61", "setuptools_scm[toml]>=6.2"]
+build-backend = "setuptools.build_meta"
 
 [project]
 name = "simple_dag"
-version = "0.1.0"
+dynamic = ["version"]
 description = "Create simple Pipelines with Python"
-readme = "README.rst"
+readme = "README.md"
 license = {file = "LICENSE"}
 authors = [{name = "Tim Rohner", email = "info@timrohner.ch"}]
 keywords = ["simple_dag"]
 # homepage = "https://github.com/leokster/simple_dag"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Intended Audience :: Developers",
@@ -17,43 +18,34 @@
     "Natural Language :: English",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8"
 ]
 dependencies = [
-    "Click>=7.0, <=8.1.3",
-    "dagit>=1.3.4",
-    "dagster>=0.10.0",
-    "pandas>=2.0.1, <=2.0.1"
+    "Click>=7.0, <=8.1.6",
+    "dagit >= 1.3.7, <= 1.4.2",
+    "dagster >= 1.3.7, <= 1.4.2",
+    "matplotlib >=3.4.2, <=3.7.2",
+    "pandas >=2.0.1, <=2.0.3"
 ]
 
 
 [project.scripts]
 simple_dag = "simple_dag.cli:main"
 
 [project.urls]
 Source = "https://github.com/leokster/simple_dag"
 
 
 [project.optional-dependencies]
 dev = [
-    "pip >=19.2.3, <= 23.1.2",
-    "bump2version >=0.5.11, <= 1.0.1",
-    "wheel >=0.33.6, <= 0.40.0",
-    "watchdog >=0.9.0, <= 3.0.0",
-    "flake8 >=3.7.8, <= 3.7.8",
+    "black >=21.7b0, <= 23.3.0",
     "tox >=3.14.0, <= 4.5.1",
-    "coverage >=4.5.4, <= 7.2.5",
-    "Sphinx >=1.8.5, <= 6.2.1",
-    "sphinx-rtd-theme >= 1.2.0, <= 1.2.0",
-    "twine >=1.14.0, <= 1.14.0",
-    "Click >=7.1.2, <= 8.1.3",
-    "pytest >=6.2.4, <= 7.3.1",
-    "black >=21.7b0, <= 23.3.0"
+    "twine >=1.14.0, <= 1.14.0"
 ]
 
 
 [tool.setuptools.packages.find]
 include = ["simple_dag", "simple_dag.*"]
 
 # [tool.setuptools.package-data]
```

