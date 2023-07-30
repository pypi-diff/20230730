# Comparing `tmp/sneakpeek_py-0.1.9.tar.gz` & `tmp/sneakpeek_py-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sneakpeek_py-0.1.9.tar", max compression
+gzip compressed data, was "sneakpeek_py-0.2.1.tar", max compression
```

## Comparing `sneakpeek_py-0.1.9.tar` & `sneakpeek_py-0.2.1.tar`

### file list

```diff
@@ -1,170 +1,45 @@
--rw-r--r--   0        0        0     7337 2023-06-01 07:52:06.506995 sneakpeek_py-0.1.9/README.md
--rw-r--r--   0        0        0     2233 2023-06-01 07:52:06.514996 sneakpeek_py-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     6098 2023-06-01 07:52:06.514996 sneakpeek_py-0.1.9/sneakpeek/api.py
--rw-r--r--   0        0        0      821 2023-06-01 07:52:06.514996 sneakpeek_py-0.1.9/sneakpeek/errors.py
--rw-r--r--   0        0        0     2914 2023-06-01 07:52:06.514996 sneakpeek_py-0.1.9/sneakpeek/logging.py
--rw-r--r--   0        0        0     5028 2023-06-01 07:52:06.514996 sneakpeek_py-0.1.9/sneakpeek/metrics.py
--rw-r--r--   0        0        0     3461 2023-06-01 07:52:06.514996 sneakpeek_py-0.1.9/sneakpeek/models.py
--rw-r--r--   0        0        0     1560 2023-06-01 07:52:06.514996 sneakpeek_py-0.1.9/sneakpeek/plugins/proxy_plugin.py
--rw-r--r--   0        0        0     4969 2023-06-01 07:52:06.514996 sneakpeek_py-0.1.9/sneakpeek/plugins/rate_limiter_plugin.py
--rw-r--r--   0        0        0     2273 2023-06-01 07:52:06.514996 sneakpeek_py-0.1.9/sneakpeek/plugins/requests_logging_plugin.py
--rw-r--r--   0        0        0     4120 2023-06-01 07:52:06.514996 sneakpeek_py-0.1.9/sneakpeek/plugins/robots_txt_plugin.py
--rw-r--r--   0        0        0     1755 2023-06-01 07:52:06.514996 sneakpeek_py-0.1.9/sneakpeek/plugins/user_agent_injecter_plugin.py
--rw-r--r--   0        0        0      659 2023-06-01 07:52:06.514996 sneakpeek_py-0.1.9/sneakpeek/plugins/utils.py
--rw-r--r--   0        0        0     6955 2023-06-01 07:52:06.514996 sneakpeek_py-0.1.9/sneakpeek/queue.py
--rw-r--r--   0        0        0     9226 2023-06-01 07:52:06.514996 sneakpeek_py-0.1.9/sneakpeek/runner.py
--rw-r--r--   0        0        0    13929 2023-06-01 07:52:06.514996 sneakpeek_py-0.1.9/sneakpeek/scheduler.py
--rw-r--r--   0        0        0      527 2023-06-01 07:52:06.514996 sneakpeek_py-0.1.9/sneakpeek/scraper_config.py
--rw-r--r--   0        0        0    20687 2023-06-01 07:52:06.518996 sneakpeek_py-0.1.9/sneakpeek/scraper_context.py
--rw-r--r--   0        0        0      655 2023-06-01 07:52:06.518996 sneakpeek_py-0.1.9/sneakpeek/scraper_handler.py
--rw-r--r--   0        0        0     7117 2023-06-01 07:52:06.518996 sneakpeek_py-0.1.9/sneakpeek/server.py
--rw-r--r--   0        0        0      550 2023-06-01 07:52:06.518996 sneakpeek_py-0.1.9/sneakpeek/static/assets/ErrorNotFound.9617f9a7.js
--rw-r--r--   0        0        0    20436 2023-06-01 07:52:06.518996 sneakpeek_py-0.1.9/sneakpeek/static/assets/KFOkCnqEu92Fr1MmgVxIIzQ.34e9582c.woff
--rw-r--r--   0        0        0    20544 2023-06-01 07:52:06.518996 sneakpeek_py-0.1.9/sneakpeek/static/assets/KFOlCnqEu92Fr1MmEU9fBBc-.9ce7f3ac.woff
--rw-r--r--   0        0        0    20416 2023-06-01 07:52:06.518996 sneakpeek_py-0.1.9/sneakpeek/static/assets/KFOlCnqEu92Fr1MmSU5fBBc-.bf14c7d7.woff
--rw-r--r--   0        0        0    20408 2023-06-01 07:52:06.518996 sneakpeek_py-0.1.9/sneakpeek/static/assets/KFOlCnqEu92Fr1MmWUlfBBc-.e0fd57c0.woff
--rw-r--r--   0        0        0    20424 2023-06-01 07:52:06.518996 sneakpeek_py-0.1.9/sneakpeek/static/assets/KFOlCnqEu92Fr1MmYUtfBBc-.f6537e32.woff
--rw-r--r--   0        0        0    20344 2023-06-01 07:52:06.518996 sneakpeek_py-0.1.9/sneakpeek/static/assets/KFOmCnqEu92Fr1Mu4mxM.f2abf7fb.woff
--rw-r--r--   0        0        0    24866 2023-06-01 07:52:06.518996 sneakpeek_py-0.1.9/sneakpeek/static/assets/MainLayout.06dc30a3.js
--rw-r--r--   0        0        0      538 2023-06-01 07:52:06.518996 sneakpeek_py-0.1.9/sneakpeek/static/assets/NewScraperPage.abf42128.js
--rw-r--r--   0        0        0    30651 2023-06-01 07:52:06.518996 sneakpeek_py-0.1.9/sneakpeek/static/assets/PriorityChip.61343a15.js
--rw-r--r--   0        0        0      655 2023-06-01 07:52:06.518996 sneakpeek_py-0.1.9/sneakpeek/static/assets/QList.7f24c43e.js
--rw-r--r--   0        0        0    76403 2023-06-01 07:52:06.518996 sneakpeek_py-0.1.9/sneakpeek/static/assets/QPage.6206ab40.js
--rw-r--r--   0        0        0  1333182 2023-06-01 07:52:06.526996 sneakpeek_py-0.1.9/sneakpeek/static/assets/ScraperEditForm.197dd68f.js
--rw-r--r--   0        0        0     3323 2023-06-01 07:52:06.526996 sneakpeek_py-0.1.9/sneakpeek/static/assets/ScraperEditForm.640de0df.css
--rw-r--r--   0        0        0    26587 2023-06-01 07:52:06.526996 sneakpeek_py-0.1.9/sneakpeek/static/assets/ScraperPage.732b3035.js
--rw-r--r--   0        0        0     2479 2023-06-01 07:52:06.526996 sneakpeek_py-0.1.9/sneakpeek/static/assets/ScrapersPage.06097019.js
--rw-r--r--   0        0        0    11097 2023-06-01 07:52:06.526996 sneakpeek_py-0.1.9/sneakpeek/static/assets/api.8025d512.js
--rw-r--r--   0        0        0   187208 2023-06-01 07:52:06.530996 sneakpeek_py-0.1.9/sneakpeek/static/assets/fa-brands-400.20c4a58b.ttf
--rw-r--r--   0        0        0   108020 2023-06-01 07:52:06.530996 sneakpeek_py-0.1.9/sneakpeek/static/assets/fa-brands-400.74833209.woff2
--rw-r--r--   0        0        0    63952 2023-06-01 07:52:06.530996 sneakpeek_py-0.1.9/sneakpeek/static/assets/fa-regular-400.528d022d.ttf
--rw-r--r--   0        0        0    24948 2023-06-01 07:52:06.530996 sneakpeek_py-0.1.9/sneakpeek/static/assets/fa-regular-400.8e7e5ea1.woff2
--rw-r--r--   0        0        0   394628 2023-06-01 07:52:06.530996 sneakpeek_py-0.1.9/sneakpeek/static/assets/fa-solid-900.67a65763.ttf
--rw-r--r--   0        0        0   150124 2023-06-01 07:52:06.534996 sneakpeek_py-0.1.9/sneakpeek/static/assets/fa-solid-900.7152a693.woff2
--rw-r--r--   0        0        0    10172 2023-06-01 07:52:06.534996 sneakpeek_py-0.1.9/sneakpeek/static/assets/fa-v4compatibility.0515a423.ttf
--rw-r--r--   0        0        0     4564 2023-06-01 07:52:06.534996 sneakpeek_py-0.1.9/sneakpeek/static/assets/fa-v4compatibility.694a17c3.woff2
--rw-r--r--   0        0        0   164912 2023-06-01 07:52:06.534996 sneakpeek_py-0.1.9/sneakpeek/static/assets/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.fd84f88b.woff
--rw-r--r--   0        0        0   128616 2023-06-01 07:52:06.534996 sneakpeek_py-0.1.9/sneakpeek/static/assets/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.4a4dbc62.woff2
--rw-r--r--   0        0        0   132320 2023-06-01 07:52:06.534996 sneakpeek_py-0.1.9/sneakpeek/static/assets/index.422cc3a0.js
--rw-r--r--   0        0        0   307194 2023-06-01 07:52:06.534996 sneakpeek_py-0.1.9/sneakpeek/static/assets/index.99b1d043.css
--rw-r--r--   0        0        0      230 2023-06-01 07:54:27.408548 sneakpeek_py-0.1.9/sneakpeek/static/docs/.buildinfo
--rw-r--r--   0        0        0  1124153 2023-06-01 07:54:25.804490 sneakpeek_py-0.1.9/sneakpeek/static/docs/.doctrees/api.doctree
--rw-r--r--   0        0        0     8116 2023-06-01 07:54:25.820490 sneakpeek_py-0.1.9/sneakpeek/static/docs/.doctrees/deployment.doctree
--rw-r--r--   0        0        0    40019 2023-06-01 07:54:25.972496 sneakpeek_py-0.1.9/sneakpeek/static/docs/.doctrees/design.doctree
--rw-r--r--   0        0        0    78291 2023-06-01 07:54:26.080500 sneakpeek_py-0.1.9/sneakpeek/static/docs/.doctrees/environment.pickle
--rw-r--r--   0        0        0     5428 2023-06-01 07:54:25.984496 sneakpeek_py-0.1.9/sneakpeek/static/docs/.doctrees/index.doctree
--rw-r--r--   0        0        0     7467 2023-06-01 07:54:25.996497 sneakpeek_py-0.1.9/sneakpeek/static/docs/.doctrees/local_debugging.doctree
--rw-r--r--   0        0        0     3823 2023-06-01 07:54:26.000497 sneakpeek_py-0.1.9/sneakpeek/static/docs/.doctrees/plugins/index.doctree
--rw-r--r--   0        0        0    13997 2023-06-01 07:54:26.016497 sneakpeek_py-0.1.9/sneakpeek/static/docs/.doctrees/plugins/new_plugin.doctree
--rw-r--r--   0        0        0     6215 2023-06-01 07:54:26.020498 sneakpeek_py-0.1.9/sneakpeek/static/docs/.doctrees/plugins/proxy_plugin.doctree
--rw-r--r--   0        0        0     8218 2023-06-01 07:54:26.032498 sneakpeek_py-0.1.9/sneakpeek/static/docs/.doctrees/plugins/rate_limiter_plugin.doctree
--rw-r--r--   0        0        0     6215 2023-06-01 07:54:26.040498 sneakpeek_py-0.1.9/sneakpeek/static/docs/.doctrees/plugins/requests_logging_plugin.doctree
--rw-r--r--   0        0        0     6235 2023-06-01 07:54:26.048498 sneakpeek_py-0.1.9/sneakpeek/static/docs/.doctrees/plugins/robots_txt_plugin.doctree
--rw-r--r--   0        0        0     7249 2023-06-01 07:54:26.056499 sneakpeek_py-0.1.9/sneakpeek/static/docs/.doctrees/plugins/user_agent_injecter_plugin.doctree
--rw-r--r--   0        0        0    13699 2023-06-01 07:54:26.072499 sneakpeek_py-0.1.9/sneakpeek/static/docs/.doctrees/quick_start.doctree
--rw-r--r--   0        0        0      947 2023-06-01 07:52:06.506995 sneakpeek_py-0.1.9/sneakpeek/static/docs/_sources/api.rst.txt
--rw-r--r--   0        0        0     1335 2023-06-01 07:52:06.506995 sneakpeek_py-0.1.9/sneakpeek/static/docs/_sources/deployment.rst.txt
--rw-r--r--   0        0        0     5816 2023-06-01 07:52:06.506995 sneakpeek_py-0.1.9/sneakpeek/static/docs/_sources/design.rst.txt
--rw-r--r--   0        0        0      496 2023-06-01 07:52:06.506995 sneakpeek_py-0.1.9/sneakpeek/static/docs/_sources/index.rst.txt
--rw-r--r--   0        0        0     1176 2023-06-01 07:52:06.506995 sneakpeek_py-0.1.9/sneakpeek/static/docs/_sources/local_debugging.rst.txt
--rw-r--r--   0        0        0      457 2023-06-01 07:52:06.506995 sneakpeek_py-0.1.9/sneakpeek/static/docs/_sources/plugins/index.rst.txt
--rw-r--r--   0        0        0     4271 2023-06-01 07:52:06.506995 sneakpeek_py-0.1.9/sneakpeek/static/docs/_sources/plugins/new_plugin.rst.txt
--rw-r--r--   0        0        0     1389 2023-06-01 07:52:06.506995 sneakpeek_py-0.1.9/sneakpeek/static/docs/_sources/plugins/proxy_plugin.rst.txt
--rw-r--r--   0        0        0     2053 2023-06-01 07:52:06.506995 sneakpeek_py-0.1.9/sneakpeek/static/docs/_sources/plugins/rate_limiter_plugin.rst.txt
--rw-r--r--   0        0        0     1338 2023-06-01 07:52:06.506995 sneakpeek_py-0.1.9/sneakpeek/static/docs/_sources/plugins/requests_logging_plugin.rst.txt
--rw-r--r--   0        0        0     1367 2023-06-01 07:52:06.506995 sneakpeek_py-0.1.9/sneakpeek/static/docs/_sources/plugins/robots_txt_plugin.rst.txt
--rw-r--r--   0        0        0     1507 2023-06-01 07:52:06.506995 sneakpeek_py-0.1.9/sneakpeek/static/docs/_sources/plugins/user_agent_injecter_plugin.rst.txt
--rw-r--r--   0        0        0     5404 2023-06-01 07:52:06.506995 sneakpeek_py-0.1.9/sneakpeek/static/docs/_sources/quick_start.rst.txt
--rw-r--r--   0        0        0    14638 2023-06-01 07:54:27.396547 sneakpeek_py-0.1.9/sneakpeek/static/docs/_static/basic.css
--rw-r--r--   0        0        0     3275 2023-06-01 07:52:30.699952 sneakpeek_py-0.1.9/sneakpeek/static/docs/_static/css/badge_only.css
--rw-r--r--   0        0        0    87624 2023-06-01 07:52:30.699952 sneakpeek_py-0.1.9/sneakpeek/static/docs/_static/css/fonts/Roboto-Slab-Bold.woff
--rw-r--r--   0        0        0    67312 2023-06-01 07:52:30.699952 sneakpeek_py-0.1.9/sneakpeek/static/docs/_static/css/fonts/Roboto-Slab-Bold.woff2
--rw-r--r--   0        0        0    86288 2023-06-01 07:52:30.703952 sneakpeek_py-0.1.9/sneakpeek/static/docs/_static/css/fonts/Roboto-Slab-Regular.woff
--rw-r--r--   0        0        0    66444 2023-06-01 07:52:30.703952 sneakpeek_py-0.1.9/sneakpeek/static/docs/_static/css/fonts/Roboto-Slab-Regular.woff2
--rw-r--r--   0        0        0   165742 2023-06-01 07:52:30.703952 sneakpeek_py-0.1.9/sneakpeek/static/docs/_static/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0        0        0   444379 2023-06-01 07:52:30.707952 sneakpeek_py-0.1.9/sneakpeek/static/docs/_static/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0        0        0   165548 2023-06-01 07:52:30.711953 sneakpeek_py-0.1.9/sneakpeek/static/docs/_static/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0        0        0    98024 2023-06-01 07:52:30.711953 sneakpeek_py-0.1.9/sneakpeek/static/docs/_static/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0        0        0    77160 2023-06-01 07:52:30.711953 sneakpeek_py-0.1.9/sneakpeek/static/docs/_static/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0        0        0   323344 2023-06-01 07:52:30.715953 sneakpeek_py-0.1.9/sneakpeek/static/docs/_static/css/fonts/lato-bold-italic.woff
--rw-r--r--   0        0        0   193308 2023-06-01 07:52:30.719953 sneakpeek_py-0.1.9/sneakpeek/static/docs/_static/css/fonts/lato-bold-italic.woff2
--rw-r--r--   0        0        0   309728 2023-06-01 07:52:30.719953 sneakpeek_py-0.1.9/sneakpeek/static/docs/_static/css/fonts/lato-bold.woff
--rw-r--r--   0        0        0   184912 2023-06-01 07:52:30.723953 sneakpeek_py-0.1.9/sneakpeek/static/docs/_static/css/fonts/lato-bold.woff2
--rw-r--r--   0        0        0   328412 2023-06-01 07:52:30.727953 sneakpeek_py-0.1.9/sneakpeek/static/docs/_static/css/fonts/lato-normal-italic.woff
--rw-r--r--   0        0        0   195704 2023-06-01 07:52:30.727953 sneakpeek_py-0.1.9/sneakpeek/static/docs/_static/css/fonts/lato-normal-italic.woff2
--rw-r--r--   0        0        0   309192 2023-06-01 07:52:30.731953 sneakpeek_py-0.1.9/sneakpeek/static/docs/_static/css/fonts/lato-normal.woff
--rw-r--r--   0        0        0   182708 2023-06-01 07:52:30.731953 sneakpeek_py-0.1.9/sneakpeek/static/docs/_static/css/fonts/lato-normal.woff2
--rw-r--r--   0        0        0   129674 2023-06-01 07:52:30.699952 sneakpeek_py-0.1.9/sneakpeek/static/docs/_static/css/theme.css
--rw-r--r--   0        0        0     9630 2023-06-01 07:52:30.023925 sneakpeek_py-0.1.9/sneakpeek/static/docs/_static/doctools.js
--rw-r--r--   0        0        0      353 2023-06-01 07:54:27.392547 sneakpeek_py-0.1.9/sneakpeek/static/docs/_static/documentation_options.js
--rw-r--r--   0        0        0      286 2023-06-01 07:52:30.027925 sneakpeek_py-0.1.9/sneakpeek/static/docs/_static/file.png
--rw-r--r--   0        0        0   287630 2023-06-01 07:52:30.027925 sneakpeek_py-0.1.9/sneakpeek/static/docs/_static/jquery-3.5.1.js
--rw-r--r--   0        0        0    89476 2023-06-01 07:52:30.031926 sneakpeek_py-0.1.9/sneakpeek/static/docs/_static/jquery.js
--rw-r--r--   0        0        0      934 2023-06-01 07:52:30.735953 sneakpeek_py-0.1.9/sneakpeek/static/docs/_static/js/badge_only.js
--rw-r--r--   0        0        0     4370 2023-06-01 07:52:30.735953 sneakpeek_py-0.1.9/sneakpeek/static/docs/_static/js/html5shiv-printshiv.min.js
--rw-r--r--   0        0        0     2734 2023-06-01 07:52:30.735953 sneakpeek_py-0.1.9/sneakpeek/static/docs/_static/js/html5shiv.min.js
--rw-r--r--   0        0        0     5023 2023-06-01 07:52:30.735953 sneakpeek_py-0.1.9/sneakpeek/static/docs/_static/js/theme.js
--rw-r--r--   0        0        0    10854 2023-06-01 07:54:27.400548 sneakpeek_py-0.1.9/sneakpeek/static/docs/_static/language_data.js
--rw-r--r--   0        0        0       90 2023-06-01 07:52:30.031926 sneakpeek_py-0.1.9/sneakpeek/static/docs/_static/minus.png
--rw-r--r--   0        0        0       90 2023-06-01 07:52:30.031926 sneakpeek_py-0.1.9/sneakpeek/static/docs/_static/plus.png
--rw-r--r--   0        0        0     4846 2023-06-01 07:54:27.388547 sneakpeek_py-0.1.9/sneakpeek/static/docs/_static/pygments.css
--rw-r--r--   0        0        0    16733 2023-06-01 07:52:30.031926 sneakpeek_py-0.1.9/sneakpeek/static/docs/_static/searchtools.js
--rw-r--r--   0        0        0    68420 2023-06-01 07:52:30.031926 sneakpeek_py-0.1.9/sneakpeek/static/docs/_static/underscore-1.13.1.js
--rw-r--r--   0        0        0    19530 2023-06-01 07:52:30.031926 sneakpeek_py-0.1.9/sneakpeek/static/docs/_static/underscore.js
--rw-r--r--   0        0        0   336661 2023-06-01 07:54:26.968532 sneakpeek_py-0.1.9/sneakpeek/static/docs/api.html
--rw-r--r--   0        0        0     7543 2023-06-01 07:54:26.992533 sneakpeek_py-0.1.9/sneakpeek/static/docs/deployment.html
--rw-r--r--   0        0        0    19310 2023-06-01 07:54:27.028534 sneakpeek_py-0.1.9/sneakpeek/static/docs/design.html
--rw-r--r--   0        0        0    47637 2023-06-01 07:54:27.352546 sneakpeek_py-0.1.9/sneakpeek/static/docs/genindex.html
--rw-r--r--   0        0        0     8726 2023-06-01 07:54:27.056535 sneakpeek_py-0.1.9/sneakpeek/static/docs/index.html
--rw-r--r--   0        0        0     8226 2023-06-01 07:54:27.096536 sneakpeek_py-0.1.9/sneakpeek/static/docs/local_debugging.html
--rw-r--r--   0        0        0     2154 2023-06-01 07:54:27.420548 sneakpeek_py-0.1.9/sneakpeek/static/docs/objects.inv
--rw-r--r--   0        0        0     7106 2023-06-01 07:54:27.116537 sneakpeek_py-0.1.9/sneakpeek/static/docs/plugins/index.html
--rw-r--r--   0        0        0    19746 2023-06-01 07:54:27.152539 sneakpeek_py-0.1.9/sneakpeek/static/docs/plugins/new_plugin.html
--rw-r--r--   0        0        0     9843 2023-06-01 07:54:27.180539 sneakpeek_py-0.1.9/sneakpeek/static/docs/plugins/proxy_plugin.html
--rw-r--r--   0        0        0    10368 2023-06-01 07:54:27.208541 sneakpeek_py-0.1.9/sneakpeek/static/docs/plugins/rate_limiter_plugin.html
--rw-r--r--   0        0        0     9179 2023-06-01 07:54:27.232541 sneakpeek_py-0.1.9/sneakpeek/static/docs/plugins/requests_logging_plugin.html
--rw-r--r--   0        0        0     9180 2023-06-01 07:54:27.260542 sneakpeek_py-0.1.9/sneakpeek/static/docs/plugins/robots_txt_plugin.html
--rw-r--r--   0        0        0     9609 2023-06-01 07:54:27.284543 sneakpeek_py-0.1.9/sneakpeek/static/docs/plugins/user_agent_injecter_plugin.html
--rw-r--r--   0        0        0    10214 2023-06-01 07:54:27.372547 sneakpeek_py-0.1.9/sneakpeek/static/docs/py-modindex.html
--rw-r--r--   0        0        0    18672 2023-06-01 07:54:27.320545 sneakpeek_py-0.1.9/sneakpeek/static/docs/quick_start.html
--rw-r--r--   0        0        0     5257 2023-06-01 07:54:27.388547 sneakpeek_py-0.1.9/sneakpeek/static/docs/search.html
--rw-r--r--   0        0        0    20711 2023-06-01 07:54:27.416548 sneakpeek_py-0.1.9/sneakpeek/static/docs/searchindex.js
--rw-r--r--   0        0        0    64483 2023-06-01 07:52:06.566998 sneakpeek_py-0.1.9/sneakpeek/static/favicon.ico
--rw-r--r--   0        0        0     2359 2023-06-01 07:52:06.566998 sneakpeek_py-0.1.9/sneakpeek/static/icons/favicon.png
--rw-r--r--   0        0        0      659 2023-06-01 07:52:06.566998 sneakpeek_py-0.1.9/sneakpeek/static/index.html
--rw-r--r--   0        0        0      550 2023-06-01 07:54:18.712218 sneakpeek_py-0.1.9/sneakpeek/static/ui/assets/ErrorNotFound.972e7850.js
--rw-r--r--   0        0        0    20436 2023-06-01 07:54:18.708218 sneakpeek_py-0.1.9/sneakpeek/static/ui/assets/KFOkCnqEu92Fr1MmgVxIIzQ.34e9582c.woff
--rw-r--r--   0        0        0    20544 2023-06-01 07:54:18.708218 sneakpeek_py-0.1.9/sneakpeek/static/ui/assets/KFOlCnqEu92Fr1MmEU9fBBc-.9ce7f3ac.woff
--rw-r--r--   0        0        0    20416 2023-06-01 07:54:18.708218 sneakpeek_py-0.1.9/sneakpeek/static/ui/assets/KFOlCnqEu92Fr1MmSU5fBBc-.bf14c7d7.woff
--rw-r--r--   0        0        0    20408 2023-06-01 07:54:18.708218 sneakpeek_py-0.1.9/sneakpeek/static/ui/assets/KFOlCnqEu92Fr1MmWUlfBBc-.e0fd57c0.woff
--rw-r--r--   0        0        0    20424 2023-06-01 07:54:18.708218 sneakpeek_py-0.1.9/sneakpeek/static/ui/assets/KFOlCnqEu92Fr1MmYUtfBBc-.f6537e32.woff
--rw-r--r--   0        0        0    20344 2023-06-01 07:54:18.708218 sneakpeek_py-0.1.9/sneakpeek/static/ui/assets/KFOmCnqEu92Fr1Mu4mxM.f2abf7fb.woff
--rw-r--r--   0        0        0    24988 2023-06-01 07:54:18.708218 sneakpeek_py-0.1.9/sneakpeek/static/ui/assets/MainLayout.7e461f65.js
--rw-r--r--   0        0        0      538 2023-06-01 07:54:18.712218 sneakpeek_py-0.1.9/sneakpeek/static/ui/assets/NewScraperPage.5377db97.js
--rw-r--r--   0        0        0    30657 2023-06-01 07:54:18.712218 sneakpeek_py-0.1.9/sneakpeek/static/ui/assets/PriorityChip.8abde99a.js
--rw-r--r--   0        0        0      655 2023-06-01 07:54:18.708218 sneakpeek_py-0.1.9/sneakpeek/static/ui/assets/QList.d29bf9dc.js
--rw-r--r--   0        0        0    76443 2023-06-01 07:54:18.712218 sneakpeek_py-0.1.9/sneakpeek/static/ui/assets/QPage.ace663b7.js
--rw-r--r--   0        0        0  1333099 2023-06-01 07:54:18.716218 sneakpeek_py-0.1.9/sneakpeek/static/ui/assets/ScraperEditForm.0ba5391a.js
--rw-r--r--   0        0        0     3323 2023-06-01 07:54:18.712218 sneakpeek_py-0.1.9/sneakpeek/static/ui/assets/ScraperEditForm.640de0df.css
--rw-r--r--   0        0        0    26582 2023-06-01 07:54:18.712218 sneakpeek_py-0.1.9/sneakpeek/static/ui/assets/ScraperPage.c8962e15.js
--rw-r--r--   0        0        0     2479 2023-06-01 07:54:18.712218 sneakpeek_py-0.1.9/sneakpeek/static/ui/assets/ScrapersPage.93db66c8.js
--rw-r--r--   0        0        0    11097 2023-06-01 07:54:18.708218 sneakpeek_py-0.1.9/sneakpeek/static/ui/assets/api.feb19451.js
--rw-r--r--   0        0        0   187208 2023-06-01 07:54:18.708218 sneakpeek_py-0.1.9/sneakpeek/static/ui/assets/fa-brands-400.20c4a58b.ttf
--rw-r--r--   0        0        0   108020 2023-06-01 07:54:18.704218 sneakpeek_py-0.1.9/sneakpeek/static/ui/assets/fa-brands-400.74833209.woff2
--rw-r--r--   0        0        0    63952 2023-06-01 07:54:18.708218 sneakpeek_py-0.1.9/sneakpeek/static/ui/assets/fa-regular-400.528d022d.ttf
--rw-r--r--   0        0        0    24948 2023-06-01 07:54:18.708218 sneakpeek_py-0.1.9/sneakpeek/static/ui/assets/fa-regular-400.8e7e5ea1.woff2
--rw-r--r--   0        0        0   394628 2023-06-01 07:54:18.708218 sneakpeek_py-0.1.9/sneakpeek/static/ui/assets/fa-solid-900.67a65763.ttf
--rw-r--r--   0        0        0   150124 2023-06-01 07:54:18.708218 sneakpeek_py-0.1.9/sneakpeek/static/ui/assets/fa-solid-900.7152a693.woff2
--rw-r--r--   0        0        0    10172 2023-06-01 07:54:18.708218 sneakpeek_py-0.1.9/sneakpeek/static/ui/assets/fa-v4compatibility.0515a423.ttf
--rw-r--r--   0        0        0     4564 2023-06-01 07:54:18.708218 sneakpeek_py-0.1.9/sneakpeek/static/ui/assets/fa-v4compatibility.694a17c3.woff2
--rw-r--r--   0        0        0   164912 2023-06-01 07:54:18.708218 sneakpeek_py-0.1.9/sneakpeek/static/ui/assets/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.fd84f88b.woff
--rw-r--r--   0        0        0   128616 2023-06-01 07:54:18.708218 sneakpeek_py-0.1.9/sneakpeek/static/ui/assets/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.4a4dbc62.woff2
--rw-r--r--   0        0        0   132977 2023-06-01 07:54:18.708218 sneakpeek_py-0.1.9/sneakpeek/static/ui/assets/index.75361530.js
--rw-r--r--   0        0        0   307193 2023-06-01 07:54:18.712218 sneakpeek_py-0.1.9/sneakpeek/static/ui/assets/index.e4ba73d8.css
--rw-r--r--   0        0        0     2359 2023-06-01 07:54:17.428167 sneakpeek_py-0.1.9/sneakpeek/static/ui/icons/favicon.png
--rw-r--r--   0        0        0      659 2023-06-01 07:54:18.712218 sneakpeek_py-0.1.9/sneakpeek/static/ui/index.html
--rw-r--r--   0        0        0     6067 2023-06-01 07:52:06.598999 sneakpeek_py-0.1.9/sneakpeek/storage/base.py
--rw-r--r--   0        0        0    10250 2023-06-01 07:52:06.598999 sneakpeek_py-0.1.9/sneakpeek/storage/in_memory_storage.py
--rw-r--r--   0        0        0     9838 2023-06-01 07:52:06.598999 sneakpeek_py-0.1.9/sneakpeek/storage/redis_storage.py
--rw-r--r--   0        0        0     4305 2023-06-01 07:52:06.598999 sneakpeek_py-0.1.9/sneakpeek/worker.py
--rw-r--r--   0        0        0     9430 1970-01-01 00:00:00.000000 sneakpeek_py-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     7605 2023-07-30 12:54:50.973317 sneakpeek_py-0.2.1/README.md
+-rw-r--r--   0        0        0     2279 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     7556 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/sneakpeek/api.py
+-rw-r--r--   0        0        0     2513 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/sneakpeek/logging.py
+-rw-r--r--   0        0        0     5028 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/sneakpeek/metrics.py
+-rw-r--r--   0        0        0     1289 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/sneakpeek/middleware/base.py
+-rw-r--r--   0        0        0     1141 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/sneakpeek/middleware/parser.py
+-rw-r--r--   0        0        0     1627 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/sneakpeek/middleware/proxy_middleware.py
+-rw-r--r--   0        0        0     5015 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/sneakpeek/middleware/rate_limiter_middleware.py
+-rw-r--r--   0        0        0     2301 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/sneakpeek/middleware/requests_logging_middleware.py
+-rw-r--r--   0        0        0     4187 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/sneakpeek/middleware/robots_txt_middleware.py
+-rw-r--r--   0        0        0     1822 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/sneakpeek/middleware/user_agent_injecter_middleware.py
+-rw-r--r--   0        0        0     5157 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/sneakpeek/queue/consumer.py
+-rw-r--r--   0        0        0     3510 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/sneakpeek/queue/in_memory_storage.py
+-rw-r--r--   0        0        0     7678 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/sneakpeek/queue/model.py
+-rw-r--r--   0        0        0     4132 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/sneakpeek/queue/queue.py
+-rw-r--r--   0        0        0     5065 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/sneakpeek/queue/redis_storage.py
+-rw-r--r--   0        0        0     1765 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/sneakpeek/queue/tasks.py
+-rw-r--r--   0        0        0     4257 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/sneakpeek/queue/tests/test_consumer.py
+-rw-r--r--   0        0        0     4318 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/sneakpeek/queue/tests/test_queue.py
+-rw-r--r--   0        0        0     2920 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/sneakpeek/queue/tests/test_queue_storage.py
+-rw-r--r--   0        0        0     1829 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/sneakpeek/scheduler/in_memory_lease_storage.py
+-rw-r--r--   0        0        0     4285 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/sneakpeek/scheduler/model.py
+-rw-r--r--   0        0        0     1676 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/sneakpeek/scheduler/redis_lease_storage.py
+-rw-r--r--   0        0        0     8923 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/sneakpeek/scheduler/scheduler.py
+-rw-r--r--   0        0        0     1867 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/sneakpeek/scheduler/tests/test_lease_storage.py
+-rw-r--r--   0        0        0     7941 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/sneakpeek/scraper/context.py
+-rw-r--r--   0        0        0     1889 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/sneakpeek/scraper/dynamic_scraper_handler.py
+-rw-r--r--   0        0        0     1398 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/sneakpeek/scraper/ephemeral_scraper_task_handler.py
+-rw-r--r--   0        0        0     2484 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/sneakpeek/scraper/in_memory_storage.py
+-rw-r--r--   0        0        0    18460 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/sneakpeek/scraper/model.py
+-rw-r--r--   0        0        0     2720 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/sneakpeek/scraper/redis_storage.py
+-rw-r--r--   0        0        0     4129 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/sneakpeek/scraper/runner.py
+-rw-r--r--   0        0        0     1193 2023-07-30 12:54:50.981317 sneakpeek_py-0.2.1/sneakpeek/scraper/task_handler.py
+-rw-r--r--   0        0        0    12021 2023-07-30 12:54:50.985317 sneakpeek_py-0.2.1/sneakpeek/scraper/tests/test_context.py
+-rw-r--r--   0        0        0     3239 2023-07-30 12:54:50.985317 sneakpeek_py-0.2.1/sneakpeek/scraper/tests/test_dynamic_scraper_handler.py
+-rw-r--r--   0        0        0     3673 2023-07-30 12:54:50.985317 sneakpeek_py-0.2.1/sneakpeek/scraper/tests/test_scraper_storage.py
+-rw-r--r--   0        0        0     8576 2023-07-30 12:54:50.985317 sneakpeek_py-0.2.1/sneakpeek/server.py
+-rw-r--r--   0        0        0      851 2023-07-30 12:54:50.985317 sneakpeek_py-0.2.1/sneakpeek/session_loggers/base.py
+-rw-r--r--   0        0        0     3728 2023-07-30 12:54:50.985317 sneakpeek_py-0.2.1/sneakpeek/session_loggers/file_logger.py
+-rw-r--r--   0        0        0     1844 2023-07-30 12:54:50.985317 sneakpeek_py-0.2.1/sneakpeek/session_loggers/redis_logger.py
+-rw-r--r--   0        0        0        0 2023-07-30 12:54:50.985317 sneakpeek_py-0.2.1/sneakpeek/static/.gitkeep
+-rw-r--r--   0        0        0    11392 2023-07-30 12:54:50.985317 sneakpeek_py-0.2.1/sneakpeek/tests/test_integration.py
+-rw-r--r--   0        0        0     4063 2023-07-30 12:54:50.985317 sneakpeek_py-0.2.1/sneakpeek/tests/test_metrics.py
+-rw-r--r--   0        0        0     9749 1970-01-01 00:00:00.000000 sneakpeek_py-0.2.1/PKG-INFO
```

### Comparing `sneakpeek_py-0.1.9/README.md` & `sneakpeek_py-0.2.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Sneakpeek
 
 ![CI](https://github.com/flulemon/sneakpeek/actions/workflows/ci.yml/badge.svg)
 [![PyPI version](https://badge.fury.io/py/sneakpeek-py.svg)](https://badge.fury.io/py/sneakpeek-py)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/sneakpeek-py?color=)
+[![Downloads](https://static.pepy.tech/badge/sneakpeek-py)](https://pepy.tech/project/sneakpeek-py)
 [![Documentation Status](https://readthedocs.org/projects/sneakpeek-py/badge/?version=latest)](https://sneakpeek-py.readthedocs.io/en/latest/?badge=latest)
 [![codecov](https://codecov.io/gh/flulemon/sneakpeek/branch/main/graph/badge.svg?token=7h45P8qHRG)](https://codecov.io/gh/flulemon/sneakpeek)
 
 **Sneakpeek** - is a framework that helps to quickly and conviniently develop scrapers.
 It's the best choice for scrapers that have some specific complex scraping logic that needs
 to be run on a constant basis.
 
@@ -217,7 +217,14 @@
 ## Documentation
 
 For the full documentation please visit [sneakpeek-py.readthedocs.io](https://sneakpeek-py.readthedocs.io/en/latest/)
 
 ## Contributing
 
 Please take a look at our [contributing](https://github.com/flulemon/sneakpeek/blob/main/CONTRIBUTING.md) guidelines if you're interested in helping!
+
+## Future plans
+
+- Support for developing and executing scrapers right in the browser
+- Plugins for headful and headless browser engines (Selenium and Playwright)
+- SQL storage implementation
+- Advanced monitoring for the scrapers' health
```

### Comparing `sneakpeek_py-0.1.9/pyproject.toml` & `sneakpeek_py-0.2.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "sneakpeek-py"
 packages = [{ include = "sneakpeek" }]
-version = "0.1.9"
+version = "0.2.1"
 description = "Sneakpeek is a framework that helps to quickly and conviniently develop scrapers. It's the best choice for scrapers that have some specific complex scraping logic that needs to be run on a constant basis."
 authors = ["Dan Yazovsky <daniil.yazovsky@gmail.com>"]
 maintainers = ["Dan Yazovsky <daniil.yazovsky@gmail.com>"]
 repository = "https://github.com/flulemon/sneakpeek"
 documentation = "https://sneakpeek-py.readthedocs.io/en/latest/"
 homepage = "https://github.com/flulemon/sneakpeek"
 license = "BSD-3-Clause"
@@ -14,14 +14,15 @@
     "Operating System :: OS Independent",
     "Development Status :: 2 - Pre-Alpha",
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Intended Audience :: Developers",
     "Framework :: FastAPI",
     "Framework :: Pydantic",
     "Topic :: Software Development :: Libraries :: Application Frameworks",
     "Topic :: Internet :: WWW/HTTP :: Indexing/Search"
 ]
```

### Comparing `sneakpeek_py-0.1.9/sneakpeek/metrics.py` & `sneakpeek_py-0.2.1/sneakpeek/metrics.py`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.1.9/sneakpeek/plugins/proxy_plugin.py` & `sneakpeek_py-0.2.1/sneakpeek/middleware/proxy_middleware.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,51 +1,53 @@
 from typing import Any
 
 from aiohttp import BasicAuth
 from fake_useragent import UserAgent
 from pydantic import BaseModel
+from typing_extensions import override
 from yarl import URL
 
-from sneakpeek.plugins.utils import parse_config_from_obj
-from sneakpeek.scraper_context import BeforeRequestPlugin, Request
+from sneakpeek.middleware.base import BaseMiddleware, parse_config_from_obj
+from sneakpeek.scraper.model import Request
 
 
-class ProxyPluginConfig(BaseModel):
-    """Proxy plugin config"""
+class ProxyMiddlewareConfig(BaseModel):
+    """Proxy middleware config"""
 
     proxy: str | URL | None = None  #: Proxy URL
     proxy_auth: BasicAuth | None = None  #: Proxy authentication info to use
 
     class Config:
         arbitrary_types_allowed = True
 
 
-class ProxyPlugin(BeforeRequestPlugin):
-    """Proxy plugin automatically sets proxy arguments for all HTTP requests."""
+class ProxyMiddleware(BaseMiddleware):
+    """Proxy middleware automatically sets proxy arguments for all HTTP requests."""
 
-    def __init__(self, default_config: ProxyPluginConfig | None = None) -> None:
-        self._default_config = default_config or ProxyPluginConfig()
+    def __init__(self, default_config: ProxyMiddlewareConfig | None = None) -> None:
+        self._default_config = default_config or ProxyMiddlewareConfig()
         self._user_agents = UserAgent(
             use_external_data=self._default_config.use_external_data,
             browsers=self._default_config.browsers,
         )
 
     @property
     def name(self) -> str:
         return "proxy"
 
-    async def before_request(
+    @override
+    async def on_request(
         self,
         request: Request,
         config: Any | None,
     ) -> Request:
         config = parse_config_from_obj(
             config,
             self.name,
-            ProxyPluginConfig,
+            ProxyMiddlewareConfig,
             self._default_config,
         )
         if not request.kwargs:
             request.kwargs = {}
         if config.proxy:
             request.kwargs["proxy"] = config.proxy
         if config.proxy_auth:
```

### Comparing `sneakpeek_py-0.1.9/sneakpeek/plugins/rate_limiter_plugin.py` & `sneakpeek_py-0.2.1/sneakpeek/middleware/rate_limiter_middleware.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 from random import randint
 from typing import Any
 from urllib.parse import urlparse
 
 from cachetools.func import ttl_cache
 from pydantic import BaseModel, validator
 
-from sneakpeek.plugins.utils import parse_config_from_obj
-from sneakpeek.scraper_context import BeforeRequestPlugin, Request
+from sneakpeek.middleware.base import BaseMiddleware, parse_config_from_obj
+from sneakpeek.scraper.model import Request
 
 DEFAULT_BUCKET_TIME_WINDOW = timedelta(minutes=1)
 
 
 def rate_limited_delay_jitter() -> timedelta:
     return timedelta(milliseconds=randint(0, 500))
 
@@ -57,16 +57,16 @@
 class RateLimitedStrategy(Enum):
     """What to do if the request is rate limited"""
 
     THROW = auto()  #: Throw an exception
     WAIT = auto()  #: Wait until request is no longer rate limited
 
 
-class RateLimiterPluginConfig(BaseModel):
-    """Rate limiter plugin configuration"""
+class RateLimiterMiddlewareConfig(BaseModel):
+    """Rate limiter middleware configuration"""
 
     #: Maximum number of allowed requests per host within time window
     max_requests: int = 60
     #: What to do if the request is rate limited
     rate_limited_strategy: RateLimitedStrategy = RateLimitedStrategy.WAIT
     #: Time window to aggregate requests
     time_window: timedelta = DEFAULT_BUCKET_TIME_WINDOW
@@ -85,43 +85,47 @@
                 self.max_requests,
                 self.rate_limited_strategy,
                 self.time_window,
             )
         )
 
 
-class RateLimiterPlugin(BeforeRequestPlugin):
+class RateLimiterMiddleware(BaseMiddleware):
     """
     Rate limiter implements `leaky bucket algorithm <https://en.wikipedia.org/wiki/Leaky_bucket>`_
     to limit number of requests made to the hosts. If the request is rate limited it can either
     raise an exception or wait until the request won't be limited anymore.
     """
 
-    def __init__(self, default_config: RateLimiterPluginConfig | None = None) -> None:
-        self._default_config = default_config or RateLimiterPluginConfig()
+    def __init__(
+        self, default_config: RateLimiterMiddlewareConfig | None = None
+    ) -> None:
+        self._default_config = default_config or RateLimiterMiddlewareConfig()
         self._logger = logging.getLogger(__name__)
 
     @property
     def name(self) -> str:
         return "rate_limiter"
 
     def _extract_key(self, url: str) -> str:
         return urlparse(url).hostname
 
     @ttl_cache(maxsize=None, ttl=timedelta(minutes=5).total_seconds())
-    def _get_bucket(self, key: str, config: RateLimiterPluginConfig) -> _LeakyBucket:
+    def _get_bucket(
+        self, key: str, config: RateLimiterMiddlewareConfig
+    ) -> _LeakyBucket:
         return _LeakyBucket(
             size=config.max_requests,
             time_window=config.time_window,
         )
 
     async def _wait_for_admission(
         self,
         url: str,
-        config: RateLimiterPluginConfig,
+        config: RateLimiterMiddlewareConfig,
     ) -> None:
         key = self._extract_key(url)
         bucket = self._get_bucket(key, config)
         while True:
             next_attempt_dt = await bucket.add()
             if not next_attempt_dt:
                 return
@@ -135,20 +139,20 @@
             if config.rate_limited_strategy == RateLimitedStrategy.THROW:
                 raise RateLimitedException(error_message)
             self._logger.info(error_message)
             attempt_delay = next_attempt_dt - datetime.utcnow()
             attempt_delay += rate_limited_delay_jitter()
             await asyncio.sleep(attempt_delay.total_seconds())
 
-    async def before_request(
+    async def on_request(
         self,
         request: Request,
         config: Any | None,
     ) -> Request:
         config = parse_config_from_obj(
             config,
             self.name,
-            RateLimiterPluginConfig,
+            RateLimiterMiddlewareConfig,
             self._default_config,
         )
         await self._wait_for_admission(request.url, config)
         return request
```

### Comparing `sneakpeek_py-0.1.9/sneakpeek/plugins/requests_logging_plugin.py` & `sneakpeek_py-0.2.1/sneakpeek/middleware/requests_logging_middleware.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,68 +1,71 @@
 import logging
 from typing import Any
 
 import aiohttp
 from pydantic import BaseModel
+from typing_extensions import override
 
-from sneakpeek.plugins.utils import parse_config_from_obj
-from sneakpeek.scraper_context import AfterResponsePlugin, BeforeRequestPlugin, Request
+from sneakpeek.middleware.base import parse_config_from_obj
+from sneakpeek.scraper.model import Middleware, Request
 
 
-class RequestsLoggingPluginConfig(BaseModel):
-    """Requests logging plugin config"""
+class RequestsLoggingMiddlewareConfig(BaseModel):
+    """Requests logging middleware config"""
 
     log_request: bool = True  #: Whether to log request being made
     log_response: bool = True  #: Whether to log response being made
 
 
-class RequestsLoggingPlugin(BeforeRequestPlugin, AfterResponsePlugin):
+class RequestsLoggingMiddleware(Middleware):
     """Requests logging middleware logs all requests being made and received responses."""
 
     def __init__(
-        self, default_config: RequestsLoggingPluginConfig | None = None
+        self, default_config: RequestsLoggingMiddlewareConfig | None = None
     ) -> None:
-        self._default_config = default_config or RequestsLoggingPluginConfig()
+        self._default_config = default_config or RequestsLoggingMiddlewareConfig()
         self._logger = logging.getLogger(__name__)
 
     @property
     def name(self) -> str:
         return "requests_logging"
 
-    async def before_request(
+    @override
+    async def on_request(
         self,
         request: Request,
         config: Any | None,
     ) -> Request:
         config = parse_config_from_obj(
             config,
             self.name,
-            RequestsLoggingPluginConfig,
+            RequestsLoggingMiddlewareConfig,
             self._default_config,
         )
         if config.log_request:
             self._logger.info(
                 f"{request.method.upper()} {request.url}",
                 extra={
                     "headers": request.headers,
                     "kwargs": request.kwargs,
                 },
             )
         return request
 
-    async def after_response(
+    @override
+    async def on_response(
         self,
         request: Request,
         response: aiohttp.ClientResponse,
         config: Any | None,
     ) -> aiohttp.ClientResponse:
         config = parse_config_from_obj(
             config,
             self.name,
-            RequestsLoggingPluginConfig,
+            RequestsLoggingMiddlewareConfig,
             self._default_config,
         )
         if config.log_response:
             response_body = await response.text()
             self._logger.info(
                 f"{request.method.upper()} {request.url} - {response.status} ",
                 extra={
```

### Comparing `sneakpeek_py-0.1.9/sneakpeek/plugins/robots_txt_plugin.py` & `sneakpeek_py-0.2.1/sneakpeek/middleware/robots_txt_middleware.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,17 +6,18 @@
 from typing import Any
 from urllib.parse import urlparse
 from urllib.robotparser import RobotFileParser
 
 import aiohttp
 from cachetools import TTLCache
 from pydantic import BaseModel
+from typing_extensions import override
 
-from sneakpeek.plugins.utils import parse_config_from_obj
-from sneakpeek.scraper_context import BeforeRequestPlugin, Request
+from sneakpeek.middleware.base import BaseMiddleware, parse_config_from_obj
+from sneakpeek.scraper.model import Request
 
 
 class RobotsTxtViolationException(Exception):
     """Exception which is raised if request is disallowed by website robots.txt"""
 
     pass
 
@@ -24,25 +25,25 @@
 class RobotsTxtViolationStrategy(Enum):
     """What to do if the request is disallowed by website robots.txt"""
 
     LOG = auto()  #: Only log violation
     THROW = auto()  #: Raise an exception on vioalation
 
 
-class RobotsTxtPluginConfig(BaseModel):
-    """robots.txt plugin configuration"""
+class RobotsTxtMiddlewareConfig(BaseModel):
+    """robots.txt middleware configuration"""
 
     violation_strategy: RobotsTxtViolationStrategy = RobotsTxtViolationStrategy.LOG
 
 
-class RobotsTxtPlugin(BeforeRequestPlugin):
-    """Robots.txt plugin can log and optionally block requests if they are disallowed by website robots.txt."""
+class RobotsTxtMiddleware(BaseMiddleware):
+    """Robots.txt middleware can log and optionally block requests if they are disallowed by website robots.txt."""
 
-    def __init__(self, default_config: RobotsTxtPluginConfig | None = None) -> None:
-        self._default_config = default_config or RobotsTxtPluginConfig()
+    def __init__(self, default_config: RobotsTxtMiddlewareConfig | None = None) -> None:
+        self._default_config = default_config or RobotsTxtMiddlewareConfig()
         self._logger = logging.getLogger(__name__)
         self._cache = TTLCache(
             maxsize=sys.maxsize,
             ttl=timedelta(hours=1).total_seconds(),
         )
 
     @property
@@ -77,23 +78,24 @@
                 except Exception as e:
                     self._logger.error(f"Failed to get robots.txt for {host}: {e}")
                     self._logger.debug(
                         f"Failed to get robots.txt for {host}. Traceback: {format_exc()}"
                     )
         return None
 
-    async def before_request(
+    @override
+    async def on_request(
         self,
         request: Request,
         config: Any | None,
     ) -> Request:
         config = parse_config_from_obj(
             config,
             self.name,
-            RobotsTxtPluginConfig,
+            RobotsTxtMiddlewareConfig,
             self._default_config,
         )
         host = self._extract_host(request.url)
         robots_txt = await self._load_robots_txt(host)
         if not robots_txt:
             self._logger.debug(
                 f"No robots.txt was retrieved for {request.url}. Defaulting to allow"
```

### Comparing `sneakpeek_py-0.1.9/sneakpeek/plugins/user_agent_injecter_plugin.py` & `sneakpeek_py-0.2.1/sneakpeek/middleware/user_agent_injecter_middleware.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,54 +1,56 @@
 from typing import Any
 
 from fake_useragent import UserAgent
 from pydantic import BaseModel
+from typing_extensions import override
 
-from sneakpeek.plugins.utils import parse_config_from_obj
-from sneakpeek.scraper_context import BeforeRequestPlugin, Request
+from sneakpeek.middleware.base import BaseMiddleware, parse_config_from_obj
+from sneakpeek.scraper.model import Request
 
 
-class UserAgentInjecterPluginConfig(BaseModel):
-    """Plugin configuration"""
+class UserAgentInjecterMiddlewareConfig(BaseModel):
+    """Middleware configuration"""
 
     #: Whether to use external data as a fallback
     use_external_data: bool = True
 
     #: List of browsers which are used to generate user agents
     browsers: list[str] = ["chrome", "edge", "firefox", "safari", "opera"]
 
 
-class UserAgentInjecterPlugin(BeforeRequestPlugin):
+class UserAgentInjecterMiddleware(BaseMiddleware):
     """
-    This plugin automatically adds ``User-Agent`` header if it's not present.
+    This middleware automatically adds ``User-Agent`` header if it's not present.
     It uses `fake-useragent <https://pypi.org/project/fake-useragent/>`_ in order to generate fake real world user agents.
     """
 
     def __init__(
-        self, default_config: UserAgentInjecterPluginConfig | None = None
+        self, default_config: UserAgentInjecterMiddlewareConfig | None = None
     ) -> None:
-        self._default_config = default_config or UserAgentInjecterPluginConfig()
+        self._default_config = default_config or UserAgentInjecterMiddlewareConfig()
         self._user_agents = UserAgent(
             use_external_data=self._default_config.use_external_data,
             browsers=self._default_config.browsers,
         )
 
     @property
     def name(self) -> str:
         return "user_agent_injecter"
 
-    async def before_request(
+    @override
+    async def on_request(
         self,
         request: Request,
         config: Any | None,
     ) -> Request:
         config = parse_config_from_obj(
             config,
             self.name,
-            UserAgentInjecterPluginConfig,
+            UserAgentInjecterMiddlewareConfig,
             self._default_config,
         )
         if (request.headers or {}).get("User-Agent"):
             return request
         if not request.headers:
             request.headers = {}
         request.headers["User-Agent"] = self._user_agents.random
```

### Comparing `sneakpeek_py-0.1.9/sneakpeek/scraper_context.py` & `sneakpeek_py-0.2.1/sneakpeek/scraper/model.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,128 @@
-import asyncio
-import logging
-import os
-import re
-import sys
-import tempfile
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
+from datetime import timedelta
 from enum import Enum
 from typing import Any, Awaitable, Callable
-from uuid import uuid4
 
 import aiohttp
+import fastapi_jsonrpc as jsonrpc
+from pydantic import BaseModel
+from typing_extensions import override
+
+from sneakpeek.queue.model import TaskPriority
+from sneakpeek.scheduler.model import (
+    PeriodicTask,
+    PeriodicTasksStorageABC,
+    TaskSchedule,
+)
 
-from sneakpeek.models import Scraper
-from sneakpeek.scraper_config import ScraperConfig
+SCRAPER_PERIODIC_TASK_HANDLER_NAME = "scraper"
+EPHEMERAL_SCRAPER_TASK_HANDLER_NAME = "ephemeral_scraper"
 
+ScraperId = str
 HttpHeaders = dict[str, str]
-PluginConfig = Any
+MiddlewareConfig = Any
+Response = aiohttp.ClientResponse | list[aiohttp.ClientResponse | Exception]
+
+
+class ScraperConfig(BaseModel):
+    #: Scraper configuration that is passed to the handler. Defaults to None.
+    params: dict[str, Any] | None = None
+    #: Middleware configuration that defines which middleware to use (besides global ones). Takes precedence over global middleware configuration. Defaults to None.
+    middleware_config: dict[str, Any] | None = None
+
+
+class Scraper(BaseModel):
+    """Scraper metadata"""
+
+    id: ScraperId  #: Scraper unique identifier
+    name: str  #: Scraper name
+    handler: str  #: Name of the scraper handler that implements scraping logic
+    schedule: TaskSchedule  #: Scraper schedule configuration
+    schedule_crontab: str | None  #: Must be defined if schedule equals to ``CRONTAB``
+    config: ScraperConfig  #: Scraper configuration that is passed to the handler
+    #: Default priority to enqueue scraper jobs with
+    priority: TaskPriority = TaskPriority.NORMAL
+    #: Scraper state (might be useful to optimise scraping, e.g. only process pages that weren't processed in the last jobs)
+    state: str | None = None
+    #: Timeout for the single scraper job
+    timeout: timedelta | None = None
+
+
+class ScraperNotFoundError(jsonrpc.BaseError):
+    CODE = 5000
+    MESSAGE = "Scraper not found"
+
+
+class StorageIsReadOnlyError(jsonrpc.BaseError):
+    CODE = 5001
+    MESSAGE = "StorageIsReadOnlyError"
+
+
+class UnknownScraperHandlerError(jsonrpc.BaseError):
+    CODE = 10002
+    MESSAGE = "Unknown scraper handler"
+
+
+class CreateScraperRequest(BaseModel):
+    name: str  #: Scraper name
+    handler: str  #: Name of the scraper handler that implements scraping logic
+    schedule: TaskSchedule  #: Scraper schedule configuration
+    schedule_crontab: str | None  #: Must be defined if schedule equals to ``CRONTAB``
+    config: ScraperConfig  #: Scraper configuration that is passed to the handler
+    #: Default priority to enqueue scraper jobs with
+    priority: TaskPriority = TaskPriority.NORMAL
+    #: Timeout for the single scraper job
+    timeout_seconds: int | None = None
+
+
+class ScraperStorageABC(PeriodicTasksStorageABC):
+    @abstractmethod
+    def is_read_only(self) -> bool:
+        ...
+
+    @abstractmethod
+    async def create_scraper(self, request: CreateScraperRequest) -> Scraper:
+        ...
+
+    @abstractmethod
+    async def update_scraper(self, request: Scraper) -> Scraper:
+        ...
+
+    @abstractmethod
+    async def delete_scraper(self, id: ScraperId) -> Scraper:
+        ...
+
+    @abstractmethod
+    async def get_scraper(self, id: ScraperId) -> Scraper:
+        ...
+
+    @abstractmethod
+    async def get_scrapers(self) -> list[Scraper]:
+        ...
+
+    def _convert_scraper_to_periodic_task(self, scraper: Scraper) -> PeriodicTask:
+        return PeriodicTask(
+            id=scraper.id,
+            name=scraper.id,
+            handler=SCRAPER_PERIODIC_TASK_HANDLER_NAME,
+            priority=scraper.priority,
+            schedule=scraper.schedule,
+            schedule_crontab=scraper.schedule_crontab,
+            timeout=timedelta(seconds=scraper.timeout) if scraper.timeout else None,
+            payload="",
+        )
+
+    @override
+    async def get_periodic_tasks(self) -> list[PeriodicTask]:
+        return [
+            self._convert_scraper_to_periodic_task(scraper)
+            for scraper in await self.get_scrapers()
+        ]
 
 
 class HttpMethod(str, Enum):
     """HTTP method"""
 
     GET = "get"
     POST = "post"
@@ -36,213 +138,92 @@
 
     method: HttpMethod
     url: str
     headers: HttpHeaders | None = None
     kwargs: dict[str, Any] | None = None
 
 
-@dataclass
-class _BatchRequest:
-    """HTTP Batch request metadata"""
-
-    method: HttpMethod
-    urls: list[str]
-    headers: HttpHeaders | None = None
-    kwargs: dict[str, Any] | None = None
-
-    def to_single_requests(self) -> list[Request]:
-        return [
-            Request(
-                method=self.method,
-                url=url,
-                headers=self.headers,
-                kwargs=self.kwargs,
-            )
-            for url in self.urls
-        ]
-
-
-@dataclass
-class RegexMatch:
-    """Regex match"""
-
-    full_match: str  #: Full regular expression match
-    groups: dict[str, str]  #: Regular expression group matches
-
-
-class BeforeRequestPlugin(ABC):
-    """Abstract class for the plugin which is called before each request (like Middleware)"""
+class Middleware(ABC):
+    """Abstract class for the middleware which is called before each request and response"""
 
     @property
     @abstractmethod
     def name(self) -> str:
-        """Name of the plugin"""
+        """Name of the middleware"""
         ...
 
     @abstractmethod
-    async def before_request(
+    async def on_request(
         self,
         request: Request,
-        config: Any | None = None,
+        config: MiddlewareConfig | None = None,
     ) -> Request:
         """
         Function that is called on each (HTTP) request before its dispatched.
 
         Args:
             request (Request): Request metadata
-            config (Any | None, optional): Plugin configuration. Defaults to None.
+            config (Any | None, optional): Middleware configuration. Defaults to None.
 
         Returns:
             Request: Request metadata
         """
-        ...
-
-
-class AfterResponsePlugin(ABC):
-    """Abstract class for the plugin which is called after each request"""
-
-    @property
-    @abstractmethod
-    def name(self) -> str:
-        """Name of the plugin"""
-        ...
+        return request
 
     @abstractmethod
-    async def after_response(
+    async def on_response(
         self,
         request: Request,
         response: aiohttp.ClientResponse,
-        config: Any | None = None,
+        config: MiddlewareConfig | None = None,
     ) -> aiohttp.ClientResponse:
         """
         Function that is called on each (HTTP) response before its result returned to the caller.
 
         Args:
             request (Request): Request metadata
             response (aiohttp.ClientResponse): HTTP Response
-            config (Any | None, optional): Plugin configuration. Defaults to None.
+            config (Any | None, optional): Middleware configuration. Defaults to None.
 
         Returns:
             aiohttp.ClientResponse: HTTP Response
         """
-        ...
-
-
-Plugin = BeforeRequestPlugin | AfterResponsePlugin
-Response = aiohttp.ClientResponse | list[aiohttp.ClientResponse | Exception]
+        return response
 
 
-class ScraperContext:
+class ScraperContextABC(ABC):
     """
     Scraper context - helper class that implements basic HTTP client which logic can be extended by
-    plugins that can preprocess request (e.g. Rate Limiter) and postprocess response (e.g. Response logger).
+    middleware that can preprocess request (e.g. Rate Limiter) and postprocess response (e.g. Response logger).
     """
 
-    def __init__(
-        self,
-        config: ScraperConfig,
-        plugins: list[Plugin] | None = None,
-        scraper_state: str | None = None,
-        update_scraper_state_func: Callable | None = None,
-    ) -> None:
-        """
-        Args:
-            config (ScraperConfig): Scraper configuration
-            plugins (list[BeforeRequestPlugin | AfterResponsePlugin] | None, optional): List of available plugins. Defaults to None.
-            scraper_state (str | None, optional): Scraper state. Defaults to None.
-            update_scraper_state_func (Callable | None, optional): Function that update scraper state. Defaults to None.
-        """
-        self.params = config.params
-        self.state = scraper_state
-        self._update_scraper_state_func = update_scraper_state_func
-        self._logger = logging.getLogger(__name__)
-        self._plugins_configs = config.plugins or {}
-        self._session: aiohttp.ClientSession | None = None
-        self._before_request_plugins = []
-        self._after_response_plugins = []
-        self._init_plugins(plugins)
-
-    def _init_plugins(self, plugins: list[Plugin] | None = None) -> None:
-        for plugin in plugins or []:
-            if not plugin.name.isidentifier():
-                raise ValueError(
-                    "Plugin name must be a Python identifier. "
-                    f"Plugin {plugin.__class__} has invalid name: {plugin.name}"
-                )
-            setattr(self, plugin.name, plugin)
-            if isinstance(plugin, BeforeRequestPlugin):
-                self._before_request_plugins.append(plugin)
-            if isinstance(plugin, AfterResponsePlugin):
-                self._after_response_plugins.append(plugin)
-
     async def start_session(self) -> None:
         self._session = aiohttp.ClientSession()
         await self._session.__aenter__()
         return self
 
     async def close(self) -> None:
         if self._session:
             await self._session.close()
             self._session = None
         return self
 
-    async def _before_request(self, request: Request) -> Request:
-        for plugin in self._before_request_plugins:
-            request = await plugin.before_request(
-                request,
-                self._plugins_configs.get(plugin.name),
-            )
+    @abstractmethod
+    async def on_request(self, request: Request) -> Request:
         return request
 
-    async def _after_response(
+    @abstractmethod
+    async def on_response(
         self,
         request: Request,
         response: aiohttp.ClientResponse,
     ) -> aiohttp.ClientResponse:
-        for plugin in self._after_response_plugins:
-            response = await plugin.after_response(
-                request,
-                response,
-                self._plugins_configs.get(plugin.name),
-            )
-        return response
-
-    async def _single_request(self, request: Request) -> aiohttp.ClientResponse:
-        request = await self._before_request(request)
-        response = await getattr(self._session, request.method)(
-            request.url,
-            headers=request.headers,
-            **(request.kwargs or {}),
-        )
-        response = await self._after_response(request, response)
         return response
 
-    async def _request(
-        self,
-        request: _BatchRequest,
-        max_concurrency: int = 0,
-        return_exceptions: bool = False,
-    ) -> Response:
-        single_requests = request.to_single_requests()
-        if len(single_requests) == 1:
-            return await self._single_request(single_requests[0])
-
-        semaphore = asyncio.Semaphore(max_concurrency) if max_concurrency > 0 else None
-
-        async def process_request(request: Request):
-            if semaphore:
-                async with semaphore:
-                    return await self._single_request(request)
-            return await self._single_request(request)
-
-        return await asyncio.gather(
-            *[process_request(request) for request in single_requests],
-            return_exceptions=return_exceptions,
-        )
-
+    @abstractmethod
     async def request(
         self,
         method: HttpMethod,
         url: str | list[str],
         *,
         headers: HttpHeaders | None = None,
         max_concurrency: int = 0,
@@ -258,25 +239,17 @@
             max_concurrency (int, optional): Maximum number of concurrent requests. If set to 0 no limit is applied. Defaults to 0.
             return_exceptions (bool, optional): Whether to return exceptions instead of raising if there are multiple URLs provided. Defaults to False,
             **kwargs: See aiohttp.request() for the full list of arguments
 
         Returns:
             Response: HTTP response(s)
         """
-        return await self._request(
-            _BatchRequest(
-                method=method,
-                urls=url if isinstance(url, list) else [url],
-                headers=headers,
-                kwargs=kwargs,
-            ),
-            max_concurrency=max_concurrency,
-            return_exceptions=return_exceptions,
-        )
+        ...
 
+    @abstractmethod
     async def download_file(
         self,
         method: HttpMethod,
         url: str,
         *,
         file_path: str | None = None,
         file_process_fn: Callable[[str], Awaitable[Any]] | None = None,
@@ -292,31 +265,17 @@
             file_process_fn (Callable[[str], Any], optional): Function to process the file. If specified then function will be applied to the file and its result will be returned, the file will be removed after the function call. Defaults to None.
             headers (HttpHeaders | None, optional): HTTP headers. Defaults to None.
             **kwargs: See aiohttp.request() for the full list of arguments
 
         Returns:
             str | Any: File path if file process function is not defined or file process function result otherwise
         """
-        if not file_path:
-            file_path = os.path.join(tempfile.mkdtemp(), str(uuid4()))
-        response = await self.request(
-            method=method,
-            url=url,
-            headers=headers,
-            **kwargs,
-        )
-        contents = await response.read()
-        with open(file_path, "wb") as f:
-            f.write(contents)
-        if not file_process_fn:
-            return file_path
-        result = await file_process_fn(file_path)
-        os.remove(file_path)
-        return result
+        ...
 
+    @abstractmethod
     async def download_files(
         self,
         method: HttpMethod,
         urls: list[str],
         *,
         file_paths: list[str] | None = None,
         file_process_fn: Callable[[str], Awaitable[Any]] | None = None,
@@ -336,42 +295,15 @@
             max_concurrency (int, optional): Maximum number of concurrent requests. If set to 0 no limit is applied. Defaults to 0.
             return_exceptions (bool, optional): Whether to return exceptions instead of raising if there are multiple URLs provided. Defaults to False,
             **kwargs: See aiohttp.request() for the full list of arguments
 
         Returns:
             list[str | Any | Exception]: For each URL: file path if file process function is not defined or file process function result otherwise
         """
-        if file_paths:
-            if len(file_paths) != len(urls):
-                raise ValueError(
-                    f"Expected to have 1 file path per 1 URL, only have {len(file_paths)} for {len(urls)} URLs"
-                )
-
-        semaphore = asyncio.Semaphore(
-            max_concurrency if max_concurrency > 0 else sys.maxsize
-        )
-
-        async def process_request(url: str, file_path: str):
-            async with semaphore:
-                return await self.download_file(
-                    method,
-                    url,
-                    file_path=file_path,
-                    file_process_fn=file_process_fn,
-                    headers=headers,
-                    **kwargs,
-                )
-
-        return await asyncio.gather(
-            *[
-                process_request(url, file_path)
-                for url, file_path in zip(urls, file_paths)
-            ],
-            return_exceptions=return_exceptions,
-        )
+        ...
 
     async def get(
         self,
         url: str | list[str],
         *,
         headers: HttpHeaders | None = None,
         max_concurrency: int = 0,
@@ -545,43 +477,60 @@
             url,
             headers=headers,
             max_concurrency=max_concurrency,
             return_exceptions=return_exceptions,
             **kwargs,
         )
 
-    def regex(
-        self,
-        text: str,
-        pattern: str,
-        flags: re.RegexFlag = re.UNICODE | re.MULTILINE | re.IGNORECASE,
-    ) -> list[RegexMatch]:
-        """Find matches in the text using regular expression
+    @abstractmethod
+    async def update_scraper_state(self, state: str) -> Scraper:
+        """Update scraper state
 
         Args:
-            text (str): Text to search in
-            pattern (str): Regular expression
-            flags (re.RegexFlag, optional): Regular expression flags. Defaults to re.UNICODE | re.MULTILINE | re.IGNORECASE.
+            state (str): State to persist
 
         Returns:
-            list[RegexMatch]: Matches found in the text
+            Scraper: Updated scraper metadata
         """
-        return [
-            RegexMatch(full_match=match.group(0), groups=match.groupdict())
-            for match in re.finditer(pattern, text, flags)
-        ]
+        ...
 
-    async def update_scraper_state(self, state: str) -> Scraper:
-        """Update scraper state
+
+class ScraperHandler(ABC):
+    """Abstract class that scraper logic handler must implement"""
+
+    @property
+    @abstractmethod
+    def name(self) -> str:
+        """Name of the handler"""
+        ...
+
+    @abstractmethod
+    async def run(self, context: ScraperContextABC) -> str:
+        """Execute scraper logic
 
         Args:
-            state (str): State to persist
+            context (ScraperContext): Scraper context
 
         Returns:
-            Scraper: Updated scraper metadata
+            str: scraper result that will be persisted in the storage (should be relatively small information to give sense on job result)
+        """
+        ...
+
+
+class ScraperRunnerABC(ABC):
+    @abstractmethod
+    async def run(self, handler: ScraperHandler, scraper: Scraper) -> str:
         """
-        if not self._update_scraper_state_func:
-            self._logger.warning(
-                "Tried to update scraper state, but the function to do it is not set"
-            )
-            return
-        return await self._update_scraper_state_func(state)
+        Args:
+            handler (ScraperHandler): Scraper logic implementation
+            scraper (Scraper): Scraper metadata
+        """
+        ...
+
+    @abstractmethod
+    async def run_ephemeral(
+        self,
+        handler: ScraperHandler,
+        config: ScraperConfig | None = None,
+        state: str | None = None,
+    ) -> str | None:
+        ...
```

### Comparing `sneakpeek_py-0.1.9/sneakpeek/server.py` & `sneakpeek_py-0.2.1/sneakpeek/server.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,21 +4,33 @@
 from signal import SIGINT, SIGTERM
 from traceback import format_exc
 
 import fastapi_jsonrpc as jsonrpc
 import uvicorn
 
 from sneakpeek.api import create_api
-from sneakpeek.queue import Queue
-from sneakpeek.runner import Runner
-from sneakpeek.scheduler import Scheduler, SchedulerABC
-from sneakpeek.scraper_context import Plugin
-from sneakpeek.scraper_handler import ScraperHandler
-from sneakpeek.storage.base import LeaseStorage, ScraperJobsStorage, ScrapersStorage
-from sneakpeek.worker import Worker, WorkerABC
+from sneakpeek.queue.consumer import Consumer
+from sneakpeek.queue.model import QueueStorageABC
+from sneakpeek.queue.queue import Queue
+from sneakpeek.queue.tasks import (
+    DeleteOldTasksHandler,
+    KillDeadTasksHandler,
+    queue_periodic_tasks,
+)
+from sneakpeek.scheduler.model import (
+    LeaseStorageABC,
+    MultiPeriodicTasksStorage,
+    SchedulerABC,
+)
+from sneakpeek.scheduler.scheduler import Scheduler
+from sneakpeek.scraper.dynamic_scraper_handler import DynamicScraperHandler
+from sneakpeek.scraper.ephemeral_scraper_task_handler import EphemeralScraperTaskHandler
+from sneakpeek.scraper.model import Middleware, ScraperHandler, ScraperStorageABC
+from sneakpeek.scraper.runner import ScraperRunner
+from sneakpeek.scraper.task_handler import ScraperTaskHandler
 
 WEB_SERVER_DEFAULT_PORT = 8080
 WORKER_DEFAULT_CONCURRENCY = 50
 SCHEDULER_DEFAULT_LEASE_DURATION = timedelta(minutes=1)
 SCHEDULER_DEFAULT_STORAGE_POLL_DELAY = timedelta(seconds=5)
 
 
@@ -29,97 +41,120 @@
     * API - allows interactions with scrapers storage and scrapers via JsonRPC or UI
     * Worker - executes scheduled scrapers
     * Scheduler - automatically schedules scrapers that are stored in the storage
     """
 
     def __init__(
         self,
-        worker: WorkerABC | None = None,
+        consumer: Consumer | None = None,
         scheduler: SchedulerABC | None = None,
         web_server: jsonrpc.API | None = None,
         web_server_port: int = WEB_SERVER_DEFAULT_PORT,
     ) -> None:
         """
         Args:
-            worker (WorkerABC | None, optional): Worker that consumes scraper jobs queue. Defaults to None.
+            consumer (Consumer | None, optional): Worker that consumes tasks queue. Defaults to None.
             scheduler (SchedulerABC | None, optional): Scrapers scheduler. Defaults to None.
             web_server (jsonrpc.API | None, optional): Web Server that implements API and exposes UI to interact with the system. Defaults to None.
             web_server_port (int, optional): Port which is used for Web Server (API, UI and metrics). Defaults to 8080.
         """
         self._logger = logging.getLogger(__name__)
-        self.worker = worker
+        self.consumer = consumer
         self.scheduler = scheduler
         self.api_config = (
             uvicorn.Config(
                 web_server, host="0.0.0.0", port=web_server_port, log_config=None
             )
             if web_server
             else None
         )
-        self.web_server = uvicorn.Server(self.api_config) if web_server else None
         self.scheduler = scheduler
+        self.web_server = uvicorn.Server(self.api_config) if web_server else None
+        self.web_server_task: asyncio.Task | None = None
 
     @staticmethod
     def create(
         handlers: list[ScraperHandler],
-        scrapers_storage: ScrapersStorage,
-        jobs_storage: ScraperJobsStorage,
-        lease_storage: LeaseStorage,
+        scraper_storage: ScraperStorageABC,
+        queue_storage: QueueStorageABC,
+        lease_storage: LeaseStorageABC,
         with_web_server: bool = True,
         with_worker: bool = True,
         with_scheduler: bool = True,
         worker_max_concurrency: int = WORKER_DEFAULT_CONCURRENCY,
         web_server_port: int = WEB_SERVER_DEFAULT_PORT,
         scheduler_storage_poll_delay: timedelta = SCHEDULER_DEFAULT_STORAGE_POLL_DELAY,
         scheduler_lease_duration: timedelta = SCHEDULER_DEFAULT_LEASE_DURATION,
-        plugins: list[Plugin] | None = None,
+        middlewares: list[Middleware] | None = None,
+        add_dynamic_scraper_handler: bool = False,
+        session_logger_handler: logging.Handler | None = None,
     ):
         """
         Create Sneakpeek server using default API, worker and scheduler implementations
 
         Args:
             handlers (list[ScraperHandler]): List of handlers that implement scraper logic
-            scrapers_storage (ScrapersStorage): Scrapers storage
+            scraper_storage (ScrapersStorage): Scrapers storage
             jobs_storage (ScraperJobsStorage): Jobs storage
             lease_storage (LeaseStorage): Lease storage
             with_web_server (bool, optional): Whether to run API service. Defaults to True.
             with_worker (bool, optional): Whether to run worker service. Defaults to True.
             with_scheduler (bool, optional): Whether to run scheduler service. Defaults to True.
             worker_max_concurrency (int, optional): Maximum number of concurrently executed scrapers. Defaults to 50.
             web_server_port (int, optional): Port which is used for Web Server (API, UI and metrics). Defaults to 8080.
             scheduler_storage_poll_delay (timedelta, optional): How much scheduler wait before polling storage for scrapers updates. Defaults to 5 seconds.
             scheduler_lease_duration (timedelta, optional): How long scheduler lease lasts. Lease is required for scheduler to be able to create new scraper jobs. This is needed so at any point of time there's only one active scheduler instance. Defaults to 1 minute.
             plugins (list[Plugin] | None, optional): List of plugins that will be used by scraper runner. Can be omitted if run_worker is False. Defaults to None.
-            metrics_port (int, optional): Port which is used to expose metric. Defaults to 9090.
+            add_dynamic_scraper_handler (bool, optional): Whether to add dynamic scraper handler which can execute arbitrary user scripts. Defaults to False.
         """
-        queue = Queue(scrapers_storage, jobs_storage)
+        if add_dynamic_scraper_handler:
+            dynamic_scraper_handler = DynamicScraperHandler()
+            if not any(h for h in handlers if h.name == dynamic_scraper_handler.name):
+                handlers.append(dynamic_scraper_handler)
+
+        runner = ScraperRunner(scraper_storage, middlewares)
+        queue = Queue(queue_storage)
+        task_handlers = [
+            KillDeadTasksHandler(queue),
+            DeleteOldTasksHandler(queue),
+            ScraperTaskHandler(handlers, runner, scraper_storage),
+            EphemeralScraperTaskHandler(handlers, runner),
+        ]
+        periodic_tasks_storage = MultiPeriodicTasksStorage(
+            [
+                queue_periodic_tasks,
+                scraper_storage,
+            ]
+        )
         scheduler = (
             Scheduler(
-                scrapers_storage,
-                jobs_storage,
+                periodic_tasks_storage,
                 lease_storage,
                 queue,
-                scheduler_storage_poll_delay,
-                scheduler_lease_duration,
+                tasks_poll_delay=scheduler_storage_poll_delay,
+                lease_duration=scheduler_lease_duration,
             )
             if with_scheduler
             else None
         )
-        runner = Runner(handlers, queue, scrapers_storage, jobs_storage, plugins)
-        worker = (
-            Worker(runner, queue, max_concurrency=worker_max_concurrency)
+        consumer = (
+            Consumer(
+                queue,
+                task_handlers,
+                max_concurrency=worker_max_concurrency,
+            )
             if with_worker
             else None
         )
         api = (
-            create_api(scrapers_storage, jobs_storage, queue, handlers)
+            create_api(scraper_storage, queue, handlers, session_logger_handler)
             if with_web_server
             else None
         )
-        return SneakpeekServer(worker, scheduler, api, web_server_port)
+        return SneakpeekServer(consumer, scheduler, api, web_server_port)
 
     def serve(
         self,
         loop: asyncio.AbstractEventLoop | None = None,
         blocking: bool = True,
     ) -> None:
         """
@@ -128,19 +163,19 @@
         Args:
             loop (asyncio.AbstractEventLoop | None, optional): AsyncIO loop to use. In case it's None result of `asyncio.get_event_loop()` will be used. Defaults to None.
             blocking (bool, optional): Whether to block thread while server is running. Defaults to True.
         """
         loop = loop or asyncio.get_event_loop()
         self._logger.info("Starting sneakpeek server")
         if self.scheduler:
-            loop.create_task(self.scheduler.start())
-        if self.worker:
-            loop.create_task(self.worker.start())
+            self.scheduler.start()
+        if self.consumer:
+            self.consumer.start()
         if self.web_server:
-            loop.create_task(self.web_server.serve())
+            self.web_server_task = loop.create_task(self.web_server.serve())
         loop.create_task(self._install_signals())
         if blocking:
             loop.run_forever()
 
     async def _install_signals(self) -> None:
         loop = asyncio.get_running_loop()
         for signal in [SIGINT, SIGTERM]:
@@ -149,16 +184,18 @@
     def stop(self, loop: asyncio.AbstractEventLoop | None = None) -> None:
         """Stop Sneakpeek server
 
         Args:
             loop (asyncio.AbstractEventLoop | None, optional): AsyncIO loop to use. In case it's None result of `asyncio.get_event_loop()` will be used. Defaults to None.
         """
         loop = loop or asyncio.get_event_loop()
-        loop.stop()
         self._logger.info("Stopping sneakpeek server")
         try:
             if self.scheduler:
                 self.scheduler.stop()
-            if self.worker:
-                self.worker.stop()
+            if self.consumer:
+                self.consumer.stop()
+            if self.web_server_task:
+                self.web_server_task.cancel()
+            loop.stop()
         except Exception:
             self._logger.error(f"Failed to stop: {format_exc()}")
```

### Comparing `sneakpeek_py-0.1.9/sneakpeek/static/docs/.doctrees/quick_start.doctree` & `sneakpeek_py-0.2.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,857 +1,610 @@
-00000000: 8005 9578 3500 0000 0000 008c 0f73 7068  ...x5........sph
-00000010: 696e 782e 6164 646e 6f64 6573 948c 0864  inx.addnodes...d
-00000020: 6f63 756d 656e 7494 9394 2981 947d 9428  ocument...)..}.(
-00000030: 8c09 7261 7773 6f75 7263 6594 8c00 948c  ..rawsource.....
-00000040: 0863 6869 6c64 7265 6e94 5d94 8c0e 646f  .children.]...do
-00000050: 6375 7469 6c73 2e6e 6f64 6573 948c 0773  cutils.nodes...s
-00000060: 6563 7469 6f6e 9493 9429 8194 7d94 2868  ection...)..}.(h
-00000070: 0568 0668 075d 9428 6809 8c05 7469 746c  .h.h.].(h...titl
-00000080: 6594 9394 2981 947d 9428 6805 8c0b 5175  e...)..}.(h...Qu
-00000090: 6963 6b20 7374 6172 7494 6807 5d94 6809  ick start.h.].h.
-000000a0: 8c04 5465 7874 9493 948c 0b51 7569 636b  ..Text.....Quick
-000000b0: 2073 7461 7274 9485 9481 947d 9428 6805   start.....}.(h.
-000000c0: 6813 8c06 7061 7265 6e74 9468 118c 095f  h...parent.h..._
-000000d0: 646f 6375 6d65 6e74 9468 038c 0673 6f75  document.h...sou
-000000e0: 7263 6594 4e8c 046c 696e 6594 4e75 6261  rce.N..line.Nuba
-000000f0: 8c0a 6174 7472 6962 7574 6573 947d 9428  ..attributes.}.(
-00000100: 8c03 6964 7394 5d94 8c07 636c 6173 7365  ..ids.]...classe
-00000110: 7394 5d94 8c05 6e61 6d65 7394 5d94 8c08  s.]...names.]...
-00000120: 6475 706e 616d 6573 945d 948c 0862 6163  dupnames.]...bac
-00000130: 6b72 6566 7394 5d94 758c 0774 6167 6e61  krefs.].u..tagna
-00000140: 6d65 9468 0f68 1b68 0c68 1c68 0368 1d8c  me.h.h.h.h.h.h..
-00000150: 3a2f 686f 6d65 2f72 756e 6e65 722f 776f  :/home/runner/wo
-00000160: 726b 2f73 6e65 616b 7065 656b 2f73 6e65  rk/sneakpeek/sne
-00000170: 616b 7065 656b 2f64 6f63 732f 7175 6963  akpeek/docs/quic
-00000180: 6b5f 7374 6172 742e 7273 7494 681e 4b03  k_start.rst.h.K.
-00000190: 7562 6809 8c09 7061 7261 6772 6170 6894  ubh...paragraph.
-000001a0: 9394 2981 947d 9428 6805 8c62 536f 2079  ..)..}.(h..bSo y
-000001b0: 6f75 2077 616e 7420 746f 2063 7265 6174  ou want to creat
-000001c0: 6520 6120 6e65 7720 7363 7261 7065 722c  e a new scraper,
-000001d0: 2066 6972 7374 2079 6f75 206e 6565 6420   first you need 
-000001e0: 746f 206d 616b 6520 7375 7265 2079 6f75  to make sure you
-000001f0: 2068 6176 6520 696e 7374 616c 6c65 6420   have installed 
-00000200: 2a2a 536e 6561 6b70 6565 6b2a 2a3a 9468  **Sneakpeek**:.h
-00000210: 075d 9428 6816 8c54 536f 2079 6f75 2077  .].(h..TSo you w
-00000220: 616e 7420 746f 2063 7265 6174 6520 6120  ant to create a 
-00000230: 6e65 7720 7363 7261 7065 722c 2066 6972  new scraper, fir
-00000240: 7374 2079 6f75 206e 6565 6420 746f 206d  st you need to m
-00000250: 616b 6520 7375 7265 2079 6f75 2068 6176  ake sure you hav
-00000260: 6520 696e 7374 616c 6c65 6420 9485 9481  e installed ....
-00000270: 947d 9428 6805 8c54 536f 2079 6f75 2077  .}.(h..TSo you w
-00000280: 616e 7420 746f 2063 7265 6174 6520 6120  ant to create a 
-00000290: 6e65 7720 7363 7261 7065 722c 2066 6972  new scraper, fir
-000002a0: 7374 2079 6f75 206e 6565 6420 746f 206d  st you need to m
-000002b0: 616b 6520 7375 7265 2079 6f75 2068 6176  ake sure you hav
-000002c0: 6520 696e 7374 616c 6c65 6420 9468 1b68  e installed .h.h
-000002d0: 2f68 1c68 0368 1d4e 681e 4e75 6268 098c  /h.h.h.Nh.Nubh..
-000002e0: 0673 7472 6f6e 6794 9394 2981 947d 9428  .strong...)..}.(
-000002f0: 6805 8c0d 2a2a 536e 6561 6b70 6565 6b2a  h...**Sneakpeek*
-00000300: 2a94 6807 5d94 6816 8c09 536e 6561 6b70  *.h.].h...Sneakp
-00000310: 6565 6b94 8594 8194 7d94 2868 0568 0668  eek.....}.(h.h.h
-00000320: 1b68 3a68 1c68 0368 1d4e 681e 4e75 6261  .h:h.h.h.Nh.Nuba
-00000330: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
-00000340: 9468 275d 9468 295d 9475 682b 6838 681b  .h'].h)].uh+h8h.
-00000350: 682f 7562 6816 8c01 3a94 8594 8194 7d94  h/ubh...:.....}.
-00000360: 2868 058c 013a 9468 1b68 2f68 1c68 0368  (h...:.h.h/h.h.h
-00000370: 1d4e 681e 4e75 6265 681f 7d94 2868 215d  .Nh.Nubeh.}.(h!]
-00000380: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
-00000390: 9475 682b 682d 681d 682c 681e 4b05 681b  .uh+h-h.h,h.K.h.
-000003a0: 680c 681c 6803 7562 6809 8c0d 6c69 7465  h.h.h.ubh...lite
-000003b0: 7261 6c5f 626c 6f63 6b94 9394 2981 947d  ral_block...)..}
-000003c0: 9428 6805 8c18 7069 7020 696e 7374 616c  .(h...pip instal
-000003d0: 6c20 736e 6561 6b70 6565 6b2d 7079 9468  l sneakpeek-py.h
-000003e0: 075d 9468 168c 1870 6970 2069 6e73 7461  .].h...pip insta
-000003f0: 6c6c 2073 6e65 616b 7065 656b 2d70 7994  ll sneakpeek-py.
-00000400: 8594 8194 7d94 2868 0568 0668 1b68 5575  ....}.(h.h.h.hUu
-00000410: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
-00000420: 255d 9468 275d 9468 295d 948c 0978 6d6c  %].h'].h)]...xml
-00000430: 3a73 7061 6365 948c 0870 7265 7365 7276  :space...preserv
-00000440: 6594 8c05 666f 7263 6594 898c 086c 616e  e...force....lan
-00000450: 6775 6167 6594 8c04 6261 7368 948c 0e68  guage...bash...h
-00000460: 6967 686c 6967 6874 5f61 7267 7394 7d94  ighlight_args.}.
-00000470: 7568 2b68 5368 1d68 2c68 1e4b 0768 1b68  uh+hSh.h,h.K.h.h
-00000480: 0c68 1c68 0375 6268 2e29 8194 7d94 2868  .h.h.ubh.)..}.(h
-00000490: 058c 5154 6865 206e 6578 7420 7374 6570  ..QThe next step
-000004a0: 2077 6f75 6c64 2062 6520 696d 706c 656d   would be implem
-000004b0: 656e 7469 6e67 2073 6372 6170 6572 206c  enting scraper l
-000004c0: 6f67 6963 2028 6f72 2073 6f20 6361 6c6c  ogic (or so call
-000004d0: 6564 2073 6372 6170 6572 2068 616e 646c  ed scraper handl
-000004e0: 6572 293a 9468 075d 9468 168c 5154 6865  er):.h.].h..QThe
-000004f0: 206e 6578 7420 7374 6570 2077 6f75 6c64   next step would
-00000500: 2062 6520 696d 706c 656d 656e 7469 6e67   be implementing
-00000510: 2073 6372 6170 6572 206c 6f67 6963 2028   scraper logic (
-00000520: 6f72 2073 6f20 6361 6c6c 6564 2073 6372  or so called scr
-00000530: 6170 6572 2068 616e 646c 6572 293a 9485  aper handler):..
-00000540: 9481 947d 9428 6805 686c 681b 686a 681c  ...}.(h.hlh.hjh.
-00000550: 6803 681d 4e68 1e4e 7562 6168 1f7d 9428  h.h.Nh.Nubah.}.(
-00000560: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
-00000570: 6829 5d94 7568 2b68 2d68 1d68 2c68 1e4b  h)].uh+h-h.h,h.K
-00000580: 0b68 1b68 0c68 1c68 0375 6268 5429 8194  .h.h.h.h.ubhT)..
-00000590: 7d94 2868 0558 6807 0000 2320 6669 6c65  }.(h.Xh...# file
-000005a0: 3a20 6465 6d6f 5f73 6372 6170 6572 2e70  : demo_scraper.p
-000005b0: 790a 0a69 6d70 6f72 7420 6a73 6f6e 0a69  y..import json.i
-000005c0: 6d70 6f72 7420 6c6f 6767 696e 670a 0a66  mport logging..f
-000005d0: 726f 6d20 7079 6461 6e74 6963 2069 6d70  rom pydantic imp
-000005e0: 6f72 7420 4261 7365 4d6f 6465 6c0a 0a66  ort BaseModel..f
-000005f0: 726f 6d20 736e 6561 6b70 6565 6b2e 7363  rom sneakpeek.sc
-00000600: 7261 7065 725f 636f 6e74 6578 7420 696d  raper_context im
-00000610: 706f 7274 2053 6372 6170 6572 436f 6e74  port ScraperCont
-00000620: 6578 740a 6672 6f6d 2073 6e65 616b 7065  ext.from sneakpe
-00000630: 656b 2e73 6372 6170 6572 5f68 616e 646c  ek.scraper_handl
-00000640: 6572 2069 6d70 6f72 7420 5363 7261 7065  er import Scrape
-00000650: 7248 616e 646c 6572 0a0a 0a23 2054 6869  rHandler...# Thi
-00000660: 7320 6465 6669 6e65 7320 6d6f 6465 6c20  s defines model 
-00000670: 6f66 2068 616e 646c 6572 2070 6172 616d  of handler param
-00000680: 6574 6572 7320 7468 6174 2061 7265 2064  eters that are d
-00000690: 6566 696e 6564 0a23 2069 6e20 7468 6520  efined.# in the 
-000006a0: 7363 7261 7065 7220 636f 6e66 6967 2061  scraper config a
-000006b0: 6e64 2074 6865 6e20 7061 7373 6564 2074  nd then passed t
-000006c0: 6f20 7468 6520 6861 6e64 6c65 720a 636c  o the handler.cl
-000006d0: 6173 7320 4465 6d6f 5363 7261 7065 7250  ass DemoScraperP
-000006e0: 6172 616d 7328 4261 7365 4d6f 6465 6c29  arams(BaseModel)
-000006f0: 3a0a 2020 2020 7572 6c3a 2073 7472 0a0a  :.    url: str..
-00000700: 2320 5468 6973 2069 7320 6120 636c 6173  # This is a clas
-00000710: 7320 7768 6963 6820 6163 7475 616c 6c79  s which actually
-00000720: 2069 6d70 6c65 6d65 6e74 7320 6c6f 6769   implements logi
-00000730: 630a 2320 4e6f 7465 2074 6861 7420 796f  c.# Note that yo
-00000740: 7520 6e65 6564 2074 6f20 696e 6865 7269  u need to inheri
-00000750: 7420 7468 6520 696d 706c 656d 656e 7461  t the implementa
-00000760: 7469 6f6e 2066 726f 6d0a 2320 7468 6520  tion from.# the 
-00000770: 6073 6e65 616b 7065 656b 2e73 6372 6170  `sneakpeek.scrap
-00000780: 6572 5f68 616e 646c 6572 2e53 6372 6170  er_handler.Scrap
-00000790: 6572 4861 6e64 6c65 7260 0a63 6c61 7373  erHandler`.class
-000007a0: 2044 656d 6f53 6372 6170 6572 2853 6372   DemoScraper(Scr
-000007b0: 6170 6572 4861 6e64 6c65 7229 3a0a 2020  aperHandler):.  
-000007c0: 2020 2320 596f 7520 6361 6e20 6861 7665    # You can have
-000007d0: 2061 6e79 2064 6570 656e 6465 6e63 6965   any dependencie
-000007e0: 7320 796f 7520 7761 6e74 2061 6e64 2070  s you want and p
-000007f0: 6173 7320 7468 656d 0a20 2020 2023 2069  ass them.    # i
-00000800: 6e20 7468 6520 7365 7276 6572 2063 6f6e  n the server con
-00000810: 6669 6775 7261 7469 6f6e 0a20 2020 2064  figuration.    d
-00000820: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
-00000830: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-00000840: 2020 2073 656c 662e 5f6c 6f67 6765 7220     self._logger 
-00000850: 3d20 6c6f 6767 696e 672e 6765 744c 6f67  = logging.getLog
-00000860: 6765 7228 5f5f 6e61 6d65 5f5f 290a 0a20  ger(__name__).. 
-00000870: 2020 2023 2045 6163 6820 6861 6e64 6c65     # Each handle
-00000880: 7220 6d75 7374 2064 6566 696e 6520 6974  r must define it
-00000890: 7320 6e61 6d65 2073 6f20 6974 206c 6174  s name so it lat
-000008a0: 6572 0a20 2020 2023 2063 616e 2062 6520  er.    # can be 
-000008b0: 7265 6665 7265 6e63 6564 2069 6e20 7363  referenced in sc
-000008c0: 7261 7065 7273 2720 636f 6e66 6967 7572  rapers' configur
-000008d0: 6174 696f 6e0a 2020 2020 4070 726f 7065  ation.    @prope
-000008e0: 7274 790a 2020 2020 6465 6620 6e61 6d65  rty.    def name
-000008f0: 2873 656c 6629 202d 3e20 7374 723a 0a20  (self) -> str:. 
-00000900: 2020 2020 2020 2072 6574 7572 6e20 2264         return "d
-00000910: 656d 6f5f 7363 7261 7065 7222 0a0a 2020  emo_scraper"..  
-00000920: 2020 2320 536f 6d65 2065 7861 6d70 6c65    # Some example
-00000930: 2066 756e 6374 696f 6e20 7468 6174 2070   function that p
-00000940: 726f 6365 7373 6573 2074 6865 2072 6573  rocesses the res
-00000950: 706f 6e73 650a 2020 2020 2320 616e 6420  ponse.    # and 
-00000960: 6578 7472 6163 7473 2076 616c 7561 626c  extracts valuabl
-00000970: 6520 696e 666f 726d 6174 696f 6e0a 2020  e information.  
-00000980: 2020 6173 796e 6320 6465 6620 7072 6f63    async def proc
-00000990: 6573 735f 7061 6765 2873 656c 662c 2072  ess_page(self, r
-000009a0: 6573 706f 6e73 653a 2073 7472 293a 0a20  esponse: str):. 
-000009b0: 2020 2020 2020 202e 2e2e 0a0a 2020 2020         .....    
-000009c0: 2320 5468 6973 2066 756e 6374 696f 6e20  # This function 
-000009d0: 6973 2063 616c 6c65 6420 6279 2074 6865  is called by the
-000009e0: 2077 6f72 6b65 7220 746f 2065 7865 6375   worker to execu
-000009f0: 7465 2074 6865 206c 6f67 6963 0a20 2020  te the logic.   
-00000a00: 2023 2054 6865 206f 6e6c 7920 6172 6775   # The only argu
-00000a10: 6d65 6e74 2074 6861 7420 6973 2070 6173  ment that is pas
-00000a20: 7365 6420 6973 2060 736e 6561 6b70 6565  sed is `sneakpee
-00000a30: 6b2e 7363 7261 7065 725f 636f 6e74 6578  k.scraper_contex
-00000a40: 742e 5363 7261 7065 7243 6f6e 7465 7874  t.ScraperContext
-00000a50: 600a 2020 2020 2320 4974 2069 6d70 6c65  `.    # It imple
-00000a60: 6d65 6e74 7320 6261 7369 6320 6173 796e  ments basic asyn
-00000a70: 6320 4854 5450 2063 6c69 656e 7420 616e  c HTTP client an
-00000a80: 6420 616c 736f 2070 726f 7669 6465 7320  d also provides 
-00000a90: 7061 7261 6d65 7465 7273 0a20 2020 2023  parameters.    #
-00000aa0: 2074 6861 7420 6172 6520 6465 6669 6e65   that are define
-00000ab0: 6420 696e 2074 6865 2073 6372 6170 6572  d in the scraper
-00000ac0: 2063 6f6e 6669 670a 2020 2020 6173 796e   config.    asyn
-00000ad0: 6320 6465 6620 7275 6e28 7365 6c66 2c20  c def run(self, 
-00000ae0: 636f 6e74 6578 743a 2053 6372 6170 6572  context: Scraper
-00000af0: 436f 6e74 6578 7429 202d 3e20 7374 723a  Context) -> str:
-00000b00: 0a20 2020 2020 2020 2070 6172 616d 7320  .        params 
-00000b10: 3d20 4465 6d6f 5363 7261 7065 7250 6172  = DemoScraperPar
-00000b20: 616d 732e 7061 7273 655f 6f62 6a28 636f  ams.parse_obj(co
-00000b30: 6e74 6578 742e 7061 7261 6d73 290a 2020  ntext.params).  
-00000b40: 2020 2020 2020 2320 5065 7266 6f72 6d20        # Perform 
-00000b50: 4745 5420 7265 7175 6573 7420 746f 2074  GET request to t
-00000b60: 6865 2055 524c 2064 6566 696e 6564 2069  he URL defined i
-00000b70: 6e20 7468 6520 7363 7261 7065 7220 636f  n the scraper co
-00000b80: 6e66 6967 0a20 2020 2020 2020 2072 6573  nfig.        res
-00000b90: 706f 6e73 6520 3d20 6177 6169 7420 636f  ponse = await co
-00000ba0: 6e74 6578 742e 6765 7428 7061 7261 6d73  ntext.get(params
-00000bb0: 2e75 726c 290a 2020 2020 2020 2020 7265  .url).        re
-00000bc0: 7370 6f6e 7365 5f62 6f64 7920 3d20 6177  sponse_body = aw
-00000bd0: 6169 7420 7265 7370 6f6e 7365 2e74 6578  ait response.tex
-00000be0: 7428 290a 0a20 2020 2020 2020 2023 2050  t()..        # P
-00000bf0: 6572 666f 726d 2073 6f6d 6520 6275 7369  erform some busi
-00000c00: 6e65 7373 206c 6f67 6963 206f 6e20 6120  ness logic on a 
-00000c10: 7265 7370 6f6e 7365 0a20 2020 2020 2020  response.       
-00000c20: 2072 6573 756c 7420 3d20 6177 6169 7420   result = await 
-00000c30: 7365 6c66 2e70 726f 6365 7373 5f70 6167  self.process_pag
-00000c40: 6528 7265 7370 6f6e 7365 5f62 6f64 7929  e(response_body)
-00000c50: 0a0a 2020 2020 2020 2020 2320 5265 7475  ..        # Retu
-00000c60: 726e 206d 6561 6e69 6e67 6675 6c20 6a6f  rn meaningful jo
-00000c70: 6220 7375 6d6d 6172 7920 2d20 6d75 7374  b summary - must
-00000c80: 2072 6574 7572 6e20 6120 7374 7269 6e67   return a string
-00000c90: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00000ca0: 6a73 6f6e 2e64 756d 7073 287b 0a20 2020  json.dumps({.   
-00000cb0: 2020 2020 2020 2020 2022 7072 6f63 6573           "proces
-00000cc0: 7365 645f 7572 6c73 223a 2031 2c0a 2020  sed_urls": 1,.  
-00000cd0: 2020 2020 2020 2020 2020 2266 6f75 6e64            "found
-00000ce0: 5f72 6573 756c 7473 223a 206c 656e 2872  _results": len(r
-00000cf0: 6573 756c 7429 2c0a 2020 2020 2020 2020  esult),.        
-00000d00: 7d29 9468 075d 9468 1658 6807 0000 2320  }).h.].h.Xh...# 
-00000d10: 6669 6c65 3a20 6465 6d6f 5f73 6372 6170  file: demo_scrap
-00000d20: 6572 2e70 790a 0a69 6d70 6f72 7420 6a73  er.py..import js
-00000d30: 6f6e 0a69 6d70 6f72 7420 6c6f 6767 696e  on.import loggin
-00000d40: 670a 0a66 726f 6d20 7079 6461 6e74 6963  g..from pydantic
-00000d50: 2069 6d70 6f72 7420 4261 7365 4d6f 6465   import BaseMode
-00000d60: 6c0a 0a66 726f 6d20 736e 6561 6b70 6565  l..from sneakpee
-00000d70: 6b2e 7363 7261 7065 725f 636f 6e74 6578  k.scraper_contex
-00000d80: 7420 696d 706f 7274 2053 6372 6170 6572  t import Scraper
-00000d90: 436f 6e74 6578 740a 6672 6f6d 2073 6e65  Context.from sne
-00000da0: 616b 7065 656b 2e73 6372 6170 6572 5f68  akpeek.scraper_h
-00000db0: 616e 646c 6572 2069 6d70 6f72 7420 5363  andler import Sc
-00000dc0: 7261 7065 7248 616e 646c 6572 0a0a 0a23  raperHandler...#
-00000dd0: 2054 6869 7320 6465 6669 6e65 7320 6d6f   This defines mo
-00000de0: 6465 6c20 6f66 2068 616e 646c 6572 2070  del of handler p
-00000df0: 6172 616d 6574 6572 7320 7468 6174 2061  arameters that a
-00000e00: 7265 2064 6566 696e 6564 0a23 2069 6e20  re defined.# in 
-00000e10: 7468 6520 7363 7261 7065 7220 636f 6e66  the scraper conf
-00000e20: 6967 2061 6e64 2074 6865 6e20 7061 7373  ig and then pass
-00000e30: 6564 2074 6f20 7468 6520 6861 6e64 6c65  ed to the handle
-00000e40: 720a 636c 6173 7320 4465 6d6f 5363 7261  r.class DemoScra
-00000e50: 7065 7250 6172 616d 7328 4261 7365 4d6f  perParams(BaseMo
-00000e60: 6465 6c29 3a0a 2020 2020 7572 6c3a 2073  del):.    url: s
-00000e70: 7472 0a0a 2320 5468 6973 2069 7320 6120  tr..# This is a 
-00000e80: 636c 6173 7320 7768 6963 6820 6163 7475  class which actu
-00000e90: 616c 6c79 2069 6d70 6c65 6d65 6e74 7320  ally implements 
-00000ea0: 6c6f 6769 630a 2320 4e6f 7465 2074 6861  logic.# Note tha
-00000eb0: 7420 796f 7520 6e65 6564 2074 6f20 696e  t you need to in
-00000ec0: 6865 7269 7420 7468 6520 696d 706c 656d  herit the implem
-00000ed0: 656e 7461 7469 6f6e 2066 726f 6d0a 2320  entation from.# 
-00000ee0: 7468 6520 6073 6e65 616b 7065 656b 2e73  the `sneakpeek.s
-00000ef0: 6372 6170 6572 5f68 616e 646c 6572 2e53  craper_handler.S
-00000f00: 6372 6170 6572 4861 6e64 6c65 7260 0a63  craperHandler`.c
-00000f10: 6c61 7373 2044 656d 6f53 6372 6170 6572  lass DemoScraper
-00000f20: 2853 6372 6170 6572 4861 6e64 6c65 7229  (ScraperHandler)
-00000f30: 3a0a 2020 2020 2320 596f 7520 6361 6e20  :.    # You can 
-00000f40: 6861 7665 2061 6e79 2064 6570 656e 6465  have any depende
-00000f50: 6e63 6965 7320 796f 7520 7761 6e74 2061  ncies you want a
-00000f60: 6e64 2070 6173 7320 7468 656d 0a20 2020  nd pass them.   
-00000f70: 2023 2069 6e20 7468 6520 7365 7276 6572   # in the server
-00000f80: 2063 6f6e 6669 6775 7261 7469 6f6e 0a20   configuration. 
-00000f90: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-00000fa0: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
-00000fb0: 2020 2020 2020 2073 656c 662e 5f6c 6f67         self._log
-00000fc0: 6765 7220 3d20 6c6f 6767 696e 672e 6765  ger = logging.ge
-00000fd0: 744c 6f67 6765 7228 5f5f 6e61 6d65 5f5f  tLogger(__name__
-00000fe0: 290a 0a20 2020 2023 2045 6163 6820 6861  )..    # Each ha
-00000ff0: 6e64 6c65 7220 6d75 7374 2064 6566 696e  ndler must defin
-00001000: 6520 6974 7320 6e61 6d65 2073 6f20 6974  e its name so it
-00001010: 206c 6174 6572 0a20 2020 2023 2063 616e   later.    # can
-00001020: 2062 6520 7265 6665 7265 6e63 6564 2069   be referenced i
-00001030: 6e20 7363 7261 7065 7273 2720 636f 6e66  n scrapers' conf
-00001040: 6967 7572 6174 696f 6e0a 2020 2020 4070  iguration.    @p
-00001050: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-00001060: 6e61 6d65 2873 656c 6629 202d 3e20 7374  name(self) -> st
-00001070: 723a 0a20 2020 2020 2020 2072 6574 7572  r:.        retur
-00001080: 6e20 2264 656d 6f5f 7363 7261 7065 7222  n "demo_scraper"
-00001090: 0a0a 2020 2020 2320 536f 6d65 2065 7861  ..    # Some exa
-000010a0: 6d70 6c65 2066 756e 6374 696f 6e20 7468  mple function th
-000010b0: 6174 2070 726f 6365 7373 6573 2074 6865  at processes the
-000010c0: 2072 6573 706f 6e73 650a 2020 2020 2320   response.    # 
-000010d0: 616e 6420 6578 7472 6163 7473 2076 616c  and extracts val
-000010e0: 7561 626c 6520 696e 666f 726d 6174 696f  uable informatio
-000010f0: 6e0a 2020 2020 6173 796e 6320 6465 6620  n.    async def 
-00001100: 7072 6f63 6573 735f 7061 6765 2873 656c  process_page(sel
-00001110: 662c 2072 6573 706f 6e73 653a 2073 7472  f, response: str
-00001120: 293a 0a20 2020 2020 2020 202e 2e2e 0a0a  ):.        .....
-00001130: 2020 2020 2320 5468 6973 2066 756e 6374      # This funct
-00001140: 696f 6e20 6973 2063 616c 6c65 6420 6279  ion is called by
-00001150: 2074 6865 2077 6f72 6b65 7220 746f 2065   the worker to e
-00001160: 7865 6375 7465 2074 6865 206c 6f67 6963  xecute the logic
-00001170: 0a20 2020 2023 2054 6865 206f 6e6c 7920  .    # The only 
-00001180: 6172 6775 6d65 6e74 2074 6861 7420 6973  argument that is
-00001190: 2070 6173 7365 6420 6973 2060 736e 6561   passed is `snea
-000011a0: 6b70 6565 6b2e 7363 7261 7065 725f 636f  kpeek.scraper_co
-000011b0: 6e74 6578 742e 5363 7261 7065 7243 6f6e  ntext.ScraperCon
-000011c0: 7465 7874 600a 2020 2020 2320 4974 2069  text`.    # It i
-000011d0: 6d70 6c65 6d65 6e74 7320 6261 7369 6320  mplements basic 
-000011e0: 6173 796e 6320 4854 5450 2063 6c69 656e  async HTTP clien
-000011f0: 7420 616e 6420 616c 736f 2070 726f 7669  t and also provi
-00001200: 6465 7320 7061 7261 6d65 7465 7273 0a20  des parameters. 
-00001210: 2020 2023 2074 6861 7420 6172 6520 6465     # that are de
-00001220: 6669 6e65 6420 696e 2074 6865 2073 6372  fined in the scr
-00001230: 6170 6572 2063 6f6e 6669 670a 2020 2020  aper config.    
-00001240: 6173 796e 6320 6465 6620 7275 6e28 7365  async def run(se
-00001250: 6c66 2c20 636f 6e74 6578 743a 2053 6372  lf, context: Scr
-00001260: 6170 6572 436f 6e74 6578 7429 202d 3e20  aperContext) -> 
-00001270: 7374 723a 0a20 2020 2020 2020 2070 6172  str:.        par
-00001280: 616d 7320 3d20 4465 6d6f 5363 7261 7065  ams = DemoScrape
-00001290: 7250 6172 616d 732e 7061 7273 655f 6f62  rParams.parse_ob
-000012a0: 6a28 636f 6e74 6578 742e 7061 7261 6d73  j(context.params
-000012b0: 290a 2020 2020 2020 2020 2320 5065 7266  ).        # Perf
-000012c0: 6f72 6d20 4745 5420 7265 7175 6573 7420  orm GET request 
-000012d0: 746f 2074 6865 2055 524c 2064 6566 696e  to the URL defin
-000012e0: 6564 2069 6e20 7468 6520 7363 7261 7065  ed in the scrape
-000012f0: 7220 636f 6e66 6967 0a20 2020 2020 2020  r config.       
-00001300: 2072 6573 706f 6e73 6520 3d20 6177 6169   response = awai
-00001310: 7420 636f 6e74 6578 742e 6765 7428 7061  t context.get(pa
-00001320: 7261 6d73 2e75 726c 290a 2020 2020 2020  rams.url).      
-00001330: 2020 7265 7370 6f6e 7365 5f62 6f64 7920    response_body 
-00001340: 3d20 6177 6169 7420 7265 7370 6f6e 7365  = await response
-00001350: 2e74 6578 7428 290a 0a20 2020 2020 2020  .text()..       
-00001360: 2023 2050 6572 666f 726d 2073 6f6d 6520   # Perform some 
-00001370: 6275 7369 6e65 7373 206c 6f67 6963 206f  business logic o
-00001380: 6e20 6120 7265 7370 6f6e 7365 0a20 2020  n a response.   
-00001390: 2020 2020 2072 6573 756c 7420 3d20 6177       result = aw
-000013a0: 6169 7420 7365 6c66 2e70 726f 6365 7373  ait self.process
-000013b0: 5f70 6167 6528 7265 7370 6f6e 7365 5f62  _page(response_b
-000013c0: 6f64 7929 0a0a 2020 2020 2020 2020 2320  ody)..        # 
-000013d0: 5265 7475 726e 206d 6561 6e69 6e67 6675  Return meaningfu
-000013e0: 6c20 6a6f 6220 7375 6d6d 6172 7920 2d20  l job summary - 
-000013f0: 6d75 7374 2072 6574 7572 6e20 6120 7374  must return a st
-00001400: 7269 6e67 0a20 2020 2020 2020 2072 6574  ring.        ret
-00001410: 7572 6e20 6a73 6f6e 2e64 756d 7073 287b  urn json.dumps({
-00001420: 0a20 2020 2020 2020 2020 2020 2022 7072  .            "pr
-00001430: 6f63 6573 7365 645f 7572 6c73 223a 2031  ocessed_urls": 1
-00001440: 2c0a 2020 2020 2020 2020 2020 2020 2266  ,.            "f
-00001450: 6f75 6e64 5f72 6573 756c 7473 223a 206c  ound_results": l
-00001460: 656e 2872 6573 756c 7429 2c0a 2020 2020  en(result),.    
-00001470: 2020 2020 7d29 9485 9481 947d 9428 6805      }).....}.(h.
-00001480: 6806 681b 6878 7562 6168 1f7d 9428 6821  h.h.hxubah.}.(h!
-00001490: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
-000014a0: 5d94 6863 6864 6865 8968 668c 0770 7974  ].hchdhe.hf..pyt
-000014b0: 686f 6e33 9468 687d 9475 682b 6853 681d  hon3.hh}.uh+hSh.
-000014c0: 682c 681e 4b0d 681b 680c 681c 6803 7562  h,h.K.h.h.h.h.ub
-000014d0: 682e 2981 947d 9428 6805 8c72 4e6f 7720  h.)..}.(h..rNow 
-000014e0: 7468 6174 2077 6520 6861 7665 2073 6f6d  that we have som
-000014f0: 6520 7363 7261 7065 7220 6c6f 6769 632c  e scraper logic,
-00001500: 206c 6574 2773 206d 616b 6520 6974 2072   let's make it r
-00001510: 756e 2070 6572 696f 6469 6361 6c6c 792e  un periodically.
-00001520: 0a54 6f20 646f 2073 6f20 6c65 7427 7320  .To do so let's 
-00001530: 636f 6e66 6967 7572 6520 2a2a 536e 6561  configure **Snea
-00001540: 6b70 6565 6b53 6572 7665 722a 2a3a 9468  kpeekServer**:.h
-00001550: 075d 9428 6816 8c62 4e6f 7720 7468 6174  .].(h..bNow that
-00001560: 2077 6520 6861 7665 2073 6f6d 6520 7363   we have some sc
-00001570: 7261 7065 7220 6c6f 6769 632c 206c 6574  raper logic, let
-00001580: e280 9973 206d 616b 6520 6974 2072 756e  ...s make it run
-00001590: 2070 6572 696f 6469 6361 6c6c 792e 0a54   periodically..T
-000015a0: 6f20 646f 2073 6f20 6c65 74e2 8099 7320  o do so let...s 
-000015b0: 636f 6e66 6967 7572 6520 9485 9481 947d  configure .....}
-000015c0: 9428 6805 8c5e 4e6f 7720 7468 6174 2077  .(h..^Now that w
-000015d0: 6520 6861 7665 2073 6f6d 6520 7363 7261  e have some scra
-000015e0: 7065 7220 6c6f 6769 632c 206c 6574 2773  per logic, let's
-000015f0: 206d 616b 6520 6974 2072 756e 2070 6572   make it run per
-00001600: 696f 6469 6361 6c6c 792e 0a54 6f20 646f  iodically..To do
-00001610: 2073 6f20 6c65 7427 7320 636f 6e66 6967   so let's config
-00001620: 7572 6520 9468 1b68 8868 1c68 0368 1d4e  ure .h.h.h.h.h.N
-00001630: 681e 4e75 6268 3929 8194 7d94 2868 058c  h.Nubh9)..}.(h..
-00001640: 132a 2a53 6e65 616b 7065 656b 5365 7276  .**SneakpeekServ
-00001650: 6572 2a2a 9468 075d 9468 168c 0f53 6e65  er**.h.].h...Sne
-00001660: 616b 7065 656b 5365 7276 6572 9485 9481  akpeekServer....
-00001670: 947d 9428 6805 6806 681b 6891 681c 6803  .}.(h.h.h.h.h.h.
-00001680: 681d 4e68 1e4e 7562 6168 1f7d 9428 6821  h.Nh.Nubah.}.(h!
-00001690: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
-000016a0: 5d94 7568 2b68 3868 1b68 8875 6268 168c  ].uh+h8h.h.ubh..
-000016b0: 013a 9485 9481 947d 9428 6805 684c 681b  .:.....}.(h.hLh.
-000016c0: 6888 681c 6803 681d 4e68 1e4e 7562 6568  h.h.h.h.Nh.Nubeh
-000016d0: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
-000016e0: 6827 5d94 6829 5d94 7568 2b68 2d68 1d68  h'].h)].uh+h-h.h
-000016f0: 2c68 1e4b 4768 1b68 0c68 1c68 0375 6268  ,h.KGh.h.h.h.ubh
-00001700: 5429 8194 7d94 2868 0558 4009 0000 2320  T)..}.(h.X@...# 
-00001710: 6669 6c65 3a20 6d61 696e 2e70 790a 0a66  file: main.py..f
-00001720: 726f 6d20 736e 6561 6b70 6565 6b2e 6d6f  rom sneakpeek.mo
-00001730: 6465 6c73 2069 6d70 6f72 7420 5363 7261  dels import Scra
-00001740: 7065 722c 2053 6372 6170 6572 4a6f 6250  per, ScraperJobP
-00001750: 7269 6f72 6974 792c 2053 6372 6170 6572  riority, Scraper
-00001760: 5363 6865 6475 6c65 0a66 726f 6d20 736e  Schedule.from sn
-00001770: 6561 6b70 6565 6b2e 7374 6f72 6167 652e  eakpeek.storage.
-00001780: 696e 5f6d 656d 6f72 795f 7374 6f72 6167  in_memory_storag
-00001790: 6520 696d 706f 7274 2028 0a20 2020 2049  e import (.    I
-000017a0: 6e4d 656d 6f72 794c 6561 7365 5374 6f72  nMemoryLeaseStor
-000017b0: 6167 652c 0a20 2020 2049 6e4d 656d 6f72  age,.    InMemor
-000017c0: 7953 6372 6170 6572 4a6f 6273 5374 6f72  yScraperJobsStor
-000017d0: 6167 652c 0a20 2020 2049 6e4d 656d 6f72  age,.    InMemor
-000017e0: 7953 6372 6170 6572 7353 746f 7261 6765  yScrapersStorage
-000017f0: 2c0a 290a 6672 6f6d 2073 6e65 616b 7065  ,.).from sneakpe
-00001800: 656b 2e6c 6f67 6769 6e67 2069 6d70 6f72  ek.logging impor
-00001810: 7420 636f 6e66 6967 7572 655f 6c6f 6767  t configure_logg
-00001820: 696e 670a 6672 6f6d 2073 6e65 616b 7065  ing.from sneakpe
-00001830: 656b 2e70 6c75 6769 6e73 2e72 6571 7565  ek.plugins.reque
-00001840: 7374 735f 6c6f 6767 696e 675f 706c 7567  sts_logging_plug
-00001850: 696e 2069 6d70 6f72 7420 5265 7175 6573  in import Reques
-00001860: 7473 4c6f 6767 696e 6750 6c75 6769 6e0a  tsLoggingPlugin.
-00001870: 6672 6f6d 2073 6e65 616b 7065 656b 2e73  from sneakpeek.s
-00001880: 6372 6170 6572 5f63 6f6e 6669 6720 696d  craper_config im
-00001890: 706f 7274 2053 6372 6170 6572 436f 6e66  port ScraperConf
-000018a0: 6967 0a66 726f 6d20 736e 6561 6b70 6565  ig.from sneakpee
-000018b0: 6b2e 7365 7276 6572 2069 6d70 6f72 7420  k.server import 
-000018c0: 536e 6561 6b70 6565 6b53 6572 7665 720a  SneakpeekServer.
-000018d0: 0a66 726f 6d20 6465 6d6f 5f73 6372 6170  .from demo_scrap
-000018e0: 6572 2069 6d70 6f72 7420 4465 6d6f 5363  er import DemoSc
-000018f0: 7261 7065 720a 0a23 2046 6f72 206e 6f77  raper..# For now
-00001900: 206c 6574 2773 2068 6176 6520 6120 7374   let's have a st
-00001910: 6174 6963 206c 6973 7420 6f66 2073 6372  atic list of scr
-00001920: 6170 6572 730a 2320 6275 7420 7468 6973  apers.# but this
-00001930: 2063 616e 2061 7320 7765 6c6c 2062 6520   can as well be 
-00001940: 6120 6479 6e61 6d69 6320 6c69 7374 2077  a dynamic list w
-00001950: 6869 6368 2069 730a 2320 7374 6f72 6564  hich is.# stored
-00001960: 2069 6e20 736f 6d65 2053 514c 2044 420a   in some SQL DB.
-00001970: 7363 7261 7065 7273 203d 205b 0a20 2020  scrapers = [.   
-00001980: 2053 6372 6170 6572 280a 2020 2020 2020   Scraper(.      
-00001990: 2020 2320 556e 6971 7565 2049 4420 6f66    # Unique ID of
-000019a0: 2074 6865 2073 6372 6170 6572 0a20 2020   the scraper.   
-000019b0: 2020 2020 2069 643d 312c 0a20 2020 2020       id=1,.     
-000019c0: 2020 2023 204e 616d 6520 6f66 2074 6865     # Name of the
-000019d0: 2073 6372 6170 6572 0a20 2020 2020 2020   scraper.       
-000019e0: 206e 616d 653d 6622 4465 6d6f 2053 6372   name=f"Demo Scr
-000019f0: 6170 6572 222c 0a20 2020 2020 2020 2023  aper",.        #
-00001a00: 2048 6f77 2066 7265 7175 656e 7420 7368   How frequent sh
-00001a10: 6f75 6c64 2073 6372 6170 6572 2062 6520  ould scraper be 
-00001a20: 6578 6563 7574 6564 0a20 2020 2020 2020  executed.       
-00001a30: 2073 6368 6564 756c 653d 5363 7261 7065   schedule=Scrape
-00001a40: 7253 6368 6564 756c 652e 4556 4552 595f  rSchedule.EVERY_
-00001a50: 4d49 4e55 5445 2c0a 2020 2020 2020 2020  MINUTE,.        
-00001a60: 2320 4f75 7220 6861 6e64 6c65 7220 6e61  # Our handler na
-00001a70: 6d65 0a20 2020 2020 2020 2068 616e 646c  me.        handl
-00001a80: 6572 3d22 6465 6d6f 5f73 6372 6170 6572  er="demo_scraper
-00001a90: 222c 0a20 2020 2020 2020 2023 2053 6372  ",.        # Scr
-00001aa0: 6170 6572 2063 6f6e 6669 672c 206e 6f74  aper config, not
-00001ab0: 6520 7468 6174 2070 6172 616d 7320 6d75  e that params mu
-00001ac0: 7374 2062 6520 7375 6363 6573 7366 756c  st be successful
-00001ad0: 6c79 0a20 2020 2020 2020 2023 2064 6573  ly.        # des
-00001ae0: 6572 6961 6c69 7a65 6420 696e 746f 2060  erialized into `
-00001af0: 4465 6d6f 5363 7261 7065 7250 6172 616d  DemoScraperParam
-00001b00: 7360 2063 6c61 7373 0a20 2020 2020 2020  s` class.       
-00001b10: 2063 6f6e 6669 673d 5363 7261 7065 7243   config=ScraperC
-00001b20: 6f6e 6669 6728 7061 7261 6d73 3d7b 2275  onfig(params={"u
-00001b30: 726c 223a 2075 726c 7d29 2c0a 2020 2020  rl": url}),.    
-00001b40: 2020 2020 2320 5072 696f 7269 7479 206f      # Priority o
-00001b50: 6620 7468 6520 7065 7269 6f64 6963 2073  f the periodic s
-00001b60: 6372 6170 6572 206a 6f62 732e 0a20 2020  craper jobs..   
-00001b70: 2020 2020 2023 204e 6f74 6520 7468 6174       # Note that
-00001b80: 206d 616e 7561 6c6c 7920 696e 766f 6b65   manually invoke
-00001b90: 6420 6a6f 6273 2061 7265 2061 6c77 6179  d jobs are alway
-00001ba0: 730a 2020 2020 2020 2020 2320 7363 6865  s.        # sche
-00001bb0: 6475 6c65 6420 7769 7468 2060 5554 4d4f  duled with `UTMO
-00001bc0: 5354 6020 7072 696f 7269 7479 0a20 2020  ST` priority.   
-00001bd0: 2020 2020 2073 6368 6564 756c 655f 7072       schedule_pr
-00001be0: 696f 7269 7479 3d53 6372 6170 6572 4a6f  iority=ScraperJo
-00001bf0: 6250 7269 6f72 6974 792e 5554 4d4f 5354  bPriority.UTMOST
-00001c00: 2c0a 2020 2020 290a 5d0a 0a23 2044 6566  ,.    ).]..# Def
-00001c10: 696e 6520 6120 7374 6f72 6167 6520 746f  ine a storage to
-00001c20: 2075 7365 2074 6f20 7374 6f72 6520 7468   use to store th
-00001c30: 6520 6c69 7374 206f 6620 7468 6520 7363  e list of the sc
-00001c40: 7261 7065 7273 0a73 6372 6170 6572 735f  rapers.scrapers_
-00001c50: 7374 6f72 6167 6520 3d20 496e 4d65 6d6f  storage = InMemo
-00001c60: 7279 5363 7261 7065 7273 5374 6f72 6167  ryScrapersStorag
-00001c70: 6528 7363 7261 7065 7273 290a 0a23 2044  e(scrapers)..# D
-00001c80: 6566 696e 6520 6120 6a6f 6273 2073 746f  efine a jobs sto
-00001c90: 7261 6765 2074 6f20 7573 650a 6a6f 6273  rage to use.jobs
-00001ca0: 5f73 746f 7261 6765 203d 2049 6e4d 656d  _storage = InMem
-00001cb0: 6f72 7953 6372 6170 6572 4a6f 6273 5374  oryScraperJobsSt
-00001cc0: 6f72 6167 6528 290a 0a23 2044 6566 696e  orage()..# Defin
-00001cd0: 6520 6120 6c65 6173 6520 7374 6f72 6167  e a lease storag
-00001ce0: 6520 666f 7220 7468 6520 7363 6865 6475  e for the schedu
-00001cf0: 6c65 7220 746f 2065 6e73 7572 650a 2320  ler to ensure.# 
-00001d00: 7468 6174 2061 7420 616e 7920 706f 696e  that at any poin
-00001d10: 7420 6f66 2074 696d 6520 7468 6572 6527  t of time there'
-00001d20: 7320 6f6e 6c79 2031 2061 6374 6976 6520  s only 1 active 
-00001d30: 7363 6865 6475 6c65 722e 0a23 2054 6869  scheduler..# Thi
-00001d40: 7320 656c 696d 696e 6174 6573 2063 6f6e  s eliminates con
-00001d50: 6375 7272 656e 7420 7363 7261 7065 7273  current scrapers
-00001d60: 2065 7865 6375 7469 6f6e 0a6c 6561 7365   execution.lease
-00001d70: 5f73 746f 7261 6765 203d 2049 6e4d 656d  _storage = InMem
-00001d80: 6f72 794c 6561 7365 5374 6f72 6167 6528  oryLeaseStorage(
-00001d90: 290a 0a23 2043 6f6e 6669 6775 7265 2073  )..# Configure s
-00001da0: 6572 7665 720a 7365 7276 6572 203d 2053  erver.server = S
-00001db0: 6e65 616b 7065 656b 5365 7276 6572 2e63  neakpeekServer.c
-00001dc0: 7265 6174 6528 0a20 2020 2023 204c 6973  reate(.    # Lis
-00001dd0: 7420 6f66 2069 6d70 6c65 6d65 6e74 6564  t of implemented
-00001de0: 2073 6372 6170 6572 2068 616e 646c 6572   scraper handler
-00001df0: 730a 2020 2020 6861 6e64 6c65 7273 3d5b  s.    handlers=[
-00001e00: 4465 6d6f 5363 7261 7065 7228 295d 2c0a  DemoScraper()],.
-00001e10: 2020 2020 7363 7261 7065 7273 5f73 746f      scrapers_sto
-00001e20: 7261 6765 3d73 6372 6170 6572 735f 7374  rage=scrapers_st
-00001e30: 6f72 6167 652c 0a20 2020 206a 6f62 735f  orage,.    jobs_
-00001e40: 7374 6f72 6167 653d 6a6f 6273 5f73 746f  storage=jobs_sto
-00001e50: 7261 6765 2c0a 2020 2020 6c65 6173 655f  rage,.    lease_
-00001e60: 7374 6f72 6167 653d 6c65 6173 655f 7374  storage=lease_st
-00001e70: 6f72 6167 652c 0a0a 2020 2020 2320 4c69  orage,..    # Li
-00001e80: 7374 206f 6620 706c 7567 696e 7320 7768  st of plugins wh
-00001e90: 6963 6820 7769 6c6c 2062 6520 696e 766f  ich will be invo
-00001ea0: 6b65 6420 6265 666f 7265 2072 6571 7565  ked before reque
-00001eb0: 7374 0a20 2020 2023 2069 7320 6469 7370  st.    # is disp
-00001ec0: 6174 6368 6564 206f 7220 6166 7465 7220  atched or after 
-00001ed0: 7265 7370 6f6e 7365 2069 7320 7265 6365  response is rece
-00001ee0: 6976 6564 2e0a 2020 2020 2320 496e 2074  ived..    # In t
-00001ef0: 6865 2065 7861 6d70 6c65 2077 6520 7573  he example we us
-00001f00: 6520 6073 6e65 616b 7065 656b 2e70 6c75  e `sneakpeek.plu
-00001f10: 6769 6e73 2e72 6571 7565 7374 735f 6c6f  gins.requests_lo
-00001f20: 6767 696e 675f 706c 7567 696e 2e52 6571  gging_plugin.Req
-00001f30: 7565 7374 734c 6f67 6769 6e67 506c 7567  uestsLoggingPlug
-00001f40: 696e 600a 2020 2020 2320 7768 6963 6820  in`.    # which 
-00001f50: 6c6f 6773 2061 6c6c 2072 6571 7565 7374  logs all request
-00001f60: 7320 616e 6420 7265 7370 6f6e 7365 7320  s and responses 
-00001f70: 6265 696e 6720 6d61 6465 0a20 2020 2070  being made.    p
-00001f80: 6c75 6769 6e73 3d5b 5265 7175 6573 7473  lugins=[Requests
-00001f90: 4c6f 6767 696e 6750 6c75 6769 6e28 295d  LoggingPlugin()]
-00001fa0: 2c0a 290a 0a69 6620 5f5f 6e61 6d65 5f5f  ,.)..if __name__
-00001fb0: 203d 3d20 225f 5f6d 6169 6e5f 5f22 3a0a   == "__main__":.
-00001fc0: 2020 2020 636f 6e66 6967 7572 655f 6c6f      configure_lo
-00001fd0: 6767 696e 6728 290a 2020 2020 2320 5275  gging().    # Ru
-00001fe0: 6e20 7365 7276 6572 2028 7370 6177 6e73  n server (spawns
-00001ff0: 2073 6368 6564 756c 6572 2c20 4150 4920   scheduler, API 
-00002000: 616e 6420 776f 726b 6572 290a 2020 2020  and worker).    
-00002010: 2320 6f70 656e 2068 7474 703a 2f2f 6c6f  # open http://lo
-00002020: 6361 6c68 6f73 743a 3830 3830 2061 6e64  calhost:8080 and
-00002030: 2065 7870 6c6f 7265 2055 490a 2020 2020   explore UI.    
-00002040: 7365 7276 6572 2e73 6572 7665 2829 9468  server.serve().h
-00002050: 075d 9468 1658 4009 0000 2320 6669 6c65  .].h.X@...# file
-00002060: 3a20 6d61 696e 2e70 790a 0a66 726f 6d20  : main.py..from 
-00002070: 736e 6561 6b70 6565 6b2e 6d6f 6465 6c73  sneakpeek.models
-00002080: 2069 6d70 6f72 7420 5363 7261 7065 722c   import Scraper,
-00002090: 2053 6372 6170 6572 4a6f 6250 7269 6f72   ScraperJobPrior
-000020a0: 6974 792c 2053 6372 6170 6572 5363 6865  ity, ScraperSche
-000020b0: 6475 6c65 0a66 726f 6d20 736e 6561 6b70  dule.from sneakp
-000020c0: 6565 6b2e 7374 6f72 6167 652e 696e 5f6d  eek.storage.in_m
-000020d0: 656d 6f72 795f 7374 6f72 6167 6520 696d  emory_storage im
-000020e0: 706f 7274 2028 0a20 2020 2049 6e4d 656d  port (.    InMem
-000020f0: 6f72 794c 6561 7365 5374 6f72 6167 652c  oryLeaseStorage,
-00002100: 0a20 2020 2049 6e4d 656d 6f72 7953 6372  .    InMemoryScr
-00002110: 6170 6572 4a6f 6273 5374 6f72 6167 652c  aperJobsStorage,
-00002120: 0a20 2020 2049 6e4d 656d 6f72 7953 6372  .    InMemoryScr
-00002130: 6170 6572 7353 746f 7261 6765 2c0a 290a  apersStorage,.).
-00002140: 6672 6f6d 2073 6e65 616b 7065 656b 2e6c  from sneakpeek.l
-00002150: 6f67 6769 6e67 2069 6d70 6f72 7420 636f  ogging import co
-00002160: 6e66 6967 7572 655f 6c6f 6767 696e 670a  nfigure_logging.
-00002170: 6672 6f6d 2073 6e65 616b 7065 656b 2e70  from sneakpeek.p
-00002180: 6c75 6769 6e73 2e72 6571 7565 7374 735f  lugins.requests_
-00002190: 6c6f 6767 696e 675f 706c 7567 696e 2069  logging_plugin i
-000021a0: 6d70 6f72 7420 5265 7175 6573 7473 4c6f  mport RequestsLo
-000021b0: 6767 696e 6750 6c75 6769 6e0a 6672 6f6d  ggingPlugin.from
-000021c0: 2073 6e65 616b 7065 656b 2e73 6372 6170   sneakpeek.scrap
-000021d0: 6572 5f63 6f6e 6669 6720 696d 706f 7274  er_config import
-000021e0: 2053 6372 6170 6572 436f 6e66 6967 0a66   ScraperConfig.f
-000021f0: 726f 6d20 736e 6561 6b70 6565 6b2e 7365  rom sneakpeek.se
-00002200: 7276 6572 2069 6d70 6f72 7420 536e 6561  rver import Snea
-00002210: 6b70 6565 6b53 6572 7665 720a 0a66 726f  kpeekServer..fro
-00002220: 6d20 6465 6d6f 5f73 6372 6170 6572 2069  m demo_scraper i
-00002230: 6d70 6f72 7420 4465 6d6f 5363 7261 7065  mport DemoScrape
-00002240: 720a 0a23 2046 6f72 206e 6f77 206c 6574  r..# For now let
-00002250: 2773 2068 6176 6520 6120 7374 6174 6963  's have a static
-00002260: 206c 6973 7420 6f66 2073 6372 6170 6572   list of scraper
-00002270: 730a 2320 6275 7420 7468 6973 2063 616e  s.# but this can
-00002280: 2061 7320 7765 6c6c 2062 6520 6120 6479   as well be a dy
-00002290: 6e61 6d69 6320 6c69 7374 2077 6869 6368  namic list which
-000022a0: 2069 730a 2320 7374 6f72 6564 2069 6e20   is.# stored in 
-000022b0: 736f 6d65 2053 514c 2044 420a 7363 7261  some SQL DB.scra
-000022c0: 7065 7273 203d 205b 0a20 2020 2053 6372  pers = [.    Scr
-000022d0: 6170 6572 280a 2020 2020 2020 2020 2320  aper(.        # 
-000022e0: 556e 6971 7565 2049 4420 6f66 2074 6865  Unique ID of the
-000022f0: 2073 6372 6170 6572 0a20 2020 2020 2020   scraper.       
-00002300: 2069 643d 312c 0a20 2020 2020 2020 2023   id=1,.        #
-00002310: 204e 616d 6520 6f66 2074 6865 2073 6372   Name of the scr
-00002320: 6170 6572 0a20 2020 2020 2020 206e 616d  aper.        nam
-00002330: 653d 6622 4465 6d6f 2053 6372 6170 6572  e=f"Demo Scraper
-00002340: 222c 0a20 2020 2020 2020 2023 2048 6f77  ",.        # How
-00002350: 2066 7265 7175 656e 7420 7368 6f75 6c64   frequent should
-00002360: 2073 6372 6170 6572 2062 6520 6578 6563   scraper be exec
-00002370: 7574 6564 0a20 2020 2020 2020 2073 6368  uted.        sch
-00002380: 6564 756c 653d 5363 7261 7065 7253 6368  edule=ScraperSch
-00002390: 6564 756c 652e 4556 4552 595f 4d49 4e55  edule.EVERY_MINU
-000023a0: 5445 2c0a 2020 2020 2020 2020 2320 4f75  TE,.        # Ou
-000023b0: 7220 6861 6e64 6c65 7220 6e61 6d65 0a20  r handler name. 
-000023c0: 2020 2020 2020 2068 616e 646c 6572 3d22         handler="
-000023d0: 6465 6d6f 5f73 6372 6170 6572 222c 0a20  demo_scraper",. 
-000023e0: 2020 2020 2020 2023 2053 6372 6170 6572         # Scraper
-000023f0: 2063 6f6e 6669 672c 206e 6f74 6520 7468   config, note th
-00002400: 6174 2070 6172 616d 7320 6d75 7374 2062  at params must b
-00002410: 6520 7375 6363 6573 7366 756c 6c79 0a20  e successfully. 
-00002420: 2020 2020 2020 2023 2064 6573 6572 6961         # deseria
-00002430: 6c69 7a65 6420 696e 746f 2060 4465 6d6f  lized into `Demo
-00002440: 5363 7261 7065 7250 6172 616d 7360 2063  ScraperParams` c
-00002450: 6c61 7373 0a20 2020 2020 2020 2063 6f6e  lass.        con
-00002460: 6669 673d 5363 7261 7065 7243 6f6e 6669  fig=ScraperConfi
-00002470: 6728 7061 7261 6d73 3d7b 2275 726c 223a  g(params={"url":
-00002480: 2075 726c 7d29 2c0a 2020 2020 2020 2020   url}),.        
-00002490: 2320 5072 696f 7269 7479 206f 6620 7468  # Priority of th
-000024a0: 6520 7065 7269 6f64 6963 2073 6372 6170  e periodic scrap
-000024b0: 6572 206a 6f62 732e 0a20 2020 2020 2020  er jobs..       
-000024c0: 2023 204e 6f74 6520 7468 6174 206d 616e   # Note that man
-000024d0: 7561 6c6c 7920 696e 766f 6b65 6420 6a6f  ually invoked jo
-000024e0: 6273 2061 7265 2061 6c77 6179 730a 2020  bs are always.  
-000024f0: 2020 2020 2020 2320 7363 6865 6475 6c65        # schedule
-00002500: 6420 7769 7468 2060 5554 4d4f 5354 6020  d with `UTMOST` 
-00002510: 7072 696f 7269 7479 0a20 2020 2020 2020  priority.       
-00002520: 2073 6368 6564 756c 655f 7072 696f 7269   schedule_priori
-00002530: 7479 3d53 6372 6170 6572 4a6f 6250 7269  ty=ScraperJobPri
-00002540: 6f72 6974 792e 5554 4d4f 5354 2c0a 2020  ority.UTMOST,.  
-00002550: 2020 290a 5d0a 0a23 2044 6566 696e 6520    ).]..# Define 
-00002560: 6120 7374 6f72 6167 6520 746f 2075 7365  a storage to use
-00002570: 2074 6f20 7374 6f72 6520 7468 6520 6c69   to store the li
-00002580: 7374 206f 6620 7468 6520 7363 7261 7065  st of the scrape
-00002590: 7273 0a73 6372 6170 6572 735f 7374 6f72  rs.scrapers_stor
-000025a0: 6167 6520 3d20 496e 4d65 6d6f 7279 5363  age = InMemorySc
-000025b0: 7261 7065 7273 5374 6f72 6167 6528 7363  rapersStorage(sc
-000025c0: 7261 7065 7273 290a 0a23 2044 6566 696e  rapers)..# Defin
-000025d0: 6520 6120 6a6f 6273 2073 746f 7261 6765  e a jobs storage
-000025e0: 2074 6f20 7573 650a 6a6f 6273 5f73 746f   to use.jobs_sto
-000025f0: 7261 6765 203d 2049 6e4d 656d 6f72 7953  rage = InMemoryS
-00002600: 6372 6170 6572 4a6f 6273 5374 6f72 6167  craperJobsStorag
-00002610: 6528 290a 0a23 2044 6566 696e 6520 6120  e()..# Define a 
-00002620: 6c65 6173 6520 7374 6f72 6167 6520 666f  lease storage fo
-00002630: 7220 7468 6520 7363 6865 6475 6c65 7220  r the scheduler 
-00002640: 746f 2065 6e73 7572 650a 2320 7468 6174  to ensure.# that
-00002650: 2061 7420 616e 7920 706f 696e 7420 6f66   at any point of
-00002660: 2074 696d 6520 7468 6572 6527 7320 6f6e   time there's on
-00002670: 6c79 2031 2061 6374 6976 6520 7363 6865  ly 1 active sche
-00002680: 6475 6c65 722e 0a23 2054 6869 7320 656c  duler..# This el
-00002690: 696d 696e 6174 6573 2063 6f6e 6375 7272  iminates concurr
-000026a0: 656e 7420 7363 7261 7065 7273 2065 7865  ent scrapers exe
-000026b0: 6375 7469 6f6e 0a6c 6561 7365 5f73 746f  cution.lease_sto
-000026c0: 7261 6765 203d 2049 6e4d 656d 6f72 794c  rage = InMemoryL
-000026d0: 6561 7365 5374 6f72 6167 6528 290a 0a23  easeStorage()..#
-000026e0: 2043 6f6e 6669 6775 7265 2073 6572 7665   Configure serve
-000026f0: 720a 7365 7276 6572 203d 2053 6e65 616b  r.server = Sneak
-00002700: 7065 656b 5365 7276 6572 2e63 7265 6174  peekServer.creat
-00002710: 6528 0a20 2020 2023 204c 6973 7420 6f66  e(.    # List of
-00002720: 2069 6d70 6c65 6d65 6e74 6564 2073 6372   implemented scr
-00002730: 6170 6572 2068 616e 646c 6572 730a 2020  aper handlers.  
-00002740: 2020 6861 6e64 6c65 7273 3d5b 4465 6d6f    handlers=[Demo
-00002750: 5363 7261 7065 7228 295d 2c0a 2020 2020  Scraper()],.    
-00002760: 7363 7261 7065 7273 5f73 746f 7261 6765  scrapers_storage
-00002770: 3d73 6372 6170 6572 735f 7374 6f72 6167  =scrapers_storag
-00002780: 652c 0a20 2020 206a 6f62 735f 7374 6f72  e,.    jobs_stor
-00002790: 6167 653d 6a6f 6273 5f73 746f 7261 6765  age=jobs_storage
-000027a0: 2c0a 2020 2020 6c65 6173 655f 7374 6f72  ,.    lease_stor
-000027b0: 6167 653d 6c65 6173 655f 7374 6f72 6167  age=lease_storag
-000027c0: 652c 0a0a 2020 2020 2320 4c69 7374 206f  e,..    # List o
-000027d0: 6620 706c 7567 696e 7320 7768 6963 6820  f plugins which 
-000027e0: 7769 6c6c 2062 6520 696e 766f 6b65 6420  will be invoked 
-000027f0: 6265 666f 7265 2072 6571 7565 7374 0a20  before request. 
-00002800: 2020 2023 2069 7320 6469 7370 6174 6368     # is dispatch
-00002810: 6564 206f 7220 6166 7465 7220 7265 7370  ed or after resp
-00002820: 6f6e 7365 2069 7320 7265 6365 6976 6564  onse is received
-00002830: 2e0a 2020 2020 2320 496e 2074 6865 2065  ..    # In the e
-00002840: 7861 6d70 6c65 2077 6520 7573 6520 6073  xample we use `s
-00002850: 6e65 616b 7065 656b 2e70 6c75 6769 6e73  neakpeek.plugins
-00002860: 2e72 6571 7565 7374 735f 6c6f 6767 696e  .requests_loggin
-00002870: 675f 706c 7567 696e 2e52 6571 7565 7374  g_plugin.Request
-00002880: 734c 6f67 6769 6e67 506c 7567 696e 600a  sLoggingPlugin`.
-00002890: 2020 2020 2320 7768 6963 6820 6c6f 6773      # which logs
-000028a0: 2061 6c6c 2072 6571 7565 7374 7320 616e   all requests an
-000028b0: 6420 7265 7370 6f6e 7365 7320 6265 696e  d responses bein
-000028c0: 6720 6d61 6465 0a20 2020 2070 6c75 6769  g made.    plugi
-000028d0: 6e73 3d5b 5265 7175 6573 7473 4c6f 6767  ns=[RequestsLogg
-000028e0: 696e 6750 6c75 6769 6e28 295d 2c0a 290a  ingPlugin()],.).
-000028f0: 0a69 6620 5f5f 6e61 6d65 5f5f 203d 3d20  .if __name__ == 
-00002900: 225f 5f6d 6169 6e5f 5f22 3a0a 2020 2020  "__main__":.    
-00002910: 636f 6e66 6967 7572 655f 6c6f 6767 696e  configure_loggin
-00002920: 6728 290a 2020 2020 2320 5275 6e20 7365  g().    # Run se
-00002930: 7276 6572 2028 7370 6177 6e73 2073 6368  rver (spawns sch
-00002940: 6564 756c 6572 2c20 4150 4920 616e 6420  eduler, API and 
-00002950: 776f 726b 6572 290a 2020 2020 2320 6f70  worker).    # op
-00002960: 656e 2068 7474 703a 2f2f 6c6f 6361 6c68  en http://localh
-00002970: 6f73 743a 3830 3830 2061 6e64 2065 7870  ost:8080 and exp
-00002980: 6c6f 7265 2055 490a 2020 2020 7365 7276  lore UI.    serv
-00002990: 6572 2e73 6572 7665 2829 9485 9481 947d  er.serve().....}
-000029a0: 9428 6805 6806 681b 68a9 7562 6168 1f7d  .(h.h.h.h.ubah.}
-000029b0: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
-000029c0: 5d94 6829 5d94 6863 6864 6865 8968 668c  ].h)].hchdhe.hf.
-000029d0: 0770 7974 686f 6e33 9468 687d 9475 682b  .python3.hh}.uh+
-000029e0: 6853 681d 682c 681e 4b4a 681b 680c 681c  hSh.h,h.KJh.h.h.
-000029f0: 6803 7562 682e 2981 947d 9428 6805 8c3a  h.ubh.)..}.(h..:
-00002a00: 4e6f 772c 2074 6865 206f 6e6c 7920 7468  Now, the only th
-00002a10: 696e 6720 6973 206c 6566 7420 6973 2074  ing is left is t
-00002a20: 6f20 6163 7475 616c 6c79 2072 756e 2074  o actually run t
-00002a30: 6865 2073 6572 7665 723a 9468 075d 9468  he server:.h.].h
-00002a40: 168c 3a4e 6f77 2c20 7468 6520 6f6e 6c79  ..:Now, the only
-00002a50: 2074 6869 6e67 2069 7320 6c65 6674 2069   thing is left i
-00002a60: 7320 746f 2061 6374 7561 6c6c 7920 7275  s to actually ru
-00002a70: 6e20 7468 6520 7365 7276 6572 3a94 8594  n the server:...
-00002a80: 8194 7d94 2868 0568 bb68 1b68 b968 1c68  ..}.(h.h.h.h.h.h
-00002a90: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
-00002aa0: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
-00002ab0: 295d 9475 682b 682d 681d 682c 681e 4b92  )].uh+h-h.h,h.K.
-00002ac0: 681b 680c 681c 6803 7562 6854 2981 947d  h.h.h.h.ubhT)..}
-00002ad0: 9428 6805 8c13 7079 7468 6f6e 3320 7275  .(h...python3 ru
-00002ae0: 6e20 6d61 696e 2e70 7994 6807 5d94 6816  n main.py.h.].h.
-00002af0: 8c13 7079 7468 6f6e 3320 7275 6e20 6d61  ..python3 run ma
-00002b00: 696e 2e70 7994 8594 8194 7d94 2868 0568  in.py.....}.(h.h
-00002b10: 0668 1b68 c775 6261 681f 7d94 2868 215d  .h.h.ubah.}.(h!]
-00002b20: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
-00002b30: 9468 6368 6468 6589 6866 8c04 6261 7368  .hchdhe.hf..bash
-00002b40: 9468 687d 9475 682b 6853 681d 682c 681e  .hh}.uh+hSh.h,h.
-00002b50: 4b94 681b 680c 681c 6803 7562 682e 2981  K.h.h.h.h.ubh.).
-00002b60: 947d 9428 6805 8c8a 5468 6174 2773 2069  .}.(h...That's i
-00002b70: 7421 204e 6f77 2079 6f75 2063 616e 206f  t! Now you can o
-00002b80: 7065 6e20 6874 7470 3a2f 2f6c 6f63 616c  pen http://local
-00002b90: 686f 7374 3a38 3038 3020 616e 6420 6578  host:8080 and ex
-00002ba0: 706c 6f72 6520 7468 6520 5549 2074 6f20  plore the UI to 
-00002bb0: 7365 650a 686f 7720 796f 7520 7363 7261  see.how you scra
-00002bc0: 7065 7220 6973 2062 6569 6e67 2061 7574  per is being aut
-00002bd0: 6f6d 6174 6963 616c 6c79 2073 6368 6564  omatically sched
-00002be0: 756c 6564 2061 6e64 2065 7865 6375 7465  uled and execute
-00002bf0: 642e 9468 075d 9428 6816 8c1e 5468 6174  d..h.].(h...That
-00002c00: e280 9973 2069 7421 204e 6f77 2079 6f75  ...s it! Now you
-00002c10: 2063 616e 206f 7065 6e20 9485 9481 947d   can open .....}
-00002c20: 9428 6805 8c1c 5468 6174 2773 2069 7421  .(h...That's it!
-00002c30: 204e 6f77 2079 6f75 2063 616e 206f 7065   Now you can ope
-00002c40: 6e20 9468 1b68 d768 1c68 0368 1d4e 681e  n .h.h.h.h.h.Nh.
-00002c50: 4e75 6268 098c 0972 6566 6572 656e 6365  Nubh...reference
-00002c60: 9493 9429 8194 7d94 2868 058c 1568 7474  ...)..}.(h...htt
-00002c70: 703a 2f2f 6c6f 6361 6c68 6f73 743a 3830  p://localhost:80
-00002c80: 3830 9468 075d 9468 168c 1568 7474 703a  80.h.].h...http:
-00002c90: 2f2f 6c6f 6361 6c68 6f73 743a 3830 3830  //localhost:8080
-00002ca0: 9485 9481 947d 9428 6805 6806 681b 68e2  .....}.(h.h.h.h.
-00002cb0: 681c 6803 681d 4e68 1e4e 7562 6168 1f7d  h.h.h.Nh.Nubah.}
-00002cc0: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
-00002cd0: 5d94 6829 5d94 8c06 7265 6675 7269 9468  ].h)]...refuri.h
-00002ce0: e475 682b 68e0 681b 68d7 7562 6816 8c59  .uh+h.h.h.ubh..Y
-00002cf0: 2061 6e64 2065 7870 6c6f 7265 2074 6865   and explore the
-00002d00: 2055 4920 746f 2073 6565 0a68 6f77 2079   UI to see.how y
-00002d10: 6f75 2073 6372 6170 6572 2069 7320 6265  ou scraper is be
-00002d20: 696e 6720 6175 746f 6d61 7469 6361 6c6c  ing automaticall
-00002d30: 7920 7363 6865 6475 6c65 6420 616e 6420  y scheduled and 
-00002d40: 6578 6563 7574 6564 2e94 8594 8194 7d94  executed......}.
-00002d50: 2868 058c 5920 616e 6420 6578 706c 6f72  (h..Y and explor
-00002d60: 6520 7468 6520 5549 2074 6f20 7365 650a  e the UI to see.
-00002d70: 686f 7720 796f 7520 7363 7261 7065 7220  how you scraper 
-00002d80: 6973 2062 6569 6e67 2061 7574 6f6d 6174  is being automat
-00002d90: 6963 616c 6c79 2073 6368 6564 756c 6564  ically scheduled
-00002da0: 2061 6e64 2065 7865 6375 7465 642e 9468   and executed..h
-00002db0: 1b68 d768 1c68 0368 1d4e 681e 4e75 6265  .h.h.h.h.Nh.Nube
-00002dc0: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
-00002dd0: 9468 275d 9468 295d 9475 682b 682d 681d  .h'].h)].uh+h-h.
-00002de0: 682c 681e 4b98 681b 680c 681c 6803 7562  h,h.K.h.h.h.h.ub
-00002df0: 6568 1f7d 9428 6821 5d94 8c0b 7175 6963  eh.}.(h!]...quic
-00002e00: 6b2d 7374 6172 7494 6168 235d 9468 255d  k-start.ah#].h%]
-00002e10: 948c 0b71 7569 636b 2073 7461 7274 9461  ...quick start.a
-00002e20: 6827 5d94 6829 5d94 7568 2b68 0a68 1b68  h'].h)].uh+h.h.h
-00002e30: 0368 1c68 0368 1d68 2c68 1e4b 0375 6261  .h.h.h.h,h.K.uba
-00002e40: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
-00002e50: 9468 275d 9468 295d 948c 0673 6f75 7263  .h'].h)]...sourc
-00002e60: 6594 682c 7568 2b68 018c 0e63 7572 7265  e.h,uh+h...curre
-00002e70: 6e74 5f73 6f75 7263 6594 4e8c 0c63 7572  nt_source.N..cur
-00002e80: 7265 6e74 5f6c 696e 6594 4e8c 0873 6574  rent_line.N..set
-00002e90: 7469 6e67 7394 8c11 646f 6375 7469 6c73  tings...docutils
-00002ea0: 2e66 726f 6e74 656e 6494 8c06 5661 6c75  .frontend...Valu
-00002eb0: 6573 9493 9429 8194 7d94 2868 0f4e 8c09  es...)..}.(h.N..
-00002ec0: 6765 6e65 7261 746f 7294 4e8c 0964 6174  generator.N..dat
-00002ed0: 6573 7461 6d70 944e 8c0b 736f 7572 6365  estamp.N..source
-00002ee0: 5f6c 696e 6b94 4e8c 0a73 6f75 7263 655f  _link.N..source_
-00002ef0: 7572 6c94 4e8c 0d74 6f63 5f62 6163 6b6c  url.N..toc_backl
-00002f00: 696e 6b73 948c 0565 6e74 7279 948c 1266  inks...entry...f
-00002f10: 6f6f 746e 6f74 655f 6261 636b 6c69 6e6b  ootnote_backlink
-00002f20: 7394 4b01 8c0d 7365 6374 6e75 6d5f 7866  s.K...sectnum_xf
-00002f30: 6f72 6d94 4b01 8c0e 7374 7269 705f 636f  orm.K...strip_co
-00002f40: 6d6d 656e 7473 944e 8c1b 7374 7269 705f  mments.N..strip_
-00002f50: 656c 656d 656e 7473 5f77 6974 685f 636c  elements_with_cl
-00002f60: 6173 7365 7394 4e8c 0d73 7472 6970 5f63  asses.N..strip_c
-00002f70: 6c61 7373 6573 944e 8c0c 7265 706f 7274  lasses.N..report
-00002f80: 5f6c 6576 656c 944b 028c 0a68 616c 745f  _level.K...halt_
-00002f90: 6c65 7665 6c94 4b05 8c11 6578 6974 5f73  level.K...exit_s
-00002fa0: 7461 7475 735f 6c65 7665 6c94 4b05 8c05  tatus_level.K...
-00002fb0: 6465 6275 6794 4e8c 0e77 6172 6e69 6e67  debug.N..warning
-00002fc0: 5f73 7472 6561 6d94 4e8c 0974 7261 6365  _stream.N..trace
-00002fd0: 6261 636b 9488 8c0e 696e 7075 745f 656e  back....input_en
-00002fe0: 636f 6469 6e67 948c 0975 7466 2d38 2d73  coding...utf-8-s
-00002ff0: 6967 948c 1c69 6e70 7574 5f65 6e63 6f64  ig...input_encod
-00003000: 696e 675f 6572 726f 725f 6861 6e64 6c65  ing_error_handle
-00003010: 7294 8c06 7374 7269 6374 948c 0f6f 7574  r...strict...out
-00003020: 7075 745f 656e 636f 6469 6e67 948c 0575  put_encoding...u
-00003030: 7466 2d38 948c 1d6f 7574 7075 745f 656e  tf-8...output_en
-00003040: 636f 6469 6e67 5f65 7272 6f72 5f68 616e  coding_error_han
-00003050: 646c 6572 946a 2701 0000 8c0e 6572 726f  dler.j'.....erro
-00003060: 725f 656e 636f 6469 6e67 948c 0575 7466  r_encoding...utf
-00003070: 2d38 948c 1c65 7272 6f72 5f65 6e63 6f64  -8...error_encod
-00003080: 696e 675f 6572 726f 725f 6861 6e64 6c65  ing_error_handle
-00003090: 7294 8c10 6261 636b 736c 6173 6872 6570  r...backslashrep
-000030a0: 6c61 6365 948c 0d6c 616e 6775 6167 655f  lace...language_
-000030b0: 636f 6465 948c 0265 6e94 8c13 7265 636f  code...en...reco
-000030c0: 7264 5f64 6570 656e 6465 6e63 6965 7394  rd_dependencies.
-000030d0: 4e8c 0663 6f6e 6669 6794 4e8c 0969 645f  N..config.N..id_
-000030e0: 7072 6566 6978 9468 068c 0e61 7574 6f5f  prefix.h...auto_
-000030f0: 6964 5f70 7265 6669 7894 8c02 6964 948c  id_prefix...id..
-00003100: 0d64 756d 705f 7365 7474 696e 6773 944e  .dump_settings.N
-00003110: 8c0e 6475 6d70 5f69 6e74 6572 6e61 6c73  ..dump_internals
-00003120: 944e 8c0f 6475 6d70 5f74 7261 6e73 666f  .N..dump_transfo
-00003130: 726d 7394 4e8c 0f64 756d 705f 7073 6575  rms.N..dump_pseu
-00003140: 646f 5f78 6d6c 944e 8c10 6578 706f 7365  do_xml.N..expose
-00003150: 5f69 6e74 6572 6e61 6c73 944e 8c0e 7374  _internals.N..st
-00003160: 7269 6374 5f76 6973 6974 6f72 944e 8c0f  rict_visitor.N..
-00003170: 5f64 6973 6162 6c65 5f63 6f6e 6669 6794  _disable_config.
-00003180: 4e8c 075f 736f 7572 6365 9468 2c8c 0c5f  N.._source.h,.._
-00003190: 6465 7374 696e 6174 696f 6e94 4e8c 0d5f  destination.N.._
-000031a0: 636f 6e66 6967 5f66 696c 6573 945d 948c  config_files.]..
-000031b0: 1666 696c 655f 696e 7365 7274 696f 6e5f  .file_insertion_
-000031c0: 656e 6162 6c65 6494 888c 0b72 6177 5f65  enabled....raw_e
-000031d0: 6e61 626c 6564 944b 018c 116c 696e 655f  nabled.K...line_
-000031e0: 6c65 6e67 7468 5f6c 696d 6974 944d 1027  length_limit.M.'
-000031f0: 8c0e 7065 705f 7265 6665 7265 6e63 6573  ..pep_references
-00003200: 944e 8c0c 7065 705f 6261 7365 5f75 726c  .N..pep_base_url
-00003210: 948c 2068 7474 7073 3a2f 2f77 7777 2e70  .. https://www.p
-00003220: 7974 686f 6e2e 6f72 672f 6465 762f 7065  ython.org/dev/pe
-00003230: 7073 2f94 8c15 7065 705f 6669 6c65 5f75  ps/...pep_file_u
-00003240: 726c 5f74 656d 706c 6174 6594 8c08 7065  rl_template...pe
-00003250: 702d 2530 3464 948c 0e72 6663 5f72 6566  p-%04d...rfc_ref
-00003260: 6572 656e 6365 7394 4e8c 0c72 6663 5f62  erences.N..rfc_b
-00003270: 6173 655f 7572 6c94 8c1c 6874 7470 733a  ase_url...https:
-00003280: 2f2f 746f 6f6c 732e 6965 7466 2e6f 7267  //tools.ietf.org
-00003290: 2f68 746d 6c2f 948c 0974 6162 5f77 6964  /html/...tab_wid
-000032a0: 7468 944b 088c 1d74 7269 6d5f 666f 6f74  th.K...trim_foot
-000032b0: 6e6f 7465 5f72 6566 6572 656e 6365 5f73  note_reference_s
-000032c0: 7061 6365 9489 8c10 7379 6e74 6178 5f68  pace....syntax_h
-000032d0: 6967 686c 6967 6874 948c 046c 6f6e 6794  ighlight...long.
-000032e0: 8c0c 736d 6172 745f 7175 6f74 6573 9488  ..smart_quotes..
-000032f0: 8c13 736d 6172 7471 756f 7465 735f 6c6f  ..smartquotes_lo
-00003300: 6361 6c65 7394 5d94 8c1d 6368 6172 6163  cales.]...charac
-00003310: 7465 725f 6c65 7665 6c5f 696e 6c69 6e65  ter_level_inline
-00003320: 5f6d 6172 6b75 7094 898c 0e64 6f63 7469  _markup....docti
-00003330: 746c 655f 7866 6f72 6d94 898c 0d64 6f63  tle_xform....doc
-00003340: 696e 666f 5f78 666f 726d 944b 018c 1273  info_xform.K...s
-00003350: 6563 7473 7562 7469 746c 655f 7866 6f72  ectsubtitle_xfor
-00003360: 6d94 898c 1065 6d62 6564 5f73 7479 6c65  m....embed_style
-00003370: 7368 6565 7494 898c 1563 6c6f 616b 5f65  sheet....cloak_e
-00003380: 6d61 696c 5f61 6464 7265 7373 6573 9488  mail_addresses..
-00003390: 8c03 656e 7694 4e75 628c 0872 6570 6f72  ..env.Nub..repor
-000033a0: 7465 7294 4e8c 1069 6e64 6972 6563 745f  ter.N..indirect_
-000033b0: 7461 7267 6574 7394 5d94 8c11 7375 6273  targets.]...subs
-000033c0: 7469 7475 7469 6f6e 5f64 6566 7394 7d94  titution_defs.}.
-000033d0: 8c12 7375 6273 7469 7475 7469 6f6e 5f6e  ..substitution_n
-000033e0: 616d 6573 947d 948c 0872 6566 6e61 6d65  ames.}...refname
-000033f0: 7394 7d94 8c06 7265 6669 6473 947d 948c  s.}...refids.}..
-00003400: 076e 616d 6569 6473 947d 946a 0101 0000  .nameids.}.j....
-00003410: 68fe 738c 096e 616d 6574 7970 6573 947d  h.s..nametypes.}
-00003420: 946a 0101 0000 4e73 6821 7d94 68fe 680c  .j....Nsh!}.h.h.
-00003430: 738c 0d66 6f6f 746e 6f74 655f 7265 6673  s..footnote_refs
-00003440: 947d 948c 0d63 6974 6174 696f 6e5f 7265  .}...citation_re
-00003450: 6673 947d 948c 0d61 7574 6f66 6f6f 746e  fs.}...autofootn
-00003460: 6f74 6573 945d 948c 1161 7574 6f66 6f6f  otes.]...autofoo
-00003470: 746e 6f74 655f 7265 6673 945d 948c 1073  tnote_refs.]...s
-00003480: 796d 626f 6c5f 666f 6f74 6e6f 7465 7394  ymbol_footnotes.
-00003490: 5d94 8c14 7379 6d62 6f6c 5f66 6f6f 746e  ]...symbol_footn
-000034a0: 6f74 655f 7265 6673 945d 948c 0966 6f6f  ote_refs.]...foo
-000034b0: 746e 6f74 6573 945d 948c 0963 6974 6174  tnotes.]...citat
-000034c0: 696f 6e73 945d 948c 1261 7574 6f66 6f6f  ions.]...autofoo
-000034d0: 746e 6f74 655f 7374 6172 7494 4b01 8c15  tnote_start.K...
-000034e0: 7379 6d62 6f6c 5f66 6f6f 746e 6f74 655f  symbol_footnote_
-000034f0: 7374 6172 7494 4b00 8c0a 6964 5f63 6f75  start.K...id_cou
-00003500: 6e74 6572 948c 0b63 6f6c 6c65 6374 696f  nter...collectio
-00003510: 6e73 948c 0743 6f75 6e74 6572 9493 947d  ns...Counter...}
-00003520: 9485 9452 948c 0e70 6172 7365 5f6d 6573  ...R...parse_mes
-00003530: 7361 6765 7394 5d94 8c12 7472 616e 7366  sages.]...transf
-00003540: 6f72 6d5f 6d65 7373 6167 6573 945d 948c  orm_messages.]..
-00003550: 0b74 7261 6e73 666f 726d 6572 944e 8c0b  .transformer.N..
-00003560: 696e 636c 7564 655f 6c6f 6794 5d94 8c0a  include_log.]...
-00003570: 6465 636f 7261 7469 6f6e 944e 681c 6803  decoration.Nh.h.
-00003580: 7562 2e                                  ub.
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 736e 6561  : 2.1.Name: snea
+00000020: 6b70 6565 6b2d 7079 0a56 6572 7369 6f6e  kpeek-py.Version
+00000030: 3a20 302e 322e 310a 5375 6d6d 6172 793a  : 0.2.1.Summary:
+00000040: 2053 6e65 616b 7065 656b 2069 7320 6120   Sneakpeek is a 
+00000050: 6672 616d 6577 6f72 6b20 7468 6174 2068  framework that h
+00000060: 656c 7073 2074 6f20 7175 6963 6b6c 7920  elps to quickly 
+00000070: 616e 6420 636f 6e76 696e 6965 6e74 6c79  and conviniently
+00000080: 2064 6576 656c 6f70 2073 6372 6170 6572   develop scraper
+00000090: 732e 2049 7427 7320 7468 6520 6265 7374  s. It's the best
+000000a0: 2063 686f 6963 6520 666f 7220 7363 7261   choice for scra
+000000b0: 7065 7273 2074 6861 7420 6861 7665 2073  pers that have s
+000000c0: 6f6d 6520 7370 6563 6966 6963 2063 6f6d  ome specific com
+000000d0: 706c 6578 2073 6372 6170 696e 6720 6c6f  plex scraping lo
+000000e0: 6769 6320 7468 6174 206e 6565 6473 2074  gic that needs t
+000000f0: 6f20 6265 2072 756e 206f 6e20 6120 636f  o be run on a co
+00000100: 6e73 7461 6e74 2062 6173 6973 2e0a 486f  nstant basis..Ho
+00000110: 6d65 2d70 6167 653a 2068 7474 7073 3a2f  me-page: https:/
+00000120: 2f67 6974 6875 622e 636f 6d2f 666c 756c  /github.com/flul
+00000130: 656d 6f6e 2f73 6e65 616b 7065 656b 0a4c  emon/sneakpeek.L
+00000140: 6963 656e 7365 3a20 4253 442d 332d 436c  icense: BSD-3-Cl
+00000150: 6175 7365 0a41 7574 686f 723a 2044 616e  ause.Author: Dan
+00000160: 2059 617a 6f76 736b 790a 4175 7468 6f72   Yazovsky.Author
+00000170: 2d65 6d61 696c 3a20 6461 6e69 696c 2e79  -email: daniil.y
+00000180: 617a 6f76 736b 7940 676d 6169 6c2e 636f  azovsky@gmail.co
+00000190: 6d0a 4d61 696e 7461 696e 6572 3a20 4461  m.Maintainer: Da
+000001a0: 6e20 5961 7a6f 7673 6b79 0a4d 6169 6e74  n Yazovsky.Maint
+000001b0: 6169 6e65 722d 656d 6169 6c3a 2064 616e  ainer-email: dan
+000001c0: 6969 6c2e 7961 7a6f 7673 6b79 4067 6d61  iil.yazovsky@gma
+000001d0: 696c 2e63 6f6d 0a52 6571 7569 7265 732d  il.com.Requires-
+000001e0: 5079 7468 6f6e 3a20 3e3d 332e 3130 2c3c  Python: >=3.10,<
+000001f0: 342e 300a 436c 6173 7369 6669 6572 3a20  4.0.Classifier: 
+00000200: 4465 7665 6c6f 706d 656e 7420 5374 6174  Development Stat
+00000210: 7573 203a 3a20 3220 2d20 5072 652d 416c  us :: 2 - Pre-Al
+00000220: 7068 610a 436c 6173 7369 6669 6572 3a20  pha.Classifier: 
+00000230: 4672 616d 6577 6f72 6b20 3a3a 2046 6173  Framework :: Fas
+00000240: 7441 5049 0a43 6c61 7373 6966 6965 723a  tAPI.Classifier:
+00000250: 2046 7261 6d65 776f 726b 203a 3a20 5079   Framework :: Py
+00000260: 6461 6e74 6963 0a43 6c61 7373 6966 6965  dantic.Classifie
+00000270: 723a 2049 6e74 656e 6465 6420 4175 6469  r: Intended Audi
+00000280: 656e 6365 203a 3a20 4465 7665 6c6f 7065  ence :: Develope
+00000290: 7273 0a43 6c61 7373 6966 6965 723a 204c  rs.Classifier: L
+000002a0: 6963 656e 7365 203a 3a20 4f53 4920 4170  icense :: OSI Ap
+000002b0: 7072 6f76 6564 203a 3a20 4253 4420 4c69  proved :: BSD Li
+000002c0: 6365 6e73 650a 436c 6173 7369 6669 6572  cense.Classifier
+000002d0: 3a20 4f70 6572 6174 696e 6720 5379 7374  : Operating Syst
+000002e0: 656d 203a 3a20 4f53 2049 6e64 6570 656e  em :: OS Indepen
+000002f0: 6465 6e74 0a43 6c61 7373 6966 6965 723a  dent.Classifier:
+00000300: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
+00000310: 6775 6167 6520 3a3a 2050 7974 686f 6e0a  guage :: Python.
+00000320: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
+00000330: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000340: 203a 3a20 5079 7468 6f6e 203a 3a20 330a   :: Python :: 3.
+00000350: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
+00000360: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000370: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+00000380: 3130 0a43 6c61 7373 6966 6965 723a 2050  10.Classifier: P
+00000390: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+000003a0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+000003b0: 2033 2e31 310a 436c 6173 7369 6669 6572   3.11.Classifier
+000003c0: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
+000003d0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+000003e0: 203a 3a20 330a 436c 6173 7369 6669 6572   :: 3.Classifier
+000003f0: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
+00000400: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000410: 203a 3a20 332e 3130 0a43 6c61 7373 6966   :: 3.10.Classif
+00000420: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
+00000430: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+00000440: 686f 6e20 3a3a 2033 2e31 310a 436c 6173  hon :: 3.11.Clas
+00000450: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
+00000460: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000470: 5079 7468 6f6e 203a 3a20 332e 3132 0a43  Python :: 3.12.C
+00000480: 6c61 7373 6966 6965 723a 2054 6f70 6963  lassifier: Topic
+00000490: 203a 3a20 496e 7465 726e 6574 203a 3a20   :: Internet :: 
+000004a0: 5757 572f 4854 5450 203a 3a20 496e 6465  WWW/HTTP :: Inde
+000004b0: 7869 6e67 2f53 6561 7263 680a 436c 6173  xing/Search.Clas
+000004c0: 7369 6669 6572 3a20 546f 7069 6320 3a3a  sifier: Topic ::
+000004d0: 2053 6f66 7477 6172 6520 4465 7665 6c6f   Software Develo
+000004e0: 706d 656e 7420 3a3a 204c 6962 7261 7269  pment :: Librari
+000004f0: 6573 203a 3a20 4170 706c 6963 6174 696f  es :: Applicatio
+00000500: 6e20 4672 616d 6577 6f72 6b73 0a50 726f  n Frameworks.Pro
+00000510: 7669 6465 732d 4578 7472 613a 2064 6f63  vides-Extra: doc
+00000520: 730a 5265 7175 6972 6573 2d44 6973 743a  s.Requires-Dist:
+00000530: 2053 7068 696e 7820 283d 3d34 2e32 2e30   Sphinx (==4.2.0
+00000540: 2920 3b20 6578 7472 6120 3d3d 2022 646f  ) ; extra == "do
+00000550: 6373 220a 5265 7175 6972 6573 2d44 6973  cs".Requires-Dis
+00000560: 743a 2061 696f 6874 7470 2028 3e3d 332e  t: aiohttp (>=3.
+00000570: 382e 342c 3c34 2e30 2e30 290a 5265 7175  8.4,<4.0.0).Requ
+00000580: 6972 6573 2d44 6973 743a 2061 7073 6368  ires-Dist: apsch
+00000590: 6564 756c 6572 2028 3e3d 332e 3130 2e31  eduler (>=3.10.1
+000005a0: 2c3c 342e 302e 3029 0a52 6571 7569 7265  ,<4.0.0).Require
+000005b0: 732d 4469 7374 3a20 6361 6368 6574 6f6f  s-Dist: cachetoo
+000005c0: 6c73 2028 3e3d 352e 332e 302c 3c36 2e30  ls (>=5.3.0,<6.0
+000005d0: 2e30 290a 5265 7175 6972 6573 2d44 6973  .0).Requires-Dis
+000005e0: 743a 2066 616b 652d 7573 6572 6167 656e  t: fake-useragen
+000005f0: 7420 283e 3d31 2e31 2e33 2c3c 322e 302e  t (>=1.1.3,<2.0.
+00000600: 3029 0a52 6571 7569 7265 732d 4469 7374  0).Requires-Dist
+00000610: 3a20 6661 7374 6170 6920 283e 3d30 2e39  : fastapi (>=0.9
+00000620: 352e 302c 3c30 2e39 362e 3029 0a52 6571  5.0,<0.96.0).Req
+00000630: 7569 7265 732d 4469 7374 3a20 6661 7374  uires-Dist: fast
+00000640: 6170 692d 6a73 6f6e 7270 6320 283e 3d32  api-jsonrpc (>=2
+00000650: 2e34 2e31 2c3c 332e 302e 3029 0a52 6571  .4.1,<3.0.0).Req
+00000660: 7569 7265 732d 4469 7374 3a20 7072 6f6d  uires-Dist: prom
+00000670: 6574 6865 7573 2d63 6c69 656e 7420 283e  etheus-client (>
+00000680: 3d30 2e31 362e 302c 3c30 2e31 372e 3029  =0.16.0,<0.17.0)
+00000690: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+000006a0: 7079 6461 6e74 6963 2028 3e3d 312e 3130  pydantic (>=1.10
+000006b0: 2e37 2c3c 322e 302e 3029 0a52 6571 7569  .7,<2.0.0).Requi
+000006c0: 7265 732d 4469 7374 3a20 7265 6469 7320  res-Dist: redis 
+000006d0: 283e 3d34 2e35 2e34 2c3c 352e 302e 3029  (>=4.5.4,<5.0.0)
+000006e0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+000006f0: 7370 6869 6e78 2d72 7464 2d74 6865 6d65  sphinx-rtd-theme
+00000700: 2028 3d3d 312e 302e 3029 203b 2065 7874   (==1.0.0) ; ext
+00000710: 7261 203d 3d20 2264 6f63 7322 0a52 6571  ra == "docs".Req
+00000720: 7569 7265 732d 4469 7374 3a20 7370 6869  uires-Dist: sphi
+00000730: 6e78 636f 6e74 7269 622d 6e61 706f 6c65  nxcontrib-napole
+00000740: 6f6e 2028 3d3d 302e 3729 203b 2065 7874  on (==0.7) ; ext
+00000750: 7261 203d 3d20 2264 6f63 7322 0a52 6571  ra == "docs".Req
+00000760: 7569 7265 732d 4469 7374 3a20 7576 6963  uires-Dist: uvic
+00000770: 6f72 6e20 283e 3d30 2e32 312e 312c 3c30  orn (>=0.21.1,<0
+00000780: 2e32 322e 3029 0a52 6571 7569 7265 732d  .22.0).Requires-
+00000790: 4469 7374 3a20 7961 726c 2028 3e3d 312e  Dist: yarl (>=1.
+000007a0: 392e 312c 3c32 2e30 2e30 290a 5072 6f6a  9.1,<2.0.0).Proj
+000007b0: 6563 742d 5552 4c3a 2044 6f63 756d 656e  ect-URL: Documen
+000007c0: 7461 7469 6f6e 2c20 6874 7470 733a 2f2f  tation, https://
+000007d0: 736e 6561 6b70 6565 6b2d 7079 2e72 6561  sneakpeek-py.rea
+000007e0: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
+000007f0: 6174 6573 742f 0a50 726f 6a65 6374 2d55  atest/.Project-U
+00000800: 524c 3a20 5265 706f 7369 746f 7279 2c20  RL: Repository, 
+00000810: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000820: 6f6d 2f66 6c75 6c65 6d6f 6e2f 736e 6561  om/flulemon/snea
+00000830: 6b70 6565 6b0a 4465 7363 7269 7074 696f  kpeek.Descriptio
+00000840: 6e2d 436f 6e74 656e 742d 5479 7065 3a20  n-Content-Type: 
+00000850: 7465 7874 2f6d 6172 6b64 6f77 6e0a 0a23  text/markdown..#
+00000860: 2053 6e65 616b 7065 656b 0a0a 215b 4349   Sneakpeek..![CI
+00000870: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000880: 2e63 6f6d 2f66 6c75 6c65 6d6f 6e2f 736e  .com/flulemon/sn
+00000890: 6561 6b70 6565 6b2f 6163 7469 6f6e 732f  eakpeek/actions/
+000008a0: 776f 726b 666c 6f77 732f 6369 2e79 6d6c  workflows/ci.yml
+000008b0: 2f62 6164 6765 2e73 7667 290a 5b21 5b50  /badge.svg).[![P
+000008c0: 7950 4920 7665 7273 696f 6e5d 2868 7474  yPI version](htt
+000008d0: 7073 3a2f 2f62 6164 6765 2e66 7572 792e  ps://badge.fury.
+000008e0: 696f 2f70 792f 736e 6561 6b70 6565 6b2d  io/py/sneakpeek-
+000008f0: 7079 2e73 7667 295d 2868 7474 7073 3a2f  py.svg)](https:/
+00000900: 2f62 6164 6765 2e66 7572 792e 696f 2f70  /badge.fury.io/p
+00000910: 792f 736e 6561 6b70 6565 6b2d 7079 290a  y/sneakpeek-py).
+00000920: 5b21 5b44 6f77 6e6c 6f61 6473 5d28 6874  [![Downloads](ht
+00000930: 7470 733a 2f2f 7374 6174 6963 2e70 6570  tps://static.pep
+00000940: 792e 7465 6368 2f62 6164 6765 2f73 6e65  y.tech/badge/sne
+00000950: 616b 7065 656b 2d70 7929 5d28 6874 7470  akpeek-py)](http
+00000960: 733a 2f2f 7065 7079 2e74 6563 682f 7072  s://pepy.tech/pr
+00000970: 6f6a 6563 742f 736e 6561 6b70 6565 6b2d  oject/sneakpeek-
+00000980: 7079 290a 5b21 5b44 6f63 756d 656e 7461  py).[![Documenta
+00000990: 7469 6f6e 2053 7461 7475 735d 2868 7474  tion Status](htt
+000009a0: 7073 3a2f 2f72 6561 6474 6865 646f 6373  ps://readthedocs
+000009b0: 2e6f 7267 2f70 726f 6a65 6374 732f 736e  .org/projects/sn
+000009c0: 6561 6b70 6565 6b2d 7079 2f62 6164 6765  eakpeek-py/badge
+000009d0: 2f3f 7665 7273 696f 6e3d 6c61 7465 7374  /?version=latest
+000009e0: 295d 2868 7474 7073 3a2f 2f73 6e65 616b  )](https://sneak
+000009f0: 7065 656b 2d70 792e 7265 6164 7468 6564  peek-py.readthed
+00000a00: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
+00000a10: 2f3f 6261 6467 653d 6c61 7465 7374 290a  /?badge=latest).
+00000a20: 5b21 5b63 6f64 6563 6f76 5d28 6874 7470  [![codecov](http
+00000a30: 733a 2f2f 636f 6465 636f 762e 696f 2f67  s://codecov.io/g
+00000a40: 682f 666c 756c 656d 6f6e 2f73 6e65 616b  h/flulemon/sneak
+00000a50: 7065 656b 2f62 7261 6e63 682f 6d61 696e  peek/branch/main
+00000a60: 2f67 7261 7068 2f62 6164 6765 2e73 7667  /graph/badge.svg
+00000a70: 3f74 6f6b 656e 3d37 6834 3550 3871 4852  ?token=7h45P8qHR
+00000a80: 4729 5d28 6874 7470 733a 2f2f 636f 6465  G)](https://code
+00000a90: 636f 762e 696f 2f67 682f 666c 756c 656d  cov.io/gh/flulem
+00000aa0: 6f6e 2f73 6e65 616b 7065 656b 290a 0a2a  on/sneakpeek)..*
+00000ab0: 2a53 6e65 616b 7065 656b 2a2a 202d 2069  *Sneakpeek** - i
+00000ac0: 7320 6120 6672 616d 6577 6f72 6b20 7468  s a framework th
+00000ad0: 6174 2068 656c 7073 2074 6f20 7175 6963  at helps to quic
+00000ae0: 6b6c 7920 616e 6420 636f 6e76 696e 6965  kly and convinie
+00000af0: 6e74 6c79 2064 6576 656c 6f70 2073 6372  ntly develop scr
+00000b00: 6170 6572 732e 0a49 7427 7320 7468 6520  apers..It's the 
+00000b10: 6265 7374 2063 686f 6963 6520 666f 7220  best choice for 
+00000b20: 7363 7261 7065 7273 2074 6861 7420 6861  scrapers that ha
+00000b30: 7665 2073 6f6d 6520 7370 6563 6966 6963  ve some specific
+00000b40: 2063 6f6d 706c 6578 2073 6372 6170 696e   complex scrapin
+00000b50: 6720 6c6f 6769 6320 7468 6174 206e 6565  g logic that nee
+00000b60: 6473 0a74 6f20 6265 2072 756e 206f 6e20  ds.to be run on 
+00000b70: 6120 636f 6e73 7461 6e74 2062 6173 6973  a constant basis
+00000b80: 2e0a 0a23 2320 4465 6d6f 0a0a 5b48 6572  ...## Demo..[Her
+00000b90: 6527 7320 6120 6465 6d6f 2070 726f 6a65  e's a demo proje
+00000ba0: 6374 5d28 6874 7470 733a 2f2f 6769 7468  ct](https://gith
+00000bb0: 7562 2e63 6f6d 2f66 6c75 6c65 6d6f 6e2f  ub.com/flulemon/
+00000bc0: 736e 6561 6b70 6565 6b2d 6465 6d6f 2920  sneakpeek-demo) 
+00000bd0: 7768 6963 6820 7573 6573 202a 2a53 6e65  which uses **Sne
+00000be0: 616b 7065 656b 2a2a 2066 7261 6d65 776f  akpeek** framewo
+00000bf0: 726b 2e0a 0a59 6f75 2063 616e 2061 6c73  rk...You can als
+00000c00: 6f20 7275 6e20 7468 6520 6465 6d6f 2075  o run the demo u
+00000c10: 7369 6e67 2044 6f63 6b65 723a 0a0a 6060  sing Docker:..``
+00000c20: 6062 6173 680a 646f 636b 6572 2072 756e  `bash.docker run
+00000c30: 202d 6974 202d 2d72 6d20 2d70 2038 3038   -it --rm -p 808
+00000c40: 303a 3830 3830 2066 6c75 6c65 6d6f 6e2f  0:8080 flulemon/
+00000c50: 736e 6561 6b70 6565 6b2d 6465 6d6f 0a60  sneakpeek-demo.`
+00000c60: 6060 0a0a 4f6e 6365 2069 7420 6861 7320  ``..Once it has 
+00000c70: 7374 6172 7465 6420 6865 6164 206f 7665  started head ove
+00000c80: 7220 746f 2068 7474 703a 2f2f 6c6f 6361  r to http://loca
+00000c90: 6c68 6f73 743a 3830 3830 2074 6f20 706c  lhost:8080 to pl
+00000ca0: 6179 2061 726f 756e 6420 7769 7468 2069  ay around with i
+00000cb0: 742e 0a0a 2323 2051 7569 636b 2073 7461  t...## Quick sta
+00000cc0: 7274 0a0a 536f 2079 6f75 2077 616e 7420  rt..So you want 
+00000cd0: 746f 2063 7265 6174 6520 6120 6e65 7720  to create a new 
+00000ce0: 7363 7261 7065 722c 2066 6972 7374 2079  scraper, first y
+00000cf0: 6f75 206e 6565 6420 746f 206d 616b 6520  ou need to make 
+00000d00: 7375 7265 2079 6f75 0a68 6176 6520 696e  sure you.have in
+00000d10: 7374 616c 6c65 6420 2a2a 536e 6561 6b70  stalled **Sneakp
+00000d20: 6565 6b2a 2a3a 0a0a 6060 6062 6173 680a  eek**:..```bash.
+00000d30: 7069 7020 696e 7374 616c 6c20 736e 6561  pip install snea
+00000d40: 6b70 6565 6b2d 7079 0a60 6060 0a0a 5468  kpeek-py.```..Th
+00000d50: 6520 6e65 7874 2073 7465 7020 776f 756c  e next step woul
+00000d60: 6420 6265 2069 6d70 6c65 6d65 6e74 696e  d be implementin
+00000d70: 6720 7363 7261 7065 7220 6c6f 6769 6320  g scraper logic 
+00000d80: 286f 7220 736f 2063 616c 6c65 6420 7363  (or so called sc
+00000d90: 7261 7065 720a 6861 6e64 6c65 7229 3a0a  raper.handler):.
+00000da0: 0a60 6060 7079 7468 6f6e 330a 2320 6669  .```python3.# fi
+00000db0: 6c65 3a20 6465 6d6f 5f73 6372 6170 6572  le: demo_scraper
+00000dc0: 2e70 790a 0a69 6d70 6f72 7420 6a73 6f6e  .py..import json
+00000dd0: 0a69 6d70 6f72 7420 6c6f 6767 696e 670a  .import logging.
+00000de0: 0a66 726f 6d20 7079 6461 6e74 6963 2069  .from pydantic i
+00000df0: 6d70 6f72 7420 4261 7365 4d6f 6465 6c0a  mport BaseModel.
+00000e00: 0a66 726f 6d20 736e 6561 6b70 6565 6b2e  .from sneakpeek.
+00000e10: 7363 7261 7065 725f 636f 6e74 6578 7420  scraper_context 
+00000e20: 696d 706f 7274 2053 6372 6170 6572 436f  import ScraperCo
+00000e30: 6e74 6578 740a 6672 6f6d 2073 6e65 616b  ntext.from sneak
+00000e40: 7065 656b 2e73 6372 6170 6572 5f68 616e  peek.scraper_han
+00000e50: 646c 6572 2069 6d70 6f72 7420 5363 7261  dler import Scra
+00000e60: 7065 7248 616e 646c 6572 0a0a 0a23 2054  perHandler...# T
+00000e70: 6869 7320 6465 6669 6e65 7320 6d6f 6465  his defines mode
+00000e80: 6c20 6f66 2068 616e 646c 6572 2070 6172  l of handler par
+00000e90: 616d 6574 6572 7320 7468 6174 2061 7265  ameters that are
+00000ea0: 2064 6566 696e 6564 0a23 2069 6e20 7468   defined.# in th
+00000eb0: 6520 7363 7261 7065 7220 636f 6e66 6967  e scraper config
+00000ec0: 2061 6e64 2074 6865 6e20 7061 7373 6564   and then passed
+00000ed0: 2074 6f20 7468 6520 6861 6e64 6c65 720a   to the handler.
+00000ee0: 636c 6173 7320 4465 6d6f 5363 7261 7065  class DemoScrape
+00000ef0: 7250 6172 616d 7328 4261 7365 4d6f 6465  rParams(BaseMode
+00000f00: 6c29 3a0a 2020 2020 7572 6c3a 2073 7472  l):.    url: str
+00000f10: 0a0a 2320 5468 6973 2069 7320 6120 636c  ..# This is a cl
+00000f20: 6173 7320 7768 6963 6820 6163 7475 616c  ass which actual
+00000f30: 6c79 2069 6d70 6c65 6d65 6e74 7320 6c6f  ly implements lo
+00000f40: 6769 630a 2320 4e6f 7465 2074 6861 7420  gic.# Note that 
+00000f50: 796f 7520 6e65 6564 2074 6f20 696e 6865  you need to inhe
+00000f60: 7269 7420 7468 6520 696d 706c 656d 656e  rit the implemen
+00000f70: 7461 7469 6f6e 2066 726f 6d0a 2320 7468  tation from.# th
+00000f80: 6520 6073 6e65 616b 7065 656b 2e73 6372  e `sneakpeek.scr
+00000f90: 6170 6572 5f68 616e 646c 6572 2e53 6372  aper_handler.Scr
+00000fa0: 6170 6572 4861 6e64 6c65 7260 0a63 6c61  aperHandler`.cla
+00000fb0: 7373 2044 656d 6f53 6372 6170 6572 2853  ss DemoScraper(S
+00000fc0: 6372 6170 6572 4861 6e64 6c65 7229 3a0a  craperHandler):.
+00000fd0: 2020 2020 2320 596f 7520 6361 6e20 6861      # You can ha
+00000fe0: 7665 2061 6e79 2064 6570 656e 6465 6e63  ve any dependenc
+00000ff0: 6965 7320 796f 7520 7761 6e74 2061 6e64  ies you want and
+00001000: 2070 6173 7320 7468 656d 0a20 2020 2023   pass them.    #
+00001010: 2069 6e20 7468 6520 7365 7276 6572 2063   in the server c
+00001020: 6f6e 6669 6775 7261 7469 6f6e 0a20 2020  onfiguration.   
+00001030: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
+00001040: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
+00001050: 2020 2020 2073 656c 662e 5f6c 6f67 6765       self._logge
+00001060: 7220 3d20 6c6f 6767 696e 672e 6765 744c  r = logging.getL
+00001070: 6f67 6765 7228 5f5f 6e61 6d65 5f5f 290a  ogger(__name__).
+00001080: 0a20 2020 2023 2045 6163 6820 6861 6e64  .    # Each hand
+00001090: 6c65 7220 6d75 7374 2064 6566 696e 6520  ler must define 
+000010a0: 6974 7320 6e61 6d65 2073 6f20 6974 206c  its name so it l
+000010b0: 6174 6572 0a20 2020 2023 2063 616e 2062  ater.    # can b
+000010c0: 6520 7265 6665 7265 6e63 6564 2069 6e20  e referenced in 
+000010d0: 7363 7261 7065 7273 2720 636f 6e66 6967  scrapers' config
+000010e0: 7572 6174 696f 6e0a 2020 2020 4070 726f  uration.    @pro
+000010f0: 7065 7274 790a 2020 2020 6465 6620 6e61  perty.    def na
+00001100: 6d65 2873 656c 6629 202d 3e20 7374 723a  me(self) -> str:
+00001110: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00001120: 2264 656d 6f5f 7363 7261 7065 7222 0a0a  "demo_scraper"..
+00001130: 2020 2020 2320 536f 6d65 2065 7861 6d70      # Some examp
+00001140: 6c65 2066 756e 6374 696f 6e20 7468 6174  le function that
+00001150: 2070 726f 6365 7373 6573 2074 6865 2072   processes the r
+00001160: 6573 706f 6e73 650a 2020 2020 2320 616e  esponse.    # an
+00001170: 6420 6578 7472 6163 7473 2076 616c 7561  d extracts valua
+00001180: 626c 6520 696e 666f 726d 6174 696f 6e0a  ble information.
+00001190: 2020 2020 6173 796e 6320 6465 6620 7072      async def pr
+000011a0: 6f63 6573 735f 7061 6765 2873 656c 662c  ocess_page(self,
+000011b0: 2072 6573 706f 6e73 653a 2073 7472 293a   response: str):
+000011c0: 0a20 2020 2020 2020 202e 2e2e 0a0a 2020  .        .....  
+000011d0: 2020 2320 5468 6973 2066 756e 6374 696f    # This functio
+000011e0: 6e20 6973 2063 616c 6c65 6420 6279 2074  n is called by t
+000011f0: 6865 2077 6f72 6b65 7220 746f 2065 7865  he worker to exe
+00001200: 6375 7465 2074 6865 206c 6f67 6963 0a20  cute the logic. 
+00001210: 2020 2023 2054 6865 206f 6e6c 7920 6172     # The only ar
+00001220: 6775 6d65 6e74 2074 6861 7420 6973 2070  gument that is p
+00001230: 6173 7365 6420 6973 2060 736e 6561 6b70  assed is `sneakp
+00001240: 6565 6b2e 7363 7261 7065 725f 636f 6e74  eek.scraper_cont
+00001250: 6578 742e 5363 7261 7065 7243 6f6e 7465  ext.ScraperConte
+00001260: 7874 600a 2020 2020 2320 4974 2069 6d70  xt`.    # It imp
+00001270: 6c65 6d65 6e74 7320 6261 7369 6320 6173  lements basic as
+00001280: 796e 6320 4854 5450 2063 6c69 656e 7420  ync HTTP client 
+00001290: 616e 6420 616c 736f 2070 726f 7669 6465  and also provide
+000012a0: 7320 7061 7261 6d65 7465 7273 0a20 2020  s parameters.   
+000012b0: 2023 2074 6861 7420 6172 6520 6465 6669   # that are defi
+000012c0: 6e65 6420 696e 2074 6865 2073 6372 6170  ned in the scrap
+000012d0: 6572 2063 6f6e 6669 670a 2020 2020 6173  er config.    as
+000012e0: 796e 6320 6465 6620 7275 6e28 7365 6c66  ync def run(self
+000012f0: 2c20 636f 6e74 6578 743a 2053 6372 6170  , context: Scrap
+00001300: 6572 436f 6e74 6578 7429 202d 3e20 7374  erContext) -> st
+00001310: 723a 0a20 2020 2020 2020 2070 6172 616d  r:.        param
+00001320: 7320 3d20 4465 6d6f 5363 7261 7065 7250  s = DemoScraperP
+00001330: 6172 616d 732e 7061 7273 655f 6f62 6a28  arams.parse_obj(
+00001340: 636f 6e74 6578 742e 7061 7261 6d73 290a  context.params).
+00001350: 2020 2020 2020 2020 2320 5065 7266 6f72          # Perfor
+00001360: 6d20 4745 5420 7265 7175 6573 7420 746f  m GET request to
+00001370: 2074 6865 2055 524c 2064 6566 696e 6564   the URL defined
+00001380: 2069 6e20 7468 6520 7363 7261 7065 7220   in the scraper 
+00001390: 636f 6e66 6967 0a20 2020 2020 2020 2072  config.        r
+000013a0: 6573 706f 6e73 6520 3d20 6177 6169 7420  esponse = await 
+000013b0: 636f 6e74 6578 742e 6765 7428 7061 7261  context.get(para
+000013c0: 6d73 2e75 726c 290a 2020 2020 2020 2020  ms.url).        
+000013d0: 7265 7370 6f6e 7365 5f62 6f64 7920 3d20  response_body = 
+000013e0: 6177 6169 7420 7265 7370 6f6e 7365 2e74  await response.t
+000013f0: 6578 7428 290a 0a20 2020 2020 2020 2023  ext()..        #
+00001400: 2050 6572 666f 726d 2073 6f6d 6520 6275   Perform some bu
+00001410: 7369 6e65 7373 206c 6f67 6963 206f 6e20  siness logic on 
+00001420: 6120 7265 7370 6f6e 7365 0a20 2020 2020  a response.     
+00001430: 2020 2072 6573 756c 7420 3d20 6177 6169     result = awai
+00001440: 7420 7365 6c66 2e70 726f 6365 7373 5f70  t self.process_p
+00001450: 6167 6528 7265 7370 6f6e 7365 5f62 6f64  age(response_bod
+00001460: 7929 0a0a 2020 2020 2020 2020 2320 5265  y)..        # Re
+00001470: 7475 726e 206d 6561 6e69 6e67 6675 6c20  turn meaningful 
+00001480: 6a6f 6220 7375 6d6d 6172 7920 2d20 6d75  job summary - mu
+00001490: 7374 2072 6574 7572 6e20 6120 7374 7269  st return a stri
+000014a0: 6e67 0a20 2020 2020 2020 2072 6574 7572  ng.        retur
+000014b0: 6e20 6a73 6f6e 2e64 756d 7073 287b 0a20  n json.dumps({. 
+000014c0: 2020 2020 2020 2020 2020 2022 7072 6f63             "proc
+000014d0: 6573 7365 645f 7572 6c73 223a 2031 2c0a  essed_urls": 1,.
+000014e0: 2020 2020 2020 2020 2020 2020 2266 6f75              "fou
+000014f0: 6e64 5f72 6573 756c 7473 223a 206c 656e  nd_results": len
+00001500: 2872 6573 756c 7429 2c0a 2020 2020 2020  (result),.      
+00001510: 2020 7d29 0a60 6060 0a0a 4e6f 7720 7468    }).```..Now th
+00001520: 6174 2077 6520 6861 7665 2073 6f6d 6520  at we have some 
+00001530: 7363 7261 7065 7220 6c6f 6769 632c 206c  scraper logic, l
+00001540: 6574 5c27 7320 6d61 6b65 2069 7420 7275  et\'s make it ru
+00001550: 6e20 7065 7269 6f64 6963 616c 6c79 2e20  n periodically. 
+00001560: 546f 0a64 6f20 736f 206c 6574 5c27 7320  To.do so let\'s 
+00001570: 636f 6e66 6967 7572 6520 2a2a 536e 6561  configure **Snea
+00001580: 6b70 6565 6b53 6572 7665 722a 2a3a 0a0a  kpeekServer**:..
+00001590: 6060 6070 7974 686f 6e33 0a23 2066 696c  ```python3.# fil
+000015a0: 653a 206d 6169 6e2e 7079 0a0a 6672 6f6d  e: main.py..from
+000015b0: 2073 6e65 616b 7065 656b 2e6d 6f64 656c   sneakpeek.model
+000015c0: 7320 696d 706f 7274 2053 6372 6170 6572  s import Scraper
+000015d0: 2c20 5363 7261 7065 724a 6f62 5072 696f  , ScraperJobPrio
+000015e0: 7269 7479 2c20 5363 7261 7065 7253 6368  rity, ScraperSch
+000015f0: 6564 756c 650a 6672 6f6d 2073 6e65 616b  edule.from sneak
+00001600: 7065 656b 2e73 746f 7261 6765 2e69 6e5f  peek.storage.in_
+00001610: 6d65 6d6f 7279 5f73 746f 7261 6765 2069  memory_storage i
+00001620: 6d70 6f72 7420 280a 2020 2020 496e 4d65  mport (.    InMe
+00001630: 6d6f 7279 4c65 6173 6553 746f 7261 6765  moryLeaseStorage
+00001640: 2c0a 2020 2020 496e 4d65 6d6f 7279 5363  ,.    InMemorySc
+00001650: 7261 7065 724a 6f62 7353 746f 7261 6765  raperJobsStorage
+00001660: 2c0a 2020 2020 496e 4d65 6d6f 7279 5363  ,.    InMemorySc
+00001670: 7261 7065 7273 5374 6f72 6167 652c 0a29  rapersStorage,.)
+00001680: 0a66 726f 6d20 736e 6561 6b70 6565 6b2e  .from sneakpeek.
+00001690: 6c6f 6767 696e 6720 696d 706f 7274 2063  logging import c
+000016a0: 6f6e 6669 6775 7265 5f6c 6f67 6769 6e67  onfigure_logging
+000016b0: 0a66 726f 6d20 736e 6561 6b70 6565 6b2e  .from sneakpeek.
+000016c0: 706c 7567 696e 732e 7265 7175 6573 7473  plugins.requests
+000016d0: 5f6c 6f67 6769 6e67 5f70 6c75 6769 6e20  _logging_plugin 
+000016e0: 696d 706f 7274 2052 6571 7565 7374 734c  import RequestsL
+000016f0: 6f67 6769 6e67 506c 7567 696e 0a66 726f  oggingPlugin.fro
+00001700: 6d20 736e 6561 6b70 6565 6b2e 7363 7261  m sneakpeek.scra
+00001710: 7065 725f 636f 6e66 6967 2069 6d70 6f72  per_config impor
+00001720: 7420 5363 7261 7065 7243 6f6e 6669 670a  t ScraperConfig.
+00001730: 6672 6f6d 2073 6e65 616b 7065 656b 2e73  from sneakpeek.s
+00001740: 6572 7665 7220 696d 706f 7274 2053 6e65  erver import Sne
+00001750: 616b 7065 656b 5365 7276 6572 0a0a 6672  akpeekServer..fr
+00001760: 6f6d 2064 656d 6f5f 7363 7261 7065 7220  om demo_scraper 
+00001770: 696d 706f 7274 2044 656d 6f53 6372 6170  import DemoScrap
+00001780: 6572 0a0a 2320 466f 7220 6e6f 7720 6c65  er..# For now le
+00001790: 7427 7320 6861 7665 2061 2073 7461 7469  t's have a stati
+000017a0: 6320 6c69 7374 206f 6620 7363 7261 7065  c list of scrape
+000017b0: 7273 0a23 2062 7574 2074 6869 7320 6361  rs.# but this ca
+000017c0: 6e20 6173 2077 656c 6c20 6265 2061 2064  n as well be a d
+000017d0: 796e 616d 6963 206c 6973 7420 7768 6963  ynamic list whic
+000017e0: 6820 6973 0a23 2073 746f 7265 6420 696e  h is.# stored in
+000017f0: 2073 6f6d 6520 5351 4c20 4442 0a73 6372   some SQL DB.scr
+00001800: 6170 6572 7320 3d20 5b0a 2020 2020 5363  apers = [.    Sc
+00001810: 7261 7065 7228 0a20 2020 2020 2020 2023  raper(.        #
+00001820: 2055 6e69 7175 6520 4944 206f 6620 7468   Unique ID of th
+00001830: 6520 7363 7261 7065 720a 2020 2020 2020  e scraper.      
+00001840: 2020 6964 3d31 2c0a 2020 2020 2020 2020    id=1,.        
+00001850: 2320 4e61 6d65 206f 6620 7468 6520 7363  # Name of the sc
+00001860: 7261 7065 720a 2020 2020 2020 2020 6e61  raper.        na
+00001870: 6d65 3d66 2244 656d 6f20 5363 7261 7065  me=f"Demo Scrape
+00001880: 7222 2c0a 2020 2020 2020 2020 2320 486f  r",.        # Ho
+00001890: 7720 6672 6571 7565 6e74 2073 686f 756c  w frequent shoul
+000018a0: 6420 7363 7261 7065 7220 6265 2065 7865  d scraper be exe
+000018b0: 6375 7465 640a 2020 2020 2020 2020 7363  cuted.        sc
+000018c0: 6865 6475 6c65 3d53 6372 6170 6572 5363  hedule=ScraperSc
+000018d0: 6865 6475 6c65 2e45 5645 5259 5f4d 494e  hedule.EVERY_MIN
+000018e0: 5554 452c 0a20 2020 2020 2020 2023 204f  UTE,.        # O
+000018f0: 7572 2068 616e 646c 6572 206e 616d 650a  ur handler name.
+00001900: 2020 2020 2020 2020 6861 6e64 6c65 723d          handler=
+00001910: 2264 656d 6f5f 7363 7261 7065 7222 2c0a  "demo_scraper",.
+00001920: 2020 2020 2020 2020 2320 5363 7261 7065          # Scrape
+00001930: 7220 636f 6e66 6967 2c20 6e6f 7465 2074  r config, note t
+00001940: 6861 7420 7061 7261 6d73 206d 7573 7420  hat params must 
+00001950: 6265 2073 7563 6365 7373 6675 6c6c 790a  be successfully.
+00001960: 2020 2020 2020 2020 2320 6465 7365 7269          # deseri
+00001970: 616c 697a 6564 2069 6e74 6f20 6044 656d  alized into `Dem
+00001980: 6f53 6372 6170 6572 5061 7261 6d73 6020  oScraperParams` 
+00001990: 636c 6173 730a 2020 2020 2020 2020 636f  class.        co
+000019a0: 6e66 6967 3d53 6372 6170 6572 436f 6e66  nfig=ScraperConf
+000019b0: 6967 2870 6172 616d 733d 7b22 7572 6c22  ig(params={"url"
+000019c0: 3a20 7572 6c7d 292c 0a20 2020 2020 2020  : url}),.       
+000019d0: 2023 2050 7269 6f72 6974 7920 6f66 2074   # Priority of t
+000019e0: 6865 2070 6572 696f 6469 6320 7363 7261  he periodic scra
+000019f0: 7065 7220 6a6f 6273 2e0a 2020 2020 2020  per jobs..      
+00001a00: 2020 2320 4e6f 7465 2074 6861 7420 6d61    # Note that ma
+00001a10: 6e75 616c 6c79 2069 6e76 6f6b 6564 206a  nually invoked j
+00001a20: 6f62 7320 6172 6520 616c 7761 7973 0a20  obs are always. 
+00001a30: 2020 2020 2020 2023 2073 6368 6564 756c         # schedul
+00001a40: 6564 2077 6974 6820 6055 544d 4f53 5460  ed with `UTMOST`
+00001a50: 2070 7269 6f72 6974 790a 2020 2020 2020   priority.      
+00001a60: 2020 7363 6865 6475 6c65 5f70 7269 6f72    schedule_prior
+00001a70: 6974 793d 5363 7261 7065 724a 6f62 5072  ity=ScraperJobPr
+00001a80: 696f 7269 7479 2e55 544d 4f53 542c 0a20  iority.UTMOST,. 
+00001a90: 2020 2029 0a5d 0a0a 2320 4465 6669 6e65     ).]..# Define
+00001aa0: 2061 2073 746f 7261 6765 2074 6f20 7573   a storage to us
+00001ab0: 6520 746f 2073 746f 7265 2074 6865 206c  e to store the l
+00001ac0: 6973 7420 6f66 2074 6865 2073 6372 6170  ist of the scrap
+00001ad0: 6572 730a 7363 7261 7065 7273 5f73 746f  ers.scrapers_sto
+00001ae0: 7261 6765 203d 2049 6e4d 656d 6f72 7953  rage = InMemoryS
+00001af0: 6372 6170 6572 7353 746f 7261 6765 2873  crapersStorage(s
+00001b00: 6372 6170 6572 7329 0a0a 2320 4465 6669  crapers)..# Defi
+00001b10: 6e65 2061 206a 6f62 7320 7374 6f72 6167  ne a jobs storag
+00001b20: 6520 746f 2075 7365 0a6a 6f62 735f 7374  e to use.jobs_st
+00001b30: 6f72 6167 6520 3d20 496e 4d65 6d6f 7279  orage = InMemory
+00001b40: 5363 7261 7065 724a 6f62 7353 746f 7261  ScraperJobsStora
+00001b50: 6765 2829 0a0a 2320 4465 6669 6e65 2061  ge()..# Define a
+00001b60: 206c 6561 7365 2073 746f 7261 6765 2066   lease storage f
+00001b70: 6f72 2074 6865 2073 6368 6564 756c 6572  or the scheduler
+00001b80: 2074 6f20 656e 7375 7265 0a23 2074 6861   to ensure.# tha
+00001b90: 7420 6174 2061 6e79 2070 6f69 6e74 206f  t at any point o
+00001ba0: 6620 7469 6d65 2074 6865 7265 2773 206f  f time there's o
+00001bb0: 6e6c 7920 3120 6163 7469 7665 2073 6368  nly 1 active sch
+00001bc0: 6564 756c 6572 2e0a 2320 5468 6973 2065  eduler..# This e
+00001bd0: 6c69 6d69 6e61 7465 7320 636f 6e63 7572  liminates concur
+00001be0: 7265 6e74 2073 6372 6170 6572 7320 6578  rent scrapers ex
+00001bf0: 6563 7574 696f 6e0a 6c65 6173 655f 7374  ecution.lease_st
+00001c00: 6f72 6167 6520 3d20 496e 4d65 6d6f 7279  orage = InMemory
+00001c10: 4c65 6173 6553 746f 7261 6765 2829 0a0a  LeaseStorage()..
+00001c20: 2320 436f 6e66 6967 7572 6520 7365 7276  # Configure serv
+00001c30: 6572 0a73 6572 7665 7220 3d20 536e 6561  er.server = Snea
+00001c40: 6b70 6565 6b53 6572 7665 722e 6372 6561  kpeekServer.crea
+00001c50: 7465 280a 2020 2020 2320 4c69 7374 206f  te(.    # List o
+00001c60: 6620 696d 706c 656d 656e 7465 6420 7363  f implemented sc
+00001c70: 7261 7065 7220 6861 6e64 6c65 7273 0a20  raper handlers. 
+00001c80: 2020 2068 616e 646c 6572 733d 5b44 656d     handlers=[Dem
+00001c90: 6f53 6372 6170 6572 2829 5d2c 0a20 2020  oScraper()],.   
+00001ca0: 2073 6372 6170 6572 735f 7374 6f72 6167   scrapers_storag
+00001cb0: 653d 7363 7261 7065 7273 5f73 746f 7261  e=scrapers_stora
+00001cc0: 6765 2c0a 2020 2020 6a6f 6273 5f73 746f  ge,.    jobs_sto
+00001cd0: 7261 6765 3d6a 6f62 735f 7374 6f72 6167  rage=jobs_storag
+00001ce0: 652c 0a20 2020 206c 6561 7365 5f73 746f  e,.    lease_sto
+00001cf0: 7261 6765 3d6c 6561 7365 5f73 746f 7261  rage=lease_stora
+00001d00: 6765 2c0a 0a20 2020 2023 204c 6973 7420  ge,..    # List 
+00001d10: 6f66 2070 6c75 6769 6e73 2077 6869 6368  of plugins which
+00001d20: 2077 696c 6c20 6265 2069 6e76 6f6b 6564   will be invoked
+00001d30: 2062 6566 6f72 6520 7265 7175 6573 740a   before request.
+00001d40: 2020 2020 2320 6973 2064 6973 7061 7463      # is dispatc
+00001d50: 6865 6420 6f72 2061 6674 6572 2072 6573  hed or after res
+00001d60: 706f 6e73 6520 6973 2072 6563 6569 7665  ponse is receive
+00001d70: 642e 0a20 2020 2023 2049 6e20 7468 6520  d..    # In the 
+00001d80: 6578 616d 706c 6520 7765 2075 7365 2060  example we use `
+00001d90: 736e 6561 6b70 6565 6b2e 706c 7567 696e  sneakpeek.plugin
+00001da0: 732e 7265 7175 6573 7473 5f6c 6f67 6769  s.requests_loggi
+00001db0: 6e67 5f70 6c75 6769 6e2e 5265 7175 6573  ng_plugin.Reques
+00001dc0: 7473 4c6f 6767 696e 6750 6c75 6769 6e60  tsLoggingPlugin`
+00001dd0: 0a20 2020 2023 2077 6869 6368 206c 6f67  .    # which log
+00001de0: 7320 616c 6c20 7265 7175 6573 7473 2061  s all requests a
+00001df0: 6e64 2072 6573 706f 6e73 6573 2062 6569  nd responses bei
+00001e00: 6e67 206d 6164 650a 2020 2020 706c 7567  ng made.    plug
+00001e10: 696e 733d 5b52 6571 7565 7374 734c 6f67  ins=[RequestsLog
+00001e20: 6769 6e67 506c 7567 696e 2829 5d2c 0a29  gingPlugin()],.)
+00001e30: 0a0a 6966 205f 5f6e 616d 655f 5f20 3d3d  ..if __name__ ==
+00001e40: 2022 5f5f 6d61 696e 5f5f 223a 0a20 2020   "__main__":.   
+00001e50: 2063 6f6e 6669 6775 7265 5f6c 6f67 6769   configure_loggi
+00001e60: 6e67 2829 0a20 2020 2023 2052 756e 2073  ng().    # Run s
+00001e70: 6572 7665 7220 2873 7061 776e 7320 7363  erver (spawns sc
+00001e80: 6865 6475 6c65 722c 2041 5049 2061 6e64  heduler, API and
+00001e90: 2077 6f72 6b65 7229 0a20 2020 2023 206f   worker).    # o
+00001ea0: 7065 6e20 6874 7470 3a2f 2f6c 6f63 616c  pen http://local
+00001eb0: 686f 7374 3a38 3038 3020 616e 6420 6578  host:8080 and ex
+00001ec0: 706c 6f72 6520 5549 0a20 2020 2073 6572  plore UI.    ser
+00001ed0: 7665 722e 7365 7276 6528 290a 6060 600a  ver.serve().```.
+00001ee0: 0a4e 6f77 2c20 7468 6520 6f6e 6c79 2074  .Now, the only t
+00001ef0: 6869 6e67 2069 7320 6c65 6674 2069 7320  hing is left is 
+00001f00: 746f 2061 6374 7561 6c6c 7920 7275 6e20  to actually run 
+00001f10: 7468 6520 7365 7276 6572 3a0a 0a60 6060  the server:..```
+00001f20: 6261 7368 0a70 7974 686f 6e20 7275 6e20  bash.python run 
+00001f30: 6d61 696e 2e70 790a 6060 600a 0a54 6861  main.py.```..Tha
+00001f40: 745c 2773 2069 7421 204e 6f77 2079 6f75  t\'s it! Now you
+00001f50: 2063 616e 206f 7065 6e20 3c68 7474 703a   can open <http:
+00001f60: 2f2f 6c6f 6361 6c68 6f73 743a 3830 3830  //localhost:8080
+00001f70: 3e20 616e 6420 6578 706c 6f72 6520 7468  > and explore th
+00001f80: 6520 5549 0a74 6f20 7365 6520 686f 7720  e UI.to see how 
+00001f90: 796f 7520 7363 7261 7065 7220 6973 2062  you scraper is b
+00001fa0: 6569 6e67 2061 7574 6f6d 6174 6963 616c  eing automatical
+00001fb0: 6c79 2073 6368 6564 756c 6564 2061 6e64  ly scheduled and
+00001fc0: 2065 7865 6375 7465 642e 0a0a 2323 204c   executed...## L
+00001fd0: 6f63 616c 2068 616e 646c 6572 2074 6573  ocal handler tes
+00001fe0: 7469 6e67 0a0a 596f 7520 6361 6e20 6561  ting..You can ea
+00001ff0: 7369 6c79 2074 6573 7420 6861 6e64 6c65  sily test handle
+00002000: 7220 7769 7468 6f75 7420 7275 6e6e 696e  r without runnin
+00002010: 6720 6675 6c6c 2d66 6561 7475 7265 6420  g full-featured 
+00002020: 7365 7276 6572 2e20 4865 7265 2773 2068  server. Here's h
+00002030: 6f77 2079 6f75 2063 616e 2064 6f20 7468  ow you can do th
+00002040: 6174 2066 6f72 2074 6865 2060 4465 6d6f  at for the `Demo
+00002050: 5363 7261 7065 7260 2074 6861 7420 7765  Scraper` that we
+00002060: 2068 6176 6520 6465 7665 6c6f 7065 6420   have developed 
+00002070: 696e 2074 6865 205b 5175 6963 6b20 7374  in the [Quick st
+00002080: 6172 745d 2823 7175 6963 6b2d 7374 6172  art](#quick-star
+00002090: 7429 2e0a 0a41 6464 2069 6d70 6f72 7420  t)...Add import 
+000020a0: 696e 2074 6865 2062 6567 696e 6e69 6e67  in the beginning
+000020b0: 206f 6620 7468 6520 6669 6c65 3a0a 0a60   of the file:..`
+000020c0: 6060 7079 7468 6f6e 330a 6672 6f6d 2073  ``python3.from s
+000020d0: 6e65 616b 7065 656b 2e72 756e 6e65 7220  neakpeek.runner 
+000020e0: 696d 706f 7274 204c 6f63 616c 5275 6e6e  import LocalRunn
+000020f0: 6572 0a60 6060 0a0a 416e 6420 6164 6420  er.```..And add 
+00002100: 7468 6520 666f 6c6c 6f77 696e 6720 6c69  the following li
+00002110: 6e65 7320 746f 2074 6865 2065 6e64 206f  nes to the end o
+00002120: 6620 7468 6520 6669 6c65 3a0a 0a60 6060  f the file:..```
+00002130: 7079 7468 6f6e 330a 6966 205f 5f6e 616d  python3.if __nam
+00002140: 655f 5f20 3d3d 2022 5f5f 6d61 696e 5f5f  e__ == "__main__
+00002150: 223a 0a20 2020 204c 6f63 616c 5275 6e6e  ":.    LocalRunn
+00002160: 6572 2e72 756e 280a 2020 2020 2020 2020  er.run(.        
+00002170: 4465 6d6f 5363 7261 7065 7228 292c 0a20  DemoScraper(),. 
+00002180: 2020 2020 2020 2053 6372 6170 6572 436f         ScraperCo
+00002190: 6e66 6967 280a 2020 2020 2020 2020 2020  nfig(.          
+000021a0: 2020 7061 7261 6d73 3d44 656d 6f53 6372    params=DemoScr
+000021b0: 6170 6572 5061 7261 6d73 280a 2020 2020  aperParams(.    
+000021c0: 2020 2020 2020 2020 2020 2020 7572 6c3d              url=
+000021d0: 2268 7474 703a 2f2f 676f 6f67 6c65 2e63  "http://google.c
+000021e0: 6f6d 222c 0a20 2020 2020 2020 2020 2020  om",.           
+000021f0: 2029 2e64 6963 7428 292c 0a20 2020 2020   ).dict(),.     
+00002200: 2020 2029 2c0a 2020 2020 2020 2020 706c     ),.        pl
+00002210: 7567 696e 733d 5b0a 2020 2020 2020 2020  ugins=[.        
+00002220: 2020 2020 5265 7175 6573 7473 4c6f 6767      RequestsLogg
+00002230: 696e 6750 6c75 6769 6e28 292c 0a20 2020  ingPlugin(),.   
+00002240: 2020 2020 205d 2c0a 2020 2020 290a 6060       ],.    ).``
+00002250: 600a 0a46 6f72 2074 6865 2061 7267 756d  `..For the argum
+00002260: 656e 7420 604c 6f63 616c 5275 6e6e 6572  ent `LocalRunner
+00002270: 2e72 756e 6020 7461 6b65 733a 0a0a 312e  .run` takes:..1.
+00002280: 2041 6e20 696e 7374 616e 6365 206f 6620   An instance of 
+00002290: 796f 7572 2073 6372 6170 6572 2068 616e  your scraper han
+000022a0: 646c 6572 0a32 2e20 5363 7261 7065 7220  dler.2. Scraper 
+000022b0: 636f 6e66 6967 0a33 2e20 2a2a 5b4f 7074  config.3. **[Opt
+000022c0: 696f 6e61 6c5d 2a2a 204c 6973 7420 6f66  ional]** List of
+000022d0: 2070 6c75 6769 6e73 2074 6861 7420 7769   plugins that wi
+000022e0: 6c6c 2062 6520 7573 6564 2069 6e20 7468  ll be used in th
+000022f0: 6520 6861 6e64 6c65 7220 285b 7365 6520  e handler ([see 
+00002300: 6675 6c6c 206c 6973 7420 6f66 2074 6865  full list of the
+00002310: 2070 6c75 6769 6e73 2068 6572 655d 2868   plugins here](h
+00002320: 7474 7073 3a2f 2f73 6e65 616b 7065 656b  ttps://sneakpeek
+00002330: 2d70 792e 7265 6164 7468 6564 6f63 732e  -py.readthedocs.
+00002340: 696f 2f65 6e2f 6c61 7465 7374 2f70 6c75  io/en/latest/plu
+00002350: 6769 6e73 2f69 6e64 6578 2e68 746d 6c29  gins/index.html)
+00002360: 290a 0a4e 6f77 2079 6f75 2063 616e 2072  )..Now you can r
+00002370: 756e 2079 6f75 2068 616e 646c 6572 2061  un you handler a
+00002380: 7320 616e 206f 7264 696e 6172 7920 5079  s an ordinary Py
+00002390: 7468 6f6e 2073 6372 6970 742e 2047 6976  thon script. Giv
+000023a0: 656e 2069 7427 7320 696e 2060 6465 6d6f  en it's in `demo
+000023b0: 5f73 6372 6170 6572 2e70 7960 2066 696c  _scraper.py` fil
+000023c0: 6520 796f 7520 6361 6e20 7573 653a 0a0a  e you can use:..
+000023d0: 6060 6062 6173 680a 7079 7468 6f6e 2064  ```bash.python d
+000023e0: 656d 6f5f 7363 7261 7065 722e 7079 0a60  emo_scraper.py.`
+000023f0: 6060 0a0a 2323 2044 6f63 756d 656e 7461  ``..## Documenta
+00002400: 7469 6f6e 0a0a 466f 7220 7468 6520 6675  tion..For the fu
+00002410: 6c6c 2064 6f63 756d 656e 7461 7469 6f6e  ll documentation
+00002420: 2070 6c65 6173 6520 7669 7369 7420 5b73   please visit [s
+00002430: 6e65 616b 7065 656b 2d70 792e 7265 6164  neakpeek-py.read
+00002440: 7468 6564 6f63 732e 696f 5d28 6874 7470  thedocs.io](http
+00002450: 733a 2f2f 736e 6561 6b70 6565 6b2d 7079  s://sneakpeek-py
+00002460: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
+00002470: 656e 2f6c 6174 6573 742f 290a 0a23 2320  en/latest/)..## 
+00002480: 436f 6e74 7269 6275 7469 6e67 0a0a 506c  Contributing..Pl
+00002490: 6561 7365 2074 616b 6520 6120 6c6f 6f6b  ease take a look
+000024a0: 2061 7420 6f75 7220 5b63 6f6e 7472 6962   at our [contrib
+000024b0: 7574 696e 675d 2868 7474 7073 3a2f 2f67  uting](https://g
+000024c0: 6974 6875 622e 636f 6d2f 666c 756c 656d  ithub.com/flulem
+000024d0: 6f6e 2f73 6e65 616b 7065 656b 2f62 6c6f  on/sneakpeek/blo
+000024e0: 622f 6d61 696e 2f43 4f4e 5452 4942 5554  b/main/CONTRIBUT
+000024f0: 494e 472e 6d64 2920 6775 6964 656c 696e  ING.md) guidelin
+00002500: 6573 2069 6620 796f 7527 7265 2069 6e74  es if you're int
+00002510: 6572 6573 7465 6420 696e 2068 656c 7069  erested in helpi
+00002520: 6e67 210a 0a23 2320 4675 7475 7265 2070  ng!..## Future p
+00002530: 6c61 6e73 0a0a 2d20 5375 7070 6f72 7420  lans..- Support 
+00002540: 666f 7220 6465 7665 6c6f 7069 6e67 2061  for developing a
+00002550: 6e64 2065 7865 6375 7469 6e67 2073 6372  nd executing scr
+00002560: 6170 6572 7320 7269 6768 7420 696e 2074  apers right in t
+00002570: 6865 2062 726f 7773 6572 0a2d 2050 6c75  he browser.- Plu
+00002580: 6769 6e73 2066 6f72 2068 6561 6466 756c  gins for headful
+00002590: 2061 6e64 2068 6561 646c 6573 7320 6272   and headless br
+000025a0: 6f77 7365 7220 656e 6769 6e65 7320 2853  owser engines (S
+000025b0: 656c 656e 6975 6d20 616e 6420 506c 6179  elenium and Play
+000025c0: 7772 6967 6874 290a 2d20 5351 4c20 7374  wright).- SQL st
+000025d0: 6f72 6167 6520 696d 706c 656d 656e 7461  orage implementa
+000025e0: 7469 6f6e 0a2d 2041 6476 616e 6365 6420  tion.- Advanced 
+000025f0: 6d6f 6e69 746f 7269 6e67 2066 6f72 2074  monitoring for t
+00002600: 6865 2073 6372 6170 6572 7327 2068 6561  he scrapers' hea
+00002610: 6c74 680a 0a                             lth..
```

