# Comparing `tmp/sneakpeek_py-0.2.1.tar.gz` & `tmp/sneakpeek_py-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sneakpeek_py-0.2.1.tar", max compression
+gzip compressed data, was "sneakpeek_py-0.2.2.tar", max compression
```

## Comparing `sneakpeek_py-0.2.1.tar` & `sneakpeek_py-0.2.2.tar`

### file list

```diff
@@ -1,45 +1,246 @@
--rw-r--r--   0        0        0     7605 2023-07-30 12:54:50.973317 sneakpeek_py-0.2.1/README.md
--rw-r--r--   0        0        0     2279 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     7556 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/sneakpeek/api.py
--rw-r--r--   0        0        0     2513 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/sneakpeek/logging.py
--rw-r--r--   0        0        0     5028 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/sneakpeek/metrics.py
--rw-r--r--   0        0        0     1289 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/sneakpeek/middleware/base.py
--rw-r--r--   0        0        0     1141 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/sneakpeek/middleware/parser.py
--rw-r--r--   0        0        0     1627 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/sneakpeek/middleware/proxy_middleware.py
--rw-r--r--   0        0        0     5015 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/sneakpeek/middleware/rate_limiter_middleware.py
--rw-r--r--   0        0        0     2301 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/sneakpeek/middleware/requests_logging_middleware.py
--rw-r--r--   0        0        0     4187 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/sneakpeek/middleware/robots_txt_middleware.py
--rw-r--r--   0        0        0     1822 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/sneakpeek/middleware/user_agent_injecter_middleware.py
--rw-r--r--   0        0        0     5157 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/sneakpeek/queue/consumer.py
--rw-r--r--   0        0        0     3510 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/sneakpeek/queue/in_memory_storage.py
--rw-r--r--   0        0        0     7678 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/sneakpeek/queue/model.py
--rw-r--r--   0        0        0     4132 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/sneakpeek/queue/queue.py
--rw-r--r--   0        0        0     5065 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/sneakpeek/queue/redis_storage.py
--rw-r--r--   0        0        0     1765 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/sneakpeek/queue/tasks.py
--rw-r--r--   0        0        0     4257 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/sneakpeek/queue/tests/test_consumer.py
--rw-r--r--   0        0        0     4318 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/sneakpeek/queue/tests/test_queue.py
--rw-r--r--   0        0        0     2920 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/sneakpeek/queue/tests/test_queue_storage.py
--rw-r--r--   0        0        0     1829 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/sneakpeek/scheduler/in_memory_lease_storage.py
--rw-r--r--   0        0        0     4285 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/sneakpeek/scheduler/model.py
--rw-r--r--   0        0        0     1676 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/sneakpeek/scheduler/redis_lease_storage.py
--rw-r--r--   0        0        0     8923 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/sneakpeek/scheduler/scheduler.py
--rw-r--r--   0        0        0     1867 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/sneakpeek/scheduler/tests/test_lease_storage.py
--rw-r--r--   0        0        0     7941 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/sneakpeek/scraper/context.py
--rw-r--r--   0        0        0     1889 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/sneakpeek/scraper/dynamic_scraper_handler.py
--rw-r--r--   0        0        0     1398 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/sneakpeek/scraper/ephemeral_scraper_task_handler.py
--rw-r--r--   0        0        0     2484 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/sneakpeek/scraper/in_memory_storage.py
--rw-r--r--   0        0        0    18460 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/sneakpeek/scraper/model.py
--rw-r--r--   0        0        0     2720 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/sneakpeek/scraper/redis_storage.py
--rw-r--r--   0        0        0     4129 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/sneakpeek/scraper/runner.py
--rw-r--r--   0        0        0     1193 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/sneakpeek/scraper/task_handler.py
--rw-r--r--   0        0        0    12021 2023-07-30 12:54:50.985317 sneakpeek_py-0.2.1/sneakpeek/scraper/tests/test_context.py
--rw-r--r--   0        0        0     3239 2023-07-30 12:54:50.985317 sneakpeek_py-0.2.1/sneakpeek/scraper/tests/test_dynamic_scraper_handler.py
--rw-r--r--   0        0        0     3673 2023-07-30 12:54:50.985317 sneakpeek_py-0.2.1/sneakpeek/scraper/tests/test_scraper_storage.py
--rw-r--r--   0        0        0     8576 2023-07-30 12:54:50.985317 sneakpeek_py-0.2.1/sneakpeek/server.py
--rw-r--r--   0        0        0      851 2023-07-30 12:54:50.985317 sneakpeek_py-0.2.1/sneakpeek/session_loggers/base.py
--rw-r--r--   0        0        0     3728 2023-07-30 12:54:50.985317 sneakpeek_py-0.2.1/sneakpeek/session_loggers/file_logger.py
--rw-r--r--   0        0        0     1844 2023-07-30 12:54:50.985317 sneakpeek_py-0.2.1/sneakpeek/session_loggers/redis_logger.py
--rw-r--r--   0        0        0        0 2023-07-30 12:54:50.985317 sneakpeek_py-0.2.1/sneakpeek/static/.gitkeep
--rw-r--r--   0        0        0    11392 2023-07-30 12:54:50.985317 sneakpeek_py-0.2.1/sneakpeek/tests/test_integration.py
--rw-r--r--   0        0        0     4063 2023-07-30 12:54:50.985317 sneakpeek_py-0.2.1/sneakpeek/tests/test_metrics.py
--rw-r--r--   0        0        0     9749 1970-01-01 00:00:00.000000 sneakpeek_py-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     7605 2023-07-30 13:18:53.789283 sneakpeek_py-0.2.2/README.md
+-rw-r--r--   0        0        0     2279 2023-07-30 13:18:53.797283 sneakpeek_py-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     7556 2023-07-30 13:18:53.797283 sneakpeek_py-0.2.2/sneakpeek/api.py
+-rw-r--r--   0        0        0     2513 2023-07-30 13:18:53.797283 sneakpeek_py-0.2.2/sneakpeek/logging.py
+-rw-r--r--   0        0        0     5028 2023-07-30 13:18:53.797283 sneakpeek_py-0.2.2/sneakpeek/metrics.py
+-rw-r--r--   0        0        0     1289 2023-07-30 13:18:53.797283 sneakpeek_py-0.2.2/sneakpeek/middleware/base.py
+-rw-r--r--   0        0        0     1141 2023-07-30 13:18:53.797283 sneakpeek_py-0.2.2/sneakpeek/middleware/parser.py
+-rw-r--r--   0        0        0     1627 2023-07-30 13:18:53.797283 sneakpeek_py-0.2.2/sneakpeek/middleware/proxy_middleware.py
+-rw-r--r--   0        0        0     5015 2023-07-30 13:18:53.797283 sneakpeek_py-0.2.2/sneakpeek/middleware/rate_limiter_middleware.py
+-rw-r--r--   0        0        0     2301 2023-07-30 13:18:53.797283 sneakpeek_py-0.2.2/sneakpeek/middleware/requests_logging_middleware.py
+-rw-r--r--   0        0        0     4187 2023-07-30 13:18:53.797283 sneakpeek_py-0.2.2/sneakpeek/middleware/robots_txt_middleware.py
+-rw-r--r--   0        0        0     1822 2023-07-30 13:18:53.797283 sneakpeek_py-0.2.2/sneakpeek/middleware/user_agent_injecter_middleware.py
+-rw-r--r--   0        0        0     5157 2023-07-30 13:18:53.797283 sneakpeek_py-0.2.2/sneakpeek/queue/consumer.py
+-rw-r--r--   0        0        0     3510 2023-07-30 13:18:53.797283 sneakpeek_py-0.2.2/sneakpeek/queue/in_memory_storage.py
+-rw-r--r--   0        0        0     7678 2023-07-30 13:18:53.797283 sneakpeek_py-0.2.2/sneakpeek/queue/model.py
+-rw-r--r--   0        0        0     4132 2023-07-30 13:18:53.797283 sneakpeek_py-0.2.2/sneakpeek/queue/queue.py
+-rw-r--r--   0        0        0     5065 2023-07-30 13:18:53.797283 sneakpeek_py-0.2.2/sneakpeek/queue/redis_storage.py
+-rw-r--r--   0        0        0     1765 2023-07-30 13:18:53.797283 sneakpeek_py-0.2.2/sneakpeek/queue/tasks.py
+-rw-r--r--   0        0        0     4257 2023-07-30 13:18:53.797283 sneakpeek_py-0.2.2/sneakpeek/queue/tests/test_consumer.py
+-rw-r--r--   0        0        0     4318 2023-07-30 13:18:53.797283 sneakpeek_py-0.2.2/sneakpeek/queue/tests/test_queue.py
+-rw-r--r--   0        0        0     2920 2023-07-30 13:18:53.797283 sneakpeek_py-0.2.2/sneakpeek/queue/tests/test_queue_storage.py
+-rw-r--r--   0        0        0     1829 2023-07-30 13:18:53.797283 sneakpeek_py-0.2.2/sneakpeek/scheduler/in_memory_lease_storage.py
+-rw-r--r--   0        0        0     4285 2023-07-30 13:18:53.797283 sneakpeek_py-0.2.2/sneakpeek/scheduler/model.py
+-rw-r--r--   0        0        0     1676 2023-07-30 13:18:53.797283 sneakpeek_py-0.2.2/sneakpeek/scheduler/redis_lease_storage.py
+-rw-r--r--   0        0        0     8923 2023-07-30 13:18:53.797283 sneakpeek_py-0.2.2/sneakpeek/scheduler/scheduler.py
+-rw-r--r--   0        0        0     1867 2023-07-30 13:18:53.797283 sneakpeek_py-0.2.2/sneakpeek/scheduler/tests/test_lease_storage.py
+-rw-r--r--   0        0        0     7941 2023-07-30 13:18:53.797283 sneakpeek_py-0.2.2/sneakpeek/scraper/context.py
+-rw-r--r--   0        0        0     1889 2023-07-30 13:18:53.797283 sneakpeek_py-0.2.2/sneakpeek/scraper/dynamic_scraper_handler.py
+-rw-r--r--   0        0        0     1398 2023-07-30 13:18:53.797283 sneakpeek_py-0.2.2/sneakpeek/scraper/ephemeral_scraper_task_handler.py
+-rw-r--r--   0        0        0     2484 2023-07-30 13:18:53.797283 sneakpeek_py-0.2.2/sneakpeek/scraper/in_memory_storage.py
+-rw-r--r--   0        0        0    18460 2023-07-30 13:18:53.797283 sneakpeek_py-0.2.2/sneakpeek/scraper/model.py
+-rw-r--r--   0        0        0     2720 2023-07-30 13:18:53.797283 sneakpeek_py-0.2.2/sneakpeek/scraper/redis_storage.py
+-rw-r--r--   0        0        0     4129 2023-07-30 13:18:53.797283 sneakpeek_py-0.2.2/sneakpeek/scraper/runner.py
+-rw-r--r--   0        0        0     1193 2023-07-30 13:18:53.797283 sneakpeek_py-0.2.2/sneakpeek/scraper/task_handler.py
+-rw-r--r--   0        0        0    12021 2023-07-30 13:18:53.797283 sneakpeek_py-0.2.2/sneakpeek/scraper/tests/test_context.py
+-rw-r--r--   0        0        0     3239 2023-07-30 13:18:53.797283 sneakpeek_py-0.2.2/sneakpeek/scraper/tests/test_dynamic_scraper_handler.py
+-rw-r--r--   0        0        0     3673 2023-07-30 13:18:53.797283 sneakpeek_py-0.2.2/sneakpeek/scraper/tests/test_scraper_storage.py
+-rw-r--r--   0        0        0     8576 2023-07-30 13:18:53.797283 sneakpeek_py-0.2.2/sneakpeek/server.py
+-rw-r--r--   0        0        0      851 2023-07-30 13:18:53.797283 sneakpeek_py-0.2.2/sneakpeek/session_loggers/base.py
+-rw-r--r--   0        0        0     3728 2023-07-30 13:18:53.797283 sneakpeek_py-0.2.2/sneakpeek/session_loggers/file_logger.py
+-rw-r--r--   0        0        0     1844 2023-07-30 13:18:53.797283 sneakpeek_py-0.2.2/sneakpeek/session_loggers/redis_logger.py
+-rw-r--r--   0        0        0        0 2023-07-30 13:18:53.797283 sneakpeek_py-0.2.2/sneakpeek/static/.gitkeep
+-rw-r--r--   0        0        0      230 2023-07-30 13:21:14.576128 sneakpeek_py-0.2.2/sneakpeek/static/docs/.buildinfo
+-rw-r--r--   0        0        0  1149879 2023-07-30 13:21:13.344102 sneakpeek_py-0.2.2/sneakpeek/static/docs/.doctrees/api.doctree
+-rw-r--r--   0        0        0     8116 2023-07-30 13:21:13.428104 sneakpeek_py-0.2.2/sneakpeek/static/docs/.doctrees/deployment.doctree
+-rw-r--r--   0        0        0    26294 2023-07-30 13:21:13.456105 sneakpeek_py-0.2.2/sneakpeek/static/docs/.doctrees/design.doctree
+-rw-r--r--   0        0        0    83697 2023-07-30 13:21:13.532106 sneakpeek_py-0.2.2/sneakpeek/static/docs/.doctrees/environment.pickle
+-rw-r--r--   0        0        0     5431 2023-07-30 13:21:13.460105 sneakpeek_py-0.2.2/sneakpeek/static/docs/.doctrees/index.doctree
+-rw-r--r--   0        0        0     7911 2023-07-30 13:21:13.472105 sneakpeek_py-0.2.2/sneakpeek/static/docs/.doctrees/local_debugging.doctree
+-rw-r--r--   0        0        0     3883 2023-07-30 13:21:13.476105 sneakpeek_py-0.2.2/sneakpeek/static/docs/.doctrees/middleware/index.doctree
+-rw-r--r--   0        0        0    18586 2023-07-30 13:21:13.488105 sneakpeek_py-0.2.2/sneakpeek/static/docs/.doctrees/middleware/new_middleware.doctree
+-rw-r--r--   0        0        0     6422 2023-07-30 13:21:13.496106 sneakpeek_py-0.2.2/sneakpeek/static/docs/.doctrees/middleware/proxy_middleware.doctree
+-rw-r--r--   0        0        0     8397 2023-07-30 13:21:13.500106 sneakpeek_py-0.2.2/sneakpeek/static/docs/.doctrees/middleware/rate_limiter_middleware.doctree
+-rw-r--r--   0        0        0     6394 2023-07-30 13:21:13.508106 sneakpeek_py-0.2.2/sneakpeek/static/docs/.doctrees/middleware/requests_logging_middleware.doctree
+-rw-r--r--   0        0        0     6422 2023-07-30 13:21:13.512106 sneakpeek_py-0.2.2/sneakpeek/static/docs/.doctrees/middleware/robots_txt_middleware.doctree
+-rw-r--r--   0        0        0     7440 2023-07-30 13:21:13.520106 sneakpeek_py-0.2.2/sneakpeek/static/docs/.doctrees/middleware/user_agent_injecter_middleware.doctree
+-rw-r--r--   0        0        0    13317 2023-07-30 13:21:13.528106 sneakpeek_py-0.2.2/sneakpeek/static/docs/.doctrees/quick_start.doctree
+-rw-r--r--   0        0        0     1347 2023-07-30 13:18:53.789283 sneakpeek_py-0.2.2/sneakpeek/static/docs/_sources/api.rst.txt
+-rw-r--r--   0        0        0     1335 2023-07-30 13:18:53.789283 sneakpeek_py-0.2.2/sneakpeek/static/docs/_sources/deployment.rst.txt
+-rw-r--r--   0        0        0     3757 2023-07-30 13:18:53.789283 sneakpeek_py-0.2.2/sneakpeek/static/docs/_sources/design.rst.txt
+-rw-r--r--   0        0        0      499 2023-07-30 13:18:53.789283 sneakpeek_py-0.2.2/sneakpeek/static/docs/_sources/index.rst.txt
+-rw-r--r--   0        0        0     1409 2023-07-30 13:18:53.789283 sneakpeek_py-0.2.2/sneakpeek/static/docs/_sources/local_debugging.rst.txt
+-rw-r--r--   0        0        0      484 2023-07-30 13:18:53.789283 sneakpeek_py-0.2.2/sneakpeek/static/docs/_sources/middleware/index.rst.txt
+-rw-r--r--   0        0        0     5760 2023-07-30 13:18:53.789283 sneakpeek_py-0.2.2/sneakpeek/static/docs/_sources/middleware/new_middleware.rst.txt
+-rw-r--r--   0        0        0     1468 2023-07-30 13:18:53.789283 sneakpeek_py-0.2.2/sneakpeek/static/docs/_sources/middleware/proxy_middleware.rst.txt
+-rw-r--r--   0        0        0     2124 2023-07-30 13:18:53.789283 sneakpeek_py-0.2.2/sneakpeek/static/docs/_sources/middleware/rate_limiter_middleware.rst.txt
+-rw-r--r--   0        0        0     1409 2023-07-30 13:18:53.789283 sneakpeek_py-0.2.2/sneakpeek/static/docs/_sources/middleware/requests_logging_middleware.rst.txt
+-rw-r--r--   0        0        0     1442 2023-07-30 13:18:53.789283 sneakpeek_py-0.2.2/sneakpeek/static/docs/_sources/middleware/robots_txt_middleware.rst.txt
+-rw-r--r--   0        0        0     1582 2023-07-30 13:18:53.789283 sneakpeek_py-0.2.2/sneakpeek/static/docs/_sources/middleware/user_agent_injecter_middleware.rst.txt
+-rw-r--r--   0        0        0     5188 2023-07-30 13:18:53.789283 sneakpeek_py-0.2.2/sneakpeek/static/docs/_sources/quick_start.rst.txt
+-rw-r--r--   0        0        0    14638 2023-07-30 13:21:14.564128 sneakpeek_py-0.2.2/sneakpeek/static/docs/_static/basic.css
+-rw-r--r--   0        0        0     3275 2023-07-30 13:19:21.757835 sneakpeek_py-0.2.2/sneakpeek/static/docs/_static/css/badge_only.css
+-rw-r--r--   0        0        0    87624 2023-07-30 13:19:21.757835 sneakpeek_py-0.2.2/sneakpeek/static/docs/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-r--r--   0        0        0    67312 2023-07-30 13:19:21.757835 sneakpeek_py-0.2.2/sneakpeek/static/docs/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-r--r--   0        0        0    86288 2023-07-30 13:19:21.757835 sneakpeek_py-0.2.2/sneakpeek/static/docs/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-r--r--   0        0        0    66444 2023-07-30 13:19:21.761835 sneakpeek_py-0.2.2/sneakpeek/static/docs/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-r--r--   0        0        0   165742 2023-07-30 13:19:21.761835 sneakpeek_py-0.2.2/sneakpeek/static/docs/_static/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0        0        0   444379 2023-07-30 13:19:21.765835 sneakpeek_py-0.2.2/sneakpeek/static/docs/_static/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0        0        0   165548 2023-07-30 13:19:21.769835 sneakpeek_py-0.2.2/sneakpeek/static/docs/_static/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0        0        0    98024 2023-07-30 13:19:21.769835 sneakpeek_py-0.2.2/sneakpeek/static/docs/_static/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0        0        0    77160 2023-07-30 13:19:21.769835 sneakpeek_py-0.2.2/sneakpeek/static/docs/_static/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0        0        0   323344 2023-07-30 13:19:21.769835 sneakpeek_py-0.2.2/sneakpeek/static/docs/_static/css/fonts/lato-bold-italic.woff
+-rw-r--r--   0        0        0   193308 2023-07-30 13:19:21.773835 sneakpeek_py-0.2.2/sneakpeek/static/docs/_static/css/fonts/lato-bold-italic.woff2
+-rw-r--r--   0        0        0   309728 2023-07-30 13:19:21.773835 sneakpeek_py-0.2.2/sneakpeek/static/docs/_static/css/fonts/lato-bold.woff
+-rw-r--r--   0        0        0   184912 2023-07-30 13:19:21.777835 sneakpeek_py-0.2.2/sneakpeek/static/docs/_static/css/fonts/lato-bold.woff2
+-rw-r--r--   0        0        0   328412 2023-07-30 13:19:21.777835 sneakpeek_py-0.2.2/sneakpeek/static/docs/_static/css/fonts/lato-normal-italic.woff
+-rw-r--r--   0        0        0   195704 2023-07-30 13:19:21.781835 sneakpeek_py-0.2.2/sneakpeek/static/docs/_static/css/fonts/lato-normal-italic.woff2
+-rw-r--r--   0        0        0   309192 2023-07-30 13:19:21.781835 sneakpeek_py-0.2.2/sneakpeek/static/docs/_static/css/fonts/lato-normal.woff
+-rw-r--r--   0        0        0   182708 2023-07-30 13:19:21.785835 sneakpeek_py-0.2.2/sneakpeek/static/docs/_static/css/fonts/lato-normal.woff2
+-rw-r--r--   0        0        0   129674 2023-07-30 13:19:21.757835 sneakpeek_py-0.2.2/sneakpeek/static/docs/_static/css/theme.css
+-rw-r--r--   0        0        0     9630 2023-07-30 13:19:21.257825 sneakpeek_py-0.2.2/sneakpeek/static/docs/_static/doctools.js
+-rw-r--r--   0        0        0      353 2023-07-30 13:21:14.568128 sneakpeek_py-0.2.2/sneakpeek/static/docs/_static/documentation_options.js
+-rw-r--r--   0        0        0      286 2023-07-30 13:19:21.257825 sneakpeek_py-0.2.2/sneakpeek/static/docs/_static/file.png
+-rw-r--r--   0        0        0   287630 2023-07-30 13:19:21.261825 sneakpeek_py-0.2.2/sneakpeek/static/docs/_static/jquery-3.5.1.js
+-rw-r--r--   0        0        0    89476 2023-07-30 13:19:21.261825 sneakpeek_py-0.2.2/sneakpeek/static/docs/_static/jquery.js
+-rw-r--r--   0        0        0      934 2023-07-30 13:19:21.785835 sneakpeek_py-0.2.2/sneakpeek/static/docs/_static/js/badge_only.js
+-rw-r--r--   0        0        0     4370 2023-07-30 13:19:21.785835 sneakpeek_py-0.2.2/sneakpeek/static/docs/_static/js/html5shiv-printshiv.min.js
+-rw-r--r--   0        0        0     2734 2023-07-30 13:19:21.785835 sneakpeek_py-0.2.2/sneakpeek/static/docs/_static/js/html5shiv.min.js
+-rw-r--r--   0        0        0     5023 2023-07-30 13:19:21.785835 sneakpeek_py-0.2.2/sneakpeek/static/docs/_static/js/theme.js
+-rw-r--r--   0        0        0    10854 2023-07-30 13:21:14.564128 sneakpeek_py-0.2.2/sneakpeek/static/docs/_static/language_data.js
+-rw-r--r--   0        0        0       90 2023-07-30 13:19:21.261825 sneakpeek_py-0.2.2/sneakpeek/static/docs/_static/minus.png
+-rw-r--r--   0        0        0       90 2023-07-30 13:19:21.261825 sneakpeek_py-0.2.2/sneakpeek/static/docs/_static/plus.png
+-rw-r--r--   0        0        0     4846 2023-07-30 13:21:14.560128 sneakpeek_py-0.2.2/sneakpeek/static/docs/_static/pygments.css
+-rw-r--r--   0        0        0    16733 2023-07-30 13:19:21.261825 sneakpeek_py-0.2.2/sneakpeek/static/docs/_static/searchtools.js
+-rw-r--r--   0        0        0    68420 2023-07-30 13:19:21.261825 sneakpeek_py-0.2.2/sneakpeek/static/docs/_static/underscore-1.13.1.js
+-rw-r--r--   0        0        0    19530 2023-07-30 13:19:21.261825 sneakpeek_py-0.2.2/sneakpeek/static/docs/_static/underscore.js
+-rw-r--r--   0        0        0   338884 2023-07-30 13:21:14.224120 sneakpeek_py-0.2.2/sneakpeek/static/docs/api.html
+-rw-r--r--   0        0        0     7617 2023-07-30 13:21:14.244121 sneakpeek_py-0.2.2/sneakpeek/static/docs/deployment.html
+-rw-r--r--   0        0        0    14281 2023-07-30 13:21:14.268122 sneakpeek_py-0.2.2/sneakpeek/static/docs/design.html
+-rw-r--r--   0        0        0    51601 2023-07-30 13:21:14.532127 sneakpeek_py-0.2.2/sneakpeek/static/docs/genindex.html
+-rw-r--r--   0        0        0     8868 2023-07-30 13:21:14.288122 sneakpeek_py-0.2.2/sneakpeek/static/docs/index.html
+-rw-r--r--   0        0        0     9210 2023-07-30 13:21:14.320123 sneakpeek_py-0.2.2/sneakpeek/static/docs/local_debugging.html
+-rw-r--r--   0        0        0     7050 2023-07-30 13:21:14.340123 sneakpeek_py-0.2.2/sneakpeek/static/docs/middleware/index.html
+-rw-r--r--   0        0        0    23461 2023-07-30 13:21:14.368124 sneakpeek_py-0.2.2/sneakpeek/static/docs/middleware/new_middleware.html
+-rw-r--r--   0        0        0    10012 2023-07-30 13:21:14.392124 sneakpeek_py-0.2.2/sneakpeek/static/docs/middleware/proxy_middleware.html
+-rw-r--r--   0        0        0    10511 2023-07-30 13:21:14.412124 sneakpeek_py-0.2.2/sneakpeek/static/docs/middleware/rate_limiter_middleware.html
+-rw-r--r--   0        0        0     9352 2023-07-30 13:21:14.436125 sneakpeek_py-0.2.2/sneakpeek/static/docs/middleware/requests_logging_middleware.html
+-rw-r--r--   0        0        0     9329 2023-07-30 13:21:14.456125 sneakpeek_py-0.2.2/sneakpeek/static/docs/middleware/robots_txt_middleware.html
+-rw-r--r--   0        0        0     9766 2023-07-30 13:21:14.476126 sneakpeek_py-0.2.2/sneakpeek/static/docs/middleware/user_agent_injecter_middleware.html
+-rw-r--r--   0        0        0     2278 2023-07-30 13:21:14.584128 sneakpeek_py-0.2.2/sneakpeek/static/docs/objects.inv
+-rw-r--r--   0        0        0    11898 2023-07-30 13:21:14.548127 sneakpeek_py-0.2.2/sneakpeek/static/docs/py-modindex.html
+-rw-r--r--   0        0        0    19854 2023-07-30 13:21:14.504126 sneakpeek_py-0.2.2/sneakpeek/static/docs/quick_start.html
+-rw-r--r--   0        0        0     5319 2023-07-30 13:21:14.560128 sneakpeek_py-0.2.2/sneakpeek/static/docs/search.html
+-rw-r--r--   0        0        0    21941 2023-07-30 13:21:14.580128 sneakpeek_py-0.2.2/sneakpeek/static/docs/searchindex.js
+-rw-r--r--   0        0        0      543 2023-07-30 13:21:07.115930 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/ErrorNotFound.87a119f7.js
+-rw-r--r--   0        0        0    20436 2023-07-30 13:21:07.103930 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/KFOkCnqEu92Fr1MmgVxIIzQ.34e9582c.woff
+-rw-r--r--   0        0        0    20544 2023-07-30 13:21:07.103930 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/KFOlCnqEu92Fr1MmEU9fBBc-.9ce7f3ac.woff
+-rw-r--r--   0        0        0    20416 2023-07-30 13:21:07.103930 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/KFOlCnqEu92Fr1MmSU5fBBc-.bf14c7d7.woff
+-rw-r--r--   0        0        0    20408 2023-07-30 13:21:07.103930 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/KFOlCnqEu92Fr1MmWUlfBBc-.e0fd57c0.woff
+-rw-r--r--   0        0        0    20424 2023-07-30 13:21:07.103930 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/KFOlCnqEu92Fr1MmYUtfBBc-.f6537e32.woff
+-rw-r--r--   0        0        0    20344 2023-07-30 13:21:07.103930 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/KFOmCnqEu92Fr1Mu4mxM.f2abf7fb.woff
+-rw-r--r--   0        0        0    25344 2023-07-30 13:21:07.103930 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/MainLayout.a4d84445.js
+-rw-r--r--   0        0        0      613 2023-07-30 13:21:07.111930 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/NewScraperPage.c2aa97e0.js
+-rw-r--r--   0        0        0    30695 2023-07-30 13:21:07.111930 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/PriorityChip.ad4f92a5.js
+-rw-r--r--   0        0        0      655 2023-07-30 13:21:07.111930 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/QList.1548b7b0.js
+-rw-r--r--   0        0        0    76693 2023-07-30 13:21:07.111930 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/QPage.1ebdd4ad.js
+-rw-r--r--   0        0        0     1017 2023-07-30 13:21:07.103930 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/QSeparator.f3fa0e56.js
+-rw-r--r--   0        0        0  1331992 2023-07-30 13:21:07.115930 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/ScraperEditForm.21a534e7.js
+-rw-r--r--   0        0        0     3323 2023-07-30 13:21:07.123931 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/ScraperEditForm.640de0df.css
+-rw-r--r--   0        0        0       30 2023-07-30 13:21:07.123931 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/ScraperIde.bda1b48a.css
+-rw-r--r--   0        0        0     3692 2023-07-30 13:21:07.115930 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/ScraperIde.c338b8e5.js
+-rw-r--r--   0        0        0    78707 2023-07-30 13:21:07.123931 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/ScraperIdeComponent.1d43085e.css
+-rw-r--r--   0        0        0  2684689 2023-07-30 13:21:07.115930 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/ScraperIdeComponent.c3392f54.js
+-rw-r--r--   0        0        0      137 2023-07-30 13:21:07.123931 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/ScraperPage.05e412dc.css
+-rw-r--r--   0        0        0    21663 2023-07-30 13:21:07.115930 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/ScraperPage.1300606c.js
+-rw-r--r--   0        0        0     2872 2023-07-30 13:21:07.111930 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/ScrapersPage.70e8bdd3.js
+-rw-r--r--   0        0        0    14409 2023-07-30 13:21:07.115930 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/abap.6ba285e6.js
+-rw-r--r--   0        0        0     4198 2023-07-30 13:21:07.115930 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/apex.4a5ec4a4.js
+-rw-r--r--   0        0        0    10882 2023-07-30 13:21:07.103930 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/api.7efe3d3e.js
+-rw-r--r--   0        0        0     1094 2023-07-30 13:21:07.115930 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/azcli.4c9b6b47.js
+-rw-r--r--   0        0        0     2091 2023-07-30 13:21:07.115930 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/bat.8a420ace.js
+-rw-r--r--   0        0        0     2782 2023-07-30 13:21:07.115930 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/bicep.5032e09b.js
+-rw-r--r--   0        0        0     2431 2023-07-30 13:21:07.115930 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/cameligo.00bc63f8.js
+-rw-r--r--   0        0        0     9889 2023-07-30 13:21:07.115930 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/clojure.bc79377e.js
+-rw-r--r--   0        0        0    70776 2023-07-30 13:21:07.103930 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/codicon.c99115f8.ttf
+-rw-r--r--   0        0        0     3836 2023-07-30 13:21:07.115930 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/coffee.54897858.js
+-rw-r--r--   0        0        0     5694 2023-07-30 13:21:07.115930 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/cpp.337468ce.js
+-rw-r--r--   0        0        0     4770 2023-07-30 13:21:07.115930 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/csharp.01a8eaa8.js
+-rw-r--r--   0        0        0     1665 2023-07-30 13:21:07.115930 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/csp.aec2811b.js
+-rw-r--r--   0        0        0     4753 2023-07-30 13:21:07.115930 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/css.4c22ed20.js
+-rw-r--r--   0        0        0    33579 2023-07-30 13:21:07.123931 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/cssMode.bdc5c723.js
+-rw-r--r--   0        0        0     4496 2023-07-30 13:21:07.115930 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/dart.50deccbd.js
+-rw-r--r--   0        0        0     2115 2023-07-30 13:21:07.115930 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/dockerfile.de6a0f2c.js
+-rw-r--r--   0        0        0     5588 2023-07-30 13:21:07.115930 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/ecl.19ccc34b.js
+-rw-r--r--   0        0        0    10005 2023-07-30 13:21:07.115930 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/elixir.a6460ae7.js
+-rw-r--r--   0        0        0   187208 2023-07-30 13:21:07.103930 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/fa-brands-400.20c4a58b.ttf
+-rw-r--r--   0        0        0   108020 2023-07-30 13:21:07.099930 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/fa-brands-400.74833209.woff2
+-rw-r--r--   0        0        0    63952 2023-07-30 13:21:07.103930 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/fa-regular-400.528d022d.ttf
+-rw-r--r--   0        0        0    24948 2023-07-30 13:21:07.103930 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/fa-regular-400.8e7e5ea1.woff2
+-rw-r--r--   0        0        0   394628 2023-07-30 13:21:07.103930 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/fa-solid-900.67a65763.ttf
+-rw-r--r--   0        0        0   150124 2023-07-30 13:21:07.103930 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/fa-solid-900.7152a693.woff2
+-rw-r--r--   0        0        0    10172 2023-07-30 13:21:07.103930 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/fa-v4compatibility.0515a423.ttf
+-rw-r--r--   0        0        0     4564 2023-07-30 13:21:07.103930 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/fa-v4compatibility.694a17c3.woff2
+-rw-r--r--   0        0        0   164912 2023-07-30 13:21:07.103930 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.fd84f88b.woff
+-rw-r--r--   0        0        0   128616 2023-07-30 13:21:07.103930 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.4a4dbc62.woff2
+-rw-r--r--   0        0        0     2056 2023-07-30 13:21:07.115930 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/flow9.c44e3f2e.js
+-rw-r--r--   0        0        0    16431 2023-07-30 13:21:07.115930 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/freemarker2.f2feddff.js
+-rw-r--r--   0        0        0     3229 2023-07-30 13:21:07.115930 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/fsharp.d9204eef.js
+-rw-r--r--   0        0        0     2903 2023-07-30 13:21:07.115930 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/go.1e1292ae.js
+-rw-r--r--   0        0        0     2506 2023-07-30 13:21:07.115930 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/graphql.900d9927.js
+-rw-r--r--   0        0        0     7109 2023-07-30 13:21:07.115930 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/handlebars.e6e016d9.js
+-rw-r--r--   0        0        0     3836 2023-07-30 13:21:07.115930 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/hcl.c0959a07.js
+-rw-r--r--   0        0        0     5173 2023-07-30 13:21:07.115930 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/html.bb3a0ac5.js
+-rw-r--r--   0        0        0    34338 2023-07-30 13:21:07.123931 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/htmlMode.1a8f1e45.js
+-rw-r--r--   0        0        0   307193 2023-07-30 13:21:07.123931 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/index.91e4ba5b.css
+-rw-r--r--   0        0        0   133829 2023-07-30 13:21:07.103930 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/index.f9c30c55.js
+-rw-r--r--   0        0        0     1347 2023-07-30 13:21:07.115930 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/ini.75848fa5.js
+-rw-r--r--   0        0        0     3467 2023-07-30 13:21:07.115930 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/java.13c44e5c.js
+-rw-r--r--   0        0        0     1273 2023-07-30 13:21:07.115930 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/javascript.862df613.js
+-rw-r--r--   0        0        0    39828 2023-07-30 13:21:07.123931 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/jsonMode.57ed33b2.js
+-rw-r--r--   0        0        0     7473 2023-07-30 13:21:07.123931 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/julia.21f68d09.js
+-rw-r--r--   0        0        0     3685 2023-07-30 13:21:07.123931 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/kotlin.3399aeb6.js
+-rw-r--r--   0        0        0     4141 2023-07-30 13:21:07.123931 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/less.b6aad23a.js
+-rw-r--r--   0        0        0     2683 2023-07-30 13:21:07.123931 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/lexon.44f813b3.js
+-rw-r--r--   0        0        0     4295 2023-07-30 13:21:07.123931 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/liquid.f36ec0b2.js
+-rw-r--r--   0        0        0     2369 2023-07-30 13:21:07.123931 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/lua.bbdfa9c0.js
+-rw-r--r--   0        0        0     3063 2023-07-30 13:21:07.123931 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/m3.92f755b1.js
+-rw-r--r--   0        0        0     4034 2023-07-30 13:21:07.123931 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/markdown.236ff8ef.js
+-rw-r--r--   0        0        0     2825 2023-07-30 13:21:07.123931 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/mips.148d2978.js
+-rw-r--r--   0        0        0     5158 2023-07-30 13:21:07.123931 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/msdax.f39564e2.js
+-rw-r--r--   0        0        0    11503 2023-07-30 13:21:07.123931 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/mysql.fdc04fe1.js
+-rw-r--r--   0        0        0     2648 2023-07-30 13:21:07.123931 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/objective-c.67633c2a.js
+-rw-r--r--   0        0        0     3241 2023-07-30 13:21:07.123931 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/pascal.c9d19959.js
+-rw-r--r--   0        0        0     2246 2023-07-30 13:21:07.123931 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/pascaligo.1c7de3c7.js
+-rw-r--r--   0        0        0     8501 2023-07-30 13:21:07.123931 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/perl.140c1c72.js
+-rw-r--r--   0        0        0    13650 2023-07-30 13:21:07.123931 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/pgsql.1a3b46c8.js
+-rw-r--r--   0        0        0     8273 2023-07-30 13:21:07.123931 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/php.a9540a84.js
+-rw-r--r--   0        0        0     1929 2023-07-30 13:21:07.123931 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/pla.c3f817e8.js
+-rw-r--r--   0        0        0     8102 2023-07-30 13:21:07.123931 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/postiats.8064247a.js
+-rw-r--r--   0        0        0    17185 2023-07-30 13:21:07.123931 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/powerquery.bc98d188.js
+-rw-r--r--   0        0        0     3515 2023-07-30 13:21:07.123931 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/powershell.d93de61d.js
+-rw-r--r--   0        0        0     9292 2023-07-30 13:21:07.123931 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/protobuf.0ea0cf3d.js
+-rw-r--r--   0        0        0     5074 2023-07-30 13:21:07.123931 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/pug.03a3b993.js
+-rw-r--r--   0        0        0     3922 2023-07-30 13:21:07.123931 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/python.95d3ecf9.js
+-rw-r--r--   0        0        0     3170 2023-07-30 13:21:07.123931 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/qsharp.c08b4fea.js
+-rw-r--r--   0        0        0     3377 2023-07-30 13:21:07.123931 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/r.1e4576a7.js
+-rw-r--r--   0        0        0     9108 2023-07-30 13:21:07.123931 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/razor.1abe54ff.js
+-rw-r--r--   0        0        0     3802 2023-07-30 13:21:07.123931 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/redis.8da5f515.js
+-rw-r--r--   0        0        0    12046 2023-07-30 13:21:07.123931 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/redshift.4a60845d.js
+-rw-r--r--   0        0        0     4139 2023-07-30 13:21:07.123931 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/restructuredtext.992abef6.js
+-rw-r--r--   0        0        0     8750 2023-07-30 13:21:07.123931 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/ruby.71d129bb.js
+-rw-r--r--   0        0        0     4406 2023-07-30 13:21:07.123931 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/rust.349e1143.js
+-rw-r--r--   0        0        0     2075 2023-07-30 13:21:07.123931 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/sb.e7ab3b92.js
+-rw-r--r--   0        0        0     7564 2023-07-30 13:21:07.123931 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/scala.ef542eb6.js
+-rw-r--r--   0        0        0     2013 2023-07-30 13:21:07.123931 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/scheme.d835dccb.js
+-rw-r--r--   0        0        0     6652 2023-07-30 13:21:07.123931 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/scss.19caa34f.js
+-rw-r--r--   0        0        0     3319 2023-07-30 13:21:07.123931 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/shell.4305d323.js
+-rw-r--r--   0        0        0    18843 2023-07-30 13:21:07.123931 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/solidity.212cde55.js
+-rw-r--r--   0        0        0     3010 2023-07-30 13:21:07.123931 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/sophia.69f82176.js
+-rw-r--r--   0        0        0     2798 2023-07-30 13:21:07.123931 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/sparql.1dcfd6e8.js
+-rw-r--r--   0        0        0    10543 2023-07-30 13:21:07.123931 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/sql.5f2f7ebd.js
+-rw-r--r--   0        0        0     7636 2023-07-30 13:21:07.123931 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/st.3f9156a8.js
+-rw-r--r--   0        0        0     5417 2023-07-30 13:21:07.123931 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/swift.575aa114.js
+-rw-r--r--   0        0        0     7849 2023-07-30 13:21:07.123931 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/systemverilog.a897e382.js
+-rw-r--r--   0        0        0     3817 2023-07-30 13:21:07.123931 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/tcl.50105b28.js
+-rw-r--r--   0        0        0    22361 2023-07-30 13:21:07.123931 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/tsMode.a26535a0.js
+-rw-r--r--   0        0        0     6218 2023-07-30 13:21:07.123931 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/twig.74745959.js
+-rw-r--r--   0        0        0     5722 2023-07-30 13:21:07.115930 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/typescript.8aef1446.js
+-rw-r--r--   0        0        0     6037 2023-07-30 13:21:07.123931 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/vb.42b9f30d.js
+-rw-r--r--   0        0        0     2748 2023-07-30 13:21:07.123931 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/xml.89ac767a.js
+-rw-r--r--   0        0        0     3790 2023-07-30 13:21:07.123931 sneakpeek_py-0.2.2/sneakpeek/static/ui/assets/yaml.7d8c6ae6.js
+-rw-r--r--   0        0        0     2359 2023-07-30 13:21:04.695882 sneakpeek_py-0.2.2/sneakpeek/static/ui/icons/favicon.png
+-rw-r--r--   0        0        0      659 2023-07-30 13:21:07.123931 sneakpeek_py-0.2.2/sneakpeek/static/ui/index.html
+-rw-r--r--   0        0        0    11392 2023-07-30 13:18:53.797283 sneakpeek_py-0.2.2/sneakpeek/tests/test_integration.py
+-rw-r--r--   0        0        0     4063 2023-07-30 13:18:53.797283 sneakpeek_py-0.2.2/sneakpeek/tests/test_metrics.py
+-rw-r--r--   0        0        0     9749 1970-01-01 00:00:00.000000 sneakpeek_py-0.2.2/PKG-INFO
```

### Comparing `sneakpeek_py-0.2.1/README.md` & `sneakpeek_py-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.2.1/pyproject.toml` & `sneakpeek_py-0.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "sneakpeek-py"
 packages = [{ include = "sneakpeek" }]
-version = "0.2.1"
+version = "0.2.2"
 description = "Sneakpeek is a framework that helps to quickly and conviniently develop scrapers. It's the best choice for scrapers that have some specific complex scraping logic that needs to be run on a constant basis."
 authors = ["Dan Yazovsky <daniil.yazovsky@gmail.com>"]
 maintainers = ["Dan Yazovsky <daniil.yazovsky@gmail.com>"]
 repository = "https://github.com/flulemon/sneakpeek"
 documentation = "https://sneakpeek-py.readthedocs.io/en/latest/"
 homepage = "https://github.com/flulemon/sneakpeek"
 license = "BSD-3-Clause"
```

### Comparing `sneakpeek_py-0.2.1/sneakpeek/api.py` & `sneakpeek_py-0.2.2/sneakpeek/api.py`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.2.1/sneakpeek/logging.py` & `sneakpeek_py-0.2.2/sneakpeek/logging.py`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.2.1/sneakpeek/metrics.py` & `sneakpeek_py-0.2.2/sneakpeek/metrics.py`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.2.1/sneakpeek/middleware/base.py` & `sneakpeek_py-0.2.2/sneakpeek/middleware/base.py`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.2.1/sneakpeek/middleware/parser.py` & `sneakpeek_py-0.2.2/sneakpeek/middleware/parser.py`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.2.1/sneakpeek/middleware/proxy_middleware.py` & `sneakpeek_py-0.2.2/sneakpeek/middleware/proxy_middleware.py`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.2.1/sneakpeek/middleware/rate_limiter_middleware.py` & `sneakpeek_py-0.2.2/sneakpeek/middleware/rate_limiter_middleware.py`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.2.1/sneakpeek/middleware/requests_logging_middleware.py` & `sneakpeek_py-0.2.2/sneakpeek/middleware/requests_logging_middleware.py`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.2.1/sneakpeek/middleware/robots_txt_middleware.py` & `sneakpeek_py-0.2.2/sneakpeek/middleware/robots_txt_middleware.py`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.2.1/sneakpeek/middleware/user_agent_injecter_middleware.py` & `sneakpeek_py-0.2.2/sneakpeek/middleware/user_agent_injecter_middleware.py`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.2.1/sneakpeek/queue/consumer.py` & `sneakpeek_py-0.2.2/sneakpeek/queue/consumer.py`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.2.1/sneakpeek/queue/in_memory_storage.py` & `sneakpeek_py-0.2.2/sneakpeek/queue/in_memory_storage.py`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.2.1/sneakpeek/queue/model.py` & `sneakpeek_py-0.2.2/sneakpeek/queue/model.py`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.2.1/sneakpeek/queue/queue.py` & `sneakpeek_py-0.2.2/sneakpeek/queue/queue.py`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.2.1/sneakpeek/queue/redis_storage.py` & `sneakpeek_py-0.2.2/sneakpeek/queue/redis_storage.py`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.2.1/sneakpeek/queue/tasks.py` & `sneakpeek_py-0.2.2/sneakpeek/queue/tasks.py`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.2.1/sneakpeek/queue/tests/test_consumer.py` & `sneakpeek_py-0.2.2/sneakpeek/queue/tests/test_consumer.py`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.2.1/sneakpeek/queue/tests/test_queue.py` & `sneakpeek_py-0.2.2/sneakpeek/queue/tests/test_queue.py`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.2.1/sneakpeek/queue/tests/test_queue_storage.py` & `sneakpeek_py-0.2.2/sneakpeek/queue/tests/test_queue_storage.py`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.2.1/sneakpeek/scheduler/in_memory_lease_storage.py` & `sneakpeek_py-0.2.2/sneakpeek/scheduler/in_memory_lease_storage.py`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.2.1/sneakpeek/scheduler/model.py` & `sneakpeek_py-0.2.2/sneakpeek/scheduler/model.py`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.2.1/sneakpeek/scheduler/redis_lease_storage.py` & `sneakpeek_py-0.2.2/sneakpeek/scheduler/redis_lease_storage.py`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.2.1/sneakpeek/scheduler/scheduler.py` & `sneakpeek_py-0.2.2/sneakpeek/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.2.1/sneakpeek/scheduler/tests/test_lease_storage.py` & `sneakpeek_py-0.2.2/sneakpeek/scheduler/tests/test_lease_storage.py`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.2.1/sneakpeek/scraper/context.py` & `sneakpeek_py-0.2.2/sneakpeek/scraper/context.py`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.2.1/sneakpeek/scraper/dynamic_scraper_handler.py` & `sneakpeek_py-0.2.2/sneakpeek/scraper/dynamic_scraper_handler.py`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.2.1/sneakpeek/scraper/ephemeral_scraper_task_handler.py` & `sneakpeek_py-0.2.2/sneakpeek/scraper/ephemeral_scraper_task_handler.py`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.2.1/sneakpeek/scraper/in_memory_storage.py` & `sneakpeek_py-0.2.2/sneakpeek/scraper/in_memory_storage.py`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.2.1/sneakpeek/scraper/model.py` & `sneakpeek_py-0.2.2/sneakpeek/scraper/model.py`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.2.1/sneakpeek/scraper/redis_storage.py` & `sneakpeek_py-0.2.2/sneakpeek/scraper/redis_storage.py`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.2.1/sneakpeek/scraper/runner.py` & `sneakpeek_py-0.2.2/sneakpeek/scraper/runner.py`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.2.1/sneakpeek/scraper/task_handler.py` & `sneakpeek_py-0.2.2/sneakpeek/scraper/task_handler.py`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.2.1/sneakpeek/scraper/tests/test_context.py` & `sneakpeek_py-0.2.2/sneakpeek/scraper/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.2.1/sneakpeek/scraper/tests/test_dynamic_scraper_handler.py` & `sneakpeek_py-0.2.2/sneakpeek/scraper/tests/test_dynamic_scraper_handler.py`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.2.1/sneakpeek/scraper/tests/test_scraper_storage.py` & `sneakpeek_py-0.2.2/sneakpeek/scraper/tests/test_scraper_storage.py`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.2.1/sneakpeek/server.py` & `sneakpeek_py-0.2.2/sneakpeek/server.py`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.2.1/sneakpeek/session_loggers/base.py` & `sneakpeek_py-0.2.2/sneakpeek/session_loggers/base.py`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.2.1/sneakpeek/session_loggers/file_logger.py` & `sneakpeek_py-0.2.2/sneakpeek/session_loggers/file_logger.py`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.2.1/sneakpeek/session_loggers/redis_logger.py` & `sneakpeek_py-0.2.2/sneakpeek/session_loggers/redis_logger.py`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.2.1/sneakpeek/tests/test_integration.py` & `sneakpeek_py-0.2.2/sneakpeek/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.2.1/sneakpeek/tests/test_metrics.py` & `sneakpeek_py-0.2.2/sneakpeek/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.2.1/PKG-INFO` & `sneakpeek_py-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sneakpeek-py
-Version: 0.2.1
+Version: 0.2.2
 Summary: Sneakpeek is a framework that helps to quickly and conviniently develop scrapers. It's the best choice for scrapers that have some specific complex scraping logic that needs to be run on a constant basis.
 Home-page: https://github.com/flulemon/sneakpeek
 License: BSD-3-Clause
 Author: Dan Yazovsky
 Author-email: daniil.yazovsky@gmail.com
 Maintainer: Dan Yazovsky
 Maintainer-email: daniil.yazovsky@gmail.com
```

