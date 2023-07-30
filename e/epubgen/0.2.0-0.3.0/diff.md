# Comparing `tmp/epubgen-0.2.0.tar.gz` & `tmp/epubgen-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epubgen-0.2.0.tar", last modified: Sun Jul 30 15:50:42 2023, max compression
+gzip compressed data, was "epubgen-0.3.0.tar", last modified: Sun Jul 30 15:52:39 2023, max compression
```

## Comparing `epubgen-0.2.0.tar` & `epubgen-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 sfluor     (501) staff       (20)        0 2023-07-30 15:50:42.666902 epubgen-0.2.0/
--rw-r--r--   0 sfluor     (501) staff       (20)     1067 2023-07-28 21:42:19.000000 epubgen-0.2.0/LICENSE
--rw-r--r--   0 sfluor     (501) staff       (20)      995 2023-07-30 15:50:42.665240 epubgen-0.2.0/PKG-INFO
--rw-r--r--   0 sfluor     (501) staff       (20)      506 2023-07-30 15:36:10.000000 epubgen-0.2.0/README.md
-drwxr-xr-x   0 sfluor     (501) staff       (20)        0 2023-07-30 15:50:42.660739 epubgen-0.2.0/epubgen/
--rw-r--r--   0 sfluor     (501) staff       (20)       26 2023-07-30 15:23:29.000000 epubgen-0.2.0/epubgen/__init__.py
--rw-r--r--   0 sfluor     (501) staff       (20)     7840 2023-07-30 15:34:52.000000 epubgen-0.2.0/epubgen/epubgen.py
-drwxr-xr-x   0 sfluor     (501) staff       (20)        0 2023-07-30 15:50:42.664256 epubgen-0.2.0/epubgen.egg-info/
--rw-r--r--   0 sfluor     (501) staff       (20)      995 2023-07-30 15:50:42.000000 epubgen-0.2.0/epubgen.egg-info/PKG-INFO
--rw-r--r--   0 sfluor     (501) staff       (20)      195 2023-07-30 15:50:42.000000 epubgen-0.2.0/epubgen.egg-info/SOURCES.txt
--rw-r--r--   0 sfluor     (501) staff       (20)        1 2023-07-30 15:50:42.000000 epubgen-0.2.0/epubgen.egg-info/dependency_links.txt
--rw-r--r--   0 sfluor     (501) staff       (20)        8 2023-07-30 15:50:42.000000 epubgen-0.2.0/epubgen.egg-info/top_level.txt
--rw-r--r--   0 sfluor     (501) staff       (20)      560 2023-07-30 15:50:34.000000 epubgen-0.2.0/pyproject.toml
--rw-r--r--   0 sfluor     (501) staff       (20)       38 2023-07-30 15:50:42.667456 epubgen-0.2.0/setup.cfg
+drwxr-xr-x   0 sfluor     (501) staff       (20)        0 2023-07-30 15:52:39.711933 epubgen-0.3.0/
+-rw-r--r--   0 sfluor     (501) staff       (20)     1067 2023-07-28 21:42:19.000000 epubgen-0.3.0/LICENSE
+-rw-r--r--   0 sfluor     (501) staff       (20)      995 2023-07-30 15:52:39.711386 epubgen-0.3.0/PKG-INFO
+-rw-r--r--   0 sfluor     (501) staff       (20)      506 2023-07-30 15:36:10.000000 epubgen-0.3.0/README.md
+drwxr-xr-x   0 sfluor     (501) staff       (20)        0 2023-07-30 15:52:39.707720 epubgen-0.3.0/epubgen/
+-rw-r--r--   0 sfluor     (501) staff       (20)       26 2023-07-30 15:23:29.000000 epubgen-0.3.0/epubgen/__init__.py
+-rw-r--r--   0 sfluor     (501) staff       (20)     7859 2023-07-30 15:52:12.000000 epubgen-0.3.0/epubgen/epubgen.py
+drwxr-xr-x   0 sfluor     (501) staff       (20)        0 2023-07-30 15:52:39.710947 epubgen-0.3.0/epubgen.egg-info/
+-rw-r--r--   0 sfluor     (501) staff       (20)      995 2023-07-30 15:52:39.000000 epubgen-0.3.0/epubgen.egg-info/PKG-INFO
+-rw-r--r--   0 sfluor     (501) staff       (20)      195 2023-07-30 15:52:39.000000 epubgen-0.3.0/epubgen.egg-info/SOURCES.txt
+-rw-r--r--   0 sfluor     (501) staff       (20)        1 2023-07-30 15:52:39.000000 epubgen-0.3.0/epubgen.egg-info/dependency_links.txt
+-rw-r--r--   0 sfluor     (501) staff       (20)        8 2023-07-30 15:52:39.000000 epubgen-0.3.0/epubgen.egg-info/top_level.txt
+-rw-r--r--   0 sfluor     (501) staff       (20)      560 2023-07-30 15:52:18.000000 epubgen-0.3.0/pyproject.toml
+-rw-r--r--   0 sfluor     (501) staff       (20)       38 2023-07-30 15:52:39.712066 epubgen-0.3.0/setup.cfg
```

### Comparing `epubgen-0.2.0/LICENSE` & `epubgen-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `epubgen-0.2.0/PKG-INFO` & `epubgen-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epubgen
-Version: 0.2.0
+Version: 0.3.0
 Summary: Tiny library to programmatically generate .epub files
 Author: Sami Tabet
 Project-URL: Homepage, https://github.com/sfluor/epubgen
 Project-URL: Bug Tracker, https://github.com/sfluor/epubgen/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `epubgen-0.2.0/epubgen/epubgen.py` & `epubgen-0.3.0/epubgen/epubgen.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,25 +30,28 @@
 
     Methods
     -------
     - add_page: add content to the EPUB
     - add_image: embed images in the EPUB
     - generate_epub: generate the EPUB file
     """
-    def __init__(self, title: str, author: str, language: str, id: str, css="", rtl=False):
+
+    def __init__(
+        self, title: str, author: str, language: str, id: str, css="", rtl=False
+    ):
+        self.id: str = id
+        self.rtl: bool = rtl
         self.metadata: ET.Element = self._generate_pkg_metadata(title, author, language)
         self.manifest: ET.Element = ET.Element("manifest")
-        self.rtl: bool = rtl
         spine_attrs = {}
         if self.rtl:
             spine_attrs["page-progression-direction"] = "rtl"
         self.spine: ET.Element = ET.Element("spine", attrib=spine_attrs)
         self.toc = ET.Element("ol")
         self.css = css
-        self.id = id
 
         # Add the table of contents to the spine and the manifest
         self._add_to_manifest_and_spine(TOC_ID, TOC_PATH, properties="nav")
 
         self.page_counts: int = 0
         self.contents: list[tuple[str, str | bytes]] = [
             ("mimetype", "application/epub+zip"),
@@ -209,15 +212,14 @@
 
         if toc_title is not None:
             li = ET.Element("li")
             link = ET.SubElement(li, "a", href=path)
             link.text = toc_title
             self.toc.append(li)
 
-
     def generate_epub(self, path: str):
         """
         Generates the EPUB and saves it at the provided path.
         """
         contents = self.contents + [
             (CONTENT_ROOT + TOC_PATH, self._generate_toc()),
             (PACKAGE_PATH, self._generate_pkg_opf()),
```

### Comparing `epubgen-0.2.0/epubgen.egg-info/PKG-INFO` & `epubgen-0.3.0/epubgen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epubgen
-Version: 0.2.0
+Version: 0.3.0
 Summary: Tiny library to programmatically generate .epub files
 Author: Sami Tabet
 Project-URL: Homepage, https://github.com/sfluor/epubgen
 Project-URL: Bug Tracker, https://github.com/sfluor/epubgen/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `epubgen-0.2.0/pyproject.toml` & `epubgen-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "epubgen"
-version = "0.2.0"
+version = "0.3.0"
 authors = [{ name = "Sami Tabet" }]
 description = "Tiny library to programmatically generate .epub files"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

