# Comparing `tmp/epubgen-0.3.0.tar.gz` & `tmp/epubgen-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epubgen-0.3.0.tar", last modified: Sun Jul 30 15:52:39 2023, max compression
+gzip compressed data, was "epubgen-0.4.0.tar", last modified: Sun Jul 30 17:56:44 2023, max compression
```

## Comparing `epubgen-0.3.0.tar` & `epubgen-0.4.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 sfluor     (501) staff       (20)        0 2023-07-30 15:52:39.711933 epubgen-0.3.0/
--rw-r--r--   0 sfluor     (501) staff       (20)     1067 2023-07-28 21:42:19.000000 epubgen-0.3.0/LICENSE
--rw-r--r--   0 sfluor     (501) staff       (20)      995 2023-07-30 15:52:39.711386 epubgen-0.3.0/PKG-INFO
--rw-r--r--   0 sfluor     (501) staff       (20)      506 2023-07-30 15:36:10.000000 epubgen-0.3.0/README.md
-drwxr-xr-x   0 sfluor     (501) staff       (20)        0 2023-07-30 15:52:39.707720 epubgen-0.3.0/epubgen/
--rw-r--r--   0 sfluor     (501) staff       (20)       26 2023-07-30 15:23:29.000000 epubgen-0.3.0/epubgen/__init__.py
--rw-r--r--   0 sfluor     (501) staff       (20)     7859 2023-07-30 15:52:12.000000 epubgen-0.3.0/epubgen/epubgen.py
-drwxr-xr-x   0 sfluor     (501) staff       (20)        0 2023-07-30 15:52:39.710947 epubgen-0.3.0/epubgen.egg-info/
--rw-r--r--   0 sfluor     (501) staff       (20)      995 2023-07-30 15:52:39.000000 epubgen-0.3.0/epubgen.egg-info/PKG-INFO
--rw-r--r--   0 sfluor     (501) staff       (20)      195 2023-07-30 15:52:39.000000 epubgen-0.3.0/epubgen.egg-info/SOURCES.txt
--rw-r--r--   0 sfluor     (501) staff       (20)        1 2023-07-30 15:52:39.000000 epubgen-0.3.0/epubgen.egg-info/dependency_links.txt
--rw-r--r--   0 sfluor     (501) staff       (20)        8 2023-07-30 15:52:39.000000 epubgen-0.3.0/epubgen.egg-info/top_level.txt
--rw-r--r--   0 sfluor     (501) staff       (20)      560 2023-07-30 15:52:18.000000 epubgen-0.3.0/pyproject.toml
--rw-r--r--   0 sfluor     (501) staff       (20)       38 2023-07-30 15:52:39.712066 epubgen-0.3.0/setup.cfg
+drwxr-xr-x   0 sfluor     (501) staff       (20)        0 2023-07-30 17:56:44.636527 epubgen-0.4.0/
+-rw-r--r--   0 sfluor     (501) staff       (20)     1067 2023-07-28 21:42:19.000000 epubgen-0.4.0/LICENSE
+-rw-r--r--   0 sfluor     (501) staff       (20)      995 2023-07-30 17:56:44.636102 epubgen-0.4.0/PKG-INFO
+-rw-r--r--   0 sfluor     (501) staff       (20)      506 2023-07-30 15:36:10.000000 epubgen-0.4.0/README.md
+drwxr-xr-x   0 sfluor     (501) staff       (20)        0 2023-07-30 17:56:44.633363 epubgen-0.4.0/epubgen/
+-rw-r--r--   0 sfluor     (501) staff       (20)       26 2023-07-30 15:23:29.000000 epubgen-0.4.0/epubgen/__init__.py
+-rw-r--r--   0 sfluor     (501) staff       (20)     8502 2023-07-30 17:55:17.000000 epubgen-0.4.0/epubgen/epubgen.py
+drwxr-xr-x   0 sfluor     (501) staff       (20)        0 2023-07-30 17:56:44.635417 epubgen-0.4.0/epubgen.egg-info/
+-rw-r--r--   0 sfluor     (501) staff       (20)      995 2023-07-30 17:56:44.000000 epubgen-0.4.0/epubgen.egg-info/PKG-INFO
+-rw-r--r--   0 sfluor     (501) staff       (20)      195 2023-07-30 17:56:44.000000 epubgen-0.4.0/epubgen.egg-info/SOURCES.txt
+-rw-r--r--   0 sfluor     (501) staff       (20)        1 2023-07-30 17:56:44.000000 epubgen-0.4.0/epubgen.egg-info/dependency_links.txt
+-rw-r--r--   0 sfluor     (501) staff       (20)        8 2023-07-30 17:56:44.000000 epubgen-0.4.0/epubgen.egg-info/top_level.txt
+-rw-r--r--   0 sfluor     (501) staff       (20)      560 2023-07-30 17:23:55.000000 epubgen-0.4.0/pyproject.toml
+-rw-r--r--   0 sfluor     (501) staff       (20)       38 2023-07-30 17:56:44.636627 epubgen-0.4.0/setup.cfg
```

### Comparing `epubgen-0.3.0/LICENSE` & `epubgen-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `epubgen-0.3.0/PKG-INFO` & `epubgen-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epubgen
-Version: 0.3.0
+Version: 0.4.0
 Summary: Tiny library to programmatically generate .epub files
 Author: Sami Tabet
 Project-URL: Homepage, https://github.com/sfluor/epubgen
 Project-URL: Bug Tracker, https://github.com/sfluor/epubgen/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `epubgen-0.3.0/epubgen/epubgen.py` & `epubgen-0.4.0/epubgen/epubgen.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     - id: a public identifier for the EPUB
     - css: optional CSS to provide to tweak the presentation of the pages
     - rtl: to enable the "right to left" reading direction mode
 
     Methods
     -------
     - add_page: add content to the EPUB
+    - add_font: add a font to the EPUB
     - add_image: embed images in the EPUB
     - generate_epub: generate the EPUB file
     """
 
     def __init__(
         self, title: str, author: str, language: str, id: str, css="", rtl=False
     ):
@@ -54,18 +55,14 @@
 
         self.page_counts: int = 0
         self.contents: list[tuple[str, str | bytes]] = [
             ("mimetype", "application/epub+zip"),
             ("META-INF/container.xml", self._generate_container()),
         ]
 
-        if self.css:
-            self.contents.append((CONTENT_ROOT + CSS_FILE, self.css))
-            self._add_to_manifest("stylesheet", CSS_FILE, "text/css")
-
     def _generate_container(self) -> str:
         container = ET.Element(
             "container",
             attrib={
                 "xmlns": "urn:oasis:names:tc:opendocument:xmlns:container",
                 "version": "1.0",
             },
@@ -77,22 +74,22 @@
             attrib={
                 "full-path": PACKAGE_PATH,
                 "media-type": "application/oebps-package+xml",
             },
         )
         return xml_to_str(container)
 
-    def _add_to_manifest(self, id, path, type, **kwargs):
+    def _add_to_manifest(self, id, path, media_type, **kwargs):
         ET.SubElement(
             self.manifest,
             "item",
             attrib={
                 "id": id,
                 "href": path,
-                "media-type": type,
+                "media-type": media_type,
                 **kwargs,
             },
         )
 
     def _current_page_id_and_path(self) -> tuple[str, str]:
         page_id = f"page{self.page_counts}"
         path = f"{page_id}.xhtml"
@@ -175,18 +172,41 @@
         """
         Embeds an image to the epub that can then be referenced using the provided path.
 
         - id: the image ID as a string
         - path: the image path in the EPUB as a string (should contain a valid image extension)
         - image_content: the raw image content as bytes
         """
-        type = os.path.splitext(path)[1]
-        self._add_to_manifest(id, path, "image/" + type)
+        media_type = os.path.splitext(path)[1][1:]
+        self._add_to_manifest(id, path, f"image/{media_type}")
         self.contents.append((CONTENT_ROOT + path, image_content))
 
+    def add_font(self, family: str, style: str, weight: int, font_type: str, font_definition: bytes):
+        """
+        Embeds a font definition into the epub that can then be used in CSS.
+
+        - family: the font family, for instance "Times New Roman"
+        - style: the font style (normal, bold, italic)
+        - weight: the font weight (200, 400, 700, etc)
+        - type: font type (ttf, otf, woff, etc)
+        - font_definition: the raw font definition data (coming from the font file)
+        """
+        path = f"fonts/{family}-{style}-{weight}.{font_type}"
+        self._add_to_manifest(family, path, f"font/{font_type}")
+        self.contents.append((CONTENT_ROOT + path, font_definition))
+
+        # We also need to add the font to the stylesheet so that it's discoverable by the epub reader.
+        self.css += f"""
+@font-face {{
+    font-family : "{family}";
+    font-weight : {weight};
+    font-style: {style};
+    src : url("{path}");
+}}"""
+
     def add_page(self, content: ET.Element, toc_title=None):
         """
         Add a new page to the EPUB.
 
         - content: the HTML content of the page to add
         - [toc_title]: optional, if provided it will add a reference to this page to the table of contents.
         """
@@ -216,27 +236,20 @@
             link.text = toc_title
             self.toc.append(li)
 
     def generate_epub(self, path: str):
         """
         Generates the EPUB and saves it at the provided path.
         """
-        contents = self.contents + [
+        contents = self.contents
+        if self.css:
+            contents.append((CONTENT_ROOT + CSS_FILE, self.css))
+            self._add_to_manifest("stylesheet", CSS_FILE, "text/css")
+
+        contents = contents + [
             (CONTENT_ROOT + TOC_PATH, self._generate_toc()),
             (PACKAGE_PATH, self._generate_pkg_opf()),
         ]
 
         with ZipFile(path, "w") as zip:
             for path, content in contents:
                 zip.writestr(path, content)
-
-
-if __name__ == "__main__":
-    book = EPUB("Test", "author-test", "en")
-    first_page = ET.Element("p")
-    first_page.text = "first-page" + 10000 * "hello "
-    book.add_page(first_page, toc_title="First chapter")
-
-    second_page = ET.Element("p")
-    second_page.text = "second-page" + 10000 * "good morning ! "
-    book.add_page(second_page, toc_title="Second chapter")
-    book.generate_epub("test.epub")
```

### Comparing `epubgen-0.3.0/epubgen.egg-info/PKG-INFO` & `epubgen-0.4.0/epubgen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epubgen
-Version: 0.3.0
+Version: 0.4.0
 Summary: Tiny library to programmatically generate .epub files
 Author: Sami Tabet
 Project-URL: Homepage, https://github.com/sfluor/epubgen
 Project-URL: Bug Tracker, https://github.com/sfluor/epubgen/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `epubgen-0.3.0/pyproject.toml` & `epubgen-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "epubgen"
-version = "0.3.0"
+version = "0.4.0"
 authors = [{ name = "Sami Tabet" }]
 description = "Tiny library to programmatically generate .epub files"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

