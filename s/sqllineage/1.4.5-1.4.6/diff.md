# Comparing `tmp/sqllineage-1.4.5.tar.gz` & `tmp/sqllineage-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqllineage-1.4.5.tar", last modified: Sun Jul  2 10:17:26 2023, max compression
+gzip compressed data, was "sqllineage-1.4.6.tar", last modified: Sun Jul 30 16:17:32 2023, max compression
```

## Comparing `sqllineage-1.4.5.tar` & `sqllineage-1.4.6.tar`

### file list

```diff
@@ -1,224 +1,282 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:17:26.779639 sqllineage-1.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-02 10:15:29.000000 sqllineage-1.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-02 10:15:29.000000 sqllineage-1.4.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7286 2023-07-02 10:17:26.779639 sqllineage-1.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-07-02 10:15:29.000000 sqllineage-1.4.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 10:17:26.779639 sqllineage-1.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-07-02 10:15:29.000000 sqllineage-1.4.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:17:26.735638 sqllineage-1.4.5/sqllineage/
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:17:26.739638 sqllineage-1.4.5/sqllineage/build/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-02 10:17:24.000000 sqllineage-1.4.5/sqllineage/build/asset-manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)   145386 2023-07-02 10:17:24.000000 sqllineage-1.4.5/sqllineage/build/editor.worker.js
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-02 10:17:24.000000 sqllineage-1.4.5/sqllineage/build/editor.worker.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)   637125 2023-07-02 10:17:24.000000 sqllineage-1.4.5/sqllineage/build/editor.worker.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-07-02 10:16:03.000000 sqllineage-1.4.5/sqllineage/build/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-02 10:17:24.000000 sqllineage-1.4.5/sqllineage/build/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-07-02 10:16:03.000000 sqllineage-1.4.5/sqllineage/build/logo192.png
--rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-07-02 10:16:03.000000 sqllineage-1.4.5/sqllineage/build/logo512.png
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-02 10:16:03.000000 sqllineage-1.4.5/sqllineage/build/manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-02 10:16:03.000000 sqllineage-1.4.5/sqllineage/build/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:17:26.735638 sqllineage-1.4.5/sqllineage/build/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:17:26.739638 sqllineage-1.4.5/sqllineage/build/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)    69444 2023-07-02 10:17:24.000000 sqllineage-1.4.5/sqllineage/build/static/css/main.c1b86fee.css
--rw-r--r--   0 runner    (1001) docker     (123)   146886 2023-07-02 10:17:24.000000 sqllineage-1.4.5/sqllineage/build/static/css/main.c1b86fee.css.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:17:26.743638 sqllineage-1.4.5/sqllineage/build/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)    18303 2023-07-02 10:17:24.000000 sqllineage-1.4.5/sqllineage/build/static/js/333.97bcedbd.chunk.js
--rw-r--r--   0 runner    (1001) docker     (123)    45386 2023-07-02 10:17:24.000000 sqllineage-1.4.5/sqllineage/build/static/js/333.97bcedbd.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (123)  3568928 2023-07-02 10:17:24.000000 sqllineage-1.4.5/sqllineage/build/static/js/main.e83a4547.js
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-02 10:17:24.000000 sqllineage-1.4.5/sqllineage/build/static/js/main.e83a4547.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123) 13448130 2023-07-02 10:17:24.000000 sqllineage-1.4.5/sqllineage/build/static/js/main.e83a4547.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:17:26.755638 sqllineage-1.4.5/sqllineage/build/static/media/
--rw-r--r--   0 runner    (1001) docker     (123)    62792 2023-07-02 10:17:24.000000 sqllineage-1.4.5/sqllineage/build/static/media/codicon.4168b9c11e5075e9cfe6.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:17:26.759639 sqllineage-1.4.5/sqllineage/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/core/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12540 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/core/holders.py
--rw-r--r--   0 runner    (1001) docker     (123)     7132 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/core/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:17:26.759639 sqllineage-1.4.5/sqllineage/core/parser/
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/core/parser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:17:26.759639 sqllineage-1.4.5/sqllineage/core/parser/sqlfluff/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/core/parser/sqlfluff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/core/parser/sqlfluff/analyzer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:17:26.759639 sqllineage-1.4.5/sqllineage/core/parser/sqlfluff/extractors/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/core/parser/sqlfluff/extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/core/parser/sqlfluff/extractors/cte_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/core/parser/sqlfluff/extractors/ddl_alter_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/core/parser/sqlfluff/extractors/ddl_drop_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/core/parser/sqlfluff/extractors/dml_insert_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/core/parser/sqlfluff/extractors/dml_merge_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/core/parser/sqlfluff/extractors/dml_select_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/core/parser/sqlfluff/extractors/lineage_holder_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/core/parser/sqlfluff/extractors/noop_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:17:26.759639 sqllineage-1.4.5/sqllineage/core/parser/sqlfluff/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/core/parser/sqlfluff/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/core/parser/sqlfluff/handlers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/core/parser/sqlfluff/handlers/source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/core/parser/sqlfluff/handlers/swap_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/core/parser/sqlfluff/handlers/target.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/core/parser/sqlfluff/holder_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8492 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/core/parser/sqlfluff/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    15990 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/core/parser/sqlfluff/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:17:26.759639 sqllineage-1.4.5/sqllineage/core/parser/sqlparse/
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/core/parser/sqlparse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11050 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/core/parser/sqlparse/analyzer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:17:26.759639 sqllineage-1.4.5/sqllineage/core/parser/sqlparse/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/core/parser/sqlparse/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/core/parser/sqlparse/handlers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/core/parser/sqlparse/handlers/cte.py
--rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/core/parser/sqlparse/handlers/source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/core/parser/sqlparse/handlers/swap_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/core/parser/sqlparse/handlers/target.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/core/parser/sqlparse/holder_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7443 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/core/parser/sqlparse/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     7518 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/core/parser/sqlparse/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:17:26.735638 sqllineage-1.4.5/sqllineage/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:17:26.771639 sqllineage-1.4.5/sqllineage/data/tpcds/
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query01.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query02.sql
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query03.sql
--rw-r--r--   0 runner    (1001) docker     (123)     6685 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query04.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query05.sql
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query06.sql
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query07.sql
--rw-r--r--   0 runner    (1001) docker     (123)     8175 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query08.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query09.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query10.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query11.sql
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query12.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query13.sql
--rw-r--r--   0 runner    (1001) docker     (123)     9010 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query14.sql
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query15.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query16.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query17.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query18.sql
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query19.sql
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query20.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query21.sql
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query22.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query23.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query24.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query25.sql
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query26.sql
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query27.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query28.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query29.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query30.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query31.sql
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query32.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query33.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query34.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query35.sql
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query36.sql
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query37.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query38.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query39.sql
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query40.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query41.sql
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query42.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query43.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query44.sql
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query45.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query46.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query47.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query48.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query49.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query50.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query51.sql
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query52.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query53.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query54.sql
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query55.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query56.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query57.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query58.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query59.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query60.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query61.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query62.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query63.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query64.sql
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query65.sql
--rw-r--r--   0 runner    (1001) docker     (123)    13194 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query66.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query67.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query68.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query69.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query70.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query71.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query72.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query73.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query74.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query75.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query76.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query77.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query78.sql
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query79.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query80.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query81.sql
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query82.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query83.sql
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query84.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query85.sql
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query86.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query87.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5794 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query88.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query89.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query90.sql
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query91.sql
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query92.sql
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query93.sql
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query94.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query95.sql
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query96.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query97.sql
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query98.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/data/tpcds/query99.sql
--rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/drawing.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:17:26.771639 sqllineage-1.4.5/sqllineage/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/utils/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/utils/entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineage/utils/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:17:26.735638 sqllineage-1.4.5/sqllineage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7286 2023-07-02 10:17:25.000000 sqllineage-1.4.5/sqllineage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7168 2023-07-02 10:17:26.000000 sqllineage-1.4.5/sqllineage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 10:17:25.000000 sqllineage-1.4.5/sqllineage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-02 10:17:25.000000 sqllineage-1.4.5/sqllineage.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-02 10:17:25.000000 sqllineage-1.4.5/sqllineage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-02 10:17:25.000000 sqllineage-1.4.5/sqllineage.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:17:26.775639 sqllineage-1.4.5/sqllineagejs/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineagejs/config-overrides.js
--rw-r--r--   0 runner    (1001) docker     (123)  1282011 2023-07-02 10:16:01.000000 sqllineage-1.4.5/sqllineagejs/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineagejs/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:17:26.775639 sqllineage-1.4.5/sqllineagejs/public/
--rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineagejs/public/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineagejs/public/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineagejs/public/logo192.png
--rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineagejs/public/logo512.png
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineagejs/public/manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineagejs/public/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:17:26.775639 sqllineage-1.4.5/sqllineagejs/src/
--rw-r--r--   0 runner    (1001) docker     (123)     9038 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineagejs/src/App.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:17:26.775639 sqllineage-1.4.5/sqllineagejs/src/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineagejs/src/api/client.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:17:26.775639 sqllineage-1.4.5/sqllineagejs/src/app/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineagejs/src/app/store.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:17:26.735638 sqllineage-1.4.5/sqllineagejs/src/features/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:17:26.775639 sqllineage-1.4.5/sqllineagejs/src/features/directory/
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineagejs/src/features/directory/Directory.js
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineagejs/src/features/directory/DirectoryTreeItem.js
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineagejs/src/features/directory/directorySlice.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:17:26.775639 sqllineage-1.4.5/sqllineagejs/src/features/editor/
--rw-r--r--   0 runner    (1001) docker     (123)    12152 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineagejs/src/features/editor/DAG.js
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineagejs/src/features/editor/DAGDesc.js
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineagejs/src/features/editor/Editor.js
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineagejs/src/features/editor/editorSlice.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:17:26.775639 sqllineage-1.4.5/sqllineagejs/src/features/widget/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineagejs/src/features/widget/LoadError.js
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineagejs/src/features/widget/Loading.js
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineagejs/src/index.css
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-02 10:15:29.000000 sqllineage-1.4.5/sqllineagejs/src/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:17:32.602016 sqllineage-1.4.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-30 16:15:05.000000 sqllineage-1.4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-30 16:15:05.000000 sqllineage-1.4.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7286 2023-07-30 16:17:32.602016 sqllineage-1.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-07-30 16:15:05.000000 sqllineage-1.4.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 16:17:32.602016 sqllineage-1.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-07-30 16:15:05.000000 sqllineage-1.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:17:32.534015 sqllineage-1.4.6/sqllineage/
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:17:32.542015 sqllineage-1.4.6/sqllineage/build/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-30 16:17:30.000000 sqllineage-1.4.6/sqllineage/build/asset-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)   145386 2023-07-30 16:17:30.000000 sqllineage-1.4.6/sqllineage/build/editor.worker.js
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-30 16:17:30.000000 sqllineage-1.4.6/sqllineage/build/editor.worker.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   637125 2023-07-30 16:17:30.000000 sqllineage-1.4.6/sqllineage/build/editor.worker.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-07-30 16:15:42.000000 sqllineage-1.4.6/sqllineage/build/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-30 16:17:30.000000 sqllineage-1.4.6/sqllineage/build/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-07-30 16:15:42.000000 sqllineage-1.4.6/sqllineage/build/logo192.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-07-30 16:15:42.000000 sqllineage-1.4.6/sqllineage/build/logo512.png
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-30 16:15:42.000000 sqllineage-1.4.6/sqllineage/build/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-30 16:15:42.000000 sqllineage-1.4.6/sqllineage/build/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:17:32.526015 sqllineage-1.4.6/sqllineage/build/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:17:32.542015 sqllineage-1.4.6/sqllineage/build/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    69444 2023-07-30 16:17:30.000000 sqllineage-1.4.6/sqllineage/build/static/css/main.c1b86fee.css
+-rw-r--r--   0 runner    (1001) docker     (123)   146886 2023-07-30 16:17:30.000000 sqllineage-1.4.6/sqllineage/build/static/css/main.c1b86fee.css.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:17:32.550016 sqllineage-1.4.6/sqllineage/build/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    18303 2023-07-30 16:17:30.000000 sqllineage-1.4.6/sqllineage/build/static/js/333.97bcedbd.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (123)    45386 2023-07-30 16:17:30.000000 sqllineage-1.4.6/sqllineage/build/static/js/333.97bcedbd.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)  3568928 2023-07-30 16:17:30.000000 sqllineage-1.4.6/sqllineage/build/static/js/main.e83a4547.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-30 16:17:30.000000 sqllineage-1.4.6/sqllineage/build/static/js/main.e83a4547.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123) 13448130 2023-07-30 16:17:30.000000 sqllineage-1.4.6/sqllineage/build/static/js/main.e83a4547.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:17:32.566016 sqllineage-1.4.6/sqllineage/build/static/media/
+-rw-r--r--   0 runner    (1001) docker     (123)    62792 2023-07-30 16:17:30.000000 sqllineage-1.4.6/sqllineage/build/static/media/codicon.4168b9c11e5075e9cfe6.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:17:32.566016 sqllineage-1.4.6/sqllineage/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/core/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12540 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/core/holders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7139 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/core/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:17:32.566016 sqllineage-1.4.6/sqllineage/core/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/core/parser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:17:32.570016 sqllineage-1.4.6/sqllineage/core/parser/sqlfluff/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/core/parser/sqlfluff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/core/parser/sqlfluff/analyzer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:17:32.570016 sqllineage-1.4.6/sqllineage/core/parser/sqlfluff/extractors/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/core/parser/sqlfluff/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/core/parser/sqlfluff/extractors/cte_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/core/parser/sqlfluff/extractors/ddl_alter_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/core/parser/sqlfluff/extractors/ddl_drop_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/core/parser/sqlfluff/extractors/dml_insert_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/core/parser/sqlfluff/extractors/dml_merge_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/core/parser/sqlfluff/extractors/dml_select_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/core/parser/sqlfluff/extractors/lineage_holder_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/core/parser/sqlfluff/extractors/noop_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:17:32.570016 sqllineage-1.4.6/sqllineage/core/parser/sqlfluff/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/core/parser/sqlfluff/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/core/parser/sqlfluff/handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/core/parser/sqlfluff/handlers/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/core/parser/sqlfluff/handlers/target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/core/parser/sqlfluff/holder_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8548 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/core/parser/sqlfluff/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15479 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/core/parser/sqlfluff/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:17:32.570016 sqllineage-1.4.6/sqllineage/core/parser/sqlparse/
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/core/parser/sqlparse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11050 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/core/parser/sqlparse/analyzer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:17:32.574015 sqllineage-1.4.6/sqllineage/core/parser/sqlparse/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/core/parser/sqlparse/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/core/parser/sqlparse/handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/core/parser/sqlparse/handlers/cte.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/core/parser/sqlparse/handlers/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/core/parser/sqlparse/handlers/swap_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/core/parser/sqlparse/handlers/target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/core/parser/sqlparse/holder_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7268 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/core/parser/sqlparse/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7518 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/core/parser/sqlparse/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:17:32.526015 sqllineage-1.4.6/sqllineage/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:17:32.586016 sqllineage-1.4.6/sqllineage/data/tpcds/
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query01.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query02.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query03.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     6685 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query04.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query05.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query06.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query07.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     8175 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query08.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query09.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query10.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query11.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query12.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query13.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     9010 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query14.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query15.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query16.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query17.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query18.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query19.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query20.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query21.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query22.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query23.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query24.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query25.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query26.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query27.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query28.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query29.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query30.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query31.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query32.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query33.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query34.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query35.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query36.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query37.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query38.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query39.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query40.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query41.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query42.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query43.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query44.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query45.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query46.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query47.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query48.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query49.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query50.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query51.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query52.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query53.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query54.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query55.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query56.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query57.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query58.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query59.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query60.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query61.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query62.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query63.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query64.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query65.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    13194 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query66.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query67.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query68.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query69.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query70.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query71.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query72.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query73.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query74.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query75.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query76.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query77.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query78.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query79.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query80.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query81.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query82.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query83.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query84.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query85.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query86.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query87.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5794 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query88.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query89.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query90.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query91.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query92.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query93.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query94.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query95.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query96.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query97.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query98.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/data/tpcds/query99.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/drawing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:17:32.590016 sqllineage-1.4.6/sqllineage/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/utils/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/utils/entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineage/utils/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:17:32.534015 sqllineage-1.4.6/sqllineage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7286 2023-07-30 16:17:30.000000 sqllineage-1.4.6/sqllineage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9293 2023-07-30 16:17:32.000000 sqllineage-1.4.6/sqllineage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 16:17:30.000000 sqllineage-1.4.6/sqllineage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-30 16:17:30.000000 sqllineage-1.4.6/sqllineage.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-30 16:17:30.000000 sqllineage-1.4.6/sqllineage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-30 16:17:30.000000 sqllineage-1.4.6/sqllineage.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:17:32.590016 sqllineage-1.4.6/sqllineagejs/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineagejs/config-overrides.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1282011 2023-07-30 16:15:39.000000 sqllineage-1.4.6/sqllineagejs/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineagejs/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:17:32.590016 sqllineage-1.4.6/sqllineagejs/public/
+-rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineagejs/public/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineagejs/public/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineagejs/public/logo192.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineagejs/public/logo512.png
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineagejs/public/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineagejs/public/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:17:32.594016 sqllineage-1.4.6/sqllineagejs/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     9038 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineagejs/src/App.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:17:32.594016 sqllineage-1.4.6/sqllineagejs/src/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineagejs/src/api/client.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:17:32.594016 sqllineage-1.4.6/sqllineagejs/src/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineagejs/src/app/store.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:17:32.530015 sqllineage-1.4.6/sqllineagejs/src/features/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:17:32.594016 sqllineage-1.4.6/sqllineagejs/src/features/directory/
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineagejs/src/features/directory/Directory.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineagejs/src/features/directory/DirectoryTreeItem.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineagejs/src/features/directory/directorySlice.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:17:32.594016 sqllineage-1.4.6/sqllineagejs/src/features/editor/
+-rw-r--r--   0 runner    (1001) docker     (123)    12152 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineagejs/src/features/editor/DAG.js
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineagejs/src/features/editor/DAGDesc.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineagejs/src/features/editor/Editor.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineagejs/src/features/editor/editorSlice.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:17:32.594016 sqllineage-1.4.6/sqllineagejs/src/features/widget/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineagejs/src/features/widget/LoadError.js
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineagejs/src/features/widget/Loading.js
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineagejs/src/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-30 16:15:05.000000 sqllineage-1.4.6/sqllineagejs/src/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:17:32.530015 sqllineage-1.4.6/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:17:32.594016 sqllineage-1.4.6/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 16:15:05.000000 sqllineage-1.4.6/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-30 16:15:05.000000 sqllineage-1.4.6/tests/core/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-07-30 16:15:05.000000 sqllineage-1.4.6/tests/core/test_drawing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-30 16:15:05.000000 sqllineage-1.4.6/tests/core/test_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-30 16:15:05.000000 sqllineage-1.4.6/tests/core/test_holder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-30 16:15:05.000000 sqllineage-1.4.6/tests/core/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-30 16:15:05.000000 sqllineage-1.4.6/tests/core/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-30 16:15:05.000000 sqllineage-1.4.6/tests/core/test_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:17:32.594016 sqllineage-1.4.6/tests/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 16:15:05.000000 sqllineage-1.4.6/tests/sql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:17:32.598016 sqllineage-1.4.6/tests/sql/column/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 16:15:05.000000 sqllineage-1.4.6/tests/sql/column/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-07-30 16:15:05.000000 sqllineage-1.4.6/tests/sql/column/test_column_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-07-30 16:15:05.000000 sqllineage-1.4.6/tests/sql/column/test_column_select_case_when.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-07-30 16:15:05.000000 sqllineage-1.4.6/tests/sql/column/test_column_select_cast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-07-30 16:15:05.000000 sqllineage-1.4.6/tests/sql/column/test_column_select_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-07-30 16:15:05.000000 sqllineage-1.4.6/tests/sql/column/test_column_select_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-07-30 16:15:05.000000 sqllineage-1.4.6/tests/sql/column/test_column_select_from_cte.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-07-30 16:15:05.000000 sqllineage-1.4.6/tests/sql/column/test_column_select_from_join.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-07-30 16:15:05.000000 sqllineage-1.4.6/tests/sql/column/test_column_select_from_subquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-07-30 16:15:05.000000 sqllineage-1.4.6/tests/sql/column/test_column_select_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-30 16:15:05.000000 sqllineage-1.4.6/tests/sql/column/test_column_select_union.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:17:32.598016 sqllineage-1.4.6/tests/sql/sqlfluff_only/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-30 16:15:05.000000 sqllineage-1.4.6/tests/sql/sqlfluff_only/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-07-30 16:15:05.000000 sqllineage-1.4.6/tests/sql/sqlfluff_only/test_dialect_specific.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-07-30 16:15:05.000000 sqllineage-1.4.6/tests/sql/sqlfluff_only/test_dml_specify_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-07-30 16:15:05.000000 sqllineage-1.4.6/tests/sql/sqlfluff_only/test_keyword_as_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-30 16:15:05.000000 sqllineage-1.4.6/tests/sql/sqlfluff_only/test_parenthesized_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-30 16:15:05.000000 sqllineage-1.4.6/tests/sql/sqlfluff_only/test_parenthesized_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:17:32.602016 sqllineage-1.4.6/tests/sql/table/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 16:15:05.000000 sqllineage-1.4.6/tests/sql/table/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:17:32.602016 sqllineage-1.4.6/tests/sql/table/multiple_statements/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 16:15:05.000000 sqllineage-1.4.6/tests/sql/table/multiple_statements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-30 16:15:05.000000 sqllineage-1.4.6/tests/sql/table/multiple_statements/test_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-30 16:15:05.000000 sqllineage-1.4.6/tests/sql/table/multiple_statements/test_tmp_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-30 16:15:05.000000 sqllineage-1.4.6/tests/sql/table/multiple_statements/test_variable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:17:32.602016 sqllineage-1.4.6/tests/sql/table/object_storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 16:15:05.000000 sqllineage-1.4.6/tests/sql/table/object_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-30 16:15:05.000000 sqllineage-1.4.6/tests/sql/table/object_storage/test_path_dialect_specific.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:17:32.602016 sqllineage-1.4.6/tests/sql/table/other_single_statement/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 16:15:05.000000 sqllineage-1.4.6/tests/sql/table/other_single_statement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-30 16:15:05.000000 sqllineage-1.4.6/tests/sql/table/other_single_statement/test_other_with_lineage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-30 16:15:05.000000 sqllineage-1.4.6/tests/sql/table/other_single_statement/test_other_with_lineage_dialect_specific.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-30 16:15:05.000000 sqllineage-1.4.6/tests/sql/table/other_single_statement/test_other_without_lineage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-07-30 16:15:05.000000 sqllineage-1.4.6/tests/sql/table/other_single_statement/test_other_without_lineage_dialect_specific.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-30 16:15:05.000000 sqllineage-1.4.6/tests/sql/table/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-07-30 16:15:05.000000 sqllineage-1.4.6/tests/sql/table/test_create_dialect_specific.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-30 16:15:05.000000 sqllineage-1.4.6/tests/sql/table/test_cte.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-30 16:15:05.000000 sqllineage-1.4.6/tests/sql/table/test_cte_dialect_specific.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-30 16:15:05.000000 sqllineage-1.4.6/tests/sql/table/test_insert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-07-30 16:15:05.000000 sqllineage-1.4.6/tests/sql/table/test_insert_dialect_specific.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-30 16:15:05.000000 sqllineage-1.4.6/tests/sql/table/test_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-30 16:15:05.000000 sqllineage-1.4.6/tests/sql/table/test_merge_dialect_specific.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-07-30 16:15:05.000000 sqllineage-1.4.6/tests/sql/table/test_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-07-30 16:15:05.000000 sqllineage-1.4.6/tests/sql/table/test_select_dialect_specific.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-30 16:15:05.000000 sqllineage-1.4.6/tests/sql/table/test_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-30 16:15:05.000000 sqllineage-1.4.6/tests/sql/table/test_update_dialect_specific.py
```

### Comparing `sqllineage-1.4.5/LICENSE` & `sqllineage-1.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/PKG-INFO` & `sqllineage-1.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqllineage
-Version: 1.4.5
+Version: 1.4.6
 Summary: SQL Lineage Analysis Tool powered by Python
 Home-page: https://github.com/reata/sqllineage
 Author: Reata
 Author-email: reddevil.hjw@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sqllineage-1.4.5/README.md` & `sqllineage-1.4.6/README.md`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/setup.py` & `sqllineage-1.4.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: CPython",
     ],
     python_requires=">=3.8",
     install_requires=[
         "sqlparse>=0.4.4",
         "networkx>=2.4",
-        "sqlfluff>=2.0.0,<=2.0.3",
+        "sqlfluff>=2.1.4",
     ],
     entry_points={"console_scripts": ["sqllineage = sqllineage.cli:main"]},
     extras_require={
         "ci": [
             "bandit",
             "black",
             "flake8",
```

### Comparing `sqllineage-1.4.5/sqllineage/__init__.py` & `sqllineage-1.4.6/sqllineage/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 
 NAME = "sqllineage"
-VERSION = "1.4.5"
+VERSION = "1.4.6"
 DEFAULT_LOGGING = {
     "version": 1,
     "disable_existing_loggers": False,
     "formatters": {"default": {"format": "%(levelname)s: %(message)s"}},
     "handlers": {
         "console": {
             "level": "WARNING",
```

### Comparing `sqllineage-1.4.5/sqllineage/build/asset-manifest.json` & `sqllineage-1.4.6/sqllineage/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/build/editor.worker.js` & `sqllineage-1.4.6/sqllineage/build/editor.worker.js`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/build/editor.worker.js.map` & `sqllineage-1.4.6/sqllineage/build/editor.worker.js.map`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/build/favicon.ico` & `sqllineage-1.4.6/sqllineage/build/favicon.ico`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/build/index.html` & `sqllineage-1.4.6/sqllineage/build/index.html`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/build/logo192.png` & `sqllineage-1.4.6/sqllineage/build/logo192.png`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/build/logo512.png` & `sqllineage-1.4.6/sqllineage/build/logo512.png`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/build/static/css/main.c1b86fee.css` & `sqllineage-1.4.6/sqllineage/build/static/css/main.c1b86fee.css`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/build/static/css/main.c1b86fee.css.map` & `sqllineage-1.4.6/sqllineage/build/static/css/main.c1b86fee.css.map`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/build/static/js/333.97bcedbd.chunk.js` & `sqllineage-1.4.6/sqllineage/build/static/js/333.97bcedbd.chunk.js`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/build/static/js/333.97bcedbd.chunk.js.map` & `sqllineage-1.4.6/sqllineage/build/static/js/333.97bcedbd.chunk.js.map`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/build/static/js/main.e83a4547.js` & `sqllineage-1.4.6/sqllineage/build/static/js/main.e83a4547.js`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/build/static/js/main.e83a4547.js.LICENSE.txt` & `sqllineage-1.4.6/sqllineage/build/static/js/main.e83a4547.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/build/static/js/main.e83a4547.js.map` & `sqllineage-1.4.6/sqllineage/build/static/js/main.e83a4547.js.map`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/build/static/media/codicon.4168b9c11e5075e9cfe6.ttf` & `sqllineage-1.4.6/sqllineage/build/static/media/codicon.4168b9c11e5075e9cfe6.ttf`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/cli.py` & `sqllineage-1.4.6/sqllineage/cli.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/core/holders.py` & `sqllineage-1.4.6/sqllineage/core/holders.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/core/models.py` & `sqllineage-1.4.6/sqllineage/core/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,35 +185,35 @@
     def to_source_columns(self, alias_mapping: Dict[str, Union[Path, Table, SubQuery]]):
         """
         Best guess for source table given all the possible table/subquery and their alias.
         """
 
         def _to_src_col(
             name: str, parent: Optional[Union[Path, Table, SubQuery]] = None
-        ):
+        ) -> Column:
             col = Column(name)
             if parent:
                 col.parent = parent
             return col
 
         source_columns = set()
         for src_col, qualifier in self.source_columns:
             if qualifier is None:
                 if src_col == "*":
                     # select *
                     for table in set(alias_mapping.values()):
                         source_columns.add(_to_src_col(src_col, table))
                 else:
                     # select unqualified column
-                    src_col = _to_src_col(src_col, None)
+                    source = _to_src_col(src_col, None)
                     for table in set(alias_mapping.values()):
                         # in case of only one table, we get the right answer
                         # in case of multiple tables, a bunch of possible tables are set
-                        src_col.parent = table
-                    source_columns.add(src_col)
+                        source.parent = table
+                    source_columns.add(source)
             else:
                 if alias_mapping.get(qualifier):
                     source_columns.add(
                         _to_src_col(src_col, alias_mapping.get(qualifier))
                     )
                 else:
                     source_columns.add(_to_src_col(src_col, Table(qualifier)))
```

### Comparing `sqllineage-1.4.5/sqllineage/core/parser/__init__.py` & `sqllineage-1.4.6/sqllineage/core/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/core/parser/sqlfluff/analyzer.py` & `sqllineage-1.4.6/sqllineage/core/parser/sqlfluff/analyzer.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/core/parser/sqlfluff/extractors/cte_extractor.py` & `sqllineage-1.4.6/sqllineage/core/parser/sqlfluff/extractors/cte_extractor.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from sqllineage.core.parser.sqlfluff.extractors.dml_select_extractor import (
     DmlSelectExtractor,
 )
 from sqllineage.core.parser.sqlfluff.extractors.lineage_holder_extractor import (
     LineageHolderExtractor,
 )
 from sqllineage.core.parser.sqlfluff.models import SqlFluffSubQuery
-from sqllineage.core.parser.sqlfluff.utils import has_alias, retrieve_segments
+from sqllineage.core.parser.sqlfluff.utils import has_alias, list_child_segments
 
 
 class DmlCteExtractor(LineageHolderExtractor):
     """
     DML CTE queries lineage extractor
     """
 
@@ -34,25 +34,17 @@
         """
         Extract lineage for a given statement.
         :param statement: a sqlfluff segment with a statement
         :param context: 'AnalyzerContext'
         :param is_sub_query: determine if the statement is bracketed or not
         :return 'SubQueryLineageHolder' object
         """
-        handlers, _ = self._init_handlers()
-
         holder = self._init_holder(context)
-
         subqueries = []
-        segments = retrieve_segments(statement)
-
-        for segment in segments:
-            for current_handler in handlers:
-                current_handler.handle(segment, holder)
-
+        for segment in list_child_segments(statement):
             if segment.type in ["select_statement", "set_expression"]:
                 holder |= DmlSelectExtractor(self.dialect).extract(
                     segment,
                     AnalyzerContext(prev_cte=holder.cte, prev_write=holder.write),
                 )
 
             if segment.type == "insert_statement":
@@ -60,15 +52,15 @@
                     segment,
                     AnalyzerContext(prev_cte=holder.cte),
                 )
 
             identifier = None
             if segment.type == "common_table_expression":
                 segment_has_alias = has_alias(segment)
-                sub_segments = retrieve_segments(segment)
+                sub_segments = list_child_segments(segment)
                 for sub_segment in sub_segments:
                     if sub_segment.type == "identifier":
                         identifier = sub_segment.raw
                         if not segment_has_alias:
                             holder.add_cte(SqlFluffSubQuery.of(sub_segment, identifier))
                     if sub_segment.type == "bracketed":
                         for sq in self.parse_subquery(sub_segment):
```

### Comparing `sqllineage-1.4.5/sqllineage/core/parser/sqlfluff/extractors/ddl_alter_extractor.py` & `sqllineage-1.4.6/sqllineage/core/parser/sqlfluff/extractors/ddl_alter_extractor.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/core/parser/sqlfluff/extractors/ddl_drop_extractor.py` & `sqllineage-1.4.6/sqllineage/core/parser/sqlfluff/extractors/ddl_drop_extractor.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/core/parser/sqlfluff/extractors/dml_insert_extractor.py` & `sqllineage-1.4.6/sqllineage/core/parser/sqlfluff/extractors/dml_insert_extractor.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 from typing import Optional
 
 from sqlfluff.core.parser import BaseSegment
 
 from sqllineage.core.holders import SubQueryLineageHolder
-from sqllineage.core.models import AnalyzerContext
+from sqllineage.core.models import AnalyzerContext, Path
 from sqllineage.core.parser.sqlfluff.extractors.dml_select_extractor import (
     DmlSelectExtractor,
 )
 from sqllineage.core.parser.sqlfluff.extractors.lineage_holder_extractor import (
     LineageHolderExtractor,
 )
+from sqllineage.core.parser.sqlfluff.handlers.target import TargetHandler
 from sqllineage.core.parser.sqlfluff.models import SqlFluffSubQuery
-from sqllineage.core.parser.sqlfluff.utils import get_child, is_union, retrieve_segments
+from sqllineage.core.parser.sqlfluff.utils import (
+    get_child,
+    get_grandchildren,
+    is_union,
+    list_child_segments,
+)
 
 
 class DmlInsertExtractor(LineageHolderExtractor):
     """
     DML Insert queries lineage extractor
     """
 
@@ -43,23 +49,17 @@
         """
         Extract lineage for a given statement.
         :param statement: a sqlfluff segment with a statement
         :param context: 'AnalyzerContext'
         :param is_sub_query: determine if the statement is bracketed or not
         :return 'SubQueryLineageHolder' object
         """
-        handlers, conditional_handlers = self._init_handlers()
-
+        target_handler = TargetHandler()
         holder = self._init_holder(context)
-
-        segments = retrieve_segments(statement)
-        for segment in segments:
-            for current_handler in handlers:
-                current_handler.handle(segment, holder)
-
+        for segment in list_child_segments(statement):
             if segment.type == "with_compound_statement":
                 from .cte_extractor import DmlCteExtractor
 
                 holder |= DmlCteExtractor(self.dialect).extract(
                     segment,
                     AnalyzerContext(prev_cte=holder.cte, prev_write=holder.write),
                 )
@@ -86,23 +86,32 @@
                     self._extract_select(holder, subquery_segment)
                 elif subquery_segment := get_child(segment, "set_expression"):
                     self._extract_set(holder, subquery_segment)
             elif segment.type == "select_statement":
                 self._extract_select(holder, segment)
             elif segment.type == "set_expression":
                 self._extract_set(holder, segment)
+            elif segment.type == "from_clause":
+                for s in segment.segments:
+                    if s.type == "from_expression":
+                        for table_expression in get_grandchildren(
+                            s, "from_expression_element", "table_expression"
+                        ):
+                            if storage_location := table_expression.get_child(
+                                "storage_location"
+                            ):
+                                holder.add_read(Path(storage_location.raw))
             else:
-                for conditional_handler in conditional_handlers:
-                    if conditional_handler.indicate(segment):
-                        conditional_handler.handle(segment, holder)
+                if target_handler.indicate(segment):
+                    target_handler.handle(segment, holder)
 
         return holder
 
     def _extract_set(self, holder: SubQueryLineageHolder, set_segment: BaseSegment):
-        for sub_segment in retrieve_segments(set_segment):
+        for sub_segment in list_child_segments(set_segment):
             if sub_segment.type == "select_statement":
                 self._extract_select(holder, sub_segment, set_segment)
 
     def _extract_select(
         self,
         holder: SubQueryLineageHolder,
         select_segment: BaseSegment,
```

### Comparing `sqllineage-1.4.5/sqllineage/core/parser/sqlfluff/extractors/dml_merge_extractor.py` & `sqllineage-1.4.6/sqllineage/core/parser/sqlfluff/extractors/dml_merge_extractor.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     LineageHolderExtractor,
 )
 from sqllineage.core.parser.sqlfluff.models import SqlFluffSubQuery, SqlFluffTable
 from sqllineage.core.parser.sqlfluff.utils import (
     get_grandchildren,
     get_identifier,
     get_innermost_bracketed,
-    retrieve_segments,
+    list_child_segments,
 )
 
 
 class DmlMergeExtractor(LineageHolderExtractor):
     """
     DDL Alter queries lineage extractor
     """
@@ -35,15 +35,15 @@
         statement: BaseSegment,
         context: AnalyzerContext,
         is_sub_query: bool = False,
     ) -> SubQueryLineageHolder:
         holder = StatementLineageHolder()
         src_flag = tgt_flag = False
         direct_source: Optional[Union[Table, SubQuery]] = None
-        segments = retrieve_segments(statement)
+        segments = list_child_segments(statement)
         for i, segment in enumerate(segments):
             if segment.type == "keyword" and segment.raw_upper in {"INTO", "MERGE"}:
                 tgt_flag = True
                 continue
             if segment.type == "keyword" and segment.raw_upper == "USING":
                 src_flag = True
                 continue
@@ -107,16 +107,18 @@
                 for c in merge_insert.get_child("bracketed").get_children(
                     "column_reference"
                 ):
                     tgt_col = Column(get_identifier(c))
                     tgt_col.parent = list(holder.write)[0]
                     insert_columns.append(tgt_col)
                 for j, e in enumerate(
-                    merge_insert.get_child("values_clause")
+                    segment
+                    for segment in merge_insert.get_child("values_clause")
                     .get_child("bracketed")
-                    .get_children("expression")
+                    .segments
+                    if segment.type in ("literal", "expression")
                 ):
                     if col_ref := e.get_child("column_reference"):
                         src_col = Column(get_identifier(col_ref))
                         src_col.parent = direct_source
                         holder.add_column_lineage(src_col, insert_columns[j])
         return holder
```

### Comparing `sqllineage-1.4.5/sqllineage/core/parser/sqlfluff/extractors/dml_select_extractor.py` & `sqllineage-1.4.6/sqllineage/core/parser/sqlfluff/extractors/dml_select_extractor.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 from sqlfluff.core.parser import BaseSegment
 
 from sqllineage.core.holders import SubQueryLineageHolder
 from sqllineage.core.models import AnalyzerContext
 from sqllineage.core.parser.sqlfluff.extractors.lineage_holder_extractor import (
     LineageHolderExtractor,
 )
-from sqllineage.core.parser.sqlfluff.models import SqlFluffSubQuery
+from sqllineage.core.parser.sqlfluff.handlers.base import ConditionalSegmentBaseHandler
+from sqllineage.core.parser.sqlfluff.models import SqlFluffSubQuery, SqlFluffTable
 from sqllineage.core.parser.sqlfluff.utils import (
-    retrieve_segments,
+    get_grandchild,
+    get_grandchildren,
+    list_child_segments,
 )
+from sqllineage.utils.helpers import escape_identifier_name
 
 
 class DmlSelectExtractor(LineageHolderExtractor):
     """
     DML Select queries lineage extractor
     """
 
@@ -30,40 +34,66 @@
         """
         Extract lineage for a given statement.
         :param statement: a sqlfluff segment with a statement
         :param context: 'AnalyzerContext'
         :param is_sub_query: determine if the statement is bracketed or not
         :return 'SubQueryLineageHolder' object
         """
-        handlers, conditional_handlers = self._init_handlers()
+        # to support SELECT INTO in some dialects, we also need to initialize target handler here
+        handlers = [
+            handler_cls()
+            for handler_cls in ConditionalSegmentBaseHandler.__subclasses__()
+        ]
         holder = self._init_holder(context)
         subqueries = [SqlFluffSubQuery.of(statement, None)] if is_sub_query else []
         segments = (
             [statement]
             if statement.type == "set_expression"
-            else retrieve_segments(statement)
+            else list_child_segments(statement)
         )
         for segment in segments:
             for sq in self.parse_subquery(segment):
                 # Collecting subquery on the way, hold on parsing until last
                 # so that each handler don't have to worry about what's inside subquery
                 subqueries.append(sq)
 
-            for current_handler in handlers:
-                current_handler.handle(segment, holder)
+            self._handle_swap_partition(segment, holder)
 
-            for conditional_handler in conditional_handlers:
-                if conditional_handler.indicate(segment):
-                    conditional_handler.handle(segment, holder)
+            for handler in handlers:
+                if handler.indicate(segment):
+                    handler.handle(segment, holder)
 
         # call end of query hook here as loop is over
-        for conditional_handler in conditional_handlers:
-            conditional_handler.end_of_query_cleanup(holder)
+        for handler in handlers:
+            handler.end_of_query_cleanup(holder)
 
         # By recursively extracting each subquery of the parent and merge, we're doing Depth-first search
         for sq in subqueries:
             holder |= self.extract(sq.query, AnalyzerContext(sq, holder.cte))
 
         for sq in holder.extra_subqueries:
             holder |= self.extract(sq.query, AnalyzerContext(sq, holder.cte))
 
         return holder
+
+    @staticmethod
+    def _handle_swap_partition(segment: BaseSegment, holder: SubQueryLineageHolder):
+        """
+        A handler for swap_partitions_between_tables function
+        """
+        function_from_select = get_grandchild(
+            segment, "select_clause_element", "function"
+        )
+        if (
+            function_from_select
+            and function_from_select.first_non_whitespace_segment_raw_upper
+            == "SWAP_PARTITIONS_BETWEEN_TABLES"
+        ):
+            function_parameters = get_grandchildren(
+                function_from_select, "bracketed", "expression"
+            )
+            holder.add_read(
+                SqlFluffTable(escape_identifier_name(function_parameters[0].raw))
+            )
+            holder.add_write(
+                SqlFluffTable(escape_identifier_name(function_parameters[3].raw))
+            )
```

### Comparing `sqllineage-1.4.5/sqllineage/core/parser/sqlfluff/extractors/lineage_holder_extractor.py` & `sqllineage-1.4.6/sqllineage/core/parser/sqlfluff/extractors/lineage_holder_extractor.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 from functools import reduce
 from operator import add
-from typing import List, Tuple
+from typing import List
 
 from sqlfluff.core.parser import BaseSegment
 
 from sqllineage.core.holders import SubQueryLineageHolder
 from sqllineage.core.models import AnalyzerContext, SubQuery
-from sqllineage.core.parser.sqlfluff.handlers.base import (
-    ConditionalSegmentBaseHandler,
-    SegmentBaseHandler,
-)
 from sqllineage.core.parser.sqlfluff.models import SqlFluffSubQuery
 from sqllineage.core.parser.sqlfluff.utils import (
-    get_multiple_identifiers,
     get_subqueries,
     is_subquery,
+    list_from_expression,
 )
 from sqllineage.utils.entities import SubQueryTuple
 
 
 class LineageHolderExtractor:
     """
     Abstract class implementation for extract 'SubQueryLineageHolder' from different statement types
@@ -56,15 +52,15 @@
         """
         The parse_subquery function takes a segment as an argument.
         :param segment: segment to determine if it is a subquery
         :return: A list of `SqlFluffSubQuery` objects, otherwise, if the segment is not matching any of the expected
         types it returns an empty list.
         """
         result: List[SubQuery] = []
-        identifiers = get_multiple_identifiers(segment)
+        identifiers = list_from_expression(segment)
         if identifiers and len(identifiers) > 1:
             # for SQL89 style of JOIN or multiple CTEs, this is actually SubQueries
             return reduce(
                 add,
                 [
                     cls._parse_subquery(get_subqueries(identifier))
                     for identifier in identifiers
@@ -86,30 +82,14 @@
         :return:  a list of 'SqlFluffSubQuery'
         """
         return [
             SqlFluffSubQuery.of(bracketed_segment, alias)
             for bracketed_segment, alias in subqueries
         ]
 
-    def _init_handlers(
-        self,
-    ) -> Tuple[List[SegmentBaseHandler], List[ConditionalSegmentBaseHandler]]:
-        """
-        Initialize handlers used during the extraction of lineage
-        :return: A tuple with a list of SegmentBaseHandler and ConditionalSegmentBaseHandler
-        """
-        handlers: List[SegmentBaseHandler] = [
-            handler_cls() for handler_cls in SegmentBaseHandler.__subclasses__()
-        ]
-        conditional_handlers = [
-            handler_cls()
-            for handler_cls in ConditionalSegmentBaseHandler.__subclasses__()
-        ]
-        return handlers, conditional_handlers
-
     @staticmethod
     def _init_holder(context: AnalyzerContext) -> SubQueryLineageHolder:
         """
         Initialize lineage holder for a given 'AnalyzerContext'
         :param context: a previous context that the lineage extractor must consider
         :return: an initialized SubQueryLineageHolder
         """
```

### Comparing `sqllineage-1.4.5/sqllineage/core/parser/sqlfluff/extractors/noop_extractor.py` & `sqllineage-1.4.6/sqllineage/core/parser/sqlfluff/extractors/noop_extractor.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/core/parser/sqlfluff/handlers/base.py` & `sqllineage-1.4.6/sqllineage/core/parser/sqlfluff/handlers/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -26,20 +26,7 @@
 
     def end_of_query_cleanup(self, holder: SubQueryLineageHolder) -> None:
         """
         Optional method to be called at the end of statement or subquery
         :param holder: 'SubQueryLineageHolder' to hold lineage
         """
         pass
-
-
-class SegmentBaseHandler:
-    """
-    Extract lineage from a specific segment
-    """
-
-    def handle(self, segment: BaseSegment, holder: SubQueryLineageHolder) -> None:
-        """
-        :param segment: segment to be handled
-        :param holder: 'SubQueryLineageHolder' to hold lineage
-        """
-        raise NotImplementedError
```

### Comparing `sqllineage-1.4.5/sqllineage/core/parser/sqlfluff/handlers/target.py` & `sqllineage-1.4.6/sqllineage/core/parser/sqlfluff/handlers/target.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from sqllineage.core.parser.sqlfluff.models import (
     SqlFluffColumn,
     SqlFluffTable,
 )
 from sqllineage.core.parser.sqlfluff.utils import (
     find_table_identifier,
     get_child,
-    retrieve_segments,
+    list_child_segments,
 )
 from sqllineage.utils.helpers import escape_identifier_name
 
 
 class TargetHandler(ConditionalSegmentBaseHandler):
     """
     Target table handler
@@ -109,29 +109,29 @@
 
         elif segment.type == "from_expression":
             from_expression_element = get_child(segment, "from_expression_element")
             if from_expression_element:
                 table_identifier = find_table_identifier(from_expression_element)
                 all_segments = [
                     seg
-                    for seg in retrieve_segments(from_expression_element)
+                    for seg in list_child_segments(from_expression_element)
                     if seg.type != "keyword"
                 ]
                 if table_identifier:
                     write = retrieve_holder_data_from(
                         all_segments, holder, table_identifier
                     )
                     if write:
                         holder.add_write(write)
             join_clause = get_child(segment, "join_clause")
             if from_expression_element:
                 table_identifier = find_table_identifier(join_clause)
                 all_segments = [
                     seg
-                    for seg in retrieve_segments(join_clause)
+                    for seg in list_child_segments(join_clause)
                     if seg.type != "keyword"
                 ]
                 if table_identifier:
                     read = retrieve_holder_data_from(
                         all_segments, holder, table_identifier
                     )
                     if read:
@@ -139,15 +139,15 @@
 
         elif segment.type == "bracketed":
             """
             In case of bracketed column reference, add these target columns to holder
             so that when we compute the column level lineage
             we keep these columns into consideration
             """
-            sub_segments = retrieve_segments(segment)
+            sub_segments = list_child_segments(segment)
             if all(
                 sub_segment.type == "column_reference" for sub_segment in sub_segments
             ):
                 # target columns only apply to bracketed column references
                 holder.add_target_column(
                     *[SqlFluffColumn.of(sub_segment) for sub_segment in sub_segments]
                 )
```

### Comparing `sqllineage-1.4.5/sqllineage/core/parser/sqlfluff/holder_utils.py` & `sqllineage-1.4.6/sqllineage/core/parser/sqlfluff/holder_utils.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/core/parser/sqlfluff/models.py` & `sqllineage-1.4.6/sqllineage/core/parser/sqlfluff/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from sqllineage import SQLPARSE_DIALECT
 from sqllineage.core.models import Column, Schema, SubQuery, Table
 from sqllineage.core.parser.sqlfluff.utils import (
     get_identifier,
     is_subquery,
     is_wildcard,
-    retrieve_segments,
+    list_child_segments,
 )
 from sqllineage.utils.entities import ColumnQualifierTuple
 from sqllineage.utils.helpers import escape_identifier_name
 
 NON_IDENTIFIER_OR_COLUMN_SEGMENT_TYPE = [
     "function",
     "over_clause",
@@ -105,28 +105,29 @@
             source_columns, alias = SqlFluffColumn._get_column_and_alias(column)
             if alias:
                 return Column(
                     alias,
                     source_columns=source_columns,
                 )
             if source_columns:
-                sub_segments = retrieve_segments(column)
                 column_name = None
-                for sub_segment in sub_segments:
+                for sub_segment in list_child_segments(column):
                     if sub_segment.type == "column_reference":
                         column_name = get_identifier(sub_segment)
                     elif sub_segment.type == "expression":
                         # special handling for postgres style type cast, col as target column name instead of col::type
-                        if len(sub2_segments := retrieve_segments(sub_segment)) == 1:
+                        if len(sub2_segments := list_child_segments(sub_segment)) == 1:
                             if (
                                 sub2_segment := sub2_segments[0]
                             ).type == "cast_expression":
                                 if (
                                     len(
-                                        sub3_segments := retrieve_segments(sub2_segment)
+                                        sub3_segments := list_child_segments(
+                                            sub2_segment
+                                        )
                                     )
                                     == 2
                                 ):
                                     if (
                                         sub3_segment := sub3_segments[0]
                                     ).type == "column_reference":
                                         column_name = get_identifier(sub3_segment)
@@ -150,15 +151,15 @@
         """
         if segment.type == "identifier" or is_wildcard(segment):
             return [ColumnQualifierTuple(segment.raw, None)]
         if segment.type == "column_reference":
             parent, column = SqlFluffColumn._get_column_and_parent(segment)
             return [ColumnQualifierTuple(column, parent)]
         if segment.type in NON_IDENTIFIER_OR_COLUMN_SEGMENT_TYPE:
-            sub_segments = retrieve_segments(segment)
+            sub_segments = list_child_segments(segment)
             col_list = []
             for sub_segment in sub_segments:
                 if sub_segment.type == "bracketed":
                     if is_subquery(sub_segment):
                         col_list += SqlFluffColumn._get_column_from_subquery(
                             sub_segment
                         )
@@ -215,25 +216,25 @@
 
     @staticmethod
     def _get_column_and_alias(
         segment: BaseSegment, check_bracketed: bool = True
     ) -> Tuple[List[ColumnQualifierTuple], Optional[str]]:
         alias = None
         columns = []
-        sub_segments = retrieve_segments(segment, check_bracketed)
+        sub_segments = list_child_segments(segment, check_bracketed)
         for sub_segment in sub_segments:
             if sub_segment.type == "alias_expression":
                 alias = get_identifier(sub_segment)
             elif sub_segment.type in SOURCE_COLUMN_SEGMENT_TYPE or is_wildcard(
                 sub_segment
             ):
                 res = SqlFluffColumn._extract_source_columns(sub_segment)
                 columns += res if res else []
 
         return columns, alias
 
     @staticmethod
     def _get_column_and_parent(col_segment: BaseSegment) -> Tuple[Optional[str], str]:
-        identifiers = retrieve_segments(col_segment)
+        identifiers = list_child_segments(col_segment)
         if len(identifiers) > 1:
             return identifiers[-2].raw, identifiers[-1].raw
         return None, identifiers[-1].raw
```

### Comparing `sqllineage-1.4.5/sqllineage/core/parser/sqlfluff/utils.py` & `sqllineage-1.4.6/sqllineage/core/parser/sqlfluff/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Utils class to deal with the sqlfluff segments manipulations
 """
 import re
-from typing import Any, Iterable, List, Optional, Tuple
+from typing import Any, List, Optional, Tuple
 
 from sqlfluff.core.linter import ParsedString
 from sqlfluff.core.parser import BaseSegment
 
 from sqllineage.utils.entities import SubQueryTuple
 
 
@@ -27,15 +27,15 @@
     segment: BaseSegment,
 ) -> Tuple[BaseSegment, BaseSegment]:
     """
     :param segment: segment to be processed
     :return: a Tuple of "alias_expression" and the target table
     """
     as_segment = segment.get_child("alias_expression")
-    sublist = retrieve_segments(segment, False)
+    sublist = list_child_segments(segment, False)
     target = sublist[0] if is_subquery(sublist[0]) else sublist[0].segments[0]
     return as_segment, target
 
 
 def get_subqueries(segment: BaseSegment) -> List[SubQueryTuple]:
     """
     Retrieve a list of 'SubQueryTuple' based on the type of the segment.
@@ -62,36 +62,37 @@
                     when_clause, from_keyword="THEN", children_segments="expression"
                 ):
                     subquery.append(
                         SubQueryTuple(bracketed_segment, get_identifier(as_segment))
                     )
         return subquery
     elif segment.type in ["from_clause", "from_expression", "from_expression_element"]:
-        as_segment, target = extract_as_and_target_segment(
-            get_inner_from_expression(segment)
-        )
-        if is_subquery(target):
-            as_segment, target = extract_as_and_target_segment(
-                get_inner_from_expression(segment)
-            )
-            subquery = [
-                SubQueryTuple(
-                    get_innermost_bracketed(target) if not is_union(target) else target,
-                    get_identifier(as_segment) if as_segment else None,
+        if from_expression_element := get_from_expression_element(segment):
+            as_segment, target = extract_as_and_target_segment(from_expression_element)
+            if is_subquery(target):
+                as_segment, target = extract_as_and_target_segment(
+                    from_expression_element
                 )
-            ]
+                subquery = [
+                    SubQueryTuple(
+                        get_innermost_bracketed(target)
+                        if not is_union(target)
+                        else target,
+                        get_identifier(as_segment) if as_segment else None,
+                    )
+                ]
         return subquery
     elif segment.type in ["where_clause"]:
         expression_segments = segment.get_child("expression").segments or []
         bracketed_segments = [s for s in expression_segments if s.type == "bracketed"]
         if bracketed_segments and is_subquery(bracketed_segments[0]):
             return [SubQueryTuple(get_innermost_bracketed(bracketed_segments[0]), None)]
         return []
     elif is_union(segment):
-        for s in retrieve_segments(segment, check_bracketed=True):
+        for s in list_child_segments(segment, check_bracketed=True):
             if s.type == "bracketed" or s.type == "select_statement":
                 subquery.append(SubQueryTuple(s, None))
         return subquery
     else:
         raise NotImplementedError()
 
 
@@ -149,37 +150,44 @@
     if segment.get_child("table_expression") and segment.get_child(
         "table_expression"
     ).get_child("values_clause"):
         return True
     return False
 
 
-def get_multiple_identifiers(segment: BaseSegment) -> List[BaseSegment]:
-    """
-    :param segment: segment to be processed
-    :return: a list of segments from a 'from_clause' type segment
-    """
+def list_from_expression(segment: BaseSegment) -> List[BaseSegment]:
     if segment.type == "from_clause":
         return [seg for seg in segment.get_children("from_expression")]
     return []
 
 
-def get_inner_from_expression(segment: BaseSegment) -> BaseSegment:
+def get_from_expression_element(segment: BaseSegment) -> Optional[BaseSegment]:
     """
-    :param segment: segment to be processed
-    :return: a list of segments from a 'from_expression' or 'from_expression_element' segment
+    capable of handing:
+        from_clause as grandparent
+        from_expression/join_clause as parent
+        from_expression_element itself
     """
-    if segment.get_child("from_expression") and segment.get_child(
-        "from_expression"
-    ).get_child("from_expression_element"):
-        return segment.get_child("from_expression").get_child("from_expression_element")
-    elif segment.get_child("from_expression_element"):
-        return segment.get_child("from_expression_element")
-    else:
-        return segment
+    from_expression_element = None
+    if segment.type == "from_clause":
+        if from_expression := segment.get_child("from_expression"):
+            non_bracket = from_expression
+            while non_bracket.get_child("bracketed"):
+                non_bracket = non_bracket.get_child("bracketed")
+            if seg := non_bracket.get_child("from_expression_element"):
+                from_expression_element = seg
+            elif seg := non_bracket.get_child("from_expression"):
+                if sub_seg := seg.get_child("from_expression_element"):
+                    from_expression_element = sub_seg
+    elif segment.type in ("from_expression", "join_clause"):
+        if seg := segment.get_child("from_expression_element"):
+            from_expression_element = seg
+    elif segment.type == "from_expression_element":
+        from_expression_element = segment
+    return from_expression_element
 
 
 def filter_segments_by_keyword(
     statement: BaseSegment,
     from_keyword: Optional[str] = None,
     to_keyword: Optional[str] = None,
     children_segments: Optional[str] = None,
@@ -246,53 +254,45 @@
             else:
                 table_identifier = find_table_identifier(segment)
                 if table_identifier:
                     return table_identifier
     return table_identifier
 
 
-def retrieve_segments(
+def list_child_segments(
     segment: BaseSegment, check_bracketed: bool = True
 ) -> List[BaseSegment]:
     """
-    Filter segments for a given segment's segments if they are not negligible
-    :param segment: segment to be processed
-    :param check_bracketed: process segment if it is of type "bracketed"
-    :return: a list of segments
+    Filter segments for a given segment's children, recursive goes into bracket by default
     """
-    if segment.type == "bracketed" and is_union(segment):
-        result = []
-        for sgmt in segment.segments:
-            if sgmt.type == "set_expression":
-                result = [sgmt]
-        return result
-    elif segment.type == "bracketed" and check_bracketed:
-        segments = [
-            sg
-            for sg in segment.iter_segments(expanding=["expression"], pass_through=True)
-        ]
-        result = []
-        for sgmnt in segments:
-            if sgmnt.type == "column_reference":
-                result.append(sgmnt)
-            else:
-                for sg in sgmnt.segments:
-                    if not is_segment_negligible(sg):
-                        result.append(sg)
-        return result
+    if segment.type == "bracketed" and check_bracketed:
+        if is_union(segment):
+            return [seg for seg in segment.segments if seg.type == "set_expression"]
+        else:
+            result = []
+            for seg in segment.iter_segments(
+                expanding=["expression"], pass_through=True
+            ):
+                if seg.type == "column_reference":
+                    result.append(seg)
+                else:
+                    for s in seg.segments:
+                        if not is_segment_negligible(s):
+                            result.append(s)
+            return result
     else:
-        return [sgmnt for sgmnt in segment.segments if not is_segment_negligible(sgmnt)]
+        return [seg for seg in segment.segments if not is_segment_negligible(seg)]
 
 
 def get_identifier(col_segment: BaseSegment) -> str:
     """
     :param col_segment: column segment
     :return: the table identifier name
     """
-    identifiers = retrieve_segments(col_segment)
+    identifiers = list_child_segments(col_segment)
     col_identifier = identifiers[-1]
     return str(col_identifier.raw)
 
 
 def is_wildcard(symbol: BaseSegment):
     """
     :param symbol: symbol segment
@@ -308,43 +308,40 @@
 def get_table_alias(table_segments: List[BaseSegment]) -> Optional[str]:
     """
     :param table_segments: list of segments to search for an alias
     :return: alias found otherwise None
     """
     alias = None
     if len(table_segments) > 1 and table_segments[1].type == "alias_expression":
-        segments = retrieve_segments(table_segments[1])
+        segments = list_child_segments(table_segments[1])
         alias = segments[1].raw if len(segments) > 1 else segments[0].raw
-    elif (
-        len(table_segments) == 1 and table_segments[0].type == "from_expression_element"
-    ):
-        table_and_alias = retrieve_segments(table_segments[0])
-        if len(table_and_alias) > 1 and table_and_alias[1].type == "alias_expression":
-            segments = retrieve_segments(table_and_alias[1])
-            alias = segments[1].raw if len(segments) > 1 else segments[0].raw
     return str(alias) if alias else None
 
 
 def has_alias(segment: BaseSegment) -> bool:
     """
     :param segment: segment to be processed
     :return: True if the segment contains an alias keyword
     """
     return len([s for s in segment.get_children("keyword") if s.raw_upper == "AS"]) > 0
 
 
-def retrieve_extra_segment(segment: BaseSegment) -> Iterable[BaseSegment]:
+def list_join_clause(segment: BaseSegment) -> List[BaseSegment]:
     """
-    Yield all the extra segments of the segment if it is a 'from_expression' type.
-    :param segment: segment to be processed
+    traverse from_clause, recursively goes into bracket by default
     """
-    if segment.get_child("from_expression"):
-        for sgmnt in segment.get_child("from_expression").segments:
-            if sgmnt.type == "join_clause":
-                yield sgmnt
+    if from_expression := segment.get_child("from_expression"):
+        if bracketed := from_expression.get_child("bracketed"):
+            join_clauses = bracketed.get_children("join_clause")
+            if inner_bracket := bracketed.get_child("bracketed"):
+                join_clauses = list_join_clause(inner_bracket) + join_clauses
+            return join_clauses
+        else:
+            return from_expression.get_children("join_clause")
+    return []
 
 
 def get_grandchild(
     segment: BaseSegment, child: str, grandchild: str
 ) -> Optional[BaseSegment]:
     """
     :param segment: segment to be processed
@@ -395,41 +392,19 @@
             for x in getattr(parsed_string.tree, "segments")
             if x.type == "statement" or x.type == "batch"
         )
     )
 
 
 def is_union(segment: BaseSegment) -> bool:
-    """
-    :param segment: segment to be processed
-    :return: True if the segment contains 'UNION' or 'UNION ALL' keyword
-    """
-    return (
-        len(
-            [
-                s
-                for s in segment.raw_segments
-                if (s.raw_upper == "UNION" or s.raw_upper == "UNION ALL")
-            ]
-        )
-        > 0
+    return segment.type == "set_expression" or any(
+        seg.type == "set_expression" for seg in segment.segments
     )
 
 
-def get_union_subqueries(segment: BaseSegment) -> List[BaseSegment]:
-    """
-    :param segment: segment to be processed
-    :return: a list of subqueries or select statements from a UNION segment
-    """
-    sub_segments = retrieve_segments(segment, check_bracketed=True)
-    return [
-        s for s in sub_segments if s.type == "bracketed" or s.type == "select_statement"
-    ]
-
-
 def is_subquery_statement(stmt: str) -> bool:
     parentheses_regex = r"^\(.*\)"
     return bool(re.match(parentheses_regex, stmt))
 
 
 def remove_statement_parentheses(stmt: str) -> str:
     parentheses_regex = r"^\((.*)\)"
```

### Comparing `sqllineage-1.4.5/sqllineage/core/parser/sqlparse/__init__.py` & `sqllineage-1.4.6/sqllineage/core/parser/sqlparse/__init__.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/core/parser/sqlparse/analyzer.py` & `sqllineage-1.4.6/sqllineage/core/parser/sqlparse/analyzer.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/core/parser/sqlparse/handlers/base.py` & `sqllineage-1.4.6/sqllineage/core/parser/sqlparse/handlers/base.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/core/parser/sqlparse/handlers/cte.py` & `sqllineage-1.4.6/sqllineage/core/parser/sqlparse/handlers/cte.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,10 +24,10 @@
             ]
         else:
             # CREATE TABLE tbl1 (col1 VARCHAR) WITH (bucketed_by = ARRAY['col1'], bucket_count = 256).
             # This syntax is valid for bucketing in Trino and not the CTE, token will be Parenthesis here
             cte = []
         for token in cte:
             sublist = list(token.get_sublists())
-            if sublist:
+            if sublist and not (isinstance(sublist[0], Function)):
                 # CTE: tbl AS (SELECT 1), tbl is alias and (SELECT 1) is subquery Parenthesis
                 holder.add_cte(SqlParseSubQuery.of(sublist[0], token.get_real_name()))
```

### Comparing `sqllineage-1.4.5/sqllineage/core/parser/sqlparse/handlers/source.py` & `sqllineage-1.4.6/sqllineage/core/parser/sqlparse/handlers/source.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,16 +78,23 @@
                 # SELECT col1 FROM (SELECT col2 FROM tab1), the subquery will be parsed as Parenthesis
                 # This syntax without alias for subquery is invalid in MySQL, while valid for SparkSQL
                 self.tables.append(SqlParseSubQuery.of(token, None))
             elif is_values_clause(token):
                 # SELECT * FROM (VALUES ...), no operation needed
                 pass
             else:
-                # SELECT * FROM (tab2), which is valid syntax
-                self._handle(token.tokens[1], holder)
+                # SELECT * FROM (tab2) or SELECT * FROM (tab2 JOIN tab1), which is valid syntax
+                using_flag = False
+                for t in token.tokens:
+                    if t.is_keyword and t.normalized == "USING":
+                        using_flag = True
+                    if isinstance(t, Identifier) or (
+                        isinstance(t, Parenthesis) and using_flag is False
+                    ):
+                        self._handle(t, holder)
         elif token.ttype == Literal.String.Single:
             self.tables.append(Path(token.value))
         elif isinstance(token, Function):
             # functions like unnest or generator can output a sequence of values as source, ignore it for now
             pass
         else:
             raise SQLLineageException(
```

### Comparing `sqllineage-1.4.5/sqllineage/core/parser/sqlparse/handlers/swap_partition.py` & `sqllineage-1.4.6/sqllineage/core/parser/sqlparse/handlers/swap_partition.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/core/parser/sqlparse/handlers/target.py` & `sqllineage-1.4.6/sqllineage/core/parser/sqlparse/handlers/target.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/core/parser/sqlparse/holder_utils.py` & `sqllineage-1.4.6/sqllineage/core/parser/sqlparse/holder_utils.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/core/parser/sqlparse/models.py` & `sqllineage-1.4.6/sqllineage/core/parser/sqlparse/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,25 +63,21 @@
             alias = column.get_alias()
             if alias:
                 # handle column alias, including alias for column name or Case, Function
                 kw_idx, kw = column.token_next_by(m=(T.Keyword, "AS"))
                 if kw_idx is None:
                     # alias without AS
                     kw_idx, _ = column.token_next_by(i=Identifier)
-                if kw_idx is None:
-                    # invalid syntax: col AS, without alias
-                    return Column(alias)
-                else:
-                    idx, _ = column.token_prev(kw_idx, skip_cm=True)
-                    expr = grouping.group(TokenList(column.tokens[: idx + 1]))[0]
-                    source_columns = SqlParseColumn._extract_source_columns(expr)
-                    return Column(
-                        alias,
-                        source_columns=source_columns,
-                    )
+                idx, _ = column.token_prev(kw_idx, skip_cm=True)
+                expr = grouping.group(TokenList(column.tokens[: idx + 1]))[0]
+                source_columns = SqlParseColumn._extract_source_columns(expr)
+                return Column(
+                    alias,
+                    source_columns=source_columns,
+                )
             else:
                 # select column name directly without alias
                 return Column(
                     column.get_real_name(),
                     source_columns=(
                         (column.get_real_name(), column.get_parent_name()),
                     ),
@@ -152,15 +148,15 @@
                 cqt
                 for tk in token.get_sublists()
                 for cqt in SqlParseColumn._extract_source_columns(tk)
             ]
         elif isinstance(token, Identifier):
             real_name = token.get_real_name()
             # ignore function dtypes that don't need to check for extract column
-            FUNC_DTYPE = ["decimal", "numeric"]
+            FUNC_DTYPE = ["decimal", "numeric", "varchar"]
             has_function = any(
                 isinstance(t, Function) and t.get_real_name() not in FUNC_DTYPE
                 for t in token.tokens
             )
             is_kw = (
                 Lexer.get_default_instance().is_keyword(real_name)
                 if real_name is not None
```

### Comparing `sqllineage-1.4.5/sqllineage/core/parser/sqlparse/utils.py` & `sqllineage-1.4.6/sqllineage/core/parser/sqlparse/utils.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query01.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query01.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query02.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query02.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query04.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query04.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query05.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query05.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query06.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query06.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query07.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query07.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query08.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query08.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query09.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query09.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query10.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query10.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query11.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query11.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query12.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query12.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query13.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query13.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query14.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query14.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query15.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query15.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query16.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query16.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query17.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query17.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query18.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query18.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query19.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query19.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query20.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query20.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query21.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query21.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query23.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query23.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query24.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query24.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query25.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query25.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query26.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query26.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query27.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query27.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query28.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query28.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query29.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query29.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query30.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query30.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query31.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query31.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query32.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query32.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query33.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query33.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query34.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query34.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query35.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query35.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query36.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query36.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query37.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query37.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query38.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query38.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query39.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query39.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query40.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query40.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query41.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query41.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query42.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query42.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query43.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query43.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query44.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query44.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query45.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query45.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query46.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query46.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query47.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query47.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query48.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query48.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query49.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query49.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query50.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query50.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query51.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query51.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query53.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query53.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query54.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query54.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query56.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query56.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query57.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query57.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query58.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query58.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query59.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query59.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query60.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query60.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query61.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query61.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query62.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query62.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query63.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query63.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query64.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query64.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query65.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query65.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query66.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query66.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query67.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query67.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query68.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query68.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query69.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query69.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query70.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query70.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query71.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query71.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query72.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query72.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query73.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query73.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query74.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query74.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query75.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query75.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query76.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query76.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query77.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query77.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query78.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query78.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query79.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query79.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query80.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query80.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query81.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query81.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query82.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query82.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query83.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query83.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query84.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query84.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query85.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query85.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query86.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query86.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query87.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query87.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query88.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query88.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query89.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query89.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query90.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query90.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query91.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query91.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query92.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query92.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query93.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query93.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query94.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query94.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query95.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query95.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query97.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query97.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query98.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query98.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/data/tpcds/query99.sql` & `sqllineage-1.4.6/sqllineage/data/tpcds/query99.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/drawing.py` & `sqllineage-1.4.6/sqllineage/drawing.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/io.py` & `sqllineage-1.4.6/sqllineage/io.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/runner.py` & `sqllineage-1.4.6/sqllineage/runner.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage/utils/helpers.py` & `sqllineage-1.4.6/sqllineage/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineage.egg-info/PKG-INFO` & `sqllineage-1.4.6/sqllineage.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqllineage
-Version: 1.4.5
+Version: 1.4.6
 Summary: SQL Lineage Analysis Tool powered by Python
 Home-page: https://github.com/reata/sqllineage
 Author: Reata
 Author-email: reddevil.hjw@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sqllineage-1.4.5/sqllineagejs/package-lock.json` & `sqllineage-1.4.6/sqllineagejs/package-lock.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9165278024734967%*

 * *Differences: {"'dependencies'": "{'@babel/core': {'dependencies': {'semver': {'version': '6.3.1', 'resolved': "*

 * *                   "'https://registry.npmjs.org/semver/-/semver-6.3.1.tgz', 'integrity': "*

 * *                   "'sha512-BR7VvDCVHO+q2xBEWskxS6DJE1qRnb7DxzUrogb71CWoSficBxYsiAGd+Kl0mmq/MprG9yArRkyrQxTO6XjMzA=='}}}, "*

 * *                   "'@babel/eslint-parser': {'dependencies': {'semver': {'version': '6.3.1', "*

 * *                   "'resolved': 'https://registry.npmjs.org/semver/-/semver-6.3.1.tgz', "*

 * *              […]*

```diff
@@ -31,17 +31,17 @@
             "resolved": "https://registry.npmjs.org/@babel/compat-data/-/compat-data-7.22.5.tgz",
             "version": "7.22.5"
         },
         "@babel/core": {
             "dependencies": {
                 "semver": {
                     "dev": true,
-                    "integrity": "sha512-b39TBaTSfV6yBrapU89p5fKekE2m/NwnDocOVruQFS1/veMgdzuPcnOM34M6CwxW8jH/lxEa5rBoDeUwu5HHTw==",
-                    "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.0.tgz",
-                    "version": "6.3.0"
+                    "integrity": "sha512-BR7VvDCVHO+q2xBEWskxS6DJE1qRnb7DxzUrogb71CWoSficBxYsiAGd+Kl0mmq/MprG9yArRkyrQxTO6XjMzA==",
+                    "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.1.tgz",
+                    "version": "6.3.1"
                 }
             },
             "dev": true,
             "integrity": "sha512-SBuTAjg91A3eKOvD+bPEz3LlhHZRNu1nFOVts9lzDJTXshHTjII0BAtDS3Y2DAkdZdDKWVZGVwkDfc4Clxn1dg==",
             "requires": {
                 "@ampproject/remapping": "^2.2.0",
                 "@babel/code-frame": "^7.22.5",
@@ -68,17 +68,17 @@
                     "dev": true,
                     "integrity": "sha512-0rSmRBzXgDzIsD6mGdJgevzgezI534Cer5L/vyMX0kHzT/jiB43jRhd9YUlMGYLQy2zprNmoT8qasCGtY+QaKw==",
                     "resolved": "https://registry.npmjs.org/eslint-visitor-keys/-/eslint-visitor-keys-2.1.0.tgz",
                     "version": "2.1.0"
                 },
                 "semver": {
                     "dev": true,
-                    "integrity": "sha512-b39TBaTSfV6yBrapU89p5fKekE2m/NwnDocOVruQFS1/veMgdzuPcnOM34M6CwxW8jH/lxEa5rBoDeUwu5HHTw==",
-                    "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.0.tgz",
-                    "version": "6.3.0"
+                    "integrity": "sha512-BR7VvDCVHO+q2xBEWskxS6DJE1qRnb7DxzUrogb71CWoSficBxYsiAGd+Kl0mmq/MprG9yArRkyrQxTO6XjMzA==",
+                    "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.1.tgz",
+                    "version": "6.3.1"
                 }
             },
             "dev": true,
             "integrity": "sha512-C69RWYNYtrgIRE5CmTd77ZiLDXqgBipahJc/jHP3sLcAGj6AJzxNIuKNpVnICqbyK7X3pFUfEvL++rvtbQpZkQ==",
             "requires": {
                 "@nicolo-ribaudo/eslint-scope-5-internals": "5.1.1-v1",
                 "eslint-visitor-keys": "^2.1.0",
@@ -126,17 +126,17 @@
                         "yallist": "^3.0.2"
                     },
                     "resolved": "https://registry.npmjs.org/lru-cache/-/lru-cache-5.1.1.tgz",
                     "version": "5.1.1"
                 },
                 "semver": {
                     "dev": true,
-                    "integrity": "sha512-b39TBaTSfV6yBrapU89p5fKekE2m/NwnDocOVruQFS1/veMgdzuPcnOM34M6CwxW8jH/lxEa5rBoDeUwu5HHTw==",
-                    "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.0.tgz",
-                    "version": "6.3.0"
+                    "integrity": "sha512-BR7VvDCVHO+q2xBEWskxS6DJE1qRnb7DxzUrogb71CWoSficBxYsiAGd+Kl0mmq/MprG9yArRkyrQxTO6XjMzA==",
+                    "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.1.tgz",
+                    "version": "6.3.1"
                 },
                 "yallist": {
                     "dev": true,
                     "integrity": "sha512-a4UGQaWPH59mOXUYnAG2ewncQS4i4F43Tv3JoAM+s2VDAmS9NsK8GpDMLrCHPksFT7h3K6TOoUNn2pb7RoXx4g==",
                     "resolved": "https://registry.npmjs.org/yallist/-/yallist-3.1.1.tgz",
                     "version": "3.1.1"
                 }
@@ -153,17 +153,17 @@
             "resolved": "https://registry.npmjs.org/@babel/helper-compilation-targets/-/helper-compilation-targets-7.22.5.tgz",
             "version": "7.22.5"
         },
         "@babel/helper-create-class-features-plugin": {
             "dependencies": {
                 "semver": {
                     "dev": true,
-                    "integrity": "sha512-b39TBaTSfV6yBrapU89p5fKekE2m/NwnDocOVruQFS1/veMgdzuPcnOM34M6CwxW8jH/lxEa5rBoDeUwu5HHTw==",
-                    "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.0.tgz",
-                    "version": "6.3.0"
+                    "integrity": "sha512-BR7VvDCVHO+q2xBEWskxS6DJE1qRnb7DxzUrogb71CWoSficBxYsiAGd+Kl0mmq/MprG9yArRkyrQxTO6XjMzA==",
+                    "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.1.tgz",
+                    "version": "6.3.1"
                 }
             },
             "dev": true,
             "integrity": "sha512-xkb58MyOYIslxu3gKmVXmjTtUPvBU4odYzbiIQbWwLKIHCsx6UGZGX6F1IznMFVnDdirseUZopzN+ZRt8Xb33Q==",
             "requires": {
                 "@babel/helper-annotate-as-pure": "^7.22.5",
                 "@babel/helper-environment-visitor": "^7.22.5",
@@ -178,17 +178,17 @@
             "resolved": "https://registry.npmjs.org/@babel/helper-create-class-features-plugin/-/helper-create-class-features-plugin-7.22.5.tgz",
             "version": "7.22.5"
         },
         "@babel/helper-create-regexp-features-plugin": {
             "dependencies": {
                 "semver": {
                     "dev": true,
-                    "integrity": "sha512-b39TBaTSfV6yBrapU89p5fKekE2m/NwnDocOVruQFS1/veMgdzuPcnOM34M6CwxW8jH/lxEa5rBoDeUwu5HHTw==",
-                    "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.0.tgz",
-                    "version": "6.3.0"
+                    "integrity": "sha512-BR7VvDCVHO+q2xBEWskxS6DJE1qRnb7DxzUrogb71CWoSficBxYsiAGd+Kl0mmq/MprG9yArRkyrQxTO6XjMzA==",
+                    "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.1.tgz",
+                    "version": "6.3.1"
                 }
             },
             "dev": true,
             "integrity": "sha512-1VpEFOIbMRaXyDeUwUfmTIxExLwQ+zkW+Bh5zXpApA3oQedBx9v/updixWxnx/bZpKw7u8VxWjb/qWpIcmPq8A==",
             "requires": {
                 "@babel/helper-annotate-as-pure": "^7.22.5",
                 "regexpu-core": "^5.3.1",
@@ -197,17 +197,17 @@
             "resolved": "https://registry.npmjs.org/@babel/helper-create-regexp-features-plugin/-/helper-create-regexp-features-plugin-7.22.5.tgz",
             "version": "7.22.5"
         },
         "@babel/helper-define-polyfill-provider": {
             "dependencies": {
                 "semver": {
                     "dev": true,
-                    "integrity": "sha512-b39TBaTSfV6yBrapU89p5fKekE2m/NwnDocOVruQFS1/veMgdzuPcnOM34M6CwxW8jH/lxEa5rBoDeUwu5HHTw==",
-                    "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.0.tgz",
-                    "version": "6.3.0"
+                    "integrity": "sha512-BR7VvDCVHO+q2xBEWskxS6DJE1qRnb7DxzUrogb71CWoSficBxYsiAGd+Kl0mmq/MprG9yArRkyrQxTO6XjMzA==",
+                    "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.1.tgz",
+                    "version": "6.3.1"
                 }
             },
             "dev": true,
             "integrity": "sha512-RnanLx5ETe6aybRi1cO/edaRH+bNYWaryCEmjDDYyNr4wnSzyOp8T0dWipmqVHKEY3AbVKUom50AKSlj1zmKbg==",
             "requires": {
                 "@babel/helper-compilation-targets": "^7.17.7",
                 "@babel/helper-plugin-utils": "^7.16.7",
@@ -1177,17 +1177,17 @@
             "resolved": "https://registry.npmjs.org/@babel/plugin-transform-reserved-words/-/plugin-transform-reserved-words-7.22.5.tgz",
             "version": "7.22.5"
         },
         "@babel/plugin-transform-runtime": {
             "dependencies": {
                 "semver": {
                     "dev": true,
-                    "integrity": "sha512-b39TBaTSfV6yBrapU89p5fKekE2m/NwnDocOVruQFS1/veMgdzuPcnOM34M6CwxW8jH/lxEa5rBoDeUwu5HHTw==",
-                    "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.0.tgz",
-                    "version": "6.3.0"
+                    "integrity": "sha512-BR7VvDCVHO+q2xBEWskxS6DJE1qRnb7DxzUrogb71CWoSficBxYsiAGd+Kl0mmq/MprG9yArRkyrQxTO6XjMzA==",
+                    "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.1.tgz",
+                    "version": "6.3.1"
                 }
             },
             "dev": true,
             "integrity": "sha512-bg4Wxd1FWeFx3daHFTWk1pkSWK/AyQuiyAoeZAOkAOUBjnZPH6KT7eMxouV47tQ6hl6ax2zyAWBdWZXbrvXlaw==",
             "requires": {
                 "@babel/helper-module-imports": "^7.22.5",
                 "@babel/helper-plugin-utils": "^7.22.5",
@@ -1303,17 +1303,17 @@
                     "integrity": "sha512-SOSkfJDddaM7mak6cPEpswyTRnuRltl429hMraQEglW+OkovnCzsiszTmsrlY//qLFjCpQDFRvjdm2wA5pPm9w==",
                     "requires": {},
                     "resolved": "https://registry.npmjs.org/@babel/plugin-proposal-private-property-in-object/-/plugin-proposal-private-property-in-object-7.21.0-placeholder-for-preset-env.2.tgz",
                     "version": "7.21.0-placeholder-for-preset-env.2"
                 },
                 "semver": {
                     "dev": true,
-                    "integrity": "sha512-b39TBaTSfV6yBrapU89p5fKekE2m/NwnDocOVruQFS1/veMgdzuPcnOM34M6CwxW8jH/lxEa5rBoDeUwu5HHTw==",
-                    "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.0.tgz",
-                    "version": "6.3.0"
+                    "integrity": "sha512-BR7VvDCVHO+q2xBEWskxS6DJE1qRnb7DxzUrogb71CWoSficBxYsiAGd+Kl0mmq/MprG9yArRkyrQxTO6XjMzA==",
+                    "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.1.tgz",
+                    "version": "6.3.1"
                 }
             },
             "dev": true,
             "integrity": "sha512-fj06hw89dpiZzGZtxn+QybifF07nNiZjZ7sazs2aVDcysAZVGjW7+7iFYxg6GLNM47R/thYfLdrXc+2f11Vi9A==",
             "requires": {
                 "@babel/compat-data": "^7.22.5",
                 "@babel/helper-compilation-targets": "^7.22.5",
@@ -3739,17 +3739,17 @@
             "resolved": "https://registry.npmjs.org/babel-plugin-named-asset-import/-/babel-plugin-named-asset-import-0.3.8.tgz",
             "version": "0.3.8"
         },
         "babel-plugin-polyfill-corejs2": {
             "dependencies": {
                 "semver": {
                     "dev": true,
-                    "integrity": "sha512-b39TBaTSfV6yBrapU89p5fKekE2m/NwnDocOVruQFS1/veMgdzuPcnOM34M6CwxW8jH/lxEa5rBoDeUwu5HHTw==",
-                    "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.0.tgz",
-                    "version": "6.3.0"
+                    "integrity": "sha512-BR7VvDCVHO+q2xBEWskxS6DJE1qRnb7DxzUrogb71CWoSficBxYsiAGd+Kl0mmq/MprG9yArRkyrQxTO6XjMzA==",
+                    "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.1.tgz",
+                    "version": "6.3.1"
                 }
             },
             "dev": true,
             "integrity": "sha512-bM3gHc337Dta490gg+/AseNB9L4YLHxq1nGKZZSHbhXv4aTYU2MD2cjza1Ru4S6975YLTaL1K8uJf6ukJhhmtw==",
             "requires": {
                 "@babel/compat-data": "^7.17.7",
                 "@babel/helper-define-polyfill-provider": "^0.4.0",
@@ -5593,17 +5593,17 @@
             "resolved": "https://registry.npmjs.org/eslint-plugin-jest/-/eslint-plugin-jest-25.7.0.tgz",
             "version": "25.7.0"
         },
         "eslint-plugin-jsx-a11y": {
             "dependencies": {
                 "semver": {
                     "dev": true,
-                    "integrity": "sha512-b39TBaTSfV6yBrapU89p5fKekE2m/NwnDocOVruQFS1/veMgdzuPcnOM34M6CwxW8jH/lxEa5rBoDeUwu5HHTw==",
-                    "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.0.tgz",
-                    "version": "6.3.0"
+                    "integrity": "sha512-BR7VvDCVHO+q2xBEWskxS6DJE1qRnb7DxzUrogb71CWoSficBxYsiAGd+Kl0mmq/MprG9yArRkyrQxTO6XjMzA==",
+                    "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.1.tgz",
+                    "version": "6.3.1"
                 }
             },
             "dev": true,
             "integrity": "sha512-sXgFVNHiWffBq23uiS/JaP6eVR622DqwB4yTzKvGZGcPq6/yZ3WmOZfuBks/vHWo9GaFOqC2ZK4i6+C35knx7Q==",
             "requires": {
                 "@babel/runtime": "^7.18.9",
                 "aria-query": "^4.2.2",
@@ -5642,17 +5642,17 @@
                         "supports-preserve-symlinks-flag": "^1.0.0"
                     },
                     "resolved": "https://registry.npmjs.org/resolve/-/resolve-2.0.0-next.4.tgz",
                     "version": "2.0.0-next.4"
                 },
                 "semver": {
                     "dev": true,
-                    "integrity": "sha512-b39TBaTSfV6yBrapU89p5fKekE2m/NwnDocOVruQFS1/veMgdzuPcnOM34M6CwxW8jH/lxEa5rBoDeUwu5HHTw==",
-                    "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.0.tgz",
-                    "version": "6.3.0"
+                    "integrity": "sha512-BR7VvDCVHO+q2xBEWskxS6DJE1qRnb7DxzUrogb71CWoSficBxYsiAGd+Kl0mmq/MprG9yArRkyrQxTO6XjMzA==",
+                    "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.1.tgz",
+                    "version": "6.3.1"
                 }
             },
             "dev": true,
             "integrity": "sha512-t2fBMa+XzonrrNkyVirzKlvn5RXzzPwRHtMvLAtVZrt8oxgnTQaYbU6SXTOO1mwQgp1y5+toMSKInnzGr0Knqg==",
             "requires": {
                 "array-includes": "^3.1.6",
                 "array.prototype.flatmap": "^1.3.1",
@@ -7478,17 +7478,17 @@
             "resolved": "https://registry.npmjs.org/istanbul-lib-coverage/-/istanbul-lib-coverage-3.2.0.tgz",
             "version": "3.2.0"
         },
         "istanbul-lib-instrument": {
             "dependencies": {
                 "semver": {
                     "dev": true,
-                    "integrity": "sha512-b39TBaTSfV6yBrapU89p5fKekE2m/NwnDocOVruQFS1/veMgdzuPcnOM34M6CwxW8jH/lxEa5rBoDeUwu5HHTw==",
-                    "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.0.tgz",
-                    "version": "6.3.0"
+                    "integrity": "sha512-BR7VvDCVHO+q2xBEWskxS6DJE1qRnb7DxzUrogb71CWoSficBxYsiAGd+Kl0mmq/MprG9yArRkyrQxTO6XjMzA==",
+                    "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.1.tgz",
+                    "version": "6.3.1"
                 }
             },
             "dev": true,
             "integrity": "sha512-pzqtp31nLv/XFOzXGuvhCb8qhjmTVo5vjVk19XE4CRlSWz0KoeJ3bw9XsA7nOp9YBf4qHjwBxkDzKcME/J29Yg==",
             "requires": {
                 "@babel/core": "^7.12.3",
                 "@babel/parser": "^7.14.7",
@@ -9514,17 +9514,17 @@
             "resolved": "https://registry.npmjs.org/magic-string/-/magic-string-0.25.9.tgz",
             "version": "0.25.9"
         },
         "make-dir": {
             "dependencies": {
                 "semver": {
                     "dev": true,
-                    "integrity": "sha512-b39TBaTSfV6yBrapU89p5fKekE2m/NwnDocOVruQFS1/veMgdzuPcnOM34M6CwxW8jH/lxEa5rBoDeUwu5HHTw==",
-                    "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.0.tgz",
-                    "version": "6.3.0"
+                    "integrity": "sha512-BR7VvDCVHO+q2xBEWskxS6DJE1qRnb7DxzUrogb71CWoSficBxYsiAGd+Kl0mmq/MprG9yArRkyrQxTO6XjMzA==",
+                    "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.1.tgz",
+                    "version": "6.3.1"
                 }
             },
             "dev": true,
             "integrity": "sha512-g3FeP20LNwhALb/6Cz6Dd4F2ngze0jz7tbzrD2wAV+o9FeNHe4rL+yK2md0J/fiSf1sa1ADhXqi5+oVwOM/eGw==",
             "requires": {
                 "semver": "^6.0.0"
             },
@@ -11997,17 +11997,17 @@
                 "node-forge": "^1.2.0"
             },
             "resolved": "https://registry.npmjs.org/selfsigned/-/selfsigned-2.0.0.tgz",
             "version": "2.0.0"
         },
         "semver": {
             "dev": true,
-            "integrity": "sha512-sauaDf/PZdVgrLTNYHRtpXa1iRiKcaebiKQ1BJdpQlWH2lCvexQdX55snPFyK7QzpudqbCI0qXFfOasHdyNDGQ==",
-            "resolved": "https://registry.npmjs.org/semver/-/semver-5.7.1.tgz",
-            "version": "5.7.1"
+            "integrity": "sha512-cBznnQ9KjJqU67B52RMC65CMarK2600WFnbkcaiwWq3xy/5haFJlshgnpjovMVJ+Hff49d8GEn0b87C5pDQ10g==",
+            "resolved": "https://registry.npmjs.org/semver/-/semver-5.7.2.tgz",
+            "version": "5.7.2"
         },
         "send": {
             "dependencies": {
                 "debug": {
                     "dependencies": {
                         "ms": {
                             "dev": true,
@@ -13939,15 +13939,15 @@
             "devDependencies": {
                 "@babel/plugin-proposal-private-property-in-object": "^7.21.11",
                 "gh-pages": "^4.0.0",
                 "react-app-rewired": "^2.1.8",
                 "react-scripts": "^5.0.0"
             },
             "name": "sqllineagejs",
-            "version": "1.4.5"
+            "version": "1.4.6"
         },
         "node_modules/@aashutoshrathi/word-wrap": {
             "dev": true,
             "engines": {
                 "node": ">=0.10.0"
             },
             "integrity": "sha512-1Yjs2SvM8TflER/OD3cOjhWWOZb58A2t7wpE2S9XfBYTiIl+XFhQG2bjy4Pu1I+EAlCNUzRDYDdFwFYUKvXcIA==",
@@ -14019,17 +14019,17 @@
             "version": "7.22.5"
         },
         "node_modules/@babel/core/node_modules/semver": {
             "bin": {
                 "semver": "bin/semver.js"
             },
             "dev": true,
-            "integrity": "sha512-b39TBaTSfV6yBrapU89p5fKekE2m/NwnDocOVruQFS1/veMgdzuPcnOM34M6CwxW8jH/lxEa5rBoDeUwu5HHTw==",
-            "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.0.tgz",
-            "version": "6.3.0"
+            "integrity": "sha512-BR7VvDCVHO+q2xBEWskxS6DJE1qRnb7DxzUrogb71CWoSficBxYsiAGd+Kl0mmq/MprG9yArRkyrQxTO6XjMzA==",
+            "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.1.tgz",
+            "version": "6.3.1"
         },
         "node_modules/@babel/eslint-parser": {
             "dependencies": {
                 "@nicolo-ribaudo/eslint-scope-5-internals": "5.1.1-v1",
                 "eslint-visitor-keys": "^2.1.0",
                 "semver": "^6.3.0"
             },
@@ -14055,17 +14055,17 @@
             "version": "2.1.0"
         },
         "node_modules/@babel/eslint-parser/node_modules/semver": {
             "bin": {
                 "semver": "bin/semver.js"
             },
             "dev": true,
-            "integrity": "sha512-b39TBaTSfV6yBrapU89p5fKekE2m/NwnDocOVruQFS1/veMgdzuPcnOM34M6CwxW8jH/lxEa5rBoDeUwu5HHTw==",
-            "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.0.tgz",
-            "version": "6.3.0"
+            "integrity": "sha512-BR7VvDCVHO+q2xBEWskxS6DJE1qRnb7DxzUrogb71CWoSficBxYsiAGd+Kl0mmq/MprG9yArRkyrQxTO6XjMzA==",
+            "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.1.tgz",
+            "version": "6.3.1"
         },
         "node_modules/@babel/generator": {
             "dependencies": {
                 "@babel/types": "^7.22.5",
                 "@jridgewell/gen-mapping": "^0.3.2",
                 "@jridgewell/trace-mapping": "^0.3.17",
                 "jsesc": "^2.5.1"
@@ -14131,17 +14131,17 @@
             "version": "5.1.1"
         },
         "node_modules/@babel/helper-compilation-targets/node_modules/semver": {
             "bin": {
                 "semver": "bin/semver.js"
             },
             "dev": true,
-            "integrity": "sha512-b39TBaTSfV6yBrapU89p5fKekE2m/NwnDocOVruQFS1/veMgdzuPcnOM34M6CwxW8jH/lxEa5rBoDeUwu5HHTw==",
-            "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.0.tgz",
-            "version": "6.3.0"
+            "integrity": "sha512-BR7VvDCVHO+q2xBEWskxS6DJE1qRnb7DxzUrogb71CWoSficBxYsiAGd+Kl0mmq/MprG9yArRkyrQxTO6XjMzA==",
+            "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.1.tgz",
+            "version": "6.3.1"
         },
         "node_modules/@babel/helper-compilation-targets/node_modules/yallist": {
             "dev": true,
             "integrity": "sha512-a4UGQaWPH59mOXUYnAG2ewncQS4i4F43Tv3JoAM+s2VDAmS9NsK8GpDMLrCHPksFT7h3K6TOoUNn2pb7RoXx4g==",
             "resolved": "https://registry.npmjs.org/yallist/-/yallist-3.1.1.tgz",
             "version": "3.1.1"
         },
@@ -14169,17 +14169,17 @@
             "version": "7.22.5"
         },
         "node_modules/@babel/helper-create-class-features-plugin/node_modules/semver": {
             "bin": {
                 "semver": "bin/semver.js"
             },
             "dev": true,
-            "integrity": "sha512-b39TBaTSfV6yBrapU89p5fKekE2m/NwnDocOVruQFS1/veMgdzuPcnOM34M6CwxW8jH/lxEa5rBoDeUwu5HHTw==",
-            "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.0.tgz",
-            "version": "6.3.0"
+            "integrity": "sha512-BR7VvDCVHO+q2xBEWskxS6DJE1qRnb7DxzUrogb71CWoSficBxYsiAGd+Kl0mmq/MprG9yArRkyrQxTO6XjMzA==",
+            "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.1.tgz",
+            "version": "6.3.1"
         },
         "node_modules/@babel/helper-create-regexp-features-plugin": {
             "dependencies": {
                 "@babel/helper-annotate-as-pure": "^7.22.5",
                 "regexpu-core": "^5.3.1",
                 "semver": "^6.3.0"
             },
@@ -14195,17 +14195,17 @@
             "version": "7.22.5"
         },
         "node_modules/@babel/helper-create-regexp-features-plugin/node_modules/semver": {
             "bin": {
                 "semver": "bin/semver.js"
             },
             "dev": true,
-            "integrity": "sha512-b39TBaTSfV6yBrapU89p5fKekE2m/NwnDocOVruQFS1/veMgdzuPcnOM34M6CwxW8jH/lxEa5rBoDeUwu5HHTw==",
-            "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.0.tgz",
-            "version": "6.3.0"
+            "integrity": "sha512-BR7VvDCVHO+q2xBEWskxS6DJE1qRnb7DxzUrogb71CWoSficBxYsiAGd+Kl0mmq/MprG9yArRkyrQxTO6XjMzA==",
+            "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.1.tgz",
+            "version": "6.3.1"
         },
         "node_modules/@babel/helper-define-polyfill-provider": {
             "dependencies": {
                 "@babel/helper-compilation-targets": "^7.17.7",
                 "@babel/helper-plugin-utils": "^7.16.7",
                 "debug": "^4.1.1",
                 "lodash.debounce": "^4.0.8",
@@ -14221,17 +14221,17 @@
             "version": "0.4.0"
         },
         "node_modules/@babel/helper-define-polyfill-provider/node_modules/semver": {
             "bin": {
                 "semver": "bin/semver.js"
             },
             "dev": true,
-            "integrity": "sha512-b39TBaTSfV6yBrapU89p5fKekE2m/NwnDocOVruQFS1/veMgdzuPcnOM34M6CwxW8jH/lxEa5rBoDeUwu5HHTw==",
-            "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.0.tgz",
-            "version": "6.3.0"
+            "integrity": "sha512-BR7VvDCVHO+q2xBEWskxS6DJE1qRnb7DxzUrogb71CWoSficBxYsiAGd+Kl0mmq/MprG9yArRkyrQxTO6XjMzA==",
+            "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.1.tgz",
+            "version": "6.3.1"
         },
         "node_modules/@babel/helper-environment-visitor": {
             "dev": true,
             "engines": {
                 "node": ">=6.9.0"
             },
             "integrity": "sha512-XGmhECfVA/5sAt+H+xpSg0mfrHq6FzNr9Oxh7PSEBBRUb/mL7Kz3NICXb194rCqAEdxkhPT1a88teizAFyvk8Q==",
@@ -15700,17 +15700,17 @@
             "version": "7.22.5"
         },
         "node_modules/@babel/plugin-transform-runtime/node_modules/semver": {
             "bin": {
                 "semver": "bin/semver.js"
             },
             "dev": true,
-            "integrity": "sha512-b39TBaTSfV6yBrapU89p5fKekE2m/NwnDocOVruQFS1/veMgdzuPcnOM34M6CwxW8jH/lxEa5rBoDeUwu5HHTw==",
-            "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.0.tgz",
-            "version": "6.3.0"
+            "integrity": "sha512-BR7VvDCVHO+q2xBEWskxS6DJE1qRnb7DxzUrogb71CWoSficBxYsiAGd+Kl0mmq/MprG9yArRkyrQxTO6XjMzA==",
+            "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.1.tgz",
+            "version": "6.3.1"
         },
         "node_modules/@babel/plugin-transform-shorthand-properties": {
             "dependencies": {
                 "@babel/helper-plugin-utils": "^7.22.5"
             },
             "dev": true,
             "engines": {
@@ -15972,17 +15972,17 @@
             "version": "7.21.0-placeholder-for-preset-env.2"
         },
         "node_modules/@babel/preset-env/node_modules/semver": {
             "bin": {
                 "semver": "bin/semver.js"
             },
             "dev": true,
-            "integrity": "sha512-b39TBaTSfV6yBrapU89p5fKekE2m/NwnDocOVruQFS1/veMgdzuPcnOM34M6CwxW8jH/lxEa5rBoDeUwu5HHTw==",
-            "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.0.tgz",
-            "version": "6.3.0"
+            "integrity": "sha512-BR7VvDCVHO+q2xBEWskxS6DJE1qRnb7DxzUrogb71CWoSficBxYsiAGd+Kl0mmq/MprG9yArRkyrQxTO6XjMzA==",
+            "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.1.tgz",
+            "version": "6.3.1"
         },
         "node_modules/@babel/preset-modules": {
             "dependencies": {
                 "@babel/helper-plugin-utils": "^7.0.0",
                 "@babel/plugin-proposal-unicode-property-regex": "^7.4.4",
                 "@babel/plugin-transform-dotall-regex": "^7.4.4",
                 "@babel/types": "^7.4.4",
@@ -19164,17 +19164,17 @@
             "version": "0.4.3"
         },
         "node_modules/babel-plugin-polyfill-corejs2/node_modules/semver": {
             "bin": {
                 "semver": "bin/semver.js"
             },
             "dev": true,
-            "integrity": "sha512-b39TBaTSfV6yBrapU89p5fKekE2m/NwnDocOVruQFS1/veMgdzuPcnOM34M6CwxW8jH/lxEa5rBoDeUwu5HHTw==",
-            "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.0.tgz",
-            "version": "6.3.0"
+            "integrity": "sha512-BR7VvDCVHO+q2xBEWskxS6DJE1qRnb7DxzUrogb71CWoSficBxYsiAGd+Kl0mmq/MprG9yArRkyrQxTO6XjMzA==",
+            "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.1.tgz",
+            "version": "6.3.1"
         },
         "node_modules/babel-plugin-polyfill-corejs3": {
             "dependencies": {
                 "@babel/helper-define-polyfill-provider": "^0.4.0",
                 "core-js-compat": "^3.30.1"
             },
             "dev": true,
@@ -21453,17 +21453,17 @@
             "version": "6.6.1"
         },
         "node_modules/eslint-plugin-jsx-a11y/node_modules/semver": {
             "bin": {
                 "semver": "bin/semver.js"
             },
             "dev": true,
-            "integrity": "sha512-b39TBaTSfV6yBrapU89p5fKekE2m/NwnDocOVruQFS1/veMgdzuPcnOM34M6CwxW8jH/lxEa5rBoDeUwu5HHTw==",
-            "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.0.tgz",
-            "version": "6.3.0"
+            "integrity": "sha512-BR7VvDCVHO+q2xBEWskxS6DJE1qRnb7DxzUrogb71CWoSficBxYsiAGd+Kl0mmq/MprG9yArRkyrQxTO6XjMzA==",
+            "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.1.tgz",
+            "version": "6.3.1"
         },
         "node_modules/eslint-plugin-react": {
             "dependencies": {
                 "array-includes": "^3.1.6",
                 "array.prototype.flatmap": "^1.3.1",
                 "array.prototype.tosorted": "^1.1.1",
                 "doctrine": "^2.1.0",
@@ -21532,17 +21532,17 @@
             "version": "2.0.0-next.4"
         },
         "node_modules/eslint-plugin-react/node_modules/semver": {
             "bin": {
                 "semver": "bin/semver.js"
             },
             "dev": true,
-            "integrity": "sha512-b39TBaTSfV6yBrapU89p5fKekE2m/NwnDocOVruQFS1/veMgdzuPcnOM34M6CwxW8jH/lxEa5rBoDeUwu5HHTw==",
-            "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.0.tgz",
-            "version": "6.3.0"
+            "integrity": "sha512-BR7VvDCVHO+q2xBEWskxS6DJE1qRnb7DxzUrogb71CWoSficBxYsiAGd+Kl0mmq/MprG9yArRkyrQxTO6XjMzA==",
+            "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.1.tgz",
+            "version": "6.3.1"
         },
         "node_modules/eslint-plugin-testing-library": {
             "dependencies": {
                 "@typescript-eslint/utils": "^5.13.0"
             },
             "dev": true,
             "engines": {
@@ -24145,17 +24145,17 @@
             "version": "5.2.1"
         },
         "node_modules/istanbul-lib-instrument/node_modules/semver": {
             "bin": {
                 "semver": "bin/semver.js"
             },
             "dev": true,
-            "integrity": "sha512-b39TBaTSfV6yBrapU89p5fKekE2m/NwnDocOVruQFS1/veMgdzuPcnOM34M6CwxW8jH/lxEa5rBoDeUwu5HHTw==",
-            "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.0.tgz",
-            "version": "6.3.0"
+            "integrity": "sha512-BR7VvDCVHO+q2xBEWskxS6DJE1qRnb7DxzUrogb71CWoSficBxYsiAGd+Kl0mmq/MprG9yArRkyrQxTO6XjMzA==",
+            "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.1.tgz",
+            "version": "6.3.1"
         },
         "node_modules/istanbul-lib-report": {
             "dependencies": {
                 "istanbul-lib-coverage": "^3.0.0",
                 "make-dir": "^3.0.0",
                 "supports-color": "^7.1.0"
             },
@@ -26817,17 +26817,17 @@
             "version": "3.1.0"
         },
         "node_modules/make-dir/node_modules/semver": {
             "bin": {
                 "semver": "bin/semver.js"
             },
             "dev": true,
-            "integrity": "sha512-b39TBaTSfV6yBrapU89p5fKekE2m/NwnDocOVruQFS1/veMgdzuPcnOM34M6CwxW8jH/lxEa5rBoDeUwu5HHTw==",
-            "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.0.tgz",
-            "version": "6.3.0"
+            "integrity": "sha512-BR7VvDCVHO+q2xBEWskxS6DJE1qRnb7DxzUrogb71CWoSficBxYsiAGd+Kl0mmq/MprG9yArRkyrQxTO6XjMzA==",
+            "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.1.tgz",
+            "version": "6.3.1"
         },
         "node_modules/makeerror": {
             "dependencies": {
                 "tmpl": "1.0.5"
             },
             "dev": true,
             "integrity": "sha512-JmqCvUhmt43madlpFzG4BQzG2Z3m6tvQDNKdClZnO3VbIudJYmxsT0FNJMeiB2+JTSlTQTSbU8QdesVmwJcmLg==",
@@ -30352,17 +30352,17 @@
             "version": "2.0.0"
         },
         "node_modules/semver": {
             "bin": {
                 "semver": "bin/semver"
             },
             "dev": true,
-            "integrity": "sha512-sauaDf/PZdVgrLTNYHRtpXa1iRiKcaebiKQ1BJdpQlWH2lCvexQdX55snPFyK7QzpudqbCI0qXFfOasHdyNDGQ==",
-            "resolved": "https://registry.npmjs.org/semver/-/semver-5.7.1.tgz",
-            "version": "5.7.1"
+            "integrity": "sha512-cBznnQ9KjJqU67B52RMC65CMarK2600WFnbkcaiwWq3xy/5haFJlshgnpjovMVJ+Hff49d8GEn0b87C5pDQ10g==",
+            "resolved": "https://registry.npmjs.org/semver/-/semver-5.7.2.tgz",
+            "version": "5.7.2"
         },
         "node_modules/send": {
             "dependencies": {
                 "debug": "2.6.9",
                 "depd": "2.0.0",
                 "destroy": "1.2.0",
                 "encodeurl": "~1.0.2",
@@ -32821,9 +32821,9 @@
             },
             "integrity": "sha512-rVksvsnNCdJ/ohGc6xgPwyN8eheCxsiLM8mxuE/t/mOVqJewPuO1miLpTHQiRgTKCLexL4MeAFVagts7HmNZ2Q==",
             "resolved": "https://registry.npmjs.org/yocto-queue/-/yocto-queue-0.1.0.tgz",
             "version": "0.1.0"
         }
     },
     "requires": true,
-    "version": "1.4.5"
+    "version": "1.4.6"
 }
```

### Comparing `sqllineage-1.4.5/sqllineagejs/package.json` & `sqllineage-1.4.6/sqllineagejs/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {"'version'": "'1.4.6'"}*

```diff
@@ -43,9 +43,9 @@
     "private": true,
     "scripts": {
         "build": "react-app-rewired build",
         "deploy": "gh-pages -d build",
         "eject": "react-scripts eject",
         "start": "react-app-rewired start"
     },
-    "version": "1.4.5"
+    "version": "1.4.6"
 }
```

### Comparing `sqllineage-1.4.5/sqllineagejs/public/favicon.ico` & `sqllineage-1.4.6/sqllineagejs/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineagejs/public/index.html` & `sqllineage-1.4.6/sqllineagejs/public/index.html`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineagejs/public/logo192.png` & `sqllineage-1.4.6/sqllineagejs/public/logo192.png`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineagejs/public/logo512.png` & `sqllineage-1.4.6/sqllineagejs/public/logo512.png`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineagejs/src/App.js` & `sqllineage-1.4.6/sqllineagejs/src/App.js`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineagejs/src/api/client.js` & `sqllineage-1.4.6/sqllineagejs/src/api/client.js`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineagejs/src/features/directory/Directory.js` & `sqllineage-1.4.6/sqllineagejs/src/features/directory/Directory.js`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineagejs/src/features/directory/DirectoryTreeItem.js` & `sqllineage-1.4.6/sqllineagejs/src/features/directory/DirectoryTreeItem.js`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineagejs/src/features/directory/directorySlice.js` & `sqllineage-1.4.6/sqllineagejs/src/features/directory/directorySlice.js`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineagejs/src/features/editor/DAG.js` & `sqllineage-1.4.6/sqllineagejs/src/features/editor/DAG.js`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineagejs/src/features/editor/DAGDesc.js` & `sqllineage-1.4.6/sqllineagejs/src/features/editor/DAGDesc.js`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineagejs/src/features/editor/Editor.js` & `sqllineage-1.4.6/sqllineagejs/src/features/editor/Editor.js`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineagejs/src/features/editor/editorSlice.js` & `sqllineage-1.4.6/sqllineagejs/src/features/editor/editorSlice.js`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineagejs/src/features/widget/LoadError.js` & `sqllineage-1.4.6/sqllineagejs/src/features/widget/LoadError.js`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineagejs/src/features/widget/Loading.js` & `sqllineage-1.4.6/sqllineagejs/src/features/widget/Loading.js`

 * *Files identical despite different names*

### Comparing `sqllineage-1.4.5/sqllineagejs/src/index.css` & `sqllineage-1.4.6/sqllineagejs/src/index.css`

 * *Files identical despite different names*

