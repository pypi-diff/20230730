# Comparing `tmp/jira2markdown-0.3.5.tar.gz` & `tmp/jira2markdown-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jira2markdown-0.3.5.tar", max compression
+gzip compressed data, was "jira2markdown-0.3.6.tar", max compression
```

## Comparing `jira2markdown-0.3.5.tar` & `jira2markdown-0.3.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1073 2023-04-13 06:40:47.028860 jira2markdown-0.3.5/LICENSE
--rw-r--r--   0        0        0     6011 2023-04-06 17:32:37.179554 jira2markdown-0.3.5/README.md
--rw-r--r--   0        0        0       36 2021-01-31 16:47:22.204367 jira2markdown-0.3.5/jira2markdown/__init__.py
--rw-r--r--   0        0        0     2328 2023-07-25 05:53:49.752348 jira2markdown-0.3.5/jira2markdown/elements.py
--rw-r--r--   0        0        0        0 2021-01-31 17:11:54.757777 jira2markdown-0.3.5/jira2markdown/markup/__init__.py
--rw-r--r--   0        0        0     2207 2022-12-06 15:24:24.761173 jira2markdown-0.3.5/jira2markdown/markup/advanced.py
--rw-r--r--   0        0        0      477 2022-11-24 18:33:27.195584 jira2markdown-0.3.5/jira2markdown/markup/base.py
--rw-r--r--   0        0        0      762 2022-12-06 15:24:24.761173 jira2markdown-0.3.5/jira2markdown/markup/headings.py
--rw-r--r--   0        0        0     1555 2023-04-06 17:32:37.179554 jira2markdown-0.3.5/jira2markdown/markup/images.py
--rw-r--r--   0        0        0     3076 2023-02-03 14:53:07.283223 jira2markdown-0.3.5/jira2markdown/markup/links.py
--rw-r--r--   0        0        0     4074 2022-12-10 09:48:27.736671 jira2markdown-0.3.5/jira2markdown/markup/lists.py
--rw-r--r--   0        0        0     2213 2022-12-06 15:24:24.762173 jira2markdown-0.3.5/jira2markdown/markup/tables.py
--rw-r--r--   0        0        0     1230 2022-12-06 15:24:24.762173 jira2markdown-0.3.5/jira2markdown/markup/text_breaks.py
--rw-r--r--   0        0        0     5456 2023-07-25 06:16:48.249860 jira2markdown-0.3.5/jira2markdown/markup/text_effects.py
--rw-r--r--   0        0        0      646 2023-07-25 05:58:38.085341 jira2markdown-0.3.5/jira2markdown/parser.py
--rw-r--r--   0        0        0     1111 2023-07-26 05:58:41.464475 jira2markdown-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     7026 1970-01-01 00:00:00.000000 jira2markdown-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-13 06:40:47.028860 jira2markdown-0.3.6/LICENSE
+-rw-r--r--   0        0        0     6011 2023-04-06 17:32:37.179554 jira2markdown-0.3.6/README.md
+-rw-r--r--   0        0        0       36 2021-01-31 16:47:22.204367 jira2markdown-0.3.6/jira2markdown/__init__.py
+-rw-r--r--   0        0        0     2328 2023-07-25 05:53:49.752348 jira2markdown-0.3.6/jira2markdown/elements.py
+-rw-r--r--   0        0        0        0 2021-01-31 17:11:54.757777 jira2markdown-0.3.6/jira2markdown/markup/__init__.py
+-rw-r--r--   0        0        0     2207 2022-12-06 15:24:24.761173 jira2markdown-0.3.6/jira2markdown/markup/advanced.py
+-rw-r--r--   0        0        0      477 2022-11-24 18:33:27.195584 jira2markdown-0.3.6/jira2markdown/markup/base.py
+-rw-r--r--   0        0        0      762 2022-12-06 15:24:24.761173 jira2markdown-0.3.6/jira2markdown/markup/headings.py
+-rw-r--r--   0        0        0     1555 2023-04-06 17:32:37.179554 jira2markdown-0.3.6/jira2markdown/markup/images.py
+-rw-r--r--   0        0        0     3076 2023-02-03 14:53:07.283223 jira2markdown-0.3.6/jira2markdown/markup/links.py
+-rw-r--r--   0        0        0     4074 2022-12-10 09:48:27.736671 jira2markdown-0.3.6/jira2markdown/markup/lists.py
+-rw-r--r--   0        0        0     2213 2022-12-06 15:24:24.762173 jira2markdown-0.3.6/jira2markdown/markup/tables.py
+-rw-r--r--   0        0        0     1230 2022-12-06 15:24:24.762173 jira2markdown-0.3.6/jira2markdown/markup/text_breaks.py
+-rw-r--r--   0        0        0     5456 2023-07-25 06:16:48.249860 jira2markdown-0.3.6/jira2markdown/markup/text_effects.py
+-rw-r--r--   0        0        0      646 2023-07-25 05:58:38.085341 jira2markdown-0.3.6/jira2markdown/parser.py
+-rw-r--r--   0        0        0     1105 2023-07-30 15:20:18.803638 jira2markdown-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     7016 1970-01-01 00:00:00.000000 jira2markdown-0.3.6/PKG-INFO
```

### Comparing `jira2markdown-0.3.5/LICENSE` & `jira2markdown-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `jira2markdown-0.3.5/README.md` & `jira2markdown-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `jira2markdown-0.3.5/jira2markdown/elements.py` & `jira2markdown-0.3.6/jira2markdown/elements.py`

 * *Files identical despite different names*

### Comparing `jira2markdown-0.3.5/jira2markdown/markup/advanced.py` & `jira2markdown-0.3.6/jira2markdown/markup/advanced.py`

 * *Files identical despite different names*

### Comparing `jira2markdown-0.3.5/jira2markdown/markup/headings.py` & `jira2markdown-0.3.6/jira2markdown/markup/headings.py`

 * *Files identical despite different names*

### Comparing `jira2markdown-0.3.5/jira2markdown/markup/images.py` & `jira2markdown-0.3.6/jira2markdown/markup/images.py`

 * *Files identical despite different names*

### Comparing `jira2markdown-0.3.5/jira2markdown/markup/links.py` & `jira2markdown-0.3.6/jira2markdown/markup/links.py`

 * *Files identical despite different names*

### Comparing `jira2markdown-0.3.5/jira2markdown/markup/lists.py` & `jira2markdown-0.3.6/jira2markdown/markup/lists.py`

 * *Files identical despite different names*

### Comparing `jira2markdown-0.3.5/jira2markdown/markup/tables.py` & `jira2markdown-0.3.6/jira2markdown/markup/tables.py`

 * *Files identical despite different names*

### Comparing `jira2markdown-0.3.5/jira2markdown/markup/text_breaks.py` & `jira2markdown-0.3.6/jira2markdown/markup/text_breaks.py`

 * *Files identical despite different names*

### Comparing `jira2markdown-0.3.5/jira2markdown/markup/text_effects.py` & `jira2markdown-0.3.6/jira2markdown/markup/text_effects.py`

 * *Files identical despite different names*

### Comparing `jira2markdown-0.3.5/jira2markdown/parser.py` & `jira2markdown-0.3.6/jira2markdown/parser.py`

 * *Files identical despite different names*

### Comparing `jira2markdown-0.3.5/pyproject.toml` & `jira2markdown-0.3.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jira2markdown"
-version = "0.3.5"
+version = "0.3.6"
 description = "Convert text from JIRA markup to Markdown using parsing expression grammars"
 license = "MIT"
 authors = ["Evgeniy Krysanov <evgeniy.krysanov@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/catcombo/jira2markdown"
 packages = [
     { include = "jira2markdown" },
@@ -17,15 +17,15 @@
     "Programming Language :: Python :: 3",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
-pyparsing = "==3.0.9"
+pyparsing = "*"
 
 [tool.poetry.dev-dependencies]
 pytest = "*"
 
 black = "*"
 flake8 = "*"
 flake8-black = "*"
```

### Comparing `jira2markdown-0.3.5/PKG-INFO` & `jira2markdown-0.3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jira2markdown
-Version: 0.3.5
+Version: 0.3.6
 Summary: Convert text from JIRA markup to Markdown using parsing expression grammars
 Home-page: https://github.com/catcombo/jira2markdown
 License: MIT
 Keywords: jira,markdown
 Author: Evgeniy Krysanov
 Author-email: evgeniy.krysanov@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Text Processing :: Markup
 Classifier: Topic :: Text Processing :: Markup :: Markdown
-Requires-Dist: pyparsing (==3.0.9)
+Requires-Dist: pyparsing
 Project-URL: Repository, https://github.com/catcombo/jira2markdown
 Description-Content-Type: text/markdown
 
 # Overview
 
 `jira2markdown` is a text converter from [JIRA markup](https://jira.atlassian.com/secure/WikiRendererHelpAction.jspa?section=all) to [YouTrack Markdown](https://www.jetbrains.com/help/youtrack/standalone/youtrack-markdown-syntax-issues.html) using parsing expression grammars. The Markdown implementation in YouTrack follows the [CommonMark specification](https://spec.commonmark.org/0.29/) with extensions. Thus, `jira2markdown` can be used to convert text to any Markdown syntax with minimal modifications.
```

