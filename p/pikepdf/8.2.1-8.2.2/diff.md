# Comparing `tmp/pikepdf-8.2.1.tar.gz` & `tmp/pikepdf-8.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pikepdf-8.2.1.tar", last modified: Sun Jul 23 08:28:49 2023, max compression
+gzip compressed data, was "pikepdf-8.2.2.tar", last modified: Sat Jul 29 21:22:58 2023, max compression
```

## Comparing `pikepdf-8.2.1.tar` & `pikepdf-8.2.2.tar`

### file list

```diff
@@ -1,130 +1,191 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-23 08:28:49.359531 pikepdf-8.2.1/
--rw-r--r--   0 runner    (1001) docker     (122)    16725 2023-07-23 08:25:31.000000 pikepdf-8.2.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      122 2023-07-23 08:25:31.000000 pikepdf-8.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     6958 2023-07-23 08:28:49.359531 pikepdf-8.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5821 2023-07-23 08:25:31.000000 pikepdf-8.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     5978 2023-07-23 08:25:31.000000 pikepdf-8.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-23 08:28:49.359531 pikepdf-8.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     3856 2023-07-23 08:25:31.000000 pikepdf-8.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-23 08:28:49.331531 pikepdf-8.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-23 08:28:49.339531 pikepdf-8.2.1/src/core/
--rw-r--r--   0 runner    (1001) docker     (122)     4478 2023-07-23 08:25:31.000000 pikepdf-8.2.1/src/core/annotation.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     7216 2023-07-23 08:25:31.000000 pikepdf-8.2.1/src/core/embeddedfiles.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3953 2023-07-23 08:25:31.000000 pikepdf-8.2.1/src/core/jbig2-inl.h
--rw-r--r--   0 runner    (1001) docker     (122)     5806 2023-07-23 08:25:31.000000 pikepdf-8.2.1/src/core/job.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2256 2023-07-23 08:25:31.000000 pikepdf-8.2.1/src/core/logger.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     5731 2023-07-23 08:25:31.000000 pikepdf-8.2.1/src/core/mmap_inputsource-inl.h
--rw-r--r--   0 runner    (1001) docker     (122)     3621 2023-07-23 08:25:31.000000 pikepdf-8.2.1/src/core/nametree.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3001 2023-07-23 08:25:31.000000 pikepdf-8.2.1/src/core/numbertree.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    42072 2023-07-23 08:25:31.000000 pikepdf-8.2.1/src/core/object.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     5786 2023-07-23 08:25:31.000000 pikepdf-8.2.1/src/core/object_convert.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    10569 2023-07-23 08:25:31.000000 pikepdf-8.2.1/src/core/object_repr.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    14256 2023-07-23 08:25:31.000000 pikepdf-8.2.1/src/core/page.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    11199 2023-07-23 08:25:31.000000 pikepdf-8.2.1/src/core/parsers.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2156 2023-07-23 08:25:31.000000 pikepdf-8.2.1/src/core/parsers.h
--rw-r--r--   0 runner    (1001) docker     (122)     8253 2023-07-23 08:25:31.000000 pikepdf-8.2.1/src/core/pikepdf.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     5700 2023-07-23 08:25:31.000000 pikepdf-8.2.1/src/core/pikepdf.h
--rw-r--r--   0 runner    (1001) docker     (122)     1274 2023-07-23 08:25:31.000000 pikepdf-8.2.1/src/core/pipeline.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-07-23 08:25:31.000000 pikepdf-8.2.1/src/core/pipeline.h
--rw-r--r--   0 runner    (1001) docker     (122)    37394 2023-07-23 08:25:31.000000 pikepdf-8.2.1/src/core/qpdf.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     5594 2023-07-23 08:25:31.000000 pikepdf-8.2.1/src/core/qpdf_inputsource-inl.h
--rw-r--r--   0 runner    (1001) docker     (122)    15512 2023-07-23 08:25:31.000000 pikepdf-8.2.1/src/core/qpdf_pagelist.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1144 2023-07-23 08:25:31.000000 pikepdf-8.2.1/src/core/qpdf_pagelist.h
--rw-r--r--   0 runner    (1001) docker     (122)     3901 2023-07-23 08:25:31.000000 pikepdf-8.2.1/src/core/rectangle.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     5455 2023-07-23 08:25:31.000000 pikepdf-8.2.1/src/core/tokenfilter.cpp
--rw-r--r--   0 runner    (1001) docker     (122)      595 2023-07-23 08:25:31.000000 pikepdf-8.2.1/src/core/utils.cpp
--rw-r--r--   0 runner    (1001) docker     (122)      565 2023-07-23 08:25:31.000000 pikepdf-8.2.1/src/core/utils.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-23 08:28:49.339531 pikepdf-8.2.1/src/pikepdf/
--rw-r--r--   0 runner    (1001) docker     (122)     3001 2023-07-23 08:25:31.000000 pikepdf-8.2.1/src/pikepdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6161 2023-07-23 08:25:31.000000 pikepdf-8.2.1/src/pikepdf/_augments.py
--rw-r--r--   0 runner    (1001) docker     (122)     3030 2023-07-23 08:25:31.000000 pikepdf-8.2.1/src/pikepdf/_cpphelpers.py
--rw-r--r--   0 runner    (1001) docker     (122)      232 2023-07-23 08:25:31.000000 pikepdf-8.2.1/src/pikepdf/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1666 2023-07-23 08:25:31.000000 pikepdf-8.2.1/src/pikepdf/_io.py
--rw-r--r--   0 runner    (1001) docker     (122)    57488 2023-07-23 08:25:31.000000 pikepdf-8.2.1/src/pikepdf/_methods.py
--rw-r--r--   0 runner    (1001) docker     (122)     1876 2023-07-23 08:25:31.000000 pikepdf-8.2.1/src/pikepdf/_qpdf.py
--rw-r--r--   0 runner    (1001) docker     (122)      879 2023-07-23 08:25:31.000000 pikepdf-8.2.1/src/pikepdf/_xml.py
--rw-r--r--   0 runner    (1001) docker     (122)     5952 2023-07-23 08:25:31.000000 pikepdf-8.2.1/src/pikepdf/codec.py
--rw-r--r--   0 runner    (1001) docker     (122)     3378 2023-07-23 08:25:31.000000 pikepdf-8.2.1/src/pikepdf/jbig2.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-23 08:28:49.343531 pikepdf-8.2.1/src/pikepdf/models/
--rw-r--r--   0 runner    (1001) docker     (122)     1139 2023-07-23 08:25:31.000000 pikepdf-8.2.1/src/pikepdf/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4950 2023-07-23 08:25:31.000000 pikepdf-8.2.1/src/pikepdf/models/_content_stream.py
--rw-r--r--   0 runner    (1001) docker     (122)     8204 2023-07-23 08:25:31.000000 pikepdf-8.2.1/src/pikepdf/models/_transcoding.py
--rw-r--r--   0 runner    (1001) docker     (122)     5499 2023-07-23 08:25:31.000000 pikepdf-8.2.1/src/pikepdf/models/encryption.py
--rw-r--r--   0 runner    (1001) docker     (122)    36349 2023-07-23 08:25:31.000000 pikepdf-8.2.1/src/pikepdf/models/image.py
--rw-r--r--   0 runner    (1001) docker     (122)     5979 2023-07-23 08:25:31.000000 pikepdf-8.2.1/src/pikepdf/models/matrix.py
--rw-r--r--   0 runner    (1001) docker     (122)    32023 2023-07-23 08:25:31.000000 pikepdf-8.2.1/src/pikepdf/models/metadata.py
--rw-r--r--   0 runner    (1001) docker     (122)    15420 2023-07-23 08:25:31.000000 pikepdf-8.2.1/src/pikepdf/models/outlines.py
--rw-r--r--   0 runner    (1001) docker     (122)    10415 2023-07-23 08:25:31.000000 pikepdf-8.2.1/src/pikepdf/objects.py
--rw-r--r--   0 runner    (1001) docker     (122)      101 2023-07-23 08:25:31.000000 pikepdf-8.2.1/src/pikepdf/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)      369 2023-07-23 08:25:31.000000 pikepdf-8.2.1/src/pikepdf/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-23 08:28:49.343531 pikepdf-8.2.1/src/pikepdf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     6958 2023-07-23 08:28:49.000000 pikepdf-8.2.1/src/pikepdf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3097 2023-07-23 08:28:49.000000 pikepdf-8.2.1/src/pikepdf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-23 08:28:49.000000 pikepdf-8.2.1/src/pikepdf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      688 2023-07-23 08:28:49.000000 pikepdf-8.2.1/src/pikepdf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-07-23 08:28:49.000000 pikepdf-8.2.1/src/pikepdf.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-23 08:28:49.351531 pikepdf-8.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     1731 2023-07-23 08:25:31.000000 pikepdf-8.2.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-23 08:28:49.359531 pikepdf-8.2.1/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (122)     5661 2023-07-23 08:25:31.000000 pikepdf-8.2.1/tests/resources/1biticc.pdf
--rw-r--r--   0 runner    (1001) docker     (122)      420 2023-07-23 08:25:31.000000 pikepdf-8.2.1/tests/resources/Gray.icc
--rw-r--r--   0 runner    (1001) docker     (122)     1734 2023-07-23 08:25:31.000000 pikepdf-8.2.1/tests/resources/aquamarine-cie.pdf
--rw-r--r--   0 runner    (1001) docker     (122)     1940 2023-07-23 08:25:31.000000 pikepdf-8.2.1/tests/resources/aquamarine-cie.png
--rw-r--r--   0 runner    (1001) docker     (122)     1461 2023-07-23 08:25:31.000000 pikepdf-8.2.1/tests/resources/cmyk-jpeg.pdf
--rw-r--r--   0 runner    (1001) docker     (122)    97969 2023-07-23 08:25:31.000000 pikepdf-8.2.1/tests/resources/congress-gray.pdf
--rw-r--r--   0 runner    (1001) docker     (122)   193947 2023-07-23 08:25:31.000000 pikepdf-8.2.1/tests/resources/congress.pdf
--rw-r--r--   0 runner    (1001) docker     (122)     2889 2023-07-23 08:25:31.000000 pikepdf-8.2.1/tests/resources/content-stream-errors.pdf
--rw-r--r--   0 runner    (1001) docker     (122)    10876 2023-07-23 08:25:31.000000 pikepdf-8.2.1/tests/resources/form.pdf
--rw-r--r--   0 runner    (1001) docker     (122)     2713 2023-07-23 08:25:31.000000 pikepdf-8.2.1/tests/resources/formxobject.pdf
--rw-r--r--   0 runner    (1001) docker     (122)     2916 2023-07-23 08:25:31.000000 pikepdf-8.2.1/tests/resources/fourpages.pdf
--rw-r--r--   0 runner    (1001) docker     (122)   296661 2023-07-23 08:25:31.000000 pikepdf-8.2.1/tests/resources/graph-encrypted.pdf
--rw-r--r--   0 runner    (1001) docker     (122)   296322 2023-07-23 08:25:31.000000 pikepdf-8.2.1/tests/resources/graph.pdf
--rw-r--r--   0 runner    (1001) docker     (122)     1544 2023-07-23 08:25:31.000000 pikepdf-8.2.1/tests/resources/image-mono-inline.pdf
--rw-r--r--   0 runner    (1001) docker     (122)      965 2023-07-23 08:25:31.000000 pikepdf-8.2.1/tests/resources/invalid_creationdate.pdf
--rw-r--r--   0 runner    (1001) docker     (122)    20306 2023-07-23 08:25:31.000000 pikepdf-8.2.1/tests/resources/jbig2.pdf
--rw-r--r--   0 runner    (1001) docker     (122)    60332 2023-07-23 08:25:31.000000 pikepdf-8.2.1/tests/resources/jbig2global.pdf
--rw-r--r--   0 runner    (1001) docker     (122)     6994 2023-07-23 08:25:31.000000 pikepdf-8.2.1/tests/resources/outlines.pdf
--rw-r--r--   0 runner    (1001) docker     (122)      931 2023-07-23 08:25:31.000000 pikepdf-8.2.1/tests/resources/pal-1bit-rgb.pdf
--rw-r--r--   0 runner    (1001) docker     (122)      931 2023-07-23 08:25:31.000000 pikepdf-8.2.1/tests/resources/pal-1bit-trivial.pdf
--rw-r--r--   0 runner    (1001) docker     (122)     2918 2023-07-23 08:25:31.000000 pikepdf-8.2.1/tests/resources/pal.pdf
--rwxr-xr-x   0 runner    (1001) docker     (122)   533953 2023-07-23 08:25:31.000000 pikepdf-8.2.1/tests/resources/pdfx.pdf
--rw-r--r--   0 runner    (1001) docker     (122)    18471 2023-07-23 08:25:31.000000 pikepdf-8.2.1/tests/resources/pike-flate-jp2.pdf
--rw-r--r--   0 runner    (1001) docker     (122)    18152 2023-07-23 08:25:31.000000 pikepdf-8.2.1/tests/resources/pike-jp2.pdf
--rw-r--r--   0 runner    (1001) docker     (122)     2681 2023-07-23 08:25:31.000000 pikepdf-8.2.1/tests/resources/pink-palette-icc.pdf
--rw-r--r--   0 runner    (1001) docker     (122)     2698 2023-07-23 08:25:31.000000 pikepdf-8.2.1/tests/resources/pink-palette-icc.png
--rw-r--r--   0 runner    (1001) docker     (122)     5432 2023-07-23 08:25:31.000000 pikepdf-8.2.1/tests/resources/rle.pdf
--rw-r--r--   0 runner    (1001) docker     (122)   115546 2023-07-23 08:25:31.000000 pikepdf-8.2.1/tests/resources/sandwich.pdf
--rw-r--r--   0 runner    (1001) docker     (122)    10049 2023-07-23 08:25:31.000000 pikepdf-8.2.1/tests/resources/veraPDF test suite 6-2-10-t02-pass-a.pdf
--rw-r--r--   0 runner    (1001) docker     (122)     2676 2023-07-23 08:25:31.000000 pikepdf-8.2.1/tests/resources/veraPDF test suite 6-2-3-3-t01-fail-c.pdf
--rw-r--r--   0 runner    (1001) docker     (122)     1439 2023-07-23 08:25:31.000000 pikepdf-8.2.1/tests/test_annotation.py
--rw-r--r--   0 runner    (1001) docker     (122)     4721 2023-07-23 08:25:31.000000 pikepdf-8.2.1/tests/test_attachments.py
--rw-r--r--   0 runner    (1001) docker     (122)     1312 2023-07-23 08:25:31.000000 pikepdf-8.2.1/tests/test_augments.py
--rw-r--r--   0 runner    (1001) docker     (122)     4453 2023-07-23 08:25:31.000000 pikepdf-8.2.1/tests/test_codec.py
--rw-r--r--   0 runner    (1001) docker     (122)     1961 2023-07-23 08:25:31.000000 pikepdf-8.2.1/tests/test_decimal.py
--rw-r--r--   0 runner    (1001) docker     (122)     1181 2023-07-23 08:25:31.000000 pikepdf-8.2.1/tests/test_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (122)     5610 2023-07-23 08:25:31.000000 pikepdf-8.2.1/tests/test_encrypt.py
--rw-r--r--   0 runner    (1001) docker     (122)     1690 2023-07-23 08:25:31.000000 pikepdf-8.2.1/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (122)     3404 2023-07-23 08:25:31.000000 pikepdf-8.2.1/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (122)     3135 2023-07-23 08:25:31.000000 pikepdf-8.2.1/tests/test_foreign.py
--rw-r--r--   0 runner    (1001) docker     (122)     1988 2023-07-23 08:25:31.000000 pikepdf-8.2.1/tests/test_formxobject.py
--rw-r--r--   0 runner    (1001) docker     (122)    36948 2023-07-23 08:25:31.000000 pikepdf-8.2.1/tests/test_image_access.py
--rw-r--r--   0 runner    (1001) docker     (122)     9944 2023-07-23 08:25:31.000000 pikepdf-8.2.1/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (122)     2498 2023-07-23 08:25:31.000000 pikepdf-8.2.1/tests/test_ipython.py
--rw-r--r--   0 runner    (1001) docker     (122)     2036 2023-07-23 08:25:31.000000 pikepdf-8.2.1/tests/test_job.py
--rw-r--r--   0 runner    (1001) docker     (122)     1523 2023-07-23 08:25:31.000000 pikepdf-8.2.1/tests/test_matrix.py
--rw-r--r--   0 runner    (1001) docker     (122)    25184 2023-07-23 08:25:31.000000 pikepdf-8.2.1/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (122)     2094 2023-07-23 08:25:31.000000 pikepdf-8.2.1/tests/test_nametree.py
--rw-r--r--   0 runner    (1001) docker     (122)     2301 2023-07-23 08:25:31.000000 pikepdf-8.2.1/tests/test_numbertree.py
--rw-r--r--   0 runner    (1001) docker     (122)    22294 2023-07-23 08:25:31.000000 pikepdf-8.2.1/tests/test_object.py
--rw-r--r--   0 runner    (1001) docker     (122)      565 2023-07-23 08:25:31.000000 pikepdf-8.2.1/tests/test_objectlist.py
--rw-r--r--   0 runner    (1001) docker     (122)    17177 2023-07-23 08:25:31.000000 pikepdf-8.2.1/tests/test_outlines.py
--rw-r--r--   0 runner    (1001) docker     (122)     9131 2023-07-23 08:25:31.000000 pikepdf-8.2.1/tests/test_page.py
--rw-r--r--   0 runner    (1001) docker     (122)    15569 2023-07-23 08:25:31.000000 pikepdf-8.2.1/tests/test_pages.py
--rw-r--r--   0 runner    (1001) docker     (122)     9522 2023-07-23 08:25:31.000000 pikepdf-8.2.1/tests/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (122)    13773 2023-07-23 08:25:31.000000 pikepdf-8.2.1/tests/test_pdf.py
--rw-r--r--   0 runner    (1001) docker     (122)     3956 2023-07-23 08:25:31.000000 pikepdf-8.2.1/tests/test_pdfa.py
--rw-r--r--   0 runner    (1001) docker     (122)      754 2023-07-23 08:25:31.000000 pikepdf-8.2.1/tests/test_private_pdfs.py
--rw-r--r--   0 runner    (1001) docker     (122)     1393 2023-07-23 08:25:31.000000 pikepdf-8.2.1/tests/test_rectangle.py
--rw-r--r--   0 runner    (1001) docker     (122)     2032 2023-07-23 08:25:31.000000 pikepdf-8.2.1/tests/test_refcount.py
--rw-r--r--   0 runner    (1001) docker     (122)     3744 2023-07-23 08:25:31.000000 pikepdf-8.2.1/tests/test_repr.py
--rw-r--r--   0 runner    (1001) docker     (122)     4682 2023-07-23 08:25:31.000000 pikepdf-8.2.1/tests/test_sanity.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-29 21:22:58.287057 pikepdf-8.2.2/
+-rw-r--r--   0 runner    (1001) docker     (122)    16725 2023-07-29 21:20:23.000000 pikepdf-8.2.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      151 2023-07-29 21:20:23.000000 pikepdf-8.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     6958 2023-07-29 21:22:58.287057 pikepdf-8.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5821 2023-07-29 21:20:23.000000 pikepdf-8.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-29 21:22:58.255057 pikepdf-8.2.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     7687 2023-07-29 21:20:23.000000 pikepdf-8.2.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-29 21:22:58.255057 pikepdf-8.2.2/docs/_ext/
+-rw-r--r--   0 runner    (1001) docker     (122)     1477 2023-07-29 21:20:23.000000 pikepdf-8.2.2/docs/_ext/fix_pybind11_autodoc.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-29 21:22:58.255057 pikepdf-8.2.2/docs/_notebooks/
+-rw-r--r--   0 runner    (1001) docker     (122)     6560 2023-07-29 21:20:23.000000 pikepdf-8.2.2/docs/_notebooks/pages.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-29 21:22:58.255057 pikepdf-8.2.2/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (122)     1216 2023-07-29 21:20:23.000000 pikepdf-8.2.2/docs/api/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2879 2023-07-29 21:20:23.000000 pikepdf-8.2.2/docs/api/filters.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6429 2023-07-29 21:20:23.000000 pikepdf-8.2.2/docs/api/main.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     8520 2023-07-29 21:20:23.000000 pikepdf-8.2.2/docs/api/models.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      248 2023-07-29 21:20:23.000000 pikepdf-8.2.2/docs/api/settings.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      397 2023-07-29 21:20:23.000000 pikepdf-8.2.2/docs/binary-wheels.csv
+-rw-r--r--   0 runner    (1001) docker     (122)    12962 2023-07-29 21:20:23.000000 pikepdf-8.2.2/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-29 21:22:58.259057 pikepdf-8.2.2/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (122)   543264 2023-07-29 21:20:23.000000 pikepdf-8.2.2/docs/images/28fish.jpg
+-rw-r--r--   0 runner    (1001) docker     (122)     8489 2023-07-29 21:20:23.000000 pikepdf-8.2.2/docs/images/acrobat-attachments.png
+-rw-r--r--   0 runner    (1001) docker     (122)    26172 2023-07-29 21:20:23.000000 pikepdf-8.2.2/docs/images/congress_im0.jpg
+-rw-r--r--   0 runner    (1001) docker     (122)     2983 2023-07-29 21:20:23.000000 pikepdf-8.2.2/docs/images/pdfcoords.svg
+-rw-r--r--   0 runner    (1001) docker     (122)   148388 2023-07-29 21:20:23.000000 pikepdf-8.2.2/docs/images/pike-cartoon.png
+-rw-r--r--   0 runner    (1001) docker     (122)    88609 2023-07-29 21:20:23.000000 pikepdf-8.2.2/docs/images/pike-release.jpg
+-rw-r--r--   0 runner    (1001) docker     (122)    32321 2023-07-29 21:20:23.000000 pikepdf-8.2.2/docs/images/pike.png
+-rw-r--r--   0 runner    (1001) docker     (122)    29276 2023-07-29 21:20:23.000000 pikepdf-8.2.2/docs/images/pikemen.jpg
+-rw-r--r--   0 runner    (1001) docker     (122)    65692 2023-07-29 21:20:23.000000 pikepdf-8.2.2/docs/images/save-pike.jpg
+-rw-r--r--   0 runner    (1001) docker     (122)   155993 2023-07-29 21:20:23.000000 pikepdf-8.2.2/docs/images/sushi.jpg
+-rw-r--r--   0 runner    (1001) docker     (122)     5616 2023-07-29 21:20:23.000000 pikepdf-8.2.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     9265 2023-07-29 21:20:23.000000 pikepdf-8.2.2/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     7265 2023-07-29 21:20:23.000000 pikepdf-8.2.2/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-29 21:22:58.263057 pikepdf-8.2.2/docs/references/
+-rw-r--r--   0 runner    (1001) docker     (122)     1960 2023-07-29 21:20:23.000000 pikepdf-8.2.2/docs/references/arch.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2839 2023-07-29 21:20:23.000000 pikepdf-8.2.2/docs/references/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     4513 2023-07-29 21:20:23.000000 pikepdf-8.2.2/docs/references/debugging.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      788 2023-07-29 21:20:23.000000 pikepdf-8.2.2/docs/references/resources.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-29 21:22:58.263057 pikepdf-8.2.2/docs/releasenotes/
+-rw-r--r--   0 runner    (1001) docker     (122)      605 2023-07-29 21:20:23.000000 pikepdf-8.2.2/docs/releasenotes/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6421 2023-07-29 21:20:23.000000 pikepdf-8.2.2/docs/releasenotes/version0.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    17003 2023-07-29 21:20:23.000000 pikepdf-8.2.2/docs/releasenotes/version1.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    13480 2023-07-29 21:20:23.000000 pikepdf-8.2.2/docs/releasenotes/version2.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3972 2023-07-29 21:20:23.000000 pikepdf-8.2.2/docs/releasenotes/version3.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3768 2023-07-29 21:20:23.000000 pikepdf-8.2.2/docs/releasenotes/version4.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     4745 2023-07-29 21:20:23.000000 pikepdf-8.2.2/docs/releasenotes/version5.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2034 2023-07-29 21:20:23.000000 pikepdf-8.2.2/docs/releasenotes/version6.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3272 2023-07-29 21:20:23.000000 pikepdf-8.2.2/docs/releasenotes/version7.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2047 2023-07-29 21:20:23.000000 pikepdf-8.2.2/docs/releasenotes/version8.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      549 2023-07-29 21:20:23.000000 pikepdf-8.2.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-29 21:22:58.267057 pikepdf-8.2.2/docs/topics/
+-rw-r--r--   0 runner    (1001) docker     (122)     3429 2023-07-29 21:20:23.000000 pikepdf-8.2.2/docs/topics/attachments.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     7605 2023-07-29 21:20:23.000000 pikepdf-8.2.2/docs/topics/content_streams.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2730 2023-07-29 21:20:23.000000 pikepdf-8.2.2/docs/topics/encoding.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6010 2023-07-29 21:20:23.000000 pikepdf-8.2.2/docs/topics/images.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6187 2023-07-29 21:20:23.000000 pikepdf-8.2.2/docs/topics/metadata.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-07-29 21:20:23.000000 pikepdf-8.2.2/docs/topics/nametrees.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     5525 2023-07-29 21:20:23.000000 pikepdf-8.2.2/docs/topics/objects.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3083 2023-07-29 21:20:23.000000 pikepdf-8.2.2/docs/topics/outlines.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2661 2023-07-29 21:20:23.000000 pikepdf-8.2.2/docs/topics/overlays.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1963 2023-07-29 21:20:23.000000 pikepdf-8.2.2/docs/topics/page.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1887 2023-07-29 21:20:23.000000 pikepdf-8.2.2/docs/topics/pagelayout.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     8077 2023-07-29 21:20:23.000000 pikepdf-8.2.2/docs/topics/pages.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2689 2023-07-29 21:20:23.000000 pikepdf-8.2.2/docs/topics/security.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3409 2023-07-29 21:20:23.000000 pikepdf-8.2.2/docs/topics/streams.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     8468 2023-07-29 21:20:23.000000 pikepdf-8.2.2/docs/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     5978 2023-07-29 21:20:23.000000 pikepdf-8.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-29 21:22:58.287057 pikepdf-8.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     3856 2023-07-29 21:20:23.000000 pikepdf-8.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-29 21:22:58.247057 pikepdf-8.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-29 21:22:58.275057 pikepdf-8.2.2/src/core/
+-rw-r--r--   0 runner    (1001) docker     (122)     4478 2023-07-29 21:20:23.000000 pikepdf-8.2.2/src/core/annotation.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     7216 2023-07-29 21:20:23.000000 pikepdf-8.2.2/src/core/embeddedfiles.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3953 2023-07-29 21:20:23.000000 pikepdf-8.2.2/src/core/jbig2-inl.h
+-rw-r--r--   0 runner    (1001) docker     (122)     5806 2023-07-29 21:20:23.000000 pikepdf-8.2.2/src/core/job.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2256 2023-07-29 21:20:23.000000 pikepdf-8.2.2/src/core/logger.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5731 2023-07-29 21:20:23.000000 pikepdf-8.2.2/src/core/mmap_inputsource-inl.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3621 2023-07-29 21:20:23.000000 pikepdf-8.2.2/src/core/nametree.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3001 2023-07-29 21:20:23.000000 pikepdf-8.2.2/src/core/numbertree.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    42072 2023-07-29 21:20:23.000000 pikepdf-8.2.2/src/core/object.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5786 2023-07-29 21:20:23.000000 pikepdf-8.2.2/src/core/object_convert.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    10569 2023-07-29 21:20:23.000000 pikepdf-8.2.2/src/core/object_repr.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    14256 2023-07-29 21:20:23.000000 pikepdf-8.2.2/src/core/page.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    11199 2023-07-29 21:20:23.000000 pikepdf-8.2.2/src/core/parsers.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2156 2023-07-29 21:20:23.000000 pikepdf-8.2.2/src/core/parsers.h
+-rw-r--r--   0 runner    (1001) docker     (122)     8253 2023-07-29 21:20:23.000000 pikepdf-8.2.2/src/core/pikepdf.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5700 2023-07-29 21:20:23.000000 pikepdf-8.2.2/src/core/pikepdf.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1274 2023-07-29 21:20:23.000000 pikepdf-8.2.2/src/core/pipeline.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-07-29 21:20:23.000000 pikepdf-8.2.2/src/core/pipeline.h
+-rw-r--r--   0 runner    (1001) docker     (122)    37394 2023-07-29 21:20:23.000000 pikepdf-8.2.2/src/core/qpdf.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5594 2023-07-29 21:20:23.000000 pikepdf-8.2.2/src/core/qpdf_inputsource-inl.h
+-rw-r--r--   0 runner    (1001) docker     (122)    15512 2023-07-29 21:20:23.000000 pikepdf-8.2.2/src/core/qpdf_pagelist.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1144 2023-07-29 21:20:23.000000 pikepdf-8.2.2/src/core/qpdf_pagelist.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3901 2023-07-29 21:20:23.000000 pikepdf-8.2.2/src/core/rectangle.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5455 2023-07-29 21:20:23.000000 pikepdf-8.2.2/src/core/tokenfilter.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      595 2023-07-29 21:20:23.000000 pikepdf-8.2.2/src/core/utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      565 2023-07-29 21:20:23.000000 pikepdf-8.2.2/src/core/utils.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-29 21:22:58.275057 pikepdf-8.2.2/src/pikepdf/
+-rw-r--r--   0 runner    (1001) docker     (122)     3001 2023-07-29 21:20:23.000000 pikepdf-8.2.2/src/pikepdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6161 2023-07-29 21:20:23.000000 pikepdf-8.2.2/src/pikepdf/_augments.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3030 2023-07-29 21:20:23.000000 pikepdf-8.2.2/src/pikepdf/_cpphelpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      232 2023-07-29 21:20:23.000000 pikepdf-8.2.2/src/pikepdf/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1666 2023-07-29 21:20:23.000000 pikepdf-8.2.2/src/pikepdf/_io.py
+-rw-r--r--   0 runner    (1001) docker     (122)    57488 2023-07-29 21:20:23.000000 pikepdf-8.2.2/src/pikepdf/_methods.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1876 2023-07-29 21:20:23.000000 pikepdf-8.2.2/src/pikepdf/_qpdf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      879 2023-07-29 21:20:23.000000 pikepdf-8.2.2/src/pikepdf/_xml.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5952 2023-07-29 21:20:23.000000 pikepdf-8.2.2/src/pikepdf/codec.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3378 2023-07-29 21:20:23.000000 pikepdf-8.2.2/src/pikepdf/jbig2.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-29 21:22:58.279057 pikepdf-8.2.2/src/pikepdf/models/
+-rw-r--r--   0 runner    (1001) docker     (122)     1139 2023-07-29 21:20:23.000000 pikepdf-8.2.2/src/pikepdf/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4950 2023-07-29 21:20:23.000000 pikepdf-8.2.2/src/pikepdf/models/_content_stream.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8204 2023-07-29 21:20:23.000000 pikepdf-8.2.2/src/pikepdf/models/_transcoding.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5499 2023-07-29 21:20:23.000000 pikepdf-8.2.2/src/pikepdf/models/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36349 2023-07-29 21:20:23.000000 pikepdf-8.2.2/src/pikepdf/models/image.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5979 2023-07-29 21:20:23.000000 pikepdf-8.2.2/src/pikepdf/models/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32023 2023-07-29 21:20:23.000000 pikepdf-8.2.2/src/pikepdf/models/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15420 2023-07-29 21:20:23.000000 pikepdf-8.2.2/src/pikepdf/models/outlines.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10415 2023-07-29 21:20:23.000000 pikepdf-8.2.2/src/pikepdf/objects.py
+-rw-r--r--   0 runner    (1001) docker     (122)      101 2023-07-29 21:20:23.000000 pikepdf-8.2.2/src/pikepdf/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)      369 2023-07-29 21:20:23.000000 pikepdf-8.2.2/src/pikepdf/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-29 21:22:58.275057 pikepdf-8.2.2/src/pikepdf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     6958 2023-07-29 21:22:58.000000 pikepdf-8.2.2/src/pikepdf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4447 2023-07-29 21:22:58.000000 pikepdf-8.2.2/src/pikepdf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-29 21:22:58.000000 pikepdf-8.2.2/src/pikepdf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      688 2023-07-29 21:22:58.000000 pikepdf-8.2.2/src/pikepdf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-07-29 21:22:58.000000 pikepdf-8.2.2/src/pikepdf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-29 21:22:58.283057 pikepdf-8.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     1731 2023-07-29 21:20:23.000000 pikepdf-8.2.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-29 21:22:58.287057 pikepdf-8.2.2/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (122)     5661 2023-07-29 21:20:23.000000 pikepdf-8.2.2/tests/resources/1biticc.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)      420 2023-07-29 21:20:23.000000 pikepdf-8.2.2/tests/resources/Gray.icc
+-rw-r--r--   0 runner    (1001) docker     (122)     1734 2023-07-29 21:20:23.000000 pikepdf-8.2.2/tests/resources/aquamarine-cie.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)     1940 2023-07-29 21:20:23.000000 pikepdf-8.2.2/tests/resources/aquamarine-cie.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1461 2023-07-29 21:20:23.000000 pikepdf-8.2.2/tests/resources/cmyk-jpeg.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)    97969 2023-07-29 21:20:23.000000 pikepdf-8.2.2/tests/resources/congress-gray.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)   193947 2023-07-29 21:20:23.000000 pikepdf-8.2.2/tests/resources/congress.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)     2889 2023-07-29 21:20:23.000000 pikepdf-8.2.2/tests/resources/content-stream-errors.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)    10876 2023-07-29 21:20:23.000000 pikepdf-8.2.2/tests/resources/form.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)     2713 2023-07-29 21:20:23.000000 pikepdf-8.2.2/tests/resources/formxobject.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)     2916 2023-07-29 21:20:23.000000 pikepdf-8.2.2/tests/resources/fourpages.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)   296661 2023-07-29 21:20:23.000000 pikepdf-8.2.2/tests/resources/graph-encrypted.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)   296322 2023-07-29 21:20:23.000000 pikepdf-8.2.2/tests/resources/graph.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)     1544 2023-07-29 21:20:23.000000 pikepdf-8.2.2/tests/resources/image-mono-inline.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)      965 2023-07-29 21:20:23.000000 pikepdf-8.2.2/tests/resources/invalid_creationdate.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)    20306 2023-07-29 21:20:23.000000 pikepdf-8.2.2/tests/resources/jbig2.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)    60332 2023-07-29 21:20:23.000000 pikepdf-8.2.2/tests/resources/jbig2global.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)     6994 2023-07-29 21:20:23.000000 pikepdf-8.2.2/tests/resources/outlines.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)      931 2023-07-29 21:20:23.000000 pikepdf-8.2.2/tests/resources/pal-1bit-rgb.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)      931 2023-07-29 21:20:23.000000 pikepdf-8.2.2/tests/resources/pal-1bit-trivial.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)     2918 2023-07-29 21:20:23.000000 pikepdf-8.2.2/tests/resources/pal.pdf
+-rwxr-xr-x   0 runner    (1001) docker     (122)   533953 2023-07-29 21:20:23.000000 pikepdf-8.2.2/tests/resources/pdfx.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)    18471 2023-07-29 21:20:23.000000 pikepdf-8.2.2/tests/resources/pike-flate-jp2.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)    18152 2023-07-29 21:20:23.000000 pikepdf-8.2.2/tests/resources/pike-jp2.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)     2681 2023-07-29 21:20:23.000000 pikepdf-8.2.2/tests/resources/pink-palette-icc.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)     2698 2023-07-29 21:20:23.000000 pikepdf-8.2.2/tests/resources/pink-palette-icc.png
+-rw-r--r--   0 runner    (1001) docker     (122)     5432 2023-07-29 21:20:23.000000 pikepdf-8.2.2/tests/resources/rle.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)   115546 2023-07-29 21:20:23.000000 pikepdf-8.2.2/tests/resources/sandwich.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)    10049 2023-07-29 21:20:23.000000 pikepdf-8.2.2/tests/resources/veraPDF test suite 6-2-10-t02-pass-a.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)     2676 2023-07-29 21:20:23.000000 pikepdf-8.2.2/tests/resources/veraPDF test suite 6-2-3-3-t01-fail-c.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)     1439 2023-07-29 21:20:23.000000 pikepdf-8.2.2/tests/test_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4721 2023-07-29 21:20:23.000000 pikepdf-8.2.2/tests/test_attachments.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1312 2023-07-29 21:20:23.000000 pikepdf-8.2.2/tests/test_augments.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4453 2023-07-29 21:20:23.000000 pikepdf-8.2.2/tests/test_codec.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1961 2023-07-29 21:20:23.000000 pikepdf-8.2.2/tests/test_decimal.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1181 2023-07-29 21:20:23.000000 pikepdf-8.2.2/tests/test_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5610 2023-07-29 21:20:23.000000 pikepdf-8.2.2/tests/test_encrypt.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1690 2023-07-29 21:20:23.000000 pikepdf-8.2.2/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3404 2023-07-29 21:20:23.000000 pikepdf-8.2.2/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3135 2023-07-29 21:20:23.000000 pikepdf-8.2.2/tests/test_foreign.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1988 2023-07-29 21:20:23.000000 pikepdf-8.2.2/tests/test_formxobject.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36948 2023-07-29 21:20:23.000000 pikepdf-8.2.2/tests/test_image_access.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9944 2023-07-29 21:20:23.000000 pikepdf-8.2.2/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2498 2023-07-29 21:20:23.000000 pikepdf-8.2.2/tests/test_ipython.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2036 2023-07-29 21:20:23.000000 pikepdf-8.2.2/tests/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1523 2023-07-29 21:20:23.000000 pikepdf-8.2.2/tests/test_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25184 2023-07-29 21:20:23.000000 pikepdf-8.2.2/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2094 2023-07-29 21:20:23.000000 pikepdf-8.2.2/tests/test_nametree.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2301 2023-07-29 21:20:23.000000 pikepdf-8.2.2/tests/test_numbertree.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22294 2023-07-29 21:20:23.000000 pikepdf-8.2.2/tests/test_object.py
+-rw-r--r--   0 runner    (1001) docker     (122)      565 2023-07-29 21:20:23.000000 pikepdf-8.2.2/tests/test_objectlist.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17177 2023-07-29 21:20:23.000000 pikepdf-8.2.2/tests/test_outlines.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9131 2023-07-29 21:20:23.000000 pikepdf-8.2.2/tests/test_page.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15569 2023-07-29 21:20:23.000000 pikepdf-8.2.2/tests/test_pages.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9522 2023-07-29 21:20:23.000000 pikepdf-8.2.2/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13773 2023-07-29 21:20:23.000000 pikepdf-8.2.2/tests/test_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3956 2023-07-29 21:20:23.000000 pikepdf-8.2.2/tests/test_pdfa.py
+-rw-r--r--   0 runner    (1001) docker     (122)      754 2023-07-29 21:20:23.000000 pikepdf-8.2.2/tests/test_private_pdfs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1393 2023-07-29 21:20:23.000000 pikepdf-8.2.2/tests/test_rectangle.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2032 2023-07-29 21:20:23.000000 pikepdf-8.2.2/tests/test_refcount.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3744 2023-07-29 21:20:23.000000 pikepdf-8.2.2/tests/test_repr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4682 2023-07-29 21:20:23.000000 pikepdf-8.2.2/tests/test_sanity.py
```

### Comparing `pikepdf-8.2.1/LICENSE.txt` & `pikepdf-8.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/PKG-INFO` & `pikepdf-8.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pikepdf
-Version: 8.2.1
+Version: 8.2.2
 Summary: Read and write PDFs with Python, powered by qpdf
 Author-email: "James R. Barlow" <james@purplerock.ca>
 License: MPL-2.0
 Project-URL: documentation, https://pikepdf.readthedocs.io/
 Project-URL: repository, https://github.com/pikepdf/pikepdf
 Project-URL: changelog, https://pikepdf.readthedocs.io/en/latest/releasenotes/index.html
 Keywords: PDF
```

### Comparing `pikepdf-8.2.1/README.md` & `pikepdf-8.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/pyproject.toml` & `pikepdf-8.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
   "wheel >= 0.37",
   "pybind11 >= 2.10.1",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pikepdf"
-version = "8.2.1"
+version = "8.2.2"
 description = "Read and write PDFs with Python, powered by qpdf"
 readme = "README.md"
 requires-python = ">= 3.8"
 keywords = ["PDF"]
 authors = [
   { name = "James R. Barlow", email= "james@purplerock.ca"}
 ]
```

### Comparing `pikepdf-8.2.1/setup.py` & `pikepdf-8.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/src/core/annotation.cpp` & `pikepdf-8.2.2/src/core/annotation.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/src/core/embeddedfiles.cpp` & `pikepdf-8.2.2/src/core/embeddedfiles.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/src/core/jbig2-inl.h` & `pikepdf-8.2.2/src/core/jbig2-inl.h`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/src/core/job.cpp` & `pikepdf-8.2.2/src/core/job.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/src/core/logger.cpp` & `pikepdf-8.2.2/src/core/logger.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/src/core/mmap_inputsource-inl.h` & `pikepdf-8.2.2/src/core/mmap_inputsource-inl.h`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/src/core/nametree.cpp` & `pikepdf-8.2.2/src/core/nametree.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/src/core/numbertree.cpp` & `pikepdf-8.2.2/src/core/numbertree.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/src/core/object.cpp` & `pikepdf-8.2.2/src/core/object.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/src/core/object_convert.cpp` & `pikepdf-8.2.2/src/core/object_convert.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/src/core/object_repr.cpp` & `pikepdf-8.2.2/src/core/object_repr.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/src/core/page.cpp` & `pikepdf-8.2.2/src/core/page.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/src/core/parsers.cpp` & `pikepdf-8.2.2/src/core/parsers.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/src/core/parsers.h` & `pikepdf-8.2.2/src/core/parsers.h`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/src/core/pikepdf.cpp` & `pikepdf-8.2.2/src/core/pikepdf.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/src/core/pikepdf.h` & `pikepdf-8.2.2/src/core/pikepdf.h`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/src/core/pipeline.cpp` & `pikepdf-8.2.2/src/core/pipeline.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/src/core/pipeline.h` & `pikepdf-8.2.2/src/core/pipeline.h`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/src/core/qpdf.cpp` & `pikepdf-8.2.2/src/core/qpdf.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/src/core/qpdf_inputsource-inl.h` & `pikepdf-8.2.2/src/core/qpdf_inputsource-inl.h`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/src/core/qpdf_pagelist.cpp` & `pikepdf-8.2.2/src/core/qpdf_pagelist.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/src/core/qpdf_pagelist.h` & `pikepdf-8.2.2/src/core/qpdf_pagelist.h`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/src/core/rectangle.cpp` & `pikepdf-8.2.2/src/core/rectangle.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/src/core/tokenfilter.cpp` & `pikepdf-8.2.2/src/core/tokenfilter.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/src/core/utils.cpp` & `pikepdf-8.2.2/src/core/utils.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/src/core/utils.h` & `pikepdf-8.2.2/src/core/utils.h`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/src/pikepdf/__init__.py` & `pikepdf-8.2.2/src/pikepdf/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 """A library for manipulating PDFs."""
 
 # isort:skip_file
 
 from __future__ import annotations
 
-__version__ = "8.2.1"
+__version__ = "8.2.2"
 
 try:
     from . import _core
 except ImportError as _e:  # pragma: no cover
     _msg = "pikepdf's extension library failed to import"
     raise ImportError(_msg) from _e
```

### Comparing `pikepdf-8.2.1/src/pikepdf/_augments.py` & `pikepdf-8.2.2/src/pikepdf/_augments.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/src/pikepdf/_cpphelpers.py` & `pikepdf-8.2.2/src/pikepdf/_cpphelpers.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/src/pikepdf/_io.py` & `pikepdf-8.2.2/src/pikepdf/_io.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/src/pikepdf/_methods.py` & `pikepdf-8.2.2/src/pikepdf/_methods.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/src/pikepdf/_qpdf.py` & `pikepdf-8.2.2/src/pikepdf/_qpdf.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/src/pikepdf/_xml.py` & `pikepdf-8.2.2/src/pikepdf/_xml.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/src/pikepdf/codec.py` & `pikepdf-8.2.2/src/pikepdf/codec.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/src/pikepdf/jbig2.py` & `pikepdf-8.2.2/src/pikepdf/jbig2.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/src/pikepdf/models/__init__.py` & `pikepdf-8.2.2/src/pikepdf/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/src/pikepdf/models/_content_stream.py` & `pikepdf-8.2.2/src/pikepdf/models/_content_stream.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/src/pikepdf/models/_transcoding.py` & `pikepdf-8.2.2/src/pikepdf/models/_transcoding.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/src/pikepdf/models/encryption.py` & `pikepdf-8.2.2/src/pikepdf/models/encryption.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/src/pikepdf/models/image.py` & `pikepdf-8.2.2/src/pikepdf/models/image.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/src/pikepdf/models/matrix.py` & `pikepdf-8.2.2/src/pikepdf/models/matrix.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/src/pikepdf/models/metadata.py` & `pikepdf-8.2.2/src/pikepdf/models/metadata.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/src/pikepdf/models/outlines.py` & `pikepdf-8.2.2/src/pikepdf/models/outlines.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/src/pikepdf/objects.py` & `pikepdf-8.2.2/src/pikepdf/objects.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/src/pikepdf.egg-info/PKG-INFO` & `pikepdf-8.2.2/src/pikepdf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pikepdf
-Version: 8.2.1
+Version: 8.2.2
 Summary: Read and write PDFs with Python, powered by qpdf
 Author-email: "James R. Barlow" <james@purplerock.ca>
 License: MPL-2.0
 Project-URL: documentation, https://pikepdf.readthedocs.io/
 Project-URL: repository, https://github.com/pikepdf/pikepdf
 Project-URL: changelog, https://pikepdf.readthedocs.io/en/latest/releasenotes/index.html
 Keywords: PDF
```

### Comparing `pikepdf-8.2.1/src/pikepdf.egg-info/requires.txt` & `pikepdf-8.2.2/src/pikepdf.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/tests/conftest.py` & `pikepdf-8.2.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/tests/resources/1biticc.pdf` & `pikepdf-8.2.2/tests/resources/1biticc.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/tests/resources/aquamarine-cie.pdf` & `pikepdf-8.2.2/tests/resources/aquamarine-cie.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/tests/resources/aquamarine-cie.png` & `pikepdf-8.2.2/tests/resources/aquamarine-cie.png`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/tests/resources/cmyk-jpeg.pdf` & `pikepdf-8.2.2/tests/resources/cmyk-jpeg.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/tests/resources/congress-gray.pdf` & `pikepdf-8.2.2/tests/resources/congress-gray.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/tests/resources/congress.pdf` & `pikepdf-8.2.2/tests/resources/congress.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/tests/resources/content-stream-errors.pdf` & `pikepdf-8.2.2/tests/resources/content-stream-errors.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/tests/resources/form.pdf` & `pikepdf-8.2.2/tests/resources/form.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/tests/resources/formxobject.pdf` & `pikepdf-8.2.2/tests/resources/formxobject.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/tests/resources/fourpages.pdf` & `pikepdf-8.2.2/tests/resources/fourpages.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/tests/resources/graph-encrypted.pdf` & `pikepdf-8.2.2/tests/resources/graph-encrypted.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/tests/resources/graph.pdf` & `pikepdf-8.2.2/tests/resources/graph.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/tests/resources/image-mono-inline.pdf` & `pikepdf-8.2.2/tests/resources/image-mono-inline.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/tests/resources/invalid_creationdate.pdf` & `pikepdf-8.2.2/tests/resources/invalid_creationdate.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/tests/resources/jbig2.pdf` & `pikepdf-8.2.2/tests/resources/jbig2.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/tests/resources/jbig2global.pdf` & `pikepdf-8.2.2/tests/resources/jbig2global.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/tests/resources/outlines.pdf` & `pikepdf-8.2.2/tests/resources/outlines.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/tests/resources/pal-1bit-rgb.pdf` & `pikepdf-8.2.2/tests/resources/pal-1bit-rgb.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/tests/resources/pal-1bit-trivial.pdf` & `pikepdf-8.2.2/tests/resources/pal-1bit-trivial.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/tests/resources/pal.pdf` & `pikepdf-8.2.2/tests/resources/pal.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/tests/resources/pdfx.pdf` & `pikepdf-8.2.2/tests/resources/pdfx.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/tests/resources/pike-flate-jp2.pdf` & `pikepdf-8.2.2/tests/resources/pike-flate-jp2.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/tests/resources/pike-jp2.pdf` & `pikepdf-8.2.2/tests/resources/pike-jp2.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/tests/resources/pink-palette-icc.pdf` & `pikepdf-8.2.2/tests/resources/pink-palette-icc.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/tests/resources/pink-palette-icc.png` & `pikepdf-8.2.2/tests/resources/pink-palette-icc.png`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/tests/resources/rle.pdf` & `pikepdf-8.2.2/tests/resources/rle.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/tests/resources/sandwich.pdf` & `pikepdf-8.2.2/tests/resources/sandwich.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/tests/resources/veraPDF test suite 6-2-10-t02-pass-a.pdf` & `pikepdf-8.2.2/tests/resources/veraPDF test suite 6-2-10-t02-pass-a.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/tests/resources/veraPDF test suite 6-2-3-3-t01-fail-c.pdf` & `pikepdf-8.2.2/tests/resources/veraPDF test suite 6-2-3-3-t01-fail-c.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/tests/test_annotation.py` & `pikepdf-8.2.2/tests/test_annotation.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/tests/test_attachments.py` & `pikepdf-8.2.2/tests/test_attachments.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/tests/test_augments.py` & `pikepdf-8.2.2/tests/test_augments.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/tests/test_codec.py` & `pikepdf-8.2.2/tests/test_codec.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/tests/test_decimal.py` & `pikepdf-8.2.2/tests/test_decimal.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/tests/test_dictionary.py` & `pikepdf-8.2.2/tests/test_dictionary.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/tests/test_encrypt.py` & `pikepdf-8.2.2/tests/test_encrypt.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/tests/test_errors.py` & `pikepdf-8.2.2/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/tests/test_filters.py` & `pikepdf-8.2.2/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/tests/test_foreign.py` & `pikepdf-8.2.2/tests/test_foreign.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/tests/test_formxobject.py` & `pikepdf-8.2.2/tests/test_formxobject.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/tests/test_image_access.py` & `pikepdf-8.2.2/tests/test_image_access.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/tests/test_io.py` & `pikepdf-8.2.2/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/tests/test_ipython.py` & `pikepdf-8.2.2/tests/test_ipython.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/tests/test_job.py` & `pikepdf-8.2.2/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/tests/test_matrix.py` & `pikepdf-8.2.2/tests/test_matrix.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/tests/test_metadata.py` & `pikepdf-8.2.2/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/tests/test_nametree.py` & `pikepdf-8.2.2/tests/test_nametree.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/tests/test_numbertree.py` & `pikepdf-8.2.2/tests/test_numbertree.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/tests/test_object.py` & `pikepdf-8.2.2/tests/test_object.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/tests/test_objectlist.py` & `pikepdf-8.2.2/tests/test_objectlist.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/tests/test_outlines.py` & `pikepdf-8.2.2/tests/test_outlines.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/tests/test_page.py` & `pikepdf-8.2.2/tests/test_page.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/tests/test_pages.py` & `pikepdf-8.2.2/tests/test_pages.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/tests/test_parsers.py` & `pikepdf-8.2.2/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/tests/test_pdf.py` & `pikepdf-8.2.2/tests/test_pdf.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/tests/test_pdfa.py` & `pikepdf-8.2.2/tests/test_pdfa.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/tests/test_private_pdfs.py` & `pikepdf-8.2.2/tests/test_private_pdfs.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/tests/test_rectangle.py` & `pikepdf-8.2.2/tests/test_rectangle.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/tests/test_refcount.py` & `pikepdf-8.2.2/tests/test_refcount.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/tests/test_repr.py` & `pikepdf-8.2.2/tests/test_repr.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.2.1/tests/test_sanity.py` & `pikepdf-8.2.2/tests/test_sanity.py`

 * *Files identical despite different names*

