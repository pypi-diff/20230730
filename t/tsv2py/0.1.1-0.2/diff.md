# Comparing `tmp/tsv2py-0.1.1.tar.gz` & `tmp/tsv2py-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsv2py-0.1.1.tar", last modified: Fri Jul 14 10:24:08 2023, max compression
+gzip compressed data, was "tsv2py-0.2.tar", last modified: Sun Jul 30 18:10:54 2023, max compression
```

## Comparing `tsv2py-0.1.1.tar` & `tsv2py-0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-07-14 10:24:08.696722 tsv2py-0.1.1/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1072 2023-06-28 18:18:33.000000 tsv2py-0.1.1/LICENSE
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     4394 2023-07-14 10:24:08.696925 tsv2py-0.1.1/PKG-INFO
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3417 2023-07-08 21:32:48.000000 tsv2py-0.1.1/README.md
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-07-14 10:24:08.692010 tsv2py-0.1.1/lib/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    18402 2023-07-14 09:09:48.000000 tsv2py-0.1.1/lib/tsv_parser.c
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)       94 2023-06-28 18:18:10.000000 tsv2py-0.1.1/pyproject.toml
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1074 2023-07-14 10:24:08.697633 tsv2py-0.1.1/setup.cfg
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1212 2023-07-14 09:22:35.000000 tsv2py-0.1.1/setup.py
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-07-14 10:24:08.692903 tsv2py-0.1.1/tests/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3408 2023-07-14 08:53:50.000000 tsv2py-0.1.1/tests/test_perf.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     5262 2023-07-08 21:18:49.000000 tsv2py-0.1.1/tests/test_tsv.py
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-07-14 10:24:08.694212 tsv2py-0.1.1/tsv/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)       22 2023-07-14 10:22:39.000000 tsv2py-0.1.1/tsv/__init__.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1397 2023-07-08 21:33:36.000000 tsv2py-0.1.1/tsv/helper.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-06-28 23:16:45.000000 tsv2py-0.1.1/tsv/py.typed
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-07-14 10:24:08.696346 tsv2py-0.1.1/tsv2py.egg-info/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     4394 2023-07-14 10:24:08.000000 tsv2py-0.1.1/tsv2py.egg-info/PKG-INFO
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      293 2023-07-14 10:24:08.000000 tsv2py-0.1.1/tsv2py.egg-info/SOURCES.txt
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        1 2023-07-14 10:24:08.000000 tsv2py-0.1.1/tsv2py.egg-info/dependency_links.txt
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        4 2023-07-14 10:24:08.000000 tsv2py-0.1.1/tsv2py.egg-info/top_level.txt
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        1 2023-07-14 10:24:08.000000 tsv2py-0.1.1/tsv2py.egg-info/zip-safe
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-07-30 18:10:54.115595 tsv2py-0.2/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1072 2023-06-28 18:18:33.000000 tsv2py-0.2/LICENSE
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     4453 2023-07-30 18:10:54.115772 tsv2py-0.2/PKG-INFO
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3478 2023-07-30 16:39:08.000000 tsv2py-0.2/README.md
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-07-30 18:10:54.107858 tsv2py-0.2/lib/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    21006 2023-07-30 16:39:08.000000 tsv2py-0.2/lib/tsv_parser.c
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)       94 2023-06-28 18:18:10.000000 tsv2py-0.2/pyproject.toml
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1074 2023-07-30 18:10:54.116720 tsv2py-0.2/setup.cfg
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1420 2023-07-30 16:39:08.000000 tsv2py-0.2/setup.py
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-07-30 18:10:54.108910 tsv2py-0.2/tests/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     6533 2023-07-30 16:39:08.000000 tsv2py-0.2/tests/test_perf.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     6435 2023-07-30 16:39:08.000000 tsv2py-0.2/tests/test_tsv.py
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-07-30 18:10:54.111794 tsv2py-0.2/tsv/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)       20 2023-07-30 18:06:49.000000 tsv2py-0.2/tsv/__init__.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1494 2023-07-30 16:39:08.000000 tsv2py-0.2/tsv/helper.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-06-28 23:16:45.000000 tsv2py-0.2/tsv/py.typed
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-07-30 18:10:54.115082 tsv2py-0.2/tsv2py.egg-info/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     4453 2023-07-30 18:10:54.000000 tsv2py-0.2/tsv2py.egg-info/PKG-INFO
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      293 2023-07-30 18:10:54.000000 tsv2py-0.2/tsv2py.egg-info/SOURCES.txt
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        1 2023-07-30 18:10:54.000000 tsv2py-0.2/tsv2py.egg-info/dependency_links.txt
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        4 2023-07-30 18:10:54.000000 tsv2py-0.2/tsv2py.egg-info/top_level.txt
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        1 2023-07-30 18:10:53.000000 tsv2py-0.2/tsv2py.egg-info/zip-safe
```

### Comparing `tsv2py-0.1.1/LICENSE` & `tsv2py-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tsv2py-0.1.1/PKG-INFO` & `tsv2py-0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsv2py
-Version: 0.1.1
+Version: 0.2
 Summary: High-performance parser and generator for PostgreSQL-compatible tab-separated values (TSV)
 Home-page: https://github.com/hunyadi/tsv2py
 Author: Levente Hunyadi
 Author-email: hunyadi@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -25,15 +25,15 @@
 
 # Parse and generate tab-separated values (TSV) data
 
 [Tab-separated values](https://en.wikipedia.org/wiki/Tab-separated_values) (TSV) is a simple and popular format for data storage, data transfer, exporting data from and importing data to relational databases. For example, PostgreSQL [COPY](https://www.postgresql.org/docs/current/sql-copy.html) moves data between PostgreSQL tables and standard file-system files or in-memory stores, and its `text` format (a text file with one line per table row) is a generic version of TSV. Meanwhile, packages like [asyncpg](https://magicstack.github.io/asyncpg/current/index.html) help efficiently insert, update or query data in bulk with binary data transfer between Python and PostgreSQL.
 
 This package offers a high-performance alternative to convert data between a TSV text file and Python objects. The parser can read a TSV record into a Python tuple consisting of built-in Python types, one for each field. The generator can produce a TSV record from a tuple.
 
-## Quickstart
+## Quick start
 
 ```python
 from tsv.helper import Parser
 
 # specify the column structure
 parser = Parser(fields=(bytes, datetime, float, int, str, UUID, bool))
 
@@ -80,8 +80,12 @@
 * `bytes`. TSV escape sequences are reversed before the data is passed to Python as a `bytes` object. NUL bytes are permitted.
 * `datetime`. The input has to comply with RFC 3339 and ISO 8601. The timezone must be UTC (a.k.a. suffix `Z`).
 * `float`.
 * `int`. Arbitrary-length integers are allowed.
 * `str`. TSV escape sequences are reversed before the data is passed to Python as a `str`. NUL bytes are not allowed.
 * `uuid.UUID`. The input has to comply with RFC 4122, or be a string of 32 hexadecimal digits.
 
-Internally, the implementation uses AVX2 instructions to parse RFC 3339 date-time strings into Python `datetime` objects, and RFC 4122 UUID strings or 32-digit hexadecimal strings into Python `UUID` objects.
+Internally, the implementation uses AVX2 instructions to
+
+* parse RFC 3339 date-time strings into Python `datetime` objects,
+* parse RFC 4122 UUID strings or 32-digit hexadecimal strings into Python `UUID` objects,
+* and find `\t` delimiters between fields in a line.
```

### Comparing `tsv2py-0.1.1/README.md` & `tsv2py-0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Parse and generate tab-separated values (TSV) data
 
 [Tab-separated values](https://en.wikipedia.org/wiki/Tab-separated_values) (TSV) is a simple and popular format for data storage, data transfer, exporting data from and importing data to relational databases. For example, PostgreSQL [COPY](https://www.postgresql.org/docs/current/sql-copy.html) moves data between PostgreSQL tables and standard file-system files or in-memory stores, and its `text` format (a text file with one line per table row) is a generic version of TSV. Meanwhile, packages like [asyncpg](https://magicstack.github.io/asyncpg/current/index.html) help efficiently insert, update or query data in bulk with binary data transfer between Python and PostgreSQL.
 
 This package offers a high-performance alternative to convert data between a TSV text file and Python objects. The parser can read a TSV record into a Python tuple consisting of built-in Python types, one for each field. The generator can produce a TSV record from a tuple.
 
-## Quickstart
+## Quick start
 
 ```python
 from tsv.helper import Parser
 
 # specify the column structure
 parser = Parser(fields=(bytes, datetime, float, int, str, UUID, bool))
 
@@ -55,8 +55,12 @@
 * `bytes`. TSV escape sequences are reversed before the data is passed to Python as a `bytes` object. NUL bytes are permitted.
 * `datetime`. The input has to comply with RFC 3339 and ISO 8601. The timezone must be UTC (a.k.a. suffix `Z`).
 * `float`.
 * `int`. Arbitrary-length integers are allowed.
 * `str`. TSV escape sequences are reversed before the data is passed to Python as a `str`. NUL bytes are not allowed.
 * `uuid.UUID`. The input has to comply with RFC 4122, or be a string of 32 hexadecimal digits.
 
-Internally, the implementation uses AVX2 instructions to parse RFC 3339 date-time strings into Python `datetime` objects, and RFC 4122 UUID strings or 32-digit hexadecimal strings into Python `UUID` objects.
+Internally, the implementation uses AVX2 instructions to
+
+* parse RFC 3339 date-time strings into Python `datetime` objects,
+* parse RFC 4122 UUID strings or 32-digit hexadecimal strings into Python `UUID` objects,
+* and find `\t` delimiters between fields in a line.
```

### Comparing `tsv2py-0.1.1/lib/tsv_parser.c` & `tsv2py-0.2/lib/tsv_parser.c`

 * *Files 5% similar despite different names*

```diff
@@ -4,93 +4,141 @@
 #include <stdbool.h>
 
 #if defined(__AVX2__)
 #include <immintrin.h>
 
 #ifdef _DEBUG
 static void
-debug_print(__m128i value)
+debug_print_128(__m128i value)
 {
     uint8_t str[16];
     _mm_storeu_si128((__m128i *)str, value);
 
     for (int i = 0; i < 16; i++)
     {
         printf("0x%.2x ", str[i]);
     }
     printf("\n");
 }
+
+static void
+debug_print_256(__m256i value)
+{
+    uint8_t str[32];
+    _mm256_storeu_si256((__m256i *)str, value);
+
+    for (int i = 0; i < 32; i++)
+    {
+        printf("0x%.2x ", str[i]);
+    }
+    printf("\n");
+}
+#endif
 #endif
+
+#if defined(Py_LIMITED_API)
+#define PyTuple_SET_ITEM(tpl, index, value) PyTuple_SetItem(tpl, index, value)
+#define PyTuple_GET_ITEM(tpl, index) PyTuple_GetItem(tpl, index)
+#endif
+
+inline bool
+is_escaped(const char *data, Py_ssize_t size)
+{
+#if defined(__AVX2__)
+    if (size >= 16)
+    {
+        __m128i tocmp = _mm_set1_epi8('\\');
+        for (; size >= 16; size -= 16)
+        {
+            __m128i chunk = _mm_loadu_si128((__m128i const *)data);
+            __m128i results = _mm_cmpeq_epi8(chunk, tocmp);
+            if (_mm_movemask_epi8(results))
+            {
+                return true;
+            }
+            data += 16;
+        }
+    }
 #endif
 
-#define TSV_NOT_LEN ~((Py_ssize_t)0)
+    for (; size > 0; --size)
+    {
+        if (*data == '\\')
+        {
+            return true;
+        }
+        data++;
+    }
+    return false;
+}
 
-static Py_ssize_t
-unescape(const char *source, Py_ssize_t source_len, char **target)
+static bool
+unescape(const char *source, Py_ssize_t source_len, char **target, Py_ssize_t *target_len)
 {
     char *output = PyMem_Malloc(source_len);
 
     const char *s = source;
     char *t = output;
 
     Py_ssize_t index = 0;
-    Py_ssize_t target_len = 0;
+    Py_ssize_t output_len = 0;
 
     while (index < source_len)
     {
         if (*s == '\\')
         {
             ++s;
             ++index;
 
             switch (*s)
             {
-            case '\\':
+            case '\\': // ASCII 92
                 *t = '\\';
                 break;
-            case '0':
+            case '0': // ASCII 48
                 *t = '\0';
                 break;
-            case 'b':
+            case 'b': // ASCII 98
                 *t = '\b';
                 break;
-            case 'f':
+            case 'f': // ASCII 102
                 *t = '\f';
                 break;
-            case 'n':
+            case 'n': // ASCII 110
                 *t = '\n';
                 break;
-            case 'r':
+            case 'r': // ASCII 114
                 *t = '\r';
                 break;
-            case 't':
+            case 't': // ASCII 116
                 *t = '\t';
                 break;
-            case 'v':
+            case 'v': // ASCII 118
                 *t = '\v';
                 break;
             default:
                 PyMem_Free(output);
-                return TSV_NOT_LEN;
+                return false;
             }
-            ++target_len;
+            ++output_len;
         }
         else
         {
             *t = *s;
-            ++target_len;
+            ++output_len;
         }
 
         ++s;
         ++t;
         ++index;
     }
 
     *target = output;
-    return target_len;
+    *target_len = output_len;
+    return true;
 }
 
 #if defined(Py_LIMITED_API)
 static PyObject *datetime_module;
 static PyObject *datetime_constructor;
 #endif
 
@@ -160,20 +208,20 @@
         return NULL;
     }
 
     // convert ASCII characters into digit value (offset from character `0`)
     const __m128i ascii_digit_mask = _mm_setr_epi8(15, 15, 15, 15, 0, 15, 15, 0, 15, 15, 0, 15, 15, 0, 15, 15); // 15 = 0x0F
     const __m128i spread_integers = _mm_and_si128(characters, ascii_digit_mask);
 
-    // group spread digits `YYYY-MM-DD HH:MM` into packed digits `YYYYMMDDHHMM----`
-    const __m128i mask = _mm_set_epi8(-1, -1, -1, -1, 15, 14, 12, 11, 9, 8, 6, 5, 3, 2, 1, 0);
+    // group spread digits `YYYY-MM-DD HH:MM:SS` into packed digits `YYYYMMDDHHMMSS--`
+    const __m128i mask = _mm_set_epi8(-1, -1, 18, 17, 15, 14, 12, 11, 9, 8, 6, 5, 3, 2, 1, 0);
     const __m128i packed_integers = _mm_shuffle_epi8(spread_integers, mask);
 
     // fuse neighboring digits into a single value
-    const __m128i weights = _mm_setr_epi8(10, 1, 10, 1, 10, 1, 10, 1, 10, 1, 10, 1, 0, 0, 0, 0);
+    const __m128i weights = _mm_setr_epi8(10, 1, 10, 1, 10, 1, 10, 1, 10, 1, 10, 1, 10, 1, 0, 0);
     const __m128i values = _mm_maddubs_epi16(packed_integers, weights);
 
     // extract values
     char result[16];
     _mm_storeu_si128((__m128i *)result, values);
 
     int year = (result[0] * 100) + result[2];
@@ -187,15 +235,15 @@
 }
 #else
 static PyObject *
 create_datetime(const char *input_string, Py_ssize_t input_size)
 {
     if (input_size != 20 || input_string[4] != '-' || input_string[7] != '-' || (input_string[10] != 'T' && input_string[10] != ' ') || input_string[13] != ':' || input_string[16] != ':' || input_string[19] != 'Z')
     {
-        PyErr_SetString(PyExc_ValueError, "expected: a datetime field of the format `YYYY-MM-DDTHH:MM:SSZ` or `YYYY-MM-DD HH:MM:SSZ`");
+        PyErr_Format(PyExc_ValueError, "expected: a datetime field of the format `YYYY-MM-DDTHH:MM:SSZ` or `YYYY-MM-DD HH:MM:SSZ`; got: %.32s (len = %zd)", input_string, input_size);
         return NULL;
     }
 
     int year = atoi(input_string);
     int month = atoi(input_string + 5);
     int day = atoi(input_string + 8);
     int hour = atoi(input_string + 11);
@@ -209,15 +257,15 @@
 create_float(const char *input_string, Py_ssize_t input_size)
 {
     char *p;
     double value = PyOS_string_to_double(input_string, &p, NULL);
 
     if (p != input_string + input_size)
     {
-        PyErr_SetString(PyExc_ValueError, "expected: a field with a floating-point number");
+        PyErr_Format(PyExc_ValueError, "expected: a field with a floating-point number; got: %.32s (len = %zd)", input_string, input_size);
         return NULL;
     }
 
     return PyFloat_FromDouble(value);
 }
 
 static PyObject *
@@ -230,30 +278,34 @@
     char *p;
     PyObject *result = PyLong_FromString(str, &p, 10);
     Py_ssize_t len = p - str;
     PyMem_Free(str);
 
     if (len != input_size)
     {
-        PyErr_SetString(PyExc_ValueError, "expected: an integer field consisting of an optional sign and decimal digits");
+        PyErr_Format(PyExc_ValueError, "expected: an integer field consisting of an optional sign and decimal digits; got: %.32s (len = %zd)", input_string, input_size);
         return NULL;
     }
 
     return result;
 }
 
 static PyObject *
 create_string(const char *input_string, Py_ssize_t input_size)
 {
+    if (!is_escaped(input_string, input_size))
+    {
+        return PyUnicode_FromStringAndSize(input_string, input_size);
+    }
+
     PyObject *result;
     char *output_string;
     Py_ssize_t output_size;
 
-    output_size = unescape(input_string, input_size, &output_string);
-    if (output_size == TSV_NOT_LEN)
+    if (!unescape(input_string, input_size, &output_string, &output_size))
     {
         PyErr_SetString(PyExc_ValueError, "invalid character escape sequence, only \\0, \\b, \\f, \\n, \\r, \\t and \\v are allowed");
         return NULL;
     }
 
     result = PyUnicode_FromStringAndSize(output_string, output_size);
     PyMem_Free(output_string);
@@ -269,15 +321,15 @@
     }
     else if (input_size == 5 && !strcmp(input_string, "false"))
     {
         Py_RETURN_FALSE;
     }
     else
     {
-        PyErr_SetString(PyExc_ValueError, "expected: a boolean field with a value of either `true` or `false`");
+        PyErr_Format(PyExc_ValueError, "expected: a boolean field with a value of either `true` or `false`; got: %.32s (len = %zd)", input_string, input_size);
         return NULL;
     }
 }
 
 typedef unsigned char uuid_t[16];
 
 #if defined(__AVX2__)
@@ -306,15 +358,15 @@
     a = _mm256_sllv_epi32(a, shift);
     a = _mm256_hadd_epi32(a, _mm256_setzero_si256());
     a = _mm256_permute4x64_epi64(a, 0b00001000);
 
     return _mm256_castsi256_si128(a);
 }
 
-static bool
+inline bool
 parse_uuid_compact(const char *str, uuid_t id)
 {
     const __m256i x = _mm256_loadu_si256((__m256i *)str);
     _mm_storeu_si128((__m128i *)id, parse_uuid(x));
     return true;
 }
 
@@ -322,30 +374,30 @@
  * Converts an UUIDv4 string representation to a 128-bit unsigned int.
  *
  * UUID string is expected in the 8-4-4-4-12 format, e.g. `f81d4fae-7dec-11d0-a765-00a0c91e6bf6`.
  * Uses SIMD via Intel AVX2 instruction set.
  *
  * @see https://github.com/crashoz/uuid_v4
  */
-static bool
+inline bool
 parse_uuid_rfc_4122(const char *str, uuid_t id)
 {
     // Remove dashes and pack hexadecimal ASCII bytes in a 256-bit integer
     const __m256i dash_shuffle = _mm256_set_epi32(0x80808080, 0x0f0e0d0c, 0x0b0a0908, 0x06050403, 0x80800f0e, 0x0c0b0a09, 0x07060504, 0x03020100);
 
     __m256i x = _mm256_loadu_si256((__m256i *)str);
     x = _mm256_shuffle_epi8(x, dash_shuffle);
     x = _mm256_insert_epi16(x, *(uint16_t *)(str + 16), 7);
     x = _mm256_insert_epi32(x, *(uint32_t *)(str + 32), 7);
 
     _mm_storeu_si128((__m128i *)id, parse_uuid(x));
     return true;
 }
 #else
-static bool
+inline bool
 parse_uuid_compact(const char *str, uuid_t id)
 {
     int n = 0;
     sscanf(str,
            "%2hhx%2hhx%2hhx%2hhx"
            "%2hhx%2hhx"
            "%2hhx%2hhx"
@@ -355,15 +407,15 @@
            &id[4], &id[5],
            &id[6], &id[7],
            &id[8], &id[9],
            &id[10], &id[11], &id[12], &id[13], &id[14], &id[15], &n);
     return n == 32;
 }
 
-static bool
+inline bool
 parse_uuid_rfc_4122(const char *str, uuid_t id)
 {
     int n = 0;
     sscanf(str,
            "%2hhx%2hhx%2hhx%2hhx-"
            "%2hhx%2hhx-"
            "%2hhx%2hhx-"
@@ -387,27 +439,27 @@
     uuid_t id;
 
     switch (input_size)
     {
     case 32:
         if (!parse_uuid_compact(input_string, id))
         {
-            PyErr_SetString(PyExc_ValueError, "expected: a UUID string of 32 hexadecimal digits");
+            PyErr_Format(PyExc_ValueError, "expected: a UUID string of 32 hexadecimal digits; got: %.32s (len = %zd)", input_string, input_size);
             return NULL;
         }
         break;
     case 36:
         if (!parse_uuid_rfc_4122(input_string, id))
         {
-            PyErr_SetString(PyExc_ValueError, "expected: a UUID string in the 8-4-4-4-12 format, e.g. `f81d4fae-7dec-11d0-a765-00a0c91e6bf6`");
+            PyErr_Format(PyExc_ValueError, "expected: a UUID string in the 8-4-4-4-12 format, e.g. `f81d4fae-7dec-11d0-a765-00a0c91e6bf6`; got: %.32s (len = %zd)", input_string, input_size);
             return NULL;
         }
         break;
     default:
-        PyErr_SetString(PyExc_ValueError, "expected: a UUID string of 32 hexadecimal digits, or a UUID in the 8-4-4-4-12 format");
+        PyErr_Format(PyExc_ValueError, "expected: a UUID string of 32 hexadecimal digits, or a UUID in the 8-4-4-4-12 format; got: %.32s (len = %zd)", input_string, input_size);
         return NULL;
     }
 
     /* Python signature: uuid.UUID(hex=None, bytes=None, ...) */
     return PyObject_CallFunction(uuid_constructor, "sy#", NULL, id, (Py_ssize_t)sizeof(uuid_t));
 }
 
@@ -455,14 +507,20 @@
     {
         /* instantiate Python object based on field value */
         return create_any(field_type, input_string, input_size);
     }
 }
 
 static PyObject *
+create_optional_any_range(char field_type, const char *field_start, const char *field_end)
+{
+    return create_optional_any(field_type, field_start, field_end - field_start);
+}
+
+static PyObject *
 tsv_parse_record(PyObject *self, PyObject *args)
 {
     const char *field_types;
     Py_ssize_t field_count;
     PyObject *tsv_record;
     PyObject *py_record;
 
@@ -483,44 +541,39 @@
         return NULL;
     }
 
     py_record = PyTuple_New(field_count);
     Py_ssize_t k;
     for (k = 0; k < field_count; ++k)
     {
-#if defined(Py_LIMITED_API)
-        PyObject *tsv_field = PyTuple_GetItem(tsv_record, k);
-#else
         PyObject *tsv_field = PyTuple_GET_ITEM(tsv_record, k);
-#endif
         char *input_string;
         Py_ssize_t input_size;
 
         if (!PyBytes_Check(tsv_field))
         {
             PyErr_SetString(PyExc_TypeError, "expected: field value as a `bytes` object");
+            Py_DECREF(py_record);
             return NULL;
         }
 
         if (PyBytes_AsStringAndSize(tsv_field, &input_string, &input_size) < 0)
         {
+            Py_DECREF(py_record);
             return NULL;
         }
 
         PyObject *py_field = create_optional_any(field_types[k], input_string, input_size);
         if (!py_field)
         {
+            Py_DECREF(py_record);
             return NULL;
         }
 
-#if defined(Py_LIMITED_API)
-        PyTuple_SetItem(py_record, k, py_field);
-#else
         PyTuple_SET_ITEM(py_record, k, py_field);
-#endif
     }
 
     return py_record;
 }
 
 static PyObject *
 tsv_parse_line(PyObject *self, PyObject *args)
@@ -535,69 +588,99 @@
     if (!PyArg_ParseTuple(args, "s#y#", &field_types, &field_count, &line_string, &line_size))
     {
         return NULL;
     }
 
     const char *field_start = line_string;
     const char *field_end;
+    Py_ssize_t field_index = 0;
+
+    const char *scan_start = line_string;
+    Py_ssize_t chars_remain = line_size;
 
     py_record = PyTuple_New(field_count);
 
-    // Parse first n-1 fields (each terminated by `\t`)
-    Py_ssize_t k;
-    for (k = 0; k < field_count - 1; ++k)
+#if defined(__AVX2__)
+    __m256i tab = _mm256_set1_epi8('\t');
+    while (chars_remain >= 32)
     {
-        field_end = strchr(field_start, '\t');
-        if (field_end == NULL)
+        __m256i chunk = _mm256_loadu_si256((__m256i *)scan_start);
+        __m256i results = _mm256_cmpeq_epi8(chunk, tab);
+        unsigned int mask = _mm256_movemask_epi8(results);
+
+        while (mask)
         {
-            PyErr_SetString(PyExc_ValueError, "premature end of input");
-            return NULL;
+            unsigned int offset = _mm_tzcnt_32(mask);
+            mask &= ~(1 << offset);
+
+            field_end = scan_start + offset;
+
+            PyObject *py_field = create_optional_any_range(field_types[field_index], field_start, field_end);
+            if (!py_field)
+            {
+                Py_DECREF(py_record);
+                return NULL;
+            }
+            PyTuple_SET_ITEM(py_record, field_index, py_field);
+
+            ++field_index;
+            if (field_index >= field_count)
+            {
+                PyErr_SetString(PyExc_ValueError, "too many fields in input");
+                Py_DECREF(py_record);
+                return NULL;
+            }
+
+            field_start = field_end + 1;
         }
 
-        const char *input_string = field_start;
-        Py_ssize_t input_size = field_end - field_start;
+        scan_start += 32;
+        chars_remain -= 32;
+    }
+#endif
 
-        PyObject *py_field = create_optional_any(field_types[k], input_string, input_size);
+    while ((field_end = memchr(scan_start, '\t', chars_remain)) != NULL)
+    {
+        PyObject *py_field = create_optional_any_range(field_types[field_index], field_start, field_end);
         if (!py_field)
         {
+            Py_DECREF(py_record);
             return NULL;
         }
+        PyTuple_SET_ITEM(py_record, field_index, py_field);
 
-#if defined(Py_LIMITED_API)
-        PyTuple_SetItem(py_record, k, py_field);
-#else
-        PyTuple_SET_ITEM(py_record, k, py_field);
-#endif
+        ++field_index;
+        if (field_index >= field_count)
+        {
+            PyErr_SetString(PyExc_ValueError, "too many fields in input");
+            Py_DECREF(py_record);
+            return NULL;
+        }
 
         field_start = field_end + 1;
+        scan_start = field_start;
+        chars_remain = line_size - (field_start - line_string);
     }
 
-    // Parse last field (terminated by end of input)
-    if (strchr(field_start, '\t') != NULL)
+    if (field_index != field_count - 1)
     {
-        PyErr_SetString(PyExc_ValueError, "too many fields in input");
+        PyErr_SetString(PyExc_ValueError, "premature end of input");
         return NULL;
     }
 
     field_end = line_string + line_size;
-    const char *input_string = field_start;
-    Py_ssize_t input_size = field_end - field_start;
 
-    PyObject *py_field = create_optional_any(field_types[field_count - 1], input_string, input_size);
+    PyObject *py_field = create_optional_any_range(field_types[field_index], field_start, field_end);
     if (!py_field)
     {
+        Py_DECREF(py_record);
         return NULL;
     }
 
-#if defined(Py_LIMITED_API)
-    PyTuple_SetItem(py_record, field_count - 1, py_field);
-#else
-    PyTuple_SET_ITEM(py_record, field_count - 1, py_field);
-#endif
-
+    PyTuple_SET_ITEM(py_record, field_index, py_field);
     return py_record;
 }
 
 static PyMethodDef TsvParserMethods[] = {
     {"parse_record", tsv_parse_record, METH_VARARGS, "Parses a tuple of byte arrays representing a TSV record into a tuple of Python objects."},
     {"parse_line", tsv_parse_line, METH_VARARGS, "Parses a line representing a TSV record into a tuple of Python objects."},
     {NULL, NULL, 0, NULL}};
```

### Comparing `tsv2py-0.1.1/setup.cfg` & `tsv2py-0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `tsv2py-0.1.1/setup.py` & `tsv2py-0.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # If you have cloned the source code repository, use editable install to link the package catalog to the repository directory:
 # $ pip install -e . --config-settings editable_mode=strict
 
+import os
 import sys
 from typing import Tuple
 
 from setuptools import Extension, setup
 from wheel.bdist_wheel import bdist_wheel
 
 
@@ -16,20 +17,26 @@
             # on CPython, our wheels are abi3 and compatible back to 3.8
             return "cp38", "abi3", plat
 
         return python, abi, plat
 
 
 if sys.platform.startswith("win"):
-    compile_args = ["/arch:AVX2"]
+    compile_args = []
 else:
-    compile_args = [
-        "-mavx2",
-        "-fvisibility=hidden",
-    ]
+    compile_args = ["-fvisibility=hidden"]
+
+if os.getenv("TSV_AVX2", "1") == "1":
+    print("compiling with AVX2")
+    if sys.platform.startswith("win"):
+        compile_args.append("/arch:AVX2")
+    else:
+        compile_args.append("-mavx2")
+else:
+    print("compiling without AVX2")
 
 setup_args = dict(
     ext_modules=[
         Extension(
             "tsv.parser",
             ["lib/tsv_parser.c"],
             extra_compile_args=compile_args,
```

### Comparing `tsv2py-0.1.1/tests/test_tsv.py` & `tsv2py-0.2/tests/test_tsv.py`

 * *Files 22% similar despite different names*

```diff
@@ -120,27 +120,59 @@
             None,
             None,
             None,
             None,
         )
         self.assertEqual(parse_line("bdfisuz", tsv_record), py_record)
 
-    def test_length(self) -> None:
+    def test_field_count(self) -> None:
         tsv_record = b"0"
         parse_line("i", tsv_record)
         with self.assertRaises(ValueError):
             parse_line("ii", tsv_record)
 
         tsv_record = b"\t".join([b"1", b"2"])
         with self.assertRaises(ValueError):
             parse_line("i", tsv_record)
         parse_line("ii", tsv_record)
         with self.assertRaises(ValueError):
             parse_line("iii", tsv_record)
 
+    def test_field_length(self) -> None:
+        # insufficient characters, no SIMD operation is executed
+        tsv_record = b"string"
+        parse_line("s", tsv_record)
+        tsv_record = b"\t\t\t\t\t"
+        parse_line("ssssss", tsv_record)
+
+        # no delimiter is found with SIMD operation
+        tsv_record = b"12345678901234567890123456789012\t..."
+        parse_line("ss", tsv_record)
+
+        # one delimiter is found with SIMD operation
+        tsv_record = b"1234567890123456789012345678901\t..."
+        parse_line("ss", tsv_record)
+
+        # several delimiters found with SIMD operation
+        tsv_record = b"1\t12\t123\t1234\t12345\t...12345678901234567890123456789012"
+        parse_line("ssssss", tsv_record)
+
+    def test_string_escape(self) -> None:
+        tsv_record = b""
+        parse_line("s", tsv_record)
+
+        tsv_record = (
+            r"árvíztűrő \0, \b, \f, \n, \r, \t and \v \\\\ tükörfúrógép".encode("utf-8")
+        )
+        parse_line("s", tsv_record)
+
+        tsv_record = r"árvíztűrő \N tükörfúrógép".encode("utf-8")
+        with self.assertRaises(ValueError):
+            parse_line("s", tsv_record)
+
 
 class TestParseFile(unittest.TestCase):
     tsv_path: str
 
     def __init__(self, methodName: str = "runTest") -> None:
         super().__init__(methodName)
         self.tsv_path = os.path.join(os.path.dirname(__file__), "test.tsv")
```

### Comparing `tsv2py-0.1.1/tsv/helper.py` & `tsv2py-0.2/tsv/helper.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import datetime
 import uuid
 from typing import Any, BinaryIO, List, Tuple
 
 from . import parser
 
 
-def _type_to_format_char(typ: type) -> str:
+def type_to_format_char(typ: type) -> str:
     if typ is bool:
         return "z"
     elif typ is int:
         return "i"
     elif typ is float:
         return "f"
     elif typ is str:
@@ -20,19 +20,23 @@
         return "u"
     elif typ is bytes:
         return "b"
     else:
         raise TypeError(f"conversion for type `{typ}` is not supported")
 
 
+def types_to_format_str(fields: Tuple[type, ...]) -> str:
+    return "".join(type_to_format_char(typ) for typ in fields)
+
+
 class Parser:
     _format: str
 
     def __init__(self, fields: Tuple[type, ...]) -> None:
-        self._format = "".join(_type_to_format_char(typ) for typ in fields)
+        self._format = types_to_format_str(fields)
 
     def parse_record(self, record: Tuple[bytes, ...]) -> Tuple[Any, ...]:
         """
         Parses a tuple of byte arrays representing a TSV record into a tuple of Python objects.
         """
 
         return parser.parse_record(self._format, record)
```

### Comparing `tsv2py-0.1.1/tsv2py.egg-info/PKG-INFO` & `tsv2py-0.2/tsv2py.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsv2py
-Version: 0.1.1
+Version: 0.2
 Summary: High-performance parser and generator for PostgreSQL-compatible tab-separated values (TSV)
 Home-page: https://github.com/hunyadi/tsv2py
 Author: Levente Hunyadi
 Author-email: hunyadi@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -25,15 +25,15 @@
 
 # Parse and generate tab-separated values (TSV) data
 
 [Tab-separated values](https://en.wikipedia.org/wiki/Tab-separated_values) (TSV) is a simple and popular format for data storage, data transfer, exporting data from and importing data to relational databases. For example, PostgreSQL [COPY](https://www.postgresql.org/docs/current/sql-copy.html) moves data between PostgreSQL tables and standard file-system files or in-memory stores, and its `text` format (a text file with one line per table row) is a generic version of TSV. Meanwhile, packages like [asyncpg](https://magicstack.github.io/asyncpg/current/index.html) help efficiently insert, update or query data in bulk with binary data transfer between Python and PostgreSQL.
 
 This package offers a high-performance alternative to convert data between a TSV text file and Python objects. The parser can read a TSV record into a Python tuple consisting of built-in Python types, one for each field. The generator can produce a TSV record from a tuple.
 
-## Quickstart
+## Quick start
 
 ```python
 from tsv.helper import Parser
 
 # specify the column structure
 parser = Parser(fields=(bytes, datetime, float, int, str, UUID, bool))
 
@@ -80,8 +80,12 @@
 * `bytes`. TSV escape sequences are reversed before the data is passed to Python as a `bytes` object. NUL bytes are permitted.
 * `datetime`. The input has to comply with RFC 3339 and ISO 8601. The timezone must be UTC (a.k.a. suffix `Z`).
 * `float`.
 * `int`. Arbitrary-length integers are allowed.
 * `str`. TSV escape sequences are reversed before the data is passed to Python as a `str`. NUL bytes are not allowed.
 * `uuid.UUID`. The input has to comply with RFC 4122, or be a string of 32 hexadecimal digits.
 
-Internally, the implementation uses AVX2 instructions to parse RFC 3339 date-time strings into Python `datetime` objects, and RFC 4122 UUID strings or 32-digit hexadecimal strings into Python `UUID` objects.
+Internally, the implementation uses AVX2 instructions to
+
+* parse RFC 3339 date-time strings into Python `datetime` objects,
+* parse RFC 4122 UUID strings or 32-digit hexadecimal strings into Python `UUID` objects,
+* and find `\t` delimiters between fields in a line.
```

