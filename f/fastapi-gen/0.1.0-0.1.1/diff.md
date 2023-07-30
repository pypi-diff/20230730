# Comparing `tmp/fastapi_gen-0.1.0.tar.gz` & `tmp/fastapi_gen-0.1.1.tar.gz`

## Comparing `fastapi_gen-0.1.0.tar` & `fastapi_gen-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_gen-0.1.0/src/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fastapi_gen-0.1.0/src/cli/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_gen-0.1.0/src/cli/__init__.py
--rw-r--r--   0        0        0     2875 2020-02-02 00:00:00.000000 fastapi_gen-0.1.0/src/cli/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_gen-0.1.0/src/templates/__init__.py
--rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 fastapi_gen-0.1.0/src/templates/hello_world/.gitignore
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 fastapi_gen-0.1.0/src/templates/hello_world/Makefile
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 fastapi_gen-0.1.0/src/templates/hello_world/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_gen-0.1.0/src/templates/hello_world/__init__.py
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 fastapi_gen-0.1.0/src/templates/hello_world/main.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 fastapi_gen-0.1.0/src/templates/hello_world/requirements.txt
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 fastapi_gen-0.1.0/src/templates/hello_world/test_main.py
--rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 fastapi_gen-0.1.0/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 fastapi_gen-0.1.0/LICENSE
--rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 fastapi_gen-0.1.0/README.md
--rw-r--r--   0        0        0     3808 2020-02-02 00:00:00.000000 fastapi_gen-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4230 2020-02-02 00:00:00.000000 fastapi_gen-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_gen-0.1.1/src/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fastapi_gen-0.1.1/src/cli/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_gen-0.1.1/src/cli/__init__.py
+-rw-r--r--   0        0        0     2871 2020-02-02 00:00:00.000000 fastapi_gen-0.1.1/src/cli/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_gen-0.1.1/src/templates/__init__.py
+-rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 fastapi_gen-0.1.1/src/templates/hello_world/.gitignore
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 fastapi_gen-0.1.1/src/templates/hello_world/Makefile
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 fastapi_gen-0.1.1/src/templates/hello_world/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_gen-0.1.1/src/templates/hello_world/__init__.py
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 fastapi_gen-0.1.1/src/templates/hello_world/main.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 fastapi_gen-0.1.1/src/templates/hello_world/requirements.txt
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 fastapi_gen-0.1.1/src/templates/hello_world/test_main.py
+-rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 fastapi_gen-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 fastapi_gen-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 fastapi_gen-0.1.1/README.md
+-rw-r--r--   0        0        0     3808 2020-02-02 00:00:00.000000 fastapi_gen-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4266 2020-02-02 00:00:00.000000 fastapi_gen-0.1.1/PKG-INFO
```

### Comparing `fastapi_gen-0.1.0/src/cli/__main__.py` & `fastapi_gen-0.1.1/src/cli/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 
     {click.style('make lint', bg='blue', fg='white')}
     Starts linters.
 
 We suggest that you begin by typing:
 
     {click.style(f'cd {name}', bg='blue', fg='white')}
-    {click.style('make start-dev', bg='blue', fg='white')}
+    {click.style('make start', bg='blue', fg='white')}
 
 {click.style('Happy hacking!', blink=True, bold=True)}
 """
     click.echo(welcome_message)
 
 
 sys.exit(fastapi_create())
```

### Comparing `fastapi_gen-0.1.0/src/templates/hello_world/.gitignore` & `fastapi_gen-0.1.1/src/templates/hello_world/.gitignore`

 * *Files identical despite different names*

### Comparing `fastapi_gen-0.1.0/src/templates/hello_world/README.md` & `fastapi_gen-0.1.1/src/templates/hello_world/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_gen-0.1.0/src/templates/hello_world/main.py` & `fastapi_gen-0.1.1/src/templates/hello_world/main.py`

 * *Files identical despite different names*

### Comparing `fastapi_gen-0.1.0/src/templates/hello_world/test_main.py` & `fastapi_gen-0.1.1/src/templates/hello_world/test_main.py`

 * *Files identical despite different names*

### Comparing `fastapi_gen-0.1.0/.gitignore` & `fastapi_gen-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `fastapi_gen-0.1.0/LICENSE` & `fastapi_gen-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_gen-0.1.0/README.md` & `fastapi_gen-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,29 +9,29 @@
 
 1. Default - basic template with GET/POST examples.
 2. More to come!
 
 ## Quick Overview
 
 ```console
-pip install fastapi-gen
+pip3 install fastapi-gen
 fastapi-gen my_app
 cd my_app
 make start-dev
 ```
 
 or 
 
 ```console
-pipx fastapi-gen my_app
+pipx run fastapi-gen my_app
 cd my_app
 make start-dev
 ```
 
-If you've previously installed `fastapi-gen` globally via `pip install fastapi-gen`, we recommend you reinstall the package using `pip install fastapi-gen` or `pipx upgrade fastapi-gen` to ensure that you use the latest version.
+If you've previously installed `fastapi-gen` globally via `pip3 install fastapi-gen`, we recommend you reinstall the package using `pip3 install --upgrade --force-reinstall fastapi-gen` or `pipx upgrade fastapi-gen` to ensure that you use the latest version.
 
 Then open http://localhost:8000/docs to see your app OpenAPI documentation.
 
 ### Get Started Immediately
 
 You **don’t** need to install or configure depencendeices like FastApi or Pytest.<br>
 They are preconfigured and hidden so that you can focus on the code.
@@ -41,22 +41,22 @@
 ## Creating an App
 
 **You’ll need to have Python 3.7+ or later version on your local development machine**. We recommend using the latest LTS version. You can use [pyenv](https://github.com/pyenv/pyenv) (macOS/Linux) to switch Python versions between different projects.
 
 ### basic template
 
 ```console
-pip install fastapi-gen
+pip3 install fastapi-gen
 fastapi-gen my_app
 ```
 
 or
 
 ```console
-pip install fastapi-gen 
+pip3 install fastapi-gen
 fastapi-gen my_app --template hello_world
 ```
 
 Inside the newly created project, you can run some built-in commands:
 
 ### `make start`
```

### Comparing `fastapi_gen-0.1.0/pyproject.toml` & `fastapi_gen-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fastapi_gen-0.1.0/PKG-INFO` & `fastapi_gen-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-gen
-Version: 0.1.0
+Version: 0.1.1
 Summary: Set up a modern REST API by running one command.
 Project-URL: Documentation, https://github.com/mirpo/fastapi-gen#readme
 Project-URL: Issues, https://github.com/mirpo/fastapi-gen/issues
 Project-URL: Source, https://github.com/mirpo/fastapi-gen
 Author-email: Miroslav Pokrovskii <miroslavpokrovskiy@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -58,29 +58,29 @@
 
 1. Default - basic template with GET/POST examples.
 2. More to come!
 
 ## Quick Overview
 
 ```console
-pip install fastapi-gen
+pip3 install fastapi-gen
 fastapi-gen my_app
 cd my_app
 make start-dev
 ```
 
 or 
 
 ```console
-pipx fastapi-gen my_app
+pipx run fastapi-gen my_app
 cd my_app
 make start-dev
 ```
 
-If you've previously installed `fastapi-gen` globally via `pip install fastapi-gen`, we recommend you reinstall the package using `pip install fastapi-gen` or `pipx upgrade fastapi-gen` to ensure that you use the latest version.
+If you've previously installed `fastapi-gen` globally via `pip3 install fastapi-gen`, we recommend you reinstall the package using `pip3 install --upgrade --force-reinstall fastapi-gen` or `pipx upgrade fastapi-gen` to ensure that you use the latest version.
 
 Then open http://localhost:8000/docs to see your app OpenAPI documentation.
 
 ### Get Started Immediately
 
 You **don’t** need to install or configure depencendeices like FastApi or Pytest.<br>
 They are preconfigured and hidden so that you can focus on the code.
@@ -90,22 +90,22 @@
 ## Creating an App
 
 **You’ll need to have Python 3.7+ or later version on your local development machine**. We recommend using the latest LTS version. You can use [pyenv](https://github.com/pyenv/pyenv) (macOS/Linux) to switch Python versions between different projects.
 
 ### basic template
 
 ```console
-pip install fastapi-gen
+pip3 install fastapi-gen
 fastapi-gen my_app
 ```
 
 or
 
 ```console
-pip install fastapi-gen 
+pip3 install fastapi-gen
 fastapi-gen my_app --template hello_world
 ```
 
 Inside the newly created project, you can run some built-in commands:
 
 ### `make start`
```

