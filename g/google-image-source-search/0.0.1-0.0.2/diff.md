# Comparing `tmp/google-image-source-search-0.0.1.tar.gz` & `tmp/google-image-source-search-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-image-source-search-0.0.1.tar", last modified: Sun Jul 30 19:32:52 2023, max compression
+gzip compressed data, was "google-image-source-search-0.0.2.tar", last modified: Sun Jul 30 20:34:44 2023, max compression
```

## Comparing `google-image-source-search-0.0.1.tar` & `google-image-source-search-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 19:32:52.723258 google-image-source-search-0.0.1/
--rw-rw-rw-   0        0        0     1082 2023-07-30 19:08:21.000000 google-image-source-search-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      696 2023-07-30 19:32:52.722357 google-image-source-search-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      111 2023-07-30 19:30:22.000000 google-image-source-search-0.0.1/README.md
--rw-rw-rw-   0        0        0      751 2023-07-30 19:31:33.000000 google-image-source-search-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-30 19:32:52.723258 google-image-source-search-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-30 19:32:52.703983 google-image-source-search-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-30 19:32:52.713679 google-image-source-search-0.0.1/src/google_image_source_search.egg-info/
--rw-rw-rw-   0        0        0      696 2023-07-30 19:32:52.000000 google-image-source-search-0.0.1/src/google_image_source_search.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      711 2023-07-30 19:32:52.000000 google-image-source-search-0.0.1/src/google_image_source_search.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 19:32:52.000000 google-image-source-search-0.0.1/src/google_image_source_search.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-07-30 19:32:52.000000 google-image-source-search-0.0.1/src/google_image_source_search.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-07-30 19:32:52.000000 google-image-source-search-0.0.1/src/google_image_source_search.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 19:32:52.718670 google-image-source-search-0.0.1/src/google_img_source_search/
--rw-rw-rw-   0        0        0       58 2023-07-30 10:00:13.000000 google-image-source-search-0.0.1/src/google_img_source_search/__init__.py
--rw-rw-rw-   0        0        0     1493 2023-07-30 10:22:35.000000 google-image-source-search-0.0.1/src/google_img_source_search/api_response_parser.py
--rw-rw-rw-   0        0        0     9298 2023-07-30 10:04:58.000000 google-image-source-search-0.0.1/src/google_img_source_search/batchexecute_decoder.py
--rw-rw-rw-   0        0        0     2080 2023-07-26 21:58:28.000000 google-image-source-search-0.0.1/src/google_img_source_search/f_req_template.py
-drwxrwxrwx   0        0        0        0 2023-07-30 19:32:52.721678 google-image-source-search-0.0.1/src/google_img_source_search/google_items/
--rw-rw-rw-   0        0        0        0 2023-07-30 09:47:32.000000 google-image-source-search-0.0.1/src/google_img_source_search/google_items/__init__.py
--rw-rw-rw-   0        0        0      115 2023-07-30 10:22:35.000000 google-image-source-search-0.0.1/src/google_img_source_search/google_items/image.py
--rw-rw-rw-   0        0        0      202 2023-07-30 09:07:43.000000 google-image-source-search-0.0.1/src/google_img_source_search/google_items/search_item.py
--rw-rw-rw-   0        0        0     1733 2023-07-30 10:22:35.000000 google-image-source-search-0.0.1/src/google_img_source_search/reverse_image_searcher.py
+drwxrwxrwx   0        0        0        0 2023-07-30 20:34:44.869763 google-image-source-search-0.0.2/
+-rw-rw-rw-   0        0        0     1082 2023-07-30 19:08:21.000000 google-image-source-search-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2192 2023-07-30 20:34:44.869763 google-image-source-search-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1607 2023-07-30 20:33:19.000000 google-image-source-search-0.0.2/README.md
+-rw-rw-rw-   0        0        0      751 2023-07-30 20:34:16.000000 google-image-source-search-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-30 20:34:44.869763 google-image-source-search-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-30 20:34:44.848017 google-image-source-search-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-30 20:34:44.859795 google-image-source-search-0.0.2/src/google_image_source_search.egg-info/
+-rw-rw-rw-   0        0        0     2192 2023-07-30 20:34:44.000000 google-image-source-search-0.0.2/src/google_image_source_search.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      711 2023-07-30 20:34:44.000000 google-image-source-search-0.0.2/src/google_image_source_search.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 20:34:44.000000 google-image-source-search-0.0.2/src/google_image_source_search.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-07-30 20:34:44.000000 google-image-source-search-0.0.2/src/google_image_source_search.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-07-30 20:34:44.000000 google-image-source-search-0.0.2/src/google_image_source_search.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 20:34:44.865777 google-image-source-search-0.0.2/src/google_img_source_search/
+-rw-rw-rw-   0        0        0       58 2023-07-30 10:00:13.000000 google-image-source-search-0.0.2/src/google_img_source_search/__init__.py
+-rw-rw-rw-   0        0        0     1493 2023-07-30 10:22:35.000000 google-image-source-search-0.0.2/src/google_img_source_search/api_response_parser.py
+-rw-rw-rw-   0        0        0     9298 2023-07-30 10:04:58.000000 google-image-source-search-0.0.2/src/google_img_source_search/batchexecute_decoder.py
+-rw-rw-rw-   0        0        0     2083 2023-07-30 20:09:27.000000 google-image-source-search-0.0.2/src/google_img_source_search/f_req_template.py
+drwxrwxrwx   0        0        0        0 2023-07-30 20:34:44.868767 google-image-source-search-0.0.2/src/google_img_source_search/google_items/
+-rw-rw-rw-   0        0        0        0 2023-07-30 09:47:32.000000 google-image-source-search-0.0.2/src/google_img_source_search/google_items/__init__.py
+-rw-rw-rw-   0        0        0      115 2023-07-30 10:22:35.000000 google-image-source-search-0.0.2/src/google_img_source_search/google_items/image.py
+-rw-rw-rw-   0        0        0      202 2023-07-30 09:07:43.000000 google-image-source-search-0.0.2/src/google_img_source_search/google_items/search_item.py
+-rw-rw-rw-   0        0        0     1733 2023-07-30 10:22:35.000000 google-image-source-search-0.0.2/src/google_img_source_search/reverse_image_searcher.py
```

### Comparing `google-image-source-search-0.0.1/LICENSE` & `google-image-source-search-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `google-image-source-search-0.0.1/pyproject.toml` & `google-image-source-search-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "google-image-source-search"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Vorrik", email="author@example.com" },
 ]
 description = "A package to search image sources using google services"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `google-image-source-search-0.0.1/src/google_image_source_search.egg-info/SOURCES.txt` & `google-image-source-search-0.0.2/src/google_image_source_search.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-image-source-search-0.0.1/src/google_img_source_search/api_response_parser.py` & `google-image-source-search-0.0.2/src/google_img_source_search/api_response_parser.py`

 * *Files identical despite different names*

### Comparing `google-image-source-search-0.0.1/src/google_img_source_search/batchexecute_decoder.py` & `google-image-source-search-0.0.2/src/google_img_source_search/batchexecute_decoder.py`

 * *Files identical despite different names*

### Comparing `google-image-source-search-0.0.1/src/google_img_source_search/f_req_template.py` & `google-image-source-search-0.0.2/src/google_img_source_search/f_req_template.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 def build_f_req(id_1: str, id_2: str):
     return rf'[[["B7fdke","[[\"{id_1}\",1,1],[null,null,null,null,null,null,' \
            r'[\"\"],' \
            rf'[\"{id_2}\",[null,null,0,0]]],[null,null,' \
-           r'null,null,3,[\"ru\",null,\"US\",\"Europe/Moscow\"],null,null,[null,null,null,null,null,null,null,null,' \
+           r'null,null,3,[\"en-US\",null,\"US\",\"Europe/Moscow\"],null,null,[null,null,null,null,null,null,null,null,' \
            r'null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,' \
            r'null,null,null,null,null,1,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,' \
            r'null,null,null,null,null,null,null,null,null,null,null,null,null,null,1,null,null,null,null,null,null,' \
            r'null,null,null,null,null,null,1,null,null,null,null,null,1,null,null,null,1,null,null,null,null,null,' \
            r'null,1,1,null,null,null,null,1,null,1,null,null,1],[[null,1,1,1,1,1,1,null,null,null,1,1,1,1,null,null,' \
            r'null,1,null,null,null,null,null,null,null,null,null,1,null,null,null,null,null,null,null,null,1,null,' \
            r'null,null,null,null,null,null,1,null,null,null,null,null,null,null,null,1,null,null,null,null,null,null,' \
```

### Comparing `google-image-source-search-0.0.1/src/google_img_source_search/reverse_image_searcher.py` & `google-image-source-search-0.0.2/src/google_img_source_search/reverse_image_searcher.py`

 * *Files identical despite different names*

