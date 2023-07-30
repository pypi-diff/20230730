# Comparing `tmp/html_content_extractor-0.0.2.tar.gz` & `tmp/html_content_extractor-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "html_content_extractor-0.0.2.tar", last modified: Fri Jul 28 19:04:58 2023, max compression
+gzip compressed data, was "html_content_extractor-0.0.3.tar", last modified: Sun Jul 30 00:08:09 2023, max compression
```

## Comparing `html_content_extractor-0.0.2.tar` & `html_content_extractor-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxrwxr-x   0 kevins    (1000) kevins    (1000)        0 2023-07-28 19:04:58.132373 html_content_extractor-0.0.2/
--rw-rw-r--   0 kevins    (1000) kevins    (1000)    11357 2023-07-28 01:26:01.000000 html_content_extractor-0.0.2/LICENSE
--rw-rw-r--   0 kevins    (1000) kevins    (1000)    14480 2023-07-28 19:04:58.128373 html_content_extractor-0.0.2/PKG-INFO
--rw-rw-r--   0 kevins    (1000) kevins    (1000)      806 2023-07-28 02:45:22.000000 html_content_extractor-0.0.2/README.md
-drwxrwxr-x   0 kevins    (1000) kevins    (1000)        0 2023-07-28 19:04:58.128373 html_content_extractor-0.0.2/html_content_extractor/
--rw-rw-r--   0 kevins    (1000) kevins    (1000)       39 2023-07-28 01:33:04.000000 html_content_extractor-0.0.2/html_content_extractor/__init__.py
--rw-rw-r--   0 kevins    (1000) kevins    (1000)     2358 2023-07-28 02:50:58.000000 html_content_extractor-0.0.2/html_content_extractor/extractor.py
-drwxrwxr-x   0 kevins    (1000) kevins    (1000)        0 2023-07-28 19:04:58.128373 html_content_extractor-0.0.2/html_content_extractor.egg-info/
--rw-rw-r--   0 kevins    (1000) kevins    (1000)    14480 2023-07-28 19:04:58.000000 html_content_extractor-0.0.2/html_content_extractor.egg-info/PKG-INFO
--rw-rw-r--   0 kevins    (1000) kevins    (1000)      332 2023-07-28 19:04:58.000000 html_content_extractor-0.0.2/html_content_extractor.egg-info/SOURCES.txt
--rw-rw-r--   0 kevins    (1000) kevins    (1000)        1 2023-07-28 19:04:58.000000 html_content_extractor-0.0.2/html_content_extractor.egg-info/dependency_links.txt
--rw-rw-r--   0 kevins    (1000) kevins    (1000)       43 2023-07-28 19:04:58.000000 html_content_extractor-0.0.2/html_content_extractor.egg-info/requires.txt
--rw-rw-r--   0 kevins    (1000) kevins    (1000)       23 2023-07-28 19:04:58.000000 html_content_extractor-0.0.2/html_content_extractor.egg-info/top_level.txt
--rw-rw-r--   0 kevins    (1000) kevins    (1000)      858 2023-07-28 03:18:05.000000 html_content_extractor-0.0.2/pyproject.toml
--rw-rw-r--   0 kevins    (1000) kevins    (1000)       38 2023-07-28 19:04:58.132373 html_content_extractor-0.0.2/setup.cfg
+drwxrwxr-x   0 kevins    (1000) kevins    (1000)        0 2023-07-30 00:08:09.533872 html_content_extractor-0.0.3/
+-rw-rw-r--   0 kevins    (1000) kevins    (1000)    11357 2023-07-28 01:26:01.000000 html_content_extractor-0.0.3/LICENSE
+-rw-rw-r--   0 kevins    (1000) kevins    (1000)    14406 2023-07-30 00:08:09.533872 html_content_extractor-0.0.3/PKG-INFO
+-rw-rw-r--   0 kevins    (1000) kevins    (1000)      732 2023-07-30 00:05:12.000000 html_content_extractor-0.0.3/README.md
+drwxrwxr-x   0 kevins    (1000) kevins    (1000)        0 2023-07-30 00:08:09.525872 html_content_extractor-0.0.3/html_content_extractor/
+-rw-rw-r--   0 kevins    (1000) kevins    (1000)       39 2023-07-28 01:33:04.000000 html_content_extractor-0.0.3/html_content_extractor/__init__.py
+-rw-rw-r--   0 kevins    (1000) kevins    (1000)     2527 2023-07-30 00:01:30.000000 html_content_extractor-0.0.3/html_content_extractor/extractor.py
+drwxrwxr-x   0 kevins    (1000) kevins    (1000)        0 2023-07-30 00:08:09.533872 html_content_extractor-0.0.3/html_content_extractor.egg-info/
+-rw-rw-r--   0 kevins    (1000) kevins    (1000)    14406 2023-07-30 00:08:09.000000 html_content_extractor-0.0.3/html_content_extractor.egg-info/PKG-INFO
+-rw-rw-r--   0 kevins    (1000) kevins    (1000)      368 2023-07-30 00:08:09.000000 html_content_extractor-0.0.3/html_content_extractor.egg-info/SOURCES.txt
+-rw-rw-r--   0 kevins    (1000) kevins    (1000)        1 2023-07-30 00:08:09.000000 html_content_extractor-0.0.3/html_content_extractor.egg-info/dependency_links.txt
+-rw-rw-r--   0 kevins    (1000) kevins    (1000)       43 2023-07-30 00:08:09.000000 html_content_extractor-0.0.3/html_content_extractor.egg-info/requires.txt
+-rw-rw-r--   0 kevins    (1000) kevins    (1000)       49 2023-07-30 00:08:09.000000 html_content_extractor-0.0.3/html_content_extractor.egg-info/top_level.txt
+-rw-rw-r--   0 kevins    (1000) kevins    (1000)      921 2023-07-30 00:07:51.000000 html_content_extractor-0.0.3/pyproject.toml
+-rw-rw-r--   0 kevins    (1000) kevins    (1000)       38 2023-07-30 00:08:09.533872 html_content_extractor-0.0.3/setup.cfg
+drwxrwxr-x   0 kevins    (1000) kevins    (1000)        0 2023-07-30 00:08:09.533872 html_content_extractor-0.0.3/test/
+-rw-rw-r--   0 kevins    (1000) kevins    (1000)        0 2023-07-29 22:31:27.000000 html_content_extractor-0.0.3/test/__init__.py
+-rw-rw-r--   0 kevins    (1000) kevins    (1000)     1257 2023-07-30 00:00:22.000000 html_content_extractor-0.0.3/test/playground.py
```

### Comparing `html_content_extractor-0.0.2/LICENSE` & `html_content_extractor-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `html_content_extractor-0.0.2/PKG-INFO` & `html_content_extractor-0.0.3/html_content_extractor.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: html_content_extractor
-Version: 0.0.2
+Name: html-content-extractor
+Version: 0.0.3
 Summary: A Python package to extract the main content from HTML documents
 Author-email: Kevin Sparks <pip@just-digital.net>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -212,18 +212,20 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# html-content-extractor
+# HTML Content Extractor
 
 This Python package provides a function to extract the "main content" from HTML documents.
 
+Relevancy is determined by an algorithm that favors the deepest parent with the most h1, h2, h3 and p tags.
+
 ## Installation
 
 You can install this package via pip:
 
 ```sh
 $ pip install html-content-extractor
 
@@ -240,20 +242,8 @@
 "An HTML Page\n\nThis is some HTML content."
 
 >>> markdown = extract_content(html, format='markdown')
 >>> print(content)
 "# An HTML Page\n\nThis is some HTML content."
 ```
 
-## Build
-
-```sh
-$ python3 -m pip install --upgrade build
-$ python3 -m build
-```
 
-# Publish to PyPI
-
-```sh
-$ python3 -m pip install --upgrade twine
-$ python3 -m twine upload dist/*
-```
```

### Comparing `html_content_extractor-0.0.2/html_content_extractor/extractor.py` & `html_content_extractor-0.0.3/html_content_extractor/extractor.py`

 * *Files 7% similar despite different names*

```diff
@@ -66,13 +66,18 @@
     for t in tag.find_all("img"):
         t.replace_with("")
     return tag
 
 
 def extract_content(html: str, format="plaintext"):
     soup = BeautifulSoup(html, "html.parser")
-    relevant_tag = __get_most_relevant_tag(soup)
+    relevant_tag, score = __get_most_relevant_tag(soup)
     if format == "plaintext":
         return __get_well_presented_text(relevant_tag).get_text()
     if format == "markdown":
-        return markdownify(relevant_tag)
-    return relevant_tag[0]
+        return markdownify(str(relevant_tag))
+    if format == "both":
+        return (
+            markdownify(str(relevant_tag)),
+            __get_well_presented_text(relevant_tag).get_text(),
+        )
+    return relevant_tag
```

### Comparing `html_content_extractor-0.0.2/html_content_extractor.egg-info/PKG-INFO` & `html_content_extractor-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: html-content-extractor
-Version: 0.0.2
+Name: html_content_extractor
+Version: 0.0.3
 Summary: A Python package to extract the main content from HTML documents
 Author-email: Kevin Sparks <pip@just-digital.net>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -212,18 +212,20 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# html-content-extractor
+# HTML Content Extractor
 
 This Python package provides a function to extract the "main content" from HTML documents.
 
+Relevancy is determined by an algorithm that favors the deepest parent with the most h1, h2, h3 and p tags.
+
 ## Installation
 
 You can install this package via pip:
 
 ```sh
 $ pip install html-content-extractor
 
@@ -240,20 +242,8 @@
 "An HTML Page\n\nThis is some HTML content."
 
 >>> markdown = extract_content(html, format='markdown')
 >>> print(content)
 "# An HTML Page\n\nThis is some HTML content."
 ```
 
-## Build
-
-```sh
-$ python3 -m pip install --upgrade build
-$ python3 -m build
-```
 
-# Publish to PyPI
-
-```sh
-$ python3 -m pip install --upgrade twine
-$ python3 -m twine upload dist/*
-```
```

### Comparing `html_content_extractor-0.0.2/pyproject.toml` & `html_content_extractor-0.0.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "html_content_extractor"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Kevin Sparks", email="pip@just-digital.net" },
 ]
 description = "A Python package to extract the main content from HTML documents"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -23,7 +23,10 @@
   "beautifulsoup4>=4.12.2",
   "markdownify==0.11.6"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/just-digital/html-content-extractor"
 "Bug Tracker" = "https://github.com/just-digital/html-content-extractor/issues"
+
+[tool.setuptools.packages.find]
+exclude = ["docs*", "tests*"]
```

