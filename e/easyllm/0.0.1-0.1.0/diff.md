# Comparing `tmp/easyllm-0.0.1.tar.gz` & `tmp/easyllm-0.1.0.tar.gz`

## Comparing `easyllm-0.0.1.tar` & `easyllm-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,33 @@
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 easyllm-0.0.1/makefile
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 easyllm-0.0.1/mkdocs.yml
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 easyllm-0.0.1/.github/workflows/check.yaml
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 easyllm-0.0.1/.github/workflows/documentation.yaml
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 easyllm-0.0.1/.github/workflows/publish.yaml
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 easyllm-0.0.1/.github/workflows/test.yaml
--rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 easyllm-0.0.1/docs/index.md
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 easyllm-0.0.1/docs/references.md
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 easyllm-0.0.1/myproject/__init__.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 easyllm-0.0.1/myproject/cli.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 easyllm-0.0.1/myproject/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 easyllm-0.0.1/scripts/.gitkeep
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 easyllm-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 easyllm-0.0.1/tests/test_main.py
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 easyllm-0.0.1/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 easyllm-0.0.1/LICENSE
--rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 easyllm-0.0.1/README.md
--rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 easyllm-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3899 2020-02-02 00:00:00.000000 easyllm-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 easyllm-0.1.0/makefile
+-rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 easyllm-0.1.0/mkdocs.yml
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 easyllm-0.1.0/.github/workflows/check.yaml
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 easyllm-0.1.0/.github/workflows/documentation.yaml
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 easyllm-0.1.0/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 easyllm-0.1.0/.github/workflows/test.yaml
+-rw-r--r--   0        0        0     3823 2020-02-02 00:00:00.000000 easyllm-0.1.0/docs/clients.md
+-rw-r--r--   0        0        0     4041 2020-02-02 00:00:00.000000 easyllm-0.1.0/docs/index.md
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 easyllm-0.1.0/docs/installation.md
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 easyllm-0.1.0/docs/prompt_utils.md
+-rw-r--r--   0        0        0    19117 2020-02-02 00:00:00.000000 easyllm-0.1.0/docs/examples/chat-completion-api.ipynb
+-rw-r--r--   0        0        0    49822 2020-02-02 00:00:00.000000 easyllm-0.1.0/docs/examples/stream-chat-completions.ipynb
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 easyllm-0.1.0/easyllm/__init__.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 easyllm-0.1.0/easyllm/cli.py
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 easyllm-0.1.0/easyllm/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 easyllm-0.1.0/easyllm/clients/__init__.py
+-rw-r--r--   0        0        0     6981 2020-02-02 00:00:00.000000 easyllm-0.1.0/easyllm/clients/huggingface.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 easyllm-0.1.0/easyllm/evol_instruct/__init__.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 easyllm-0.1.0/easyllm/prompt_utils/__init__.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 easyllm-0.1.0/easyllm/prompt_utils/base.py
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 easyllm-0.1.0/easyllm/prompt_utils/llama2.py
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 easyllm-0.1.0/easyllm/schema/base.py
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 easyllm-0.1.0/easyllm/schema/openai.py
+-rw-r--r--   0        0        0    21202 2020-02-02 00:00:00.000000 easyllm-0.1.0/notebooks/chat-completion-api.ipynb
+-rw-r--r--   0        0        0    49822 2020-02-02 00:00:00.000000 easyllm-0.1.0/notebooks/stream-chat-completions.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 easyllm-0.1.0/scripts/.gitkeep
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 easyllm-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 easyllm-0.1.0/tests/test_main.py
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 easyllm-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 easyllm-0.1.0/LICENSE
+-rw-r--r--   0        0        0     3899 2020-02-02 00:00:00.000000 easyllm-0.1.0/README.md
+-rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 easyllm-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5754 2020-02-02 00:00:00.000000 easyllm-0.1.0/PKG-INFO
```

### Comparing `easyllm-0.0.1/.github/workflows/check.yaml` & `easyllm-0.1.0/.github/workflows/check.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
   quality:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
-          python-version: "3.8"
+          python-version: "3.9"
           cache: "pip"
           cache-dependency-path: pyproject.toml
       - uses: actions/cache@v3
         id: cache
         with:
           path: ${{ env.pythonLocation }}
           key: ${{ runner.os }}-python-${{ env.pythonLocation }}-${{ hashFiles('pyproject.toml') }}-check
```

### Comparing `easyllm-0.0.1/.github/workflows/documentation.yaml` & `easyllm-0.1.0/.github/workflows/documentation.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 name: Publish documentation
 
 on:
-  push:
-    branches:
-      - main
+  release:
+    types:
+      - created
   workflow_dispatch:
 
 concurrency:
   group: ${{ github.workflow }}-${{ github.head_ref || github.run_id }}
   cancel-in-progress: true
 
+permissions:
+  contents: write
+
 jobs:
   documentation:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
-          python-version: "3.8"
+          python-version: "3.9"
           cache: "pip"
           cache-dependency-path: pyproject.toml
       - uses: actions/cache@v3
         id: cache
         with:
           path: ${{ env.pythonLocation }}
           key: ${{ runner.os }}-python-${{ env.pythonLocation }}-${{ hashFiles('pyproject.toml') }}-docs
       - name: Install dependencies
         if: steps.cache.outputs.cache-hit != 'true'
         run: pip install ".[docs]"
       - name: publish documentation
-        run: mkdocs gh-deploy --force
+        run: make docs-deploy
```

### Comparing `easyllm-0.0.1/.github/workflows/publish.yaml` & `easyllm-0.1.0/.github/workflows/publish.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,15 @@
   publish:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
-          python-version: "3.8"
+          python-version: "3.9"
           cache: "pip"
           cache-dependency-path: pyproject.toml
       - uses: actions/cache@v3
         id: cache
         with:
           path: ${{ env.pythonLocation }}
           key: ${{ runner.os }}-python-${{ env.pythonLocation }}-${{ hashFiles('pyproject.toml') }}-publish
```

### Comparing `easyllm-0.0.1/.github/workflows/test.yaml` & `easyllm-0.1.0/.github/workflows/test.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
   quality:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
-          python-version: "3.8"
+          python-version: "3.9"
           cache: "pip"
           cache-dependency-path: pyproject.toml
       - uses: actions/cache@v3
         id: cache
         with:
           path: ${{ env.pythonLocation }}
           key: ${{ runner.os }}-python-${{ env.pythonLocation }}-${{ hashFiles('pyproject.toml') }}-test
```

### Comparing `easyllm-0.0.1/.gitignore` & `easyllm-0.1.0/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -123,8 +123,9 @@
 # mypy
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
-.ruff_cache
+.ruff_cache
+docs/notebooks/
```

### Comparing `easyllm-0.0.1/LICENSE` & `easyllm-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `easyllm-0.0.1/pyproject.toml` & `easyllm-0.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project.urls]
 Documentation = "https://github.com/unknown/hatch-demo#readme"
 Issues = "https://github.com/unknown/hatch-demo/issues"
 Source = "https://github.com/unknown/hatch-demo"
 
 [tool.hatch.version]
-path = "myproject/__init__.py"
+path = "easyllm/__init__.py"
 
 [project]
 name = "easyllm"
 description = "Description"
 readme = "README.md"
 requires-python = ">=3.8"
 license = "MIT"
@@ -23,31 +23,32 @@
   "Topic :: Software Development :: Libraries :: Python Modules",
   "Topic :: Software Development :: Libraries",
   "Topic :: Software Development",
   "Framework :: FastAPI",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python :: 3 :: Only",
-  "Programming Language :: Python :: 3.8",
+  "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
 ]
 dynamic = ["version"]
-scripts = { myproject = "myproject.cli:main" }
-dependencies = ["starlette==0.22.0"]
+scripts = { easyllm = "easyllm.cli:main" }
+dependencies = ["pydantic==2.1.1", "nanoid==2.0.0", "huggingface-hub==0.16.4"]
 
 [project.optional-dependencies]
 test = ["pytest", "ruff", "black", "isort", "mypy", "hatch"]
 dev = ["ruff", "black", "isort", "mypy", "hatch"]
 docs = [
   "mkdocs",
   "mkdocs-material",
   "mkdocstrings",
   "mkdocstrings-python",
   "mkdocs-autorefs",
+  "mkdocs-jupyter",
 ]
 
 [tool.isort]
 profile = "black"
 known_third_party = ["fastapi", "pydantic", "starlette"]
 
 # [tool.coverage.run]
@@ -79,15 +80,15 @@
 ]
 # Same as Black.
 line-length = 119
 
 # Allow unused variables when underscore-prefixed.
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
 
-# Assume Python 3.8.
+# Assume Python 3.9.
 target-version = "py38"
 
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["F401"]
 
 # [tool.ruff.isort]
 # known-third-party = ["fastapi", "pydantic", "starlette"]
```

