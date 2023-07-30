# Comparing `tmp/mattress-0.0.4.tar.gz` & `tmp/mattress-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mattress-0.0.4.tar", last modified: Thu Jul 27 16:56:30 2023, max compression
+gzip compressed data, was "mattress-0.0.5.tar", last modified: Sun Jul 30 01:10:35 2023, max compression
```

## Comparing `mattress-0.0.4.tar` & `mattress-0.0.5.tar`

### file list

```diff
@@ -1,236 +1,238 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.419239 mattress-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-27 16:56:16.000000 mattress-0.0.4/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.367239 mattress-0.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.383239 mattress-0.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-07-27 16:56:16.000000 mattress-0.0.4/.github/workflows/pypi-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-27 16:56:16.000000 mattress-0.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-27 16:56:16.000000 mattress-0.0.4/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-27 16:56:16.000000 mattress-0.0.4/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-27 16:56:16.000000 mattress-0.0.4/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-27 16:56:16.000000 mattress-0.0.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    13490 2023-07-27 16:56:16.000000 mattress-0.0.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-27 16:56:16.000000 mattress-0.0.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-27 16:56:16.000000 mattress-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-07-27 16:56:30.419239 mattress-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-07-27 16:56:16.000000 mattress-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.387239 mattress-0.0.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-27 16:56:16.000000 mattress-0.0.4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.387239 mattress-0.0.4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-27 16:56:16.000000 mattress-0.0.4/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-27 16:56:16.000000 mattress-0.0.4/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-27 16:56:16.000000 mattress-0.0.4/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)    10034 2023-07-27 16:56:16.000000 mattress-0.0.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-27 16:56:16.000000 mattress-0.0.4/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-27 16:56:16.000000 mattress-0.0.4/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-27 16:56:16.000000 mattress-0.0.4/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-27 16:56:16.000000 mattress-0.0.4/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-27 16:56:16.000000 mattress-0.0.4/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-27 16:56:16.000000 mattress-0.0.4/docs/tutorial
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-27 16:56:16.000000 mattress-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-27 16:56:30.419239 mattress-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-07-27 16:56:16.000000 mattress-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.371239 mattress-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.387239 mattress-0.0.4/src/mattress/
--rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-07-27 16:56:16.000000 mattress-0.0.4/src/mattress/TatamiNumericPointer.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-27 16:56:16.000000 mattress-0.0.4/src/mattress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-27 16:56:16.000000 mattress-0.0.4/src/mattress/cpphelpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.375239 mattress-0.0.4/src/mattress/extern/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.391239 mattress-0.0.4/src/mattress/extern/tatami/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-27 16:56:17.000000 mattress-0.0.4/src/mattress/extern/tatami/.git
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.371239 mattress-0.0.4/src/mattress/extern/tatami/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.391239 mattress-0.0.4/src/mattress/extern/tatami/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/.github/workflows/doxygenate.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/.github/workflows/run-gallery.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/.github/workflows/run-tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16110 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.391239 mattress-0.0.4/src/mattress/extern/tatami/docs/
--rw-r--r--   0 runner    (1001) docker     (123)   108951 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/docs/Doxyfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.391239 mattress-0.0.4/src/mattress/extern/tatami/gallery/
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/gallery/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/gallery/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.395239 mattress-0.0.4/src/mattress/extern/tatami/gallery/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/gallery/src/char2double.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/gallery/src/colsums.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/gallery/src/parallel.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/gallery/src/print_vector.h
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/gallery/src/read_h5.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/gallery/src/read_mm.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/gallery/src/sparse_extractor.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.375239 mattress-0.0.4/src/mattress/extern/tatami/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.395239 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.395239 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/base/
--rw-r--r--   0 runner    (1001) docker     (123)    13617 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/base/Extractor.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    14493 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/base/Matrix.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/base/Options.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/base/SparseRange.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/base/utils.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.399239 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/dense/
--rw-r--r--   0 runner    (1001) docker     (123)     9421 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/dense/DenseMatrix.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/dense/VirtualDenseMatrix.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.399239 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/isometric/
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/isometric/arith_utils.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.399239 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/isometric/binary/
--rw-r--r--   0 runner    (1001) docker     (123)    23796 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/isometric/binary/DelayedBinaryIsometricOp.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/isometric/binary/arith_helpers.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/isometric/binary/boolean_helpers.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/isometric/binary/compare_helpers.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/isometric/binary/utils.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/isometric/boolean_utils.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/isometric/compare_utils.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.403239 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/isometric/unary/
--rw-r--r--   0 runner    (1001) docker     (123)    31440 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/isometric/unary/DelayedUnaryIsometricOp.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    17594 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/isometric/unary/arith_helpers.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10874 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/isometric/unary/boolean_helpers.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    12346 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/isometric/unary/compare_helpers.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    27534 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/isometric/unary/math_helpers.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.403239 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/other/
--rw-r--r--   0 runner    (1001) docker     (123)    29155 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/other/DelayedBind.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    14885 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/other/DelayedCast.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/other/DelayedTranspose.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.403239 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/sparse/
--rw-r--r--   0 runner    (1001) docker     (123)    27660 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/sparse/CompressedSparseMatrix.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    27659 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/sparse/FragmentedSparseMatrix.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    31574 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/sparse/SemiCompressedSparseMatrix.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    16913 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/sparse/SparseSecondaryExtractorCore.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    14977 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/sparse/convert_to_compressed_sparse.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10037 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/sparse/convert_to_fragmented_sparse.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6562 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/sparse/primary_extraction.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/sparse/utils.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.407239 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/stats/
--rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/stats/medians.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10646 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/stats/ranges.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/stats/sums.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/stats/utils.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    14018 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/stats/variances.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.407239 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/subset/
--rw-r--r--   0 runner    (1001) docker     (123)    26535 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/subset/DelayedSubset.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    14616 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/subset/DelayedSubsetBlock.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    22752 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/subset/DelayedSubsetSorted.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11177 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/subset/DelayedSubsetSortedUnique.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    23308 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/subset/DelayedSubsetUnique.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/subset/make_DelayedSubset.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/subset/utils.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/tatami.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.411239 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/utils/ArrayView.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/utils/Oracles.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    13509 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/utils/SomeNumericArray.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/utils/bind_intersection.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5308 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/utils/compress_sparse_triplets.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/utils/convert_to_dense.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/utils/convert_to_sparse.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/utils/process_consecutive_indices.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/utils/wrap_shared_ptr.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.411239 mattress-0.0.4/src/mattress/extern/tatami/include/tatami_test/
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami_test/simulate_vector.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami_test/tatami_test.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami_test/temp_file_path.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami_test/test_access_base.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami_test/test_column_access.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami_test/test_oracle_access.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami_test/test_row_access.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami_test/utils.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.411239 mattress-0.0.4/src/mattress/extern/tatami/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.375239 mattress-0.0.4/src/mattress/extern/tatami/tests/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.411239 mattress-0.0.4/src/mattress/extern/tatami/tests/src/dense/
--rw-r--r--   0 runner    (1001) docker     (123)    10227 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/dense/DenseMatrix.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.411239 mattress-0.0.4/src/mattress/extern/tatami/tests/src/isometric/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.411239 mattress-0.0.4/src/mattress/extern/tatami/tests/src/isometric/binary/
--rw-r--r--   0 runner    (1001) docker     (123)    42584 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/isometric/binary/arith_helpers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/isometric/binary/boolean_helpers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6844 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/isometric/binary/compare_helpers.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.411239 mattress-0.0.4/src/mattress/extern/tatami/tests/src/isometric/unary/
--rw-r--r--   0 runner    (1001) docker     (123)    12095 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/isometric/unary/arith_scalar_helpers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    62084 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/isometric/unary/arith_vector_helpers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/isometric/unary/boolean_scalar_helpers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7250 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/isometric/unary/boolean_vector_helpers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6952 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/isometric/unary/compare_scalar_helpers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11093 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/isometric/unary/compare_vector_helpers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    30151 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/isometric/unary/math_helpers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/isometric/utils.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.411239 mattress-0.0.4/src/mattress/extern/tatami/tests/src/other/
--rw-r--r--   0 runner    (1001) docker     (123)    14777 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/other/DelayedBind.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    13865 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/other/DelayedCast.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7648 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/other/DelayedTranspose.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.415239 mattress-0.0.4/src/mattress/extern/tatami/tests/src/sparse/
--rw-r--r--   0 runner    (1001) docker     (123)    11288 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/sparse/CompressedSparseMatrix.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11020 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/sparse/FragmentedSparseMatrix.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9890 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/sparse/SemiCompressedSparseMatrix.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    21117 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/sparse/SparseSecondaryExtractorCore.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7623 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/sparse/convert_to_compressed_sparse.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7057 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/sparse/convert_to_fragmented_sparse.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.415239 mattress-0.0.4/src/mattress/extern/tatami/tests/src/stats/
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/stats/custom_parallel.h
--rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/stats/medians.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/stats/parallelize.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/stats/ranges.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/stats/sums.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7562 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/stats/variances.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.415239 mattress-0.0.4/src/mattress/extern/tatami/tests/src/subset/
--rw-r--r--   0 runner    (1001) docker     (123)    21245 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/subset/DelayedSubset.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11363 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/subset/DelayedSubsetBlock.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.415239 mattress-0.0.4/src/mattress/extern/tatami/tests/src/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/utils/ArrayView.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/utils/Oracles.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/utils/SomeNumericArray.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8700 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/utils/bind_intersection.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/utils/compress_sparse_triplets.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7358 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/utils/convert_to_dense.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/utils/process_consecutive_indices.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/utils/wrap_shared_ptr.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.415239 mattress-0.0.4/src/mattress/extern/tatami_hdf5/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 16:56:17.000000 mattress-0.0.4/src/mattress/extern/tatami_hdf5/.git
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.379239 mattress-0.0.4/src/mattress/extern/tatami_hdf5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.415239 mattress-0.0.4/src/mattress/extern/tatami_hdf5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami_hdf5/.github/workflows/doxygenate.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami_hdf5/.github/workflows/run-tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami_hdf5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami_hdf5/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami_hdf5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami_hdf5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.415239 mattress-0.0.4/src/mattress/extern/tatami_hdf5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)   108708 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami_hdf5/docs/Doxyfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.415239 mattress-0.0.4/src/mattress/extern/tatami_hdf5/extern/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami_hdf5/extern/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.379239 mattress-0.0.4/src/mattress/extern/tatami_hdf5/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.415239 mattress-0.0.4/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/
--rw-r--r--   0 runner    (1001) docker     (123)    48131 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/Hdf5CompressedSparseMatrix.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    20984 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/Hdf5DenseMatrix.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/load_hdf5_matrix.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/tatami_hdf5.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/utils.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    12750 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/write_sparse_matrix_to_hdf5.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.415239 mattress-0.0.4/src/mattress/extern/tatami_hdf5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami_hdf5/tests/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.419239 mattress-0.0.4/src/mattress/extern/tatami_hdf5/tests/src/
--rw-r--r--   0 runner    (1001) docker     (123)    22267 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami_hdf5/tests/src/Hdf5CompressedSparseMatrix.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    17105 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami_hdf5/tests/src/Hdf5DenseMatrix.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami_hdf5/tests/src/custom_parallel.h
--rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami_hdf5/tests/src/load_hdf5_matrix.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    14427 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami_hdf5/tests/src/write_sparse_matrix_to_hdf5.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.419239 mattress-0.0.4/src/mattress/include/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-27 16:56:16.000000 mattress-0.0.4/src/mattress/include/Mattress.h
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-07-27 16:56:16.000000 mattress-0.0.4/src/mattress/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.419239 mattress-0.0.4/src/mattress/lib/
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-27 16:56:16.000000 mattress-0.0.4/src/mattress/lib/common.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-07-27 16:56:16.000000 mattress-0.0.4/src/mattress/lib/compressed_sparse.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-07-27 16:56:16.000000 mattress-0.0.4/src/mattress/lib/dense.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-27 16:56:16.000000 mattress-0.0.4/src/mattress/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-27 16:56:16.000000 mattress-0.0.4/src/mattress/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.391239 mattress-0.0.4/src/mattress.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-07-27 16:56:30.000000 mattress-0.0.4/src/mattress.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9900 2023-07-27 16:56:30.000000 mattress-0.0.4/src/mattress.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 16:56:30.000000 mattress-0.0.4/src/mattress.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 16:56:30.000000 mattress-0.0.4/src/mattress.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-27 16:56:30.000000 mattress-0.0.4/src/mattress.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-27 16:56:30.000000 mattress-0.0.4/src/mattress.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.419239 mattress-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-27 16:56:16.000000 mattress-0.0.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-27 16:56:16.000000 mattress-0.0.4/tests/test_dense.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-27 16:56:16.000000 mattress-0.0.4/tests/test_sparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-07-27 16:56:16.000000 mattress-0.0.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:10:35.831646 mattress-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-30 01:10:17.000000 mattress-0.0.5/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:10:35.803646 mattress-0.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:10:35.815646 mattress-0.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-07-30 01:10:17.000000 mattress-0.0.5/.github/workflows/pypi-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-30 01:10:17.000000 mattress-0.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-30 01:10:17.000000 mattress-0.0.5/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-30 01:10:17.000000 mattress-0.0.5/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-30 01:10:17.000000 mattress-0.0.5/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-30 01:10:17.000000 mattress-0.0.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13490 2023-07-30 01:10:17.000000 mattress-0.0.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-30 01:10:17.000000 mattress-0.0.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-30 01:10:17.000000 mattress-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-07-30 01:10:35.831646 mattress-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-07-30 01:10:17.000000 mattress-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:10:35.815646 mattress-0.0.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-30 01:10:17.000000 mattress-0.0.5/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:10:35.815646 mattress-0.0.5/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-30 01:10:17.000000 mattress-0.0.5/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-30 01:10:17.000000 mattress-0.0.5/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-30 01:10:17.000000 mattress-0.0.5/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10034 2023-07-30 01:10:17.000000 mattress-0.0.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-30 01:10:17.000000 mattress-0.0.5/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-30 01:10:17.000000 mattress-0.0.5/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-30 01:10:17.000000 mattress-0.0.5/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-30 01:10:17.000000 mattress-0.0.5/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-30 01:10:17.000000 mattress-0.0.5/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-30 01:10:17.000000 mattress-0.0.5/docs/tutorial
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-30 01:10:17.000000 mattress-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-30 01:10:35.831646 mattress-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-07-30 01:10:17.000000 mattress-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:10:35.807646 mattress-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:10:35.815646 mattress-0.0.5/src/mattress/
+-rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-07-30 01:10:17.000000 mattress-0.0.5/src/mattress/TatamiNumericPointer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-30 01:10:17.000000 mattress-0.0.5/src/mattress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-07-30 01:10:17.000000 mattress-0.0.5/src/mattress/cpphelpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:10:35.811646 mattress-0.0.5/src/mattress/extern/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:10:35.815646 mattress-0.0.5/src/mattress/extern/tatami/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-30 01:10:17.000000 mattress-0.0.5/src/mattress/extern/tatami/.git
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:10:35.807646 mattress-0.0.5/src/mattress/extern/tatami/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:10:35.815646 mattress-0.0.5/src/mattress/extern/tatami/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/.github/workflows/doxygenate.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/.github/workflows/run-gallery.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/.github/workflows/run-tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16110 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:10:35.815646 mattress-0.0.5/src/mattress/extern/tatami/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)   108951 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/docs/Doxyfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:10:35.815646 mattress-0.0.5/src/mattress/extern/tatami/gallery/
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/gallery/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/gallery/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:10:35.819646 mattress-0.0.5/src/mattress/extern/tatami/gallery/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/gallery/src/char2double.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/gallery/src/colsums.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/gallery/src/parallel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/gallery/src/print_vector.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/gallery/src/read_h5.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/gallery/src/read_mm.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/gallery/src/sparse_extractor.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:10:35.811646 mattress-0.0.5/src/mattress/extern/tatami/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:10:35.819646 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:10:35.819646 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/base/
+-rw-r--r--   0 runner    (1001) docker     (123)    13617 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/base/Extractor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14493 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/base/Matrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/base/Options.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/base/SparseRange.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/base/utils.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:10:35.819646 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/dense/
+-rw-r--r--   0 runner    (1001) docker     (123)     9421 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/dense/DenseMatrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/dense/VirtualDenseMatrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/dense/convert_to_dense.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:10:35.819646 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/isometric/
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/isometric/arith_utils.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:10:35.819646 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/isometric/binary/
+-rw-r--r--   0 runner    (1001) docker     (123)    23796 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/isometric/binary/DelayedBinaryIsometricOp.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/isometric/binary/arith_helpers.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/isometric/binary/boolean_helpers.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/isometric/binary/compare_helpers.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/isometric/binary/utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/isometric/boolean_utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/isometric/compare_utils.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:10:35.819646 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/isometric/unary/
+-rw-r--r--   0 runner    (1001) docker     (123)    31440 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/isometric/unary/DelayedUnaryIsometricOp.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17594 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/isometric/unary/arith_helpers.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10874 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/isometric/unary/boolean_helpers.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12346 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/isometric/unary/compare_helpers.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    27534 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/isometric/unary/math_helpers.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:10:35.819646 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/other/
+-rw-r--r--   0 runner    (1001) docker     (123)    29155 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/other/DelayedBind.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14885 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/other/DelayedCast.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/other/DelayedTranspose.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:10:35.819646 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/sparse/
+-rw-r--r--   0 runner    (1001) docker     (123)    27711 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/sparse/CompressedSparseMatrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    27710 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/sparse/FragmentedSparseMatrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    31620 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/sparse/SemiCompressedSparseMatrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16795 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/sparse/SparseSecondaryExtractorCore.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14977 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/sparse/convert_to_compressed_sparse.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10037 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/sparse/convert_to_fragmented_sparse.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/sparse/primary_extraction.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/sparse/utils.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:10:35.823646 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/stats/medians.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10646 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/stats/ranges.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/stats/sums.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/stats/utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14018 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/stats/variances.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:10:35.823646 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/subset/
+-rw-r--r--   0 runner    (1001) docker     (123)    26535 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/subset/DelayedSubset.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14663 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/subset/DelayedSubsetBlock.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    22752 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/subset/DelayedSubsetSorted.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11177 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/subset/DelayedSubsetSortedUnique.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    23308 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/subset/DelayedSubsetUnique.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/subset/make_DelayedSubset.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/subset/utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/tatami.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:10:35.823646 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/utils/ArrayView.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/utils/ElementType.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/utils/Oracles.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13509 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/utils/SomeNumericArray.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/utils/bind_intersection.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5308 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/utils/compress_sparse_triplets.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/utils/convert_to_dense.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/utils/convert_to_sparse.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/utils/process_consecutive_indices.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/include/tatami/utils/wrap_shared_ptr.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:10:35.823646 mattress-0.0.5/src/mattress/extern/tatami/include/tatami_test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/include/tatami_test/simulate_vector.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/include/tatami_test/tatami_test.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/include/tatami_test/temp_file_path.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/include/tatami_test/test_access_base.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/include/tatami_test/test_column_access.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/include/tatami_test/test_oracle_access.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/include/tatami_test/test_row_access.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/include/tatami_test/utils.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:10:35.823646 mattress-0.0.5/src/mattress/extern/tatami/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/tests/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/tests/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:10:35.811646 mattress-0.0.5/src/mattress/extern/tatami/tests/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:10:35.823646 mattress-0.0.5/src/mattress/extern/tatami/tests/src/dense/
+-rw-r--r--   0 runner    (1001) docker     (123)    10227 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/tests/src/dense/DenseMatrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8652 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/tests/src/dense/convert_to_dense.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:10:35.823646 mattress-0.0.5/src/mattress/extern/tatami/tests/src/isometric/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:10:35.823646 mattress-0.0.5/src/mattress/extern/tatami/tests/src/isometric/binary/
+-rw-r--r--   0 runner    (1001) docker     (123)    42584 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/tests/src/isometric/binary/arith_helpers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/tests/src/isometric/binary/boolean_helpers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6844 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/tests/src/isometric/binary/compare_helpers.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:10:35.827646 mattress-0.0.5/src/mattress/extern/tatami/tests/src/isometric/unary/
+-rw-r--r--   0 runner    (1001) docker     (123)    12095 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/tests/src/isometric/unary/arith_scalar_helpers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    62084 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/tests/src/isometric/unary/arith_vector_helpers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/tests/src/isometric/unary/boolean_scalar_helpers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7250 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/tests/src/isometric/unary/boolean_vector_helpers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6952 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/tests/src/isometric/unary/compare_scalar_helpers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11093 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/tests/src/isometric/unary/compare_vector_helpers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    30151 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/tests/src/isometric/unary/math_helpers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/tests/src/isometric/utils.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:10:35.827646 mattress-0.0.5/src/mattress/extern/tatami/tests/src/other/
+-rw-r--r--   0 runner    (1001) docker     (123)    14777 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/tests/src/other/DelayedBind.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13865 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/tests/src/other/DelayedCast.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7648 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/tests/src/other/DelayedTranspose.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:10:35.827646 mattress-0.0.5/src/mattress/extern/tatami/tests/src/sparse/
+-rw-r--r--   0 runner    (1001) docker     (123)    11672 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/tests/src/sparse/CompressedSparseMatrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11020 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/tests/src/sparse/FragmentedSparseMatrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9890 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/tests/src/sparse/SemiCompressedSparseMatrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    21117 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/tests/src/sparse/SparseSecondaryExtractorCore.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7623 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/tests/src/sparse/convert_to_compressed_sparse.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7057 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/tests/src/sparse/convert_to_fragmented_sparse.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:10:35.827646 mattress-0.0.5/src/mattress/extern/tatami/tests/src/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/tests/src/stats/custom_parallel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/tests/src/stats/medians.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/tests/src/stats/parallelize.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/tests/src/stats/ranges.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/tests/src/stats/sums.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7562 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/tests/src/stats/variances.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:10:35.827646 mattress-0.0.5/src/mattress/extern/tatami/tests/src/subset/
+-rw-r--r--   0 runner    (1001) docker     (123)    21245 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/tests/src/subset/DelayedSubset.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12504 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/tests/src/subset/DelayedSubsetBlock.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:10:35.827646 mattress-0.0.5/src/mattress/extern/tatami/tests/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/tests/src/utils/ArrayView.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/tests/src/utils/Oracles.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/tests/src/utils/SomeNumericArray.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8700 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/tests/src/utils/bind_intersection.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/tests/src/utils/compress_sparse_triplets.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/tests/src/utils/process_consecutive_indices.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami/tests/src/utils/wrap_shared_ptr.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:10:35.827646 mattress-0.0.5/src/mattress/extern/tatami_hdf5/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami_hdf5/.git
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:10:35.811646 mattress-0.0.5/src/mattress/extern/tatami_hdf5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:10:35.827646 mattress-0.0.5/src/mattress/extern/tatami_hdf5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami_hdf5/.github/workflows/doxygenate.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami_hdf5/.github/workflows/run-tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami_hdf5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami_hdf5/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami_hdf5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami_hdf5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:10:35.831646 mattress-0.0.5/src/mattress/extern/tatami_hdf5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)   108708 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami_hdf5/docs/Doxyfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:10:35.831646 mattress-0.0.5/src/mattress/extern/tatami_hdf5/extern/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami_hdf5/extern/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:10:35.811646 mattress-0.0.5/src/mattress/extern/tatami_hdf5/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:10:35.831646 mattress-0.0.5/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/
+-rw-r--r--   0 runner    (1001) docker     (123)    48131 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/Hdf5CompressedSparseMatrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    20984 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/Hdf5DenseMatrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/load_hdf5_matrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/tatami_hdf5.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12750 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/write_sparse_matrix_to_hdf5.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:10:35.831646 mattress-0.0.5/src/mattress/extern/tatami_hdf5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami_hdf5/tests/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:10:35.831646 mattress-0.0.5/src/mattress/extern/tatami_hdf5/tests/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    22267 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami_hdf5/tests/src/Hdf5CompressedSparseMatrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17105 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami_hdf5/tests/src/Hdf5DenseMatrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami_hdf5/tests/src/custom_parallel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami_hdf5/tests/src/load_hdf5_matrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14427 2023-07-30 01:10:18.000000 mattress-0.0.5/src/mattress/extern/tatami_hdf5/tests/src/write_sparse_matrix_to_hdf5.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:10:35.831646 mattress-0.0.5/src/mattress/include/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-30 01:10:17.000000 mattress-0.0.5/src/mattress/include/Mattress.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-07-30 01:10:17.000000 mattress-0.0.5/src/mattress/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:10:35.831646 mattress-0.0.5/src/mattress/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-30 01:10:17.000000 mattress-0.0.5/src/mattress/lib/common.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-07-30 01:10:17.000000 mattress-0.0.5/src/mattress/lib/compressed_sparse.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-07-30 01:10:17.000000 mattress-0.0.5/src/mattress/lib/dense.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-30 01:10:17.000000 mattress-0.0.5/src/mattress/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-30 01:10:17.000000 mattress-0.0.5/src/mattress/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:10:35.815646 mattress-0.0.5/src/mattress.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-07-30 01:10:35.000000 mattress-0.0.5/src/mattress.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10033 2023-07-30 01:10:35.000000 mattress-0.0.5/src/mattress.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 01:10:35.000000 mattress-0.0.5/src/mattress.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 01:10:35.000000 mattress-0.0.5/src/mattress.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-30 01:10:35.000000 mattress-0.0.5/src/mattress.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-30 01:10:35.000000 mattress-0.0.5/src/mattress.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:10:35.831646 mattress-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-30 01:10:17.000000 mattress-0.0.5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-30 01:10:17.000000 mattress-0.0.5/tests/test_dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-30 01:10:17.000000 mattress-0.0.5/tests/test_sparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-07-30 01:10:17.000000 mattress-0.0.5/tox.ini
```

### Comparing `mattress-0.0.4/.coveragerc` & `mattress-0.0.5/.coveragerc`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/.github/workflows/pypi-test.yml` & `mattress-0.0.5/.github/workflows/pypi-test.yml`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/.gitignore` & `mattress-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/.readthedocs.yml` & `mattress-0.0.5/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/CONTRIBUTING.md` & `mattress-0.0.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/LICENSE.txt` & `mattress-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/PKG-INFO` & `mattress-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mattress
-Version: 0.0.4
+Version: 0.0.5
 Summary: all your matrix representations belong here!
 Home-page: https://github.com/biocpy/mattress
 Author: "Jayaram Kancherla, Aaron Lun"
 Author-email: jayaram.kancherla@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/biocpy/mattress
 Platform: any
```

### Comparing `mattress-0.0.4/README.md` & `mattress-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/docs/Makefile` & `mattress-0.0.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/docs/conf.py` & `mattress-0.0.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/docs/index.md` & `mattress-0.0.5/docs/index.md`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/docs/tutorial` & `mattress-0.0.5/docs/tutorial`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/setup.cfg` & `mattress-0.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/setup.py` & `mattress-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/TatamiNumericPointer.py` & `mattress-0.0.5/src/mattress/TatamiNumericPointer.py`

 * *Files 12% similar despite different names*

```diff
@@ -88,17 +88,31 @@
         Returns:
             TatamiNumericPointer: instance of the class.
         """
 
         if len(x.shape) != 2:
             raise ValueError("'x' should be a 2-dimensional array")
 
+        byrow = None
+        if x.flags["C_CONTIGUOUS"]:
+            byrow = True
+        elif x.flags["F_CONTIGUOUS"]:
+            byrow = False
+        else:
+            # I don't think it's possible to hit this, as a (non-view) ndarray
+            # should be contiguous in at least one direction.
+            raise ValueError("'x' must have contiguous storage for its arrays")
+
         return cls(
             ptr=lib.py_initialize_dense_matrix(
-                x.shape[0], x.shape[1], str(x.dtype).encode("utf-8"), x.ctypes.data
+                x.shape[0],
+                x.shape[1],
+                str(x.dtype).encode("utf-8"),
+                x.ctypes.data,
+                byrow,
             ),
             obj=x,
         )
 
     @classmethod
     def from_csc_array(cls, x: sp.csc_array) -> "TatamiNumericPointer":
         """Initialize class from a compressed sparse column matrix.
```

### Comparing `mattress-0.0.4/src/mattress/__init__.py` & `mattress-0.0.5/src/mattress/__init__.py`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/cpphelpers.py` & `mattress-0.0.5/src/mattress/cpphelpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,15 +49,21 @@
 lib.py_extract_ncol.argtypes = [ct.c_void_p]
 lib.py_extract_sparse.restype = ct.c_int
 lib.py_extract_sparse.argtypes = [ct.c_void_p]
 lib.py_extract_row.argtypes = [ct.c_void_p, ct.c_int, ct.c_void_p]
 lib.py_extract_column.argtypes = [ct.c_void_p, ct.c_int, ct.c_void_p]
 
 lib.py_initialize_dense_matrix.restype = ct.c_void_p
-lib.py_initialize_dense_matrix.argtypes = [ct.c_int, ct.c_int, ct.c_char_p, ct.c_void_p]
+lib.py_initialize_dense_matrix.argtypes = [
+    ct.c_int,
+    ct.c_int,
+    ct.c_char_p,
+    ct.c_void_p,
+    ct.c_uint8,
+]
 
 lib.py_initialize_compressed_sparse_matrix.restype = ct.c_void_p
 lib.py_initialize_compressed_sparse_matrix.argtypes = [
     ct.c_int,
     ct.c_int,
     ct.c_uint64,
     ct.c_char_p,
```

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/.github/workflows/doxygenate.yaml` & `mattress-0.0.5/src/mattress/extern/tatami/.github/workflows/doxygenate.yaml`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/.github/workflows/run-gallery.yaml` & `mattress-0.0.5/src/mattress/extern/tatami/.github/workflows/run-gallery.yaml`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/.github/workflows/run-tests.yaml` & `mattress-0.0.5/src/mattress/extern/tatami_hdf5/.github/workflows/run-tests.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -16,35 +16,30 @@
             omp: true
           }
         - {
             name: "Ubuntu Latest GCC, coverage enabled", 
             os: ubuntu-latest,
             cov: true
           }
-        - {
-            name: "macOS Latest Clang", 
-            os: macos-latest
-          }
 
     steps:
     - uses: actions/checkout@v3
 
     - name: Get latest CMake
       uses: lukka/get-cmake@latest
 
-    - name: Configure the build for Mac
-      if: ${{ matrix.config.os == 'macos-latest' }}
-      run: cmake -S . -B build
+    - name: Install HDF5
+      run: sudo apt-get install libhdf5-dev
 
     - name: Configure the build with coverage
-      if: ${{ matrix.config.os == 'ubuntu-latest' && matrix.config.cov }}
+      if: ${{ matrix.config.cov }}
       run: cmake -S . -B build -DCODE_COVERAGE=ON 
 
     - name: Configure the build with OpenMP
-      if: ${{ matrix.config.os == 'ubuntu-latest' && matrix.config.omp }}
+      if: ${{ matrix.config.omp }}
       run: cmake -S . -B build -DUSE_OPENMP=ON
 
     - name: Run the build
       run: cmake --build build
 
     - name: Run the tests
       run: |
```

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/CMakeLists.txt` & `mattress-0.0.5/src/mattress/extern/tatami/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/LICENSE` & `mattress-0.0.5/src/mattress/extern/tatami/LICENSE`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/README.md` & `mattress-0.0.5/src/mattress/extern/tatami/README.md`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/docs/Doxyfile` & `mattress-0.0.5/src/mattress/extern/tatami/docs/Doxyfile`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/gallery/CMakeLists.txt` & `mattress-0.0.5/src/mattress/extern/tatami/gallery/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/gallery/README.md` & `mattress-0.0.5/src/mattress/extern/tatami/gallery/README.md`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/gallery/src/char2double.cpp` & `mattress-0.0.5/src/mattress/extern/tatami/gallery/src/char2double.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/gallery/src/colsums.cpp` & `mattress-0.0.5/src/mattress/extern/tatami/gallery/src/colsums.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/gallery/src/parallel.cpp` & `mattress-0.0.5/src/mattress/extern/tatami/gallery/src/parallel.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/gallery/src/print_vector.h` & `mattress-0.0.5/src/mattress/extern/tatami/gallery/src/print_vector.h`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/gallery/src/read_h5.cpp` & `mattress-0.0.5/src/mattress/extern/tatami/gallery/src/read_h5.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/gallery/src/read_mm.cpp` & `mattress-0.0.5/src/mattress/extern/tatami/gallery/src/read_mm.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/gallery/src/sparse_extractor.cpp` & `mattress-0.0.5/src/mattress/extern/tatami/gallery/src/sparse_extractor.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/base/Extractor.hpp` & `mattress-0.0.5/src/mattress/extern/tatami/include/tatami/base/Extractor.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/base/Matrix.hpp` & `mattress-0.0.5/src/mattress/extern/tatami/include/tatami/base/Matrix.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/base/Options.hpp` & `mattress-0.0.5/src/mattress/extern/tatami/include/tatami/base/Options.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/base/SparseRange.hpp` & `mattress-0.0.5/src/mattress/extern/tatami/include/tatami/base/SparseRange.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/base/utils.hpp` & `mattress-0.0.5/src/mattress/extern/tatami/include/tatami/base/utils.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/dense/DenseMatrix.hpp` & `mattress-0.0.5/src/mattress/extern/tatami/include/tatami/dense/DenseMatrix.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/dense/VirtualDenseMatrix.hpp` & `mattress-0.0.5/src/mattress/extern/tatami/include/tatami/dense/VirtualDenseMatrix.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/isometric/arith_utils.hpp` & `mattress-0.0.5/src/mattress/extern/tatami/include/tatami/isometric/arith_utils.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/isometric/binary/DelayedBinaryIsometricOp.hpp` & `mattress-0.0.5/src/mattress/extern/tatami/include/tatami/isometric/binary/DelayedBinaryIsometricOp.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/isometric/binary/arith_helpers.hpp` & `mattress-0.0.5/src/mattress/extern/tatami/include/tatami/isometric/binary/arith_helpers.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/isometric/binary/boolean_helpers.hpp` & `mattress-0.0.5/src/mattress/extern/tatami/include/tatami/isometric/binary/boolean_helpers.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/isometric/binary/compare_helpers.hpp` & `mattress-0.0.5/src/mattress/extern/tatami/include/tatami/isometric/binary/compare_helpers.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/isometric/binary/utils.hpp` & `mattress-0.0.5/src/mattress/extern/tatami/include/tatami/isometric/binary/utils.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/isometric/boolean_utils.hpp` & `mattress-0.0.5/src/mattress/extern/tatami/include/tatami/isometric/boolean_utils.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/isometric/compare_utils.hpp` & `mattress-0.0.5/src/mattress/extern/tatami/include/tatami/isometric/compare_utils.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/isometric/unary/DelayedUnaryIsometricOp.hpp` & `mattress-0.0.5/src/mattress/extern/tatami/include/tatami/isometric/unary/DelayedUnaryIsometricOp.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/isometric/unary/arith_helpers.hpp` & `mattress-0.0.5/src/mattress/extern/tatami/include/tatami/isometric/unary/arith_helpers.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/isometric/unary/boolean_helpers.hpp` & `mattress-0.0.5/src/mattress/extern/tatami/include/tatami/isometric/unary/boolean_helpers.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/isometric/unary/compare_helpers.hpp` & `mattress-0.0.5/src/mattress/extern/tatami/include/tatami/isometric/unary/compare_helpers.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/isometric/unary/math_helpers.hpp` & `mattress-0.0.5/src/mattress/extern/tatami/include/tatami/isometric/unary/math_helpers.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/other/DelayedBind.hpp` & `mattress-0.0.5/src/mattress/extern/tatami/include/tatami/other/DelayedBind.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/other/DelayedCast.hpp` & `mattress-0.0.5/src/mattress/extern/tatami/include/tatami/other/DelayedCast.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/other/DelayedTranspose.hpp` & `mattress-0.0.5/src/mattress/extern/tatami/include/tatami/other/DelayedTranspose.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/sparse/CompressedSparseMatrix.hpp` & `mattress-0.0.5/src/mattress/extern/tatami/include/tatami/sparse/CompressedSparseMatrix.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #ifndef TATAMI_COMPRESSED_SPARSE_MATRIX_H
 #define TATAMI_COMPRESSED_SPARSE_MATRIX_H
 
 #include "../base/Matrix.hpp"
 #include "../base/utils.hpp"
 #include "primary_extraction.hpp"
 #include "SparseSecondaryExtractorCore.hpp"
+#include "../utils/ElementType.hpp"
 
 #include <vector>
 #include <algorithm>
 #include <memory>
 #include <utility>
 #include <stdexcept>
 
@@ -87,15 +88,15 @@
             }
 
             auto last = indptrs[indptrs.size() - 1]; // don't use back() as this is not guaranteed to be available for arbitrary PointerStorage_.
             if (static_cast<size_t>(last) != indices.size()) {
                 throw std::runtime_error("last element of 'indptrs' should be equal to length of 'indices'");
             }
 
-            Stored<IndexStorage_> max_index = (row_ ? ncols : nrows);
+            ElementType<IndexStorage_> max_index = (row_ ? ncols : nrows);
             for (size_t i = 1; i < indptrs.size(); ++i) {
                 auto start = indptrs[i- 1], end = indptrs[i];
                 if (end < start || end > last) {
                     throw std::runtime_error("'indptrs' should be in non-decreasing order");
                 }
 
                 for (auto x = start; x < end; ++x) {
@@ -295,16 +296,16 @@
         }
     };
 
     /*************************************
      ******* Secondary extraction ********
      *************************************/
 private:
-    typedef Stored<IndexStorage_> StoredIndex;
-    typedef Stored<PointerStorage_> StoredPointer;
+    typedef ElementType<IndexStorage_> StoredIndex;
+    typedef ElementType<PointerStorage_> StoredPointer;
 
     struct SecondaryModifier {
         static void increment(StoredPointer& ptr, const IndexStorage_&, StoredPointer) { ++ptr; }
         static void decrement(StoredPointer& ptr, const IndexStorage_&, StoredPointer) { --ptr; }
         static StoredPointer get(StoredPointer ptr) { return ptr; }
         static void set(StoredPointer& ptr, StoredPointer val) { ptr = val; }
     };
```

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/sparse/FragmentedSparseMatrix.hpp` & `mattress-0.0.5/src/mattress/extern/tatami/include/tatami/sparse/FragmentedSparseMatrix.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #ifndef TATAMI_FRAGMENTED_SPARSE_MATRIX_H
 #define TATAMI_FRAGMENTED_SPARSE_MATRIX_H
 
 #include "../base/Matrix.hpp"
 #include "../base/utils.hpp"
 #include "primary_extraction.hpp"
 #include "SparseSecondaryExtractorCore.hpp"
+#include "../utils/ElementType.hpp"
 
 #include <vector>
 #include <algorithm>
 #include <memory>
 #include <utility>
 #include <stdexcept>
 
@@ -78,15 +79,15 @@
                 }
             } else {
                 if (indices.size() != static_cast<size_t>(ncols)) {
                     throw std::runtime_error("length of 'indices' should be equal to number of columns");
                 }
             }
 
-            Stored<Stored<IndexVectorStorage_> > max_index = (row_ ? ncols : nrows);
+            ElementType<ElementType<IndexVectorStorage_> > max_index = (row_ ? ncols : nrows);
             for (size_t i = 0, end = indices.size(); i < end; ++i) {
                 const auto& curv = values[i];
                 const auto& curi = indices[i];
                 if (curv.size() != curi.size()) {
                     throw std::runtime_error("corresponding elements of 'values' and 'indices' should have the same length");
                 }
 
@@ -284,15 +285,15 @@
     };
 
     /*************************************
      ******* Secondary extraction ********
      *************************************/
 private:
     typedef typename std::remove_reference<decltype(std::declval<IndexVectorStorage_>()[0])>::type IndexStorage;
-    typedef Stored<IndexStorage> StoredIndex;
+    typedef ElementType<IndexStorage> StoredIndex;
 
     struct SecondaryModifier {
         static void increment(size_t& ptr, const IndexStorage&, size_t) { ++ptr; }
         static void decrement(size_t& ptr, const IndexStorage&, size_t) { --ptr; }
         static size_t get(size_t ptr) { return ptr; }
         static void set(size_t& ptr, size_t val) { ptr = val; }
     };
```

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/sparse/SemiCompressedSparseMatrix.hpp` & `mattress-0.0.5/src/mattress/extern/tatami/include/tatami/sparse/SemiCompressedSparseMatrix.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #ifndef TATAMI_SEMI_COMPRESSED_SPARSE_MATRIX_H
 #define TATAMI_SEMI_COMPRESSED_SPARSE_MATRIX_H
 
 #include "../base/Matrix.hpp"
 #include "../base/utils.hpp"
 #include "utils.hpp"
 #include "SparseSecondaryExtractorCore.hpp"
+#include "../utils/ElementType.hpp"
 
 #include <vector>
 #include <algorithm>
 #include <memory>
 #include <utility>
 #include <stdexcept>
 #include <string>
@@ -107,16 +108,16 @@
     }
 
 private:
     Index_ nrows, ncols;
     IndexStorage_ indices;
     PointerStorage_ indptrs;
 
-    typedef Stored<IndexStorage_> StoredIndex;
-    typedef Stored<PointerStorage_> StoredPointer;
+    typedef ElementType<IndexStorage_> StoredIndex;
+    typedef ElementType<PointerStorage_> StoredPointer;
 
 public:
     Index_ nrow() const { return nrows; }
 
     Index_ ncol() const { return ncols; }
 
     bool sparse() const { return true; }
```

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/sparse/SparseSecondaryExtractorCore.hpp` & `mattress-0.0.5/src/mattress/extern/tatami/include/tatami/sparse/SparseSecondaryExtractorCore.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -5,17 +5,14 @@
 #include <type_traits>
 #include <algorithm>
 
 #include "utils.hpp"
 
 namespace tatami {
 
-template<class Storage_>
-using Stored = typename std::remove_reference<decltype(std::declval<Storage_>()[0])>::type;
-
 template<typename Index_, typename StoredIndex_, typename CustomPointer_, class CustomPointerModifier_> 
 struct SparseSecondaryExtractorCore {
 protected:
     // The current position of the pointer at each primary element.
     std::vector<CustomPointer_> current_indptrs; 
 
     /*
```

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/sparse/convert_to_compressed_sparse.hpp` & `mattress-0.0.5/src/mattress/extern/tatami/include/tatami/sparse/convert_to_compressed_sparse.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/sparse/convert_to_fragmented_sparse.hpp` & `mattress-0.0.5/src/mattress/extern/tatami/include/tatami/sparse/convert_to_fragmented_sparse.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/sparse/primary_extraction.hpp` & `mattress-0.0.5/src/mattress/extern/tatami/include/tatami/sparse/primary_extraction.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #ifndef TATAMI_SPARSE_PRIMARY_EXTRACTION_HPP
 #define TATAMI_SPARSE_PRIMARY_EXTRACTION_HPP
 
 #include "utils.hpp"
 #include <utility>
 #include <algorithm>
+#include "../utils/ElementType.hpp"
 
 namespace tatami {
 
 namespace sparse_utils {
 
 template<typename Index_, class IndexStorage_, class PointerStorage_>
 std::pair<size_t, size_t> extract_primary_dimension(Index_ i, const IndexStorage_& indices, const PointerStorage_& indptrs) {
@@ -32,19 +33,19 @@
         }
     }
 
     auto iIt = indices.begin() + sparse_utils::get_lower_limit(indptrs, i);
     auto eIt = indices.begin() + sparse_utils::get_upper_limit(indices, indptrs, i);
 
     if (iIt != eIt) {
-        if (start > *iIt) {
+        if (start > static_cast<Index_>(*iIt)) {
             iIt = std::lower_bound(iIt, eIt, start);
         } 
 
-        auto last = start + length;
+        ElementType<IndexStorage_> last = start + length;
 
         // Comparing the one-past-the-last requested index with the last observed index at 'eIt'.
         // If the former is less than the latter, then we need to do a binary search.
         // If greater than the latter, we restore 'eIt' to its original position.
         // If equal, then the decremented 'eIt' is already the one-past-the-last index, so we keep it as-is.
         --eIt;
         if (last < *eIt) {
@@ -139,15 +140,15 @@
 
     if (iIt == eIt) {
         return;
     }
 
     Index_ counter = 0;
     while (counter < length) {
-        auto current = subset[counter];
+        ElementType<IndexStorage_> current = subset[counter];
 
         while (iIt != eIt && current > *iIt) {
             ++iIt;
         }
         if (iIt == eIt) {
             break;
         }
```

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/sparse/utils.hpp` & `mattress-0.0.5/src/mattress/extern/tatami/include/tatami/sparse/utils.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/stats/medians.hpp` & `mattress-0.0.5/src/mattress/extern/tatami/include/tatami/stats/medians.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/stats/ranges.hpp` & `mattress-0.0.5/src/mattress/extern/tatami/include/tatami/stats/ranges.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/stats/sums.hpp` & `mattress-0.0.5/src/mattress/extern/tatami/include/tatami/stats/sums.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/stats/utils.hpp` & `mattress-0.0.5/src/mattress/extern/tatami/include/tatami/stats/utils.hpp`

 * *Files 20% similar despite different names*

```diff
@@ -3,26 +3,39 @@
 
 #include "../base/Matrix.hpp"
 #include "../base/utils.hpp"
 #include "../utils/Oracles.hpp"
 
 #include <cmath>
 
+#ifndef TATAMI_CUSTOM_PARALLEL
+#ifndef _OPENMP
+#include <thread>
+#endif
+#include <string>
+#include <stdexcept>
+#include <vector>
+#endif
+
 /**
  * @file utils.hpp
  *
  * @brief Utilities for computing matrix statistics.
  */
 
 namespace tatami {
 
 /**
- * Apply a function to a set of tasks, distributing them to threads via OpenMP if enabled.
- * Callers can specify a custom parallelization scheme by defining a `TATAMI_CUSTOM_PARALLEL` function-like macro, 
- * which should accept the `fun`, `tasks` and `threads` arguments as below.
+ * Apply a function to a set of tasks in parallel.
+ * This can be done using:
+ *
+ * - OpenMP, if available and enabled by the compiler.
+ * - Using a custom parallelization scheme, by defining a `TATAMI_CUSTOM_PARALLEL` function-like macro. 
+ *   This should accept the `fun`, `tasks` and `threads` arguments as below.
+ * - `<thread>`, otherwise.
  *
  * @tparam parallel_ Whether the tasks should be run in parallel.
  * If `false`, no parallelization is performed and all tasks are run on the current thread.
  * @tparam Function_ Function to be applied for a contiguous range of tasks.
  * This should accept three arguments:
  * - `thread`, the thread number executing this task range.
  *   This will be passed as a `size_t`.
@@ -33,41 +46,74 @@
  * @tparam Index_ Integer type for the number of tasks.
  *
  * @param fun Function that executes a contiguous range of tasks.
  * @param tasks Number of tasks.
  * @param threads Number of threads.
  */
 template<bool parallel_ = true, class Function_, typename Index_>
-void parallelize(Function_ fun, Index_ tasks, size_t
-#if defined(_OPENMP) || defined(TATAMI_CUSTOM_PARALLEL)
-    threads // wrap here to avoid used variable warnings (which are in turn converted to errors).
-#endif
-) {
-#if defined(_OPENMP) || defined(TATAMI_CUSTOM_PARALLEL)
-
+void parallelize(Function_ fun, Index_ tasks, size_t threads) {
     if constexpr(parallel_) {
-
         if (threads > 1) {
 #ifndef TATAMI_CUSTOM_PARALLEL
             Index_ worker_size = (tasks / threads) + (tasks % threads > 0); // Ceiling of an integer division.
             threads = (tasks / worker_size) + (tasks % worker_size > 0); // Set the actual number of required threads.
+            std::vector<std::string> errors(threads);
 
+#if defined(_OPENMP)
             #pragma omp parallel for num_threads(threads)
             for (size_t t = 0; t < threads; ++t) {
                 Index_ start = worker_size * t; // Will not overflow due to the above recomputation of 'threads'.
                 Index_ remaining = tasks - start; // Must be positive, as otherwise 'tasks % worker_size = 0' and the iteration wouldn't even get here.
-                fun(t, start, std::min(remaining, worker_size)); // Use 'remaining' to avoid potential overflow from computing 'end = start + worker_size'.
+
+                try {
+                    fun(t, start, std::min(remaining, worker_size)); // Use 'remaining' to avoid potential overflow from computing 'end = start + worker_size'.
+                } catch (std::exception& e) {
+                    errors[t] = e.what();
+                } catch (...) {
+                    errors[t] = "unknown error in thread " + std::to_string(t);
+                }
             }
+
+#else
+            Index_ first = 0;
+            std::vector<std::thread> workers;
+            workers.reserve(threads);
+
+            for (size_t t = 0; t < threads && first < tasks; ++t) {
+                Index_ remaining = tasks - first;
+                Index_ len = std::min(remaining, worker_size);
+                workers.emplace_back([&fun,&errors](int t, Index_ first, Index_ len) -> void {
+                    try {
+                        fun(t, first, len);
+                    } catch (std::exception& e) {
+                        errors[t] = e.what();
+                    } catch (...) {
+                        errors[t] = "unknown error in thread " + std::to_string(t);
+                    }
+                }, t, first, len);
+                first += len;
+            }
+
+            for (auto& wrk : workers) {
+                wrk.join();
+            }
+#endif
+
+            for (const auto& e : errors) {
+                if (!e.empty()) {
+                    throw std::runtime_error(e);
+                }
+            }
+
 #else
             TATAMI_CUSTOM_PARALLEL(std::move(fun), tasks, threads);
 #endif
             return;
         }
     }
-#endif
 
     fun(0, 0, tasks);
     return;
 }
 
 /**
  * @tparam row_ Whether to perform extraction on rows.
```

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/stats/variances.hpp` & `mattress-0.0.5/src/mattress/extern/tatami/include/tatami/stats/variances.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/subset/DelayedSubset.hpp` & `mattress-0.0.5/src/mattress/extern/tatami/include/tatami/subset/DelayedSubset.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/subset/DelayedSubsetBlock.hpp` & `mattress-0.0.5/src/mattress/extern/tatami/include/tatami/subset/DelayedSubsetBlock.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -29,18 +29,18 @@
  * @tparam Index_ Integer type for the row/column indices.
  */
 template<int margin_, typename Value_, typename Index_>
 class DelayedSubsetBlock : public Matrix<Value_, Index_> {
 public:
     /**
      * @param p Pointer to the underlying (pre-subset) matrix.
-     * @param f Index of the start of the block. This should be a row index if `margin_ = 0` and a column index otherwise.
-     * @param l Index of the one-past-the-end of the block.
+     * @param s Index of the start of the block. This should be a row index if `margin_ = 0` and a column index otherwise.
+     * @param l Length of the block, in terms of the number of rows (if `margin_ = 0`) or columns (otherwise).
      */
-    DelayedSubsetBlock(std::shared_ptr<const Matrix<Value_, Index_> > p, Index_ f, Index_ l) : mat(std::move(p)), block_start(f), block_length(l - f) {}
+    DelayedSubsetBlock(std::shared_ptr<const Matrix<Value_, Index_> > p, Index_ s, Index_ l) : mat(std::move(p)), block_start(s), block_length(l) {}
 
 private:
     std::shared_ptr<const Matrix<Value_, Index_> > mat;
     Index_ block_start, block_length;
 
 public:
     Index_ nrow() const {
```

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/subset/DelayedSubsetSorted.hpp` & `mattress-0.0.5/src/mattress/extern/tatami/include/tatami/subset/DelayedSubsetSorted.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/subset/DelayedSubsetSortedUnique.hpp` & `mattress-0.0.5/src/mattress/extern/tatami/include/tatami/subset/DelayedSubsetSortedUnique.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/subset/DelayedSubsetUnique.hpp` & `mattress-0.0.5/src/mattress/extern/tatami/include/tatami/subset/DelayedSubsetUnique.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/subset/make_DelayedSubset.hpp` & `mattress-0.0.5/src/mattress/extern/tatami/include/tatami/subset/make_DelayedSubset.hpp`

 * *Files 12% similar despite different names*

```diff
@@ -55,17 +55,32 @@
                     has_duplicates = true;
                     break;
                 }
             }
         }
 
         if (!has_duplicates) {
-            return std::shared_ptr<Matrix<Value_, Index_> >(
-                new DelayedSubsetSortedUnique<margin_, Value_, Index_, PureIndexStorage_>(std::move(p), std::move(idx), false)
-            );
+            bool consecutive = true;
+            for (Index_ i = 0, end = idx.size(); i < end; ++i) {
+                if (idx[i] > idx[i-1] + 1) {
+                    consecutive = false;
+                    break;
+                }
+            }
+
+            if (consecutive) {
+                auto start = (idx.empty() ? 0 : idx[0]);
+                return std::shared_ptr<Matrix<Value_, Index_> >(
+                    new DelayedSubsetBlock<margin_, Value_, Index_>(std::move(p), start, idx.size())
+                );
+            } else {
+                return std::shared_ptr<Matrix<Value_, Index_> >(
+                    new DelayedSubsetSortedUnique<margin_, Value_, Index_, PureIndexStorage_>(std::move(p), std::move(idx), false)
+                );
+            }
         } else {
             return std::shared_ptr<Matrix<Value_, Index_> >(
                 new DelayedSubsetSorted<margin_, Value_, Index_, PureIndexStorage_>(std::move(p), std::move(idx), false)
             );
         }
     }
```

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/subset/utils.hpp` & `mattress-0.0.5/src/mattress/extern/tatami/include/tatami/subset/utils.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/tatami.hpp` & `mattress-0.0.5/src/mattress/extern/tatami/include/tatami/tatami.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/utils/ArrayView.hpp` & `mattress-0.0.5/src/mattress/extern/tatami/include/tatami/utils/ArrayView.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/utils/Oracles.hpp` & `mattress-0.0.5/src/mattress/extern/tatami/include/tatami/utils/Oracles.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/utils/SomeNumericArray.hpp` & `mattress-0.0.5/src/mattress/extern/tatami/include/tatami/utils/SomeNumericArray.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/utils/bind_intersection.hpp` & `mattress-0.0.5/src/mattress/extern/tatami/include/tatami/utils/bind_intersection.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/utils/compress_sparse_triplets.hpp` & `mattress-0.0.5/src/mattress/extern/tatami/include/tatami/utils/compress_sparse_triplets.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/utils/convert_to_dense.hpp` & `mattress-0.0.5/src/mattress/extern/tatami/include/tatami/dense/convert_to_dense.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/utils/convert_to_sparse.hpp` & `mattress-0.0.5/src/mattress/extern/tatami/include/tatami/utils/convert_to_sparse.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/utils/process_consecutive_indices.hpp` & `mattress-0.0.5/src/mattress/extern/tatami/include/tatami/utils/process_consecutive_indices.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/utils/wrap_shared_ptr.hpp` & `mattress-0.0.5/src/mattress/extern/tatami/include/tatami/utils/wrap_shared_ptr.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/include/tatami_test/simulate_vector.hpp` & `mattress-0.0.5/src/mattress/extern/tatami/include/tatami_test/simulate_vector.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/include/tatami_test/temp_file_path.hpp` & `mattress-0.0.5/src/mattress/extern/tatami/include/tatami_test/temp_file_path.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/include/tatami_test/test_access_base.hpp` & `mattress-0.0.5/src/mattress/extern/tatami/include/tatami_test/test_access_base.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/include/tatami_test/test_column_access.hpp` & `mattress-0.0.5/src/mattress/extern/tatami/include/tatami_test/test_column_access.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/include/tatami_test/test_oracle_access.hpp` & `mattress-0.0.5/src/mattress/extern/tatami/include/tatami_test/test_oracle_access.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/include/tatami_test/test_row_access.hpp` & `mattress-0.0.5/src/mattress/extern/tatami/include/tatami_test/test_row_access.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/include/tatami_test/utils.hpp` & `mattress-0.0.5/src/mattress/extern/tatami/include/tatami_test/utils.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/tests/README.md` & `mattress-0.0.5/src/mattress/extern/tatami/tests/README.md`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/tests/src/dense/DenseMatrix.cpp` & `mattress-0.0.5/src/mattress/extern/tatami/tests/src/dense/DenseMatrix.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/tests/src/isometric/binary/arith_helpers.cpp` & `mattress-0.0.5/src/mattress/extern/tatami/tests/src/isometric/binary/arith_helpers.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/tests/src/isometric/binary/boolean_helpers.cpp` & `mattress-0.0.5/src/mattress/extern/tatami/tests/src/isometric/binary/boolean_helpers.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/tests/src/isometric/binary/compare_helpers.cpp` & `mattress-0.0.5/src/mattress/extern/tatami/tests/src/isometric/binary/compare_helpers.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/tests/src/isometric/unary/arith_scalar_helpers.cpp` & `mattress-0.0.5/src/mattress/extern/tatami/tests/src/isometric/unary/arith_scalar_helpers.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/tests/src/isometric/unary/arith_vector_helpers.cpp` & `mattress-0.0.5/src/mattress/extern/tatami/tests/src/isometric/unary/arith_vector_helpers.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/tests/src/isometric/unary/boolean_scalar_helpers.cpp` & `mattress-0.0.5/src/mattress/extern/tatami/tests/src/isometric/unary/boolean_scalar_helpers.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/tests/src/isometric/unary/boolean_vector_helpers.cpp` & `mattress-0.0.5/src/mattress/extern/tatami/tests/src/isometric/unary/boolean_vector_helpers.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/tests/src/isometric/unary/compare_scalar_helpers.cpp` & `mattress-0.0.5/src/mattress/extern/tatami/tests/src/isometric/unary/compare_scalar_helpers.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/tests/src/isometric/unary/compare_vector_helpers.cpp` & `mattress-0.0.5/src/mattress/extern/tatami/tests/src/isometric/unary/compare_vector_helpers.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/tests/src/isometric/unary/math_helpers.cpp` & `mattress-0.0.5/src/mattress/extern/tatami/tests/src/isometric/unary/math_helpers.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/tests/src/isometric/utils.h` & `mattress-0.0.5/src/mattress/extern/tatami/tests/src/isometric/utils.h`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/tests/src/other/DelayedBind.cpp` & `mattress-0.0.5/src/mattress/extern/tatami/tests/src/other/DelayedBind.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/tests/src/other/DelayedCast.cpp` & `mattress-0.0.5/src/mattress/extern/tatami/tests/src/other/DelayedCast.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/tests/src/other/DelayedTranspose.cpp` & `mattress-0.0.5/src/mattress/extern/tatami/tests/src/other/DelayedTranspose.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/tests/src/sparse/CompressedSparseMatrix.cpp` & `mattress-0.0.5/src/mattress/extern/tatami/tests/src/sparse/CompressedSparseMatrix.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -68,18 +68,27 @@
     indptr.back() = indices.size();
     tatami_test::throws_error([&]() { tatami::CompressedSparseColumnMatrix<double, int> mat(10, 20, values, indices, indptr); }, "strictly increasing");
     tatami_test::throws_error([&]() { tatami::CompressedSparseRowMatrix<double, int> mat(20, 10, values, indices, indptr); }, "strictly increasing");
 }
 
 TEST(CompressedSparseMatrix, OddTypes) {
     // Checking for compilation warnings here when the interface and storage types are different.
-    std::vector<uint8_t> values;
-    std::vector<uint16_t> indices;
-    std::vector<uint64_t> indptr(11);
-    tatami::CompressedSparseRowMatrix<double, int, decltype(values), decltype(indices), decltype(indptr)> rmat(10, 20, values, indices, indptr);
+    {
+        std::vector<uint8_t> values;
+        std::vector<uint16_t> indices;
+        std::vector<uint64_t> indptr(11);
+        tatami::CompressedSparseRowMatrix<double, int, decltype(values), decltype(indices), decltype(indptr)> rmat(10, 20, values, indices, indptr);
+    }
+
+    {
+        std::vector<uint8_t> values;
+        std::vector<uint32_t> indices; // Check for signed/unsigned comparisons with the interface index type.
+        std::vector<uint64_t> indptr(11);
+        tatami::CompressedSparseRowMatrix<double, int32_t, decltype(values), decltype(indices), decltype(indptr)> rmat(10, 20, values, indices, indptr);
+    }
 }
 
 /*************************************
  *************************************/
 
 class SparseTestMethods {
 protected:
```

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/tests/src/sparse/FragmentedSparseMatrix.cpp` & `mattress-0.0.5/src/mattress/extern/tatami/tests/src/sparse/FragmentedSparseMatrix.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/tests/src/sparse/SemiCompressedSparseMatrix.cpp` & `mattress-0.0.5/src/mattress/extern/tatami/tests/src/sparse/SemiCompressedSparseMatrix.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/tests/src/sparse/SparseSecondaryExtractorCore.cpp` & `mattress-0.0.5/src/mattress/extern/tatami/tests/src/sparse/SparseSecondaryExtractorCore.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/tests/src/sparse/convert_to_compressed_sparse.cpp` & `mattress-0.0.5/src/mattress/extern/tatami/tests/src/sparse/convert_to_compressed_sparse.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/tests/src/sparse/convert_to_fragmented_sparse.cpp` & `mattress-0.0.5/src/mattress/extern/tatami/tests/src/sparse/convert_to_fragmented_sparse.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/tests/src/stats/custom_parallel.h` & `mattress-0.0.5/src/mattress/extern/tatami/tests/src/stats/custom_parallel.h`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/tests/src/stats/medians.cpp` & `mattress-0.0.5/src/mattress/extern/tatami/tests/src/stats/medians.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/tests/src/stats/ranges.cpp` & `mattress-0.0.5/src/mattress/extern/tatami/tests/src/stats/ranges.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/tests/src/stats/sums.cpp` & `mattress-0.0.5/src/mattress/extern/tatami/tests/src/stats/sums.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/tests/src/stats/variances.cpp` & `mattress-0.0.5/src/mattress/extern/tatami/tests/src/stats/variances.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/tests/src/subset/DelayedSubset.cpp` & `mattress-0.0.5/src/mattress/extern/tatami/tests/src/subset/DelayedSubset.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/tests/src/subset/DelayedSubsetBlock.cpp` & `mattress-0.0.5/src/mattress/extern/tatami/tests/src/subset/DelayedSubsetBlock.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #include <gtest/gtest.h>
 
 #include <vector>
 #include <memory>
 
 #include "tatami/dense/DenseMatrix.hpp"
 #include "tatami/subset/DelayedSubsetBlock.hpp"
+#include "tatami/subset/make_DelayedSubset.hpp"
 #include "tatami/utils/convert_to_sparse.hpp"
 
 #include "tatami_test/tatami_test.hpp"
 
 template<class PARAM> 
 class SubsetBlockTest : public ::testing::TestWithParam<PARAM> {
 protected:
@@ -30,26 +31,26 @@
         int first = full * std::get<1>(param).first;
         int last = full * std::get<1>(param).second;
         block_length = last - first;
 
         if (std::get<0>(param)) {
             std::vector<double> sub(simulated.data() + first * NC, simulated.data() + last * NC);
             ref.reset(new tatami::DenseRowMatrix<double>(block_length, NC, std::move(sub)));
-            dense_block = tatami::make_DelayedSubsetBlock<0>(dense, first, last);
-            sparse_block = tatami::make_DelayedSubsetBlock<0>(sparse, first, last);
+            dense_block = tatami::make_DelayedSubsetBlock<0>(dense, first, block_length);
+            sparse_block = tatami::make_DelayedSubsetBlock<0>(sparse, first, block_length);
         } else {
             std::vector<double> sub;
             sub.reserve(NR * block_length);
             for (int r = 0; r < NR; ++r) {
                 auto row = simulated.data() + r * NC;
                 sub.insert(sub.end(), row + first, row + last);
             }
             ref.reset(new tatami::DenseRowMatrix<double>(NR, block_length, std::move(sub)));
-            dense_block = tatami::make_DelayedSubsetBlock<1>(dense, first, last);
-            sparse_block = tatami::make_DelayedSubsetBlock<1>(sparse, first, last);
+            dense_block = tatami::make_DelayedSubsetBlock<1>(dense, first, block_length);
+            sparse_block = tatami::make_DelayedSubsetBlock<1>(sparse, first, block_length);
         }
     }
 };
 
 /*****************************
  *****************************/
 
@@ -226,25 +227,26 @@
         auto simulated = tatami_test::simulate_sparse_vector<double>(NR * NC, 0.2);
         auto dense = std::shared_ptr<tatami::NumericMatrix>(new tatami::DenseRowMatrix<double>(NR, NC, simulated));
         auto sparse = tatami::convert_to_sparse<false>(dense.get()); // column-major.
 
         double full =  (std::get<0>(param) ? NR : NC);
         int first = full * std::get<1>(param).first;
         int last = full * std::get<1>(param).second;
+        auto len = last - first;
 
         if (std::get<0>(param)) {
-            dense_block = tatami::make_DelayedSubsetBlock<0>(dense, first, last);
-            sparse_block = tatami::make_DelayedSubsetBlock<0>(sparse, first, last);
-            wrapped_dense_block = tatami::make_DelayedSubsetBlock<0>(tatami_test::make_CrankyMatrix(dense), first, last);
-            wrapped_sparse_block = tatami::make_DelayedSubsetBlock<0>(tatami_test::make_CrankyMatrix(sparse), first, last);
+            dense_block = tatami::make_DelayedSubsetBlock<0>(dense, first, len);
+            sparse_block = tatami::make_DelayedSubsetBlock<0>(sparse, first, len);
+            wrapped_dense_block = tatami::make_DelayedSubsetBlock<0>(tatami_test::make_CrankyMatrix(dense), first, len);
+            wrapped_sparse_block = tatami::make_DelayedSubsetBlock<0>(tatami_test::make_CrankyMatrix(sparse), first, len);
         } else {
-            dense_block = tatami::make_DelayedSubsetBlock<1>(dense, first, last);
-            sparse_block = tatami::make_DelayedSubsetBlock<1>(sparse, first, last);
-            wrapped_dense_block = tatami::make_DelayedSubsetBlock<1>(tatami_test::make_CrankyMatrix(dense), first, last);
-            wrapped_sparse_block = tatami::make_DelayedSubsetBlock<1>(tatami_test::make_CrankyMatrix(sparse), first, last);
+            dense_block = tatami::make_DelayedSubsetBlock<1>(dense, first, len);
+            sparse_block = tatami::make_DelayedSubsetBlock<1>(sparse, first, len);
+            wrapped_dense_block = tatami::make_DelayedSubsetBlock<1>(tatami_test::make_CrankyMatrix(dense), first, len);
+            wrapped_sparse_block = tatami::make_DelayedSubsetBlock<1>(tatami_test::make_CrankyMatrix(sparse), first, len);
         }
     }
 };
 
 TEST_P(SubsetBlockOracleTest, Validate) {
     auto param = GetParam();
     assemble(param);
@@ -276,12 +278,36 @@
 
 /****************************************************
  ****************************************************/
 
 TEST(DelayedSubsetBlock, ConstOverload) {
     int NR = 9, NC = 7;
     auto dense = std::shared_ptr<const tatami::NumericMatrix>(new tatami::DenseRowMatrix<double>(NR, NC, tatami_test::simulate_sparse_vector<double>(NR * NC, 0.1)));
-    auto sub = tatami::make_DelayedSubsetBlock<1>(dense, static_cast<int>(5), static_cast<int>(8));
+    auto sub = tatami::make_DelayedSubsetBlock<1>(dense, static_cast<int>(5), static_cast<int>(3));
     EXPECT_EQ(sub->ncol(), 3);
     EXPECT_EQ(sub->nrow(), NR);
 }
 
+TEST(DelayedSubsetBlock, CorrectMaker) {
+    int NR = 90, NC = 50;
+    auto dense = std::shared_ptr<const tatami::NumericMatrix>(new tatami::DenseRowMatrix<double>(NR, NC, tatami_test::simulate_dense_vector<double>(NR * NC)));
+
+    // Checking that the make function dispatches correctly to the block subset class.
+    {
+        std::vector<int> indices { 5, 6, 7, 8, 9, 10 };
+        auto sub = tatami::make_DelayedSubset<1>(dense, indices);
+        EXPECT_EQ(sub->ncol(), 6);
+        EXPECT_EQ(sub->nrow(), NR);
+
+        auto ref = tatami::make_DelayedSubsetBlock<1>(dense, static_cast<int>(5), static_cast<int>(6));
+        tatami_test::test_simple_row_access(sub.get(), ref.get(), true, 1);
+        tatami_test::test_simple_column_access(sub.get(), ref.get(), true, 1);
+    }
+
+    // Checking that it behaves correctly with an empty index vector.
+    {
+        std::vector<int> indices;
+        auto sub = tatami::make_DelayedSubset<0>(dense, indices);
+        EXPECT_EQ(sub->ncol(), NC);
+        EXPECT_EQ(sub->nrow(), 0);
+    }
+}
```

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/tests/src/utils/ArrayView.cpp` & `mattress-0.0.5/src/mattress/extern/tatami/tests/src/utils/ArrayView.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/tests/src/utils/Oracles.cpp` & `mattress-0.0.5/src/mattress/extern/tatami/tests/src/utils/Oracles.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/tests/src/utils/SomeNumericArray.cpp` & `mattress-0.0.5/src/mattress/extern/tatami/tests/src/utils/SomeNumericArray.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/tests/src/utils/bind_intersection.cpp` & `mattress-0.0.5/src/mattress/extern/tatami/tests/src/utils/bind_intersection.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/tests/src/utils/compress_sparse_triplets.cpp` & `mattress-0.0.5/src/mattress/extern/tatami/tests/src/utils/compress_sparse_triplets.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/tests/src/utils/convert_to_dense.cpp` & `mattress-0.0.5/src/mattress/extern/tatami/tests/src/dense/convert_to_dense.cpp`

 * *Files 22% similar despite different names*

```diff
@@ -2,193 +2,210 @@
 
 #include "tatami/dense/DenseMatrix.hpp"
 #include "tatami/sparse/CompressedSparseMatrix.hpp"
 #include "tatami/utils/convert_to_dense.hpp"
 
 #include "tatami_test/tatami_test.hpp"
 
-class ConvertToDenseTest : public ::testing::TestWithParam<std::tuple<int, int> > {
+class ConvertToDenseTest : public ::testing::TestWithParam<std::tuple<int, int, int> > {
 protected:
     size_t NR, NC;
+    int threads;
 
     template<class Param>
     void assemble(const Param& param) {
         NR = std::get<0>(param);
         NC = std::get<1>(param);
+        threads = std::get<2>(param);
     }
 };
 
 TEST_P(ConvertToDenseTest, RowToRow) {
     assemble(GetParam());
     auto vec = tatami_test::simulate_dense_vector<double>(NR * NC);
-    tatami::DenseMatrix<true, double, int> mat(NR, NC, vec);
+    auto mat = std::make_shared<tatami::DenseMatrix<true, double, int> >(NR, NC, vec);
 
-    auto converted = tatami::convert_to_dense<true>(&mat);
+    auto converted = tatami::convert_to_dense<true>(mat.get(), threads);
     EXPECT_TRUE(converted->prefer_rows());
     EXPECT_FALSE(converted->sparse());
-    tatami_test::test_simple_row_access(converted.get(), &mat, true, 1);
-    tatami_test::test_simple_column_access(converted.get(), &mat, true, 1);
+    tatami_test::test_simple_row_access(converted.get(), mat.get(), true, 1);
+    tatami_test::test_simple_column_access(converted.get(), mat.get(), true, 1);
 
-    auto converted2 = tatami::convert_to_dense<true, int, size_t>(&mat); // works for a different type.
+    auto converted2 = tatami::convert_to_dense<true, int, size_t>(mat.get(), threads); // works for a different type.
     EXPECT_TRUE(converted2->prefer_rows());
     EXPECT_FALSE(converted2->sparse());
 
     auto wrk2 = converted2->dense_row();
     for (size_t i = 0; i < NR; ++i) {
         auto start = vec.begin() + i * NC;
         std::vector<int> expected2(start, start + NC);
         EXPECT_EQ(wrk2->fetch(i), expected2);
     }
 
-    // Works in parallel.
-    auto convertedP = tatami::convert_to_dense<true>(&mat, 3);
-    tatami_test::test_simple_row_access(convertedP.get(), &mat, true, 1);
-    tatami_test::test_simple_column_access(convertedP.get(), &mat, true, 1);
+    // Works in cranky mode.
+    auto cranky = tatami_test::make_CrankyMatrix<double, int>(mat);
+    auto convertedC = tatami::convert_to_dense<true>(cranky.get(), threads);
+    tatami_test::test_simple_row_access(convertedC.get(), mat.get(), true, 1);
+    tatami_test::test_simple_column_access(convertedC.get(), mat.get(), true, 1);
 }
 
 TEST_P(ConvertToDenseTest, ColumnToColumn) {
     assemble(GetParam());
     auto vec = tatami_test::simulate_dense_vector<double>(NR * NC);
-    tatami::DenseMatrix<false, double, int> mat(NR, NC, vec);
+    auto mat = std::make_shared<tatami::DenseMatrix<false, double, int> >(NR, NC, vec);
 
-    auto converted = tatami::convert_to_dense<false>(&mat);
+    auto converted = tatami::convert_to_dense<false>(mat.get(), threads);
     EXPECT_FALSE(converted->prefer_rows());
     EXPECT_FALSE(converted->sparse());
-    tatami_test::test_simple_row_access(converted.get(), &mat, true, 1);
-    tatami_test::test_simple_column_access(converted.get(), &mat, true, 1);
+    tatami_test::test_simple_row_access(converted.get(), mat.get(), true, 1);
+    tatami_test::test_simple_column_access(converted.get(), mat.get(), true, 1);
 
-    auto converted2 = tatami::convert_to_dense<false, int, size_t>(&mat); // works for a different type.
+    auto converted2 = tatami::convert_to_dense<false, int, size_t>(mat.get(), threads); // works for a different type.
     EXPECT_FALSE(converted2->prefer_rows());
     EXPECT_FALSE(converted2->sparse());
 
     auto wrk2 = converted2->dense_column();
     for (size_t i = 0; i < NC; ++i) {
         auto start = vec.begin() + i * NR;
         std::vector<int> expected2(start, start + NR);
         EXPECT_EQ(wrk2->fetch(i), expected2);
     }
+
+    // Works in cranky mode.
+    auto cranky = tatami_test::make_CrankyMatrix<double, int>(mat);
+    auto convertedC = tatami::convert_to_dense<false>(cranky.get(), threads);
+    tatami_test::test_simple_row_access(convertedC.get(), mat.get(), true, 1);
+    tatami_test::test_simple_column_access(convertedC.get(), mat.get(), true, 1);
 }
 
 TEST_P(ConvertToDenseTest, RowToColumn) {
     assemble(GetParam());
     auto vec = tatami_test::simulate_dense_vector<double>(NR * NC);
-    tatami::DenseMatrix<true, double, int> mat(NR, NC, vec);
+    auto mat = std::make_shared<tatami::DenseMatrix<true, double, int> >(NR, NC, vec);
 
-    auto converted = tatami::convert_to_dense<false>(&mat);
+    auto converted = tatami::convert_to_dense<false>(mat.get(), threads);
     EXPECT_FALSE(converted->prefer_rows());
     EXPECT_FALSE(converted->sparse());
-    tatami_test::test_simple_row_access(converted.get(), &mat, true, 1);
-    tatami_test::test_simple_column_access(converted.get(), &mat, true, 1);
+    tatami_test::test_simple_row_access(converted.get(), mat.get(), true, 1);
+    tatami_test::test_simple_column_access(converted.get(), mat.get(), true, 1);
 
-    auto converted2 = tatami::convert_to_dense<false, int, size_t>(&mat); // works for a different type.
+    auto converted2 = tatami::convert_to_dense<false, int, size_t>(mat.get(), threads); // works for a different type.
     EXPECT_FALSE(converted2->prefer_rows());
     EXPECT_FALSE(converted2->sparse());
 
     auto wrk2 = converted2->dense_row();
     for (size_t i = 0; i < NR; ++i) {
         auto start = vec.begin() + i * NC;
         std::vector<int> expected2(start, start + NC);
         EXPECT_EQ(wrk2->fetch(i), expected2);
     }
 
-    // Works in parallel.
-    auto convertedP = tatami::convert_to_dense<false>(&mat, 3);
-    tatami_test::test_simple_row_access(convertedP.get(), &mat, true, 1);
-    tatami_test::test_simple_column_access(convertedP.get(), &mat, true, 1);
+    // Works in cranky mode.
+    auto cranky = tatami_test::make_CrankyMatrix<double, int>(mat);
+    auto convertedC = tatami::convert_to_dense<false>(cranky.get(), threads);
+    tatami_test::test_simple_row_access(convertedC.get(), mat.get(), true, 1);
+    tatami_test::test_simple_column_access(convertedC.get(), mat.get(), true, 1);
 }
 
 TEST_P(ConvertToDenseTest, ColumnToRow) {
     assemble(GetParam());
     auto vec = tatami_test::simulate_dense_vector<double>(NR * NC);
-    tatami::DenseMatrix<false, double, int> mat(NR, NC, vec);
+    auto mat = std::make_shared<tatami::DenseMatrix<false, double, int> >(NR, NC, vec);
 
-    auto converted = tatami::convert_to_dense<true>(&mat);
+    auto converted = tatami::convert_to_dense<true>(mat.get(), threads);
     EXPECT_TRUE(converted->prefer_rows());
     EXPECT_FALSE(converted->sparse());
-    tatami_test::test_simple_row_access(converted.get(), &mat, true, 1);
-    tatami_test::test_simple_column_access(converted.get(), &mat, true, 1);
+    tatami_test::test_simple_row_access(converted.get(), mat.get(), true, 1);
+    tatami_test::test_simple_column_access(converted.get(), mat.get(), true, 1);
 
-    auto converted2 = tatami::convert_to_dense<true, int, size_t>(&mat); // works for a different type.
+    auto converted2 = tatami::convert_to_dense<true, int, size_t>(mat.get(), threads); // works for a different type.
     EXPECT_TRUE(converted2->prefer_rows());
     EXPECT_FALSE(converted2->sparse());
 
     auto wrk2 = converted2->dense_column();
     for (size_t i = 0; i < NC; ++i) {
         auto start = vec.begin() + i * NR;
         std::vector<int> expected2(start, start + NR);
         EXPECT_EQ(wrk2->fetch(i), expected2);
     }
+
+    // Works in cranky mode.
+    auto cranky = tatami_test::make_CrankyMatrix<double, int>(mat);
+    auto convertedC = tatami::convert_to_dense<true>(cranky.get(), threads);
+    tatami_test::test_simple_row_access(convertedC.get(), mat.get(), true, 1);
+    tatami_test::test_simple_column_access(convertedC.get(), mat.get(), true, 1);
 }
 
 TEST_P(ConvertToDenseTest, Automatic) {
     assemble(GetParam());
     auto vec = tatami_test::simulate_dense_vector<double>(NR * NC);
 
     {
         tatami::DenseMatrix<false, double, int> mat(NR, NC, vec);
-        auto converted = tatami::convert_to_dense(&mat, -1);
+        auto converted = tatami::convert_to_dense(&mat, -1, threads);
         EXPECT_FALSE(converted->prefer_rows());
     }
 
     {
         tatami::DenseMatrix<true, double, int> mat(NR, NC, vec);
-        auto converted = tatami::convert_to_dense(&mat, -1);
+        auto converted = tatami::convert_to_dense(&mat, -1, threads);
         EXPECT_TRUE(converted->prefer_rows());
     }
 }
 
 TEST_P(ConvertToDenseTest, FromSparse) {
     assemble(GetParam());
 
     // From a row-major sparse matrix.
     {
         auto vec = tatami_test::simulate_sparse_compressed<double>(NR, NC, 0.2);
         tatami::CompressedSparseRowMatrix<double, int> smat(NR, NC, std::move(vec.value), std::move(vec.index), std::move(vec.ptr));
 
         {
-            auto converted = tatami::convert_to_dense<true>(&smat);
+            auto converted = tatami::convert_to_dense<true>(&smat, threads);
             EXPECT_TRUE(converted->prefer_rows());
             EXPECT_FALSE(converted->sparse());
             tatami_test::test_simple_row_access(converted.get(), &smat, true, 1);
             tatami_test::test_simple_column_access(converted.get(), &smat, true, 1);
         }
 
         {
-            auto converted = tatami::convert_to_dense<false>(&smat);
+            auto converted = tatami::convert_to_dense<false>(&smat, threads);
             EXPECT_FALSE(converted->prefer_rows());
             EXPECT_FALSE(converted->sparse());
             tatami_test::test_simple_row_access(converted.get(), &smat, true, 1);
             tatami_test::test_simple_column_access(converted.get(), &smat, true, 1);
         }
     }
 
     // From a row-major sparse matrix.
     {
         auto vec = tatami_test::simulate_sparse_compressed<double>(NC, NR, 0.2);
         tatami::CompressedSparseColumnMatrix<double, int> smat(NR, NC, std::move(vec.value), std::move(vec.index), std::move(vec.ptr));
 
         {
-            auto converted = tatami::convert_to_dense<true>(&smat);
+            auto converted = tatami::convert_to_dense<true>(&smat, threads);
             EXPECT_TRUE(converted->prefer_rows());
             EXPECT_FALSE(converted->sparse());
             tatami_test::test_simple_row_access(converted.get(), &smat, true, 1);
             tatami_test::test_simple_column_access(converted.get(), &smat, true, 1);
         }
 
         {
-            auto converted = tatami::convert_to_dense<false>(&smat);
+            auto converted = tatami::convert_to_dense<false>(&smat, threads);
             EXPECT_FALSE(converted->prefer_rows());
             EXPECT_FALSE(converted->sparse());
             tatami_test::test_simple_row_access(converted.get(), &smat, true, 1);
             tatami_test::test_simple_column_access(converted.get(), &smat, true, 1);
         }
     }
 }
 
 INSTANTIATE_TEST_SUITE_P(
     ConvertToDense,
     ConvertToDenseTest,
     ::testing::Combine(
         ::testing::Values(10, 50, 100), // number of rows
-        ::testing::Values(10, 50, 100)  // number of columns
+        ::testing::Values(10, 50, 100), // number of columns
+        ::testing::Values(1, 3)         // number of threads
     )
 );
```

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/tests/src/utils/process_consecutive_indices.cpp` & `mattress-0.0.5/src/mattress/extern/tatami/tests/src/utils/process_consecutive_indices.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami/tests/src/utils/wrap_shared_ptr.cpp` & `mattress-0.0.5/src/mattress/extern/tatami/tests/src/utils/wrap_shared_ptr.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami_hdf5/.github/workflows/doxygenate.yaml` & `mattress-0.0.5/src/mattress/extern/tatami_hdf5/.github/workflows/doxygenate.yaml`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami_hdf5/.github/workflows/run-tests.yaml` & `mattress-0.0.5/src/mattress/extern/tatami/.github/workflows/run-tests.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -7,41 +7,37 @@
     name: ${{ matrix.config.name }}
     runs-on: ${{ matrix.config.os }}
     strategy:
       fail-fast: false
       matrix:
         config:
         - {
-            name: "Ubuntu Latest GCC, OpenMP enabled", 
-            os: ubuntu-latest,
-            omp: true
-          }
-        - {
             name: "Ubuntu Latest GCC, coverage enabled", 
             os: ubuntu-latest,
             cov: true
           }
+        - {
+            name: "macOS Latest Clang", 
+            os: macos-latest
+          }
 
     steps:
     - uses: actions/checkout@v3
 
     - name: Get latest CMake
       uses: lukka/get-cmake@latest
 
-    - name: Install HDF5
-      run: sudo apt-get install libhdf5-dev
+    - name: Configure the build for Mac
+      if: ${{ matrix.config.os == 'macos-latest' }}
+      run: cmake -S . -B build
 
     - name: Configure the build with coverage
-      if: ${{ matrix.config.cov }}
+      if: ${{ matrix.config.os == 'ubuntu-latest' && matrix.config.cov }}
       run: cmake -S . -B build -DCODE_COVERAGE=ON 
 
-    - name: Configure the build with OpenMP
-      if: ${{ matrix.config.omp }}
-      run: cmake -S . -B build -DUSE_OPENMP=ON
-
     - name: Run the build
       run: cmake --build build
 
     - name: Run the tests
       run: |
         cd build
         ctest
```

### Comparing `mattress-0.0.4/src/mattress/extern/tatami_hdf5/CMakeLists.txt` & `mattress-0.0.5/src/mattress/extern/tatami_hdf5/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami_hdf5/LICENSE` & `mattress-0.0.5/src/mattress/extern/tatami_hdf5/LICENSE`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami_hdf5/README.md` & `mattress-0.0.5/src/mattress/extern/tatami_hdf5/README.md`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami_hdf5/docs/Doxyfile` & `mattress-0.0.5/src/mattress/extern/tatami_hdf5/docs/Doxyfile`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/Hdf5CompressedSparseMatrix.hpp` & `mattress-0.0.5/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/Hdf5CompressedSparseMatrix.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/Hdf5DenseMatrix.hpp` & `mattress-0.0.5/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/Hdf5DenseMatrix.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/load_hdf5_matrix.hpp` & `mattress-0.0.5/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/load_hdf5_matrix.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/utils.hpp` & `mattress-0.0.5/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/utils.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/write_sparse_matrix_to_hdf5.hpp` & `mattress-0.0.5/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/write_sparse_matrix_to_hdf5.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami_hdf5/tests/CMakeLists.txt` & `mattress-0.0.5/src/mattress/extern/tatami_hdf5/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami_hdf5/tests/src/Hdf5CompressedSparseMatrix.cpp` & `mattress-0.0.5/src/mattress/extern/tatami_hdf5/tests/src/Hdf5CompressedSparseMatrix.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami_hdf5/tests/src/Hdf5DenseMatrix.cpp` & `mattress-0.0.5/src/mattress/extern/tatami_hdf5/tests/src/Hdf5DenseMatrix.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami_hdf5/tests/src/custom_parallel.h` & `mattress-0.0.5/src/mattress/extern/tatami_hdf5/tests/src/custom_parallel.h`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami_hdf5/tests/src/load_hdf5_matrix.cpp` & `mattress-0.0.5/src/mattress/extern/tatami_hdf5/tests/src/load_hdf5_matrix.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/extern/tatami_hdf5/tests/src/write_sparse_matrix_to_hdf5.cpp` & `mattress-0.0.5/src/mattress/extern/tatami_hdf5/tests/src/write_sparse_matrix_to_hdf5.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/interface.py` & `mattress-0.0.5/src/mattress/interface.py`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/lib/common.cpp` & `mattress-0.0.5/src/mattress/lib/common.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/lib/compressed_sparse.cpp` & `mattress-0.0.5/src/mattress/lib/compressed_sparse.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress/lib/dense.cpp` & `mattress-0.0.5/src/mattress/lib/dense.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -1,52 +1,55 @@
 #include "Mattress.h"
 #include <string>
 #include <stdexcept>
 #include <cstring>
 #include <cstdint>
 
 template<typename T>
-Mattress* initialize_dense_matrix(int nr, int nc, const T* ptr) { 
+Mattress* initialize_dense_matrix(int nr, int nc, const T* ptr, bool byrow) { 
     tatami::ArrayView<T> view(ptr, static_cast<size_t>(nr) * static_cast<size_t>(nc));
-    return new Mattress(new tatami::DenseRowMatrix<double, int, decltype(view)>(nr, nc, view));
+    if (byrow) {
+        return new Mattress(new tatami::DenseRowMatrix<double, int, decltype(view)>(nr, nc, view));
+    } else { 
+        return new Mattress(new tatami::DenseColumnMatrix<double, int, decltype(view)>(nr, nc, view));
+    }
 }
 
 extern "C" {
 
-Mattress* py_initialize_dense_matrix(int nr, int nc, const char* type, void* ptr) {
+Mattress* py_initialize_dense_matrix(int nr, int nc, const char* type, void* ptr, uint8_t byrow) {
     if (std::strcmp(type, "float64") == 0) {
-        return initialize_dense_matrix(nr, nc, reinterpret_cast<double*>(ptr));
+        return initialize_dense_matrix(nr, nc, reinterpret_cast<double*>(ptr), byrow);
 
     } else if (std::strcmp(type, "float32") == 0) {
-        return initialize_dense_matrix(nr, nc, reinterpret_cast<float*>(ptr));
+        return initialize_dense_matrix(nr, nc, reinterpret_cast<float*>(ptr), byrow);
 
     } else if (std::strcmp(type, "int64") == 0) {
-        return initialize_dense_matrix(nr, nc, reinterpret_cast<int64_t*>(ptr));
+        return initialize_dense_matrix(nr, nc, reinterpret_cast<int64_t*>(ptr), byrow);
 
     } else if (std::strcmp(type, "int32") == 0) {
-        return initialize_dense_matrix(nr, nc, reinterpret_cast<int32_t*>(ptr));
+        return initialize_dense_matrix(nr, nc, reinterpret_cast<int32_t*>(ptr), byrow);
 
     } else if (std::strcmp(type, "int16") == 0) {
-        return initialize_dense_matrix(nr, nc, reinterpret_cast<int16_t*>(ptr));
+        return initialize_dense_matrix(nr, nc, reinterpret_cast<int16_t*>(ptr), byrow);
 
     } else if (std::strcmp(type, "int8") == 0) {
-        return initialize_dense_matrix(nr, nc, reinterpret_cast<int8_t*>(ptr));
+        return initialize_dense_matrix(nr, nc, reinterpret_cast<int8_t*>(ptr), byrow);
 
     } else if (std::strcmp(type, "uint64") == 0) {
-        return initialize_dense_matrix(nr, nc, reinterpret_cast<uint64_t*>(ptr));
+        return initialize_dense_matrix(nr, nc, reinterpret_cast<uint64_t*>(ptr), byrow);
 
     } else if (std::strcmp(type, "uint32") == 0) {
-        return initialize_dense_matrix(nr, nc, reinterpret_cast<uint32_t*>(ptr));
+        return initialize_dense_matrix(nr, nc, reinterpret_cast<uint32_t*>(ptr), byrow);
 
     } else if (std::strcmp(type, "uint16") == 0) {
-        return initialize_dense_matrix(nr, nc, reinterpret_cast<uint16_t*>(ptr));
+        return initialize_dense_matrix(nr, nc, reinterpret_cast<uint16_t*>(ptr), byrow);
 
     } else if (std::strcmp(type, "uint8") == 0) {
-        return initialize_dense_matrix(nr, nc, reinterpret_cast<uint8_t*>(ptr));
+        return initialize_dense_matrix(nr, nc, reinterpret_cast<uint8_t*>(ptr), byrow);
     }
 
     throw std::runtime_error("unrecognized array type '" + std::string(type) + "' for dense matrix initialization");
     return NULL;
 }
 
 }
-
```

### Comparing `mattress-0.0.4/src/mattress/utils.py` & `mattress-0.0.5/src/mattress/utils.py`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/src/mattress.egg-info/PKG-INFO` & `mattress-0.0.5/src/mattress.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mattress
-Version: 0.0.4
+Version: 0.0.5
 Summary: all your matrix representations belong here!
 Home-page: https://github.com/biocpy/mattress
 Author: "Jayaram Kancherla, Aaron Lun"
 Author-email: jayaram.kancherla@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/biocpy/mattress
 Platform: any
```

### Comparing `mattress-0.0.4/src/mattress.egg-info/SOURCES.txt` & `mattress-0.0.5/src/mattress.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 src/mattress/extern/tatami/include/tatami/base/Extractor.hpp
 src/mattress/extern/tatami/include/tatami/base/Matrix.hpp
 src/mattress/extern/tatami/include/tatami/base/Options.hpp
 src/mattress/extern/tatami/include/tatami/base/SparseRange.hpp
 src/mattress/extern/tatami/include/tatami/base/utils.hpp
 src/mattress/extern/tatami/include/tatami/dense/DenseMatrix.hpp
 src/mattress/extern/tatami/include/tatami/dense/VirtualDenseMatrix.hpp
+src/mattress/extern/tatami/include/tatami/dense/convert_to_dense.hpp
 src/mattress/extern/tatami/include/tatami/isometric/arith_utils.hpp
 src/mattress/extern/tatami/include/tatami/isometric/boolean_utils.hpp
 src/mattress/extern/tatami/include/tatami/isometric/compare_utils.hpp
 src/mattress/extern/tatami/include/tatami/isometric/binary/DelayedBinaryIsometricOp.hpp
 src/mattress/extern/tatami/include/tatami/isometric/binary/arith_helpers.hpp
 src/mattress/extern/tatami/include/tatami/isometric/binary/boolean_helpers.hpp
 src/mattress/extern/tatami/include/tatami/isometric/binary/compare_helpers.hpp
@@ -95,14 +96,15 @@
 src/mattress/extern/tatami/include/tatami/subset/DelayedSubsetBlock.hpp
 src/mattress/extern/tatami/include/tatami/subset/DelayedSubsetSorted.hpp
 src/mattress/extern/tatami/include/tatami/subset/DelayedSubsetSortedUnique.hpp
 src/mattress/extern/tatami/include/tatami/subset/DelayedSubsetUnique.hpp
 src/mattress/extern/tatami/include/tatami/subset/make_DelayedSubset.hpp
 src/mattress/extern/tatami/include/tatami/subset/utils.hpp
 src/mattress/extern/tatami/include/tatami/utils/ArrayView.hpp
+src/mattress/extern/tatami/include/tatami/utils/ElementType.hpp
 src/mattress/extern/tatami/include/tatami/utils/Oracles.hpp
 src/mattress/extern/tatami/include/tatami/utils/SomeNumericArray.hpp
 src/mattress/extern/tatami/include/tatami/utils/bind_intersection.hpp
 src/mattress/extern/tatami/include/tatami/utils/compress_sparse_triplets.hpp
 src/mattress/extern/tatami/include/tatami/utils/convert_to_dense.hpp
 src/mattress/extern/tatami/include/tatami/utils/convert_to_sparse.hpp
 src/mattress/extern/tatami/include/tatami/utils/process_consecutive_indices.hpp
@@ -114,14 +116,15 @@
 src/mattress/extern/tatami/include/tatami_test/test_column_access.hpp
 src/mattress/extern/tatami/include/tatami_test/test_oracle_access.hpp
 src/mattress/extern/tatami/include/tatami_test/test_row_access.hpp
 src/mattress/extern/tatami/include/tatami_test/utils.hpp
 src/mattress/extern/tatami/tests/CMakeLists.txt
 src/mattress/extern/tatami/tests/README.md
 src/mattress/extern/tatami/tests/src/dense/DenseMatrix.cpp
+src/mattress/extern/tatami/tests/src/dense/convert_to_dense.cpp
 src/mattress/extern/tatami/tests/src/isometric/utils.h
 src/mattress/extern/tatami/tests/src/isometric/binary/arith_helpers.cpp
 src/mattress/extern/tatami/tests/src/isometric/binary/boolean_helpers.cpp
 src/mattress/extern/tatami/tests/src/isometric/binary/compare_helpers.cpp
 src/mattress/extern/tatami/tests/src/isometric/unary/arith_scalar_helpers.cpp
 src/mattress/extern/tatami/tests/src/isometric/unary/arith_vector_helpers.cpp
 src/mattress/extern/tatami/tests/src/isometric/unary/boolean_scalar_helpers.cpp
@@ -147,15 +150,14 @@
 src/mattress/extern/tatami/tests/src/subset/DelayedSubset.cpp
 src/mattress/extern/tatami/tests/src/subset/DelayedSubsetBlock.cpp
 src/mattress/extern/tatami/tests/src/utils/ArrayView.cpp
 src/mattress/extern/tatami/tests/src/utils/Oracles.cpp
 src/mattress/extern/tatami/tests/src/utils/SomeNumericArray.cpp
 src/mattress/extern/tatami/tests/src/utils/bind_intersection.cpp
 src/mattress/extern/tatami/tests/src/utils/compress_sparse_triplets.cpp
-src/mattress/extern/tatami/tests/src/utils/convert_to_dense.cpp
 src/mattress/extern/tatami/tests/src/utils/process_consecutive_indices.cpp
 src/mattress/extern/tatami/tests/src/utils/wrap_shared_ptr.cpp
 src/mattress/extern/tatami_hdf5/.git
 src/mattress/extern/tatami_hdf5/.gitignore
 src/mattress/extern/tatami_hdf5/CMakeLists.txt
 src/mattress/extern/tatami_hdf5/LICENSE
 src/mattress/extern/tatami_hdf5/README.md
```

### Comparing `mattress-0.0.4/tests/test_sparse.py` & `mattress-0.0.5/tests/test_sparse.py`

 * *Files identical despite different names*

### Comparing `mattress-0.0.4/tox.ini` & `mattress-0.0.5/tox.ini`

 * *Files identical despite different names*

