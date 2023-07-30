# Comparing `tmp/hojichar-0.7.2.tar.gz` & `tmp/hojichar-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hojichar-0.7.2.tar", max compression
+gzip compressed data, was "hojichar-0.8.0.tar", max compression
```

## Comparing `hojichar-0.7.2.tar` & `hojichar-0.8.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    11357 2023-07-30 04:53:08.258978 hojichar-0.7.2/LICENSE
--rw-r--r--   0        0        0    14086 2023-07-30 04:53:08.258978 hojichar-0.7.2/README.md
--rw-r--r--   0        0        0      547 2023-07-30 04:53:29.338961 hojichar-0.7.2/hojichar/__init__.py
--rw-r--r--   0        0        0     4408 2023-07-30 04:53:08.258978 hojichar-0.7.2/hojichar/cli.py
--rw-r--r--   0        0        0       42 2023-07-30 04:53:08.258978 hojichar-0.7.2/hojichar/core/__init__.py
--rw-r--r--   0        0        0     5039 2023-07-30 04:53:08.258978 hojichar-0.7.2/hojichar/core/composition.py
--rw-r--r--   0        0        0     5638 2023-07-30 04:53:08.258978 hojichar-0.7.2/hojichar/core/filter_interface.py
--rw-r--r--   0        0        0     6221 2023-07-30 04:53:08.258978 hojichar-0.7.2/hojichar/core/inspection.py
--rw-r--r--   0        0        0     1087 2023-07-30 04:53:08.258978 hojichar-0.7.2/hojichar/core/models.py
--rw-r--r--   0        0        0      147 2023-07-30 04:53:08.258978 hojichar-0.7.2/hojichar/dict/__init__.py
--rw-r--r--   0        0        0      941 2023-07-30 04:53:08.258978 hojichar-0.7.2/hojichar/dict/adult_keywords_en.txt
--rw-r--r--   0        0        0    18091 2023-07-30 04:53:08.258978 hojichar-0.7.2/hojichar/dict/adult_keywords_ja.txt
--rw-r--r--   0        0        0      426 2023-07-30 04:53:08.258978 hojichar-0.7.2/hojichar/dict/advertisement_keywords_ja.txt
--rw-r--r--   0        0        0     1740 2023-07-30 04:53:08.258978 hojichar-0.7.2/hojichar/dict/discrimination_keywords_ja.txt
--rw-r--r--   0        0        0       67 2023-07-30 04:53:08.258978 hojichar-0.7.2/hojichar/dict/dummy_ng_words.txt
--rw-r--r--   0        0        0      577 2023-07-30 04:53:08.258978 hojichar-0.7.2/hojichar/dict/header_footer_keywords_ja.txt
--rw-r--r--   0        0        0      665 2023-07-30 04:53:08.258978 hojichar-0.7.2/hojichar/dict/violence_keywords_ja.txt
--rw-r--r--   0        0        0      711 2023-07-30 04:53:08.258978 hojichar-0.7.2/hojichar/filters/__init__.py
--rw-r--r--   0        0        0    12104 2023-07-30 04:53:08.258978 hojichar-0.7.2/hojichar/filters/deduplication.py
--rw-r--r--   0        0        0    23939 2023-07-30 04:53:08.258978 hojichar-0.7.2/hojichar/filters/document_filters.py
--rw-r--r--   0        0        0     1606 2023-07-30 04:53:08.258978 hojichar-0.7.2/hojichar/filters/token_filters.py
--rw-r--r--   0        0        0     2530 2023-07-30 04:53:08.258978 hojichar-0.7.2/hojichar/filters/tokenization.py
--rw-r--r--   0        0        0        0 2023-07-30 04:53:08.258978 hojichar-0.7.2/hojichar/py.typed
--rw-r--r--   0        0        0      595 2023-07-30 04:53:08.258978 hojichar-0.7.2/hojichar/utils/__init__.py
--rw-r--r--   0        0        0     1716 2023-07-30 04:53:08.258978 hojichar-0.7.2/hojichar/utils/io_iter.py
--rw-r--r--   0        0        0     3380 2023-07-30 04:53:08.258978 hojichar-0.7.2/hojichar/utils/load_compose.py
--rw-r--r--   0        0        0     1920 2023-07-30 04:53:08.258978 hojichar-0.7.2/hojichar/utils/process.py
--rw-r--r--   0        0        0     1746 2023-07-30 04:53:29.334961 hojichar-0.7.2/pyproject.toml
--rw-r--r--   0        0        0    14819 1970-01-01 00:00:00.000000 hojichar-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-30 15:25:29.668113 hojichar-0.8.0/LICENSE
+-rw-r--r--   0        0        0    14271 2023-07-30 15:25:29.668113 hojichar-0.8.0/README.md
+-rw-r--r--   0        0        0      547 2023-07-30 15:25:49.828322 hojichar-0.8.0/hojichar/__init__.py
+-rw-r--r--   0        0        0     5689 2023-07-30 15:25:29.668113 hojichar-0.8.0/hojichar/cli.py
+-rw-r--r--   0        0        0       42 2023-07-30 15:25:29.668113 hojichar-0.8.0/hojichar/core/__init__.py
+-rw-r--r--   0        0        0     5039 2023-07-30 15:25:29.668113 hojichar-0.8.0/hojichar/core/composition.py
+-rw-r--r--   0        0        0     5638 2023-07-30 15:25:29.668113 hojichar-0.8.0/hojichar/core/filter_interface.py
+-rw-r--r--   0        0        0     6221 2023-07-30 15:25:29.668113 hojichar-0.8.0/hojichar/core/inspection.py
+-rw-r--r--   0        0        0     1087 2023-07-30 15:25:29.668113 hojichar-0.8.0/hojichar/core/models.py
+-rw-r--r--   0        0        0      147 2023-07-30 15:25:29.668113 hojichar-0.8.0/hojichar/dict/__init__.py
+-rw-r--r--   0        0        0      941 2023-07-30 15:25:29.668113 hojichar-0.8.0/hojichar/dict/adult_keywords_en.txt
+-rw-r--r--   0        0        0    18091 2023-07-30 15:25:29.668113 hojichar-0.8.0/hojichar/dict/adult_keywords_ja.txt
+-rw-r--r--   0        0        0      426 2023-07-30 15:25:29.668113 hojichar-0.8.0/hojichar/dict/advertisement_keywords_ja.txt
+-rw-r--r--   0        0        0     1740 2023-07-30 15:25:29.668113 hojichar-0.8.0/hojichar/dict/discrimination_keywords_ja.txt
+-rw-r--r--   0        0        0       67 2023-07-30 15:25:29.668113 hojichar-0.8.0/hojichar/dict/dummy_ng_words.txt
+-rw-r--r--   0        0        0      577 2023-07-30 15:25:29.668113 hojichar-0.8.0/hojichar/dict/header_footer_keywords_ja.txt
+-rw-r--r--   0        0        0      665 2023-07-30 15:25:29.668113 hojichar-0.8.0/hojichar/dict/violence_keywords_ja.txt
+-rw-r--r--   0        0        0      711 2023-07-30 15:25:29.668113 hojichar-0.8.0/hojichar/filters/__init__.py
+-rw-r--r--   0        0        0    12104 2023-07-30 15:25:29.668113 hojichar-0.8.0/hojichar/filters/deduplication.py
+-rw-r--r--   0        0        0    23939 2023-07-30 15:25:29.668113 hojichar-0.8.0/hojichar/filters/document_filters.py
+-rw-r--r--   0        0        0     1606 2023-07-30 15:25:29.668113 hojichar-0.8.0/hojichar/filters/token_filters.py
+-rw-r--r--   0        0        0     2530 2023-07-30 15:25:29.668113 hojichar-0.8.0/hojichar/filters/tokenization.py
+-rw-r--r--   0        0        0        0 2023-07-30 15:25:29.668113 hojichar-0.8.0/hojichar/py.typed
+-rw-r--r--   0        0        0      595 2023-07-30 15:25:29.668113 hojichar-0.8.0/hojichar/utils/__init__.py
+-rw-r--r--   0        0        0     1716 2023-07-30 15:25:29.668113 hojichar-0.8.0/hojichar/utils/io_iter.py
+-rw-r--r--   0        0        0     3380 2023-07-30 15:25:29.668113 hojichar-0.8.0/hojichar/utils/load_compose.py
+-rw-r--r--   0        0        0     1920 2023-07-30 15:25:29.672114 hojichar-0.8.0/hojichar/utils/process.py
+-rw-r--r--   0        0        0     1788 2023-07-30 15:25:49.828322 hojichar-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0    15042 1970-01-01 00:00:00.000000 hojichar-0.8.0/PKG-INFO
```

### Comparing `hojichar-0.7.2/LICENSE` & `hojichar-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hojichar-0.7.2/README.md` & `hojichar-0.8.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -135,24 +135,26 @@
   ```bash
   cat <your_text.jsonl> | hojichar -p your_preprocessing_profile.py -o your_text_preprocessed.jsonl
   ```
 
 - `hojichar --help`
 
   ```man
-    usage: hojichar [-h] --profile <profile.py> [--args ARGS [ARGS ...]] [--output OUTPUT] [--dump-stats <path to stats.json>] [--exit-on-error] [--all] [--jobs JOBS]
+    usage: hojichar [-h] --profile <profile.py> [--args ARGS [ARGS ...]] [--output OUTPUT] [--input INPUT] [--dump-stats <path to stats.json>] [--exit-on-error] [--all] [--jobs JOBS]
 
     options:
     -h, --help            show this help message and exit
     --profile <profile.py>, -p <profile.py>
                             Path to a Python file that implements your custom filter.
-    --args ARGS [ARGS ...]E
+    --args ARGS [ARGS ...]
                             Pass additional arguments to the profile. Use it like `--args arg1 arg2` etc. The arguments should be space-separated.
     --output OUTPUT, -o OUTPUT
                             Specifies the path for the output file. Defaults to standard output.
+    --input INPUT, -i INPUT
+                            Specifies the path for the input file. Defaults to standard input. If set this path, the progress bar is enabled.
     --dump-stats <path to stats.json>
                             Dump statistics to file. If the file exists, it will be appended.
     --exit-on-error       Exit if an exception occurs during filtering. Useful for debugging custom filters.
     --all                 A flag that specifies whether to include discarded samples. This is useful when inspecting discarded samples.
     --jobs JOBS, -j JOBS  The number ob parallel jobs. By default, the nuber of the CPU core.
   ```
```

### Comparing `hojichar-0.7.2/hojichar/__init__.py` & `hojichar-0.8.0/hojichar/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 .. include:: ../README.md
 """
 from .core.composition import Compose
 from .core.filter_interface import Filter, TokenFilter
 from .core.models import Document, Token
 from .filters import deduplication, document_filters, token_filters, tokenization
 
-__version__ = "0.7.2"  # Replaced by poetry-dynamic-versioning when deploying
+__version__ = "0.8.0"  # Replaced by poetry-dynamic-versioning when deploying
 
 __all__ = [
     "core",
     "filters",
     "utils",
     "Compose",
     "Filter",
```

### Comparing `hojichar-0.7.2/hojichar/cli.py` & `hojichar-0.8.0/hojichar/cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,27 +2,44 @@
 import functools
 import json
 import logging
 import multiprocessing
 import os
 import signal
 import sys
-from typing import Dict, Iterator, Tuple
+from typing import Callable, Dict, Iterator, Optional, Tuple
+
+import tqdm
 
 import hojichar
 from hojichar.core.inspection import StatsContainer
 from hojichar.utils.io_iter import fileout_from_iter, stdin_iter, stdout_from_iter
 from hojichar.utils.load_compose import load_compose
 
 MAIN_FILTER: hojichar.Compose
 CLI_ARGS: argparse.Namespace
 
 logger = logging.getLogger("hojichar.cli")
 
 
+class ProgressBarIteratorWrapper:
+    def __init__(self, iter: Iterator[str], total_bytes: Optional[int] = None) -> None:
+        self.iter = iter
+        self.pbar = tqdm.tqdm(total=total_bytes, unit="B", unit_scale=True, unit_divisor=1024)
+
+    def __iter__(self) -> Iterator:
+        return self
+
+    def __next__(self) -> str:
+        next = self.iter.__next__()
+        delta_bytes = len(next.encode("utf-8"))
+        self.pbar.update(delta_bytes)
+        return next
+
+
 def argparser() -> argparse.Namespace:
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "--profile",
         "-p",
         required=True,
         metavar="<profile.py>",
@@ -38,14 +55,21 @@
     parser.add_argument(
         "--output",
         "-o",
         default=None,
         help="Specifies the path for the output file. Defaults to standard output.",
     )
     parser.add_argument(
+        "--input",
+        "-i",
+        default=None,
+        help="Specifies the path for the input file. Defaults to standard input.\
+            If set this path, the progress bar is enabled.",
+    )
+    parser.add_argument(
         "--dump-stats",
         default=None,
         metavar="<path to stats.json>",
         help="Dump statistics to file. If the file exists, it will be appended.",
     )
     parser.add_argument(
         "--exit-on-error",
@@ -98,39 +122,59 @@
         doc, pid, worker_stats = worker_out
         pid_stats[pid] = worker_stats
         yield doc
 
 
 def main() -> None:
     pid_stats: Dict[int, StatsContainer] = dict()
-
+    file_in = None
+    file_out = None
     args = argparser()
-    input_iter = stdin_iter()
+
+    input_iter: Iterator[str]
+    if args.input:
+        file_in = open(args.input)
+        input_iter = ProgressBarIteratorWrapper(
+            file_in,
+            total_bytes=os.path.getsize(args.input),
+        )
+    else:
+        input_iter = ProgressBarIteratorWrapper(stdin_iter())
+
+    writer: Callable[[Iterator[str]], None]
+    if args.output:
+        file_out = open(args.output, "w")
+        writer = functools.partial(fileout_from_iter, file_out)
+    else:
+        writer = stdout_from_iter
+
     input_doc_iter = (hojichar.Document(s) for s in input_iter)
     filter = load_compose(args.profile, *tuple(args.args))
     pool = multiprocessing.Pool(
         processes=args.jobs, initializer=init_worker, initargs=(filter, args)
     )
     try:
         worker_out_iter = pool.imap_unordered(worker, input_doc_iter)
         out_doc_iter = out_doc_generator(worker_out_iter, pid_stats)
         out_str_iter = (
             (doc.text for doc in out_doc_iter)
             if args.all
             else (doc.text for doc in out_doc_iter if not doc.is_rejected)
         )
-        if args.output:
-            with open(args.output, "w") as fp:
-                fileout_from_iter(out_str_iter, fp)
-        else:
-            stdout_from_iter(out_str_iter)
+        writer(out_str_iter)
+    except KeyboardInterrupt:
+        raise KeyboardInterrupt from None
     finally:
-        pool.close()
-        pool.join()
+        input_iter.pbar.close()
         pool.terminate()
+        pool.join()
+        if file_in:
+            file_in.close()
+        if file_out:
+            file_out.close()
 
     stats: StatsContainer = functools.reduce(lambda x, y: x + y, pid_stats.values())
     print(
         json.dumps(stats.get_human_readable_values(), ensure_ascii=False, indent=2),
         file=sys.stderr,
     )
     if args.dump_stats:
```

### Comparing `hojichar-0.7.2/hojichar/core/composition.py` & `hojichar-0.8.0/hojichar/core/composition.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.7.2/hojichar/core/filter_interface.py` & `hojichar-0.8.0/hojichar/core/filter_interface.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.7.2/hojichar/core/inspection.py` & `hojichar-0.8.0/hojichar/core/inspection.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.7.2/hojichar/core/models.py` & `hojichar-0.8.0/hojichar/core/models.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.7.2/hojichar/dict/adult_keywords_en.txt` & `hojichar-0.8.0/hojichar/dict/adult_keywords_en.txt`

 * *Files identical despite different names*

### Comparing `hojichar-0.7.2/hojichar/dict/adult_keywords_ja.txt` & `hojichar-0.8.0/hojichar/dict/adult_keywords_ja.txt`

 * *Files identical despite different names*

### Comparing `hojichar-0.7.2/hojichar/dict/discrimination_keywords_ja.txt` & `hojichar-0.8.0/hojichar/dict/discrimination_keywords_ja.txt`

 * *Files identical despite different names*

### Comparing `hojichar-0.7.2/hojichar/dict/header_footer_keywords_ja.txt` & `hojichar-0.8.0/hojichar/dict/header_footer_keywords_ja.txt`

 * *Files identical despite different names*

### Comparing `hojichar-0.7.2/hojichar/dict/violence_keywords_ja.txt` & `hojichar-0.8.0/hojichar/dict/violence_keywords_ja.txt`

 * *Files identical despite different names*

### Comparing `hojichar-0.7.2/hojichar/filters/__init__.py` & `hojichar-0.8.0/hojichar/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.7.2/hojichar/filters/deduplication.py` & `hojichar-0.8.0/hojichar/filters/deduplication.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.7.2/hojichar/filters/document_filters.py` & `hojichar-0.8.0/hojichar/filters/document_filters.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.7.2/hojichar/filters/token_filters.py` & `hojichar-0.8.0/hojichar/filters/token_filters.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.7.2/hojichar/filters/tokenization.py` & `hojichar-0.8.0/hojichar/filters/tokenization.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.7.2/hojichar/utils/__init__.py` & `hojichar-0.8.0/hojichar/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.7.2/hojichar/utils/io_iter.py` & `hojichar-0.8.0/hojichar/utils/io_iter.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,10 +47,10 @@
     try:
         for line in iter:
             stdout.write(line + "\n")
     except BrokenPipeError:
         sys.exit(1)
 
 
-def fileout_from_iter(iter: Iterator[str], fp: TextIO) -> None:
+def fileout_from_iter(fp: TextIO, iter: Iterator[str]) -> None:
     for line in iter:
         fp.write(line + "\n")
```

### Comparing `hojichar-0.7.2/hojichar/utils/load_compose.py` & `hojichar-0.8.0/hojichar/utils/load_compose.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.7.2/hojichar/utils/process.py` & `hojichar-0.8.0/hojichar/utils/process.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.7.2/pyproject.toml` & `hojichar-0.8.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "hojichar"
-version = "0.7.2"                                     # Versioning by git tag dinamically with https://github.com/mtkennerly/poetry-dynamic-versioning
+version = "0.8.0"                                     # Versioning by git tag dinamically with https://github.com/mtkennerly/poetry-dynamic-versioning
 description = "Text preprocessing management system."
 license = "Apache-2.0"
 authors = ["kenta.shinzato <hoppiece@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/HojiChar/HojiChar"
 repository = "https://github.com/HojiChar/HojiChar"
 
 [tool.poetry.scripts]
 hojichar = "hojichar.cli:main"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 numpy = ">=1.17.0"
 mmh3 = "^4.0"
+tqdm = "^4.65.0"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.lint]
 optional = true
 
@@ -26,14 +27,15 @@
 optional = true
 
 [tool.poetry.group.lint.dependencies]
 black = "^22.3.0"
 flake8 = "^4.0.1"
 isort = "^5.10.1"
 mypy = "^1.0"
+types-tqdm = "^4.65.0.2"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.1.2"
 pytest-cov = "^4.0.0"
 
 [tool.poetry.group.dev.dependencies]
 taskipy = "^1.10.3"
```

### Comparing `hojichar-0.7.2/PKG-INFO` & `hojichar-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: hojichar
-Version: 0.7.2
+Version: 0.8.0
 Summary: Text preprocessing management system.
 Home-page: https://github.com/HojiChar/HojiChar
 License: Apache-2.0
 Author: kenta.shinzato
 Author-email: hoppiece@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: mmh3 (>=4.0,<5.0)
 Requires-Dist: numpy (>=1.17.0)
+Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Project-URL: Repository, https://github.com/HojiChar/HojiChar
 Description-Content-Type: text/markdown
 
 # HojiChar
 
 [![PyPI version](https://badge.fury.io/py/hojichar.svg)](https://badge.fury.io/py/hojichar)
 [![Python Versions](https://img.shields.io/pypi/pyversions/hojichar.svg)](https://pypi.org/project/hojichar/)
@@ -155,24 +156,26 @@
   ```bash
   cat <your_text.jsonl> | hojichar -p your_preprocessing_profile.py -o your_text_preprocessed.jsonl
   ```
 
 - `hojichar --help`
 
   ```man
-    usage: hojichar [-h] --profile <profile.py> [--args ARGS [ARGS ...]] [--output OUTPUT] [--dump-stats <path to stats.json>] [--exit-on-error] [--all] [--jobs JOBS]
+    usage: hojichar [-h] --profile <profile.py> [--args ARGS [ARGS ...]] [--output OUTPUT] [--input INPUT] [--dump-stats <path to stats.json>] [--exit-on-error] [--all] [--jobs JOBS]
 
     options:
     -h, --help            show this help message and exit
     --profile <profile.py>, -p <profile.py>
                             Path to a Python file that implements your custom filter.
-    --args ARGS [ARGS ...]E
+    --args ARGS [ARGS ...]
                             Pass additional arguments to the profile. Use it like `--args arg1 arg2` etc. The arguments should be space-separated.
     --output OUTPUT, -o OUTPUT
                             Specifies the path for the output file. Defaults to standard output.
+    --input INPUT, -i INPUT
+                            Specifies the path for the input file. Defaults to standard input. If set this path, the progress bar is enabled.
     --dump-stats <path to stats.json>
                             Dump statistics to file. If the file exists, it will be appended.
     --exit-on-error       Exit if an exception occurs during filtering. Useful for debugging custom filters.
     --all                 A flag that specifies whether to include discarded samples. This is useful when inspecting discarded samples.
     --jobs JOBS, -j JOBS  The number ob parallel jobs. By default, the nuber of the CPU core.
   ```
```

