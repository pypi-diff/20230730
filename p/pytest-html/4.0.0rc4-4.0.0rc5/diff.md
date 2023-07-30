# Comparing `tmp/pytest_html-4.0.0rc4.tar.gz` & `tmp/pytest_html-4.0.0rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sat Apr  8 23:08:47 2023, max compression
+gzip compressed data, last modified: Fri Jul 28 15:28:57 2023, max compression
```

## Comparing `pytest_html-4.0.0rc4.tar` & `pytest_html-4.0.0rc5.tar`

### file list

```diff
@@ -1,55 +1,60 @@
--rw-r--r--   0        0        0      146 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/.coveragerc
--rw-r--r--   0        0        0     1953 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/.eslintrc.json
--rw-r--r--   0        0        0       82 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/.nycrc
--rw-r--r--   0        0        0     1694 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/.pre-commit-config.yaml
--rw-r--r--   0        0        0       63 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/.prettierrc
--rw-r--r--   0        0        0      101 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/codecov.yml
--rw-r--r--   0        0        0      215 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/docker-compose.tmpl.yml
--rw-r--r--   0        0        0   340564 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/package-lock.json
--rw-r--r--   0        0        0      661 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/package.json
--rwxr-xr-x   0        0        0      391 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/start
--rw-r--r--   0        0        0     1970 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/tox.ini
--rw-r--r--   0        0        0      634 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/docs/Makefile
--rw-r--r--   0        0        0      171 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/docs/api_reference.rst
--rw-r--r--   0        0        0    13972 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/docs/changelog.rst
--rw-r--r--   0        0        0     2208 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/docs/conf.py
--rw-r--r--   0        0        0     3460 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/docs/deprecations.rst
--rw-r--r--   0        0        0     3991 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/docs/development.rst
--rw-r--r--   0        0        0      506 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/docs/index.rst
--rw-r--r--   0        0        0      340 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/docs/installing.rst
--rw-r--r--   0        0        0      795 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/docs/make.bat
--rw-r--r--   0        0        0    10798 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/docs/user_guide.rst
--rw-r--r--   0        0        0      111 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/src/.gitattributes
--rw-r--r--   0        0        0      125 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/src/.gitignore
--rw-r--r--   0        0        0     5212 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/src/layout/css/style.scss
--rw-r--r--   0        0        0      224 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/src/pytest_html/__init__.py
--rw-r--r--   0        0        0      163 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/src/pytest_html/__version.py
--rw-r--r--   0        0        0    12862 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/src/pytest_html/basereport.py
--rw-r--r--   0        0        0     1595 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/src/pytest_html/extras.py
--rw-r--r--   0        0        0      739 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/src/pytest_html/hooks.py
--rw-r--r--   0        0        0     4514 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/src/pytest_html/plugin.py
--rw-r--r--   0        0        0     1372 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/src/pytest_html/report.py
--rw-r--r--   0        0        0     1178 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/src/pytest_html/selfcontained_report.py
--rw-r--r--   0        0        0     2429 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/src/pytest_html/table.py
--rw-r--r--   0        0        0      673 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/src/pytest_html/util.py
--rw-r--r--   0        0        0    23906 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/src/pytest_html/resources/app.js
--rw-r--r--   0        0        0     4931 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/src/pytest_html/resources/index.jinja2
--rw-r--r--   0        0        0     4313 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/src/pytest_html/resources/style.css
--rw-r--r--   0        0        0     1572 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/src/pytest_html/scripts/datamanager.js
--rw-r--r--   0        0        0     6131 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/src/pytest_html/scripts/dom.js
--rw-r--r--   0        0        0      855 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/src/pytest_html/scripts/filter.js
--rw-r--r--   0        0        0      400 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/src/pytest_html/scripts/index.js
--rw-r--r--   0        0        0     5059 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/src/pytest_html/scripts/main.js
--rw-r--r--   0        0        0     2269 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/src/pytest_html/scripts/mediaviewer.js
--rw-r--r--   0        0        0     1731 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/src/pytest_html/scripts/sort.js
--rw-r--r--   0        0        0     3696 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/src/pytest_html/scripts/storage.js
--rw-r--r--   0        0        0     1025 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/src/pytest_html/scripts/utils.js
--rw-r--r--   0        0        0    43300 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/testing/legacy_test_pytest_html.py
--rw-r--r--   0        0        0    30747 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/testing/test_integration.py
--rw-r--r--   0        0        0      728 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/testing/test_unit.py
--rw-r--r--   0        0        0    10475 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/testing/unittest.js
--rw-r--r--   0        0        0      579 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/.gitignore
--rw-r--r--   0        0        0      193 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/LICENSE
--rw-r--r--   0        0        0     1804 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/README.rst
--rw-r--r--   0        0        0     2179 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/pyproject.toml
--rw-r--r--   0        0        0     3859 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/PKG-INFO
+-rw-r--r--   0        0        0      146 2023-07-28 15:28:57.000000 pytest_html-4.0.0rc5/.coveragerc
+-rw-r--r--   0        0        0     1953 2023-07-28 15:28:57.000000 pytest_html-4.0.0rc5/.eslintrc.json
+-rw-r--r--   0        0        0       82 2023-07-28 15:28:57.000000 pytest_html-4.0.0rc5/.nycrc
+-rw-r--r--   0        0        0     1731 2023-07-28 15:28:57.000000 pytest_html-4.0.0rc5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       63 2023-07-28 15:28:57.000000 pytest_html-4.0.0rc5/.prettierrc
+-rw-r--r--   0        0        0      296 2023-07-28 15:28:57.000000 pytest_html-4.0.0rc5/.readthedocs.yaml
+-rw-r--r--   0        0        0      101 2023-07-28 15:28:57.000000 pytest_html-4.0.0rc5/codecov.yml
+-rw-r--r--   0        0        0      215 2023-07-28 15:28:57.000000 pytest_html-4.0.0rc5/docker-compose.tmpl.yml
+-rw-r--r--   0        0        0   344032 2023-07-28 15:28:57.000000 pytest_html-4.0.0rc5/package-lock.json
+-rw-r--r--   0        0        0      794 2023-07-28 15:28:57.000000 pytest_html-4.0.0rc5/package.json
+-rwxr-xr-x   0        0        0      391 2023-07-28 15:28:57.000000 pytest_html-4.0.0rc5/start
+-rw-r--r--   0        0        0     1970 2023-07-28 15:28:57.000000 pytest_html-4.0.0rc5/tox.ini
+-rw-r--r--   0        0        0      634 2023-07-28 15:28:57.000000 pytest_html-4.0.0rc5/docs/Makefile
+-rw-r--r--   0        0        0      171 2023-07-28 15:28:57.000000 pytest_html-4.0.0rc5/docs/api_reference.rst
+-rw-r--r--   0        0        0    13972 2023-07-28 15:28:57.000000 pytest_html-4.0.0rc5/docs/changelog.rst
+-rw-r--r--   0        0        0     2187 2023-07-28 15:28:57.000000 pytest_html-4.0.0rc5/docs/conf.py
+-rw-r--r--   0        0        0     3439 2023-07-28 15:28:57.000000 pytest_html-4.0.0rc5/docs/deprecations.rst
+-rw-r--r--   0        0        0     3991 2023-07-28 15:28:57.000000 pytest_html-4.0.0rc5/docs/development.rst
+-rw-r--r--   0        0        0      506 2023-07-28 15:28:57.000000 pytest_html-4.0.0rc5/docs/index.rst
+-rw-r--r--   0        0        0      340 2023-07-28 15:28:57.000000 pytest_html-4.0.0rc5/docs/installing.rst
+-rw-r--r--   0        0        0      795 2023-07-28 15:28:57.000000 pytest_html-4.0.0rc5/docs/make.bat
+-rw-r--r--   0        0        0       30 2023-07-28 15:28:57.000000 pytest_html-4.0.0rc5/docs/requirements.in
+-rw-r--r--   0        0        0     1251 2023-07-28 15:28:57.000000 pytest_html-4.0.0rc5/docs/requirements.txt
+-rw-r--r--   0        0        0    11101 2023-07-28 15:28:57.000000 pytest_html-4.0.0rc5/docs/user_guide.rst
+-rw-r--r--   0        0        0      296 2023-07-28 15:28:57.000000 pytest_html-4.0.0rc5/scripts/npm.py
+-rw-r--r--   0        0        0      111 2023-07-28 15:28:57.000000 pytest_html-4.0.0rc5/src/.gitattributes
+-rw-r--r--   0        0        0      125 2023-07-28 15:28:57.000000 pytest_html-4.0.0rc5/src/.gitignore
+-rw-r--r--   0        0        0     5478 2023-07-28 15:28:57.000000 pytest_html-4.0.0rc5/src/layout/css/style.scss
+-rw-r--r--   0        0        0      224 2023-07-28 15:28:57.000000 pytest_html-4.0.0rc5/src/pytest_html/__init__.py
+-rw-r--r--   0        0        0      163 2023-07-28 15:28:57.000000 pytest_html-4.0.0rc5/src/pytest_html/__version.py
+-rw-r--r--   0        0        0    10402 2023-07-28 15:28:57.000000 pytest_html-4.0.0rc5/src/pytest_html/basereport.py
+-rw-r--r--   0        0        0     1595 2023-07-28 15:28:57.000000 pytest_html-4.0.0rc5/src/pytest_html/extras.py
+-rw-r--r--   0        0        0     1253 2023-07-28 15:28:57.000000 pytest_html-4.0.0rc5/src/pytest_html/fixtures.py
+-rw-r--r--   0        0        0      748 2023-07-28 15:28:57.000000 pytest_html-4.0.0rc5/src/pytest_html/hooks.py
+-rw-r--r--   0        0        0     4478 2023-07-28 15:28:57.000000 pytest_html-4.0.0rc5/src/pytest_html/plugin.py
+-rw-r--r--   0        0        0     1628 2023-07-28 15:28:57.000000 pytest_html-4.0.0rc5/src/pytest_html/report.py
+-rw-r--r--   0        0        0     4639 2023-07-28 15:28:57.000000 pytest_html-4.0.0rc5/src/pytest_html/report_data.py
+-rw-r--r--   0        0        0     1433 2023-07-28 15:28:57.000000 pytest_html-4.0.0rc5/src/pytest_html/selfcontained_report.py
+-rw-r--r--   0        0        0     2106 2023-07-28 15:28:57.000000 pytest_html-4.0.0rc5/src/pytest_html/util.py
+-rw-r--r--   0        0        0    20442 2023-07-28 15:28:57.000000 pytest_html-4.0.0rc5/src/pytest_html/resources/app.js
+-rw-r--r--   0        0        0     3850 2023-07-28 15:28:57.000000 pytest_html-4.0.0rc5/src/pytest_html/resources/index.jinja2
+-rw-r--r--   0        0        0     4613 2023-07-28 15:28:57.000000 pytest_html-4.0.0rc5/src/pytest_html/resources/style.css
+-rw-r--r--   0        0        0     1651 2023-07-28 15:28:57.000000 pytest_html-4.0.0rc5/src/pytest_html/scripts/datamanager.js
+-rw-r--r--   0        0        0     3417 2023-07-28 15:28:57.000000 pytest_html-4.0.0rc5/src/pytest_html/scripts/dom.js
+-rw-r--r--   0        0        0      882 2023-07-28 15:28:57.000000 pytest_html-4.0.0rc5/src/pytest_html/scripts/filter.js
+-rw-r--r--   0        0        0      433 2023-07-28 15:28:57.000000 pytest_html-4.0.0rc5/src/pytest_html/scripts/index.js
+-rw-r--r--   0        0        0     4251 2023-07-28 15:28:57.000000 pytest_html-4.0.0rc5/src/pytest_html/scripts/main.js
+-rw-r--r--   0        0        0     2282 2023-07-28 15:28:57.000000 pytest_html-4.0.0rc5/src/pytest_html/scripts/mediaviewer.js
+-rw-r--r--   0        0        0     2902 2023-07-28 15:28:57.000000 pytest_html-4.0.0rc5/src/pytest_html/scripts/sort.js
+-rw-r--r--   0        0        0     3533 2023-07-28 15:28:57.000000 pytest_html-4.0.0rc5/src/pytest_html/scripts/storage.js
+-rw-r--r--   0        0        0    43299 2023-07-28 15:28:57.000000 pytest_html-4.0.0rc5/testing/legacy_test_pytest_html.py
+-rw-r--r--   0        0        0     2217 2023-07-28 15:28:57.000000 pytest_html-4.0.0rc5/testing/test_e2e.py
+-rw-r--r--   0        0        0    31196 2023-07-28 15:28:57.000000 pytest_html-4.0.0rc5/testing/test_integration.py
+-rw-r--r--   0        0        0     3408 2023-07-28 15:28:57.000000 pytest_html-4.0.0rc5/testing/test_unit.py
+-rw-r--r--   0        0        0    10403 2023-07-28 15:28:57.000000 pytest_html-4.0.0rc5/testing/unittest.js
+-rw-r--r--   0        0        0      579 2023-07-28 15:28:57.000000 pytest_html-4.0.0rc5/.gitignore
+-rw-r--r--   0        0        0      193 2023-07-28 15:28:57.000000 pytest_html-4.0.0rc5/LICENSE
+-rw-r--r--   0        0        0     1804 2023-07-28 15:28:57.000000 pytest_html-4.0.0rc5/README.rst
+-rw-r--r--   0        0        0     2309 2023-07-28 15:28:57.000000 pytest_html-4.0.0rc5/pyproject.toml
+-rw-r--r--   0        0        0     3930 2023-07-28 15:28:57.000000 pytest_html-4.0.0rc5/PKG-INFO
```

### Comparing `pytest_html-4.0.0rc4/.eslintrc.json` & `pytest_html-4.0.0rc5/.eslintrc.json`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc4/.pre-commit-config.yaml` & `pytest_html-4.0.0rc5/.pre-commit-config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -39,21 +39,22 @@
 
   - repo: https://github.com/asottile/pyupgrade
     rev: v2.32.0
     hooks:
       - id: pyupgrade
         args: [--py3-plus]
 
-#  - repo: https://github.com/pre-commit/mirrors-eslint
-#    rev: v7.13.0
-#    hooks:
-#      - id: eslint
-#        additional_dependencies:
-#          - eslint@7.13.0
-#        args: [src]
+  - repo: https://github.com/pre-commit/mirrors-eslint
+    rev: v8.38.0
+    hooks:
+      - id: eslint
+        additional_dependencies:
+          - eslint@8.20.0
+          - eslint-config-google@0.14.0
+        args: ["--fix"]
 
   - repo: local
     hooks:
       - id: rst
         name: rst
         entry: rst-lint --encoding utf-8
         files: ^(README.rst)$
```

### Comparing `pytest_html-4.0.0rc4/package-lock.json` & `pytest_html-4.0.0rc5/package-lock.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9975509010834083%*

 * *Differences: {"'dependencies'": "{'core-js': OrderedDict([('version', '3.32.0'), ('resolved', "*

 * *                   "'https://registry.npmjs.org/core-js/-/core-js-3.32.0.tgz'), ('integrity', "*

 * *                   "'sha512-rd4rYZNlF3WuoYuRIDEmbR/ga9CeuWX9U05umAvgrrZoHY4Z++cp/xwPQMvUpBB4Ag6J8KfD80G0zwCyaSxDww=='), "*

 * *                   "('dev', True)]), 'dom-walk': OrderedDict([('version', '0.1.2'), ('resolved', "*

 * *                   "'https://registry.npmjs.org/dom-walk/-/dom-walk-0.1.2.tgz'), ('integrity', "*

 * *                […]*

```diff
@@ -1190,14 +1190,20 @@
         },
         "convert-source-map": {
             "dev": true,
             "integrity": "sha512-Y8L5rp6jo+g9VEPgvqNfEopjTR4OTYct8lXlS8iVQdmnjDvbdbzYe9rjtFCB9egC86JoNCU61WRY+ScjkZpnIg==",
             "resolved": "https://registry.npmjs.org/convert-source-map/-/convert-source-map-1.1.3.tgz",
             "version": "1.1.3"
         },
+        "core-js": {
+            "dev": true,
+            "integrity": "sha512-rd4rYZNlF3WuoYuRIDEmbR/ga9CeuWX9U05umAvgrrZoHY4Z++cp/xwPQMvUpBB4Ag6J8KfD80G0zwCyaSxDww==",
+            "resolved": "https://registry.npmjs.org/core-js/-/core-js-3.32.0.tgz",
+            "version": "3.32.0"
+        },
         "core-util-is": {
             "dev": true,
             "integrity": "sha512-ZQBvi1DcpJ4GDqanjucZ2Hj3wEO5pZDS89BWbkcrvdxksJorwUDDZamX9ldFkp9aw2lmBDLgkObEA4DWNJ9FYQ==",
             "resolved": "https://registry.npmjs.org/core-util-is/-/core-util-is-1.0.3.tgz",
             "version": "1.0.3"
         },
         "create-ecdh": {
@@ -1389,14 +1395,20 @@
             "integrity": "sha512-yS+Q5i3hBf7GBkd4KG8a7eBNNWNGLTaEwwYWUijIYM7zrlYDM0BFXHjjPWlWZ1Rg7UaddZeIDmi9jF3HmqiQ2w==",
             "requires": {
                 "esutils": "^2.0.2"
             },
             "resolved": "https://registry.npmjs.org/doctrine/-/doctrine-3.0.0.tgz",
             "version": "3.0.0"
         },
+        "dom-walk": {
+            "dev": true,
+            "integrity": "sha512-6QvTW9mrGeIegrFXdtQi9pk7O/nSK6lSdXW2eqUspN5LWD7UTji2Fqw5V2YLjBpHEoU9Xl/eUWNpDeZvoyOv2w==",
+            "resolved": "https://registry.npmjs.org/dom-walk/-/dom-walk-0.1.2.tgz",
+            "version": "0.1.2"
+        },
         "domain-browser": {
             "dev": true,
             "integrity": "sha512-jnjyiM6eRyZl2H+W8Q/zLMA481hzi0eszAaBUzIVnmYVDBbnLxVNnfu1HgEBvCbL+71FrxMl3E6lpKH7Ge3OXA==",
             "resolved": "https://registry.npmjs.org/domain-browser/-/domain-browser-1.2.0.tgz",
             "version": "1.2.0"
         },
         "duplexer2": {
@@ -1809,14 +1821,24 @@
             "integrity": "sha512-XxwI8EOhVQgWp6iDL+3b0r86f4d6AX6zSU55HfB4ydCEuXLXc5FcYeOu+nnGftS4TEju/11rt4KJPTMgbfmv4A==",
             "requires": {
                 "is-glob": "^4.0.3"
             },
             "resolved": "https://registry.npmjs.org/glob-parent/-/glob-parent-6.0.2.tgz",
             "version": "6.0.2"
         },
+        "global": {
+            "dev": true,
+            "integrity": "sha512-wv/LAoHdRE3BeTGz53FAamhGlPLhlssK45usmGFThIi4XqnBmjKQ16u+RNbP7WvigRZDxUsM0J3gcQ5yicaL0w==",
+            "requires": {
+                "min-document": "^2.19.0",
+                "process": "^0.11.10"
+            },
+            "resolved": "https://registry.npmjs.org/global/-/global-4.4.0.tgz",
+            "version": "4.4.0"
+        },
         "globals": {
             "dev": true,
             "integrity": "sha512-Qg5QtVkCy/kv3FUSlu4ukeZDVf9ee0iXLAUYX13gbR17bnejFTzr4iS9bY7kwCf1NztRNm1t91fjOiyx4CSwPQ==",
             "requires": {
                 "type-fest": "^0.20.2"
             },
             "resolved": "https://registry.npmjs.org/globals/-/globals-13.20.0.tgz",
@@ -2433,14 +2455,23 @@
             "requires": {
                 "bn.js": "^4.0.0",
                 "brorand": "^1.0.1"
             },
             "resolved": "https://registry.npmjs.org/miller-rabin/-/miller-rabin-4.0.1.tgz",
             "version": "4.0.1"
         },
+        "min-document": {
+            "dev": true,
+            "integrity": "sha512-9Wy1B3m3f66bPPmU5hdA4DR4PB2OfDU/+GS3yAB7IQozE3tqXaVv2zOjgla7MEGSRv95+ILmOuvhLkOK6wJtCQ==",
+            "requires": {
+                "dom-walk": "^0.1.0"
+            },
+            "resolved": "https://registry.npmjs.org/min-document/-/min-document-2.19.0.tgz",
+            "version": "2.19.0"
+        },
         "minimalistic-assert": {
             "dev": true,
             "integrity": "sha512-UtJcAD4yEaGtjPezWuO9wC4nwUnVH/8/Im3yEHQP4b67cXlD/Qr9hdITCU1xDbSEXg2XKNaP8jsReV7vQd00/A==",
             "resolved": "https://registry.npmjs.org/minimalistic-assert/-/minimalistic-assert-1.0.1.tgz",
             "version": "1.0.1"
         },
         "minimalistic-crypto-utils": {
@@ -2557,14 +2588,24 @@
                 "yargs": "16.2.0",
                 "yargs-parser": "20.2.4",
                 "yargs-unparser": "2.0.0"
             },
             "resolved": "https://registry.npmjs.org/mocha/-/mocha-10.2.0.tgz",
             "version": "10.2.0"
         },
+        "mock-local-storage": {
+            "dev": true,
+            "integrity": "sha512-NEfmw+yEK9oe6xCfOnTaJ6Dz+L3eu6vsZopJlxflXYxr7Mg3EV+S0NXKUQlY9AAeDEdaPZDSUGq1Gi6kLSa5PA==",
+            "requires": {
+                "core-js": "^3.30.2",
+                "global": "^4.3.2"
+            },
+            "resolved": "https://registry.npmjs.org/mock-local-storage/-/mock-local-storage-1.1.24.tgz",
+            "version": "1.1.24"
+        },
         "module-deps": {
             "dev": true,
             "integrity": "sha512-fg7OZaQBcL4/L+AK5f4iVqf9OMbCclXfy/znXRxTVhJSeW5AIlS9AwheYwDaXM3lVW7OBeaeUEY3gbaC6cLlSA==",
             "requires": {
                 "JSONStream": "^1.0.3",
                 "browser-resolve": "^2.0.0",
                 "cached-path-relative": "^1.0.2",
@@ -3883,14 +3924,15 @@
         "": {
             "devDependencies": {
                 "browserify": "^17.0.0",
                 "chai": "^4.3.6",
                 "eslint": "^8.20.0",
                 "eslint-config-google": "^0.14.0",
                 "mocha": "^10.0.0",
+                "mock-local-storage": "^1.1.24",
                 "nyc": "^15.1.0",
                 "sass": "^1.52.3",
                 "sinon": "^14.0.0"
             }
         },
         "node_modules/@ampproject/remapping": {
             "dependencies": {
@@ -5386,14 +5428,25 @@
         },
         "node_modules/convert-source-map": {
             "dev": true,
             "integrity": "sha512-Y8L5rp6jo+g9VEPgvqNfEopjTR4OTYct8lXlS8iVQdmnjDvbdbzYe9rjtFCB9egC86JoNCU61WRY+ScjkZpnIg==",
             "resolved": "https://registry.npmjs.org/convert-source-map/-/convert-source-map-1.1.3.tgz",
             "version": "1.1.3"
         },
+        "node_modules/core-js": {
+            "dev": true,
+            "funding": {
+                "type": "opencollective",
+                "url": "https://opencollective.com/core-js"
+            },
+            "hasInstallScript": true,
+            "integrity": "sha512-rd4rYZNlF3WuoYuRIDEmbR/ga9CeuWX9U05umAvgrrZoHY4Z++cp/xwPQMvUpBB4Ag6J8KfD80G0zwCyaSxDww==",
+            "resolved": "https://registry.npmjs.org/core-js/-/core-js-3.32.0.tgz",
+            "version": "3.32.0"
+        },
         "node_modules/core-util-is": {
             "dev": true,
             "integrity": "sha512-ZQBvi1DcpJ4GDqanjucZ2Hj3wEO5pZDS89BWbkcrvdxksJorwUDDZamX9ldFkp9aw2lmBDLgkObEA4DWNJ9FYQ==",
             "resolved": "https://registry.npmjs.org/core-util-is/-/core-util-is-1.0.3.tgz",
             "version": "1.0.3"
         },
         "node_modules/create-ecdh": {
@@ -5628,14 +5681,20 @@
             "engines": {
                 "node": ">=6.0.0"
             },
             "integrity": "sha512-yS+Q5i3hBf7GBkd4KG8a7eBNNWNGLTaEwwYWUijIYM7zrlYDM0BFXHjjPWlWZ1Rg7UaddZeIDmi9jF3HmqiQ2w==",
             "resolved": "https://registry.npmjs.org/doctrine/-/doctrine-3.0.0.tgz",
             "version": "3.0.0"
         },
+        "node_modules/dom-walk": {
+            "dev": true,
+            "integrity": "sha512-6QvTW9mrGeIegrFXdtQi9pk7O/nSK6lSdXW2eqUspN5LWD7UTji2Fqw5V2YLjBpHEoU9Xl/eUWNpDeZvoyOv2w==",
+            "resolved": "https://registry.npmjs.org/dom-walk/-/dom-walk-0.1.2.tgz",
+            "version": "0.1.2"
+        },
         "node_modules/domain-browser": {
             "dev": true,
             "engines": {
                 "node": ">=0.4",
                 "npm": ">=1.2"
             },
             "integrity": "sha512-jnjyiM6eRyZl2H+W8Q/zLMA481hzi0eszAaBUzIVnmYVDBbnLxVNnfu1HgEBvCbL+71FrxMl3E6lpKH7Ge3OXA==",
@@ -6189,14 +6248,24 @@
             "engines": {
                 "node": ">=10.13.0"
             },
             "integrity": "sha512-XxwI8EOhVQgWp6iDL+3b0r86f4d6AX6zSU55HfB4ydCEuXLXc5FcYeOu+nnGftS4TEju/11rt4KJPTMgbfmv4A==",
             "resolved": "https://registry.npmjs.org/glob-parent/-/glob-parent-6.0.2.tgz",
             "version": "6.0.2"
         },
+        "node_modules/global": {
+            "dependencies": {
+                "min-document": "^2.19.0",
+                "process": "^0.11.10"
+            },
+            "dev": true,
+            "integrity": "sha512-wv/LAoHdRE3BeTGz53FAamhGlPLhlssK45usmGFThIi4XqnBmjKQ16u+RNbP7WvigRZDxUsM0J3gcQ5yicaL0w==",
+            "resolved": "https://registry.npmjs.org/global/-/global-4.4.0.tgz",
+            "version": "4.4.0"
+        },
         "node_modules/globals": {
             "dependencies": {
                 "type-fest": "^0.20.2"
             },
             "dev": true,
             "engines": {
                 "node": ">=8"
@@ -7018,14 +7087,23 @@
         },
         "node_modules/miller-rabin/node_modules/bn.js": {
             "dev": true,
             "integrity": "sha512-c98Bf3tPniI+scsdk237ku1Dc3ujXQTSgyiPUDEOe7tRkhrqridvh8klBv0HCEso1OLOYcHuCv/cS6DNxKH+ZA==",
             "resolved": "https://registry.npmjs.org/bn.js/-/bn.js-4.12.0.tgz",
             "version": "4.12.0"
         },
+        "node_modules/min-document": {
+            "dependencies": {
+                "dom-walk": "^0.1.0"
+            },
+            "dev": true,
+            "integrity": "sha512-9Wy1B3m3f66bPPmU5hdA4DR4PB2OfDU/+GS3yAB7IQozE3tqXaVv2zOjgla7MEGSRv95+ILmOuvhLkOK6wJtCQ==",
+            "resolved": "https://registry.npmjs.org/min-document/-/min-document-2.19.0.tgz",
+            "version": "2.19.0"
+        },
         "node_modules/minimalistic-assert": {
             "dev": true,
             "integrity": "sha512-UtJcAD4yEaGtjPezWuO9wC4nwUnVH/8/Im3yEHQP4b67cXlD/Qr9hdITCU1xDbSEXg2XKNaP8jsReV7vQd00/A==",
             "resolved": "https://registry.npmjs.org/minimalistic-assert/-/minimalistic-assert-1.0.1.tgz",
             "version": "1.0.1"
         },
         "node_modules/minimalistic-crypto-utils": {
@@ -7171,14 +7249,24 @@
             "funding": {
                 "url": "https://github.com/chalk/supports-color?sponsor=1"
             },
             "integrity": "sha512-MpUEN2OodtUzxvKQl72cUF7RQ5EiHsGvSsVG0ia9c5RbWGL2CI4C7EpPS8UTBIplnlzZiNuV56w+FuNxy3ty2Q==",
             "resolved": "https://registry.npmjs.org/supports-color/-/supports-color-8.1.1.tgz",
             "version": "8.1.1"
         },
+        "node_modules/mock-local-storage": {
+            "dependencies": {
+                "core-js": "^3.30.2",
+                "global": "^4.3.2"
+            },
+            "dev": true,
+            "integrity": "sha512-NEfmw+yEK9oe6xCfOnTaJ6Dz+L3eu6vsZopJlxflXYxr7Mg3EV+S0NXKUQlY9AAeDEdaPZDSUGq1Gi6kLSa5PA==",
+            "resolved": "https://registry.npmjs.org/mock-local-storage/-/mock-local-storage-1.1.24.tgz",
+            "version": "1.1.24"
+        },
         "node_modules/module-deps": {
             "bin": {
                 "module-deps": "bin/cmd.js"
             },
             "dependencies": {
                 "JSONStream": "^1.0.3",
                 "browser-resolve": "^2.0.0",
```

### Comparing `pytest_html-4.0.0rc4/package.json` & `pytest_html-4.0.0rc5/package.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8293650793650793%*

 * *Differences: {"'devDependencies'": "{'mock-local-storage': '^1.1.24'}",*

 * * "'scripts'": "{'unit': 'nyc mocha testing/**/unittest.js --require mock-local-storage', 'build': "*

 * *              "'npm run build:css && npm run build:jsapp', 'lint': 'eslint "*

 * *              "src/pytest_html/scripts/ testing/', 'all': 'npm run lint && npm run unit && npm run "*

 * *              "build:css && npm run build:jsapp', delete: ['build:ci']}"}*

```diff
@@ -1,19 +1,21 @@
 {
     "devDependencies": {
         "browserify": "^17.0.0",
         "chai": "^4.3.6",
         "eslint": "^8.20.0",
         "eslint-config-google": "^0.14.0",
         "mocha": "^10.0.0",
+        "mock-local-storage": "^1.1.24",
         "nyc": "^15.1.0",
         "sass": "^1.52.3",
         "sinon": "^14.0.0"
     },
     "scripts": {
-        "build": "npm run unit && npm run build:css && npm run build:jsapp",
-        "build:ci": "npm run build:css && npm run build:jsapp",
+        "all": "npm run lint && npm run unit && npm run build:css && npm run build:jsapp",
+        "build": "npm run build:css && npm run build:jsapp",
         "build:css": "sass --no-source-map --no-error-css src/layout/css/style.scss src/pytest_html/resources/style.css",
         "build:jsapp": "browserify ./src/pytest_html/scripts/index.js > ./src/pytest_html/resources/app.js",
-        "unit": "nyc mocha testing/**/unittest.js"
+        "lint": "eslint src/pytest_html/scripts/ testing/",
+        "unit": "nyc mocha testing/**/unittest.js --require mock-local-storage"
     }
 }
```

### Comparing `pytest_html-4.0.0rc4/tox.ini` & `pytest_html-4.0.0rc5/tox.ini`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc4/docs/Makefile` & `pytest_html-4.0.0rc5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc4/docs/changelog.rst` & `pytest_html-4.0.0rc5/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc4/docs/conf.py` & `pytest_html-4.0.0rc5/docs/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = ["sphinx.ext.autodoc"]
 
 # Add any paths that contain templates here, relative to this directory.
-templates_path = ["_templates"]
+templates_path = []
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
 
@@ -49,15 +49,15 @@
     "github_banner": "true",
     "github_type": "star",
 }
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ["_static"]
+html_static_path = []
 
 # The master toctree document.
 master_doc = "index"
 
 
 # -- Options for the autodoc extension ---------------------------------------
```

### Comparing `pytest_html-4.0.0rc4/docs/deprecations.rst` & `pytest_html-4.0.0rc5/docs/deprecations.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-User Guide
-==========
+Deprecations
+============
 
 Deprecation policy
 ------------------
 
 If not otherwise explicitly stated, deprecations are removed in the next major version.
 
 Deprecations
--------------------------------------
+------------
 
 duration_formatter
 ~~~~~~~~~~~~~~~~~~
 
 Deprecated in ``4.0.0``
 
 *'duration_formatter' has been removed and no longer has any effect!*
```

### Comparing `pytest_html-4.0.0rc4/docs/development.rst` & `pytest_html-4.0.0rc5/docs/development.rst`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc4/docs/make.bat` & `pytest_html-4.0.0rc5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc4/docs/user_guide.rst` & `pytest_html-4.0.0rc5/docs/user_guide.rst`

 * *Files 5% similar despite different names*

```diff
@@ -57,27 +57,31 @@
 The *Environment* section is provided by the `pytest-metadata`_ plugin, and can be accessed
 via the :code:`pytest_configure` and :code:`pytest_sessionfinish` hooks:
 
 To modify the *Environment* section **before** tests are run, use :code:`pytest_configure`:
 
 .. code-block:: python
 
+  from pytest_metadata.plugin import metadata_key
+
+
   def pytest_configure(config):
-      config._metadata["foo"] = "bar"
+      config.stash[metadata_key]["foo"] = "bar"
 
 To modify the *Environment* section **after** tests are run, use :code:`pytest_sessionfinish`:
 
 .. code-block:: python
 
   import pytest
+  from pytest_metadata.plugin import metadata_key
 
 
   @pytest.hookimpl(tryfirst=True)
   def pytest_sessionfinish(session, exitstatus):
-      session.config._metadata["foo"] = "bar"
+      session.config.stash[metadata_key]["foo"] = "bar"
 
 Note that in the above example `@pytest.hookimpl(tryfirst=True)`_ is important, as this ensures that a best effort attempt is made to run your
 :code:`pytest_sessionfinish` **before** any other plugins ( including :code:`pytest-html` and :code:`pytest-metadata` ) run theirs.
 If this line is omitted, then the *Environment* table will **not** be updated since the :code:`pytest_sessionfinish` of the plugins will execute first,
 and thus not pick up your change.
 
 The generated table will be sorted alphabetically unless the metadata is a :code:`collections.OrderedDict`.
@@ -278,15 +282,18 @@
 * :code:`xfailed`
 * :code:`xpassed`
 * :code:`rerun`
 
 Results Table Sorting
 ~~~~~~~~~~~~~~~~~~~~~
 
-You can change the sort order of the results table on page load by passing the :code:`sort` query parameter.
+You can change which column the results table is sorted on, on page load by passing the :code:`sort` query parameter.
+
+You can also set the initial sorting by setting :code:`initial_sort` in a configuration file (pytest.ini, setup.cfg, etc).
+Note that the query parameter takes precedence.
 
 The following values may be passed:
 
 * :code:`result`
 * :code:`testId`
 * :code:`duration`
 * :code:`original`
```

### Comparing `pytest_html-4.0.0rc4/src/layout/css/style.scss` & `pytest_html-4.0.0rc5/src/layout/css/style.scss`

 * *Files 8% similar despite different names*

```diff
@@ -42,15 +42,14 @@
 
 #environment {
   td {
     padding: $spacing;
     border: $border-width solid #e6e6e6;
     vertical-align: top;
   }
-
   tr:nth-child(odd) {
     background-color: #f6f6f6;
   }
   ul {
     margin: 0;
     padding: 0 20px;
   }
@@ -179,59 +178,72 @@
 .media__counter {
   display: flex;
   flex-direction: row;
   justify-content: space-around;
   flex: 0 0 25px;
   align-items: center;
 }
-.collapsed {
-  display: none;
-}
 
 @mixin rowToggle {
   color: #bbb;
   font-style: italic;
   cursor: pointer;
 }
 
-.col-result {
+.collapsible td:not(.col-links) {
   cursor: pointer;
   &:hover::after {
     @include rowToggle;
   }
 }
-.col-result.collapser {
+
+.col-result {
+  &:hover::after {
+    content: ' (hide details)';
+  }
+}
+.col-result.collapsed {
+  &:hover::after {
+    content: ' (show details)';
+  }
+}
+
+#environment-header h2 {
   &:hover::after {
     content: ' (hide details)';
+    @include rowToggle;
+    font-size: $font-size-text;
   }
 }
-.col-result.expander {
+#environment-header.collapsed h2 {
   &:hover::after {
     content: ' (show details)';
+    @include rowToggle;
+    font-size: $font-size-text;
   }
 }
 
 /*------------------
  * 3. Sorting items
  *------------------*/
 .sortable {
   cursor: pointer;
-  &.asc {
+  &.desc {
     &:after {
       content: ' ';
       position: relative;
       left: 5px;
       bottom: -12.5px;
       border: 10px solid #4caf50;
       border-bottom: 0;
       border-left-color: transparent;
       border-right-color: transparent;
     }
   }
-  &.desc {
+  &.asc {
     &:after {
       content: ' ';
       position: relative;
       left: 5px;
       bottom: 12.5px;
       border: 10px solid #4caf50;
       border-top: 0;
```

### Comparing `pytest_html-4.0.0rc4/src/pytest_html/basereport.py` & `pytest_html-4.0.0rc5/src/pytest_html/basereport.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,132 +1,39 @@
+# This Source Code Form is subject to the terms of the Mozilla Public
+# License, v. 2.0. If a copy of the MPL was not distributed with this
+# file, You can obtain one at http://mozilla.org/MPL/2.0/.
 import datetime
 import json
+import math
 import os
 import re
 import warnings
-from collections import defaultdict
-from functools import partial
 from pathlib import Path
 
 import pytest
-from jinja2 import Environment
-from jinja2 import FileSystemLoader
-from jinja2 import select_autoescape
+from pytest_metadata.plugin import metadata_key
 
 from pytest_html import __version__
 from pytest_html import extras
-from pytest_html.table import Header
-from pytest_html.table import Html
-from pytest_html.table import Row
 from pytest_html.util import cleanup_unserializable
 
-try:
-    from ansi2html import Ansi2HTMLConverter, style
-
-    converter = Ansi2HTMLConverter(inline=False, escaped=False)
-    _handle_ansi = partial(converter.convert, full=False)
-    _ansi_styles = style.get_styles()
-except ImportError:
-    from _pytest.logging import _remove_ansi_escape_sequences
-
-    _handle_ansi = _remove_ansi_escape_sequences
-    _ansi_styles = []
-
 
 class BaseReport:
-    class ReportData:
-        def __init__(self, title, config):
-            self._config = config
-            self._data = {
-                "title": title,
-                "collectedItems": 0,
-                "runningState": "not_started",
-                "environment": {},
-                "tests": defaultdict(list),
-                "resultsTableHeader": {},
-                "additionalSummary": defaultdict(list),
-            }
-
-            collapsed = config.getini("render_collapsed")
-            if collapsed:
-                if collapsed.lower() == "true":
-                    warnings.warn(
-                        "'render_collapsed = True' is deprecated and support "
-                        "will be removed in the next major release. "
-                        "Please use 'render_collapsed = all' instead.",
-                        DeprecationWarning,
-                    )
-                self.set_data(
-                    "collapsed", [outcome.lower() for outcome in collapsed.split(",")]
-                )
-
-        @property
-        def title(self):
-            return self._data["title"]
-
-        @title.setter
-        def title(self, title):
-            self._data["title"] = title
-
-        @property
-        def config(self):
-            return self._config
-
-        @property
-        def data(self):
-            return self._data
-
-        def set_data(self, key, value):
-            self._data[key] = value
-
-        def add_test(self, test_data, report, row, remove_log=False):
-            for sortable, value in row.sortables.items():
-                test_data[sortable] = value
-
-            # regardless of pass or fail we must add teardown logging to "call"
-            if report.when == "teardown" and not remove_log:
-                self.update_test_log(report)
-
-            # passed "setup" and "teardown" are not added to the html
-            if report.when == "call" or (
-                report.when in ["setup", "teardown"] and report.outcome != "passed"
-            ):
-                if not remove_log:
-                    processed_logs = _process_logs(report)
-                    test_data["log"] = _handle_ansi(processed_logs)
-                self._data["tests"][report.nodeid].append(test_data)
-                return True
-
-            return False
-
-        def update_test_log(self, report):
-            log = []
-            for test in self._data["tests"][report.nodeid]:
-                if test["testId"] == report.nodeid and "log" in test:
-                    for section in report.sections:
-                        header, content = section
-                        if "teardown" in header:
-                            log.append(f"{' ' + header + ' ':-^80}")
-                            log.append(content)
-                    test["log"] += _handle_ansi("\n".join(log))
-
-    def __init__(self, report_path, config, default_css="style.css"):
+    def __init__(self, report_path, config, report_data, template, css):
         self._report_path = Path(os.path.expandvars(report_path)).expanduser()
         self._report_path.parent.mkdir(parents=True, exist_ok=True)
-        self._resources_path = Path(__file__).parent.joinpath("resources")
         self._config = config
-        self._template = _read_template([self._resources_path])
-        self._css = _process_css(
-            Path(self._resources_path, default_css), self._config.getoption("css")
-        )
+        self._template = template
+        self._css = css
         self._max_asset_filename_length = int(
             config.getini("max_asset_filename_length")
         )
 
-        self._report = self.ReportData(self._report_path.name, config)
+        self._report = report_data
+        self._report.title = self._report_path.name
 
     @property
     def css(self):
         # implement in subclasses
         return
 
     def _asset_filename(self, test_id, extra_index, test_index, file_extension):
@@ -135,30 +42,35 @@
             str(extra_index),
             str(test_index),
             file_extension,
         )[-self._max_asset_filename_length :]
 
     def _generate_report(self, self_contained=False):
         generated = datetime.datetime.now()
-        rendered_report = self._render_html(
-            generated.strftime("%d-%b-%Y"),
-            generated.strftime("%H:%M:%S"),
-            __version__,
-            self.css,
+        test_data = cleanup_unserializable(self._report.data)
+        test_data = json.dumps(test_data)
+        rendered_report = self._template.render(
+            title=self._report.title,
+            date=generated.strftime("%d-%b-%Y"),
+            time=generated.strftime("%H:%M:%S"),
+            version=__version__,
+            styles=self.css,
+            run_count=self._run_count(),
+            running_state=self._report.running_state,
             self_contained=self_contained,
-            test_data=cleanup_unserializable(self._report.data),
-            prefix=self._report.data["additionalSummary"]["prefix"],
-            summary=self._report.data["additionalSummary"]["summary"],
-            postfix=self._report.data["additionalSummary"]["postfix"],
+            outcomes=self._report.outcomes,
+            test_data=test_data,
+            table_head=self._report.table_header,
+            additional_summary=self._report.additional_summary,
         )
 
         self._write_report(rendered_report)
 
     def _generate_environment(self):
-        metadata = self._config._metadata
+        metadata = self._config.stash[metadata_key]
         for key in metadata.keys():
             value = metadata[key]
             if self._is_redactable_environment_variable(key):
                 black_box_ascii_value = 0x2593
                 metadata[key] = "".join(chr(black_box_ascii_value) for _ in str(value))
 
         return metadata
@@ -204,174 +116,183 @@
             if extra["format_type"] in [extras.FORMAT_IMAGE, extras.FORMAT_VIDEO]:
                 extra["content"] = self._media_content(
                     content, asset_name=asset_name, mime_type=extra["mime_type"]
                 )
 
         return report_extras
 
-    def _render_html(
-        self,
-        date,
-        time,
-        version,
-        styles,
-        self_contained,
-        test_data,
-        summary,
-        prefix,
-        postfix,
-    ):
-        return self._template.render(
-            date=date,
-            time=time,
-            version=version,
-            styles=styles,
-            self_contained=self_contained,
-            test_data=json.dumps(test_data),
-            summary=summary,
-            prefix=prefix,
-            postfix=postfix,
-        )
-
     def _write_report(self, rendered_report):
         with self._report_path.open("w", encoding="utf-8") as f:
             f.write(rendered_report)
 
+    def _run_count(self):
+        relevant_outcomes = ["passed", "failed", "xpassed", "xfailed"]
+        counts = 0
+        for outcome in self._report.outcomes.keys():
+            if outcome in relevant_outcomes:
+                counts += self._report.outcomes[outcome]["value"]
+
+        plural = counts > 1
+        duration = _format_duration(self._report.total_duration)
+
+        if self._report.running_state == "finished":
+            return f"{counts} {'tests' if plural else 'test'} took {duration}."
+
+        return f"{counts}/{self._report.collected_items} {'tests' if plural else 'test'} done."
+
     @pytest.hookimpl(trylast=True)
     def pytest_sessionstart(self, session):
-        config = session.config
-        if hasattr(config, "_metadata") and config._metadata:
-            self._report.set_data("environment", self._generate_environment())
+        self._report.set_data("environment", self._generate_environment())
 
         session.config.hook.pytest_html_report_title(report=self._report)
 
-        header_cells = Header()
-        session.config.hook.pytest_html_results_table_header(cells=header_cells)
-        self._report.set_data("resultsTableHeader", header_cells.html)
-        self._report.set_data("headerPops", header_cells.get_pops())
+        headers = self._report.table_header
+        session.config.hook.pytest_html_results_table_header(cells=headers)
+        self._report.table_header = _fix_py(headers)
 
-        self._report.set_data("runningState", "Started")
+        self._report.running_state = "started"
         self._generate_report()
 
     @pytest.hookimpl(trylast=True)
     def pytest_sessionfinish(self, session):
         session.config.hook.pytest_html_results_summary(
-            prefix=self._report.data["additionalSummary"]["prefix"],
-            summary=self._report.data["additionalSummary"]["summary"],
-            postfix=self._report.data["additionalSummary"]["postfix"],
+            prefix=self._report.additional_summary["prefix"],
+            summary=self._report.additional_summary["summary"],
+            postfix=self._report.additional_summary["postfix"],
+            session=session,
         )
-        self._report.set_data("runningState", "Finished")
+        self._report.running_state = "finished"
         self._generate_report()
 
     @pytest.hookimpl(trylast=True)
     def pytest_terminal_summary(self, terminalreporter):
         terminalreporter.write_sep(
-            "-", f"Generated html report: file://{self._report_path.resolve()}"
+            "-",
+            f"Generated html report: file://{self._report_path.resolve().as_posix()}",
         )
 
     @pytest.hookimpl(trylast=True)
     def pytest_collection_finish(self, session):
-        self._report.set_data("collectedItems", len(session.items))
+        self._report.collected_items = len(session.items)
 
     @pytest.hookimpl(trylast=True)
     def pytest_runtest_logreport(self, report):
         if hasattr(report, "duration_formatter"):
             warnings.warn(
                 "'duration_formatter' has been removed and no longer has any effect!",
                 DeprecationWarning,
             )
 
+        outcome = _process_outcome(report)
         data = {
-            "duration": report.duration,
+            "result": outcome,
+            "duration": _format_duration(report.duration),
         }
+        self._report.total_duration += report.duration
 
         test_id = report.nodeid
         if report.when != "call":
             test_id += f"::{report.when}"
         data["testId"] = test_id
 
-        row_cells = Row()
-        self._config.hook.pytest_html_results_table_row(report=report, cells=row_cells)
-        if row_cells.html is None:
+        data["extras"] = self._process_extras(report, test_id)
+        links = [
+            extra
+            for extra in data["extras"]
+            if extra["format_type"] in ["json", "text", "url"]
+        ]
+        cells = [
+            f'<td class="col-result">{data["result"]}</td>',
+            f'<td class="col-name">{data["testId"]}</td>',
+            f'<td class="col-duration">{data["duration"]}</td>',
+            f'<td class="col-links">{_process_links(links)}</td>',
+        ]
+
+        self._config.hook.pytest_html_results_table_row(report=report, cells=cells)
+        if not cells:
             return
-        data["resultsTableRow"] = row_cells.html
 
-        table_html = Html()
-        self._config.hook.pytest_html_results_table_html(report=report, data=table_html)
-        data["tableHtml"] = table_html.html["html"]
+        cells = _fix_py(cells)
+        data["resultsTableRow"] = cells
 
-        data["result"] = _process_outcome(report)
-        data["extras"] = self._process_extras(report, test_id)
+        # don't count passed setups and teardowns
+        if not (report.when in ["setup", "teardown"] and report.outcome == "passed"):
+            self._report.outcomes = outcome
+
+        processed_logs = _process_logs(report)
+        self._config.hook.pytest_html_results_table_html(
+            report=report, data=processed_logs
+        )
 
-        if self._report.add_test(data, report, row_cells, table_html.replace_log):
+        if self._report.add_test(data, report, processed_logs):
             self._generate_report()
 
 
-def _process_css(default_css, extra_css):
-    with open(default_css, encoding="utf-8") as f:
-        css = f.read()
-
-    # Add user-provided CSS
-    for path in extra_css:
-        css += "\n/******************************"
-        css += "\n * CUSTOM CSS"
-        css += f"\n * {path}"
-        css += "\n ******************************/\n\n"
-        with open(path, encoding="utf-8") as f:
-            css += f.read()
-
-    # ANSI support
-    if _ansi_styles:
-        ansi_css = [
-            "\n/******************************",
-            " * ANSI2HTML STYLES",
-            " ******************************/\n",
-        ]
-        ansi_css.extend([str(r) for r in _ansi_styles])
-        css += "\n".join(ansi_css)
+def _format_duration(duration):
+    if duration < 1:
+        return "{} ms".format(round(duration * 1000))
+
+    hours = math.floor(duration / 3600)
+    remaining_seconds = duration % 3600
+    minutes = math.floor(remaining_seconds / 60)
+    remaining_seconds = remaining_seconds % 60
+    seconds = round(remaining_seconds)
 
-    return css
+    return f"{hours:02d}:{minutes:02d}:{seconds:02d}"
 
 
 def _is_error(report):
     return report.when in ["setup", "teardown"] and report.outcome == "failed"
 
 
 def _process_logs(report):
     log = []
     if report.longreprtext:
         log.append(report.longreprtext.replace("<", "&lt;").replace(">", "&gt;") + "\n")
-    for section in report.sections:
-        header, content = section
-        log.append(f"{' ' + header + ' ':-^80}")
-        log.append(content)
-
-        # weird formatting related to logs
-        if "log" in header:
-            log.append("")
-            if "call" in header:
+    # Don't add captured output to reruns
+    if report.outcome != "rerun":
+        for section in report.sections:
+            header, content = section
+            log.append(f"{' ' + header + ' ':-^80}\n{content}")
+
+            # weird formatting related to logs
+            if "log" in header:
                 log.append("")
+                if "call" in header:
+                    log.append("")
     if not log:
         log.append("No log output captured.")
-    return "\n".join(log)
+    return log
 
 
 def _process_outcome(report):
     if _is_error(report):
         return "Error"
     if hasattr(report, "wasxfail"):
         if report.outcome in ["passed", "failed"]:
             return "XPassed"
         if report.outcome == "skipped":
             return "XFailed"
 
     return report.outcome.capitalize()
 
 
-def _read_template(search_paths, template_name="index.jinja2"):
-    env = Environment(
-        loader=FileSystemLoader(search_paths),
-        autoescape=select_autoescape(
-            enabled_extensions=("jinja2",),
-        ),
-    )
-    return env.get_template(template_name)
+def _process_links(links):
+    a_tag = '<a target="_blank" href="{content}" class="col-links__extra {format_type}">{name}</a>'
+    return "".join([a_tag.format_map(link) for link in links])
+
+
+def _fix_py(cells):
+    # backwards-compat
+    new_cells = []
+    for html in cells:
+        if not isinstance(html, str):
+            if html.__module__.startswith("py."):
+                warnings.warn(
+                    "The 'py' module is deprecated and support "
+                    "will be removed in a future release.",
+                    DeprecationWarning,
+                )
+            html = str(html)
+            html = html.replace("col=", "data-column-type=")
+        new_cells.append(html)
+    return new_cells
```

### Comparing `pytest_html-4.0.0rc4/src/pytest_html/extras.py` & `pytest_html-4.0.0rc5/src/pytest_html/extras.py`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc4/src/pytest_html/hooks.py` & `pytest_html-4.0.0rc5/src/pytest_html/hooks.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 
 def pytest_html_report_title(report):
     """Called before adding the title to the report"""
 
 
-def pytest_html_results_summary(prefix, summary, postfix):
+def pytest_html_results_summary(prefix, summary, postfix, session):
     """Called before adding the summary section to the report"""
 
 
 def pytest_html_results_table_header(cells):
     """Called after building results table header."""
```

### Comparing `pytest_html-4.0.0rc4/src/pytest_html/report.py` & `pytest_html-4.0.0rc5/src/pytest_html/report.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 import base64
 import binascii
 from pathlib import Path
 
 from pytest_html.basereport import BaseReport
 
+# This Source Code Form is subject to the terms of the Mozilla Public
+# License, v. 2.0. If a copy of the MPL was not distributed with this
+# file, You can obtain one at http://mozilla.org/MPL/2.0/.
+
 
 class Report(BaseReport):
-    def __init__(self, report_path, config):
-        super().__init__(report_path, config)
+    def __init__(self, report_path, config, report_data, template, css):
+        super().__init__(report_path, config, report_data, template, css)
         self._assets_path = Path(self._report_path.parent, "assets")
         self._assets_path.mkdir(parents=True, exist_ok=True)
         self._css_path = Path(self._assets_path, "style.css")
 
         with self._css_path.open("w", encoding="utf-8") as f:
             f.write(self._css)
```

### Comparing `pytest_html-4.0.0rc4/src/pytest_html/resources/app.js` & `pytest_html-4.0.0rc5/src/pytest_html/resources/app.js`

 * *Files 18% similar despite different names*

#### js-beautify {}

```diff
@@ -22,107 +22,107 @@
         for (var u = "function" == typeof require && require, i = 0; i < t.length; i++) o(t[i]);
         return o
     }
     return r
 })()({
     1: [function(require, module, exports) {
         const {
-            getCollapsedCategory
+            getCollapsedCategory,
+            setCollapsedIds
         } = require('./storage.js')
 
         class DataManager {
             setManager(data) {
-                const collapsedCategories = [...getCollapsedCategory(data.collapsed)]
+                const collapsedCategories = [...getCollapsedCategory(data.renderCollapsed)]
+                const collapsedIds = []
+                const tests = Object.values(data.tests).flat().map((test, index) => {
+                    const collapsed = collapsedCategories.includes(test.result.toLowerCase())
+                    const id = `test_${index}`
+                    if (collapsed) {
+                        collapsedIds.push(id)
+                    }
+                    return {
+                        ...test,
+                        id,
+                        collapsed,
+                    }
+                })
                 const dataBlob = {
                     ...data,
-                    tests: Object.values(data.tests).flat().map((test, index) => ({
-                        ...test,
-                        id: `test_${index}`,
-                        collapsed: collapsedCategories.includes(test.result.toLowerCase()),
-                    }))
+                    tests
                 }
                 this.data = {
                     ...dataBlob
                 }
                 this.renderData = {
                     ...dataBlob
                 }
+                setCollapsedIds(collapsedIds)
             }
 
             get allData() {
                 return {
                     ...this.data
                 }
             }
+
             resetRender() {
                 this.renderData = {
                     ...this.data
                 }
             }
+
             setRender(data) {
                 this.renderData.tests = [...data]
             }
+
             toggleCollapsedItem(id) {
                 this.renderData.tests = this.renderData.tests.map((test) =>
                     test.id === id ? {
                         ...test,
                         collapsed: !test.collapsed
                     } : test,
                 )
             }
+
             set allCollapsed(collapsed) {
                 this.renderData = {
                     ...this.renderData,
                     tests: [...this.renderData.tests.map((test) => ({
                         ...test,
                         collapsed
                     }))]
                 }
             }
 
             get testSubset() {
                 return [...this.renderData.tests]
             }
-            get allTests() {
-                return [...this.data.tests]
-            }
-            get title() {
-                return this.renderData.title
-            }
+
             get environment() {
                 return this.renderData.environment
             }
-            get collectedItems() {
-                return this.renderData.collectedItems
-            }
-            get isFinished() {
-                return this.data.runningState === 'Finished'
+
+            get initialSort() {
+                return this.data.initialSort
             }
         }
 
         module.exports = {
             manager: new DataManager(),
         }
 
     }, {
         "./storage.js": 8
     }],
     2: [function(require, module, exports) {
-        const storageModule = require('./storage.js')
-        const {
-            formatDuration,
-            transformTableObj
-        } = require('./utils.js')
         const mediaViewer = require('./mediaviewer.js')
-        const templateEnvRow = document.querySelector('#template_environment_row')
-        const templateCollGroup = document.querySelector('#template_table-colgroup')
-        const templateResult = document.querySelector('#template_results-table__tbody')
-        const aTag = document.querySelector('#template_a')
-        const listHeader = document.querySelector('#template_results-table__head')
-        const listHeaderEmpty = document.querySelector('#template_results-table__head--empty')
+        const templateEnvRow = document.getElementById('template_environment_row')
+        const templateResult = document.getElementById('template_results-table__tbody')
+        const listHeaderEmpty = document.getElementById('template_results-table__head--empty')
 
         function htmlToElements(html) {
             const temp = document.createElement('template')
             temp.innerHTML = html
             return temp.content.childNodes
         }
 
@@ -136,162 +136,113 @@
         const findAll = (selector, elem) => {
             if (!elem) {
                 elem = document
             }
             return [...elem.querySelectorAll(selector)]
         }
 
-        const insertAdditionalHTML = (html, element, selector, position = 'beforebegin') => {
-            Object.keys(html).map((key) => {
-                element.querySelectorAll(selector).item(key).insertAdjacentHTML(position, html[key])
-            })
-        }
-
         const dom = {
             getStaticRow: (key, value) => {
                 const envRow = templateEnvRow.content.cloneNode(true)
                 const isObj = typeof value === 'object' && value !== null
                 const values = isObj ? Object.keys(value).map((k) => `${k}: ${value[k]}`) : null
 
                 const valuesElement = htmlToElements(
                     values ? `<ul>${values.map((val) => `<li>${val}</li>`).join('')}<ul>` : `<div>${value}</div>`)[0]
                 const td = findAll('td', envRow)
                 td[0].textContent = key
                 td[1].appendChild(valuesElement)
 
                 return envRow
             },
-            getListHeader: ({
-                resultsTableHeader
-            }) => {
-                const header = listHeader.content.cloneNode(true)
-                const sortAttr = storageModule.getSort()
-                const sortAsc = JSON.parse(storageModule.getSortDirection())
-
-                const regex = /data-column-type="(\w+)/
-                const cols = Object.values(resultsTableHeader).reduce((result, value) => {
-                    if (value.includes("sortable")) {
-                        const matches = regex.exec(value)
-                        if (matches) {
-                            result.push(matches[1])
-                        }
-                    }
-                    return result
-                }, [])
-                const sortables = ['result', 'testId', 'duration', ...cols]
-
-                // Add custom html from the pytest_html_results_table_header hook
-                const headers = transformTableObj(resultsTableHeader)
-                insertAdditionalHTML(headers.inserts, header, 'th')
-                insertAdditionalHTML(headers.appends, header, 'tr', 'beforeend')
-
-                sortables.forEach((sortCol) => {
-                    if (sortCol === sortAttr) {
-                        header.querySelector(`[data-column-type="${sortCol}"]`).classList.add(sortAsc ? 'desc' : 'asc')
-                    }
-                })
-
-                return header
-            },
             getListHeaderEmpty: () => listHeaderEmpty.content.cloneNode(true),
-            getColGroup: () => templateCollGroup.content.cloneNode(true),
             getResultTBody: ({
                 testId,
                 id,
                 log,
                 duration,
                 extras,
                 resultsTableRow,
                 tableHtml,
                 result,
                 collapsed
             }) => {
                 const resultLower = result.toLowerCase()
-                let formattedDuration = formatDuration(duration)
-                formattedDuration = formatDuration < 1 ? formattedDuration.ms : formattedDuration.formatted
                 const resultBody = templateResult.content.cloneNode(true)
                 resultBody.querySelector('tbody').classList.add(resultLower)
                 resultBody.querySelector('tbody').id = testId
-                resultBody.querySelector('.col-result').innerText = result
-                resultBody.querySelector('.col-result').classList.add(`${collapsed ? 'expander' : 'collapser'}`)
-                resultBody.querySelector('.col-result').dataset.id = id
-                resultBody.querySelector('.col-name').innerText = testId
+                resultBody.querySelector('.collapsible').dataset.id = id
 
-                resultBody.querySelector('.col-duration').innerText = duration < 1 ? formatDuration(duration).ms : formatDuration(duration).formatted
+                resultsTableRow.forEach((html) => {
+                    const t = document.createElement('template')
+                    t.innerHTML = html
+                    resultBody.querySelector('.collapsible').appendChild(t.content)
+                })
 
                 if (log) {
                     // Wrap lines starting with "E" with span.error to color those lines red
                     const wrappedLog = log.replace(/^E.*$/gm, (match) => `<span class="error">${match}</span>`)
                     resultBody.querySelector('.log').innerHTML = wrappedLog
                 } else {
                     resultBody.querySelector('.log').remove()
                 }
 
                 if (collapsed) {
+                    resultBody.querySelector('.collapsible > td')?.classList.add('collapsed')
                     resultBody.querySelector('.extras-row').classList.add('hidden')
+                } else {
+                    resultBody.querySelector('.collapsible > td')?.classList.remove('collapsed')
                 }
 
                 const media = []
                 extras?.forEach(({
                     name,
                     format_type,
                     content
                 }) => {
-                    if (['json', 'text', 'url'].includes(format_type)) {
-                        const extraLink = aTag.content.cloneNode(true)
-                        const extraLinkItem = extraLink.querySelector('a')
-
-                        extraLinkItem.href = content
-                        extraLinkItem.className = `col-links__extra ${format_type}`
-                        extraLinkItem.innerText = name
-                        resultBody.querySelector('.col-links').appendChild(extraLinkItem)
-                    }
-
                     if (['image', 'video'].includes(format_type)) {
                         media.push({
                             path: content,
                             name,
                             format_type
                         })
                     }
 
                     if (format_type === 'html') {
                         resultBody.querySelector('.extraHTML').insertAdjacentHTML('beforeend', `<div>${content}</div>`)
                     }
                 })
-                mediaViewer.setUp(resultBody, media)
-
-                // Add custom html from the pytest_html_results_table_row hook
-                const rows = transformTableObj(resultsTableRow)
-                resultsTableRow && insertAdditionalHTML(rows.inserts, resultBody, 'td')
-                resultsTableRow && insertAdditionalHTML(rows.appends, resultBody, 'tr', 'beforeend')
+                mediaViewer.setup(resultBody, media)
 
                 // Add custom html from the pytest_html_results_table_html hook
                 tableHtml?.forEach((item) => {
                     resultBody.querySelector('td[class="extra"]').insertAdjacentHTML('beforeend', item)
                 })
 
                 return resultBody
             },
         }
 
-        exports.dom = dom
-        exports.htmlToElements = htmlToElements
-        exports.find = find
-        exports.findAll = findAll
+        module.exports = {
+            dom,
+            htmlToElements,
+            find,
+            findAll,
+        }
 
     }, {
-        "./mediaviewer.js": 6,
-        "./storage.js": 8,
-        "./utils.js": 9
+        "./mediaviewer.js": 6
     }],
     3: [function(require, module, exports) {
         const {
             manager
         } = require('./datamanager.js')
+        const {
+            doSort
+        } = require('./sort.js')
         const storageModule = require('./storage.js')
 
         const getFilteredSubSet = (filter) =>
             manager.allData.tests.filter(({
                 result
             }) => filter.includes(result.toLowerCase()))
 
@@ -305,275 +256,261 @@
             if (show) {
                 storageModule.showCategory(type)
             } else {
                 storageModule.hideCategory(type)
             }
 
             const currentFilter = storageModule.getVisible()
+            const filteredSubset = getFilteredSubSet(currentFilter)
+            manager.setRender(filteredSubset)
 
-            if (currentFilter.length) {
-                const filteredSubset = getFilteredSubSet(currentFilter)
-                manager.setRender(filteredSubset)
-            } else {
-                manager.resetRender()
-            }
+            const sortColumn = storageModule.getSort()
+            doSort(sortColumn, true)
         }
 
         module.exports = {
             doFilter,
             doInitFilter,
         }
 
     }, {
         "./datamanager.js": 1,
+        "./sort.js": 7,
         "./storage.js": 8
     }],
     4: [function(require, module, exports) {
         const {
             redraw,
-            bindEvents
+            bindEvents,
+            renderStatic
         } = require('./main.js')
         const {
             doInitFilter
         } = require('./filter.js')
         const {
             doInitSort
         } = require('./sort.js')
         const {
             manager
         } = require('./datamanager.js')
-        const data = JSON.parse(document.querySelector('#data-container').dataset.jsonblob)
+        const data = JSON.parse(document.getElementById('data-container').dataset.jsonblob)
 
         function init() {
             manager.setManager(data)
             doInitFilter()
             doInitSort()
+            renderStatic()
             redraw()
             bindEvents()
         }
 
         init()
 
     }, {
         "./datamanager.js": 1,
         "./filter.js": 3,
         "./main.js": 5,
         "./sort.js": 7
     }],
     5: [function(require, module, exports) {
         const {
-            formatDuration
-        } = require('./utils.js')
-        const {
             dom,
             findAll
         } = require('./dom.js')
         const {
             manager
         } = require('./datamanager.js')
         const {
             doSort
         } = require('./sort.js')
         const {
             doFilter
         } = require('./filter.js')
         const {
             getVisible,
-            possibleResults
+            getCollapsedIds,
+            setCollapsedIds,
+            getSort,
+            getSortDirection,
+            possibleFilters,
         } = require('./storage.js')
 
         const removeChildren = (node) => {
             while (node.firstChild) {
                 node.removeChild(node.firstChild)
             }
         }
 
         const renderStatic = () => {
-            const renderTitle = () => {
-                const title = manager.title
-                document.querySelector('#title').innerText = title
-                document.querySelector('#head-title').innerText = title
-            }
-            const renderTable = () => {
+            const renderEnvironmentTable = () => {
                 const environment = manager.environment
                 const rows = Object.keys(environment).map((key) => dom.getStaticRow(key, environment[key]))
-                const table = document.querySelector('#environment')
+                const table = document.getElementById('environment')
                 removeChildren(table)
                 rows.forEach((row) => table.appendChild(row))
             }
-            renderTitle()
-            renderTable()
+            renderEnvironmentTable()
         }
 
         const renderContent = (tests) => {
+            const sortAttr = getSort(manager.initialSort)
+            const sortAsc = JSON.parse(getSortDirection())
             const rows = tests.map(dom.getResultTBody)
-            const table = document.querySelector('#results-table')
+            const table = document.getElementById('results-table')
+            const tableHeader = document.getElementById('template_results-table__head').content.cloneNode(true)
+
             removeChildren(table)
-            const tableHeader = dom.getListHeader(manager.renderData)
+
+            tableHeader.querySelector(`.sortable[data-column-type="${sortAttr}"]`)?.classList.add(sortAsc ? 'desc' : 'asc')
             if (!rows.length) {
                 tableHeader.appendChild(dom.getListHeaderEmpty())
             }
-            table.appendChild(dom.getColGroup())
             table.appendChild(tableHeader)
 
             rows.forEach((row) => !!row && table.appendChild(row))
 
             table.querySelectorAll('.extra').forEach((item) => {
                 item.colSpan = document.querySelectorAll('th').length
             })
 
-            const {
-                headerPops
-            } = manager.renderData
-            if (headerPops > 0) {
-                // remove 'headerPops' number of header columns
-                findAll('#results-table-head th').splice(-headerPops).forEach(column => column.remove())
-
-                // remove 'headerPops' number of row columns
-                const resultRows = findAll('.results-table-row')
-                resultRows.forEach((elem) => {
-                    findAll('td:not(.extra)', elem).splice(-headerPops).forEach(column => column.remove())
-                })
-            }
-
             findAll('.sortable').forEach((elem) => {
                 elem.addEventListener('click', (evt) => {
                     const {
                         target: element
                     } = evt
                     const {
                         columnType
                     } = element.dataset
                     doSort(columnType)
                     redraw()
                 })
             })
-            findAll('.col-result').forEach((elem) => {
+
+            findAll('.collapsible td:not(.col-links').forEach((elem) => {
                 elem.addEventListener('click', ({
                     target
                 }) => {
-                    manager.toggleCollapsedItem(target.dataset.id)
+                    const id = target.parentElement.dataset.id
+                    manager.toggleCollapsedItem(id)
+
+                    const collapsedIds = getCollapsedIds()
+                    if (collapsedIds.includes(id)) {
+                        const updated = collapsedIds.filter((item) => item !== id)
+                        setCollapsedIds(updated)
+                    } else {
+                        collapsedIds.push(id)
+                        setCollapsedIds(collapsedIds)
+                    }
                     redraw()
                 })
             })
         }
 
-        const renderDerived = (tests, collectedItems, isFinished) => {
+        const renderDerived = () => {
             const currentFilter = getVisible()
-            possibleResults.forEach(({
-                result,
-                label
-            }) => {
-                const count = tests.filter((test) => test.result.toLowerCase() === result).length
+            possibleFilters.forEach((result) => {
                 const input = document.querySelector(`input[data-test-result="${result}"]`)
-                const lastInput = document.querySelector(`input[data-test-result="${result}"]:last-of-type`)
-                document.querySelector(`.${result}`).innerText = `${count} ${label}`
-                // add a comma and whitespace between the results
-                if (input !== lastInput) {
-                    document.querySelector(`.${result}`).innerText += ', '
-                }
-
-                input.disabled = !count
                 input.checked = currentFilter.includes(result)
             })
-
-            const numberOfTests = tests.filter(({
-                result
-            }) => ['Passed', 'Failed', 'XPassed', 'XFailed'].includes(result)).length
-
-            if (isFinished) {
-                const accTime = tests.reduce((prev, {
-                    duration
-                }) => prev + duration, 0)
-                const formattedAccTime = formatDuration(accTime)
-                const testWord = numberOfTests > 1 ? 'tests' : 'test'
-                const durationText = formattedAccTime.hasOwnProperty('ms') ? formattedAccTime.ms : formattedAccTime.formatted
-
-                document.querySelector('.run-count').innerText = `${numberOfTests} ${testWord} took ${durationText}.`
-                document.querySelector('.summary__reload__button').classList.add('hidden')
-            } else {
-                document.querySelector('.run-count').innerText = `${numberOfTests} / ${collectedItems} tests done`
-            }
         }
 
         const bindEvents = () => {
             const filterColumn = (evt) => {
                 const {
                     target: element
                 } = evt
                 const {
                     testResult
                 } = element.dataset
 
                 doFilter(testResult, element.checked)
+                const collapsedIds = getCollapsedIds()
+                const updated = manager.renderData.tests.map((test) => {
+                    return {
+                        ...test,
+                        collapsed: collapsedIds.includes(test.id),
+                    }
+                })
+                manager.setRender(updated)
                 redraw()
             }
+
+            const header = document.getElementById('environment-header')
+            header.addEventListener('click', () => {
+                const table = document.getElementById('environment')
+                table.classList.toggle('hidden')
+                header.classList.toggle('collapsed')
+            })
+
             findAll('input[name="filter_checkbox"]').forEach((elem) => {
-                elem.removeEventListener('click', filterColumn)
                 elem.addEventListener('click', filterColumn)
             })
-            document.querySelector('#show_all_details').addEventListener('click', () => {
+            document.getElementById('show_all_details').addEventListener('click', () => {
                 manager.allCollapsed = false
+                setCollapsedIds([])
                 redraw()
             })
-            document.querySelector('#hide_all_details').addEventListener('click', () => {
+            document.getElementById('hide_all_details').addEventListener('click', () => {
                 manager.allCollapsed = true
+                const allIds = manager.renderData.tests.map((test) => test.id)
+                setCollapsedIds(allIds)
                 redraw()
             })
         }
 
         const redraw = () => {
             const {
-                testSubset,
-                allTests,
-                collectedItems,
-                isFinished
+                testSubset
             } = manager
 
-            renderStatic()
             renderContent(testSubset)
-            renderDerived(allTests, collectedItems, isFinished)
+            renderDerived()
         }
 
-        exports.redraw = redraw
-        exports.bindEvents = bindEvents
+        module.exports = {
+            redraw,
+            bindEvents,
+            renderStatic,
+        }
 
     }, {
         "./datamanager.js": 1,
         "./dom.js": 2,
         "./filter.js": 3,
         "./sort.js": 7,
-        "./storage.js": 8,
-        "./utils.js": 9
+        "./storage.js": 8
     }],
     6: [function(require, module, exports) {
         class MediaViewer {
             constructor(assets) {
                 this.assets = assets
                 this.index = 0
             }
+
             nextActive() {
                 this.index = this.index === this.assets.length - 1 ? 0 : this.index + 1
                 return [this.activeFile, this.index]
             }
+
             prevActive() {
                 this.index = this.index === 0 ? this.assets.length - 1 : this.index - 1
                 return [this.activeFile, this.index]
             }
 
             get currentIndex() {
                 return this.index
             }
+
             get activeFile() {
                 return this.assets[this.index]
             }
         }
 
 
-        const setUp = (resultBody, assets) => {
+        const setup = (resultBody, assets) => {
             if (!assets.length) {
                 resultBody.querySelector('.media').classList.add('hidden')
                 return
             }
 
             const mediaViewer = new MediaViewer(assets)
             const leftArrow = resultBody.querySelector('.media-container__nav--left')
@@ -615,15 +552,17 @@
             }
 
             leftArrow.addEventListener('click', moveLeft)
             rightArrow.addEventListener('click', doRight)
             imageEl.addEventListener('click', openImg)
         }
 
-        exports.setUp = setUp
+        module.exports = {
+            setup,
+        }
 
     }, {}],
     7: [function(require, module, exports) {
         const {
             manager
         } = require('./datamanager.js')
         const storageModule = require('./storage.js')
@@ -631,217 +570,205 @@
         const genericSort = (list, key, ascending, customOrder) => {
             let sorted
             if (customOrder) {
                 sorted = list.sort((a, b) => {
                     const aValue = a.result.toLowerCase()
                     const bValue = b.result.toLowerCase()
 
-                    const aIndex = customOrder.findIndex(item => item.toLowerCase() === aValue)
-                    const bIndex = customOrder.findIndex(item => item.toLowerCase() === bValue)
+                    const aIndex = customOrder.findIndex((item) => item.toLowerCase() === aValue)
+                    const bIndex = customOrder.findIndex((item) => item.toLowerCase() === bValue)
 
                     // Compare the indices to determine the sort order
                     return aIndex - bIndex
                 })
             } else {
                 sorted = list.sort((a, b) => a[key] === b[key] ? 0 : a[key] > b[key] ? 1 : -1)
             }
 
             if (ascending) {
                 sorted.reverse()
             }
             return sorted
         }
 
+        const durationSort = (list, ascending) => {
+            const parseDuration = (duration) => {
+                if (duration.includes(':')) {
+                    // If it's in the format "HH:mm:ss"
+                    const [hours, minutes, seconds] = duration.split(':').map(Number)
+                    return (hours * 3600 + minutes * 60 + seconds) * 1000
+                } else {
+                    // If it's in the format "nnn ms"
+                    return parseInt(duration)
+                }
+            }
+            const sorted = list.sort((a, b) => parseDuration(a['duration']) - parseDuration(b['duration']))
+            if (ascending) {
+                sorted.reverse()
+            }
+            return sorted
+        }
+
         const doInitSort = () => {
-            const type = storageModule.getSort()
+            const type = storageModule.getSort(manager.initialSort)
             const ascending = storageModule.getSortDirection()
             const list = manager.testSubset
             const initialOrder = ['Error', 'Failed', 'Rerun', 'XFailed', 'XPassed', 'Skipped', 'Passed']
+
+            storageModule.setSort(type)
+            storageModule.setSortDirection(ascending)
+
             if (type?.toLowerCase() === 'original') {
                 manager.setRender(list)
             } else {
-                const sortedList = genericSort(list, type, ascending, initialOrder)
+                let sortedList
+                switch (type) {
+                    case 'duration':
+                        sortedList = durationSort(list, ascending)
+                        break
+                    case 'result':
+                        sortedList = genericSort(list, type, ascending, initialOrder)
+                        break
+                    default:
+                        sortedList = genericSort(list, type, ascending)
+                        break
+                }
                 manager.setRender(sortedList)
             }
         }
 
-        const doSort = (type) => {
-            const newSortType = storageModule.getSort() !== type
+        const doSort = (type, skipDirection) => {
+            const newSortType = storageModule.getSort(manager.initialSort) !== type
             const currentAsc = storageModule.getSortDirection()
-            const ascending = newSortType ? true : !currentAsc
+            let ascending
+            if (skipDirection) {
+                ascending = currentAsc
+            } else {
+                ascending = newSortType ? false : !currentAsc
+            }
             storageModule.setSort(type)
             storageModule.setSortDirection(ascending)
-            const list = manager.testSubset
 
-            const sortedList = genericSort(list, type, ascending)
+            const list = manager.testSubset
+            const sortedList = type === 'duration' ? durationSort(list, ascending) : genericSort(list, type, ascending)
             manager.setRender(sortedList)
         }
 
-        exports.doSort = doSort
-        exports.doInitSort = doInitSort
+        module.exports = {
+            doInitSort,
+            doSort,
+        }
 
     }, {
         "./datamanager.js": 1,
         "./storage.js": 8
     }],
     8: [function(require, module, exports) {
-        const possibleResults = [{
-            result: 'passed',
-            label: 'Passed'
-        }, {
-            result: 'skipped',
-            label: 'Skipped'
-        }, {
-            result: 'failed',
-            label: 'Failed'
-        }, {
-            result: 'error',
-            label: 'Errors'
-        }, {
-            result: 'xfailed',
-            label: 'Unexpected failures'
-        }, {
-            result: 'xpassed',
-            label: 'Unexpected passes'
-        }, {
-            result: 'rerun',
-            label: 'Reruns'
-        }, ]
-        const possibleFilters = possibleResults.map((item) => item.result)
+        const possibleFilters = [
+            'passed',
+            'skipped',
+            'failed',
+            'error',
+            'xfailed',
+            'xpassed',
+            'rerun',
+        ]
 
         const getVisible = () => {
             const url = new URL(window.location.href)
-            const settings = new URLSearchParams(url.search).get('visible') || ''
-            return settings ? [...new Set(settings.split(',').filter((filter) => possibleFilters.includes(filter)))] : possibleFilters
+            const settings = new URLSearchParams(url.search).get('visible')
+            const lower = (item) => {
+                const lowerItem = item.toLowerCase()
+                if (possibleFilters.includes(lowerItem)) {
+                    return lowerItem
+                }
+                return null
+            }
+            return settings === null ?
+                possibleFilters : [...new Set(settings?.split(',').map(lower).filter((item) => item))]
         }
+
         const hideCategory = (categoryToHide) => {
             const url = new URL(window.location.href)
             const visibleParams = new URLSearchParams(url.search).get('visible')
             const currentVisible = visibleParams ? visibleParams.split(',') : [...possibleFilters]
             const settings = [...new Set(currentVisible)].filter((f) => f !== categoryToHide).join(',')
 
             url.searchParams.set('visible', settings)
-            history.pushState({}, null, unescape(url.href))
+            window.history.pushState({}, null, unescape(url.href))
         }
 
         const showCategory = (categoryToShow) => {
             if (typeof window === 'undefined') {
                 return
             }
             const url = new URL(window.location.href)
-            const currentVisible = new URLSearchParams(url.search).get('visible')?.split(',') || [...possibleFilters]
+            const currentVisible = new URLSearchParams(url.search).get('visible')?.split(',').filter(Boolean) || [...possibleFilters]
             const settings = [...new Set([categoryToShow, ...currentVisible])]
             const noFilter = possibleFilters.length === settings.length || !settings.length
 
             noFilter ? url.searchParams.delete('visible') : url.searchParams.set('visible', settings.join(','))
-            history.pushState({}, null, unescape(url.href))
+            window.history.pushState({}, null, unescape(url.href))
         }
-        const setFilter = (currentFilter) => {
-            if (!possibleFilters.includes(currentFilter)) {
-                return
-            }
-            const url = new URL(window.location.href)
-            const settings = [currentFilter, ...new Set(new URLSearchParams(url.search).get('filter').split(','))]
 
-            url.searchParams.set('filter', settings)
-            history.pushState({}, null, unescape(url.href))
-        }
-
-        const getSort = () => {
+        const getSort = (initialSort) => {
             const url = new URL(window.location.href)
-            return new URLSearchParams(url.search).get('sort') || 'result'
+            let sort = new URLSearchParams(url.search).get('sort')
+            if (!sort) {
+                sort = initialSort || 'result'
+            }
+            return sort
         }
+
         const setSort = (type) => {
             const url = new URL(window.location.href)
             url.searchParams.set('sort', type)
-            history.pushState({}, null, unescape(url.href))
+            window.history.pushState({}, null, unescape(url.href))
         }
 
-        const getCollapsedCategory = (config) => {
+        const getCollapsedCategory = (renderCollapsed) => {
             let categories
             if (typeof window !== 'undefined') {
                 const url = new URL(window.location.href)
                 const collapsedItems = new URLSearchParams(url.search).get('collapsed')
                 switch (true) {
-                    case !config && collapsedItems === null:
+                    case !renderCollapsed && collapsedItems === null:
                         categories = ['passed']
                         break
                     case collapsedItems?.length === 0 || /^["']{2}$/.test(collapsedItems):
                         categories = []
                         break
-                    case /^all$/.test(collapsedItems) || (collapsedItems === null && /^all$/.test(config)):
+                    case /^all$/.test(collapsedItems) || collapsedItems === null && /^all$/.test(renderCollapsed):
                         categories = [...possibleFilters]
                         break
                     default:
-                        categories = collapsedItems?.split(',').map(item => item.toLowerCase()) || config
+                        categories = collapsedItems?.split(',').map((item) => item.toLowerCase()) || renderCollapsed
                         break
                 }
             } else {
                 categories = []
             }
             return categories
         }
 
-        const getSortDirection = () => JSON.parse(sessionStorage.getItem('sortAsc'))
-
+        const getSortDirection = () => JSON.parse(sessionStorage.getItem('sortAsc')) || false
         const setSortDirection = (ascending) => sessionStorage.setItem('sortAsc', ascending)
 
+        const getCollapsedIds = () => JSON.parse(sessionStorage.getItem('collapsedIds')) || []
+        const setCollapsedIds = (list) => sessionStorage.setItem('collapsedIds', JSON.stringify(list))
+
         module.exports = {
             getVisible,
-            setFilter,
             hideCategory,
             showCategory,
+            getCollapsedIds,
+            setCollapsedIds,
             getSort,
-            getSortDirection,
             setSort,
+            getSortDirection,
             setSortDirection,
             getCollapsedCategory,
             possibleFilters,
-            possibleResults,
-        }
-
-    }, {}],
-    9: [function(require, module, exports) {
-        const formattedNumber = (number) =>
-            number.toLocaleString('en-US', {
-                minimumIntegerDigits: 2,
-                useGrouping: false,
-            })
-
-        const formatDuration = (totalSeconds) => {
-            if (totalSeconds < 1) {
-                return {
-                    ms: `${Math.round(totalSeconds * 1000)} ms`
-                }
-            }
-
-            const hours = Math.floor(totalSeconds / 3600)
-            let remainingSeconds = totalSeconds % 3600
-            const minutes = Math.floor(remainingSeconds / 60)
-            remainingSeconds = remainingSeconds % 60
-            const seconds = Math.round(remainingSeconds)
-
-            return {
-                seconds: `${Math.round(totalSeconds)} seconds`,
-                formatted: `${formattedNumber(hours)}:${formattedNumber(minutes)}:${formattedNumber(seconds)}`,
-            }
-        }
-
-        const transformTableObj = (obj) => {
-            const appends = {}
-            const inserts = {}
-            for (const key in obj) {
-                key.startsWith("Z") ? appends[key] = obj[key] : inserts[key] = obj[key]
-            }
-            return {
-                appends,
-                inserts,
-            }
-        }
-
-        module.exports = {
-            formatDuration,
-            transformTableObj,
         }
 
     }, {}]
 }, {}, [4]);
```

### Comparing `pytest_html-4.0.0rc4/src/pytest_html/resources/style.css` & `pytest_html-4.0.0rc5/src/pytest_html/resources/style.css`

 * *Files 4% similar despite different names*

```diff
@@ -160,52 +160,64 @@
   display: flex;
   flex-direction: row;
   justify-content: space-around;
   flex: 0 0 25px;
   align-items: center;
 }
 
-.collapsed {
-  display: none;
-}
-
-.col-result {
+.collapsible td:not(.col-links) {
   cursor: pointer;
 }
-.col-result:hover::after {
+.collapsible td:not(.col-links):hover::after {
   color: #bbb;
   font-style: italic;
   cursor: pointer;
 }
 
-.col-result.collapser:hover::after {
+.col-result:hover::after {
+  content: " (hide details)";
+}
+
+.col-result.collapsed:hover::after {
+  content: " (show details)";
+}
+
+#environment-header h2:hover::after {
   content: " (hide details)";
+  color: #bbb;
+  font-style: italic;
+  cursor: pointer;
+  font-size: 12px;
 }
 
-.col-result.expander:hover::after {
+#environment-header.collapsed h2:hover::after {
   content: " (show details)";
+  color: #bbb;
+  font-style: italic;
+  cursor: pointer;
+  font-size: 12px;
 }
 
 /*------------------
  * 3. Sorting items
  *------------------*/
 .sortable {
   cursor: pointer;
 }
-.sortable.asc:after {
+.sortable.desc:after {
   content: " ";
   position: relative;
   left: 5px;
   bottom: -12.5px;
   border: 10px solid #4caf50;
   border-bottom: 0;
   border-left-color: transparent;
   border-right-color: transparent;
 }
-.sortable.desc:after {
+.sortable.asc:after {
   content: " ";
   position: relative;
   left: 5px;
   bottom: 12.5px;
   border: 10px solid #4caf50;
   border-top: 0;
   border-left-color: transparent;
```

### Comparing `pytest_html-4.0.0rc4/src/pytest_html/scripts/datamanager.js` & `pytest_html-4.0.0rc5/src/pytest_html/scripts/datamanager.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,77 +1,85 @@
 const {
-    getCollapsedCategory
+    getCollapsedCategory,
+    setCollapsedIds
 } = require('./storage.js')
 
 class DataManager {
     setManager(data) {
-        const collapsedCategories = [...getCollapsedCategory(data.collapsed)]
+        const collapsedCategories = [...getCollapsedCategory(data.renderCollapsed)]
+        const collapsedIds = []
+        const tests = Object.values(data.tests).flat().map((test, index) => {
+            const collapsed = collapsedCategories.includes(test.result.toLowerCase())
+            const id = `test_${index}`
+            if (collapsed) {
+                collapsedIds.push(id)
+            }
+            return {
+                ...test,
+                id,
+                collapsed,
+            }
+        })
         const dataBlob = {
             ...data,
-            tests: Object.values(data.tests).flat().map((test, index) => ({
-                ...test,
-                id: `test_${index}`,
-                collapsed: collapsedCategories.includes(test.result.toLowerCase()),
-            }))
+            tests
         }
         this.data = {
             ...dataBlob
         }
         this.renderData = {
             ...dataBlob
         }
+        setCollapsedIds(collapsedIds)
     }
 
     get allData() {
         return {
             ...this.data
         }
     }
+
     resetRender() {
         this.renderData = {
             ...this.data
         }
     }
+
     setRender(data) {
         this.renderData.tests = [...data]
     }
+
     toggleCollapsedItem(id) {
         this.renderData.tests = this.renderData.tests.map((test) =>
             test.id === id ? {
                 ...test,
                 collapsed: !test.collapsed
             } : test,
         )
     }
+
     set allCollapsed(collapsed) {
         this.renderData = {
             ...this.renderData,
             tests: [...this.renderData.tests.map((test) => ({
                 ...test,
                 collapsed
             }))]
         }
     }
 
     get testSubset() {
         return [...this.renderData.tests]
     }
-    get allTests() {
-        return [...this.data.tests]
-    }
-    get title() {
-        return this.renderData.title
-    }
+
     get environment() {
         return this.renderData.environment
     }
-    get collectedItems() {
-        return this.renderData.collectedItems
-    }
-    get isFinished() {
-        return this.data.runningState === 'Finished'
+
+    get initialSort() {
+        return this.data.initialSort
     }
 }
 
 module.exports = {
     manager: new DataManager(),
 }
```

### Comparing `pytest_html-4.0.0rc4/src/pytest_html/scripts/filter.js` & `pytest_html-4.0.0rc5/src/pytest_html/scripts/filter.js`

 * *Files 24% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,13 @@
 const {
     manager
 } = require('./datamanager.js')
+const {
+    doSort
+} = require('./sort.js')
 const storageModule = require('./storage.js')
 
 const getFilteredSubSet = (filter) =>
     manager.allData.tests.filter(({
         result
     }) => filter.includes(result.toLowerCase()))
 
@@ -18,20 +21,18 @@
     if (show) {
         storageModule.showCategory(type)
     } else {
         storageModule.hideCategory(type)
     }
 
     const currentFilter = storageModule.getVisible()
+    const filteredSubset = getFilteredSubSet(currentFilter)
+    manager.setRender(filteredSubset)
 
-    if (currentFilter.length) {
-        const filteredSubset = getFilteredSubSet(currentFilter)
-        manager.setRender(filteredSubset)
-    } else {
-        manager.resetRender()
-    }
+    const sortColumn = storageModule.getSort()
+    doSort(sortColumn, true)
 }
 
 module.exports = {
     doFilter,
     doInitFilter,
 }
```

### Comparing `pytest_html-4.0.0rc4/src/pytest_html/scripts/mediaviewer.js` & `pytest_html-4.0.0rc5/src/pytest_html/scripts/mediaviewer.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -1,31 +1,34 @@
 class MediaViewer {
     constructor(assets) {
         this.assets = assets
         this.index = 0
     }
+
     nextActive() {
         this.index = this.index === this.assets.length - 1 ? 0 : this.index + 1
         return [this.activeFile, this.index]
     }
+
     prevActive() {
         this.index = this.index === 0 ? this.assets.length - 1 : this.index - 1
         return [this.activeFile, this.index]
     }
 
     get currentIndex() {
         return this.index
     }
+
     get activeFile() {
         return this.assets[this.index]
     }
 }
 
 
-const setUp = (resultBody, assets) => {
+const setup = (resultBody, assets) => {
     if (!assets.length) {
         resultBody.querySelector('.media').classList.add('hidden')
         return
     }
 
     const mediaViewer = new MediaViewer(assets)
     const leftArrow = resultBody.querySelector('.media-container__nav--left')
@@ -67,8 +70,10 @@
     }
 
     leftArrow.addEventListener('click', moveLeft)
     rightArrow.addEventListener('click', doRight)
     imageEl.addEventListener('click', openImg)
 }
 
-exports.setUp = setUp
+module.exports = {
+    setup,
+}
```

### Comparing `pytest_html-4.0.0rc4/src/pytest_html/scripts/sort.js` & `pytest_html-4.0.0rc5/src/pytest_html/scripts/sort.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -6,50 +6,90 @@
 const genericSort = (list, key, ascending, customOrder) => {
     let sorted
     if (customOrder) {
         sorted = list.sort((a, b) => {
             const aValue = a.result.toLowerCase()
             const bValue = b.result.toLowerCase()
 
-            const aIndex = customOrder.findIndex(item => item.toLowerCase() === aValue)
-            const bIndex = customOrder.findIndex(item => item.toLowerCase() === bValue)
+            const aIndex = customOrder.findIndex((item) => item.toLowerCase() === aValue)
+            const bIndex = customOrder.findIndex((item) => item.toLowerCase() === bValue)
 
             // Compare the indices to determine the sort order
             return aIndex - bIndex
         })
     } else {
         sorted = list.sort((a, b) => a[key] === b[key] ? 0 : a[key] > b[key] ? 1 : -1)
     }
 
     if (ascending) {
         sorted.reverse()
     }
     return sorted
 }
 
+const durationSort = (list, ascending) => {
+    const parseDuration = (duration) => {
+        if (duration.includes(':')) {
+            // If it's in the format "HH:mm:ss"
+            const [hours, minutes, seconds] = duration.split(':').map(Number)
+            return (hours * 3600 + minutes * 60 + seconds) * 1000
+        } else {
+            // If it's in the format "nnn ms"
+            return parseInt(duration)
+        }
+    }
+    const sorted = list.sort((a, b) => parseDuration(a['duration']) - parseDuration(b['duration']))
+    if (ascending) {
+        sorted.reverse()
+    }
+    return sorted
+}
+
 const doInitSort = () => {
-    const type = storageModule.getSort()
+    const type = storageModule.getSort(manager.initialSort)
     const ascending = storageModule.getSortDirection()
     const list = manager.testSubset
     const initialOrder = ['Error', 'Failed', 'Rerun', 'XFailed', 'XPassed', 'Skipped', 'Passed']
+
+    storageModule.setSort(type)
+    storageModule.setSortDirection(ascending)
+
     if (type?.toLowerCase() === 'original') {
         manager.setRender(list)
     } else {
-        const sortedList = genericSort(list, type, ascending, initialOrder)
+        let sortedList
+        switch (type) {
+            case 'duration':
+                sortedList = durationSort(list, ascending)
+                break
+            case 'result':
+                sortedList = genericSort(list, type, ascending, initialOrder)
+                break
+            default:
+                sortedList = genericSort(list, type, ascending)
+                break
+        }
         manager.setRender(sortedList)
     }
 }
 
-const doSort = (type) => {
-    const newSortType = storageModule.getSort() !== type
+const doSort = (type, skipDirection) => {
+    const newSortType = storageModule.getSort(manager.initialSort) !== type
     const currentAsc = storageModule.getSortDirection()
-    const ascending = newSortType ? true : !currentAsc
+    let ascending
+    if (skipDirection) {
+        ascending = currentAsc
+    } else {
+        ascending = newSortType ? false : !currentAsc
+    }
     storageModule.setSort(type)
     storageModule.setSortDirection(ascending)
-    const list = manager.testSubset
 
-    const sortedList = genericSort(list, type, ascending)
+    const list = manager.testSubset
+    const sortedList = type === 'duration' ? durationSort(list, ascending) : genericSort(list, type, ascending)
     manager.setRender(sortedList)
 }
 
-exports.doSort = doSort
-exports.doInitSort = doInitSort
+module.exports = {
+    doInitSort,
+    doSort,
+}
```

### Comparing `pytest_html-4.0.0rc4/src/pytest_html/scripts/storage.js` & `pytest_html-4.0.0rc5/src/pytest_html/scripts/storage.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -1,114 +1,106 @@
-const possibleResults = [{
-    result: 'passed',
-    label: 'Passed'
-}, {
-    result: 'skipped',
-    label: 'Skipped'
-}, {
-    result: 'failed',
-    label: 'Failed'
-}, {
-    result: 'error',
-    label: 'Errors'
-}, {
-    result: 'xfailed',
-    label: 'Unexpected failures'
-}, {
-    result: 'xpassed',
-    label: 'Unexpected passes'
-}, {
-    result: 'rerun',
-    label: 'Reruns'
-}, ]
-const possibleFilters = possibleResults.map((item) => item.result)
+const possibleFilters = [
+    'passed',
+    'skipped',
+    'failed',
+    'error',
+    'xfailed',
+    'xpassed',
+    'rerun',
+]
 
 const getVisible = () => {
     const url = new URL(window.location.href)
-    const settings = new URLSearchParams(url.search).get('visible') || ''
-    return settings ? [...new Set(settings.split(',').filter((filter) => possibleFilters.includes(filter)))] : possibleFilters
+    const settings = new URLSearchParams(url.search).get('visible')
+    const lower = (item) => {
+        const lowerItem = item.toLowerCase()
+        if (possibleFilters.includes(lowerItem)) {
+            return lowerItem
+        }
+        return null
+    }
+    return settings === null ?
+        possibleFilters : [...new Set(settings?.split(',').map(lower).filter((item) => item))]
 }
+
 const hideCategory = (categoryToHide) => {
     const url = new URL(window.location.href)
     const visibleParams = new URLSearchParams(url.search).get('visible')
     const currentVisible = visibleParams ? visibleParams.split(',') : [...possibleFilters]
     const settings = [...new Set(currentVisible)].filter((f) => f !== categoryToHide).join(',')
 
     url.searchParams.set('visible', settings)
-    history.pushState({}, null, unescape(url.href))
+    window.history.pushState({}, null, unescape(url.href))
 }
 
 const showCategory = (categoryToShow) => {
     if (typeof window === 'undefined') {
         return
     }
     const url = new URL(window.location.href)
-    const currentVisible = new URLSearchParams(url.search).get('visible')?.split(',') || [...possibleFilters]
+    const currentVisible = new URLSearchParams(url.search).get('visible')?.split(',').filter(Boolean) || [...possibleFilters]
     const settings = [...new Set([categoryToShow, ...currentVisible])]
     const noFilter = possibleFilters.length === settings.length || !settings.length
 
     noFilter ? url.searchParams.delete('visible') : url.searchParams.set('visible', settings.join(','))
-    history.pushState({}, null, unescape(url.href))
-}
-const setFilter = (currentFilter) => {
-    if (!possibleFilters.includes(currentFilter)) {
-        return
-    }
-    const url = new URL(window.location.href)
-    const settings = [currentFilter, ...new Set(new URLSearchParams(url.search).get('filter').split(','))]
-
-    url.searchParams.set('filter', settings)
-    history.pushState({}, null, unescape(url.href))
+    window.history.pushState({}, null, unescape(url.href))
 }
 
-const getSort = () => {
+const getSort = (initialSort) => {
     const url = new URL(window.location.href)
-    return new URLSearchParams(url.search).get('sort') || 'result'
+    let sort = new URLSearchParams(url.search).get('sort')
+    if (!sort) {
+        sort = initialSort || 'result'
+    }
+    return sort
 }
+
 const setSort = (type) => {
     const url = new URL(window.location.href)
     url.searchParams.set('sort', type)
-    history.pushState({}, null, unescape(url.href))
+    window.history.pushState({}, null, unescape(url.href))
 }
 
-const getCollapsedCategory = (config) => {
+const getCollapsedCategory = (renderCollapsed) => {
     let categories
     if (typeof window !== 'undefined') {
         const url = new URL(window.location.href)
         const collapsedItems = new URLSearchParams(url.search).get('collapsed')
         switch (true) {
-            case !config && collapsedItems === null:
+            case !renderCollapsed && collapsedItems === null:
                 categories = ['passed']
                 break
             case collapsedItems?.length === 0 || /^["']{2}$/.test(collapsedItems):
                 categories = []
                 break
-            case /^all$/.test(collapsedItems) || (collapsedItems === null && /^all$/.test(config)):
+            case /^all$/.test(collapsedItems) || collapsedItems === null && /^all$/.test(renderCollapsed):
                 categories = [...possibleFilters]
                 break
             default:
-                categories = collapsedItems?.split(',').map(item => item.toLowerCase()) || config
+                categories = collapsedItems?.split(',').map((item) => item.toLowerCase()) || renderCollapsed
                 break
         }
     } else {
         categories = []
     }
     return categories
 }
 
-const getSortDirection = () => JSON.parse(sessionStorage.getItem('sortAsc'))
-
+const getSortDirection = () => JSON.parse(sessionStorage.getItem('sortAsc')) || false
 const setSortDirection = (ascending) => sessionStorage.setItem('sortAsc', ascending)
 
+const getCollapsedIds = () => JSON.parse(sessionStorage.getItem('collapsedIds')) || []
+const setCollapsedIds = (list) => sessionStorage.setItem('collapsedIds', JSON.stringify(list))
+
 module.exports = {
     getVisible,
-    setFilter,
     hideCategory,
     showCategory,
+    getCollapsedIds,
+    setCollapsedIds,
     getSort,
-    getSortDirection,
     setSort,
+    getSortDirection,
     setSortDirection,
     getCollapsedCategory,
     possibleFilters,
-    possibleResults,
 }
```

### Comparing `pytest_html-4.0.0rc4/testing/legacy_test_pytest_html.py` & `pytest_html-4.0.0rc5/testing/legacy_test_pytest_html.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,14 @@
                 r'<td class="col-duration">ABC\d{2}  \d{2} \d{2}123</td>',
             ),
         ],
     )
     def test_can_format_duration_column(
         self, testdir, duration_formatter, expected_report_content
     ):
-
         testdir.makeconftest(
             f"""
             import pytest
 
             @pytest.hookimpl(hookwrapper=True)
             def pytest_runtest_makereport(item, call):
                 outcome = yield
```

### Comparing `pytest_html-4.0.0rc4/testing/test_integration.py` & `pytest_html-4.0.0rc5/testing/test_integration.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import os
 import random
 import re
 import urllib.parse
 from base64 import b64encode
 from pathlib import Path
 
-import pkg_resources
 import pytest
 from assertpy import assert_that
 from bs4 import BeautifulSoup
 from selenium import webdriver
 
 pytest_plugins = ("pytester",)
 
@@ -24,20 +23,16 @@
     "xfailed": "Unexpected failures",
     "xpassed": "Unexpected passes",
     "rerun": "Reruns",
 }
 
 
 def run(pytester, path="report.html", cmd_flags=None, query_params=None):
-    if cmd_flags is None:
-        cmd_flags = []
-
-    if query_params is None:
-        query_params = {}
-    query_params = urllib.parse.urlencode(query_params)
+    cmd_flags = cmd_flags or []
+    query_params = urllib.parse.urlencode(query_params) if query_params else {}
 
     path = pytester.path.joinpath(path)
     pytester.runpytest("--html", path, *cmd_flags)
 
     chrome_options = webdriver.ChromeOptions()
     if os.environ.get("CI", False):
         chrome_options.add_argument("--headless")
@@ -89,15 +84,15 @@
 
 
 def get_text(page, selector):
     return get_element(page, selector).string
 
 
 def is_collapsed(page, test_name):
-    return get_element(page, f".summary tbody[id$='{test_name}'] .expander")
+    return get_element(page, f".summary tbody[id$='{test_name}'] .collapsed")
 
 
 def get_log(page, test_id=None):
     # TODO(jim) move to get_text (use .contents)
     if test_id:
         log = get_element(page, f".summary tbody[id$='{test_id}'] div[class='log']")
     else:
@@ -116,14 +111,16 @@
             .joinpath("resources", "style.css")
             .read_bytes()
             .decode("utf-8")
             .strip()
         )
     except AttributeError:
         # Needed for python < 3.9
+        import pkg_resources
+
         return pkg_resources.resource_string(
             "pytest_html", os.path.join("resources", "style.css")
         ).decode("utf-8")
 
 
 class TestHTML:
     @pytest.mark.parametrize(
@@ -649,15 +646,15 @@
                 cells.insert(2, "<td>A description</td>")
                 cells.insert(1, '<td class="col-time">A time</td>')
         """
         )
         pytester.makepyfile("def test_pass(): pass")
         page = run(pytester)
 
-        description_index = 3
+        description_index = 4
         time_index = 2
         assert_that(get_text(page, header_selector.format(time_index))).is_equal_to(
             "Time"
         )
         assert_that(
             get_text(page, header_selector.format(description_index))
         ).is_equal_to("Description")
@@ -758,89 +755,101 @@
             log_cli_date_format = %Y-%m-%d %H:%M:%S
             log_cli_format = %(asctime)s %(levelname)s: %(message)s
         """
         )
 
     @pytest.fixture
     def test_file(self):
-        return """
-            import pytest
-            import logging
-            @pytest.fixture
-            def setup():
-                logging.info("this is setup")
-                {setup}
-                yield
-                logging.info("this is teardown")
-                {teardown}
+        def formatter(assertion, setup="", teardown="", flaky=""):
+            return f"""
+                import pytest
+                import logging
+                @pytest.fixture
+                def setup():
+                    logging.info("this is setup")
+                    {setup}
+                    yield
+                    logging.info("this is teardown")
+                    {teardown}
+
+                {flaky}
+                def test_logging(setup):
+                    logging.info("this is test")
+                    assert {assertion}
+            """
 
-            def test_logging(setup):
-                logging.info("this is test")
-                assert {assertion}
-        """
+        return formatter
 
     @pytest.mark.usefixtures("log_cli")
     def test_all_pass(self, test_file, pytester):
-        pytester.makepyfile(test_file.format(setup="", teardown="", assertion=True))
+        pytester.makepyfile(test_file(assertion=True))
         page = run(pytester)
         assert_results(page, passed=1)
 
         log = get_log(page)
         for when in ["setup", "test", "teardown"]:
             assert_that(log).matches(self.LOG_LINE_REGEX.format(when))
 
     @pytest.mark.usefixtures("log_cli")
     def test_setup_error(self, test_file, pytester):
-        pytester.makepyfile(
-            test_file.format(setup="error", teardown="", assertion=True)
-        )
+        pytester.makepyfile(test_file(assertion=True, setup="error"))
         page = run(pytester)
         assert_results(page, error=1)
 
         log = get_log(page)
         assert_that(log).matches(self.LOG_LINE_REGEX.format("setup"))
         assert_that(log).does_not_match(self.LOG_LINE_REGEX.format("test"))
         assert_that(log).does_not_match(self.LOG_LINE_REGEX.format("teardown"))
 
     @pytest.mark.usefixtures("log_cli")
     def test_test_fails(self, test_file, pytester):
-        pytester.makepyfile(test_file.format(setup="", teardown="", assertion=False))
+        pytester.makepyfile(test_file(assertion=False))
         page = run(pytester)
         assert_results(page, failed=1)
 
         log = get_log(page)
         for when in ["setup", "test", "teardown"]:
             assert_that(log).matches(self.LOG_LINE_REGEX.format(when))
 
     @pytest.mark.usefixtures("log_cli")
     @pytest.mark.parametrize(
         "assertion, result", [(True, {"passed": 1}), (False, {"failed": 1})]
     )
     def test_teardown_error(self, test_file, pytester, assertion, result):
-        pytester.makepyfile(
-            test_file.format(setup="", teardown="error", assertion=assertion)
-        )
+        pytester.makepyfile(test_file(assertion=assertion, teardown="error"))
         page = run(pytester)
         assert_results(page, error=1, **result)
 
         for test_name in ["test_logging", "test_logging::teardown"]:
             log = get_log(page, test_name)
             for when in ["setup", "test", "teardown"]:
                 assert_that(log).matches(self.LOG_LINE_REGEX.format(when))
 
     def test_no_log(self, test_file, pytester):
-        pytester.makepyfile(test_file.format(setup="", teardown="", assertion=True))
+        pytester.makepyfile(test_file(assertion=True))
         page = run(pytester)
         assert_results(page, passed=1)
 
         log = get_log(page, "test_logging")
         assert_that(log).contains("No log output captured.")
         for when in ["setup", "test", "teardown"]:
             assert_that(log).does_not_match(self.LOG_LINE_REGEX.format(when))
 
+    @pytest.mark.usefixtures("log_cli")
+    def test_rerun(self, test_file, pytester):
+        pytester.makepyfile(
+            test_file(assertion=False, flaky="@pytest.mark.flaky(reruns=2)")
+        )
+        page = run(pytester, query_params={"visible": "failed"})
+        assert_results(page, failed=1, rerun=2)
+
+        log = get_log(page)
+        assert_that(log.count("Captured log setup")).is_equal_to(3)
+        assert_that(log.count("Captured log teardown")).is_equal_to(5)
+
 
 class TestCollapsedQueryParam:
     @pytest.fixture
     def test_file(self):
         return """
             import pytest
             @pytest.fixture
```

### Comparing `pytest_html-4.0.0rc4/testing/unittest.js` & `pytest_html-4.0.0rc5/testing/unittest.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -6,24 +6,20 @@
     doInitFilter,
     doFilter
 } = require('../src/pytest_html/scripts/filter.js')
 const {
     doInitSort,
     doSort
 } = require('../src/pytest_html/scripts/sort.js')
-const {
-    formatDuration,
-    transformTableObj
-} = require('../src/pytest_html/scripts/utils.js')
 const dataModule = require('../src/pytest_html/scripts/datamanager.js')
 const storageModule = require('../src/pytest_html/scripts/storage.js')
 
 
 const setTestData = () => {
-    const jsonDatan = {
+    const jsonData = {
         'tests': [{
             'id': 'passed_1',
             'result': 'passed',
         }, {
             'id': 'failed_2',
             'result': 'failed',
         }, {
@@ -36,15 +32,28 @@
             'id': 'passed_5',
             'result': 'passed',
         }, {
             'id': 'passed_6',
             'result': 'passed',
         }, ],
     }
-    dataModule.manager.setManager(jsonDatan)
+    dataModule.manager.setManager(jsonData)
+}
+
+const mockWindow = (queryParam) => {
+    const mock = {
+        location: {
+            href: `https://example.com/page?${queryParam}`,
+        },
+        history: {
+            pushState: sinon.stub(),
+        },
+    }
+    originalWindow = global.window
+    global.window = mock
 }
 
 describe('Filter tests', () => {
     let getFilterMock
     let managerSpy
 
     beforeEach(setTestData)
@@ -72,47 +81,94 @@
             expect(managerSpy.callCount).to.eql(1)
             expect(dataModule.manager.testSubset.map(({
                 result
             }) => result)).to.eql(['failed'])
         })
     })
     describe('doFilter', () => {
-        let setFilterMock
-        afterEach(() => setFilterMock.restore())
+        let originalWindow
+
+        after(() => global.window = originalWindow)
+
         it('removes all but passed', () => {
+            mockWindow()
             getFilterMock = sinon.stub(storageModule, 'getVisible').returns(['passed'])
-            setFilterMock = sinon.stub(storageModule, 'setFilter')
             managerSpy = sinon.spy(dataModule.manager, 'setRender')
 
             doFilter('passed', true)
-            expect(managerSpy.callCount).to.eql(1)
+            expect(managerSpy.callCount).to.eql(2)
             expect(dataModule.manager.testSubset.map(({
                 result
             }) => result)).to.eql([
                 'passed', 'passed', 'passed', 'passed', 'passed',
             ])
         })
     })
+    describe('getVisible', () => {
+        let originalWindow
+
+        after(() => global.window = originalWindow)
+
+        it('returns all filters by default', () => {
+            mockWindow()
+            const visibleItems = storageModule.getVisible()
+            expect(visibleItems).to.eql(storageModule.possibleFilters)
+        })
+
+        it('returns specified filters', () => {
+            mockWindow('visible=failed,error')
+            const visibleItems = storageModule.getVisible()
+            expect(visibleItems).to.eql(['failed', 'error'])
+        })
+
+        it('handles case insensitive params', () => {
+            mockWindow('visible=fAiLeD,ERROR,passed')
+            const visibleItems = storageModule.getVisible()
+            expect(visibleItems).to.eql(['failed', 'error', 'passed'])
+        })
+
+        const falsy = [{
+            param: 'visible'
+        }, {
+            param: 'visible='
+        }, {
+            param: 'visible=""'
+        }, {
+            param: 'visible=\'\''
+        }, ]
+        falsy.forEach(({
+            param
+        }) => {
+            it(`returns no filters with ${param}`, () => {
+                mockWindow(param)
+                const visibleItems = storageModule.getVisible()
+                expect(visibleItems).to.be.empty
+            })
+        })
+    })
 })
 
 
 describe('Sort tests', () => {
     beforeEach(setTestData)
     after(() => dataModule.manager.setManager({
         tests: []
     }))
     describe('doInitSort', () => {
         let managerSpy
         let sortMock
         let sortDirectionMock
-        beforeEach(() => dataModule.manager.resetRender())
+        let originalWindow
 
+        before(() => mockWindow())
+        beforeEach(() => dataModule.manager.resetRender())
         afterEach(() => [sortMock, sortDirectionMock, managerSpy].forEach((fn) => fn.restore()))
+        after(() => global.window = originalWindow)
         it('has no stored sort', () => {
-            sortMock = sinon.stub(storageModule, 'getSort').returns(null)
+            sortMock = sinon.stub(storageModule, 'getSort').returns('result')
             sortDirectionMock = sinon.stub(storageModule, 'getSortDirection').returns(null)
             managerSpy = sinon.spy(dataModule.manager, 'setRender')
 
             doInitSort()
             expect(managerSpy.callCount).to.eql(1)
             expect(dataModule.manager.testSubset.map(({
                 result
@@ -165,90 +221,24 @@
             managerSpy = sinon.spy(dataModule.manager, 'setRender')
 
             doSort('result')
             expect(managerSpy.callCount).to.eql(1)
             expect(dataModule.manager.testSubset.map(({
                 result
             }) => result)).to.eql([
-                'passed', 'passed', 'passed', 'passed', 'passed', 'failed',
+                'failed', 'passed', 'passed', 'passed', 'passed', 'passed',
             ])
         })
     })
 })
 
-describe('utils tests', () => {
-    describe('formatDuration', () => {
-        it('handles small durations', () => {
-            expect(formatDuration(0.123).ms).to.eql('123 ms')
-            expect(formatDuration(0).ms).to.eql('0 ms')
-            expect(formatDuration(0.999).ms).to.eql('999 ms')
-        })
-        it('handles larger durations', () => {
-            expect(formatDuration(1.234).formatted).to.eql('00:00:01')
-            expect(formatDuration(12345.678).formatted).to.eql('03:25:46')
-        })
-    })
-    describe('transformTableObj', () => {
-        it('handles empty object', () => {
-            expect(transformTableObj({})).to.eql({
-                appends: {},
-                inserts: {}
-            })
-        })
-        it('handles no appends', () => {
-            const expected = {
-                1: "hello",
-                2: "goodbye"
-            }
-            expect(transformTableObj(expected)).to.eql({
-                appends: {},
-                inserts: expected
-            })
-        })
-        it('handles no inserts', () => {
-            const expected = {
-                "Z1": "hello",
-                "Z2": "goodbye"
-            }
-            expect(transformTableObj(expected)).to.eql({
-                appends: expected,
-                inserts: {}
-            })
-        })
-        it('handles both', () => {
-            const expected = {
-                appends: {
-                    "Z1": "hello",
-                    "Z2": "goodbye"
-                },
-                inserts: {
-                    1: "mee",
-                    2: "moo"
-                }
-            }
-            expect(transformTableObj({
-                ...expected.appends,
-                ...expected.inserts
-            })).to.eql(expected)
-        })
-    })
-})
-
 describe('Storage tests', () => {
     describe('getCollapsedCategory', () => {
         let originalWindow
-        const mockWindow = (queryParam) => {
-            const mock = {
-                location: {
-                    href: `https://example.com/page?${queryParam}`
-                }
-            }
-            originalWindow = global.window
-            global.window = mock
-        }
+
         after(() => global.window = originalWindow)
 
         it('collapses passed by default', () => {
             mockWindow()
             const collapsedItems = storageModule.getCollapsedCategory()
             expect(collapsedItems).to.eql(['passed'])
         })
@@ -273,60 +263,60 @@
 
         const config = [{
             value: ['failed', 'error'],
             expected: ['failed', 'error']
         }, {
             value: ['all'],
             expected: storageModule.possibleFilters
-        }]
+        }, ]
         config.forEach(({
             value,
             expected
         }) => {
             it(`handles python config: ${value}`, () => {
                 mockWindow()
                 const collapsedItems = storageModule.getCollapsedCategory(value)
                 expect(collapsedItems).to.eql(expected)
             })
         })
 
         const precedence = [{
             query: 'collapsed=xpassed,xfailed',
-            config: ['failed', 'error'],
+            value: ['failed', 'error'],
             expected: ['xpassed', 'xfailed']
         }, {
             query: 'collapsed=all',
-            config: ['failed', 'error'],
+            value: ['failed', 'error'],
             expected: storageModule.possibleFilters
         }, {
             query: 'collapsed=xpassed,xfailed',
-            config: ['all'],
+            value: ['all'],
             expected: ['xpassed', 'xfailed']
         }, ]
         precedence.forEach(({
             query,
-            config,
+            value,
             expected
         }, index) => {
             it(`handles python config precedence ${index + 1}`, () => {
                 mockWindow(query)
-                const collapsedItems = storageModule.getCollapsedCategory(config)
+                const collapsedItems = storageModule.getCollapsedCategory(value)
                 expect(collapsedItems).to.eql(expected)
             })
         })
 
         const falsy = [{
             param: 'collapsed'
         }, {
             param: 'collapsed='
         }, {
             param: 'collapsed=""'
         }, {
             param: 'collapsed=\'\''
-        }]
+        }, ]
         falsy.forEach(({
             param
         }) => {
             it(`collapses none with ${param}`, () => {
                 mockWindow(param)
                 const collapsedItems = storageModule.getCollapsedCategory()
                 expect(collapsedItems).to.be.empty
```

### Comparing `pytest_html-4.0.0rc4/.gitignore` & `pytest_html-4.0.0rc5/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc4/README.rst` & `pytest_html-4.0.0rc5/README.rst`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc4/pyproject.toml` & `pytest_html-4.0.0rc5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -38,22 +38,25 @@
   "Programming Language :: Python :: Implementation :: PyPy",
   "Topic :: Software Development :: Quality Assurance",
   "Topic :: Software Development :: Testing",
   "Topic :: Utilities",
 ]
 dependencies = [
   "pytest>=7.0.0",
-  "pytest-metadata>=2.0.2",
+  "pytest-metadata>=3.0.0",
   "Jinja2>=3.0.0",
 ]
 dynamic = [
   "version",
 ]
 
 [project.optional-dependencies]
+docs = [
+  "pip-tools>=6.13.0",
+]
 test = [
   "assertpy>=1.1",
   "beautifulsoup4>=4.11.1",
   "black>=22.1.0",
   "flake8>=4.0.1",
   "pre-commit>=2.17.0",
   "pytest-xdist>=2.4.0",
@@ -66,14 +69,15 @@
 [project.urls]
 Homepage = "https://github.com/pytest-dev/pytest-html"
 Tracker = "https://github.com/pytest-dev/pytest-html/issues"
 Source = "https://github.com/pytest-dev/pytest-html"
 
 [project.entry-points.pytest11]
 html = "pytest_html.plugin"
+html_fixtures = "pytest_html.fixtures"
 
 [tool.hatch.envs.test]
 features = [
   "test",
 ]
 
 [tool.hatch.version]
@@ -87,7 +91,10 @@
 [tool.hatch.build.targets.sdist]
 exclude = [
   "/.github",
 ]
 
 [tool.hatch.build.hooks.vcs]
 version-file = "src/pytest_html/__version.py"
+
+[tool.hatch.build.hooks.custom]
+path = "scripts/npm.py"
```

### Comparing `pytest_html-4.0.0rc4/PKG-INFO` & `pytest_html-4.0.0rc5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-html
-Version: 4.0.0rc4
+Version: 4.0.0rc5
 Summary: pytest plugin for generating HTML reports
 Project-URL: Homepage, https://github.com/pytest-dev/pytest-html
 Project-URL: Tracker, https://github.com/pytest-dev/pytest-html/issues
 Project-URL: Source, https://github.com/pytest-dev/pytest-html
 Author-email: Dave Hunt <dhunt@mozilla.com>, Jim Brannlund <jimbrannlund@fastmail.com>
 License-Expression: MPL-2.0
 License-File: LICENSE
@@ -25,16 +25,18 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Requires-Dist: jinja2>=3.0.0
-Requires-Dist: pytest-metadata>=2.0.2
+Requires-Dist: pytest-metadata>=3.0.0
 Requires-Dist: pytest>=7.0.0
+Provides-Extra: docs
+Requires-Dist: pip-tools>=6.13.0; extra == 'docs'
 Provides-Extra: test
 Requires-Dist: assertpy>=1.1; extra == 'test'
 Requires-Dist: beautifulsoup4>=4.11.1; extra == 'test'
 Requires-Dist: black>=22.1.0; extra == 'test'
 Requires-Dist: flake8>=4.0.1; extra == 'test'
 Requires-Dist: pre-commit>=2.17.0; extra == 'test'
 Requires-Dist: pytest-mock>=3.7.0; extra == 'test'
```

