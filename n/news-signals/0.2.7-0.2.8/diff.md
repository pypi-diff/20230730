# Comparing `tmp/news-signals-0.2.7.tar.gz` & `tmp/news-signals-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "news-signals-0.2.7.tar", last modified: Tue Jul 11 08:22:31 2023, max compression
+gzip compressed data, was "news-signals-0.2.8.tar", last modified: Sat Jul 29 22:37:17 2023, max compression
```

## Comparing `news-signals-0.2.7.tar` & `news-signals-0.2.8.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:22:31.806055 news-signals-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-11 08:22:21.000000 news-signals-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-11 08:22:21.000000 news-signals-0.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-07-11 08:22:31.806055 news-signals-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-07-11 08:22:21.000000 news-signals-0.2.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-11 08:22:21.000000 news-signals-0.2.7/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:22:31.802055 news-signals-0.2.7/news_signals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 08:22:21.000000 news-signals-0.2.7/news_signals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-11 08:22:21.000000 news-signals-0.2.7/news_signals/anomaly_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-07-11 08:22:21.000000 news-signals-0.2.7/news_signals/aql_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-07-11 08:22:21.000000 news-signals-0.2.7/news_signals/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-11 08:22:21.000000 news-signals-0.2.7/news_signals/dataset_transformations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-07-11 08:22:21.000000 news-signals-0.2.7/news_signals/exogenous_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-11 08:22:21.000000 news-signals-0.2.7/news_signals/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     6333 2023-07-11 08:22:21.000000 news-signals-0.2.7/news_signals/newsapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-07-11 08:22:21.000000 news-signals-0.2.7/news_signals/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-07-11 08:22:21.000000 news-signals-0.2.7/news_signals/representative_story.py
--rw-r--r--   0 runner    (1001) docker     (123)    38571 2023-07-11 08:22:21.000000 news-signals-0.2.7/news_signals/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)    18152 2023-07-11 08:22:21.000000 news-signals-0.2.7/news_signals/signals_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    13060 2023-07-11 08:22:21.000000 news-signals-0.2.7/news_signals/summarization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-07-11 08:22:21.000000 news-signals-0.2.7/news_signals/test_anomaly_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-11 08:22:21.000000 news-signals-0.2.7/news_signals/test_aql_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-11 08:22:21.000000 news-signals-0.2.7/news_signals/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-07-11 08:22:21.000000 news-signals-0.2.7/news_signals/test_dataset_transformations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-11 08:22:21.000000 news-signals-0.2.7/news_signals/test_exogenous_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-07-11 08:22:21.000000 news-signals-0.2.7/news_signals/test_newsapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-11 08:22:21.000000 news-signals-0.2.7/news_signals/test_representative_story.py
--rw-r--r--   0 runner    (1001) docker     (123)    23975 2023-07-11 08:22:21.000000 news-signals-0.2.7/news_signals/test_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11433 2023-07-11 08:22:21.000000 news-signals-0.2.7/news_signals/test_signals_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-07-11 08:22:21.000000 news-signals-0.2.7/news_signals/test_summarization.py
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-07-11 08:22:21.000000 news-signals-0.2.7/news_signals/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-11 08:22:21.000000 news-signals-0.2.7/news_signals/wikidata_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-11 08:22:21.000000 news-signals-0.2.7/news_signals/yfinance_timeseries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:22:31.802055 news-signals-0.2.7/news_signals.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-07-11 08:22:31.000000 news-signals-0.2.7/news_signals.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-07-11 08:22:31.000000 news-signals-0.2.7/news_signals.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 08:22:31.000000 news-signals-0.2.7/news_signals.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-11 08:22:31.000000 news-signals-0.2.7/news_signals.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-11 08:22:31.000000 news-signals-0.2.7/news_signals.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:22:31.798055 news-signals-0.2.7/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:22:31.802055 news-signals-0.2.7/resources/test/
--rw-r--r--   0 runner    (1001) docker     (123)    28512 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/elon_musk_timeseries.json
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/nasdaq100.small.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:22:31.806055 news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDI0NDU0IiwgIm1ldGFkYXRhIjoge319.df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDI0NDU0IiwgIm1ldGFkYXRhIjoge319.static_fields.json
--rw-r--r--   0 runner    (1001) docker     (123)   110293 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDI0NDU0IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDU1MzkwIiwgIm1ldGFkYXRhIjoge319.df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDU1MzkwIiwgIm1ldGFkYXRhIjoge319.static_fields.json
--rw-r--r--   0 runner    (1001) docker     (123)   113236 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDU1MzkwIiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDkyNTcxIiwgIm1ldGFkYXRhIjoge319.df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDkyNTcxIiwgIm1ldGFkYXRhIjoge319.static_fields.json
--rw-r--r--   0 runner    (1001) docker     (123)    90390 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDkyNTcxIiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTQ2MyIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTQ2MyIsICJtZXRhZGF0YSI6IHt9fQ==.static_fields.json
--rw-r--r--   0 runner    (1001) docker     (123)   131955 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTQ2MyIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTU1NjY4IiwgIm1ldGFkYXRhIjoge319.df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTU1NjY4IiwgIm1ldGFkYXRhIjoge319.static_fields.json
--rw-r--r--   0 runner    (1001) docker     (123)   123388 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTU1NjY4IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMzgzNjY5IiwgIm1ldGFkYXRhIjoge319.df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMzgzNjY5IiwgIm1ldGFkYXRhIjoge319.static_fields.json
--rw-r--r--   0 runner    (1001) docker     (123)   109117 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMzgzNjY5IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNDc3MiIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNDc3MiIsICJtZXRhZGF0YSI6IHt9fQ==.static_fields.json
--rw-r--r--   0 runner    (1001) docker     (123)    91683 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNDc3MiIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTEwOTg2NSIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTEwOTg2NSIsICJtZXRhZGF0YSI6IHt9fQ==.static_fields.json
--rw-r--r--   0 runner    (1001) docker     (123)    94002 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTEwOTg2NSIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTQ1MDc2IiwgIm1ldGFkYXRhIjoge319.df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTQ1MDc2IiwgIm1ldGFkYXRhIjoge319.static_fields.json
--rw-r--r--   0 runner    (1001) docker     (123)   100871 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTQ1MDc2IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNzA4MTYxMiIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNzA4MTYxMiIsICJtZXRhZGF0YSI6IHt9fQ==.static_fields.json
--rw-r--r--   0 runner    (1001) docker     (123)   135305 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNzA4MTYxMiIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)    28298 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/politics_china_australia_timeseries.json
--rw-r--r--   0 runner    (1001) docker     (123)   235658 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/sample_stories.json
--rw-r--r--   0 runner    (1001) docker     (123)   218541 2023-07-11 08:22:21.000000 news-signals-0.2.7/resources/test/tesla_stories.json
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 08:22:31.806055 news-signals-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-11 08:22:21.000000 news-signals-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 22:37:17.289679 news-signals-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-29 22:37:07.000000 news-signals-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-29 22:37:07.000000 news-signals-0.2.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-07-29 22:37:17.289679 news-signals-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-07-29 22:37:07.000000 news-signals-0.2.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-29 22:37:07.000000 news-signals-0.2.8/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 22:37:17.281679 news-signals-0.2.8/news_signals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 22:37:07.000000 news-signals-0.2.8/news_signals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-29 22:37:07.000000 news-signals-0.2.8/news_signals/anomaly_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-07-29 22:37:07.000000 news-signals-0.2.8/news_signals/aql_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-07-29 22:37:07.000000 news-signals-0.2.8/news_signals/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-29 22:37:07.000000 news-signals-0.2.8/news_signals/dataset_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-07-29 22:37:07.000000 news-signals-0.2.8/news_signals/exogenous_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-29 22:37:07.000000 news-signals-0.2.8/news_signals/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6333 2023-07-29 22:37:07.000000 news-signals-0.2.8/news_signals/newsapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-07-29 22:37:07.000000 news-signals-0.2.8/news_signals/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-07-29 22:37:07.000000 news-signals-0.2.8/news_signals/representative_story.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38571 2023-07-29 22:37:07.000000 news-signals-0.2.8/news_signals/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18434 2023-07-29 22:37:07.000000 news-signals-0.2.8/news_signals/signals_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13060 2023-07-29 22:37:07.000000 news-signals-0.2.8/news_signals/summarization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-07-29 22:37:07.000000 news-signals-0.2.8/news_signals/test_anomaly_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-29 22:37:07.000000 news-signals-0.2.8/news_signals/test_aql_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-29 22:37:07.000000 news-signals-0.2.8/news_signals/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-07-29 22:37:07.000000 news-signals-0.2.8/news_signals/test_dataset_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-29 22:37:07.000000 news-signals-0.2.8/news_signals/test_exogenous_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-07-29 22:37:07.000000 news-signals-0.2.8/news_signals/test_newsapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-29 22:37:07.000000 news-signals-0.2.8/news_signals/test_representative_story.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23975 2023-07-29 22:37:07.000000 news-signals-0.2.8/news_signals/test_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-07-29 22:37:07.000000 news-signals-0.2.8/news_signals/test_signals_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-07-29 22:37:07.000000 news-signals-0.2.8/news_signals/test_summarization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-07-29 22:37:07.000000 news-signals-0.2.8/news_signals/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-29 22:37:07.000000 news-signals-0.2.8/news_signals/wikidata_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-29 22:37:07.000000 news-signals-0.2.8/news_signals/yfinance_timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 22:37:17.281679 news-signals-0.2.8/news_signals.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-07-29 22:37:17.000000 news-signals-0.2.8/news_signals.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-07-29 22:37:17.000000 news-signals-0.2.8/news_signals.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 22:37:17.000000 news-signals-0.2.8/news_signals.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-29 22:37:17.000000 news-signals-0.2.8/news_signals.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-29 22:37:17.000000 news-signals-0.2.8/news_signals.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 22:37:17.277679 news-signals-0.2.8/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 22:37:17.285679 news-signals-0.2.8/resources/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    28512 2023-07-29 22:37:07.000000 news-signals-0.2.8/resources/test/elon_musk_timeseries.json
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-29 22:37:07.000000 news-signals-0.2.8/resources/test/nasdaq100.small.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 22:37:17.289679 news-signals-0.2.8/resources/test/nasdaq100_sample_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-29 22:37:07.000000 news-signals-0.2.8/resources/test/nasdaq100_sample_dataset/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-07-29 22:37:07.000000 news-signals-0.2.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDI0NDU0IiwgIm1ldGFkYXRhIjoge319.df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-29 22:37:07.000000 news-signals-0.2.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDI0NDU0IiwgIm1ldGFkYXRhIjoge319.static_fields.json
+-rw-r--r--   0 runner    (1001) docker     (123)   110293 2023-07-29 22:37:07.000000 news-signals-0.2.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDI0NDU0IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-29 22:37:07.000000 news-signals-0.2.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDU1MzkwIiwgIm1ldGFkYXRhIjoge319.df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-29 22:37:07.000000 news-signals-0.2.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDU1MzkwIiwgIm1ldGFkYXRhIjoge319.static_fields.json
+-rw-r--r--   0 runner    (1001) docker     (123)   113236 2023-07-29 22:37:07.000000 news-signals-0.2.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDU1MzkwIiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-07-29 22:37:07.000000 news-signals-0.2.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDkyNTcxIiwgIm1ldGFkYXRhIjoge319.df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-29 22:37:07.000000 news-signals-0.2.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDkyNTcxIiwgIm1ldGFkYXRhIjoge319.static_fields.json
+-rw-r--r--   0 runner    (1001) docker     (123)    90390 2023-07-29 22:37:07.000000 news-signals-0.2.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDkyNTcxIiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-07-29 22:37:07.000000 news-signals-0.2.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTQ2MyIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-29 22:37:07.000000 news-signals-0.2.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTQ2MyIsICJtZXRhZGF0YSI6IHt9fQ==.static_fields.json
+-rw-r--r--   0 runner    (1001) docker     (123)   131955 2023-07-29 22:37:07.000000 news-signals-0.2.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTQ2MyIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-07-29 22:37:07.000000 news-signals-0.2.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTU1NjY4IiwgIm1ldGFkYXRhIjoge319.df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-29 22:37:07.000000 news-signals-0.2.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTU1NjY4IiwgIm1ldGFkYXRhIjoge319.static_fields.json
+-rw-r--r--   0 runner    (1001) docker     (123)   123388 2023-07-29 22:37:07.000000 news-signals-0.2.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTU1NjY4IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-07-29 22:37:07.000000 news-signals-0.2.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMzgzNjY5IiwgIm1ldGFkYXRhIjoge319.df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-29 22:37:07.000000 news-signals-0.2.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMzgzNjY5IiwgIm1ldGFkYXRhIjoge319.static_fields.json
+-rw-r--r--   0 runner    (1001) docker     (123)   109117 2023-07-29 22:37:07.000000 news-signals-0.2.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMzgzNjY5IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-07-29 22:37:07.000000 news-signals-0.2.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNDc3MiIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-29 22:37:07.000000 news-signals-0.2.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNDc3MiIsICJtZXRhZGF0YSI6IHt9fQ==.static_fields.json
+-rw-r--r--   0 runner    (1001) docker     (123)    91683 2023-07-29 22:37:07.000000 news-signals-0.2.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNDc3MiIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-07-29 22:37:07.000000 news-signals-0.2.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTEwOTg2NSIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-29 22:37:07.000000 news-signals-0.2.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTEwOTg2NSIsICJtZXRhZGF0YSI6IHt9fQ==.static_fields.json
+-rw-r--r--   0 runner    (1001) docker     (123)    94002 2023-07-29 22:37:07.000000 news-signals-0.2.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTEwOTg2NSIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-07-29 22:37:07.000000 news-signals-0.2.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTQ1MDc2IiwgIm1ldGFkYXRhIjoge319.df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-29 22:37:07.000000 news-signals-0.2.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTQ1MDc2IiwgIm1ldGFkYXRhIjoge319.static_fields.json
+-rw-r--r--   0 runner    (1001) docker     (123)   100871 2023-07-29 22:37:07.000000 news-signals-0.2.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTQ1MDc2IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-29 22:37:07.000000 news-signals-0.2.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNzA4MTYxMiIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-29 22:37:07.000000 news-signals-0.2.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNzA4MTYxMiIsICJtZXRhZGF0YSI6IHt9fQ==.static_fields.json
+-rw-r--r--   0 runner    (1001) docker     (123)   135305 2023-07-29 22:37:07.000000 news-signals-0.2.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNzA4MTYxMiIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)    28298 2023-07-29 22:37:07.000000 news-signals-0.2.8/resources/test/politics_china_australia_timeseries.json
+-rw-r--r--   0 runner    (1001) docker     (123)   235658 2023-07-29 22:37:07.000000 news-signals-0.2.8/resources/test/sample_stories.json
+-rw-r--r--   0 runner    (1001) docker     (123)   218541 2023-07-29 22:37:07.000000 news-signals-0.2.8/resources/test/tesla_stories.json
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 22:37:17.289679 news-signals-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-29 22:37:07.000000 news-signals-0.2.8/setup.py
```

### Comparing `news-signals-0.2.7/LICENSE` & `news-signals-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.7/PKG-INFO` & `news-signals-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: news-signals
-Version: 0.2.7
+Version: 0.2.8
 Summary: A library for working with text and timeseries data.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # News Signals
 
 ### Example Colab Notebooks
```

### Comparing `news-signals-0.2.7/README.md` & `news-signals-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.7/news_signals/anomaly_detection.py` & `news-signals-0.2.8/news_signals/anomaly_detection.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.7/news_signals/aql_builder.py` & `news-signals-0.2.8/news_signals/aql_builder.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.7/news_signals/data.py` & `news-signals-0.2.8/news_signals/data.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.7/news_signals/dataset_transformations.py` & `news-signals-0.2.8/news_signals/dataset_transformations.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.7/news_signals/exogenous_signals.py` & `news-signals-0.2.8/news_signals/exogenous_signals.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.7/news_signals/newsapi.py` & `news-signals-0.2.8/news_signals/newsapi.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.7/news_signals/plotting.py` & `news-signals-0.2.8/news_signals/plotting.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.7/news_signals/representative_story.py` & `news-signals-0.2.8/news_signals/representative_story.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.7/news_signals/signals.py` & `news-signals-0.2.8/news_signals/signals.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.7/news_signals/signals_dataset.py` & `news-signals-0.2.8/news_signals/signals_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -304,26 +304,35 @@
         "period": period,
         "language": "en",
         "aql": aql,
     })
     return new_params
 
 
-def reduce_aylien_story(s):
-    body = " ".join(s["body"].split()[:MAX_BODY_TOKENS])
+def reduce_aylien_story(
+        s,
+        max_body_tokens=MAX_BODY_TOKENS,
+        additional_fields=None
+    ):
+    if additional_fields is None:
+        additional_fields = []
+    body = " ".join(s["body"].split()[:max_body_tokens])
     smart_cats = extract_aylien_smart_tagger_categories(s)
-    reduced = {
-        "title": s["title"],
-        "body": body,
-        "id": s["id"],
-        "published_at": s["published_at"],
-        "language": s["language"],
-        "url": s["links"]["permalink"],
-        "smart_tagger_categories": smart_cats,
-    }
+    reduced = dict(
+        {
+            "title": s["title"],
+            "body": body,
+            "id": s["id"],
+            "published_at": s["published_at"],
+            "language": s["language"],
+            "url": s["links"]["permalink"],
+            "smart_tagger_categories": smart_cats,
+            "clusters": s["clusters"]
+        }, **{f: s[f] for f in additional_fields}
+    )
     return reduced
 
 
 def extract_aylien_smart_tagger_categories(s):
     category_items = []
     for c in s["categories"]:
         if c["taxonomy"] == "aylien":
```

### Comparing `news-signals-0.2.7/news_signals/summarization.py` & `news-signals-0.2.8/news_signals/summarization.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.7/news_signals/test_anomaly_detection.py` & `news-signals-0.2.8/news_signals/test_anomaly_detection.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.7/news_signals/test_aql_builder.py` & `news-signals-0.2.8/news_signals/test_aql_builder.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.7/news_signals/test_data.py` & `news-signals-0.2.8/news_signals/test_data.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.7/news_signals/test_dataset_transformations.py` & `news-signals-0.2.8/news_signals/test_dataset_transformations.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.7/news_signals/test_exogenous_signals.py` & `news-signals-0.2.8/news_signals/test_exogenous_signals.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.7/news_signals/test_newsapi.py` & `news-signals-0.2.8/news_signals/test_newsapi.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.7/news_signals/test_representative_story.py` & `news-signals-0.2.8/news_signals/test_representative_story.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.7/news_signals/test_signals.py` & `news-signals-0.2.8/news_signals/test_signals.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.7/news_signals/test_signals_dataset.py` & `news-signals-0.2.8/news_signals/test_signals_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -325,7 +325,27 @@
         that write data into the signal's state.
         '''
         dataset = SignalsDataset(self.aylien_signals())
         def anomaly_transform(signal):
             return signal.anomaly_signal()
         dataset.map(anomaly_transform)
         assert all('anomalies' in s.columns for s in dataset.signals.values())
+
+    def test_reduce_aylien_story(self):
+        sample_stories = json.load(open(resources / 'tesla_stories.json'))
+        max_body_tokens = 100
+        for s in sample_stories:
+            reduced_s = signals_dataset.reduce_aylien_story(s, max_body_tokens=max_body_tokens)
+            assert len(s['body'].split()) >= len(reduced_s['body'].split())
+            if len(s['body'].split()) > max_body_tokens:
+                assert len(reduced_s['body'].split()) == max_body_tokens
+        
+        s_without_entities = \
+            signals_dataset.reduce_aylien_story(
+                sample_stories[0]
+            )
+        assert 'entities' not in s_without_entities
+        s_with_entities = \
+            signals_dataset.reduce_aylien_story(
+                sample_stories[0], additional_fields=['entities']
+            )
+        assert 'entities' in s_with_entities
```

### Comparing `news-signals-0.2.7/news_signals/test_summarization.py` & `news-signals-0.2.8/news_signals/test_summarization.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.7/news_signals/users.py` & `news-signals-0.2.8/news_signals/users.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.7/news_signals/wikidata_utils.py` & `news-signals-0.2.8/news_signals/wikidata_utils.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.7/news_signals/yfinance_timeseries.py` & `news-signals-0.2.8/news_signals/yfinance_timeseries.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.7/news_signals.egg-info/PKG-INFO` & `news-signals-0.2.8/news_signals.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: news-signals
-Version: 0.2.7
+Version: 0.2.8
 Summary: A library for working with text and timeseries data.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # News Signals
 
 ### Example Colab Notebooks
```

### Comparing `news-signals-0.2.7/news_signals.egg-info/SOURCES.txt` & `news-signals-0.2.8/news_signals.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.7/resources/test/elon_musk_timeseries.json` & `news-signals-0.2.8/resources/test/elon_musk_timeseries.json`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDI0NDU0IiwgIm1ldGFkYXRhIjoge319.df.parquet` & `news-signals-0.2.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDI0NDU0IiwgIm1ldGFkYXRhIjoge319.df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDI0NDU0IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet` & `news-signals-0.2.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDI0NDU0IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDU1MzkwIiwgIm1ldGFkYXRhIjoge319.df.parquet` & `news-signals-0.2.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDU1MzkwIiwgIm1ldGFkYXRhIjoge319.df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDU1MzkwIiwgIm1ldGFkYXRhIjoge319.stories_df.parquet` & `news-signals-0.2.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDU1MzkwIiwgIm1ldGFkYXRhIjoge319.stories_df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDkyNTcxIiwgIm1ldGFkYXRhIjoge319.df.parquet` & `news-signals-0.2.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDkyNTcxIiwgIm1ldGFkYXRhIjoge319.df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDkyNTcxIiwgIm1ldGFkYXRhIjoge319.stories_df.parquet` & `news-signals-0.2.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDkyNTcxIiwgIm1ldGFkYXRhIjoge319.stories_df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTQ2MyIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet` & `news-signals-0.2.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTQ2MyIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTQ2MyIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet` & `news-signals-0.2.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTQ2MyIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTU1NjY4IiwgIm1ldGFkYXRhIjoge319.df.parquet` & `news-signals-0.2.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTU1NjY4IiwgIm1ldGFkYXRhIjoge319.df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTU1NjY4IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet` & `news-signals-0.2.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTU1NjY4IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMzgzNjY5IiwgIm1ldGFkYXRhIjoge319.df.parquet` & `news-signals-0.2.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMzgzNjY5IiwgIm1ldGFkYXRhIjoge319.df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMzgzNjY5IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet` & `news-signals-0.2.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMzgzNjY5IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNDc3MiIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet` & `news-signals-0.2.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNDc3MiIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNDc3MiIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet` & `news-signals-0.2.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNDc3MiIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTEwOTg2NSIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet` & `news-signals-0.2.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTEwOTg2NSIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTEwOTg2NSIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet` & `news-signals-0.2.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTEwOTg2NSIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTQ1MDc2IiwgIm1ldGFkYXRhIjoge319.df.parquet` & `news-signals-0.2.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTQ1MDc2IiwgIm1ldGFkYXRhIjoge319.df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTQ1MDc2IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet` & `news-signals-0.2.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTQ1MDc2IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNzA4MTYxMiIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet` & `news-signals-0.2.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNzA4MTYxMiIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.7/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNzA4MTYxMiIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet` & `news-signals-0.2.8/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNzA4MTYxMiIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.7/resources/test/politics_china_australia_timeseries.json` & `news-signals-0.2.8/resources/test/politics_china_australia_timeseries.json`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.7/resources/test/sample_stories.json` & `news-signals-0.2.8/resources/test/sample_stories.json`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.7/resources/test/tesla_stories.json` & `news-signals-0.2.8/resources/test/tesla_stories.json`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.7/setup.py` & `news-signals-0.2.8/setup.py`

 * *Files identical despite different names*

