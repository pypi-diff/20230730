# Comparing `tmp/webint_code-0.0.22.tar.gz` & `tmp/webint_code-0.0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webint_code-0.0.22.tar", max compression
+gzip compressed data, was "webint_code-0.0.23.tar", max compression
```

## Comparing `webint_code-0.0.22.tar` & `webint_code-0.0.23.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1131 2023-05-20 02:29:42.503980 webint_code-0.0.22/pyproject.toml
--rw-r--r--   0        0        0    19164 2023-05-20 01:56:58.382846 webint_code-0.0.22/webint_code/__init__.py
--rw-r--r--   0        0        0      474 2023-01-27 00:43:27.567919 webint_code-0.0.22/webint_code/templates/__init__.py
--rw-r--r--   0        0        0      161 2023-02-20 19:30:47.711101 webint_code-0.0.22/webint_code/templates/index.html
--rw-r--r--   0        0        0     1225 2023-01-27 00:43:27.575919 webint_code-0.0.22/webint_code/templates/project/commit.html
--rw-r--r--   0        0        0      651 2023-01-27 00:43:27.567919 webint_code-0.0.22/webint_code/templates/project/commit_log.html
--rw-r--r--   0        0        0      116 2023-01-27 00:43:27.571919 webint_code-0.0.22/webint_code/templates/project/created.html
--rw-r--r--   0        0        0    10118 2023-01-27 00:43:27.571919 webint_code-0.0.22/webint_code/templates/project/index.html
--rw-r--r--   0        0        0      872 2023-01-27 00:43:27.575919 webint_code-0.0.22/webint_code/templates/project/issues.html
--rw-r--r--   0        0        0     2921 2023-01-27 00:43:27.571919 webint_code-0.0.22/webint_code/templates/project/namespace.html
--rw-r--r--   0        0        0      294 2023-01-27 00:43:27.571919 webint_code-0.0.22/webint_code/templates/project/release.html
--rw-r--r--   0        0        0      777 2023-01-27 00:43:27.575919 webint_code-0.0.22/webint_code/templates/project/release_file.html
--rw-r--r--   0        0        0     1063 2023-05-20 02:29:12.683472 webint_code-0.0.22/webint_code/templates/project/repository_file.html
--rw-r--r--   0        0        0      485 2023-01-27 00:43:27.575919 webint_code-0.0.22/webint_code/templates/project/settings.html
--rw-r--r--   0        0        0      373 2023-01-27 00:43:27.579919 webint_code-0.0.22/webint_code/templates/projects.html
--rw-r--r--   0        0        0      136 2023-01-27 00:43:27.579919 webint_code-0.0.22/webint_code/templates/pypi/index.html
--rw-r--r--   0        0        0      227 2023-01-27 00:43:27.579919 webint_code-0.0.22/webint_code/templates/pypi/project.html
--rw-r--r--   0        0        0       87 2023-01-27 00:43:27.579919 webint_code-0.0.22/webint_code/templates/search/index.html
--rw-r--r--   0        0        0     1029 2023-01-27 00:43:27.583919 webint_code-0.0.22/webint_code/templates/search/results.html
--rw-r--r--   0        0        0     4967 2023-05-18 23:21:54.011448 webint_code-0.0.22/webint_code/templates/system.html
--rw-r--r--   0        0        0      149 2023-01-27 00:43:27.567919 webint_code-0.0.22/webint_code/templates/template.html
--rw-r--r--   0        0        0      905 1970-01-01 00:00:00.000000 webint_code-0.0.22/setup.py
--rw-r--r--   0        0        0      729 1970-01-01 00:00:00.000000 webint_code-0.0.22/PKG-INFO
+-rw-r--r--   0        0        0     1131 2023-07-30 01:57:25.106895 webint_code-0.0.23/pyproject.toml
+-rw-r--r--   0        0        0    19176 2023-07-30 01:42:02.236213 webint_code-0.0.23/webint_code/__init__.py
+-rw-r--r--   0        0        0      474 2023-01-27 00:43:27.567919 webint_code-0.0.23/webint_code/templates/__init__.py
+-rw-r--r--   0        0        0      161 2023-02-20 19:30:47.711101 webint_code-0.0.23/webint_code/templates/index.html
+-rw-r--r--   0        0        0     1225 2023-01-27 00:43:27.575919 webint_code-0.0.23/webint_code/templates/project/commit.html
+-rw-r--r--   0        0        0      651 2023-01-27 00:43:27.567919 webint_code-0.0.23/webint_code/templates/project/commit_log.html
+-rw-r--r--   0        0        0      116 2023-01-27 00:43:27.571919 webint_code-0.0.23/webint_code/templates/project/created.html
+-rw-r--r--   0        0        0    10118 2023-01-27 00:43:27.571919 webint_code-0.0.23/webint_code/templates/project/index.html
+-rw-r--r--   0        0        0      872 2023-01-27 00:43:27.575919 webint_code-0.0.23/webint_code/templates/project/issues.html
+-rw-r--r--   0        0        0     2921 2023-01-27 00:43:27.571919 webint_code-0.0.23/webint_code/templates/project/namespace.html
+-rw-r--r--   0        0        0      294 2023-01-27 00:43:27.571919 webint_code-0.0.23/webint_code/templates/project/release.html
+-rw-r--r--   0        0        0      777 2023-01-27 00:43:27.575919 webint_code-0.0.23/webint_code/templates/project/release_file.html
+-rw-r--r--   0        0        0     1063 2023-05-20 02:42:12.401245 webint_code-0.0.23/webint_code/templates/project/repository_file.html
+-rw-r--r--   0        0        0      485 2023-01-27 00:43:27.575919 webint_code-0.0.23/webint_code/templates/project/settings.html
+-rw-r--r--   0        0        0      373 2023-01-27 00:43:27.579919 webint_code-0.0.23/webint_code/templates/projects.html
+-rw-r--r--   0        0        0      136 2023-01-27 00:43:27.579919 webint_code-0.0.23/webint_code/templates/pypi/index.html
+-rw-r--r--   0        0        0      227 2023-01-27 00:43:27.579919 webint_code-0.0.23/webint_code/templates/pypi/project.html
+-rw-r--r--   0        0        0       87 2023-01-27 00:43:27.579919 webint_code-0.0.23/webint_code/templates/search/index.html
+-rw-r--r--   0        0        0     1029 2023-01-27 00:43:27.583919 webint_code-0.0.23/webint_code/templates/search/results.html
+-rw-r--r--   0        0        0     4967 2023-05-18 23:21:54.011448 webint_code-0.0.23/webint_code/templates/system.html
+-rw-r--r--   0        0        0      149 2023-01-27 00:43:27.567919 webint_code-0.0.23/webint_code/templates/template.html
+-rw-r--r--   0        0        0      905 1970-01-01 00:00:00.000000 webint_code-0.0.23/setup.py
+-rw-r--r--   0        0        0      729 1970-01-01 00:00:00.000000 webint_code-0.0.23/PKG-INFO
```

### Comparing `webint_code-0.0.22/pyproject.toml` & `webint_code-0.0.23/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "webint-code"
-version = "0.0.22"
+version = "0.0.23"
 description = "manage code on your website"
 keywords = ["webint", "Git", "PyPI"]
 homepage = "https://ragt.ag/code/projects/webint-code"
 repository = "https://ragt.ag/code/projects/webint-code.git"
 documentation = "https://ragt.ag/code/projects/webint-code/api"
 authors = ["Angelo Gladding <angelo@ragt.ag>"]
 license = "BSD-2-Clause"
```

### Comparing `webint_code-0.0.22/webint_code/__init__.py` & `webint_code-0.0.23/webint_code/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -158,15 +158,15 @@
     repo.config("http.receivepack", "true")
     post_receive_hook = bare_repo / "hooks/post-receive"
     with post_receive_hook.open("w") as fp:
         fp.write(
             "\n".join(
                 (
                     "#!/bin/sh",
-                    "git -C $PWD/../working --git-dir=.git pull --rebase",
+                    "git -C $PWD/../working --git-dir=.git pull origin main --rebase",
                     f"wget --method=post -qO- {web.tx.origin}/code/projects/{name}",
                 )
             )
         )
     gmpg.clone_repo(bare_repo, working_repo)
     subprocess.run(["chmod", "775", post_receive_hook])
     subprocess.run(["chgrp", "www-data", bare_repo, working_repo, "-R"])
```

### Comparing `webint_code-0.0.22/webint_code/templates/project/commit.html` & `webint_code-0.0.23/webint_code/templates/project/commit.html`

 * *Files identical despite different names*

### Comparing `webint_code-0.0.22/webint_code/templates/project/commit_log.html` & `webint_code-0.0.23/webint_code/templates/project/commit_log.html`

 * *Files identical despite different names*

### Comparing `webint_code-0.0.22/webint_code/templates/project/index.html` & `webint_code-0.0.23/webint_code/templates/project/index.html`

 * *Files identical despite different names*

### Comparing `webint_code-0.0.22/webint_code/templates/project/issues.html` & `webint_code-0.0.23/webint_code/templates/project/issues.html`

 * *Files identical despite different names*

### Comparing `webint_code-0.0.22/webint_code/templates/project/namespace.html` & `webint_code-0.0.23/webint_code/templates/project/namespace.html`

 * *Files identical despite different names*

### Comparing `webint_code-0.0.22/webint_code/templates/project/release_file.html` & `webint_code-0.0.23/webint_code/templates/project/release_file.html`

 * *Files identical despite different names*

### Comparing `webint_code-0.0.22/webint_code/templates/project/repository_file.html` & `webint_code-0.0.23/webint_code/templates/project/repository_file.html`

 * *Files identical despite different names*

### Comparing `webint_code-0.0.22/webint_code/templates/search/results.html` & `webint_code-0.0.23/webint_code/templates/search/results.html`

 * *Files identical despite different names*

### Comparing `webint_code-0.0.22/webint_code/templates/system.html` & `webint_code-0.0.23/webint_code/templates/system.html`

 * *Files identical despite different names*

### Comparing `webint_code-0.0.22/setup.py` & `webint_code-0.0.23/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'webint>=0.0']
 
 entry_points = \
 {'webapps': ['code = webint_code:app']}
 
 setup_kwargs = {
     'name': 'webint-code',
-    'version': '0.0.22',
+    'version': '0.0.23',
     'description': 'manage code on your website',
     'long_description': 'None',
     'author': 'Angelo Gladding',
     'author_email': 'angelo@ragt.ag',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://ragt.ag/code/projects/webint-code',
```

### Comparing `webint_code-0.0.22/PKG-INFO` & `webint_code-0.0.23/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webint-code
-Version: 0.0.22
+Version: 0.0.23
 Summary: manage code on your website
 Home-page: https://ragt.ag/code/projects/webint-code
 License: BSD-2-Clause
 Keywords: webint,Git,PyPI
 Author: Angelo Gladding
 Author-email: angelo@ragt.ag
 Requires-Python: >=3.10,<3.11
```

