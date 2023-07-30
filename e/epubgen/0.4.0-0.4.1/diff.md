# Comparing `tmp/epubgen-0.4.0.tar.gz` & `tmp/epubgen-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epubgen-0.4.0.tar", last modified: Sun Jul 30 17:56:44 2023, max compression
+gzip compressed data, was "epubgen-0.4.1.tar", last modified: Sun Jul 30 18:07:45 2023, max compression
```

## Comparing `epubgen-0.4.0.tar` & `epubgen-0.4.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 sfluor     (501) staff       (20)        0 2023-07-30 17:56:44.636527 epubgen-0.4.0/
--rw-r--r--   0 sfluor     (501) staff       (20)     1067 2023-07-28 21:42:19.000000 epubgen-0.4.0/LICENSE
--rw-r--r--   0 sfluor     (501) staff       (20)      995 2023-07-30 17:56:44.636102 epubgen-0.4.0/PKG-INFO
--rw-r--r--   0 sfluor     (501) staff       (20)      506 2023-07-30 15:36:10.000000 epubgen-0.4.0/README.md
-drwxr-xr-x   0 sfluor     (501) staff       (20)        0 2023-07-30 17:56:44.633363 epubgen-0.4.0/epubgen/
--rw-r--r--   0 sfluor     (501) staff       (20)       26 2023-07-30 15:23:29.000000 epubgen-0.4.0/epubgen/__init__.py
--rw-r--r--   0 sfluor     (501) staff       (20)     8502 2023-07-30 17:55:17.000000 epubgen-0.4.0/epubgen/epubgen.py
-drwxr-xr-x   0 sfluor     (501) staff       (20)        0 2023-07-30 17:56:44.635417 epubgen-0.4.0/epubgen.egg-info/
--rw-r--r--   0 sfluor     (501) staff       (20)      995 2023-07-30 17:56:44.000000 epubgen-0.4.0/epubgen.egg-info/PKG-INFO
--rw-r--r--   0 sfluor     (501) staff       (20)      195 2023-07-30 17:56:44.000000 epubgen-0.4.0/epubgen.egg-info/SOURCES.txt
--rw-r--r--   0 sfluor     (501) staff       (20)        1 2023-07-30 17:56:44.000000 epubgen-0.4.0/epubgen.egg-info/dependency_links.txt
--rw-r--r--   0 sfluor     (501) staff       (20)        8 2023-07-30 17:56:44.000000 epubgen-0.4.0/epubgen.egg-info/top_level.txt
--rw-r--r--   0 sfluor     (501) staff       (20)      560 2023-07-30 17:23:55.000000 epubgen-0.4.0/pyproject.toml
--rw-r--r--   0 sfluor     (501) staff       (20)       38 2023-07-30 17:56:44.636627 epubgen-0.4.0/setup.cfg
+drwxr-xr-x   0 sfluor     (501) staff       (20)        0 2023-07-30 18:07:45.420667 epubgen-0.4.1/
+-rw-r--r--   0 sfluor     (501) staff       (20)     1067 2023-07-28 21:42:19.000000 epubgen-0.4.1/LICENSE
+-rw-r--r--   0 sfluor     (501) staff       (20)      995 2023-07-30 18:07:45.420274 epubgen-0.4.1/PKG-INFO
+-rw-r--r--   0 sfluor     (501) staff       (20)      506 2023-07-30 15:36:10.000000 epubgen-0.4.1/README.md
+drwxr-xr-x   0 sfluor     (501) staff       (20)        0 2023-07-30 18:07:45.416602 epubgen-0.4.1/epubgen/
+-rw-r--r--   0 sfluor     (501) staff       (20)       26 2023-07-30 15:23:29.000000 epubgen-0.4.1/epubgen/__init__.py
+-rw-r--r--   0 sfluor     (501) staff       (20)     9067 2023-07-30 18:05:46.000000 epubgen-0.4.1/epubgen/epubgen.py
+drwxr-xr-x   0 sfluor     (501) staff       (20)        0 2023-07-30 18:07:45.419616 epubgen-0.4.1/epubgen.egg-info/
+-rw-r--r--   0 sfluor     (501) staff       (20)      995 2023-07-30 18:07:45.000000 epubgen-0.4.1/epubgen.egg-info/PKG-INFO
+-rw-r--r--   0 sfluor     (501) staff       (20)      195 2023-07-30 18:07:45.000000 epubgen-0.4.1/epubgen.egg-info/SOURCES.txt
+-rw-r--r--   0 sfluor     (501) staff       (20)        1 2023-07-30 18:07:45.000000 epubgen-0.4.1/epubgen.egg-info/dependency_links.txt
+-rw-r--r--   0 sfluor     (501) staff       (20)        8 2023-07-30 18:07:45.000000 epubgen-0.4.1/epubgen.egg-info/top_level.txt
+-rw-r--r--   0 sfluor     (501) staff       (20)      560 2023-07-30 18:07:19.000000 epubgen-0.4.1/pyproject.toml
+-rw-r--r--   0 sfluor     (501) staff       (20)       38 2023-07-30 18:07:45.420778 epubgen-0.4.1/setup.cfg
```

### Comparing `epubgen-0.4.0/LICENSE` & `epubgen-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `epubgen-0.4.0/PKG-INFO` & `epubgen-0.4.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epubgen
-Version: 0.4.0
+Version: 0.4.1
 Summary: Tiny library to programmatically generate .epub files
 Author: Sami Tabet
 Project-URL: Homepage, https://github.com/sfluor/epubgen
 Project-URL: Bug Tracker, https://github.com/sfluor/epubgen/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `epubgen-0.4.0/epubgen/epubgen.py` & `epubgen-0.4.1/epubgen/epubgen.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     - rtl: to enable the "right to left" reading direction mode
 
     Methods
     -------
     - add_page: add content to the EPUB
     - add_font: add a font to the EPUB
     - add_image: embed images in the EPUB
+    - add_cover: add a cover image for the EPUB
     - generate_epub: generate the EPUB file
     """
 
     def __init__(
         self, title: str, author: str, language: str, id: str, css="", rtl=False
     ):
         self.id: str = id
@@ -164,14 +165,28 @@
         date_t.text = now
 
         meta_t = ET.SubElement(metadata, "meta", property="dcterms:modified")
         meta_t.text = now
 
         return metadata
 
+    def add_cover(self, image_type:str, cover_content: bytes):
+        """
+        Add a cover image for the EPUB
+
+        - image_type: the encoding of the image (jpg, png, ...)
+        - cover_content: the raw image content as bytes
+        """
+
+        COVER = "cover"
+        path = f"{COVER}.{image_type}"
+        ET.SubElement(self.metadata, "meta", name=COVER, content=COVER)
+        self._add_to_manifest(COVER, path, f"image/{image_type}")
+        self.contents.append((CONTENT_ROOT + path, cover_content))
+
     def add_image(self, id: str, path: str, image_content: bytes):
         """
         Embeds an image to the epub that can then be referenced using the provided path.
 
         - id: the image ID as a string
         - path: the image path in the EPUB as a string (should contain a valid image extension)
         - image_content: the raw image content as bytes
```

### Comparing `epubgen-0.4.0/epubgen.egg-info/PKG-INFO` & `epubgen-0.4.1/epubgen.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epubgen
-Version: 0.4.0
+Version: 0.4.1
 Summary: Tiny library to programmatically generate .epub files
 Author: Sami Tabet
 Project-URL: Homepage, https://github.com/sfluor/epubgen
 Project-URL: Bug Tracker, https://github.com/sfluor/epubgen/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `epubgen-0.4.0/pyproject.toml` & `epubgen-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "epubgen"
-version = "0.4.0"
+version = "0.4.1"
 authors = [{ name = "Sami Tabet" }]
 description = "Tiny library to programmatically generate .epub files"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

