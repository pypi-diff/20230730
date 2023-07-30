# Comparing `tmp/dl_matrix-0.4.tar.gz` & `tmp/dl_matrix-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dl_matrix-0.4.tar", last modified: Sat Jul 29 23:12:40 2023, max compression
+gzip compressed data, was "dl_matrix-0.5.tar", last modified: Sun Jul 30 01:11:23 2023, max compression
```

## Comparing `dl_matrix-0.4.tar` & `dl_matrix-0.5.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-29 23:12:40.735035 dl_matrix-0.4/
--rw-r--r--   0 mo         (501) staff       (20)     1073 2023-07-29 21:15:54.000000 dl_matrix-0.4/LICENSE
--rw-r--r--   0 mo         (501) staff       (20)       25 2023-07-29 23:03:07.000000 dl_matrix-0.4/MANIFEST.in
--rw-r--r--   0 mo         (501) staff       (20)     3125 2023-07-29 23:12:40.734888 dl_matrix-0.4/PKG-INFO
--rw-r--r--   0 mo         (501) staff       (20)     2670 2023-07-29 21:36:22.000000 dl_matrix-0.4/README.md
-drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-29 23:12:40.716038 dl_matrix-0.4/dl_matrix/
--rw-rw-r--   0 mo         (501) staff       (20)      109 2023-07-29 21:38:05.000000 dl_matrix-0.4/dl_matrix/__init__.py
--rw-rw-r--   0 mo         (501) staff       (20)    11557 2023-07-29 21:01:15.000000 dl_matrix-0.4/dl_matrix/builder.py
--rw-rw-r--   0 mo         (501) staff       (20)     5889 2023-07-27 22:03:15.000000 dl_matrix-0.4/dl_matrix/context.py
-drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-29 23:12:40.720283 dl_matrix-0.4/dl_matrix/coordinate/
--rw-rw-r--   0 mo         (501) staff       (20)       21 2023-07-28 00:45:01.000000 dl_matrix-0.4/dl_matrix/coordinate/__init__.py
--rw-rw-r--   0 mo         (501) staff       (20)    19532 2023-07-28 02:59:26.000000 dl_matrix-0.4/dl_matrix/coordinate/base.py
--rw-r--r--   0 mo         (501) staff       (20)     9568 2023-07-28 14:07:23.000000 dl_matrix-0.4/dl_matrix/coordinate/complex.py
-drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-29 23:12:40.722874 dl_matrix-0.4/dl_matrix/coordinate/components/
--rw-rw-r--   0 mo         (501) staff       (20)      153 2023-07-27 02:26:31.000000 dl_matrix-0.4/dl_matrix/coordinate/components/__init__.py
--rw-rw-r--   0 mo         (501) staff       (20)     1773 2023-07-26 00:08:02.000000 dl_matrix-0.4/dl_matrix/coordinate/components/base.py
--rw-rw-r--   0 mo         (501) staff       (20)     1874 2023-07-27 18:06:28.000000 dl_matrix-0.4/dl_matrix/coordinate/components/depth.py
--rw-rw-r--   0 mo         (501) staff       (20)     1460 2023-07-27 18:06:28.000000 dl_matrix-0.4/dl_matrix/coordinate/components/sibling.py
--rw-rw-r--   0 mo         (501) staff       (20)     1636 2023-07-27 18:06:28.000000 dl_matrix-0.4/dl_matrix/coordinate/components/sibling_count.py
--rw-rw-r--   0 mo         (501) staff       (20)     2286 2023-07-27 18:06:28.000000 dl_matrix-0.4/dl_matrix/coordinate/components/time.py
--rw-r--r--   0 mo         (501) staff       (20)    11877 2023-07-28 14:07:23.000000 dl_matrix-0.4/dl_matrix/coordinate/matcher.py
--rw-r--r--   0 mo         (501) staff       (20)     6824 2023-07-28 02:59:20.000000 dl_matrix-0.4/dl_matrix/coordinate/model.py
--rw-r--r--   0 mo         (501) staff       (20)     5921 2023-07-28 02:59:31.000000 dl_matrix-0.4/dl_matrix/coordinate/tree.py
--rw-r--r--   0 mo         (501) staff       (20)    11906 2023-07-28 02:12:21.000000 dl_matrix-0.4/dl_matrix/coordinate/utils.py
--rw-rw-r--   0 mo         (501) staff       (20)     3817 2023-07-28 02:12:21.000000 dl_matrix-0.4/dl_matrix/parsers.py
--rw-rw-r--   0 mo         (501) staff       (20)    26111 2023-07-29 20:48:16.000000 dl_matrix-0.4/dl_matrix/relationship.py
-drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-29 23:12:40.725481 dl_matrix-0.4/dl_matrix/representation/
--rw-rw-r--   0 mo         (501) staff       (20)       96 2023-07-28 13:18:53.000000 dl_matrix-0.4/dl_matrix/representation/__init__.py
--rw-r--r--   0 mo         (501) staff       (20)     4648 2023-07-28 02:59:41.000000 dl_matrix-0.4/dl_matrix/representation/animate.py
--rw-rw-r--   0 mo         (501) staff       (20)    10399 2023-07-29 20:47:32.000000 dl_matrix-0.4/dl_matrix/representation/base.py
--rw-r--r--   0 mo         (501) staff       (20)    11017 2023-07-29 20:44:23.000000 dl_matrix-0.4/dl_matrix/representation/combine.py
--rw-rw-r--   0 mo         (501) staff       (20)    14786 2023-07-29 20:43:20.000000 dl_matrix-0.4/dl_matrix/representation/compute.py
--rw-rw-r--   0 mo         (501) staff       (20)     6965 2023-07-28 02:33:05.000000 dl_matrix-0.4/dl_matrix/representation/estimator.py
--rw-rw-r--   0 mo         (501) staff       (20)     9633 2023-07-29 01:48:25.000000 dl_matrix-0.4/dl_matrix/representation/filters.py
--rw-r--r--   0 mo         (501) staff       (20)     5379 2023-07-28 14:07:23.000000 dl_matrix-0.4/dl_matrix/representation/handler.py
--rw-rw-r--   0 mo         (501) staff       (20)    11569 2023-07-29 16:28:17.000000 dl_matrix-0.4/dl_matrix/schema.py
--rw-rw-r--   0 mo         (501) staff       (20)    10299 2023-07-29 00:46:29.000000 dl_matrix-0.4/dl_matrix/similarity.py
-drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-29 23:12:40.726195 dl_matrix-0.4/dl_matrix/structure/
--rw-rw-r--   0 mo         (501) staff       (20)       43 2023-07-26 16:06:54.000000 dl_matrix-0.4/dl_matrix/structure/__init__.py
--rw-rw-r--   0 mo         (501) staff       (20)    12267 2023-07-29 12:38:03.000000 dl_matrix-0.4/dl_matrix/structure/base.py
-drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-29 23:12:40.726716 dl_matrix-0.4/dl_matrix/structure/mapping/
--rw-rw-r--   0 mo         (501) staff       (20)       76 2023-07-24 15:55:42.000000 dl_matrix-0.4/dl_matrix/structure/mapping/__init__.py
--rw-rw-r--   0 mo         (501) staff       (20)     5688 2023-07-28 21:42:12.000000 dl_matrix-0.4/dl_matrix/structure/mapping/base.py
-drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-29 23:12:40.727310 dl_matrix-0.4/dl_matrix/structure/mapping/message/
--rw-rw-r--   0 mo         (501) staff       (20)       20 2023-07-21 22:10:26.000000 dl_matrix-0.4/dl_matrix/structure/mapping/message/__init__.py
-drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-29 23:12:40.729458 dl_matrix-0.4/dl_matrix/structure/mapping/message/author/
--rw-rw-r--   0 mo         (501) staff       (20)       57 2023-07-29 01:48:25.000000 dl_matrix-0.4/dl_matrix/structure/mapping/message/author/__init__.py
--rw-rw-r--   0 mo         (501) staff       (20)     1303 2023-07-24 22:43:21.000000 dl_matrix-0.4/dl_matrix/structure/mapping/message/author/author.py
--rw-rw-r--   0 mo         (501) staff       (20)     1767 2023-07-24 22:49:37.000000 dl_matrix-0.4/dl_matrix/structure/mapping/message/author/role.py
--rw-rw-r--   0 mo         (501) staff       (20)     4387 2023-07-24 22:49:37.000000 dl_matrix-0.4/dl_matrix/structure/mapping/message/author/synthesis.py
--rw-rw-r--   0 mo         (501) staff       (20)      519 2023-07-29 00:01:46.000000 dl_matrix-0.4/dl_matrix/structure/mapping/message/author/types.py
--rw-rw-r--   0 mo         (501) staff       (20)     4098 2023-07-26 22:20:17.000000 dl_matrix-0.4/dl_matrix/structure/mapping/message/base.py
-drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-29 23:12:40.730175 dl_matrix-0.4/dl_matrix/structure/mapping/message/connection/
--rw-rw-r--   0 mo         (501) staff       (20)       26 2023-07-26 18:33:05.000000 dl_matrix-0.4/dl_matrix/structure/mapping/message/connection/__init__.py
--rw-r--r--   0 mo         (501) staff       (20)     3246 2023-07-26 19:03:33.000000 dl_matrix-0.4/dl_matrix/structure/mapping/message/connection/connection.py
--rw-r--r--   0 mo         (501) staff       (20)      390 2023-07-26 19:03:33.000000 dl_matrix-0.4/dl_matrix/structure/mapping/message/connection/types.py
-drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-29 23:12:40.731032 dl_matrix-0.4/dl_matrix/structure/mapping/message/content/
--rw-rw-r--   0 mo         (501) staff       (20)       26 2023-07-23 02:50:38.000000 dl_matrix-0.4/dl_matrix/structure/mapping/message/content/__init__.py
--rw-rw-r--   0 mo         (501) staff       (20)     1979 2023-07-28 21:42:12.000000 dl_matrix-0.4/dl_matrix/structure/mapping/message/content/base.py
-drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-29 23:12:40.731529 dl_matrix-0.4/dl_matrix/structure/mapping/message/content/embedding/
--rw-r--r--   0 mo         (501) staff       (20)       28 2023-07-27 14:28:59.000000 dl_matrix-0.4/dl_matrix/structure/mapping/message/content/embedding/__init__.py
--rw-r--r--   0 mo         (501) staff       (20)     1779 2023-07-27 14:28:59.000000 dl_matrix-0.4/dl_matrix/structure/mapping/message/content/embedding/base.py
-drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-29 23:12:40.732002 dl_matrix-0.4/dl_matrix/structure/mapping/message/content/moderation/
--rw-r--r--   0 mo         (501) staff       (20)       41 2023-07-26 18:15:19.000000 dl_matrix-0.4/dl_matrix/structure/mapping/message/content/moderation/__init__.py
--rw-r--r--   0 mo         (501) staff       (20)     1641 2023-07-26 18:41:17.000000 dl_matrix-0.4/dl_matrix/structure/mapping/message/content/moderation/moderation.py
-drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-29 23:12:40.732507 dl_matrix-0.4/dl_matrix/structure/mapping/message/content/production/
--rw-r--r--   0 mo         (501) staff       (20)       40 2023-07-28 15:06:09.000000 dl_matrix-0.4/dl_matrix/structure/mapping/message/content/production/__init__.py
--rw-r--r--   0 mo         (501) staff       (20)     9478 2023-07-26 18:03:16.000000 dl_matrix-0.4/dl_matrix/structure/mapping/message/content/production/production.py
-drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-29 23:12:40.733322 dl_matrix-0.4/dl_matrix/structure/mapping/message/content/query/
--rw-rw-r--   0 mo         (501) staff       (20)       59 2023-07-28 19:09:39.000000 dl_matrix-0.4/dl_matrix/structure/mapping/message/content/query/__init__.py
--rw-r--r--   0 mo         (501) staff       (20)    10697 2023-07-28 21:42:12.000000 dl_matrix-0.4/dl_matrix/structure/mapping/message/content/query/query_generator.py
--rw-r--r--   0 mo         (501) staff       (20)     6479 2023-07-28 21:42:12.000000 dl_matrix-0.4/dl_matrix/structure/mapping/message/content/query/query_parser.py
--rw-rw-r--   0 mo         (501) staff       (20)     1089 2023-07-21 22:09:42.000000 dl_matrix-0.4/dl_matrix/structure/mapping/message/content/types.py
-drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-29 23:12:40.733823 dl_matrix-0.4/dl_matrix/structure/mapping/message/metadata/
--rw-rw-r--   0 mo         (501) staff       (20)       31 2023-07-21 22:10:58.000000 dl_matrix-0.4/dl_matrix/structure/mapping/message/metadata/__init__.py
--rw-rw-r--   0 mo         (501) staff       (20)     5866 2023-07-25 01:35:05.000000 dl_matrix-0.4/dl_matrix/structure/mapping/message/metadata/metadata.py
-drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-29 23:12:40.734538 dl_matrix-0.4/dl_matrix/visualization/
--rw-rw-r--   0 mo         (501) staff       (20)       46 2023-07-27 18:06:28.000000 dl_matrix-0.4/dl_matrix/visualization/__init__.py
--rw-rw-r--   0 mo         (501) staff       (20)     4176 2023-07-27 18:06:29.000000 dl_matrix-0.4/dl_matrix/visualization/app.py
--rw-rw-r--   0 mo         (501) staff       (20)     8755 2023-07-29 21:01:15.000000 dl_matrix-0.4/dl_matrix/visualization/psychedelic.py
-drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-29 23:12:40.716968 dl_matrix-0.4/dl_matrix.egg-info/
--rw-r--r--   0 mo         (501) staff       (20)     3125 2023-07-29 23:12:40.000000 dl_matrix-0.4/dl_matrix.egg-info/PKG-INFO
--rw-r--r--   0 mo         (501) staff       (20)     2783 2023-07-29 23:12:40.000000 dl_matrix-0.4/dl_matrix.egg-info/SOURCES.txt
--rw-r--r--   0 mo         (501) staff       (20)        1 2023-07-29 23:12:40.000000 dl_matrix-0.4/dl_matrix.egg-info/dependency_links.txt
--rw-r--r--   0 mo         (501) staff       (20)     3063 2023-07-29 23:12:40.000000 dl_matrix-0.4/dl_matrix.egg-info/requires.txt
--rw-r--r--   0 mo         (501) staff       (20)       10 2023-07-29 23:12:40.000000 dl_matrix-0.4/dl_matrix.egg-info/top_level.txt
--rw-r--r--   0 mo         (501) staff       (20)     3064 2023-07-29 21:12:00.000000 dl_matrix-0.4/requirements.txt
--rw-r--r--   0 mo         (501) staff       (20)       38 2023-07-29 23:12:40.735079 dl_matrix-0.4/setup.cfg
--rw-r--r--   0 mo         (501) staff       (20)      735 2023-07-29 23:12:20.000000 dl_matrix-0.4/setup.py
+drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-30 01:11:23.344265 dl_matrix-0.5/
+-rw-r--r--   0 mo         (501) staff       (20)     1073 2023-07-29 21:15:54.000000 dl_matrix-0.5/LICENSE
+-rw-r--r--   0 mo         (501) staff       (20)       25 2023-07-29 23:03:07.000000 dl_matrix-0.5/MANIFEST.in
+-rw-r--r--   0 mo         (501) staff       (20)     3125 2023-07-30 01:11:23.344117 dl_matrix-0.5/PKG-INFO
+-rw-r--r--   0 mo         (501) staff       (20)     2670 2023-07-29 21:36:22.000000 dl_matrix-0.5/README.md
+drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-30 01:11:23.323192 dl_matrix-0.5/dl_matrix/
+-rw-rw-r--   0 mo         (501) staff       (20)      109 2023-07-29 21:38:05.000000 dl_matrix-0.5/dl_matrix/__init__.py
+-rw-rw-r--   0 mo         (501) staff       (20)    11557 2023-07-29 21:01:15.000000 dl_matrix-0.5/dl_matrix/builder.py
+-rw-rw-r--   0 mo         (501) staff       (20)     5889 2023-07-27 22:03:15.000000 dl_matrix-0.5/dl_matrix/context.py
+drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-30 01:11:23.326128 dl_matrix-0.5/dl_matrix/coordinate/
+-rw-rw-r--   0 mo         (501) staff       (20)       21 2023-07-28 00:45:01.000000 dl_matrix-0.5/dl_matrix/coordinate/__init__.py
+-rw-rw-r--   0 mo         (501) staff       (20)    19532 2023-07-28 02:59:26.000000 dl_matrix-0.5/dl_matrix/coordinate/base.py
+-rw-r--r--   0 mo         (501) staff       (20)     9568 2023-07-28 14:07:23.000000 dl_matrix-0.5/dl_matrix/coordinate/complex.py
+drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-30 01:11:23.328297 dl_matrix-0.5/dl_matrix/coordinate/components/
+-rw-rw-r--   0 mo         (501) staff       (20)      153 2023-07-27 02:26:31.000000 dl_matrix-0.5/dl_matrix/coordinate/components/__init__.py
+-rw-rw-r--   0 mo         (501) staff       (20)     1773 2023-07-26 00:08:02.000000 dl_matrix-0.5/dl_matrix/coordinate/components/base.py
+-rw-rw-r--   0 mo         (501) staff       (20)     1874 2023-07-27 18:06:28.000000 dl_matrix-0.5/dl_matrix/coordinate/components/depth.py
+-rw-rw-r--   0 mo         (501) staff       (20)     1460 2023-07-27 18:06:28.000000 dl_matrix-0.5/dl_matrix/coordinate/components/sibling.py
+-rw-rw-r--   0 mo         (501) staff       (20)     1636 2023-07-27 18:06:28.000000 dl_matrix-0.5/dl_matrix/coordinate/components/sibling_count.py
+-rw-rw-r--   0 mo         (501) staff       (20)     2286 2023-07-27 18:06:28.000000 dl_matrix-0.5/dl_matrix/coordinate/components/time.py
+-rw-r--r--   0 mo         (501) staff       (20)    11877 2023-07-28 14:07:23.000000 dl_matrix-0.5/dl_matrix/coordinate/matcher.py
+-rw-r--r--   0 mo         (501) staff       (20)     6824 2023-07-28 02:59:20.000000 dl_matrix-0.5/dl_matrix/coordinate/model.py
+-rw-r--r--   0 mo         (501) staff       (20)     5921 2023-07-28 02:59:31.000000 dl_matrix-0.5/dl_matrix/coordinate/tree.py
+-rw-r--r--   0 mo         (501) staff       (20)    11906 2023-07-28 02:12:21.000000 dl_matrix-0.5/dl_matrix/coordinate/utils.py
+-rw-rw-r--   0 mo         (501) staff       (20)     3817 2023-07-28 02:12:21.000000 dl_matrix-0.5/dl_matrix/parsers.py
+-rw-rw-r--   0 mo         (501) staff       (20)    26111 2023-07-29 20:48:16.000000 dl_matrix-0.5/dl_matrix/relationship.py
+drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-30 01:11:23.330448 dl_matrix-0.5/dl_matrix/representation/
+-rw-rw-r--   0 mo         (501) staff       (20)       96 2023-07-28 13:18:53.000000 dl_matrix-0.5/dl_matrix/representation/__init__.py
+-rw-r--r--   0 mo         (501) staff       (20)     4648 2023-07-28 02:59:41.000000 dl_matrix-0.5/dl_matrix/representation/animate.py
+-rw-rw-r--   0 mo         (501) staff       (20)    10399 2023-07-29 20:47:32.000000 dl_matrix-0.5/dl_matrix/representation/base.py
+-rw-r--r--   0 mo         (501) staff       (20)    11017 2023-07-29 20:44:23.000000 dl_matrix-0.5/dl_matrix/representation/combine.py
+-rw-rw-r--   0 mo         (501) staff       (20)    14786 2023-07-29 20:43:20.000000 dl_matrix-0.5/dl_matrix/representation/compute.py
+-rw-rw-r--   0 mo         (501) staff       (20)     6965 2023-07-28 02:33:05.000000 dl_matrix-0.5/dl_matrix/representation/estimator.py
+-rw-rw-r--   0 mo         (501) staff       (20)     9633 2023-07-29 01:48:25.000000 dl_matrix-0.5/dl_matrix/representation/filters.py
+-rw-r--r--   0 mo         (501) staff       (20)     5379 2023-07-28 14:07:23.000000 dl_matrix-0.5/dl_matrix/representation/handler.py
+-rw-rw-r--   0 mo         (501) staff       (20)    11569 2023-07-29 16:28:17.000000 dl_matrix-0.5/dl_matrix/schema.py
+-rw-rw-r--   0 mo         (501) staff       (20)    10299 2023-07-29 00:46:29.000000 dl_matrix-0.5/dl_matrix/similarity.py
+drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-30 01:11:23.331076 dl_matrix-0.5/dl_matrix/structure/
+-rw-rw-r--   0 mo         (501) staff       (20)       43 2023-07-26 16:06:54.000000 dl_matrix-0.5/dl_matrix/structure/__init__.py
+-rw-rw-r--   0 mo         (501) staff       (20)    12267 2023-07-29 12:38:03.000000 dl_matrix-0.5/dl_matrix/structure/base.py
+drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-30 01:11:23.331606 dl_matrix-0.5/dl_matrix/structure/mapping/
+-rw-rw-r--   0 mo         (501) staff       (20)       76 2023-07-24 15:55:42.000000 dl_matrix-0.5/dl_matrix/structure/mapping/__init__.py
+-rw-rw-r--   0 mo         (501) staff       (20)     5688 2023-07-28 21:42:12.000000 dl_matrix-0.5/dl_matrix/structure/mapping/base.py
+drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-30 01:11:23.332216 dl_matrix-0.5/dl_matrix/structure/mapping/message/
+-rw-rw-r--   0 mo         (501) staff       (20)       20 2023-07-21 22:10:26.000000 dl_matrix-0.5/dl_matrix/structure/mapping/message/__init__.py
+drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-30 01:11:23.334411 dl_matrix-0.5/dl_matrix/structure/mapping/message/author/
+-rw-rw-r--   0 mo         (501) staff       (20)       57 2023-07-29 01:48:25.000000 dl_matrix-0.5/dl_matrix/structure/mapping/message/author/__init__.py
+-rw-rw-r--   0 mo         (501) staff       (20)     1303 2023-07-24 22:43:21.000000 dl_matrix-0.5/dl_matrix/structure/mapping/message/author/author.py
+-rw-rw-r--   0 mo         (501) staff       (20)     1767 2023-07-24 22:49:37.000000 dl_matrix-0.5/dl_matrix/structure/mapping/message/author/role.py
+-rw-rw-r--   0 mo         (501) staff       (20)     4387 2023-07-24 22:49:37.000000 dl_matrix-0.5/dl_matrix/structure/mapping/message/author/synthesis.py
+-rw-rw-r--   0 mo         (501) staff       (20)      519 2023-07-29 00:01:46.000000 dl_matrix-0.5/dl_matrix/structure/mapping/message/author/types.py
+-rw-rw-r--   0 mo         (501) staff       (20)     4098 2023-07-26 22:20:17.000000 dl_matrix-0.5/dl_matrix/structure/mapping/message/base.py
+drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-30 01:11:23.335195 dl_matrix-0.5/dl_matrix/structure/mapping/message/connection/
+-rw-rw-r--   0 mo         (501) staff       (20)       26 2023-07-26 18:33:05.000000 dl_matrix-0.5/dl_matrix/structure/mapping/message/connection/__init__.py
+-rw-r--r--   0 mo         (501) staff       (20)     3246 2023-07-26 19:03:33.000000 dl_matrix-0.5/dl_matrix/structure/mapping/message/connection/connection.py
+-rw-r--r--   0 mo         (501) staff       (20)      390 2023-07-26 19:03:33.000000 dl_matrix-0.5/dl_matrix/structure/mapping/message/connection/types.py
+drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-30 01:11:23.336173 dl_matrix-0.5/dl_matrix/structure/mapping/message/content/
+-rw-rw-r--   0 mo         (501) staff       (20)       26 2023-07-23 02:50:38.000000 dl_matrix-0.5/dl_matrix/structure/mapping/message/content/__init__.py
+-rw-rw-r--   0 mo         (501) staff       (20)     1979 2023-07-28 21:42:12.000000 dl_matrix-0.5/dl_matrix/structure/mapping/message/content/base.py
+drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-30 01:11:23.339616 dl_matrix-0.5/dl_matrix/structure/mapping/message/content/embedding/
+-rw-r--r--   0 mo         (501) staff       (20)       28 2023-07-27 14:28:59.000000 dl_matrix-0.5/dl_matrix/structure/mapping/message/content/embedding/__init__.py
+-rw-r--r--   0 mo         (501) staff       (20)     1779 2023-07-27 14:28:59.000000 dl_matrix-0.5/dl_matrix/structure/mapping/message/content/embedding/base.py
+drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-30 01:11:23.340210 dl_matrix-0.5/dl_matrix/structure/mapping/message/content/moderation/
+-rw-r--r--   0 mo         (501) staff       (20)       41 2023-07-26 18:15:19.000000 dl_matrix-0.5/dl_matrix/structure/mapping/message/content/moderation/__init__.py
+-rw-r--r--   0 mo         (501) staff       (20)     1641 2023-07-26 18:41:17.000000 dl_matrix-0.5/dl_matrix/structure/mapping/message/content/moderation/moderation.py
+drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-30 01:11:23.340801 dl_matrix-0.5/dl_matrix/structure/mapping/message/content/production/
+-rw-r--r--   0 mo         (501) staff       (20)       40 2023-07-28 15:06:09.000000 dl_matrix-0.5/dl_matrix/structure/mapping/message/content/production/__init__.py
+-rw-r--r--   0 mo         (501) staff       (20)     9478 2023-07-26 18:03:16.000000 dl_matrix-0.5/dl_matrix/structure/mapping/message/content/production/production.py
+drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-30 01:11:23.342426 dl_matrix-0.5/dl_matrix/structure/mapping/message/content/query/
+-rw-rw-r--   0 mo         (501) staff       (20)       59 2023-07-28 19:09:39.000000 dl_matrix-0.5/dl_matrix/structure/mapping/message/content/query/__init__.py
+-rw-r--r--   0 mo         (501) staff       (20)    10697 2023-07-28 21:42:12.000000 dl_matrix-0.5/dl_matrix/structure/mapping/message/content/query/query_generator.py
+-rw-r--r--   0 mo         (501) staff       (20)     6479 2023-07-28 21:42:12.000000 dl_matrix-0.5/dl_matrix/structure/mapping/message/content/query/query_parser.py
+-rw-rw-r--   0 mo         (501) staff       (20)     1089 2023-07-21 22:09:42.000000 dl_matrix-0.5/dl_matrix/structure/mapping/message/content/types.py
+drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-30 01:11:23.342995 dl_matrix-0.5/dl_matrix/structure/mapping/message/metadata/
+-rw-rw-r--   0 mo         (501) staff       (20)       31 2023-07-21 22:10:58.000000 dl_matrix-0.5/dl_matrix/structure/mapping/message/metadata/__init__.py
+-rw-rw-r--   0 mo         (501) staff       (20)     5866 2023-07-25 01:35:05.000000 dl_matrix-0.5/dl_matrix/structure/mapping/message/metadata/metadata.py
+drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-30 01:11:23.343766 dl_matrix-0.5/dl_matrix/visualization/
+-rw-rw-r--   0 mo         (501) staff       (20)       46 2023-07-27 18:06:28.000000 dl_matrix-0.5/dl_matrix/visualization/__init__.py
+-rw-rw-r--   0 mo         (501) staff       (20)     4176 2023-07-27 18:06:29.000000 dl_matrix-0.5/dl_matrix/visualization/app.py
+-rw-rw-r--   0 mo         (501) staff       (20)     8755 2023-07-29 21:01:15.000000 dl_matrix-0.5/dl_matrix/visualization/psychedelic.py
+drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-30 01:11:23.324061 dl_matrix-0.5/dl_matrix.egg-info/
+-rw-r--r--   0 mo         (501) staff       (20)     3125 2023-07-30 01:11:23.000000 dl_matrix-0.5/dl_matrix.egg-info/PKG-INFO
+-rw-r--r--   0 mo         (501) staff       (20)     2783 2023-07-30 01:11:23.000000 dl_matrix-0.5/dl_matrix.egg-info/SOURCES.txt
+-rw-r--r--   0 mo         (501) staff       (20)        1 2023-07-30 01:11:23.000000 dl_matrix-0.5/dl_matrix.egg-info/dependency_links.txt
+-rw-r--r--   0 mo         (501) staff       (20)     2856 2023-07-30 01:11:23.000000 dl_matrix-0.5/dl_matrix.egg-info/requires.txt
+-rw-r--r--   0 mo         (501) staff       (20)       10 2023-07-30 01:11:23.000000 dl_matrix-0.5/dl_matrix.egg-info/top_level.txt
+-rw-r--r--   0 mo         (501) staff       (20)     2856 2023-07-30 01:10:37.000000 dl_matrix-0.5/requirements.txt
+-rw-r--r--   0 mo         (501) staff       (20)       38 2023-07-30 01:11:23.344320 dl_matrix-0.5/setup.cfg
+-rw-r--r--   0 mo         (501) staff       (20)      735 2023-07-30 01:10:56.000000 dl_matrix-0.5/setup.py
```

### Comparing `dl_matrix-0.4/LICENSE` & `dl_matrix-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.4/PKG-INFO` & `dl_matrix-0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dl_matrix
-Version: 0.4
+Version: 0.5
 Summary: A Divergent Language Matrix package
 Home-page: https://github.com/diomandeee/dl_matrix
 Author: Mohamed Diomande
 Author-email: gdiomande7907@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dl_matrix-0.4/README.md` & `dl_matrix-0.5/README.md`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.4/dl_matrix/builder.py` & `dl_matrix-0.5/dl_matrix/builder.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.4/dl_matrix/context.py` & `dl_matrix-0.5/dl_matrix/context.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.4/dl_matrix/coordinate/base.py` & `dl_matrix-0.5/dl_matrix/coordinate/base.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.4/dl_matrix/coordinate/complex.py` & `dl_matrix-0.5/dl_matrix/coordinate/complex.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.4/dl_matrix/coordinate/components/base.py` & `dl_matrix-0.5/dl_matrix/coordinate/components/base.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.4/dl_matrix/coordinate/components/depth.py` & `dl_matrix-0.5/dl_matrix/coordinate/components/depth.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.4/dl_matrix/coordinate/components/sibling.py` & `dl_matrix-0.5/dl_matrix/coordinate/components/sibling.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.4/dl_matrix/coordinate/components/sibling_count.py` & `dl_matrix-0.5/dl_matrix/coordinate/components/sibling_count.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.4/dl_matrix/coordinate/components/time.py` & `dl_matrix-0.5/dl_matrix/coordinate/components/time.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.4/dl_matrix/coordinate/matcher.py` & `dl_matrix-0.5/dl_matrix/coordinate/matcher.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.4/dl_matrix/coordinate/model.py` & `dl_matrix-0.5/dl_matrix/coordinate/model.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.4/dl_matrix/coordinate/tree.py` & `dl_matrix-0.5/dl_matrix/coordinate/tree.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.4/dl_matrix/coordinate/utils.py` & `dl_matrix-0.5/dl_matrix/coordinate/utils.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.4/dl_matrix/parsers.py` & `dl_matrix-0.5/dl_matrix/parsers.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.4/dl_matrix/relationship.py` & `dl_matrix-0.5/dl_matrix/relationship.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.4/dl_matrix/representation/animate.py` & `dl_matrix-0.5/dl_matrix/representation/animate.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.4/dl_matrix/representation/base.py` & `dl_matrix-0.5/dl_matrix/representation/base.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.4/dl_matrix/representation/combine.py` & `dl_matrix-0.5/dl_matrix/representation/combine.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.4/dl_matrix/representation/compute.py` & `dl_matrix-0.5/dl_matrix/representation/compute.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.4/dl_matrix/representation/estimator.py` & `dl_matrix-0.5/dl_matrix/representation/estimator.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.4/dl_matrix/representation/filters.py` & `dl_matrix-0.5/dl_matrix/representation/filters.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.4/dl_matrix/representation/handler.py` & `dl_matrix-0.5/dl_matrix/representation/handler.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.4/dl_matrix/schema.py` & `dl_matrix-0.5/dl_matrix/schema.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.4/dl_matrix/similarity.py` & `dl_matrix-0.5/dl_matrix/similarity.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.4/dl_matrix/structure/base.py` & `dl_matrix-0.5/dl_matrix/structure/base.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.4/dl_matrix/structure/mapping/base.py` & `dl_matrix-0.5/dl_matrix/structure/mapping/base.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.4/dl_matrix/structure/mapping/message/author/author.py` & `dl_matrix-0.5/dl_matrix/structure/mapping/message/author/author.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.4/dl_matrix/structure/mapping/message/author/role.py` & `dl_matrix-0.5/dl_matrix/structure/mapping/message/author/role.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.4/dl_matrix/structure/mapping/message/author/synthesis.py` & `dl_matrix-0.5/dl_matrix/structure/mapping/message/author/synthesis.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.4/dl_matrix/structure/mapping/message/author/types.py` & `dl_matrix-0.5/dl_matrix/structure/mapping/message/author/types.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.4/dl_matrix/structure/mapping/message/base.py` & `dl_matrix-0.5/dl_matrix/structure/mapping/message/base.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.4/dl_matrix/structure/mapping/message/connection/connection.py` & `dl_matrix-0.5/dl_matrix/structure/mapping/message/connection/connection.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.4/dl_matrix/structure/mapping/message/content/base.py` & `dl_matrix-0.5/dl_matrix/structure/mapping/message/content/base.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.4/dl_matrix/structure/mapping/message/content/embedding/base.py` & `dl_matrix-0.5/dl_matrix/structure/mapping/message/content/embedding/base.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.4/dl_matrix/structure/mapping/message/content/moderation/moderation.py` & `dl_matrix-0.5/dl_matrix/structure/mapping/message/content/moderation/moderation.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.4/dl_matrix/structure/mapping/message/content/production/production.py` & `dl_matrix-0.5/dl_matrix/structure/mapping/message/content/production/production.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.4/dl_matrix/structure/mapping/message/content/query/query_generator.py` & `dl_matrix-0.5/dl_matrix/structure/mapping/message/content/query/query_generator.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.4/dl_matrix/structure/mapping/message/content/query/query_parser.py` & `dl_matrix-0.5/dl_matrix/structure/mapping/message/content/query/query_parser.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.4/dl_matrix/structure/mapping/message/content/types.py` & `dl_matrix-0.5/dl_matrix/structure/mapping/message/content/types.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.4/dl_matrix/structure/mapping/message/metadata/metadata.py` & `dl_matrix-0.5/dl_matrix/structure/mapping/message/metadata/metadata.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.4/dl_matrix/visualization/app.py` & `dl_matrix-0.5/dl_matrix/visualization/app.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.4/dl_matrix/visualization/psychedelic.py` & `dl_matrix-0.5/dl_matrix/visualization/psychedelic.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.4/dl_matrix.egg-info/PKG-INFO` & `dl_matrix-0.5/dl_matrix.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dl-matrix
-Version: 0.4
+Version: 0.5
 Summary: A Divergent Language Matrix package
 Home-page: https://github.com/diomandeee/dl_matrix
 Author: Mohamed Diomande
 Author-email: gdiomande7907@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dl_matrix-0.4/dl_matrix.egg-info/SOURCES.txt` & `dl_matrix-0.5/dl_matrix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.4/dl_matrix.egg-info/requires.txt` & `dl_matrix-0.5/dl_matrix.egg-info/requires.txt`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 dash-table==5.0.0
 dataclasses-json==0.5.13
 datasets==2.14.1
 debugpy==1.6.7
 decorator==5.1.1
 dill==0.3.7
 editdistpy==0.1.3
-en-core-web-md@ https://github.com/explosion/spacy-models/releases/download/en_core_web_md-3.6.0/en_core_web_md-3.6.0-py3-none-any.whl#sha256=1618fc62e7aedc2b778caa3ea6e9c8280beac3b83fe7b93316cbb9e8f3abe7c5
 executing==1.2.0
 filelock==3.12.2
 Flask==2.2.5
 fonttools==4.41.1
 frozenlist==1.4.0
 fsspec==2023.6.0
 googleapis-common-protos==1.59.1
```

### Comparing `dl_matrix-0.4/requirements.txt` & `dl_matrix-0.5/requirements.txt`

 * *Files 9% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 dash-table==5.0.0
 dataclasses-json==0.5.13
 datasets==2.14.1
 debugpy==1.6.7
 decorator==5.1.1
 dill==0.3.7
 editdistpy==0.1.3
-en-core-web-md @ https://github.com/explosion/spacy-models/releases/download/en_core_web_md-3.6.0/en_core_web_md-3.6.0-py3-none-any.whl#sha256=1618fc62e7aedc2b778caa3ea6e9c8280beac3b83fe7b93316cbb9e8f3abe7c5
 executing==1.2.0
 filelock==3.12.2
 Flask==2.2.5
 fonttools==4.41.1
 frozenlist==1.4.0
 fsspec==2023.6.0
 googleapis-common-protos==1.59.1
```

### Comparing `dl_matrix-0.4/setup.py` & `dl_matrix-0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='dl_matrix',
-    version="0.4",
+    version="0.5",
     author="Mohamed Diomande",
     author_email="gdiomande7907@gmail.com",
     description='A Divergent Language Matrix package',
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/diomandeee/dl_matrix",
     packages=find_packages(),
```

