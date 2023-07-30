# Comparing `tmp/datawords-0.7.1.tar.gz` & `tmp/datawords-0.7.2.tar.gz`

## Comparing `datawords-0.7.1.tar` & `datawords-0.7.2.tar`

### file list

```diff
@@ -1,46 +1,47 @@
--rw-r--r--   0        0        0    20849 2020-02-02 00:00:00.000000 datawords-0.7.1/.pylintrc
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 datawords-0.7.1/Makefile
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 datawords-0.7.1/mypy.ini
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 datawords-0.7.1/readthedocs.yml
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 datawords-0.7.1/datawords/__about__.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 datawords-0.7.1/datawords/__init__.py
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 datawords-0.7.1/datawords/_utils.py
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 datawords-0.7.1/datawords/constants.py
--rw-r--r--   0        0        0    15202 2020-02-02 00:00:00.000000 datawords-0.7.1/datawords/indexes.py
--rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 datawords-0.7.1/datawords/install_pytorch.py
--rw-r--r--   0        0        0     6074 2020-02-02 00:00:00.000000 datawords-0.7.1/datawords/models.py
--rw-r--r--   0        0        0    14532 2020-02-02 00:00:00.000000 datawords-0.7.1/datawords/parsers.py
--rw-r--r--   0        0        0     7034 2020-02-02 00:00:00.000000 datawords-0.7.1/datawords/ranking.py
--rw-r--r--   0        0        0     5872 2020-02-02 00:00:00.000000 datawords-0.7.1/datawords/utils.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 datawords-0.7.1/datawords/deepnlp/__init__.py
--rw-r--r--   0        0        0     3387 2020-02-02 00:00:00.000000 datawords-0.7.1/datawords/deepnlp/core.py
--rw-r--r--   0        0        0     4001 2020-02-02 00:00:00.000000 datawords-0.7.1/datawords/deepnlp/translators.py
--rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 datawords-0.7.1/datawords/deepnlp/translators2.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 datawords-0.7.1/datawords/deepnlp/utils.py
--rw-r--r--   0        0        0     6276 2020-02-02 00:00:00.000000 datawords-0.7.1/datawords/files/stop_en.txt
--rw-r--r--   0        0        0     4421 2020-02-02 00:00:00.000000 datawords-0.7.1/datawords/files/stop_es.txt
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 datawords-0.7.1/datawords/files/stop_pt.txt
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 datawords-0.7.1/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 datawords-0.7.1/docs/make.bat
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 datawords-0.7.1/docs/source/api_reference.rst
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 datawords-0.7.1/docs/source/conf.py
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 datawords-0.7.1/docs/source/index.rst
--rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 datawords-0.7.1/docs/source/introduction.rst
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 datawords-0.7.1/docs/source/api/deepnlp.rst
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 datawords-0.7.1/docs/source/api/indexes.rst
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 datawords-0.7.1/docs/source/api/models.rst
--rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 datawords-0.7.1/docs/source/api/parsers.rst
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 datawords-0.7.1/docs/source/api/ranking.rst
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 datawords-0.7.1/tests/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 datawords-0.7.1/tests/shared.py
--rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 datawords-0.7.1/tests/test_indexes.py
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 datawords-0.7.1/tests/test_models.py
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 datawords-0.7.1/tests/test_parsers.py
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 datawords-0.7.1/tests/test_rankings.py
--rw-r--r--   0        0        0    21956 2020-02-02 00:00:00.000000 datawords-0.7.1/tests/texts.txt
--rw-r--r--   0        0        0     7876 2020-02-02 00:00:00.000000 datawords-0.7.1/.gitignore
--rw-r--r--   0        0        0    15977 2020-02-02 00:00:00.000000 datawords-0.7.1/LICENSE
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 datawords-0.7.1/NOTICE.md
--rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 datawords-0.7.1/README.md
--rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 datawords-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 datawords-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0    20849 2020-02-02 00:00:00.000000 datawords-0.7.2/.pylintrc
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 datawords-0.7.2/Makefile
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 datawords-0.7.2/mypy.ini
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 datawords-0.7.2/readthedocs.yml
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 datawords-0.7.2/datawords/__about__.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 datawords-0.7.2/datawords/__init__.py
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 datawords-0.7.2/datawords/_utils.py
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 datawords-0.7.2/datawords/constants.py
+-rw-r--r--   0        0        0    15230 2020-02-02 00:00:00.000000 datawords-0.7.2/datawords/indexes.py
+-rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 datawords-0.7.2/datawords/install_pytorch.py
+-rw-r--r--   0        0        0     6074 2020-02-02 00:00:00.000000 datawords-0.7.2/datawords/models.py
+-rw-r--r--   0        0        0    14532 2020-02-02 00:00:00.000000 datawords-0.7.2/datawords/parsers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 datawords-0.7.2/datawords/py.typed
+-rw-r--r--   0        0        0     7034 2020-02-02 00:00:00.000000 datawords-0.7.2/datawords/ranking.py
+-rw-r--r--   0        0        0     5872 2020-02-02 00:00:00.000000 datawords-0.7.2/datawords/utils.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 datawords-0.7.2/datawords/deepnlp/__init__.py
+-rw-r--r--   0        0        0     3387 2020-02-02 00:00:00.000000 datawords-0.7.2/datawords/deepnlp/core.py
+-rw-r--r--   0        0        0     4001 2020-02-02 00:00:00.000000 datawords-0.7.2/datawords/deepnlp/translators.py
+-rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 datawords-0.7.2/datawords/deepnlp/translators2.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 datawords-0.7.2/datawords/deepnlp/utils.py
+-rw-r--r--   0        0        0     6276 2020-02-02 00:00:00.000000 datawords-0.7.2/datawords/files/stop_en.txt
+-rw-r--r--   0        0        0     4421 2020-02-02 00:00:00.000000 datawords-0.7.2/datawords/files/stop_es.txt
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 datawords-0.7.2/datawords/files/stop_pt.txt
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 datawords-0.7.2/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 datawords-0.7.2/docs/make.bat
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 datawords-0.7.2/docs/source/api_reference.rst
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 datawords-0.7.2/docs/source/conf.py
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 datawords-0.7.2/docs/source/index.rst
+-rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 datawords-0.7.2/docs/source/introduction.rst
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 datawords-0.7.2/docs/source/api/deepnlp.rst
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 datawords-0.7.2/docs/source/api/indexes.rst
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 datawords-0.7.2/docs/source/api/models.rst
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 datawords-0.7.2/docs/source/api/parsers.rst
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 datawords-0.7.2/docs/source/api/ranking.rst
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 datawords-0.7.2/tests/__init__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 datawords-0.7.2/tests/shared.py
+-rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 datawords-0.7.2/tests/test_indexes.py
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 datawords-0.7.2/tests/test_models.py
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 datawords-0.7.2/tests/test_parsers.py
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 datawords-0.7.2/tests/test_rankings.py
+-rw-r--r--   0        0        0    21956 2020-02-02 00:00:00.000000 datawords-0.7.2/tests/texts.txt
+-rw-r--r--   0        0        0     7876 2020-02-02 00:00:00.000000 datawords-0.7.2/.gitignore
+-rw-r--r--   0        0        0    15977 2020-02-02 00:00:00.000000 datawords-0.7.2/LICENSE
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 datawords-0.7.2/NOTICE.md
+-rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 datawords-0.7.2/README.md
+-rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 datawords-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 datawords-0.7.2/PKG-INFO
```

### Comparing `datawords-0.7.1/.pylintrc` & `datawords-0.7.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `datawords-0.7.1/Makefile` & `datawords-0.7.2/Makefile`

 * *Files identical despite different names*

### Comparing `datawords-0.7.1/datawords/_utils.py` & `datawords-0.7.2/datawords/_utils.py`

 * *Files identical despite different names*

### Comparing `datawords-0.7.1/datawords/constants.py` & `datawords-0.7.2/datawords/constants.py`

 * *Files identical despite different names*

### Comparing `datawords-0.7.1/datawords/indexes.py` & `datawords-0.7.2/datawords/indexes.py`

 * *Files 1% similar despite different names*

```diff
@@ -270,18 +270,18 @@
         cur = self.db.cursor()
         cur.execute("PRAGMA jounral_mode=WAL;")
         cur.close()
 
     def _create_tables(self):
         cur = self.db.cursor()
         cur.execute(
-            'create virtual table search_docs using fts5(id, text, tokenize="ascii");'
+            'CREATE VIRTUAL TABLE IF NOT EXISTS search_docs using fts5(id, text, tokenize="ascii");'
         )
         cur.execute(
-            """CREATE TABLE search_index
+            """CREATE TABLE IF NOT EXISTS search_index
         (id INTEGER PRIMARY KEY,doc_id TEXT NOT NULL UNIQUE);"""
         )
         cur.close()
 
     def _parse(self, txt) -> List[str]:
         tokens = parsers.doc_parser(
             txt,
```

### Comparing `datawords-0.7.1/datawords/install_pytorch.py` & `datawords-0.7.2/datawords/install_pytorch.py`

 * *Files identical despite different names*

### Comparing `datawords-0.7.1/datawords/models.py` & `datawords-0.7.2/datawords/models.py`

 * *Files identical despite different names*

### Comparing `datawords-0.7.1/datawords/parsers.py` & `datawords-0.7.2/datawords/parsers.py`

 * *Files identical despite different names*

### Comparing `datawords-0.7.1/datawords/ranking.py` & `datawords-0.7.2/datawords/ranking.py`

 * *Files identical despite different names*

### Comparing `datawords-0.7.1/datawords/utils.py` & `datawords-0.7.2/datawords/utils.py`

 * *Files identical despite different names*

### Comparing `datawords-0.7.1/datawords/deepnlp/core.py` & `datawords-0.7.2/datawords/deepnlp/core.py`

 * *Files identical despite different names*

### Comparing `datawords-0.7.1/datawords/deepnlp/translators.py` & `datawords-0.7.2/datawords/deepnlp/translators.py`

 * *Files identical despite different names*

### Comparing `datawords-0.7.1/datawords/deepnlp/translators2.py` & `datawords-0.7.2/datawords/deepnlp/translators2.py`

 * *Files identical despite different names*

### Comparing `datawords-0.7.1/datawords/files/stop_en.txt` & `datawords-0.7.2/datawords/files/stop_en.txt`

 * *Files identical despite different names*

### Comparing `datawords-0.7.1/datawords/files/stop_es.txt` & `datawords-0.7.2/datawords/files/stop_es.txt`

 * *Files identical despite different names*

### Comparing `datawords-0.7.1/datawords/files/stop_pt.txt` & `datawords-0.7.2/datawords/files/stop_pt.txt`

 * *Files identical despite different names*

### Comparing `datawords-0.7.1/docs/Makefile` & `datawords-0.7.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `datawords-0.7.1/docs/make.bat` & `datawords-0.7.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `datawords-0.7.1/docs/source/conf.py` & `datawords-0.7.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `datawords-0.7.1/docs/source/index.rst` & `datawords-0.7.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `datawords-0.7.1/docs/source/introduction.rst` & `datawords-0.7.2/docs/source/introduction.rst`

 * *Files identical despite different names*

### Comparing `datawords-0.7.1/docs/source/api/deepnlp.rst` & `datawords-0.7.2/docs/source/api/deepnlp.rst`

 * *Files identical despite different names*

### Comparing `datawords-0.7.1/docs/source/api/indexes.rst` & `datawords-0.7.2/docs/source/api/indexes.rst`

 * *Files identical despite different names*

### Comparing `datawords-0.7.1/docs/source/api/parsers.rst` & `datawords-0.7.2/docs/source/api/parsers.rst`

 * *Files identical despite different names*

### Comparing `datawords-0.7.1/tests/test_indexes.py` & `datawords-0.7.2/tests/test_indexes.py`

 * *Files identical despite different names*

### Comparing `datawords-0.7.1/tests/test_models.py` & `datawords-0.7.2/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `datawords-0.7.1/tests/test_parsers.py` & `datawords-0.7.2/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `datawords-0.7.1/tests/test_rankings.py` & `datawords-0.7.2/tests/test_rankings.py`

 * *Files identical despite different names*

### Comparing `datawords-0.7.1/tests/texts.txt` & `datawords-0.7.2/tests/texts.txt`

 * *Files identical despite different names*

### Comparing `datawords-0.7.1/.gitignore` & `datawords-0.7.2/.gitignore`

 * *Files identical despite different names*

### Comparing `datawords-0.7.1/LICENSE` & `datawords-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `datawords-0.7.1/README.md` & `datawords-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `datawords-0.7.1/pyproject.toml` & `datawords-0.7.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datawords-0.7.1/PKG-INFO` & `datawords-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datawords
-Version: 0.7.1
+Version: 0.7.2
 Summary: A library to work with text data
 Project-URL: Documentation, https://github.com/unknown/datawords#readme
 Project-URL: Issues, https://github.com/unknown/datawords/issues
 Project-URL: Source, https://github.com/unknown/datawords
 Author-email: Xavier Petit <nuxion@gmail.com>
 License-Expression: MPL-2.0
 License-File: LICENSE
```

