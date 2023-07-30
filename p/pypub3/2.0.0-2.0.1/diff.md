# Comparing `tmp/pypub3-2.0.0.tar.gz` & `tmp/pypub3-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypub3-2.0.0.tar", last modified: Fri Apr 14 23:32:56 2023, max compression
+gzip compressed data, was "pypub3-2.0.1.tar", last modified: Sun Jul 30 20:27:12 2023, max compression
```

## Comparing `pypub3-2.0.0.tar` & `pypub3-2.0.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-14 23:32:56.120629 pypub3-2.0.0/
--rw-r--r--   0 andrew    (1000) andrew    (1000)     1075 2020-06-20 20:57:00.000000 pypub3-2.0.0/LICENSE
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     2043 2023-04-14 23:32:56.120629 pypub3-2.0.0/PKG-INFO
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1587 2023-04-14 23:31:44.000000 pypub3-2.0.0/README.md
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-14 23:32:56.116629 pypub3-2.0.0/pypub/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      558 2023-04-14 23:31:44.000000 pypub3-2.0.0/pypub/__init__.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)    10259 2023-04-14 23:31:44.000000 pypub3-2.0.0/pypub/builder.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     6452 2023-04-14 23:31:44.000000 pypub3-2.0.0/pypub/chapter.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     2133 2023-04-14 23:31:44.000000 pypub3-2.0.0/pypub/epub.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     9221 2023-04-14 23:31:44.000000 pypub3-2.0.0/pypub/factory.py
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-14 23:32:56.116629 pypub3-2.0.0/pypub/static/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      232 2023-03-28 06:24:00.000000 pypub3-2.0.0/pypub/static/container.xml
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      627 2023-03-28 06:24:00.000000 pypub3-2.0.0/pypub/static/coverpage.xhtml
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-14 23:32:56.116629 pypub3-2.0.0/pypub/static/css/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       85 2023-03-28 06:24:00.000000 pypub3-2.0.0/pypub/static/css/coverpage.css
--rw-rw-r--   0 andrew    (1000) andrew    (1000)        1 2023-03-28 06:24:00.000000 pypub3-2.0.0/pypub/static/css/styles.css
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-14 23:32:56.116629 pypub3-2.0.0/pypub/static/fonts/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)   592752 2023-03-28 06:24:00.000000 pypub3-2.0.0/pypub/static/fonts/free_mono.ttf
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-14 23:32:56.116629 pypub3-2.0.0/pypub/static/img/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)    88953 2023-03-28 06:24:00.000000 pypub3-2.0.0/pypub/static/img/cover.png
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       20 2023-03-28 06:24:00.000000 pypub3-2.0.0/pypub/static/mimetype
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-14 23:32:56.116629 pypub3-2.0.0/pypub/templates/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      705 2023-04-14 23:31:44.000000 pypub3-2.0.0/pypub/templates/book.ncx.j2
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1978 2023-04-14 23:31:44.000000 pypub3-2.0.0/pypub/templates/book.opf.j2
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      635 2023-04-14 23:31:44.000000 pypub3-2.0.0/pypub/templates/page.xhtml.j2
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      606 2023-04-14 23:31:44.000000 pypub3-2.0.0/pypub/templates/toc.xhtml.j2
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-14 23:32:56.116629 pypub3-2.0.0/pypub/tests/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      196 2023-04-14 23:31:44.000000 pypub3-2.0.0/pypub/tests/__init__.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      113 2023-04-14 23:31:44.000000 pypub3-2.0.0/pypub/tests/__main__.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1272 2023-04-14 23:31:44.000000 pypub3-2.0.0/pypub/tests/chapter.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1305 2023-04-14 23:31:44.000000 pypub3-2.0.0/pypub/tests/epub.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     3265 2023-04-14 23:31:44.000000 pypub3-2.0.0/pypub/tests/factory.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1140 2023-04-14 23:31:44.000000 pypub3-2.0.0/pypub/tests/profile.py
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-14 23:32:56.120629 pypub3-2.0.0/pypub3.egg-info/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     2043 2023-04-14 23:32:56.000000 pypub3-2.0.0/pypub3.egg-info/PKG-INFO
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      707 2023-04-14 23:32:56.000000 pypub3-2.0.0/pypub3.egg-info/SOURCES.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)        1 2023-04-14 23:32:56.000000 pypub3-2.0.0/pypub3.egg-info/dependency_links.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       33 2023-04-14 23:32:56.000000 pypub3-2.0.0/pypub3.egg-info/requires.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)        6 2023-04-14 23:32:56.000000 pypub3-2.0.0/pypub3.egg-info/top_level.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       38 2023-04-14 23:32:56.120629 pypub3-2.0.0/setup.cfg
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      961 2023-04-14 23:32:03.000000 pypub3-2.0.0/setup.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-07-30 20:27:12.861072 pypub3-2.0.1/
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     1075 2020-06-20 20:57:00.000000 pypub3-2.0.1/LICENSE
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     2420 2023-07-30 20:27:12.861072 pypub3-2.0.1/PKG-INFO
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1587 2023-04-14 23:31:44.000000 pypub3-2.0.1/README.md
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-07-30 20:27:12.857072 pypub3-2.0.1/pypub/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      558 2023-04-14 23:31:44.000000 pypub3-2.0.1/pypub/__init__.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)    10531 2023-07-30 20:09:14.000000 pypub3-2.0.1/pypub/builder.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     6452 2023-06-29 02:32:03.000000 pypub3-2.0.1/pypub/chapter.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     2133 2023-07-30 19:48:46.000000 pypub3-2.0.1/pypub/epub.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     9337 2023-07-30 20:27:03.000000 pypub3-2.0.1/pypub/factory.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-07-30 20:27:12.857072 pypub3-2.0.1/pypub/static/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      232 2023-03-28 06:24:00.000000 pypub3-2.0.1/pypub/static/container.xml
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-07-30 20:27:12.857072 pypub3-2.0.1/pypub/static/css/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       85 2023-03-28 06:24:00.000000 pypub3-2.0.1/pypub/static/css/coverpage.css
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)        1 2023-03-28 06:24:00.000000 pypub3-2.0.1/pypub/static/css/styles.css
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-07-30 20:27:12.857072 pypub3-2.0.1/pypub/static/fonts/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)   592752 2023-03-28 06:24:00.000000 pypub3-2.0.1/pypub/static/fonts/free_mono.ttf
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-07-30 20:27:12.857072 pypub3-2.0.1/pypub/static/img/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)    88953 2023-03-28 06:24:00.000000 pypub3-2.0.1/pypub/static/img/cover.png
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       20 2023-03-28 06:24:00.000000 pypub3-2.0.1/pypub/static/mimetype
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-07-30 20:27:12.857072 pypub3-2.0.1/pypub/templates/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      705 2023-04-14 23:31:44.000000 pypub3-2.0.1/pypub/templates/book.ncx.j2
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1978 2023-04-14 23:31:44.000000 pypub3-2.0.1/pypub/templates/book.opf.j2
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      622 2023-07-30 18:14:49.000000 pypub3-2.0.1/pypub/templates/coverpage.xhtml.j2
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      635 2023-04-14 23:31:44.000000 pypub3-2.0.1/pypub/templates/page.xhtml.j2
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      606 2023-04-14 23:31:44.000000 pypub3-2.0.1/pypub/templates/toc.xhtml.j2
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-07-30 20:27:12.861072 pypub3-2.0.1/pypub/tests/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      412 2023-07-30 19:45:33.000000 pypub3-2.0.1/pypub/tests/__init__.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      113 2023-04-14 23:31:44.000000 pypub3-2.0.1/pypub/tests/__main__.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1629 2023-07-30 18:44:57.000000 pypub3-2.0.1/pypub/tests/chapter.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1868 2023-07-30 19:48:57.000000 pypub3-2.0.1/pypub/tests/epub.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     5104 2023-07-30 19:47:37.000000 pypub3-2.0.1/pypub/tests/factory.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1139 2023-07-30 19:02:06.000000 pypub3-2.0.1/pypub/tests/profile.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-07-30 20:27:12.861072 pypub3-2.0.1/pypub3.egg-info/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     2420 2023-07-30 20:27:12.000000 pypub3-2.0.1/pypub3.egg-info/PKG-INFO
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      713 2023-07-30 20:27:12.000000 pypub3-2.0.1/pypub3.egg-info/SOURCES.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)        1 2023-07-30 20:27:12.000000 pypub3-2.0.1/pypub3.egg-info/dependency_links.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       60 2023-07-30 20:27:12.000000 pypub3-2.0.1/pypub3.egg-info/requires.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)        6 2023-07-30 20:27:12.000000 pypub3-2.0.1/pypub3.egg-info/top_level.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       38 2023-07-30 20:27:12.861072 pypub3-2.0.1/setup.cfg
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      984 2023-07-30 19:53:35.000000 pypub3-2.0.1/setup.py
```

### Comparing `pypub3-2.0.0/LICENSE` & `pypub3-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pypub3-2.0.0/PKG-INFO` & `pypub3-2.0.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,61 +1,61 @@
 Metadata-Version: 2.1
 Name: pypub3
-Version: 2.0.0
+Version: 2.0.1
 Summary: A python3 library to generate custom epub books.
 Home-page: https://github.com/imgurbot12/pypub
 Author: Andrew Scott
 Author-email: imgurbot12@gmail.com
 License: MIT
+Description: pypub
+        ------
+        
+        Create epub's using Python. 
+        Pypub is a Python library to create epub files quickly, 
+        without having to worry about the intricacies of the epub specification.
+        
+        This package was originally forked and re-written based on WCember's Python 2 
+        version, but due to a lack of response has been re-released as a new package 
+        to support Python 3.
+        
+        The codebase has since gone through a few substantial rewrites and operates 
+        as its own library moving forward.
+        
+        ### Installation
+        
+        ```
+        pip install pypub3
+        ```
+        
+        ### Quickstart
+        
+        ```python
+        import pypub
+        
+        my_first_epub = pypub.Epub('My First Epub')
+        my_first_chapter = pypub.create_chapter_from_url('https://en.wikipedia.org/wiki/EPUB')
+        my_first_epub.add_chapter(my_first_chapter)
+        my_first_epub.create('./my-first-epub.epub')
+        ```
+        
+        # Features #
+        * Pypub is **easy to install** and has minimal dependencies.
+        * Pypub **abstracts the epub specification**. 
+          Create epubs without worrying about what an NCX is.
+        * Pypub can **create epubs from websites, html files, strings**, 
+          or a combination of all three.
+        * Pypub can **clean up poorly formatted and complicated html**, 
+          so it will show cleanly as a chapter in your book.
+        * Pypub **creates epubs specifically so they can be converted into 
+          Amazon Kindle mobi or azw3 files**. Don't know which tags Amazon 
+          supports? Don't worry about it because pypub does. 
+        * Pypub is **customizable**. Don't like the way pypub sanitizes html 
+          files for you ebook? Pypub can be configured with your own sanitation 
+          function.
+        * Pypub is **licensed under the MIT license**. Do what you want with it.
+        
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-pypub
-------
-
-Create epub's using Python. 
-Pypub is a Python library to create epub files quickly, 
-without having to worry about the intricacies of the epub specification.
-
-This package was originally forked and re-written based on WCember's Python 2 
-version, but due to a lack of response has been re-released as a new package 
-to support Python 3.
-
-The codebase has since gone through a few substantial rewrites and operates 
-as its own library moving forward.
-
-### Installation
-
-```
-pip install pypub3
-```
-
-### Quickstart
-
-```python
-import pypub
-
-my_first_epub = pypub.Epub('My First Epub')
-my_first_chapter = pypub.create_chapter_from_url('https://en.wikipedia.org/wiki/EPUB')
-my_first_epub.add_chapter(my_first_chapter)
-my_first_epub.create('./my-first-epub.epub')
-```
-
-# Features #
-* Pypub is **easy to install** and has minimal dependencies.
-* Pypub **abstracts the epub specification**. 
-  Create epubs without worrying about what an NCX is.
-* Pypub can **create epubs from websites, html files, strings**, 
-  or a combination of all three.
-* Pypub can **clean up poorly formatted and complicated html**, 
-  so it will show cleanly as a chapter in your book.
-* Pypub **creates epubs specifically so they can be converted into 
-  Amazon Kindle mobi or azw3 files**. Don't know which tags Amazon 
-  supports? Don't worry about it because pypub does. 
-* Pypub is **customizable**. Don't like the way pypub sanitizes html 
-  files for you ebook? Pypub can be configured with your own sanitation 
-  function.
-* Pypub is **licensed under the MIT license**. Do what you want with it.
```

### Comparing `pypub3-2.0.0/README.md` & `pypub3-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pypub3-2.0.0/pypub/__init__.py` & `pypub3-2.0.1/pypub/__init__.py`

 * *Files identical despite different names*

### Comparing `pypub3-2.0.0/pypub/builder.py` & `pypub3-2.0.1/pypub/builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,36 +180,42 @@
 
     def __exit__(self, *_):
         """cleanup on exit of context-manager"""
         self.cleanup()
 
     def begin(self) -> EpubDirs:
         """begin building operations w/ basic file structure"""
+        # read jinja2 chapter template
+        if not self.template:
+            self.template = jinja_env.get_template('page.xhtml.j2')
         if self.dirs:
             return self.dirs
         args = (self.epub.title, self.epub.creator)
         self.logger.info('generating: %r (by: %s)' % args)
         # generate base directories and copy static files
         self.dirs = epub_dirs(self.epub.epub_dir)
         copy_static('mimetype', self.dirs.basedir)
         copy_static('container.xml', self.dirs.metainf)
-        copy_static('coverpage.xhtml', self.dirs.oebps)
         copy_static('css/coverpage.css', self.dirs.styles)
         copy_static('css/styles.css', self.dirs.styles)
         for path in self.epub.css_paths:
             copy_file(path, self.dirs.styles)
         # generate cover-image
         if self.epub.cover is not None:
             self.cover = os.path.basename(self.epub.cover)
             copy_file(self.epub.cover, self.dirs.images)
-            return self.dirs 
-        self.logger.info('generating cover-image (%r by %r)' % args)
-        self.cover = generate_cover(*args, self.dirs.images)
-        # read jinja2 chapter template
-        self.template = jinja_env.get_template('page.xhtml.j2')
+        else:
+            self.logger.info('generating cover-image (%r by %r)' % args)
+            self.cover = generate_cover(*args, self.dirs.images)
+        # render cover-image
+        fpath    = os.path.join(self.dirs.oebps, 'coverpage.xhtml')
+        template = jinja_env.get_template('coverpage.xhtml.j2')
+        with open(fpath, 'w') as f:
+            cover = template.render(cover=os.path.join('images', self.cover))
+            f.write(cover)
         return self.dirs
 
     def render_chapter(self, assign: Assignment, chapter: Chapter):
         """render an assigned chapter into the ebook"""
         if not self.dirs or not self.template:
             raise RuntimeError('cannot render_chapter before `begin`')
         # log chapter generation
```

### Comparing `pypub3-2.0.0/pypub/chapter.py` & `pypub3-2.0.1/pypub/chapter.py`

 * *Files identical despite different names*

### Comparing `pypub3-2.0.0/pypub/epub.py` & `pypub3-2.0.1/pypub/epub.py`

 * *Files identical despite different names*

### Comparing `pypub3-2.0.0/pypub/factory.py` & `pypub3-2.0.1/pypub/factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import uuid
 import urllib.error
 import urllib.parse
 import urllib.request
 from logging import Logger
 from abc import abstractmethod
 from dataclasses import dataclass, field
-from typing import Protocol
+from typing import Protocol, cast
 
 import imghdr
 import pyxml.html
 from pyxml.html import HtmlElement
 from jinja2 import Template
 
 from .chapter import Chapter, urlrequest, htmltostring
@@ -98,16 +98,17 @@
             image.attrib['src'] = downloads[url]
             continue
         # download url into local image folder for epub
         ctx.logger.debug(f'chapter[%s] downloading image: %r' % fmt)
         try:
             res = urlrequest(url, timeout=ctx.timeout)
             # ensure status of response is valid
-            if res.status and res.status != 200:
-                raise urllib.error.URLError(f'status: {res.status}')
+            status = getattr(res, 'status', None)
+            if status and status != 200:
+                raise urllib.error.URLError(f'status: {status}')
             # read first chunk to determine content-type
             chunk = res.read(chunk_size)
             mime  = imghdr.what(None, h=chunk)
             if not mime:
                 ctx.logger.warning('chapter[%s] cannot identify %r mime' % fmt)
                 continue
             fname = f'{uuid.uuid4()}.{mime}'
@@ -225,27 +226,28 @@
             if elem.tag in SUPPORTED_TAGS:
                 # remove attributes not approved for specific tag
                 for attr in list(elem.attrib.keys()):
                     if attr not in SUPPORTED_TAGS[elem.tag]:
                         elem.attrib.pop(attr)
             # if element is not supported, append children to parent
             else:
-                parent = elem.getparent()
+                # retrieve parent
+                parent = cast(HtmlElement, elem.getparent())
                 for child in elem.getchildren():
                     parent.append(child)
                 parent.remove(elem)
                 #NOTE: this is a bug with lxml, some children have
                 # text in the parent included in the tail rather
                 # than text attribute, so we also append tail to text
                 if elem.tail and elem.tail.strip():
                     parent.text = (parent.text or '') + elem.tail.strip()
         # ensure all images with no src are removed
         for img in etree.xpath('.//img'):
             if 'src' not in img.attrib:
-                img.getparent().remove(img)
+                cast(HtmlElement, img.getparent()).remove(img)
         # return new element-tree
         return etree
 
     def hydrate(self, ctx: RenderCtx):
         """
         modify chapter element-tree to render images
         """
```

### Comparing `pypub3-2.0.0/pypub/static/coverpage.xhtml` & `pypub3-2.0.1/pypub/templates/coverpage.xhtml.j2`

 * *Files 20% similar despite different names*

#### Comparing `pypub3-2.0.0/pypub/static/coverpage.xhtml` & `pypub3-2.0.1/pypub/templates/coverpage.xhtml.j2`

```diff
@@ -7,11 +7,11 @@
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8"/>
     <link type="text/css" rel="stylesheet" href="styles/styles.css"/>
     <link type="text/css" rel="stylesheet" href="styles/coverpage.css"/>
     <title>Cover Image</title>
   </head>
   <body>
     <div>
-      <img src="images/cover.png" alt="Cover image" style="width: 100%;height: 100%"/>
+      <img src="{{ cover }}" alt="Cover image" style="width: 100%;height: 100%"/>
     </div>
   </body>
 </html>
```

### Comparing `pypub3-2.0.0/pypub/static/fonts/free_mono.ttf` & `pypub3-2.0.1/pypub/static/fonts/free_mono.ttf`

 * *Files identical despite different names*

### Comparing `pypub3-2.0.0/pypub/static/img/cover.png` & `pypub3-2.0.1/pypub/static/img/cover.png`

 * *Files identical despite different names*

### Comparing `pypub3-2.0.0/pypub/templates/book.ncx.j2` & `pypub3-2.0.1/pypub/templates/book.ncx.j2`

 * *Files identical despite different names*

### Comparing `pypub3-2.0.0/pypub/templates/book.opf.j2` & `pypub3-2.0.1/pypub/templates/book.opf.j2`

 * *Files identical despite different names*

### Comparing `pypub3-2.0.0/pypub/templates/page.xhtml.j2` & `pypub3-2.0.1/pypub/templates/page.xhtml.j2`

 * *Files identical despite different names*

### Comparing `pypub3-2.0.0/pypub/templates/toc.xhtml.j2` & `pypub3-2.0.1/pypub/templates/toc.xhtml.j2`

 * *Files identical despite different names*

### Comparing `pypub3-2.0.0/pypub/tests/profile.py` & `pypub3-2.0.1/pypub/tests/profile.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
             os.remove('./profile-test.epub')
         except Exception:
             pass
 
 #** Tests **#
 
 class Profiling(unittest.TestCase):
-    """profile based unit-tests"""
+    """Profile Based UnitTests"""
 
     def test_epub_profile(self):
         """complete profile on generating the given epub"""
         # enable profile
         pr = cProfile.Profile()
         pr.enable()
         # generate stats
```

### Comparing `pypub3-2.0.0/pypub3.egg-info/PKG-INFO` & `pypub3-2.0.1/pypub3.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,61 +1,61 @@
 Metadata-Version: 2.1
 Name: pypub3
-Version: 2.0.0
+Version: 2.0.1
 Summary: A python3 library to generate custom epub books.
 Home-page: https://github.com/imgurbot12/pypub
 Author: Andrew Scott
 Author-email: imgurbot12@gmail.com
 License: MIT
+Description: pypub
+        ------
+        
+        Create epub's using Python. 
+        Pypub is a Python library to create epub files quickly, 
+        without having to worry about the intricacies of the epub specification.
+        
+        This package was originally forked and re-written based on WCember's Python 2 
+        version, but due to a lack of response has been re-released as a new package 
+        to support Python 3.
+        
+        The codebase has since gone through a few substantial rewrites and operates 
+        as its own library moving forward.
+        
+        ### Installation
+        
+        ```
+        pip install pypub3
+        ```
+        
+        ### Quickstart
+        
+        ```python
+        import pypub
+        
+        my_first_epub = pypub.Epub('My First Epub')
+        my_first_chapter = pypub.create_chapter_from_url('https://en.wikipedia.org/wiki/EPUB')
+        my_first_epub.add_chapter(my_first_chapter)
+        my_first_epub.create('./my-first-epub.epub')
+        ```
+        
+        # Features #
+        * Pypub is **easy to install** and has minimal dependencies.
+        * Pypub **abstracts the epub specification**. 
+          Create epubs without worrying about what an NCX is.
+        * Pypub can **create epubs from websites, html files, strings**, 
+          or a combination of all three.
+        * Pypub can **clean up poorly formatted and complicated html**, 
+          so it will show cleanly as a chapter in your book.
+        * Pypub **creates epubs specifically so they can be converted into 
+          Amazon Kindle mobi or azw3 files**. Don't know which tags Amazon 
+          supports? Don't worry about it because pypub does. 
+        * Pypub is **customizable**. Don't like the way pypub sanitizes html 
+          files for you ebook? Pypub can be configured with your own sanitation 
+          function.
+        * Pypub is **licensed under the MIT license**. Do what you want with it.
+        
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-pypub
-------
-
-Create epub's using Python. 
-Pypub is a Python library to create epub files quickly, 
-without having to worry about the intricacies of the epub specification.
-
-This package was originally forked and re-written based on WCember's Python 2 
-version, but due to a lack of response has been re-released as a new package 
-to support Python 3.
-
-The codebase has since gone through a few substantial rewrites and operates 
-as its own library moving forward.
-
-### Installation
-
-```
-pip install pypub3
-```
-
-### Quickstart
-
-```python
-import pypub
-
-my_first_epub = pypub.Epub('My First Epub')
-my_first_chapter = pypub.create_chapter_from_url('https://en.wikipedia.org/wiki/EPUB')
-my_first_epub.add_chapter(my_first_chapter)
-my_first_epub.create('./my-first-epub.epub')
-```
-
-# Features #
-* Pypub is **easy to install** and has minimal dependencies.
-* Pypub **abstracts the epub specification**. 
-  Create epubs without worrying about what an NCX is.
-* Pypub can **create epubs from websites, html files, strings**, 
-  or a combination of all three.
-* Pypub can **clean up poorly formatted and complicated html**, 
-  so it will show cleanly as a chapter in your book.
-* Pypub **creates epubs specifically so they can be converted into 
-  Amazon Kindle mobi or azw3 files**. Don't know which tags Amazon 
-  supports? Don't worry about it because pypub does. 
-* Pypub is **customizable**. Don't like the way pypub sanitizes html 
-  files for you ebook? Pypub can be configured with your own sanitation 
-  function.
-* Pypub is **licensed under the MIT license**. Do what you want with it.
```

### Comparing `pypub3-2.0.0/pypub3.egg-info/SOURCES.txt` & `pypub3-2.0.1/pypub3.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 setup.py
 pypub/__init__.py
 pypub/builder.py
 pypub/chapter.py
 pypub/epub.py
 pypub/factory.py
 pypub/static/container.xml
-pypub/static/coverpage.xhtml
 pypub/static/mimetype
 pypub/static/css/coverpage.css
 pypub/static/css/styles.css
 pypub/static/fonts/free_mono.ttf
 pypub/static/img/cover.png
 pypub/templates/book.ncx.j2
 pypub/templates/book.opf.j2
+pypub/templates/coverpage.xhtml.j2
 pypub/templates/page.xhtml.j2
 pypub/templates/toc.xhtml.j2
 pypub/tests/__init__.py
 pypub/tests/__main__.py
 pypub/tests/chapter.py
 pypub/tests/epub.py
 pypub/tests/factory.py
```

### Comparing `pypub3-2.0.0/setup.py` & `pypub3-2.0.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     readme = f.read()
 
 setup(
     name='pypub3',
-    version='2.0.0',
+    version='2.0.1',
     license='MIT',
     author='Andrew Scott',
     author_email='imgurbot12@gmail.com',
     url='https://github.com/imgurbot12/pypub',
     description="A python3 library to generate custom epub books.",
     long_description=readme,
     long_description_content_type="text/markdown",
     python_requires='>=3.6',
     packages=find_packages(),
     install_requires=[
-        'jinja2',
-        'pyxml3',
-        'pillow',
-        'dataclasses',
+        'pyxml3>=0.0.2',
+        'jinja2>=3.1.2',
+        'dataclasses>=0.6',
+        'pillow>=10.0.0',
     ],
     package_data={
         'pypub': [
-            'templates/*', 
-            'static/*', 
-            'static/css/*', 
-            'static/img/*', 
+            'templates/*',
+            'static/*',
+            'static/css/*',
+            'static/img/*',
             'static/fonts/*'
         ]
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

