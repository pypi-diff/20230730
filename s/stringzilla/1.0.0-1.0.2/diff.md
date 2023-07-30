# Comparing `tmp/stringzilla-1.0.0-cp39-cp39-win_amd64.whl.zip` & `tmp/stringzilla-1.0.2-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 99259 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat   244224 b- defN 23-Jul-13 17:25 stringzilla.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     4564 b- defN 23-Jul-13 17:26 stringzilla-1.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Jul-13 17:26 stringzilla-1.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 23-Jul-13 17:26 stringzilla-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      404 b- defN 23-Jul-13 17:26 stringzilla-1.0.0.dist-info/RECORD
-5 files, 249304 bytes uncompressed, 98509 bytes compressed:  60.5%
+Zip file size: 103124 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat   256000 b- defN 23-Jul-30 18:34 stringzilla.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     4573 b- defN 23-Jul-30 18:34 stringzilla-1.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Jul-30 18:34 stringzilla-1.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 23-Jul-30 18:34 stringzilla-1.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      404 b- defN 23-Jul-30 18:34 stringzilla-1.0.2.dist-info/RECORD
+5 files, 261089 bytes uncompressed, 102374 bytes compressed:  60.8%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: stringzilla.cp39-win_amd64.pyd
 Comment: 
 
-Filename: stringzilla-1.0.0.dist-info/METADATA
+Filename: stringzilla-1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: stringzilla-1.0.0.dist-info/WHEEL
+Filename: stringzilla-1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: stringzilla-1.0.0.dist-info/top_level.txt
+Filename: stringzilla-1.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: stringzilla-1.0.0.dist-info/RECORD
+Filename: stringzilla-1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `stringzilla-1.0.0.dist-info/METADATA` & `stringzilla-1.0.2.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stringzilla
-Version: 1.0.0
+Version: 1.0.2
 Summary: Crunch 100+ GB Strings in Python with ease
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
@@ -18,21 +18,21 @@
 Classifier: Topic :: Internet :: Log Analysis
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: System :: Logging
 Classifier: Topic :: Text Processing :: General
 Classifier: Topic :: Text Processing :: Indexing
 Description-Content-Type: text/markdown
 
-# Stringzilla
+# Stringzilla 🦖
 
 ## Crunch 100+ GB Strings in Python with ease, leveraging SIMD Assembly
 
 Stringzilla was born many years ago as a [tutorial for SIMD accelerated string-processing][tutorial].
-But one day, processing 100+ GB Chemistry and AI datasets, I decided to transform it into a library.
-It's designed to replace `open(...).readlines()`, `str().splitlines()` and many other common workloads with very long strings.
+But one day, processing 100+ GB of Chemistry and AI datasets, I transformed it into a library.
+It's designed to replace `open(...).readlines()`, `str().splitlines()`, and many other typical workloads with very long strings.
 
 <table>
 <tr>
 <td>
 
 <table>
 <thead>
@@ -76,25 +76,25 @@
 
 ## Usage
 
 ```sh
 pip install stringzilla
 ```
 
-There are two classes you can use interchangibly:
+There are two classes you can use interchangeably:
 
 ```python
 from stringzilla import Str, File, Strs
 
 text: str = 'some-string'
 text: Str = Str('some-string')
 text: File = File('some-file.txt')
 ```
 
-Once constructed, following interfaces are supported:
+Once constructed, the following interfaces are supported:
 
 ```python
 len(text) -> int
 'substring' in text -> bool
 text[42] -> str
 
 text.contains(
@@ -135,33 +135,33 @@
 
 ```sh
 rm -rf build && pip install -e . && pytest scripts/test.py -s -x
 
 pip install -e . --no-index --no-deps
 ```
 
-To benchmark on some custom file and pattern combination:
+To benchmark on some custom file and pattern combinations:
 
 ```sh
 python scripts/bench.py --haystack_path "your file" --needle "your pattern"
 ```
 
-To benchmark on syntetic data:
+To benchmark on synthetic data:
 
 ```sh
 python scripts/bench.py --haystack_pattern "abcd" --haystack_length 1e9 --needle "abce"
 ```
 
 To validate packaging:
 
 ```sh
 cibuildwheel --platform linux
 ```
 
-Compilin C++ tests:
+Compiling C++ tests:
 
 
 ```sh
 brew install libomp llvm
 cmake -B ./build_release \
     -DCMAKE_C_COMPILER="/opt/homebrew/opt/llvm/bin/clang" \
     -DCMAKE_CXX_COMPILER="/opt/homebrew/opt/llvm/bin/clang++" \
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

