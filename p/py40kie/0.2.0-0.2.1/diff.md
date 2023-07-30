# Comparing `tmp/py40kie-0.2.0.tar.gz` & `tmp/py40kie-0.2.1.tar.gz`

## Comparing `py40kie-0.2.0.tar` & `py40kie-0.2.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 py40kie-0.2.0/.github/workflows/publish-to-test-pypi.yml
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 py40kie-0.2.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py40kie-0.2.0/src/__init__.py
--rw-r--r--   0        0        0    11081 2020-02-02 00:00:00.000000 py40kie-0.2.0/src/py40kie.py
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 py40kie-0.2.0/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 py40kie-0.2.0/LICENSE
--rw-r--r--   0        0        0     3362 2020-02-02 00:00:00.000000 py40kie-0.2.0/README.md
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 py40kie-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 py40kie-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 py40kie-0.2.1/.github/workflows/publish-to-test-pypi.yml
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 py40kie-0.2.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py40kie-0.2.1/src/__init__.py
+-rw-r--r--   0        0        0    11081 2020-02-02 00:00:00.000000 py40kie-0.2.1/src/py40kie.py
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 py40kie-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 py40kie-0.2.1/LICENSE
+-rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 py40kie-0.2.1/README.md
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 py40kie-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4515 2020-02-02 00:00:00.000000 py40kie-0.2.1/PKG-INFO
```

### Comparing `py40kie-0.2.0/.github/workflows/publish-to-test-pypi.yml` & `py40kie-0.2.1/.github/workflows/publish-to-test-pypi.yml`

 * *Files identical despite different names*

### Comparing `py40kie-0.2.0/.github/workflows/python-publish.yml` & `py40kie-0.2.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `py40kie-0.2.0/src/py40kie.py` & `py40kie-0.2.1/src/py40kie.py`

 * *Files identical despite different names*

### Comparing `py40kie-0.2.0/.gitignore` & `py40kie-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `py40kie-0.2.0/LICENSE` & `py40kie-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py40kie-0.2.0/README.md` & `py40kie-0.2.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,16 @@
     - -v: Optional flag to override page extraction. Will extract only the page numbers specified from the main index  
 
 # Contributions  
 ## Future features  
 Any suggested features would be appreciated  
  - [x] Allied units from other Indexes/Imperial Armour/Legends  
  - [x] Extract Adeptus Astartes army rule page for Space Marine lists  
- - [x] Convert Google Sheet army builder lists to runnable command https://www.reddit.com/r/WarhammerCompetitive/comments/14br6rw/10e_40k_list_builder_spreadsheets/  
+ - [x] Create runnable command from [Google Sheet army builder lists](https://www.reddit.com/r/WarhammerCompetitive/comments/14br6rw/10e_40k_list_builder_spreadsheets/)  
+       Copy the cells in the yellow box from here to your own sheet: https://docs.google.com/spreadsheets/d/1A1lDqmL0f_iH9OIUQWL_v83_leyhm3t0rhyC20UfrPA  
  - [ ] Extract extra rule pages. e.g. Deathwatch Armoury  
  - [ ] Handle exceptions gracefully  
  - [ ] Webapp version?...  
 
 
 ## Issues  
-py40kie was not tested on all indexes. If there is any problem extracting cards please submit an issue https://github.com/Dragons-Ire/40k-index-pdf-extractor/issues/new
+py40kie was not tested on all indexes. If there is any problem extracting cards please submit an issue https://github.com/Dragons-Ire/40k-index-pdf-extractor/issues/new
```

### Comparing `py40kie-0.2.0/pyproject.toml` & `py40kie-0.2.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "py40kie"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="Chris Austin", email="dragons.ire.oce@gmail.com" },
 ]
 description = "Command line Python program to extract army rules and unit cards from 10th edition Warhammer 40k indexes to create army list specific pdfs with reduced file size."
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `py40kie-0.2.0/PKG-INFO` & `py40kie-0.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py40kie
-Version: 0.2.0
+Version: 0.2.1
 Summary: Command line Python program to extract army rules and unit cards from 10th edition Warhammer 40k indexes to create army list specific pdfs with reduced file size.
 Project-URL: Homepage, https://github.com/Dragons-Ire/40k-index-pdf-extractor
 Project-URL: Bug Tracker, https://github.com/Dragons-Ire/40k-index-pdf-extractor/issues
 Author-email: Chris Austin <dragons.ire.oce@gmail.com>
 License-File: LICENSE
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
@@ -63,15 +63,16 @@
     - -v: Optional flag to override page extraction. Will extract only the page numbers specified from the main index  
 
 # Contributions  
 ## Future features  
 Any suggested features would be appreciated  
  - [x] Allied units from other Indexes/Imperial Armour/Legends  
  - [x] Extract Adeptus Astartes army rule page for Space Marine lists  
- - [x] Convert Google Sheet army builder lists to runnable command https://www.reddit.com/r/WarhammerCompetitive/comments/14br6rw/10e_40k_list_builder_spreadsheets/  
+ - [x] Create runnable command from [Google Sheet army builder lists](https://www.reddit.com/r/WarhammerCompetitive/comments/14br6rw/10e_40k_list_builder_spreadsheets/)  
+       Copy the cells in the yellow box from here to your own sheet: https://docs.google.com/spreadsheets/d/1A1lDqmL0f_iH9OIUQWL_v83_leyhm3t0rhyC20UfrPA  
  - [ ] Extract extra rule pages. e.g. Deathwatch Armoury  
  - [ ] Handle exceptions gracefully  
  - [ ] Webapp version?...  
 
 
 ## Issues  
-py40kie was not tested on all indexes. If there is any problem extracting cards please submit an issue https://github.com/Dragons-Ire/40k-index-pdf-extractor/issues/new
+py40kie was not tested on all indexes. If there is any problem extracting cards please submit an issue https://github.com/Dragons-Ire/40k-index-pdf-extractor/issues/new
```

