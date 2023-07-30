# Comparing `tmp/hojichar-0.7.1.tar.gz` & `tmp/hojichar-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hojichar-0.7.1.tar", max compression
+gzip compressed data, was "hojichar-0.7.2.tar", max compression
```

## Comparing `hojichar-0.7.1.tar` & `hojichar-0.7.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    11357 2023-07-29 05:26:46.953899 hojichar-0.7.1/LICENSE
--rw-r--r--   0        0        0    14086 2023-07-29 05:26:46.953899 hojichar-0.7.1/README.md
--rw-r--r--   0        0        0      547 2023-07-29 05:27:06.330181 hojichar-0.7.1/hojichar/__init__.py
--rw-r--r--   0        0        0     4264 2023-07-29 05:26:46.953899 hojichar-0.7.1/hojichar/cli.py
--rw-r--r--   0        0        0       42 2023-07-29 05:26:46.953899 hojichar-0.7.1/hojichar/core/__init__.py
--rw-r--r--   0        0        0     5039 2023-07-29 05:26:46.953899 hojichar-0.7.1/hojichar/core/composition.py
--rw-r--r--   0        0        0     5638 2023-07-29 05:26:46.953899 hojichar-0.7.1/hojichar/core/filter_interface.py
--rw-r--r--   0        0        0     6221 2023-07-29 05:26:46.953899 hojichar-0.7.1/hojichar/core/inspection.py
--rw-r--r--   0        0        0     1087 2023-07-29 05:26:46.953899 hojichar-0.7.1/hojichar/core/models.py
--rw-r--r--   0        0        0      147 2023-07-29 05:26:46.953899 hojichar-0.7.1/hojichar/dict/__init__.py
--rw-r--r--   0        0        0      941 2023-07-29 05:26:46.953899 hojichar-0.7.1/hojichar/dict/adult_keywords_en.txt
--rw-r--r--   0        0        0    18091 2023-07-29 05:26:46.953899 hojichar-0.7.1/hojichar/dict/adult_keywords_ja.txt
--rw-r--r--   0        0        0      426 2023-07-29 05:26:46.953899 hojichar-0.7.1/hojichar/dict/advertisement_keywords_ja.txt
--rw-r--r--   0        0        0     1740 2023-07-29 05:26:46.953899 hojichar-0.7.1/hojichar/dict/discrimination_keywords_ja.txt
--rw-r--r--   0        0        0       67 2023-07-29 05:26:46.953899 hojichar-0.7.1/hojichar/dict/dummy_ng_words.txt
--rw-r--r--   0        0        0      577 2023-07-29 05:26:46.953899 hojichar-0.7.1/hojichar/dict/header_footer_keywords_ja.txt
--rw-r--r--   0        0        0      665 2023-07-29 05:26:46.953899 hojichar-0.7.1/hojichar/dict/violence_keywords_ja.txt
--rw-r--r--   0        0        0      711 2023-07-29 05:26:46.953899 hojichar-0.7.1/hojichar/filters/__init__.py
--rw-r--r--   0        0        0    12104 2023-07-29 05:26:46.953899 hojichar-0.7.1/hojichar/filters/deduplication.py
--rw-r--r--   0        0        0    23939 2023-07-29 05:26:46.953899 hojichar-0.7.1/hojichar/filters/document_filters.py
--rw-r--r--   0        0        0     1606 2023-07-29 05:26:46.953899 hojichar-0.7.1/hojichar/filters/token_filters.py
--rw-r--r--   0        0        0     2530 2023-07-29 05:26:46.953899 hojichar-0.7.1/hojichar/filters/tokenization.py
--rw-r--r--   0        0        0        0 2023-07-29 05:26:46.953899 hojichar-0.7.1/hojichar/py.typed
--rw-r--r--   0        0        0      595 2023-07-29 05:26:46.953899 hojichar-0.7.1/hojichar/utils/__init__.py
--rw-r--r--   0        0        0     1716 2023-07-29 05:26:46.953899 hojichar-0.7.1/hojichar/utils/io_iter.py
--rw-r--r--   0        0        0     3380 2023-07-29 05:26:46.953899 hojichar-0.7.1/hojichar/utils/load_compose.py
--rw-r--r--   0        0        0     1920 2023-07-29 05:26:46.953899 hojichar-0.7.1/hojichar/utils/process.py
--rw-r--r--   0        0        0     1746 2023-07-29 05:27:06.330181 hojichar-0.7.1/pyproject.toml
--rw-r--r--   0        0        0    14819 1970-01-01 00:00:00.000000 hojichar-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-30 04:53:08.258978 hojichar-0.7.2/LICENSE
+-rw-r--r--   0        0        0    14086 2023-07-30 04:53:08.258978 hojichar-0.7.2/README.md
+-rw-r--r--   0        0        0      547 2023-07-30 04:53:29.338961 hojichar-0.7.2/hojichar/__init__.py
+-rw-r--r--   0        0        0     4408 2023-07-30 04:53:08.258978 hojichar-0.7.2/hojichar/cli.py
+-rw-r--r--   0        0        0       42 2023-07-30 04:53:08.258978 hojichar-0.7.2/hojichar/core/__init__.py
+-rw-r--r--   0        0        0     5039 2023-07-30 04:53:08.258978 hojichar-0.7.2/hojichar/core/composition.py
+-rw-r--r--   0        0        0     5638 2023-07-30 04:53:08.258978 hojichar-0.7.2/hojichar/core/filter_interface.py
+-rw-r--r--   0        0        0     6221 2023-07-30 04:53:08.258978 hojichar-0.7.2/hojichar/core/inspection.py
+-rw-r--r--   0        0        0     1087 2023-07-30 04:53:08.258978 hojichar-0.7.2/hojichar/core/models.py
+-rw-r--r--   0        0        0      147 2023-07-30 04:53:08.258978 hojichar-0.7.2/hojichar/dict/__init__.py
+-rw-r--r--   0        0        0      941 2023-07-30 04:53:08.258978 hojichar-0.7.2/hojichar/dict/adult_keywords_en.txt
+-rw-r--r--   0        0        0    18091 2023-07-30 04:53:08.258978 hojichar-0.7.2/hojichar/dict/adult_keywords_ja.txt
+-rw-r--r--   0        0        0      426 2023-07-30 04:53:08.258978 hojichar-0.7.2/hojichar/dict/advertisement_keywords_ja.txt
+-rw-r--r--   0        0        0     1740 2023-07-30 04:53:08.258978 hojichar-0.7.2/hojichar/dict/discrimination_keywords_ja.txt
+-rw-r--r--   0        0        0       67 2023-07-30 04:53:08.258978 hojichar-0.7.2/hojichar/dict/dummy_ng_words.txt
+-rw-r--r--   0        0        0      577 2023-07-30 04:53:08.258978 hojichar-0.7.2/hojichar/dict/header_footer_keywords_ja.txt
+-rw-r--r--   0        0        0      665 2023-07-30 04:53:08.258978 hojichar-0.7.2/hojichar/dict/violence_keywords_ja.txt
+-rw-r--r--   0        0        0      711 2023-07-30 04:53:08.258978 hojichar-0.7.2/hojichar/filters/__init__.py
+-rw-r--r--   0        0        0    12104 2023-07-30 04:53:08.258978 hojichar-0.7.2/hojichar/filters/deduplication.py
+-rw-r--r--   0        0        0    23939 2023-07-30 04:53:08.258978 hojichar-0.7.2/hojichar/filters/document_filters.py
+-rw-r--r--   0        0        0     1606 2023-07-30 04:53:08.258978 hojichar-0.7.2/hojichar/filters/token_filters.py
+-rw-r--r--   0        0        0     2530 2023-07-30 04:53:08.258978 hojichar-0.7.2/hojichar/filters/tokenization.py
+-rw-r--r--   0        0        0        0 2023-07-30 04:53:08.258978 hojichar-0.7.2/hojichar/py.typed
+-rw-r--r--   0        0        0      595 2023-07-30 04:53:08.258978 hojichar-0.7.2/hojichar/utils/__init__.py
+-rw-r--r--   0        0        0     1716 2023-07-30 04:53:08.258978 hojichar-0.7.2/hojichar/utils/io_iter.py
+-rw-r--r--   0        0        0     3380 2023-07-30 04:53:08.258978 hojichar-0.7.2/hojichar/utils/load_compose.py
+-rw-r--r--   0        0        0     1920 2023-07-30 04:53:08.258978 hojichar-0.7.2/hojichar/utils/process.py
+-rw-r--r--   0        0        0     1746 2023-07-30 04:53:29.334961 hojichar-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0    14819 1970-01-01 00:00:00.000000 hojichar-0.7.2/PKG-INFO
```

### Comparing `hojichar-0.7.1/LICENSE` & `hojichar-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hojichar-0.7.1/README.md` & `hojichar-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `hojichar-0.7.1/hojichar/__init__.py` & `hojichar-0.7.2/hojichar/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 .. include:: ../README.md
 """
 from .core.composition import Compose
 from .core.filter_interface import Filter, TokenFilter
 from .core.models import Document, Token
 from .filters import deduplication, document_filters, token_filters, tokenization
 
-__version__ = "0.7.1"  # Replaced by poetry-dynamic-versioning when deploying
+__version__ = "0.7.2"  # Replaced by poetry-dynamic-versioning when deploying
 
 __all__ = [
     "core",
     "filters",
     "utils",
     "Compose",
     "Filter",
```

### Comparing `hojichar-0.7.1/hojichar/cli.py` & `hojichar-0.7.2/hojichar/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import argparse
 import functools
 import json
 import logging
 import multiprocessing
 import os
+import signal
 import sys
 from typing import Dict, Iterator, Tuple
 
 import hojichar
 from hojichar.core.inspection import StatsContainer
 from hojichar.utils.io_iter import fileout_from_iter, stdin_iter, stdout_from_iter
 from hojichar.utils.load_compose import load_compose
@@ -67,14 +68,15 @@
         help="The number ob parallel jobs. By default, the nuber of the CPU core.",
     )
     args = parser.parse_args()
     return args
 
 
 def init_worker(filter: hojichar.Compose, args: argparse.Namespace) -> None:
+    signal.signal(signal.SIGINT, signal.SIG_IGN)
     global MAIN_FILTER, CLI_ARGS
     MAIN_FILTER = filter
     CLI_ARGS = args
 
 
 def worker(doc: hojichar.Document) -> Tuple[hojichar.Document, int, StatsContainer]:
     global MAIN_FILTER, CLI_ARGS
@@ -101,29 +103,34 @@
 def main() -> None:
     pid_stats: Dict[int, StatsContainer] = dict()
 
     args = argparser()
     input_iter = stdin_iter()
     input_doc_iter = (hojichar.Document(s) for s in input_iter)
     filter = load_compose(args.profile, *tuple(args.args))
-    with multiprocessing.Pool(
+    pool = multiprocessing.Pool(
         processes=args.jobs, initializer=init_worker, initargs=(filter, args)
-    ) as pool:
+    )
+    try:
         worker_out_iter = pool.imap_unordered(worker, input_doc_iter)
         out_doc_iter = out_doc_generator(worker_out_iter, pid_stats)
         out_str_iter = (
             (doc.text for doc in out_doc_iter)
             if args.all
             else (doc.text for doc in out_doc_iter if not doc.is_rejected)
         )
         if args.output:
             with open(args.output, "w") as fp:
                 fileout_from_iter(out_str_iter, fp)
         else:
             stdout_from_iter(out_str_iter)
+    finally:
+        pool.close()
+        pool.join()
+        pool.terminate()
 
     stats: StatsContainer = functools.reduce(lambda x, y: x + y, pid_stats.values())
     print(
         json.dumps(stats.get_human_readable_values(), ensure_ascii=False, indent=2),
         file=sys.stderr,
     )
     if args.dump_stats:
```

### Comparing `hojichar-0.7.1/hojichar/core/composition.py` & `hojichar-0.7.2/hojichar/core/composition.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.7.1/hojichar/core/filter_interface.py` & `hojichar-0.7.2/hojichar/core/filter_interface.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.7.1/hojichar/core/inspection.py` & `hojichar-0.7.2/hojichar/core/inspection.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.7.1/hojichar/core/models.py` & `hojichar-0.7.2/hojichar/core/models.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.7.1/hojichar/dict/adult_keywords_en.txt` & `hojichar-0.7.2/hojichar/dict/adult_keywords_en.txt`

 * *Files identical despite different names*

### Comparing `hojichar-0.7.1/hojichar/dict/adult_keywords_ja.txt` & `hojichar-0.7.2/hojichar/dict/adult_keywords_ja.txt`

 * *Files identical despite different names*

### Comparing `hojichar-0.7.1/hojichar/dict/discrimination_keywords_ja.txt` & `hojichar-0.7.2/hojichar/dict/discrimination_keywords_ja.txt`

 * *Files identical despite different names*

### Comparing `hojichar-0.7.1/hojichar/dict/header_footer_keywords_ja.txt` & `hojichar-0.7.2/hojichar/dict/header_footer_keywords_ja.txt`

 * *Files identical despite different names*

### Comparing `hojichar-0.7.1/hojichar/dict/violence_keywords_ja.txt` & `hojichar-0.7.2/hojichar/dict/violence_keywords_ja.txt`

 * *Files identical despite different names*

### Comparing `hojichar-0.7.1/hojichar/filters/__init__.py` & `hojichar-0.7.2/hojichar/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.7.1/hojichar/filters/deduplication.py` & `hojichar-0.7.2/hojichar/filters/deduplication.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.7.1/hojichar/filters/document_filters.py` & `hojichar-0.7.2/hojichar/filters/document_filters.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.7.1/hojichar/filters/token_filters.py` & `hojichar-0.7.2/hojichar/filters/token_filters.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.7.1/hojichar/filters/tokenization.py` & `hojichar-0.7.2/hojichar/filters/tokenization.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.7.1/hojichar/utils/__init__.py` & `hojichar-0.7.2/hojichar/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.7.1/hojichar/utils/io_iter.py` & `hojichar-0.7.2/hojichar/utils/io_iter.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.7.1/hojichar/utils/load_compose.py` & `hojichar-0.7.2/hojichar/utils/load_compose.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.7.1/hojichar/utils/process.py` & `hojichar-0.7.2/hojichar/utils/process.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.7.1/pyproject.toml` & `hojichar-0.7.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hojichar"
-version = "0.7.1"                                     # Versioning by git tag dinamically with https://github.com/mtkennerly/poetry-dynamic-versioning
+version = "0.7.2"                                     # Versioning by git tag dinamically with https://github.com/mtkennerly/poetry-dynamic-versioning
 description = "Text preprocessing management system."
 license = "Apache-2.0"
 authors = ["kenta.shinzato <hoppiece@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/HojiChar/HojiChar"
 repository = "https://github.com/HojiChar/HojiChar"
```

### Comparing `hojichar-0.7.1/PKG-INFO` & `hojichar-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hojichar
-Version: 0.7.1
+Version: 0.7.2
 Summary: Text preprocessing management system.
 Home-page: https://github.com/HojiChar/HojiChar
 License: Apache-2.0
 Author: kenta.shinzato
 Author-email: hoppiece@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

