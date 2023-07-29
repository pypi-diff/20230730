# Comparing `tmp/dl_matrix-0.2.tar.gz` & `tmp/dl_matrix-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dl_matrix-0.2.tar", last modified: Sat Jul 29 22:44:23 2023, max compression
+gzip compressed data, was "dl_matrix-0.4.tar", last modified: Sat Jul 29 23:12:40 2023, max compression
```

## Comparing `dl_matrix-0.2.tar` & `dl_matrix-0.4.tar`

### file list

```diff
@@ -1,87 +1,89 @@
-drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-29 22:44:23.257489 dl_matrix-0.2/
--rw-r--r--   0 mo         (501) staff       (20)     1073 2023-07-29 21:15:54.000000 dl_matrix-0.2/LICENSE
--rw-r--r--   0 mo         (501) staff       (20)     3303 2023-07-29 22:44:23.257362 dl_matrix-0.2/PKG-INFO
--rw-r--r--   0 mo         (501) staff       (20)     2670 2023-07-29 21:36:22.000000 dl_matrix-0.2/README.md
-drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-29 22:44:23.241374 dl_matrix-0.2/dl_matrix/
--rw-rw-r--   0 mo         (501) staff       (20)      109 2023-07-29 21:38:05.000000 dl_matrix-0.2/dl_matrix/__init__.py
--rw-rw-r--   0 mo         (501) staff       (20)    11557 2023-07-29 21:01:15.000000 dl_matrix-0.2/dl_matrix/builder.py
--rw-rw-r--   0 mo         (501) staff       (20)     5889 2023-07-27 22:03:15.000000 dl_matrix-0.2/dl_matrix/context.py
-drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-29 22:44:23.244042 dl_matrix-0.2/dl_matrix/coordinate/
--rw-rw-r--   0 mo         (501) staff       (20)       21 2023-07-28 00:45:01.000000 dl_matrix-0.2/dl_matrix/coordinate/__init__.py
--rw-rw-r--   0 mo         (501) staff       (20)    19532 2023-07-28 02:59:26.000000 dl_matrix-0.2/dl_matrix/coordinate/base.py
--rw-r--r--   0 mo         (501) staff       (20)     9568 2023-07-28 14:07:23.000000 dl_matrix-0.2/dl_matrix/coordinate/complex.py
-drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-29 22:44:23.246034 dl_matrix-0.2/dl_matrix/coordinate/components/
--rw-rw-r--   0 mo         (501) staff       (20)      153 2023-07-27 02:26:31.000000 dl_matrix-0.2/dl_matrix/coordinate/components/__init__.py
--rw-rw-r--   0 mo         (501) staff       (20)     1773 2023-07-26 00:08:02.000000 dl_matrix-0.2/dl_matrix/coordinate/components/base.py
--rw-rw-r--   0 mo         (501) staff       (20)     1874 2023-07-27 18:06:28.000000 dl_matrix-0.2/dl_matrix/coordinate/components/depth.py
--rw-rw-r--   0 mo         (501) staff       (20)     1460 2023-07-27 18:06:28.000000 dl_matrix-0.2/dl_matrix/coordinate/components/sibling.py
--rw-rw-r--   0 mo         (501) staff       (20)     1636 2023-07-27 18:06:28.000000 dl_matrix-0.2/dl_matrix/coordinate/components/sibling_count.py
--rw-rw-r--   0 mo         (501) staff       (20)     2286 2023-07-27 18:06:28.000000 dl_matrix-0.2/dl_matrix/coordinate/components/time.py
--rw-r--r--   0 mo         (501) staff       (20)    11877 2023-07-28 14:07:23.000000 dl_matrix-0.2/dl_matrix/coordinate/matcher.py
--rw-r--r--   0 mo         (501) staff       (20)     6824 2023-07-28 02:59:20.000000 dl_matrix-0.2/dl_matrix/coordinate/model.py
--rw-r--r--   0 mo         (501) staff       (20)     5921 2023-07-28 02:59:31.000000 dl_matrix-0.2/dl_matrix/coordinate/tree.py
--rw-r--r--   0 mo         (501) staff       (20)    11906 2023-07-28 02:12:21.000000 dl_matrix-0.2/dl_matrix/coordinate/utils.py
--rw-rw-r--   0 mo         (501) staff       (20)     3817 2023-07-28 02:12:21.000000 dl_matrix-0.2/dl_matrix/parsers.py
--rw-rw-r--   0 mo         (501) staff       (20)    26111 2023-07-29 20:48:16.000000 dl_matrix-0.2/dl_matrix/relationship.py
-drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-29 22:44:23.248043 dl_matrix-0.2/dl_matrix/representation/
--rw-rw-r--   0 mo         (501) staff       (20)       96 2023-07-28 13:18:53.000000 dl_matrix-0.2/dl_matrix/representation/__init__.py
--rw-r--r--   0 mo         (501) staff       (20)     4648 2023-07-28 02:59:41.000000 dl_matrix-0.2/dl_matrix/representation/animate.py
--rw-rw-r--   0 mo         (501) staff       (20)    10399 2023-07-29 20:47:32.000000 dl_matrix-0.2/dl_matrix/representation/base.py
--rw-r--r--   0 mo         (501) staff       (20)    11017 2023-07-29 20:44:23.000000 dl_matrix-0.2/dl_matrix/representation/combine.py
--rw-rw-r--   0 mo         (501) staff       (20)    14786 2023-07-29 20:43:20.000000 dl_matrix-0.2/dl_matrix/representation/compute.py
--rw-rw-r--   0 mo         (501) staff       (20)     6965 2023-07-28 02:33:05.000000 dl_matrix-0.2/dl_matrix/representation/estimator.py
--rw-rw-r--   0 mo         (501) staff       (20)     9633 2023-07-29 01:48:25.000000 dl_matrix-0.2/dl_matrix/representation/filters.py
--rw-r--r--   0 mo         (501) staff       (20)     5379 2023-07-28 14:07:23.000000 dl_matrix-0.2/dl_matrix/representation/handler.py
--rw-rw-r--   0 mo         (501) staff       (20)    11569 2023-07-29 16:28:17.000000 dl_matrix-0.2/dl_matrix/schema.py
--rw-rw-r--   0 mo         (501) staff       (20)    10299 2023-07-29 00:46:29.000000 dl_matrix-0.2/dl_matrix/similarity.py
-drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-29 22:44:23.248577 dl_matrix-0.2/dl_matrix/structure/
--rw-rw-r--   0 mo         (501) staff       (20)       43 2023-07-26 16:06:54.000000 dl_matrix-0.2/dl_matrix/structure/__init__.py
--rw-rw-r--   0 mo         (501) staff       (20)    12267 2023-07-29 12:38:03.000000 dl_matrix-0.2/dl_matrix/structure/base.py
-drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-29 22:44:23.249077 dl_matrix-0.2/dl_matrix/structure/mapping/
--rw-rw-r--   0 mo         (501) staff       (20)       76 2023-07-24 15:55:42.000000 dl_matrix-0.2/dl_matrix/structure/mapping/__init__.py
--rw-rw-r--   0 mo         (501) staff       (20)     5688 2023-07-28 21:42:12.000000 dl_matrix-0.2/dl_matrix/structure/mapping/base.py
-drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-29 22:44:23.249629 dl_matrix-0.2/dl_matrix/structure/mapping/message/
--rw-rw-r--   0 mo         (501) staff       (20)       20 2023-07-21 22:10:26.000000 dl_matrix-0.2/dl_matrix/structure/mapping/message/__init__.py
-drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-29 22:44:23.251716 dl_matrix-0.2/dl_matrix/structure/mapping/message/author/
--rw-rw-r--   0 mo         (501) staff       (20)       57 2023-07-29 01:48:25.000000 dl_matrix-0.2/dl_matrix/structure/mapping/message/author/__init__.py
--rw-rw-r--   0 mo         (501) staff       (20)     1303 2023-07-24 22:43:21.000000 dl_matrix-0.2/dl_matrix/structure/mapping/message/author/author.py
--rw-rw-r--   0 mo         (501) staff       (20)     1767 2023-07-24 22:49:37.000000 dl_matrix-0.2/dl_matrix/structure/mapping/message/author/role.py
--rw-rw-r--   0 mo         (501) staff       (20)     4387 2023-07-24 22:49:37.000000 dl_matrix-0.2/dl_matrix/structure/mapping/message/author/synthesis.py
--rw-rw-r--   0 mo         (501) staff       (20)      519 2023-07-29 00:01:46.000000 dl_matrix-0.2/dl_matrix/structure/mapping/message/author/types.py
--rw-rw-r--   0 mo         (501) staff       (20)     4098 2023-07-26 22:20:17.000000 dl_matrix-0.2/dl_matrix/structure/mapping/message/base.py
-drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-29 22:44:23.252378 dl_matrix-0.2/dl_matrix/structure/mapping/message/connection/
--rw-rw-r--   0 mo         (501) staff       (20)       26 2023-07-26 18:33:05.000000 dl_matrix-0.2/dl_matrix/structure/mapping/message/connection/__init__.py
--rw-r--r--   0 mo         (501) staff       (20)     3246 2023-07-26 19:03:33.000000 dl_matrix-0.2/dl_matrix/structure/mapping/message/connection/connection.py
--rw-r--r--   0 mo         (501) staff       (20)      390 2023-07-26 19:03:33.000000 dl_matrix-0.2/dl_matrix/structure/mapping/message/connection/types.py
-drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-29 22:44:23.253276 dl_matrix-0.2/dl_matrix/structure/mapping/message/content/
--rw-rw-r--   0 mo         (501) staff       (20)       26 2023-07-23 02:50:38.000000 dl_matrix-0.2/dl_matrix/structure/mapping/message/content/__init__.py
--rw-rw-r--   0 mo         (501) staff       (20)     1979 2023-07-28 21:42:12.000000 dl_matrix-0.2/dl_matrix/structure/mapping/message/content/base.py
-drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-29 22:44:23.253800 dl_matrix-0.2/dl_matrix/structure/mapping/message/content/embedding/
--rw-r--r--   0 mo         (501) staff       (20)       28 2023-07-27 14:28:59.000000 dl_matrix-0.2/dl_matrix/structure/mapping/message/content/embedding/__init__.py
--rw-r--r--   0 mo         (501) staff       (20)     1779 2023-07-27 14:28:59.000000 dl_matrix-0.2/dl_matrix/structure/mapping/message/content/embedding/base.py
-drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-29 22:44:23.254368 dl_matrix-0.2/dl_matrix/structure/mapping/message/content/moderation/
--rw-r--r--   0 mo         (501) staff       (20)       41 2023-07-26 18:15:19.000000 dl_matrix-0.2/dl_matrix/structure/mapping/message/content/moderation/__init__.py
--rw-r--r--   0 mo         (501) staff       (20)     1641 2023-07-26 18:41:17.000000 dl_matrix-0.2/dl_matrix/structure/mapping/message/content/moderation/moderation.py
-drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-29 22:44:23.254919 dl_matrix-0.2/dl_matrix/structure/mapping/message/content/production/
--rw-r--r--   0 mo         (501) staff       (20)       40 2023-07-28 15:06:09.000000 dl_matrix-0.2/dl_matrix/structure/mapping/message/content/production/__init__.py
--rw-r--r--   0 mo         (501) staff       (20)     9478 2023-07-26 18:03:16.000000 dl_matrix-0.2/dl_matrix/structure/mapping/message/content/production/production.py
-drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-29 22:44:23.255823 dl_matrix-0.2/dl_matrix/structure/mapping/message/content/query/
--rw-rw-r--   0 mo         (501) staff       (20)       59 2023-07-28 19:09:39.000000 dl_matrix-0.2/dl_matrix/structure/mapping/message/content/query/__init__.py
--rw-r--r--   0 mo         (501) staff       (20)    10697 2023-07-28 21:42:12.000000 dl_matrix-0.2/dl_matrix/structure/mapping/message/content/query/query_generator.py
--rw-r--r--   0 mo         (501) staff       (20)     6479 2023-07-28 21:42:12.000000 dl_matrix-0.2/dl_matrix/structure/mapping/message/content/query/query_parser.py
--rw-rw-r--   0 mo         (501) staff       (20)     1089 2023-07-21 22:09:42.000000 dl_matrix-0.2/dl_matrix/structure/mapping/message/content/types.py
-drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-29 22:44:23.256336 dl_matrix-0.2/dl_matrix/structure/mapping/message/metadata/
--rw-rw-r--   0 mo         (501) staff       (20)       31 2023-07-21 22:10:58.000000 dl_matrix-0.2/dl_matrix/structure/mapping/message/metadata/__init__.py
--rw-rw-r--   0 mo         (501) staff       (20)     5866 2023-07-25 01:35:05.000000 dl_matrix-0.2/dl_matrix/structure/mapping/message/metadata/metadata.py
-drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-29 22:44:23.257057 dl_matrix-0.2/dl_matrix/visualization/
--rw-rw-r--   0 mo         (501) staff       (20)       46 2023-07-27 18:06:28.000000 dl_matrix-0.2/dl_matrix/visualization/__init__.py
--rw-rw-r--   0 mo         (501) staff       (20)     4176 2023-07-27 18:06:29.000000 dl_matrix-0.2/dl_matrix/visualization/app.py
--rw-rw-r--   0 mo         (501) staff       (20)     8755 2023-07-29 21:01:15.000000 dl_matrix-0.2/dl_matrix/visualization/psychedelic.py
-drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-29 22:44:23.242127 dl_matrix-0.2/dl_matrix.egg-info/
--rw-r--r--   0 mo         (501) staff       (20)     3303 2023-07-29 22:44:23.000000 dl_matrix-0.2/dl_matrix.egg-info/PKG-INFO
--rw-r--r--   0 mo         (501) staff       (20)     2754 2023-07-29 22:44:23.000000 dl_matrix-0.2/dl_matrix.egg-info/SOURCES.txt
--rw-r--r--   0 mo         (501) staff       (20)        1 2023-07-29 22:44:23.000000 dl_matrix-0.2/dl_matrix.egg-info/dependency_links.txt
--rw-r--r--   0 mo         (501) staff       (20)     3063 2023-07-29 22:44:23.000000 dl_matrix-0.2/dl_matrix.egg-info/requires.txt
--rw-r--r--   0 mo         (501) staff       (20)       10 2023-07-29 22:44:23.000000 dl_matrix-0.2/dl_matrix.egg-info/top_level.txt
--rw-r--r--   0 mo         (501) staff       (20)       38 2023-07-29 22:44:23.257529 dl_matrix-0.2/setup.cfg
--rw-r--r--   0 mo         (501) staff       (20)      915 2023-07-29 22:43:29.000000 dl_matrix-0.2/setup.py
+drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-29 23:12:40.735035 dl_matrix-0.4/
+-rw-r--r--   0 mo         (501) staff       (20)     1073 2023-07-29 21:15:54.000000 dl_matrix-0.4/LICENSE
+-rw-r--r--   0 mo         (501) staff       (20)       25 2023-07-29 23:03:07.000000 dl_matrix-0.4/MANIFEST.in
+-rw-r--r--   0 mo         (501) staff       (20)     3125 2023-07-29 23:12:40.734888 dl_matrix-0.4/PKG-INFO
+-rw-r--r--   0 mo         (501) staff       (20)     2670 2023-07-29 21:36:22.000000 dl_matrix-0.4/README.md
+drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-29 23:12:40.716038 dl_matrix-0.4/dl_matrix/
+-rw-rw-r--   0 mo         (501) staff       (20)      109 2023-07-29 21:38:05.000000 dl_matrix-0.4/dl_matrix/__init__.py
+-rw-rw-r--   0 mo         (501) staff       (20)    11557 2023-07-29 21:01:15.000000 dl_matrix-0.4/dl_matrix/builder.py
+-rw-rw-r--   0 mo         (501) staff       (20)     5889 2023-07-27 22:03:15.000000 dl_matrix-0.4/dl_matrix/context.py
+drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-29 23:12:40.720283 dl_matrix-0.4/dl_matrix/coordinate/
+-rw-rw-r--   0 mo         (501) staff       (20)       21 2023-07-28 00:45:01.000000 dl_matrix-0.4/dl_matrix/coordinate/__init__.py
+-rw-rw-r--   0 mo         (501) staff       (20)    19532 2023-07-28 02:59:26.000000 dl_matrix-0.4/dl_matrix/coordinate/base.py
+-rw-r--r--   0 mo         (501) staff       (20)     9568 2023-07-28 14:07:23.000000 dl_matrix-0.4/dl_matrix/coordinate/complex.py
+drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-29 23:12:40.722874 dl_matrix-0.4/dl_matrix/coordinate/components/
+-rw-rw-r--   0 mo         (501) staff       (20)      153 2023-07-27 02:26:31.000000 dl_matrix-0.4/dl_matrix/coordinate/components/__init__.py
+-rw-rw-r--   0 mo         (501) staff       (20)     1773 2023-07-26 00:08:02.000000 dl_matrix-0.4/dl_matrix/coordinate/components/base.py
+-rw-rw-r--   0 mo         (501) staff       (20)     1874 2023-07-27 18:06:28.000000 dl_matrix-0.4/dl_matrix/coordinate/components/depth.py
+-rw-rw-r--   0 mo         (501) staff       (20)     1460 2023-07-27 18:06:28.000000 dl_matrix-0.4/dl_matrix/coordinate/components/sibling.py
+-rw-rw-r--   0 mo         (501) staff       (20)     1636 2023-07-27 18:06:28.000000 dl_matrix-0.4/dl_matrix/coordinate/components/sibling_count.py
+-rw-rw-r--   0 mo         (501) staff       (20)     2286 2023-07-27 18:06:28.000000 dl_matrix-0.4/dl_matrix/coordinate/components/time.py
+-rw-r--r--   0 mo         (501) staff       (20)    11877 2023-07-28 14:07:23.000000 dl_matrix-0.4/dl_matrix/coordinate/matcher.py
+-rw-r--r--   0 mo         (501) staff       (20)     6824 2023-07-28 02:59:20.000000 dl_matrix-0.4/dl_matrix/coordinate/model.py
+-rw-r--r--   0 mo         (501) staff       (20)     5921 2023-07-28 02:59:31.000000 dl_matrix-0.4/dl_matrix/coordinate/tree.py
+-rw-r--r--   0 mo         (501) staff       (20)    11906 2023-07-28 02:12:21.000000 dl_matrix-0.4/dl_matrix/coordinate/utils.py
+-rw-rw-r--   0 mo         (501) staff       (20)     3817 2023-07-28 02:12:21.000000 dl_matrix-0.4/dl_matrix/parsers.py
+-rw-rw-r--   0 mo         (501) staff       (20)    26111 2023-07-29 20:48:16.000000 dl_matrix-0.4/dl_matrix/relationship.py
+drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-29 23:12:40.725481 dl_matrix-0.4/dl_matrix/representation/
+-rw-rw-r--   0 mo         (501) staff       (20)       96 2023-07-28 13:18:53.000000 dl_matrix-0.4/dl_matrix/representation/__init__.py
+-rw-r--r--   0 mo         (501) staff       (20)     4648 2023-07-28 02:59:41.000000 dl_matrix-0.4/dl_matrix/representation/animate.py
+-rw-rw-r--   0 mo         (501) staff       (20)    10399 2023-07-29 20:47:32.000000 dl_matrix-0.4/dl_matrix/representation/base.py
+-rw-r--r--   0 mo         (501) staff       (20)    11017 2023-07-29 20:44:23.000000 dl_matrix-0.4/dl_matrix/representation/combine.py
+-rw-rw-r--   0 mo         (501) staff       (20)    14786 2023-07-29 20:43:20.000000 dl_matrix-0.4/dl_matrix/representation/compute.py
+-rw-rw-r--   0 mo         (501) staff       (20)     6965 2023-07-28 02:33:05.000000 dl_matrix-0.4/dl_matrix/representation/estimator.py
+-rw-rw-r--   0 mo         (501) staff       (20)     9633 2023-07-29 01:48:25.000000 dl_matrix-0.4/dl_matrix/representation/filters.py
+-rw-r--r--   0 mo         (501) staff       (20)     5379 2023-07-28 14:07:23.000000 dl_matrix-0.4/dl_matrix/representation/handler.py
+-rw-rw-r--   0 mo         (501) staff       (20)    11569 2023-07-29 16:28:17.000000 dl_matrix-0.4/dl_matrix/schema.py
+-rw-rw-r--   0 mo         (501) staff       (20)    10299 2023-07-29 00:46:29.000000 dl_matrix-0.4/dl_matrix/similarity.py
+drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-29 23:12:40.726195 dl_matrix-0.4/dl_matrix/structure/
+-rw-rw-r--   0 mo         (501) staff       (20)       43 2023-07-26 16:06:54.000000 dl_matrix-0.4/dl_matrix/structure/__init__.py
+-rw-rw-r--   0 mo         (501) staff       (20)    12267 2023-07-29 12:38:03.000000 dl_matrix-0.4/dl_matrix/structure/base.py
+drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-29 23:12:40.726716 dl_matrix-0.4/dl_matrix/structure/mapping/
+-rw-rw-r--   0 mo         (501) staff       (20)       76 2023-07-24 15:55:42.000000 dl_matrix-0.4/dl_matrix/structure/mapping/__init__.py
+-rw-rw-r--   0 mo         (501) staff       (20)     5688 2023-07-28 21:42:12.000000 dl_matrix-0.4/dl_matrix/structure/mapping/base.py
+drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-29 23:12:40.727310 dl_matrix-0.4/dl_matrix/structure/mapping/message/
+-rw-rw-r--   0 mo         (501) staff       (20)       20 2023-07-21 22:10:26.000000 dl_matrix-0.4/dl_matrix/structure/mapping/message/__init__.py
+drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-29 23:12:40.729458 dl_matrix-0.4/dl_matrix/structure/mapping/message/author/
+-rw-rw-r--   0 mo         (501) staff       (20)       57 2023-07-29 01:48:25.000000 dl_matrix-0.4/dl_matrix/structure/mapping/message/author/__init__.py
+-rw-rw-r--   0 mo         (501) staff       (20)     1303 2023-07-24 22:43:21.000000 dl_matrix-0.4/dl_matrix/structure/mapping/message/author/author.py
+-rw-rw-r--   0 mo         (501) staff       (20)     1767 2023-07-24 22:49:37.000000 dl_matrix-0.4/dl_matrix/structure/mapping/message/author/role.py
+-rw-rw-r--   0 mo         (501) staff       (20)     4387 2023-07-24 22:49:37.000000 dl_matrix-0.4/dl_matrix/structure/mapping/message/author/synthesis.py
+-rw-rw-r--   0 mo         (501) staff       (20)      519 2023-07-29 00:01:46.000000 dl_matrix-0.4/dl_matrix/structure/mapping/message/author/types.py
+-rw-rw-r--   0 mo         (501) staff       (20)     4098 2023-07-26 22:20:17.000000 dl_matrix-0.4/dl_matrix/structure/mapping/message/base.py
+drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-29 23:12:40.730175 dl_matrix-0.4/dl_matrix/structure/mapping/message/connection/
+-rw-rw-r--   0 mo         (501) staff       (20)       26 2023-07-26 18:33:05.000000 dl_matrix-0.4/dl_matrix/structure/mapping/message/connection/__init__.py
+-rw-r--r--   0 mo         (501) staff       (20)     3246 2023-07-26 19:03:33.000000 dl_matrix-0.4/dl_matrix/structure/mapping/message/connection/connection.py
+-rw-r--r--   0 mo         (501) staff       (20)      390 2023-07-26 19:03:33.000000 dl_matrix-0.4/dl_matrix/structure/mapping/message/connection/types.py
+drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-29 23:12:40.731032 dl_matrix-0.4/dl_matrix/structure/mapping/message/content/
+-rw-rw-r--   0 mo         (501) staff       (20)       26 2023-07-23 02:50:38.000000 dl_matrix-0.4/dl_matrix/structure/mapping/message/content/__init__.py
+-rw-rw-r--   0 mo         (501) staff       (20)     1979 2023-07-28 21:42:12.000000 dl_matrix-0.4/dl_matrix/structure/mapping/message/content/base.py
+drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-29 23:12:40.731529 dl_matrix-0.4/dl_matrix/structure/mapping/message/content/embedding/
+-rw-r--r--   0 mo         (501) staff       (20)       28 2023-07-27 14:28:59.000000 dl_matrix-0.4/dl_matrix/structure/mapping/message/content/embedding/__init__.py
+-rw-r--r--   0 mo         (501) staff       (20)     1779 2023-07-27 14:28:59.000000 dl_matrix-0.4/dl_matrix/structure/mapping/message/content/embedding/base.py
+drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-29 23:12:40.732002 dl_matrix-0.4/dl_matrix/structure/mapping/message/content/moderation/
+-rw-r--r--   0 mo         (501) staff       (20)       41 2023-07-26 18:15:19.000000 dl_matrix-0.4/dl_matrix/structure/mapping/message/content/moderation/__init__.py
+-rw-r--r--   0 mo         (501) staff       (20)     1641 2023-07-26 18:41:17.000000 dl_matrix-0.4/dl_matrix/structure/mapping/message/content/moderation/moderation.py
+drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-29 23:12:40.732507 dl_matrix-0.4/dl_matrix/structure/mapping/message/content/production/
+-rw-r--r--   0 mo         (501) staff       (20)       40 2023-07-28 15:06:09.000000 dl_matrix-0.4/dl_matrix/structure/mapping/message/content/production/__init__.py
+-rw-r--r--   0 mo         (501) staff       (20)     9478 2023-07-26 18:03:16.000000 dl_matrix-0.4/dl_matrix/structure/mapping/message/content/production/production.py
+drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-29 23:12:40.733322 dl_matrix-0.4/dl_matrix/structure/mapping/message/content/query/
+-rw-rw-r--   0 mo         (501) staff       (20)       59 2023-07-28 19:09:39.000000 dl_matrix-0.4/dl_matrix/structure/mapping/message/content/query/__init__.py
+-rw-r--r--   0 mo         (501) staff       (20)    10697 2023-07-28 21:42:12.000000 dl_matrix-0.4/dl_matrix/structure/mapping/message/content/query/query_generator.py
+-rw-r--r--   0 mo         (501) staff       (20)     6479 2023-07-28 21:42:12.000000 dl_matrix-0.4/dl_matrix/structure/mapping/message/content/query/query_parser.py
+-rw-rw-r--   0 mo         (501) staff       (20)     1089 2023-07-21 22:09:42.000000 dl_matrix-0.4/dl_matrix/structure/mapping/message/content/types.py
+drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-29 23:12:40.733823 dl_matrix-0.4/dl_matrix/structure/mapping/message/metadata/
+-rw-rw-r--   0 mo         (501) staff       (20)       31 2023-07-21 22:10:58.000000 dl_matrix-0.4/dl_matrix/structure/mapping/message/metadata/__init__.py
+-rw-rw-r--   0 mo         (501) staff       (20)     5866 2023-07-25 01:35:05.000000 dl_matrix-0.4/dl_matrix/structure/mapping/message/metadata/metadata.py
+drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-29 23:12:40.734538 dl_matrix-0.4/dl_matrix/visualization/
+-rw-rw-r--   0 mo         (501) staff       (20)       46 2023-07-27 18:06:28.000000 dl_matrix-0.4/dl_matrix/visualization/__init__.py
+-rw-rw-r--   0 mo         (501) staff       (20)     4176 2023-07-27 18:06:29.000000 dl_matrix-0.4/dl_matrix/visualization/app.py
+-rw-rw-r--   0 mo         (501) staff       (20)     8755 2023-07-29 21:01:15.000000 dl_matrix-0.4/dl_matrix/visualization/psychedelic.py
+drwxr-xr-x   0 mo         (501) staff       (20)        0 2023-07-29 23:12:40.716968 dl_matrix-0.4/dl_matrix.egg-info/
+-rw-r--r--   0 mo         (501) staff       (20)     3125 2023-07-29 23:12:40.000000 dl_matrix-0.4/dl_matrix.egg-info/PKG-INFO
+-rw-r--r--   0 mo         (501) staff       (20)     2783 2023-07-29 23:12:40.000000 dl_matrix-0.4/dl_matrix.egg-info/SOURCES.txt
+-rw-r--r--   0 mo         (501) staff       (20)        1 2023-07-29 23:12:40.000000 dl_matrix-0.4/dl_matrix.egg-info/dependency_links.txt
+-rw-r--r--   0 mo         (501) staff       (20)     3063 2023-07-29 23:12:40.000000 dl_matrix-0.4/dl_matrix.egg-info/requires.txt
+-rw-r--r--   0 mo         (501) staff       (20)       10 2023-07-29 23:12:40.000000 dl_matrix-0.4/dl_matrix.egg-info/top_level.txt
+-rw-r--r--   0 mo         (501) staff       (20)     3064 2023-07-29 21:12:00.000000 dl_matrix-0.4/requirements.txt
+-rw-r--r--   0 mo         (501) staff       (20)       38 2023-07-29 23:12:40.735079 dl_matrix-0.4/setup.cfg
+-rw-r--r--   0 mo         (501) staff       (20)      735 2023-07-29 23:12:20.000000 dl_matrix-0.4/setup.py
```

### Comparing `dl_matrix-0.2/LICENSE` & `dl_matrix-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.2/PKG-INFO` & `dl_matrix-0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 Metadata-Version: 2.1
 Name: dl_matrix
-Version: 0.2
+Version: 0.4
 Summary: A Divergent Language Matrix package
-Home-page: http://github.com/yourusername/dl_matrix
-Author: Your Name
-Author-email: your.email@example.com
+Home-page: https://github.com/diomandeee/dl_matrix
+Author: Mohamed Diomande
+Author-email: gdiomande7907@gmail.com
 License: MIT
-Keywords: divergent language matrix
-Classifier: Development Status :: 3 - Alpha
+Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Divergent Language Matrix
 
 ## Description
```

### Comparing `dl_matrix-0.2/README.md` & `dl_matrix-0.4/README.md`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.2/dl_matrix/builder.py` & `dl_matrix-0.4/dl_matrix/builder.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.2/dl_matrix/context.py` & `dl_matrix-0.4/dl_matrix/context.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.2/dl_matrix/coordinate/base.py` & `dl_matrix-0.4/dl_matrix/coordinate/base.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.2/dl_matrix/coordinate/complex.py` & `dl_matrix-0.4/dl_matrix/coordinate/complex.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.2/dl_matrix/coordinate/components/base.py` & `dl_matrix-0.4/dl_matrix/coordinate/components/base.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.2/dl_matrix/coordinate/components/depth.py` & `dl_matrix-0.4/dl_matrix/coordinate/components/depth.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.2/dl_matrix/coordinate/components/sibling.py` & `dl_matrix-0.4/dl_matrix/coordinate/components/sibling.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.2/dl_matrix/coordinate/components/sibling_count.py` & `dl_matrix-0.4/dl_matrix/coordinate/components/sibling_count.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.2/dl_matrix/coordinate/components/time.py` & `dl_matrix-0.4/dl_matrix/coordinate/components/time.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.2/dl_matrix/coordinate/matcher.py` & `dl_matrix-0.4/dl_matrix/coordinate/matcher.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.2/dl_matrix/coordinate/model.py` & `dl_matrix-0.4/dl_matrix/coordinate/model.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.2/dl_matrix/coordinate/tree.py` & `dl_matrix-0.4/dl_matrix/coordinate/tree.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.2/dl_matrix/coordinate/utils.py` & `dl_matrix-0.4/dl_matrix/coordinate/utils.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.2/dl_matrix/parsers.py` & `dl_matrix-0.4/dl_matrix/parsers.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.2/dl_matrix/relationship.py` & `dl_matrix-0.4/dl_matrix/relationship.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.2/dl_matrix/representation/animate.py` & `dl_matrix-0.4/dl_matrix/representation/animate.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.2/dl_matrix/representation/base.py` & `dl_matrix-0.4/dl_matrix/representation/base.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.2/dl_matrix/representation/combine.py` & `dl_matrix-0.4/dl_matrix/representation/combine.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.2/dl_matrix/representation/compute.py` & `dl_matrix-0.4/dl_matrix/representation/compute.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.2/dl_matrix/representation/estimator.py` & `dl_matrix-0.4/dl_matrix/representation/estimator.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.2/dl_matrix/representation/filters.py` & `dl_matrix-0.4/dl_matrix/representation/filters.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.2/dl_matrix/representation/handler.py` & `dl_matrix-0.4/dl_matrix/representation/handler.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.2/dl_matrix/schema.py` & `dl_matrix-0.4/dl_matrix/schema.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.2/dl_matrix/similarity.py` & `dl_matrix-0.4/dl_matrix/similarity.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.2/dl_matrix/structure/base.py` & `dl_matrix-0.4/dl_matrix/structure/base.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.2/dl_matrix/structure/mapping/base.py` & `dl_matrix-0.4/dl_matrix/structure/mapping/base.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.2/dl_matrix/structure/mapping/message/author/author.py` & `dl_matrix-0.4/dl_matrix/structure/mapping/message/author/author.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.2/dl_matrix/structure/mapping/message/author/role.py` & `dl_matrix-0.4/dl_matrix/structure/mapping/message/author/role.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.2/dl_matrix/structure/mapping/message/author/synthesis.py` & `dl_matrix-0.4/dl_matrix/structure/mapping/message/author/synthesis.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.2/dl_matrix/structure/mapping/message/author/types.py` & `dl_matrix-0.4/dl_matrix/structure/mapping/message/author/types.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.2/dl_matrix/structure/mapping/message/base.py` & `dl_matrix-0.4/dl_matrix/structure/mapping/message/base.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.2/dl_matrix/structure/mapping/message/connection/connection.py` & `dl_matrix-0.4/dl_matrix/structure/mapping/message/connection/connection.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.2/dl_matrix/structure/mapping/message/content/base.py` & `dl_matrix-0.4/dl_matrix/structure/mapping/message/content/base.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.2/dl_matrix/structure/mapping/message/content/embedding/base.py` & `dl_matrix-0.4/dl_matrix/structure/mapping/message/content/embedding/base.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.2/dl_matrix/structure/mapping/message/content/moderation/moderation.py` & `dl_matrix-0.4/dl_matrix/structure/mapping/message/content/moderation/moderation.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.2/dl_matrix/structure/mapping/message/content/production/production.py` & `dl_matrix-0.4/dl_matrix/structure/mapping/message/content/production/production.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.2/dl_matrix/structure/mapping/message/content/query/query_generator.py` & `dl_matrix-0.4/dl_matrix/structure/mapping/message/content/query/query_generator.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.2/dl_matrix/structure/mapping/message/content/query/query_parser.py` & `dl_matrix-0.4/dl_matrix/structure/mapping/message/content/query/query_parser.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.2/dl_matrix/structure/mapping/message/content/types.py` & `dl_matrix-0.4/dl_matrix/structure/mapping/message/content/types.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.2/dl_matrix/structure/mapping/message/metadata/metadata.py` & `dl_matrix-0.4/dl_matrix/structure/mapping/message/metadata/metadata.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.2/dl_matrix/visualization/app.py` & `dl_matrix-0.4/dl_matrix/visualization/app.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.2/dl_matrix/visualization/psychedelic.py` & `dl_matrix-0.4/dl_matrix/visualization/psychedelic.py`

 * *Files identical despite different names*

### Comparing `dl_matrix-0.2/dl_matrix.egg-info/PKG-INFO` & `dl_matrix-0.4/dl_matrix.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 Metadata-Version: 2.1
 Name: dl-matrix
-Version: 0.2
+Version: 0.4
 Summary: A Divergent Language Matrix package
-Home-page: http://github.com/yourusername/dl_matrix
-Author: Your Name
-Author-email: your.email@example.com
+Home-page: https://github.com/diomandeee/dl_matrix
+Author: Mohamed Diomande
+Author-email: gdiomande7907@gmail.com
 License: MIT
-Keywords: divergent language matrix
-Classifier: Development Status :: 3 - Alpha
+Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Divergent Language Matrix
 
 ## Description
```

### Comparing `dl_matrix-0.2/dl_matrix.egg-info/SOURCES.txt` & `dl_matrix-0.4/dl_matrix.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 LICENSE
+MANIFEST.in
 README.md
+requirements.txt
 setup.py
 dl_matrix/__init__.py
 dl_matrix/builder.py
 dl_matrix/context.py
 dl_matrix/parsers.py
 dl_matrix/relationship.py
 dl_matrix/schema.py
```

### Comparing `dl_matrix-0.2/dl_matrix.egg-info/requires.txt` & `dl_matrix-0.4/dl_matrix.egg-info/requires.txt`

 * *Files identical despite different names*

