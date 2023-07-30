# Comparing `tmp/totolo-0.3.tar.gz` & `tmp/totolo-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "totolo-0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "totolo-0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `totolo-0.3.tar` & `totolo-0.4.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     1112 2023-07-29 15:49:20.024088 totolo-0.3/.github/workflows/coverage.yaml
--rw-r--r--   0        0        0     1409 2023-07-29 16:47:10.254067 totolo-0.3/.github/workflows/publish.yaml
--rw-r--r--   0        0        0      854 2023-07-29 15:47:06.414089 totolo-0.3/.github/workflows/test.yaml
--rw-r--r--   0        0        0     3081 2023-07-29 17:17:23.614057 totolo-0.3/.gitignore
--rw-r--r--   0        0        0      892 2023-07-20 23:49:12.905042 totolo-0.3/.vscode/launch.json
--rw-r--r--   0        0        0      277 2023-07-21 08:49:08.178933 totolo-0.3/.vscode/settings.json
--rw-r--r--   0        0        0     1071 2023-07-20 23:48:27.105042 totolo-0.3/LICENSE
--rw-r--r--   0        0        0      729 2023-07-27 20:44:23.163611 totolo-0.3/README.md
--rw-r--r--   0        0        0     1259 2023-07-28 19:07:41.098512 totolo-0.3/pyproject.toml
--rw-r--r--   0        0        0       38 2023-07-26 12:59:05.647420 totolo-0.3/requirements-dev.txt
--rw-r--r--   0        0        0        0 2023-07-21 07:16:17.008968 totolo-0.3/tests/__init__.py
--rw-r--r--   0        0        0       24 2023-07-21 07:17:42.658967 totolo-0.3/tests/data/cycles1.th.txt
--rw-r--r--   0        0        0       47 2023-07-21 07:17:42.658967 totolo-0.3/tests/data/cycles2.th.txt
--rw-r--r--   0        0        0       71 2023-07-21 07:17:42.658967 totolo-0.3/tests/data/cycles3.th.txt
--rw-r--r--   0        0        0   173716 2023-07-21 19:07:30.830223 totolo-0.3/tests/data/film-timeout-top100.st.txt
--rw-r--r--   0        0        0   332534 2023-07-28 18:29:09.328525 totolo-0.3/tests/data/flat.tar.gz
--rw-r--r--   0        0        0      166 2023-07-28 14:22:48.076573 totolo-0.3/tests/data/messy.st.txt
--rw-r--r--   0        0        0   332557 2023-07-27 20:34:04.643615 totolo-0.3/tests/data/sample-2023.07.23.tar.gz
--rw-r--r--   0        0        0    34632 2023-07-23 17:10:34.367505 totolo-0.3/tests/data/sample-2023.07.23/notes/collections/scifi-collections.st.txt
--rw-r--r--   0        0        0    28050 2023-07-28 11:58:13.902891 totolo-0.3/tests/data/sample-2023.07.23/notes/stories/film/film-scifi-1920s.st.txt
--rw-r--r--   0        0        0    48760 2023-07-23 17:10:34.367505 totolo-0.3/tests/data/sample-2023.07.23/notes/stories/film/film-scifi-1930s.st.txt
--rw-r--r--   0        0        0  1011578 2023-07-24 15:45:57.955943 totolo-0.3/tests/data/sample-2023.07.23/notes/themes/primary.th.txt
--rw-r--r--   0        0        0    14882 2023-07-24 15:45:57.955943 totolo-0.3/tests/data/sample-2023.07.23/notes/themes/timeperiod.th.txt
--rw-r--r--   0        0        0      428 2023-07-21 19:17:22.740219 totolo-0.3/tests/data/storytree.st.txt
--rw-r--r--   0        0        0  1011579 2023-07-21 08:01:34.098951 totolo-0.3/tests/data/to-2023.07.09.th.txt
--rw-r--r--   0        0        0     2365 2023-07-28 11:18:26.352906 totolo-0.3/tests/data/to-sample-2023.07.09-copy.st.txt
--rw-r--r--   0        0        0     2365 2023-07-22 14:49:15.654562 totolo-0.3/tests/data/to-sample-2023.07.09.st.txt
--rw-r--r--   0        0        0     6150 2023-07-28 07:54:27.717457 totolo-0.3/tests/test_entries.py
--rw-r--r--   0        0        0     5692 2023-07-28 19:02:13.738514 totolo-0.3/tests/test_impl.py
--rw-r--r--   0        0        0     2219 2023-07-28 18:43:03.928521 totolo-0.3/tests/test_lib.py
--rw-r--r--   0        0        0    10843 2023-07-28 16:10:26.086532 totolo-0.3/tests/test_totolo.py
--rw-r--r--   0        0        0      189 2023-07-29 15:22:50.924097 totolo-0.3/totolo/__init__.py
--rw-r--r--   0        0        0     1201 2023-07-26 18:32:07.507797 totolo-0.3/totolo/api.py
--rw-r--r--   0        0        0        0 2023-07-20 23:47:51.775042 totolo-0.3/totolo/impl/__init__.py
--rw-r--r--   0        0        0     2953 2023-07-28 19:02:31.728514 totolo-0.3/totolo/impl/core.py
--rw-r--r--   0        0        0     5245 2023-07-28 19:57:11.728495 totolo-0.3/totolo/impl/entry.py
--rw-r--r--   0        0        0     3160 2023-07-28 18:52:24.978517 totolo-0.3/totolo/impl/field.py
--rw-r--r--   0        0        0      424 2023-07-23 05:18:38.591248 totolo-0.3/totolo/impl/keyword.py
--rw-r--r--   0        0        0     7567 2023-07-28 19:07:02.088512 totolo-0.3/totolo/impl/parser.py
--rw-r--r--   0        0        0        0 2023-07-20 23:47:51.775042 totolo-0.3/totolo/lib/__init__.py
--rw-r--r--   0        0        0     1134 2023-07-28 18:49:06.178518 totolo-0.3/totolo/lib/files.py
--rw-r--r--   0        0        0     1283 2023-07-28 18:48:39.808519 totolo-0.3/totolo/lib/textformat.py
--rw-r--r--   0        0        0     3456 2023-07-28 19:56:14.668495 totolo-0.3/totolo/story.py
--rw-r--r--   0        0        0     2209 2023-07-28 19:56:03.888495 totolo-0.3/totolo/theme.py
--rw-r--r--   0        0        0     6687 2023-07-28 18:47:09.658519 totolo-0.3/totolo/themeontology.py
--rw-r--r--   0        0        0     1161 1970-01-01 00:00:00.000000 totolo-0.3/PKG-INFO
+-rw-r--r--   0        0        0     1112 2023-07-29 17:30:46.754441 totolo-0.4/.github/workflows/coverage.yaml
+-rw-r--r--   0        0        0     1400 2023-07-29 17:30:46.754441 totolo-0.4/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0      854 2023-07-29 17:30:46.754441 totolo-0.4/.github/workflows/test.yaml
+-rw-r--r--   0        0        0     3081 2023-07-29 17:30:46.754441 totolo-0.4/.gitignore
+-rw-r--r--   0        0        0      892 2023-07-29 17:30:46.754441 totolo-0.4/.vscode/launch.json
+-rw-r--r--   0        0        0      277 2023-07-29 17:30:46.754441 totolo-0.4/.vscode/settings.json
+-rw-r--r--   0        0        0     1071 2023-07-29 17:30:46.754441 totolo-0.4/LICENSE
+-rw-r--r--   0        0        0      729 2023-07-29 17:30:46.754441 totolo-0.4/README.md
+-rw-r--r--   0        0        0     1259 2023-07-29 17:30:46.754441 totolo-0.4/pyproject.toml
+-rw-r--r--   0        0        0       38 2023-07-29 17:30:46.754441 totolo-0.4/requirements-dev.txt
+-rw-r--r--   0        0        0        0 2023-07-29 17:30:46.754441 totolo-0.4/tests/__init__.py
+-rw-r--r--   0        0        0       24 2023-07-29 17:30:46.754441 totolo-0.4/tests/data/cycles1.th.txt
+-rw-r--r--   0        0        0       47 2023-07-29 17:30:46.754441 totolo-0.4/tests/data/cycles2.th.txt
+-rw-r--r--   0        0        0       71 2023-07-29 17:30:46.754441 totolo-0.4/tests/data/cycles3.th.txt
+-rw-r--r--   0        0        0   173716 2023-07-29 17:30:46.754441 totolo-0.4/tests/data/film-timeout-top100.st.txt
+-rw-r--r--   0        0        0   332534 2023-07-29 17:30:46.758441 totolo-0.4/tests/data/flat.tar.gz
+-rw-r--r--   0        0        0      166 2023-07-29 17:30:46.758441 totolo-0.4/tests/data/messy.st.txt
+-rw-r--r--   0        0        0   332557 2023-07-29 17:30:46.758441 totolo-0.4/tests/data/sample-2023.07.23.tar.gz
+-rw-r--r--   0        0        0    34632 2023-07-29 17:30:46.758441 totolo-0.4/tests/data/sample-2023.07.23/notes/collections/scifi-collections.st.txt
+-rw-r--r--   0        0        0    28050 2023-07-29 17:30:46.758441 totolo-0.4/tests/data/sample-2023.07.23/notes/stories/film/film-scifi-1920s.st.txt
+-rw-r--r--   0        0        0    48760 2023-07-29 17:30:46.758441 totolo-0.4/tests/data/sample-2023.07.23/notes/stories/film/film-scifi-1930s.st.txt
+-rw-r--r--   0        0        0  1011578 2023-07-29 17:30:46.762441 totolo-0.4/tests/data/sample-2023.07.23/notes/themes/primary.th.txt
+-rw-r--r--   0        0        0    14882 2023-07-29 17:30:46.762441 totolo-0.4/tests/data/sample-2023.07.23/notes/themes/timeperiod.th.txt
+-rw-r--r--   0        0        0      428 2023-07-29 17:30:46.762441 totolo-0.4/tests/data/storytree.st.txt
+-rw-r--r--   0        0        0  1011579 2023-07-29 17:30:46.770441 totolo-0.4/tests/data/to-2023.07.09.th.txt
+-rw-r--r--   0        0        0     2365 2023-07-29 17:30:46.770441 totolo-0.4/tests/data/to-sample-2023.07.09-copy.st.txt
+-rw-r--r--   0        0        0     2365 2023-07-29 17:30:46.770441 totolo-0.4/tests/data/to-sample-2023.07.09.st.txt
+-rw-r--r--   0        0        0     6150 2023-07-29 17:30:46.770441 totolo-0.4/tests/test_entries.py
+-rw-r--r--   0        0        0     5692 2023-07-29 17:30:46.770441 totolo-0.4/tests/test_impl.py
+-rw-r--r--   0        0        0     2219 2023-07-29 17:30:46.770441 totolo-0.4/tests/test_lib.py
+-rw-r--r--   0        0        0    10843 2023-07-29 17:30:46.770441 totolo-0.4/tests/test_totolo.py
+-rw-r--r--   0        0        0      189 2023-07-29 17:30:46.770441 totolo-0.4/totolo/__init__.py
+-rw-r--r--   0        0        0     1201 2023-07-29 17:30:46.770441 totolo-0.4/totolo/api.py
+-rw-r--r--   0        0        0        0 2023-07-29 17:30:46.770441 totolo-0.4/totolo/impl/__init__.py
+-rw-r--r--   0        0        0     2953 2023-07-29 17:30:46.770441 totolo-0.4/totolo/impl/core.py
+-rw-r--r--   0        0        0     5245 2023-07-29 17:30:46.770441 totolo-0.4/totolo/impl/entry.py
+-rw-r--r--   0        0        0     3160 2023-07-29 17:30:46.770441 totolo-0.4/totolo/impl/field.py
+-rw-r--r--   0        0        0      424 2023-07-29 17:30:46.770441 totolo-0.4/totolo/impl/keyword.py
+-rw-r--r--   0        0        0     7567 2023-07-29 17:30:46.770441 totolo-0.4/totolo/impl/parser.py
+-rw-r--r--   0        0        0        0 2023-07-29 17:30:46.770441 totolo-0.4/totolo/lib/__init__.py
+-rw-r--r--   0        0        0     1134 2023-07-29 17:30:46.770441 totolo-0.4/totolo/lib/files.py
+-rw-r--r--   0        0        0     1283 2023-07-29 17:30:46.770441 totolo-0.4/totolo/lib/textformat.py
+-rw-r--r--   0        0        0     3456 2023-07-29 17:30:46.770441 totolo-0.4/totolo/story.py
+-rw-r--r--   0        0        0     2209 2023-07-29 17:30:46.770441 totolo-0.4/totolo/theme.py
+-rw-r--r--   0        0        0     6687 2023-07-29 17:30:46.770441 totolo-0.4/totolo/themeontology.py
+-rw-r--r--   0        0        0     1161 1970-01-01 00:00:00.000000 totolo-0.4/PKG-INFO
```

### Comparing `totolo-0.3/.github/workflows/coverage.yaml` & `totolo-0.4/.github/workflows/coverage.yaml`

 * *Files identical despite different names*

### Comparing `totolo-0.3/.github/workflows/publish.yaml` & `totolo-0.4/.github/workflows/publish.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 jobs:
 
   test-and-build:
     runs-on: ubuntu-latest
 
     environment:
       name: pypi
-      url: https://pypi.org/project/totolo/
+      url: https://pypi.org/p/totolo
 
     permissions:
       id-token: write
 
     steps:
     - uses: actions/checkout@v3
 
@@ -51,8 +51,8 @@
     - name: Build Package
       run: flit build
 
     - name: Publish package distributions to PyPI
       uses: pypa/gh-action-pypi-publish@release/v1
       with:
         password: ${{ secrets.PYPI_API_TOKEN }}
-        repository-url: https://pypi.org/project/totolo/
+        #repository-url: https://test.pypi.org/legacy/
```

### Comparing `totolo-0.3/.github/workflows/test.yaml` & `totolo-0.4/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `totolo-0.3/.gitignore` & `totolo-0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `totolo-0.3/.vscode/launch.json` & `totolo-0.4/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `totolo-0.3/LICENSE` & `totolo-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `totolo-0.3/README.md` & `totolo-0.4/README.md`

 * *Files identical despite different names*

### Comparing `totolo-0.3/pyproject.toml` & `totolo-0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `totolo-0.3/tests/data/film-timeout-top100.st.txt` & `totolo-0.4/tests/data/film-timeout-top100.st.txt`

 * *Files identical despite different names*

### Comparing `totolo-0.3/tests/data/flat.tar.gz` & `totolo-0.4/tests/data/flat.tar.gz`

 * *Files identical despite different names*

### Comparing `totolo-0.3/tests/data/sample-2023.07.23.tar.gz` & `totolo-0.4/tests/data/sample-2023.07.23.tar.gz`

 * *Files identical despite different names*

### Comparing `totolo-0.3/tests/data/sample-2023.07.23/notes/collections/scifi-collections.st.txt` & `totolo-0.4/tests/data/sample-2023.07.23/notes/collections/scifi-collections.st.txt`

 * *Files identical despite different names*

### Comparing `totolo-0.3/tests/data/sample-2023.07.23/notes/stories/film/film-scifi-1920s.st.txt` & `totolo-0.4/tests/data/sample-2023.07.23/notes/stories/film/film-scifi-1920s.st.txt`

 * *Files identical despite different names*

### Comparing `totolo-0.3/tests/data/sample-2023.07.23/notes/stories/film/film-scifi-1930s.st.txt` & `totolo-0.4/tests/data/sample-2023.07.23/notes/stories/film/film-scifi-1930s.st.txt`

 * *Files identical despite different names*

### Comparing `totolo-0.3/tests/data/sample-2023.07.23/notes/themes/primary.th.txt` & `totolo-0.4/tests/data/sample-2023.07.23/notes/themes/primary.th.txt`

 * *Files identical despite different names*

### Comparing `totolo-0.3/tests/data/sample-2023.07.23/notes/themes/timeperiod.th.txt` & `totolo-0.4/tests/data/sample-2023.07.23/notes/themes/timeperiod.th.txt`

 * *Files identical despite different names*

### Comparing `totolo-0.3/tests/data/to-2023.07.09.th.txt` & `totolo-0.4/tests/data/to-2023.07.09.th.txt`

 * *Files identical despite different names*

### Comparing `totolo-0.3/tests/data/to-sample-2023.07.09-copy.st.txt` & `totolo-0.4/tests/data/to-sample-2023.07.09-copy.st.txt`

 * *Files identical despite different names*

### Comparing `totolo-0.3/tests/data/to-sample-2023.07.09.st.txt` & `totolo-0.4/tests/data/to-sample-2023.07.09.st.txt`

 * *Files identical despite different names*

### Comparing `totolo-0.3/tests/test_entries.py` & `totolo-0.4/tests/test_entries.py`

 * *Files identical despite different names*

### Comparing `totolo-0.3/tests/test_impl.py` & `totolo-0.4/tests/test_impl.py`

 * *Files identical despite different names*

### Comparing `totolo-0.3/tests/test_lib.py` & `totolo-0.4/tests/test_lib.py`

 * *Files identical despite different names*

### Comparing `totolo-0.3/tests/test_totolo.py` & `totolo-0.4/tests/test_totolo.py`

 * *Files identical despite different names*

### Comparing `totolo-0.3/totolo/api.py` & `totolo-0.4/totolo/api.py`

 * *Files identical despite different names*

### Comparing `totolo-0.3/totolo/impl/core.py` & `totolo-0.4/totolo/impl/core.py`

 * *Files identical despite different names*

### Comparing `totolo-0.3/totolo/impl/entry.py` & `totolo-0.4/totolo/impl/entry.py`

 * *Files identical despite different names*

### Comparing `totolo-0.3/totolo/impl/field.py` & `totolo-0.4/totolo/impl/field.py`

 * *Files identical despite different names*

### Comparing `totolo-0.3/totolo/impl/parser.py` & `totolo-0.4/totolo/impl/parser.py`

 * *Files identical despite different names*

### Comparing `totolo-0.3/totolo/lib/files.py` & `totolo-0.4/totolo/lib/files.py`

 * *Files identical despite different names*

### Comparing `totolo-0.3/totolo/lib/textformat.py` & `totolo-0.4/totolo/lib/textformat.py`

 * *Files identical despite different names*

### Comparing `totolo-0.3/totolo/story.py` & `totolo-0.4/totolo/story.py`

 * *Files identical despite different names*

### Comparing `totolo-0.3/totolo/theme.py` & `totolo-0.4/totolo/theme.py`

 * *Files identical despite different names*

### Comparing `totolo-0.3/totolo/themeontology.py` & `totolo-0.4/totolo/themeontology.py`

 * *Files identical despite different names*

### Comparing `totolo-0.3/PKG-INFO` & `totolo-0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: totolo
-Version: 0.3
+Version: 0.4
 Summary: The Python interface to themeontology.org.
 Author-email: Mikael Onsjö <mikael@odinlake.net>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Project-URL: Documentation, https://github.com/theme-ontology/theming
 Project-URL: Home, https://www.themeontology.org/
 Project-URL: Source, https://github.com/theme-ontology/python-totolo
```

