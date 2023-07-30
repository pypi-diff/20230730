# Comparing `tmp/munin-plot-1.6.tar.gz` & `tmp/munin-plot-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "munin-plot-1.6.tar", last modified: Sat Apr 29 15:32:36 2023, max compression
+gzip compressed data, was "munin-plot-1.7.tar", last modified: Sun Jul 30 11:06:36 2023, max compression
```

## Comparing `munin-plot-1.6.tar` & `munin-plot-1.7.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 15:32:36.000000 munin-plot-1.6/
--rw-r--r--   0 root         (0) root         (0)      419 2021-09-03 22:40:04.000000 munin-plot-1.6/.eslintrc.yml
--rw-r--r--   0 root         (0) root         (0)     1023 2019-12-30 21:16:14.000000 munin-plot-1.6/COPYING
--rw-r--r--   0 root         (0) root         (0)      259 2023-01-03 16:24:49.000000 munin-plot-1.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1634 2023-04-29 15:23:56.000000 munin-plot-1.6/NEWS
--rw-r--r--   0 root         (0) root         (0)     4058 2023-04-29 15:32:36.000000 munin-plot-1.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3156 2023-04-29 15:26:05.000000 munin-plot-1.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 15:32:36.000000 munin-plot-1.6/munin_plot.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4058 2023-04-29 15:32:36.000000 munin-plot-1.6/munin_plot.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      542 2023-04-29 15:32:36.000000 munin-plot-1.6/munin_plot.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-29 15:32:36.000000 munin-plot-1.6/munin_plot.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-04-29 15:32:36.000000 munin-plot-1.6/munin_plot.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 15:32:36.000000 munin-plot-1.6/muninplot/
--rw-r--r--   0 root         (0) root         (0)     1137 2020-06-21 13:02:19.000000 munin-plot-1.6/muninplot/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1716 2023-04-29 14:59:09.000000 munin-plot-1.6/muninplot/__main__.py
--rw-r--r--   0 root         (0) root         (0)     7013 2021-07-09 12:28:19.000000 munin-plot-1.6/muninplot/data.py
--rw-r--r--   0 root         (0) root         (0)     6221 2023-01-03 16:24:49.000000 munin-plot-1.6/muninplot/wsgi.py
--rw-r--r--   0 root         (0) root         (0)   356986 2023-04-29 15:31:56.000000 munin-plot-1.6/package-lock.json
--rw-r--r--   0 root         (0) root         (0)     1351 2023-04-29 14:59:09.000000 munin-plot-1.6/package.json
--rw-r--r--   0 root         (0) root         (0)     1410 2023-04-29 15:32:36.000000 munin-plot-1.6/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     2352 2021-01-31 17:46:59.000000 munin-plot-1.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 15:32:36.000000 munin-plot-1.6/src/
--rw-r--r--   0 root         (0) root         (0)     5719 2019-12-30 21:53:09.000000 munin-plot-1.6/src/apple-touch-icon.png
--rw-r--r--   0 root         (0) root         (0)      355 2019-12-30 21:53:10.000000 munin-plot-1.6/src/favicon-16x16.png
--rw-r--r--   0 root         (0) root         (0)      680 2019-12-30 21:53:10.000000 munin-plot-1.6/src/favicon-32x32.png
--rw-r--r--   0 root         (0) root         (0)     1471 2019-12-30 21:53:10.000000 munin-plot-1.6/src/favicon-64x64.png
--rw-r--r--   0 root         (0) root         (0)    12838 2019-12-30 21:53:10.000000 munin-plot-1.6/src/favicon.ico
--rw-r--r--   0 root         (0) root         (0)     9451 2023-01-03 16:24:49.000000 munin-plot-1.6/src/index.html
--rw-r--r--   0 root         (0) root         (0)     5513 2019-12-30 21:16:14.000000 munin-plot-1.6/src/logo.png
--rw-r--r--   0 root         (0) root         (0)     6767 2023-01-03 16:24:49.000000 munin-plot-1.6/src/munin-plot.css
--rw-r--r--   0 root         (0) root         (0)    32163 2023-01-03 16:24:49.000000 munin-plot-1.6/src/munin-plot.js
--rw-r--r--   0 root         (0) root         (0)      648 2023-01-03 16:24:49.000000 munin-plot-1.6/tox.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 15:32:36.000000 munin-plot-1.6/webpack-plugins/
--rw-r--r--   0 root         (0) root         (0)     1758 2023-01-03 16:24:49.000000 munin-plot-1.6/webpack-plugins/zip-plugin.js
--rw-r--r--   0 root         (0) root         (0)     2302 2023-01-03 16:24:49.000000 munin-plot-1.6/webpack.config.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 11:06:36.359421 munin-plot-1.7/
+-rw-r--r--   0 root         (0) root         (0)      419 2023-01-03 15:08:35.000000 munin-plot-1.7/.eslintrc.yml
+-rw-r--r--   0 root         (0) root         (0)     1023 2019-12-30 20:50:33.000000 munin-plot-1.7/COPYING
+-rw-r--r--   0 root         (0) root         (0)      259 2022-03-27 19:33:32.000000 munin-plot-1.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2150 2023-07-30 10:52:20.000000 munin-plot-1.7/NEWS
+-rw-r--r--   0 root         (0) root         (0)     4058 2023-07-30 11:06:36.359421 munin-plot-1.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3156 2023-04-29 15:40:24.000000 munin-plot-1.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 11:06:36.359421 munin-plot-1.7/munin_plot.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4058 2023-07-30 11:06:36.000000 munin-plot-1.7/munin_plot.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      542 2023-07-30 11:06:36.000000 munin-plot-1.7/munin_plot.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-30 11:06:36.000000 munin-plot-1.7/munin_plot.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-07-30 11:06:36.000000 munin-plot-1.7/munin_plot.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 11:06:36.359421 munin-plot-1.7/muninplot/
+-rw-r--r--   0 root         (0) root         (0)     1137 2020-01-05 15:43:28.000000 munin-plot-1.7/muninplot/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1716 2023-01-03 17:30:17.000000 munin-plot-1.7/muninplot/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     7013 2021-07-09 13:38:14.000000 munin-plot-1.7/muninplot/data.py
+-rw-r--r--   0 root         (0) root         (0)     6221 2022-02-11 18:26:57.000000 munin-plot-1.7/muninplot/wsgi.py
+-rw-r--r--   0 root         (0) root         (0)   347270 2023-07-30 11:06:13.000000 munin-plot-1.7/package-lock.json
+-rw-r--r--   0 root         (0) root         (0)     1351 2023-07-29 15:57:35.000000 munin-plot-1.7/package.json
+-rw-r--r--   0 root         (0) root         (0)     1411 2023-07-30 11:06:36.359421 munin-plot-1.7/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     2352 2021-01-31 17:30:36.000000 munin-plot-1.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 11:06:36.359421 munin-plot-1.7/src/
+-rw-r--r--   0 root         (0) root         (0)     5719 2019-12-30 21:50:34.000000 munin-plot-1.7/src/apple-touch-icon.png
+-rw-r--r--   0 root         (0) root         (0)      355 2019-12-30 21:50:34.000000 munin-plot-1.7/src/favicon-16x16.png
+-rw-r--r--   0 root         (0) root         (0)      680 2019-12-30 21:50:34.000000 munin-plot-1.7/src/favicon-32x32.png
+-rw-r--r--   0 root         (0) root         (0)     1471 2019-12-30 21:50:34.000000 munin-plot-1.7/src/favicon-64x64.png
+-rw-r--r--   0 root         (0) root         (0)    12838 2019-12-30 21:50:34.000000 munin-plot-1.7/src/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)     9959 2023-07-29 15:28:53.000000 munin-plot-1.7/src/index.html
+-rw-r--r--   0 root         (0) root         (0)     5513 2019-12-30 21:10:41.000000 munin-plot-1.7/src/logo.png
+-rw-r--r--   0 root         (0) root         (0)     6767 2021-12-12 17:20:31.000000 munin-plot-1.7/src/munin-plot.css
+-rw-r--r--   0 root         (0) root         (0)    34888 2023-07-30 10:45:56.000000 munin-plot-1.7/src/munin-plot.js
+-rw-r--r--   0 root         (0) root         (0)      648 2023-07-30 00:23:56.000000 munin-plot-1.7/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 11:06:36.359421 munin-plot-1.7/webpack-plugins/
+-rw-r--r--   0 root         (0) root         (0)     1758 2021-12-30 13:51:52.000000 munin-plot-1.7/webpack-plugins/zip-plugin.js
+-rw-r--r--   0 root         (0) root         (0)     2302 2022-01-03 18:14:11.000000 munin-plot-1.7/webpack.config.js
```

### Comparing `munin-plot-1.6/COPYING` & `munin-plot-1.7/COPYING`

 * *Files identical despite different names*

### Comparing `munin-plot-1.6/NEWS` & `munin-plot-1.7/NEWS`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+changes from 1.6 to 1.7
+-----------------------
+
+* Fix the order of items in the legend to match the Munin plugin order
+* Allow better selections of items to show in the graph via buttons (select
+  all, select none and toggle selection) as well as focusing on a single item
+  through double click
+* Various NPM package updates (includes fixes for a number of CVEs, none of
+  which should affect munin-plot because we don't supply untrusted content to
+  the affected components or don't use affected functionality)
+
+
 changes from 1.5 to 1.6
 -----------------------
 
 * Various NPM package updates (includes fixes for a number of CVEs, none of
   which should affect munin-plot because we don't supply untrusted content to
   the affected components or don't use affected functionality)
 * Show a more helpful error if static files need to be built
```

### Comparing `munin-plot-1.6/PKG-INFO` & `munin-plot-1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: munin-plot
-Version: 1.6
+Version: 1.7
 Summary: Alternative web front-end for Munin
 Home-page: https://arthurdejong.org/munin-plot/
 Author: Arthur de Jong
 Author-email: arthur@arthurdejong.org
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
```

### Comparing `munin-plot-1.6/README.md` & `munin-plot-1.7/README.md`

 * *Files identical despite different names*

### Comparing `munin-plot-1.6/munin_plot.egg-info/PKG-INFO` & `munin-plot-1.7/munin_plot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: munin-plot
-Version: 1.6
+Version: 1.7
 Summary: Alternative web front-end for Munin
 Home-page: https://arthurdejong.org/munin-plot/
 Author: Arthur de Jong
 Author-email: arthur@arthurdejong.org
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
```

### Comparing `munin-plot-1.6/munin_plot.egg-info/SOURCES.txt` & `munin-plot-1.7/munin_plot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `munin-plot-1.6/muninplot/__init__.py` & `munin-plot-1.7/muninplot/__init__.py`

 * *Files identical despite different names*

### Comparing `munin-plot-1.6/muninplot/__main__.py` & `munin-plot-1.7/muninplot/__main__.py`

 * *Files identical despite different names*

### Comparing `munin-plot-1.6/muninplot/data.py` & `munin-plot-1.7/muninplot/data.py`

 * *Files identical despite different names*

### Comparing `munin-plot-1.6/muninplot/wsgi.py` & `munin-plot-1.7/muninplot/wsgi.py`

 * *Files identical despite different names*

### Comparing `munin-plot-1.6/package-lock.json` & `munin-plot-1.7/package-lock.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9924381791401127%*

 * *Differences: {"'packages'": "{'': {'dependencies': {'bootstrap': '^5.3.1', 'd3': '^7.8.5', 'jquery': '^3.7.0', "*

 * *               "'plotly.js': '^2.25.0'}, 'devDependencies': {'css-loader': '^6.8.1', 'eslint': "*

 * *               "'^8.46.0', 'eslint-config-standard': '^17.1.0', 'eslint-plugin-import': '^2.28.0', "*

 * *               "'html-webpack-plugin': '^5.5.3', 'mini-css-extract-plugin': '^2.7.6', "*

 * *               "'postcss-loader': '^7.3.3', 'sass-loader': '^13.3.2', 'style-loader': '^3.3.3', "*

 * *               "'webpack': ' […]*

```diff
@@ -1,80 +1,89 @@
 {
     "lockfileVersion": 3,
     "name": "@arthurdejong/munin-plot",
     "packages": {
         "": {
             "dependencies": {
                 "@fortawesome/fontawesome-free": "^6.4.0",
-                "bootstrap": "^5.2.3",
-                "d3": "^7.8.4",
+                "bootstrap": "^5.3.1",
+                "d3": "^7.8.5",
                 "daterangepicker": "^3.1.0",
-                "jquery": "^3.6.4",
+                "jquery": "^3.7.0",
                 "jquery-ui": "^1.13.2",
                 "pako": "^2.1.0",
-                "plotly.js": "^2.22.0"
+                "plotly.js": "^2.25.0"
             },
             "devDependencies": {
                 "archiver": "^5.3.1",
                 "autoprefixer": "^10.4.14",
-                "css-loader": "^6.7.3",
-                "eslint": "^8.39.0",
-                "eslint-config-standard": "^17.0.0",
-                "eslint-plugin-import": "^2.27.5",
+                "css-loader": "^6.8.1",
+                "eslint": "^8.46.0",
+                "eslint-config-standard": "^17.1.0",
+                "eslint-plugin-import": "^2.28.0",
                 "eslint-plugin-node": "^11.1.0",
                 "eslint-plugin-promise": "^6.1.1",
                 "file-loader": "^6.2.0",
                 "html-loader": "^4.2.0",
-                "html-webpack-plugin": "^5.5.1",
-                "mini-css-extract-plugin": "^2.7.5",
+                "html-webpack-plugin": "^5.5.3",
+                "mini-css-extract-plugin": "^2.7.6",
                 "node-sass": "^8.0.0",
-                "postcss-loader": "^7.3.0",
-                "sass-loader": "^13.2.2",
-                "style-loader": "^3.3.2",
-                "webpack": "^5.81.0",
-                "webpack-cli": "^5.0.2"
+                "postcss-loader": "^7.3.3",
+                "sass-loader": "^13.3.2",
+                "style-loader": "^3.3.3",
+                "webpack": "^5.88.2",
+                "webpack-cli": "^5.1.4"
             },
             "license": "MIT",
             "name": "@arthurdejong/munin-plot",
             "version": "0.0.0"
         },
+        "node_modules/@aashutoshrathi/word-wrap": {
+            "dev": true,
+            "engines": {
+                "node": ">=0.10.0"
+            },
+            "integrity": "sha512-1Yjs2SvM8TflER/OD3cOjhWWOZb58A2t7wpE2S9XfBYTiIl+XFhQG2bjy4Pu1I+EAlCNUzRDYDdFwFYUKvXcIA==",
+            "resolved": "https://registry.npmjs.org/@aashutoshrathi/word-wrap/-/word-wrap-1.2.6.tgz",
+            "version": "1.2.6"
+        },
         "node_modules/@babel/code-frame": {
             "dependencies": {
-                "@babel/highlight": "^7.18.6"
+                "@babel/highlight": "^7.22.5"
             },
             "dev": true,
             "engines": {
                 "node": ">=6.9.0"
             },
-            "integrity": "sha512-LYvhNKfwWSPpocw8GI7gpK2nq3HSDuEPC/uSYaALSJu9xjsalaaYFOq0Pwt5KmVqwEbZlDu81aLXwBOmD/Fv9g==",
-            "resolved": "https://registry.npmjs.org/@babel/code-frame/-/code-frame-7.21.4.tgz",
-            "version": "7.21.4"
+            "integrity": "sha512-Xmwn266vad+6DAqEB2A6V/CcZVp62BbwVmcOJc2RPuwih1kw02TjQvWVWlcKGbBPd+8/0V5DEkOcizRGYsspYQ==",
+            "resolved": "https://registry.npmjs.org/@babel/code-frame/-/code-frame-7.22.5.tgz",
+            "version": "7.22.5"
         },
         "node_modules/@babel/helper-validator-identifier": {
             "dev": true,
             "engines": {
                 "node": ">=6.9.0"
             },
-            "integrity": "sha512-awrNfaMtnHUr653GgGEs++LlAvW6w+DcPrOliSMXWCKo597CwL5Acf/wWdNkf/tfEQE3mjkeD1YOVZOUV/od1w==",
-            "resolved": "https://registry.npmjs.org/@babel/helper-validator-identifier/-/helper-validator-identifier-7.19.1.tgz",
-            "version": "7.19.1"
+            "integrity": "sha512-aJXu+6lErq8ltp+JhkJUfk1MTGyuA4v7f3pA+BJ5HLfNC6nAQ0Cpi9uOquUj8Hehg0aUiHzWQbOVJGao6ztBAQ==",
+            "resolved": "https://registry.npmjs.org/@babel/helper-validator-identifier/-/helper-validator-identifier-7.22.5.tgz",
+            "version": "7.22.5"
         },
         "node_modules/@babel/highlight": {
             "dependencies": {
-                "@babel/helper-validator-identifier": "^7.18.6",
+                "@babel/helper-validator-identifier": "^7.22.5",
                 "chalk": "^2.0.0",
                 "js-tokens": "^4.0.0"
             },
             "dev": true,
             "engines": {
                 "node": ">=6.9.0"
             },
-            "integrity": "sha512-u7stbOuYjaPezCuLj29hNW1v64M2Md2qupEKP1fHc7WdOA3DgLh37suiSrZYY7haUB7iBeQZ9P1uiRF359do3g==",
-            "resolved": "https://registry.npmjs.org/@babel/highlight/-/highlight-7.18.6.tgz",
-            "version": "7.18.6"
+            "integrity": "sha512-BSKlD1hgnedS5XRnGOljZawtag7H1yPfQp0tdNJCHoH6AZ+Pcm9VvkrK59/Yy593Ypg0zMxH2BxD1VPYUQ7UIw==",
+            "resolved": "https://registry.npmjs.org/@babel/highlight/-/highlight-7.22.5.tgz",
+            "version": "7.22.5"
         },
         "node_modules/@babel/highlight/node_modules/ansi-styles": {
             "dependencies": {
                 "color-convert": "^1.9.0"
             },
             "dev": true,
             "engines": {
@@ -184,49 +193,49 @@
             "version": "4.4.0"
         },
         "node_modules/@eslint-community/regexpp": {
             "dev": true,
             "engines": {
                 "node": "^12.0.0 || ^14.0.0 || >=16.0.0"
             },
-            "integrity": "sha512-vITaYzIcNmjn5tF5uxcZ/ft7/RXGrMUIS9HalWckEOF6ESiwXKoMzAQf2UW0aVd6rnOeExTJVd5hmWXucBKGXQ==",
-            "resolved": "https://registry.npmjs.org/@eslint-community/regexpp/-/regexpp-4.5.0.tgz",
-            "version": "4.5.0"
+            "integrity": "sha512-pPTNuaAG3QMH+buKyBIGJs3g/S5y0caxw0ygM3YyE6yJFySwiGGSzA+mM3KJ8QQvzeLh3blwgSonkFjgQdxzMw==",
+            "resolved": "https://registry.npmjs.org/@eslint-community/regexpp/-/regexpp-4.6.2.tgz",
+            "version": "4.6.2"
         },
         "node_modules/@eslint/eslintrc": {
             "dependencies": {
                 "ajv": "^6.12.4",
                 "debug": "^4.3.2",
-                "espree": "^9.5.1",
+                "espree": "^9.6.0",
                 "globals": "^13.19.0",
                 "ignore": "^5.2.0",
                 "import-fresh": "^3.2.1",
                 "js-yaml": "^4.1.0",
                 "minimatch": "^3.1.2",
                 "strip-json-comments": "^3.1.1"
             },
             "dev": true,
             "engines": {
                 "node": "^12.22.0 || ^14.17.0 || >=16.0.0"
             },
             "funding": {
                 "url": "https://opencollective.com/eslint"
             },
-            "integrity": "sha512-3W4f5tDUra+pA+FzgugqL2pRimUTDJWKr7BINqOpkZrC0uYI0NIc0/JFgBROCU07HR6GieA5m3/rsPIhDmCXTQ==",
-            "resolved": "https://registry.npmjs.org/@eslint/eslintrc/-/eslintrc-2.0.2.tgz",
-            "version": "2.0.2"
+            "integrity": "sha512-9t7ZA7NGGK8ckelF0PQCfcxIUzs1Md5rrO6U/c+FIQNanea5UZC0wqKXH4vHBccmu4ZJgZ2idtPeW7+Q2npOEA==",
+            "resolved": "https://registry.npmjs.org/@eslint/eslintrc/-/eslintrc-2.1.1.tgz",
+            "version": "2.1.1"
         },
         "node_modules/@eslint/js": {
             "dev": true,
             "engines": {
                 "node": "^12.22.0 || ^14.17.0 || >=16.0.0"
             },
-            "integrity": "sha512-kf9RB0Fg7NZfap83B3QOqOGg9QmD9yBudqQXzzOtn3i4y7ZUXe5ONeW34Gwi+TxhH4mvj72R1Zc300KUMa9Bng==",
-            "resolved": "https://registry.npmjs.org/@eslint/js/-/js-8.39.0.tgz",
-            "version": "8.39.0"
+            "integrity": "sha512-a8TLtmPi8xzPkCbp/OGFUo5yhRkHM2Ko9kOWP4znJr0WAhWyThaw3PnwX4vOTWOAMsV2uRt32PPDcEz63esSaA==",
+            "resolved": "https://registry.npmjs.org/@eslint/js/-/js-8.46.0.tgz",
+            "version": "8.46.0"
         },
         "node_modules/@fortawesome/fontawesome-free": {
             "engines": {
                 "node": ">=6"
             },
             "hasInstallScript": true,
             "integrity": "sha512-0NyytTlPJwB/BF5LtRV8rrABDbe3TdTXqNB3PdZ+UUUZAEIrdOJdmABqKjt4AXwIoJNaRVVZEXxpNrqvE1GAYQ==",
@@ -245,17 +254,17 @@
                 "debug": "^4.1.1",
                 "minimatch": "^3.0.5"
             },
             "dev": true,
             "engines": {
                 "node": ">=10.10.0"
             },
-            "integrity": "sha512-UybHIJzJnR5Qc/MsD9Kr+RpO2h+/P1GhOwdiLPXK5TWk5sgTdu88bTD9UP+CKbPPh5Rni1u0GjAdYQLemG8g+g==",
-            "resolved": "https://registry.npmjs.org/@humanwhocodes/config-array/-/config-array-0.11.8.tgz",
-            "version": "0.11.8"
+            "integrity": "sha512-KVVjQmNUepDVGXNuoRRdmmEjruj0KfiGSbS8LVc12LMsWDQzRXJ0qdhN8L8uUigKpfEHRhlaQFY0ib1tnUbNeQ==",
+            "resolved": "https://registry.npmjs.org/@humanwhocodes/config-array/-/config-array-0.11.10.tgz",
+            "version": "0.11.10"
         },
         "node_modules/@humanwhocodes/module-importer": {
             "dev": true,
             "engines": {
                 "node": ">=12.22"
             },
             "funding": {
@@ -306,17 +315,17 @@
         },
         "node_modules/@jridgewell/source-map": {
             "dependencies": {
                 "@jridgewell/gen-mapping": "^0.3.0",
                 "@jridgewell/trace-mapping": "^0.3.9"
             },
             "dev": true,
-            "integrity": "sha512-b+fsZXeLYi9fEULmfBrhxn4IrPlINf8fiNarzTof004v3lFdntdwa9PF7vFJqm3mg7s+ScJMxXaE3Acp1irZcg==",
-            "resolved": "https://registry.npmjs.org/@jridgewell/source-map/-/source-map-0.3.3.tgz",
-            "version": "0.3.3"
+            "integrity": "sha512-UTYAUj/wviwdsMfzoSJspJxbkH5o1snzwX0//0ENX1u/55kkZZkcTZP6u9bwKGkv+dkk9at4m1Cpt0uY80kcpQ==",
+            "resolved": "https://registry.npmjs.org/@jridgewell/source-map/-/source-map-0.3.5.tgz",
+            "version": "0.3.5"
         },
         "node_modules/@jridgewell/sourcemap-codec": {
             "dev": true,
             "integrity": "sha512-eF2rxCRulEKXHTRiDrDy6erMYWqNw4LPdQ8UQA4huuxaQsVeRPFl2oM8oDGxMFhJUWZf9McpLtJasDDZb/Bpeg==",
             "resolved": "https://registry.npmjs.org/@jridgewell/sourcemap-codec/-/sourcemap-codec-1.4.15.tgz",
             "version": "1.4.15"
         },
@@ -542,18 +551,18 @@
             "version": "3.1.9"
         },
         "node_modules/@popperjs/core": {
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/popperjs"
             },
-            "integrity": "sha512-Cr4OjIkipTtcXKjAsm8agyleBuDHvxzeBoa1v543lbv1YaIwQjESsVcmjiWiPEbC1FIeHOG/Op9kdCmAmiS3Kw==",
+            "integrity": "sha512-P1st0aksCrn9sGZhp8GMYwBnQsbvAWsZAX44oXNNvLHGqAOcoVxmjZiohstwQ7SqKnbR47akdNi+uleWD8+g6A==",
             "peer": true,
-            "resolved": "https://registry.npmjs.org/@popperjs/core/-/core-2.11.7.tgz",
-            "version": "2.11.7"
+            "resolved": "https://registry.npmjs.org/@popperjs/core/-/core-2.11.8.tgz",
+            "version": "2.11.8"
         },
         "node_modules/@tootallnate/once": {
             "dev": true,
             "engines": {
                 "node": ">= 10"
             },
             "integrity": "sha512-XCuKFP5PS55gnMVu3dty8KPatLqUoy/ZYzDzAGCQ8JNFCkLXzmI7vNHCR+XpbZaMWQK/vQubr7PkYq8g470J/A==",
@@ -617,17 +626,17 @@
         },
         "node_modules/@types/eslint": {
             "dependencies": {
                 "@types/estree": "*",
                 "@types/json-schema": "*"
             },
             "dev": true,
-            "integrity": "sha512-Piet7dG2JBuDIfohBngQ3rCt7MgO9xCO4xIMKxBThCq5PNRB91IjlJ10eJVwfoNtvTErmxLzwBZ7rHZtbOMmFQ==",
-            "resolved": "https://registry.npmjs.org/@types/eslint/-/eslint-8.37.0.tgz",
-            "version": "8.37.0"
+            "integrity": "sha512-XpNDc4Z5Tb4x+SW1MriMVeIsMoONHCkWFMkR/aPJbzEsxqHy+4Glu/BqTdPrApfDeMaXbtNh6bseNgl5KaWrSg==",
+            "resolved": "https://registry.npmjs.org/@types/eslint/-/eslint-8.44.1.tgz",
+            "version": "8.44.1"
         },
         "node_modules/@types/eslint-scope": {
             "dependencies": {
                 "@types/eslint": "*",
                 "@types/estree": "*"
             },
             "dev": true,
@@ -645,17 +654,17 @@
             "dev": true,
             "integrity": "sha512-oh/6byDPnL1zeNXFrDXFLyZjkr1MsBG667IM792caf1L2UPOOMf65NFzjUH/ltyfwjAGfs1rsX1eftK0jC/KIg==",
             "resolved": "https://registry.npmjs.org/@types/html-minifier-terser/-/html-minifier-terser-6.1.0.tgz",
             "version": "6.1.0"
         },
         "node_modules/@types/json-schema": {
             "dev": true,
-            "integrity": "sha512-wOuvG1SN4Us4rez+tylwwwCV1psiNVOkJeM3AUWUNWg/jDQY2+HE/444y5gc+jBmRqASOm2Oeh5c1axHobwRKQ==",
-            "resolved": "https://registry.npmjs.org/@types/json-schema/-/json-schema-7.0.11.tgz",
-            "version": "7.0.11"
+            "integrity": "sha512-Hr5Jfhc9eYOQNPYO5WLDq/n4jqijdHNlDXjuAQkkt+mWdQR+XJToOHrsD4cPaMXpn6KO7y2+wM8AZEs8VpBLVA==",
+            "resolved": "https://registry.npmjs.org/@types/json-schema/-/json-schema-7.0.12.tgz",
+            "version": "7.0.12"
         },
         "node_modules/@types/json5": {
             "dev": true,
             "integrity": "sha512-dRLjCWHYg4oaA77cxO64oO+7JwCwnIzkZPdrrC71jQmQtlhM556pwKo5bUzqvZndkVbeFLIIi+9TC40JNF5hNQ==",
             "resolved": "https://registry.npmjs.org/@types/json5/-/json5-0.0.29.tgz",
             "version": "0.0.29"
         },
@@ -663,213 +672,213 @@
             "dev": true,
             "integrity": "sha512-jhuKLIRrhvCPLqwPcx6INqmKeiA5EWrsCOPhrlFSrbrmU4ZMPjj5Ul/oLCMDO98XRUIwVm78xICz4EPCektzeQ==",
             "resolved": "https://registry.npmjs.org/@types/minimist/-/minimist-1.2.2.tgz",
             "version": "1.2.2"
         },
         "node_modules/@types/node": {
             "dev": true,
-            "integrity": "sha512-OPs5WnnT1xkCBiuQrZA4+YAV4HEJejmHneyraIaxsbev5yCEr6KMwINNFP9wQeFIw8FWcoTqF3vQsa5CDaI+8Q==",
-            "resolved": "https://registry.npmjs.org/@types/node/-/node-18.16.3.tgz",
-            "version": "18.16.3"
+            "integrity": "sha512-rt40Nk13II9JwQBdeYqmbn2Q6IVTA5uPhvSO+JVqdXw/6/4glI6oR9ezty/A9Hg5u7JH4OmYmuQ+XvjKm0Datg==",
+            "resolved": "https://registry.npmjs.org/@types/node/-/node-20.4.5.tgz",
+            "version": "20.4.5"
         },
         "node_modules/@types/normalize-package-data": {
             "dev": true,
             "integrity": "sha512-Gj7cI7z+98M282Tqmp2K5EIsoouUEzbBJhQQzDE3jSIRk6r9gsz0oUokqIUR4u1R3dMHo0pDHM7sNOHyhulypw==",
             "resolved": "https://registry.npmjs.org/@types/normalize-package-data/-/normalize-package-data-2.4.1.tgz",
             "version": "2.4.1"
         },
         "node_modules/@webassemblyjs/ast": {
             "dependencies": {
-                "@webassemblyjs/helper-numbers": "1.11.5",
-                "@webassemblyjs/helper-wasm-bytecode": "1.11.5"
+                "@webassemblyjs/helper-numbers": "1.11.6",
+                "@webassemblyjs/helper-wasm-bytecode": "1.11.6"
             },
             "dev": true,
-            "integrity": "sha512-LHY/GSAZZRpsNQH+/oHqhRQ5FT7eoULcBqgfyTB5nQHogFnK3/7QoN7dLnwSE/JkUAF0SrRuclT7ODqMFtWxxQ==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/ast/-/ast-1.11.5.tgz",
-            "version": "1.11.5"
+            "integrity": "sha512-IN1xI7PwOvLPgjcf180gC1bqn3q/QaOCwYUahIOhbYUu8KA/3tw2RT/T0Gidi1l7Hhj5D/INhJxiICObqpMu4Q==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/ast/-/ast-1.11.6.tgz",
+            "version": "1.11.6"
         },
         "node_modules/@webassemblyjs/floating-point-hex-parser": {
             "dev": true,
-            "integrity": "sha512-1j1zTIC5EZOtCplMBG/IEwLtUojtwFVwdyVMbL/hwWqbzlQoJsWCOavrdnLkemwNoC/EOwtUFch3fuo+cbcXYQ==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/floating-point-hex-parser/-/floating-point-hex-parser-1.11.5.tgz",
-            "version": "1.11.5"
+            "integrity": "sha512-ejAj9hfRJ2XMsNHk/v6Fu2dGS+i4UaXBXGemOfQ/JfQ6mdQg/WXtwleQRLLS4OvfDhv8rYnVwH27YJLMyYsxhw==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/floating-point-hex-parser/-/floating-point-hex-parser-1.11.6.tgz",
+            "version": "1.11.6"
         },
         "node_modules/@webassemblyjs/helper-api-error": {
             "dev": true,
-            "integrity": "sha512-L65bDPmfpY0+yFrsgz8b6LhXmbbs38OnwDCf6NpnMUYqa+ENfE5Dq9E42ny0qz/PdR0LJyq/T5YijPnU8AXEpA==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-api-error/-/helper-api-error-1.11.5.tgz",
-            "version": "1.11.5"
+            "integrity": "sha512-o0YkoP4pVu4rN8aTJgAyj9hC2Sv5UlkzCHhxqWj8butaLvnpdc2jOwh4ewE6CX0txSfLn/UYaV/pheS2Txg//Q==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-api-error/-/helper-api-error-1.11.6.tgz",
+            "version": "1.11.6"
         },
         "node_modules/@webassemblyjs/helper-buffer": {
             "dev": true,
-            "integrity": "sha512-fDKo1gstwFFSfacIeH5KfwzjykIE6ldh1iH9Y/8YkAZrhmu4TctqYjSh7t0K2VyDSXOZJ1MLhht/k9IvYGcIxg==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-buffer/-/helper-buffer-1.11.5.tgz",
-            "version": "1.11.5"
+            "integrity": "sha512-z3nFzdcp1mb8nEOFFk8DrYLpHvhKC3grJD2ardfKOzmbmJvEf/tPIqCY+sNcwZIY8ZD7IkB2l7/pqhUhqm7hLA==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-buffer/-/helper-buffer-1.11.6.tgz",
+            "version": "1.11.6"
         },
         "node_modules/@webassemblyjs/helper-numbers": {
             "dependencies": {
-                "@webassemblyjs/floating-point-hex-parser": "1.11.5",
-                "@webassemblyjs/helper-api-error": "1.11.5",
+                "@webassemblyjs/floating-point-hex-parser": "1.11.6",
+                "@webassemblyjs/helper-api-error": "1.11.6",
                 "@xtuc/long": "4.2.2"
             },
             "dev": true,
-            "integrity": "sha512-DhykHXM0ZABqfIGYNv93A5KKDw/+ywBFnuWybZZWcuzWHfbp21wUfRkbtz7dMGwGgT4iXjWuhRMA2Mzod6W4WA==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-numbers/-/helper-numbers-1.11.5.tgz",
-            "version": "1.11.5"
+            "integrity": "sha512-vUIhZ8LZoIWHBohiEObxVm6hwP034jwmc9kuq5GdHZH0wiLVLIPcMCdpJzG4C11cHoQ25TFIQj9kaVADVX7N3g==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-numbers/-/helper-numbers-1.11.6.tgz",
+            "version": "1.11.6"
         },
         "node_modules/@webassemblyjs/helper-wasm-bytecode": {
             "dev": true,
-            "integrity": "sha512-oC4Qa0bNcqnjAowFn7MPCETQgDYytpsfvz4ujZz63Zu/a/v71HeCAAmZsgZ3YVKec3zSPYytG3/PrRCqbtcAvA==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-wasm-bytecode/-/helper-wasm-bytecode-1.11.5.tgz",
-            "version": "1.11.5"
+            "integrity": "sha512-sFFHKwcmBprO9e7Icf0+gddyWYDViL8bpPjJJl0WHxCdETktXdmtWLGVzoHbqUcY4Be1LkNfwTmXOJUFZYSJdA==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-wasm-bytecode/-/helper-wasm-bytecode-1.11.6.tgz",
+            "version": "1.11.6"
         },
         "node_modules/@webassemblyjs/helper-wasm-section": {
             "dependencies": {
-                "@webassemblyjs/ast": "1.11.5",
-                "@webassemblyjs/helper-buffer": "1.11.5",
-                "@webassemblyjs/helper-wasm-bytecode": "1.11.5",
-                "@webassemblyjs/wasm-gen": "1.11.5"
+                "@webassemblyjs/ast": "1.11.6",
+                "@webassemblyjs/helper-buffer": "1.11.6",
+                "@webassemblyjs/helper-wasm-bytecode": "1.11.6",
+                "@webassemblyjs/wasm-gen": "1.11.6"
             },
             "dev": true,
-            "integrity": "sha512-uEoThA1LN2NA+K3B9wDo3yKlBfVtC6rh0i4/6hvbz071E8gTNZD/pT0MsBf7MeD6KbApMSkaAK0XeKyOZC7CIA==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-wasm-section/-/helper-wasm-section-1.11.5.tgz",
-            "version": "1.11.5"
+            "integrity": "sha512-LPpZbSOwTpEC2cgn4hTydySy1Ke+XEu+ETXuoyvuyezHO3Kjdu90KK95Sh9xTbmjrCsUwvWwCOQQNta37VrS9g==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-wasm-section/-/helper-wasm-section-1.11.6.tgz",
+            "version": "1.11.6"
         },
         "node_modules/@webassemblyjs/ieee754": {
             "dependencies": {
                 "@xtuc/ieee754": "^1.2.0"
             },
             "dev": true,
-            "integrity": "sha512-37aGq6qVL8A8oPbPrSGMBcp38YZFXcHfiROflJn9jxSdSMMM5dS5P/9e2/TpaJuhE+wFrbukN2WI6Hw9MH5acg==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/ieee754/-/ieee754-1.11.5.tgz",
-            "version": "1.11.5"
+            "integrity": "sha512-LM4p2csPNvbij6U1f19v6WR56QZ8JcHg3QIJTlSwzFcmx6WSORicYj6I63f9yU1kEUtrpG+kjkiIAkevHpDXrg==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/ieee754/-/ieee754-1.11.6.tgz",
+            "version": "1.11.6"
         },
         "node_modules/@webassemblyjs/leb128": {
             "dependencies": {
                 "@xtuc/long": "4.2.2"
             },
             "dev": true,
-            "integrity": "sha512-ajqrRSXaTJoPW+xmkfYN6l8VIeNnR4vBOTQO9HzR7IygoCcKWkICbKFbVTNMjMgMREqXEr0+2M6zukzM47ZUfQ==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/leb128/-/leb128-1.11.5.tgz",
-            "version": "1.11.5"
+            "integrity": "sha512-m7a0FhE67DQXgouf1tbN5XQcdWoNgaAuoULHIfGFIEVKA6tu/edls6XnIlkmS6FrXAquJRPni3ZZKjw6FSPjPQ==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/leb128/-/leb128-1.11.6.tgz",
+            "version": "1.11.6"
         },
         "node_modules/@webassemblyjs/utf8": {
             "dev": true,
-            "integrity": "sha512-WiOhulHKTZU5UPlRl53gHR8OxdGsSOxqfpqWeA2FmcwBMaoEdz6b2x2si3IwC9/fSPLfe8pBMRTHVMk5nlwnFQ==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/utf8/-/utf8-1.11.5.tgz",
-            "version": "1.11.5"
+            "integrity": "sha512-vtXf2wTQ3+up9Zsg8sa2yWiQpzSsMyXj0qViVP6xKGCUT8p8YJ6HqI7l5eCnWx1T/FYdsv07HQs2wTFbbof/RA==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/utf8/-/utf8-1.11.6.tgz",
+            "version": "1.11.6"
         },
         "node_modules/@webassemblyjs/wasm-edit": {
             "dependencies": {
-                "@webassemblyjs/ast": "1.11.5",
-                "@webassemblyjs/helper-buffer": "1.11.5",
-                "@webassemblyjs/helper-wasm-bytecode": "1.11.5",
-                "@webassemblyjs/helper-wasm-section": "1.11.5",
-                "@webassemblyjs/wasm-gen": "1.11.5",
-                "@webassemblyjs/wasm-opt": "1.11.5",
-                "@webassemblyjs/wasm-parser": "1.11.5",
-                "@webassemblyjs/wast-printer": "1.11.5"
+                "@webassemblyjs/ast": "1.11.6",
+                "@webassemblyjs/helper-buffer": "1.11.6",
+                "@webassemblyjs/helper-wasm-bytecode": "1.11.6",
+                "@webassemblyjs/helper-wasm-section": "1.11.6",
+                "@webassemblyjs/wasm-gen": "1.11.6",
+                "@webassemblyjs/wasm-opt": "1.11.6",
+                "@webassemblyjs/wasm-parser": "1.11.6",
+                "@webassemblyjs/wast-printer": "1.11.6"
             },
             "dev": true,
-            "integrity": "sha512-C0p9D2fAu3Twwqvygvf42iGCQ4av8MFBLiTb+08SZ4cEdwzWx9QeAHDo1E2k+9s/0w1DM40oflJOpkZ8jW4HCQ==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-edit/-/wasm-edit-1.11.5.tgz",
-            "version": "1.11.5"
+            "integrity": "sha512-Ybn2I6fnfIGuCR+Faaz7YcvtBKxvoLV3Lebn1tM4o/IAJzmi9AWYIPWpyBfU8cC+JxAO57bk4+zdsTjJR+VTOw==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-edit/-/wasm-edit-1.11.6.tgz",
+            "version": "1.11.6"
         },
         "node_modules/@webassemblyjs/wasm-gen": {
             "dependencies": {
-                "@webassemblyjs/ast": "1.11.5",
-                "@webassemblyjs/helper-wasm-bytecode": "1.11.5",
-                "@webassemblyjs/ieee754": "1.11.5",
-                "@webassemblyjs/leb128": "1.11.5",
-                "@webassemblyjs/utf8": "1.11.5"
+                "@webassemblyjs/ast": "1.11.6",
+                "@webassemblyjs/helper-wasm-bytecode": "1.11.6",
+                "@webassemblyjs/ieee754": "1.11.6",
+                "@webassemblyjs/leb128": "1.11.6",
+                "@webassemblyjs/utf8": "1.11.6"
             },
             "dev": true,
-            "integrity": "sha512-14vteRlRjxLK9eSyYFvw1K8Vv+iPdZU0Aebk3j6oB8TQiQYuO6hj9s4d7qf6f2HJr2khzvNldAFG13CgdkAIfA==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-gen/-/wasm-gen-1.11.5.tgz",
-            "version": "1.11.5"
+            "integrity": "sha512-3XOqkZP/y6B4F0PBAXvI1/bky7GryoogUtfwExeP/v7Nzwo1QLcq5oQmpKlftZLbT+ERUOAZVQjuNVak6UXjPA==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-gen/-/wasm-gen-1.11.6.tgz",
+            "version": "1.11.6"
         },
         "node_modules/@webassemblyjs/wasm-opt": {
             "dependencies": {
-                "@webassemblyjs/ast": "1.11.5",
-                "@webassemblyjs/helper-buffer": "1.11.5",
-                "@webassemblyjs/wasm-gen": "1.11.5",
-                "@webassemblyjs/wasm-parser": "1.11.5"
+                "@webassemblyjs/ast": "1.11.6",
+                "@webassemblyjs/helper-buffer": "1.11.6",
+                "@webassemblyjs/wasm-gen": "1.11.6",
+                "@webassemblyjs/wasm-parser": "1.11.6"
             },
             "dev": true,
-            "integrity": "sha512-tcKwlIXstBQgbKy1MlbDMlXaxpucn42eb17H29rawYLxm5+MsEmgPzeCP8B1Cl69hCice8LeKgZpRUAPtqYPgw==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-opt/-/wasm-opt-1.11.5.tgz",
-            "version": "1.11.5"
+            "integrity": "sha512-cOrKuLRE7PCe6AsOVl7WasYf3wbSo4CeOk6PkrjS7g57MFfVUF9u6ysQBBODX0LdgSvQqRiGz3CXvIDKcPNy4g==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-opt/-/wasm-opt-1.11.6.tgz",
+            "version": "1.11.6"
         },
         "node_modules/@webassemblyjs/wasm-parser": {
             "dependencies": {
-                "@webassemblyjs/ast": "1.11.5",
-                "@webassemblyjs/helper-api-error": "1.11.5",
-                "@webassemblyjs/helper-wasm-bytecode": "1.11.5",
-                "@webassemblyjs/ieee754": "1.11.5",
-                "@webassemblyjs/leb128": "1.11.5",
-                "@webassemblyjs/utf8": "1.11.5"
+                "@webassemblyjs/ast": "1.11.6",
+                "@webassemblyjs/helper-api-error": "1.11.6",
+                "@webassemblyjs/helper-wasm-bytecode": "1.11.6",
+                "@webassemblyjs/ieee754": "1.11.6",
+                "@webassemblyjs/leb128": "1.11.6",
+                "@webassemblyjs/utf8": "1.11.6"
             },
             "dev": true,
-            "integrity": "sha512-SVXUIwsLQlc8srSD7jejsfTU83g7pIGr2YYNb9oHdtldSxaOhvA5xwvIiWIfcX8PlSakgqMXsLpLfbbJ4cBYew==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-parser/-/wasm-parser-1.11.5.tgz",
-            "version": "1.11.5"
+            "integrity": "sha512-6ZwPeGzMJM3Dqp3hCsLgESxBGtT/OeCvCZ4TA1JUPYgmhAx38tTPR9JaKy0S5H3evQpO/h2uWs2j6Yc/fjkpTQ==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-parser/-/wasm-parser-1.11.6.tgz",
+            "version": "1.11.6"
         },
         "node_modules/@webassemblyjs/wast-printer": {
             "dependencies": {
-                "@webassemblyjs/ast": "1.11.5",
+                "@webassemblyjs/ast": "1.11.6",
                 "@xtuc/long": "4.2.2"
             },
             "dev": true,
-            "integrity": "sha512-f7Pq3wvg3GSPUPzR0F6bmI89Hdb+u9WXrSKc4v+N0aV0q6r42WoF92Jp2jEorBEBRoRNXgjp53nBniDXcqZYPA==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/wast-printer/-/wast-printer-1.11.5.tgz",
-            "version": "1.11.5"
+            "integrity": "sha512-JM7AhRcE+yW2GWYaKeHL5vt4xqee5N2WcezptmgyhNS+ScggqcT1OtXykhAb13Sn5Yas0j2uv9tHgrjwvzAP4A==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wast-printer/-/wast-printer-1.11.6.tgz",
+            "version": "1.11.6"
         },
         "node_modules/@webpack-cli/configtest": {
             "dev": true,
             "engines": {
                 "node": ">=14.15.0"
             },
-            "integrity": "sha512-njsdJXJSiS2iNbQVS0eT8A/KPnmyH4pv1APj2K0d1wrZcBLw+yppxOy4CGqa0OxDJkzfL/XELDhD8rocnIwB5A==",
+            "integrity": "sha512-wy0mglZpDSiSS0XHrVR+BAdId2+yxPSoJW8fsna3ZpYSlufjvxnP4YbKTCBZnNIcGN4r6ZPXV55X4mYExOfLmw==",
             "peerDependencies": {
                 "webpack": "5.x.x",
                 "webpack-cli": "5.x.x"
             },
-            "resolved": "https://registry.npmjs.org/@webpack-cli/configtest/-/configtest-2.0.1.tgz",
-            "version": "2.0.1"
+            "resolved": "https://registry.npmjs.org/@webpack-cli/configtest/-/configtest-2.1.1.tgz",
+            "version": "2.1.1"
         },
         "node_modules/@webpack-cli/info": {
             "dev": true,
             "engines": {
                 "node": ">=14.15.0"
             },
-            "integrity": "sha512-fE1UEWTwsAxRhrJNikE7v4EotYflkEhBL7EbajfkPlf6E37/2QshOy/D48Mw8G5XMFlQtS6YV42vtbG9zBpIQA==",
+            "integrity": "sha512-zLHQdI/Qs1UyT5UBdWNqsARasIA+AaF8t+4u2aS2nEpBQh2mWIVb8qAklq0eUENnC5mOItrIB4LiS9xMtph18A==",
             "peerDependencies": {
                 "webpack": "5.x.x",
                 "webpack-cli": "5.x.x"
             },
-            "resolved": "https://registry.npmjs.org/@webpack-cli/info/-/info-2.0.1.tgz",
-            "version": "2.0.1"
+            "resolved": "https://registry.npmjs.org/@webpack-cli/info/-/info-2.0.2.tgz",
+            "version": "2.0.2"
         },
         "node_modules/@webpack-cli/serve": {
             "dev": true,
             "engines": {
                 "node": ">=14.15.0"
             },
-            "integrity": "sha512-S9h3GmOmzUseyeFW3tYNnWS7gNUuwxZ3mmMq0JyW78Vx1SGKPSkt5bT4pB0rUnVfHjP0EL9gW2bOzmtiTfQt0A==",
+            "integrity": "sha512-lqaoKnRYBdo1UgDX8uF24AfGMifWK19TxPmM5FHc2vAGxrJ/qtyUyFBWoY1tISZdelsQ5fBcOusifo5o5wSJxQ==",
             "peerDependencies": {
                 "webpack": "5.x.x",
                 "webpack-cli": "5.x.x"
             },
             "peerDependenciesMeta": {
                 "webpack-dev-server": {
                     "optional": true
                 }
             },
-            "resolved": "https://registry.npmjs.org/@webpack-cli/serve/-/serve-2.0.2.tgz",
-            "version": "2.0.2"
+            "resolved": "https://registry.npmjs.org/@webpack-cli/serve/-/serve-2.0.5.tgz",
+            "version": "2.0.5"
         },
         "node_modules/@xtuc/ieee754": {
             "dev": true,
             "integrity": "sha512-DX8nKgqcGwsc0eJSqYt5lwP4DH5FlHnmuWWBRy7X0NcaGR0ZtuyeESgMwTYVEtxmsNGY+qit4QYT/MIYTOTPeA==",
             "resolved": "https://registry.npmjs.org/@xtuc/ieee754/-/ieee754-1.2.0.tgz",
             "version": "1.2.0"
         },
@@ -894,26 +903,26 @@
             "bin": {
                 "acorn": "bin/acorn"
             },
             "dev": true,
             "engines": {
                 "node": ">=0.4.0"
             },
-            "integrity": "sha512-xjIYgE8HBrkpd/sJqOGNspf8uHG+NOHGOw6a/Urj8taM2EXfdNAH2oFcPeIFfsv3+kz/mJrS5VuMqbNLjCa2vw==",
-            "resolved": "https://registry.npmjs.org/acorn/-/acorn-8.8.2.tgz",
-            "version": "8.8.2"
+            "integrity": "sha512-F0SAmZ8iUtS//m8DmCTA0jlh6TDKkHQyK6xc6V4KDTyZKA9dnvX9/3sRTVQrWm79glUAZbnmmNcdYwUIHWVybw==",
+            "resolved": "https://registry.npmjs.org/acorn/-/acorn-8.10.0.tgz",
+            "version": "8.10.0"
         },
         "node_modules/acorn-import-assertions": {
             "dev": true,
-            "integrity": "sha512-m7VZ3jwz4eK6A4Vtt8Ew1/mNbP24u0FhdyfA7fSvnJR6LMdfOYnmuIrrJAgrYfYJ10F/otaHTtrtrtmHdMNzEw==",
+            "integrity": "sha512-cmMwop9x+8KFhxvKrKfPYmN6/pKTYYHBqLa0DfvVZcKMJWNyWLnaqND7dx/qn66R7ewM1UX5XMaDVP5wlVTaVA==",
             "peerDependencies": {
                 "acorn": "^8"
             },
-            "resolved": "https://registry.npmjs.org/acorn-import-assertions/-/acorn-import-assertions-1.8.0.tgz",
-            "version": "1.8.0"
+            "resolved": "https://registry.npmjs.org/acorn-import-assertions/-/acorn-import-assertions-1.9.0.tgz",
+            "version": "1.9.0"
         },
         "node_modules/acorn-jsx": {
             "dev": true,
             "integrity": "sha512-rq9s+JNhf0IChjtDXxllJ7g41oZk5SlXtp0LHwyA5cejwn7vKmKp4pPri6YEePv2PU65sAsegbXtIinmDFDXgQ==",
             "peerDependencies": {
                 "acorn": "^6.0.0 || ^7.0.0 || ^8.0.0"
             },
@@ -1148,22 +1157,14 @@
         },
         "node_modules/argparse": {
             "dev": true,
             "integrity": "sha512-8+9WqebbFzpX9OR+Wa6O29asIogeRMzcGtAINdpMHHyAg10f05aSFVBbcEqGf/PXw1EjAZ+q2/bEBg3DvurK3Q==",
             "resolved": "https://registry.npmjs.org/argparse/-/argparse-2.0.1.tgz",
             "version": "2.0.1"
         },
-        "node_modules/arr-flatten": {
-            "engines": {
-                "node": ">=0.10.0"
-            },
-            "integrity": "sha512-L3hKV5R/p5o81R7O02IGnwpDmkp6E982XhtbuwSe3O4qOtMMMtodicASA1Cny2U+aCXcNpml+m4dPsvsJ3jatg==",
-            "resolved": "https://registry.npmjs.org/arr-flatten/-/arr-flatten-1.1.0.tgz",
-            "version": "1.1.0"
-        },
         "node_modules/array-bounds": {
             "integrity": "sha512-8wdW3ZGk6UjMPJx/glyEt0sLzzwAE1bhToPsO1W2pbpR2gULyxe3BjSiuJFheP50T/GgODVPz2fuMUmIywt8cQ==",
             "resolved": "https://registry.npmjs.org/array-bounds/-/array-bounds-1.0.1.tgz",
             "version": "1.0.1"
         },
         "node_modules/array-buffer-byte-length": {
             "dependencies": {
@@ -1219,14 +1220,33 @@
             "version": "1.0.1"
         },
         "node_modules/array-rearrange": {
             "integrity": "sha512-UfobP5N12Qm4Qu4fwLDIi2v6+wZsSf6snYSxAMeKhrh37YGnNWZPRmVEKc/2wfms53TLQnzfpG8wCx2Y/6NG1w==",
             "resolved": "https://registry.npmjs.org/array-rearrange/-/array-rearrange-2.2.2.tgz",
             "version": "2.2.2"
         },
+        "node_modules/array.prototype.findlastindex": {
+            "dependencies": {
+                "call-bind": "^1.0.2",
+                "define-properties": "^1.1.4",
+                "es-abstract": "^1.20.4",
+                "es-shim-unscopables": "^1.0.0",
+                "get-intrinsic": "^1.1.3"
+            },
+            "dev": true,
+            "engines": {
+                "node": ">= 0.4"
+            },
+            "funding": {
+                "url": "https://github.com/sponsors/ljharb"
+            },
+            "integrity": "sha512-tb5thFFlUcp7NdNF6/MpDk/1r/4awWG1FIz3YqDf+/zJSTezBb+/5WViH41obXULHVpDzoiCLpJ/ZO9YbJMsdw==",
+            "resolved": "https://registry.npmjs.org/array.prototype.findlastindex/-/array.prototype.findlastindex-1.2.2.tgz",
+            "version": "1.2.2"
+        },
         "node_modules/array.prototype.flat": {
             "dependencies": {
                 "call-bind": "^1.0.2",
                 "define-properties": "^1.1.4",
                 "es-abstract": "^1.20.4",
                 "es-shim-unscopables": "^1.0.0"
             },
@@ -1255,14 +1275,34 @@
             "funding": {
                 "url": "https://github.com/sponsors/ljharb"
             },
             "integrity": "sha512-8UGn9O1FDVvMNB0UlLv4voxRMze7+FpHyF5mSMRjWHUMlpoDViniy05870VlxhfgTnLbpuwTzvD76MTtWxB/mQ==",
             "resolved": "https://registry.npmjs.org/array.prototype.flatmap/-/array.prototype.flatmap-1.3.1.tgz",
             "version": "1.3.1"
         },
+        "node_modules/arraybuffer.prototype.slice": {
+            "dependencies": {
+                "array-buffer-byte-length": "^1.0.0",
+                "call-bind": "^1.0.2",
+                "define-properties": "^1.2.0",
+                "get-intrinsic": "^1.2.1",
+                "is-array-buffer": "^3.0.2",
+                "is-shared-array-buffer": "^1.0.2"
+            },
+            "dev": true,
+            "engines": {
+                "node": ">= 0.4"
+            },
+            "funding": {
+                "url": "https://github.com/sponsors/ljharb"
+            },
+            "integrity": "sha512-09x0ZWFEjj4WD8PDbykUwo3t9arLn8NIzmmYEJFpYekOAQjpkGSyrQhNoRTcwwcFRu+ycWF78QZ63oWTqSjBcw==",
+            "resolved": "https://registry.npmjs.org/arraybuffer.prototype.slice/-/arraybuffer.prototype.slice-1.0.1.tgz",
+            "version": "1.0.1"
+        },
         "node_modules/arrify": {
             "dev": true,
             "engines": {
                 "node": ">=0.10.0"
             },
             "integrity": "sha512-3CYzex9M9FGQjCGMGyi6/31c8GJbgb0qGyrx5HWxPd0aCwh4cB2YjMb2Xf9UuoogrMrlO9cTqnB5rI5GHZTcUA==",
             "resolved": "https://registry.npmjs.org/arrify/-/arrify-1.0.1.tgz",
@@ -1279,19 +1319,14 @@
             "engines": {
                 "node": "*"
             },
             "integrity": "sha512-VUeSMD8nEGBWaZK4lizI1sf3yEC7pnAQ/mrI7pC2fBz2s/tq5jWWEngTwaf0Gruu/OoXRGLGg1XFqpYBiGTYJA==",
             "resolved": "https://registry.npmjs.org/async-foreach/-/async-foreach-0.1.3.tgz",
             "version": "0.1.3"
         },
-        "node_modules/atob-lite": {
-            "integrity": "sha512-LEeSAWeh2Gfa2FtlQE1shxQ8zi5F9GHarrGKz08TMdODD5T4eH6BMsvtnhbWZ+XQn+Gb6om/917ucvRu7l7ukw==",
-            "resolved": "https://registry.npmjs.org/atob-lite/-/atob-lite-2.0.0.tgz",
-            "version": "2.0.0"
-        },
         "node_modules/autoprefixer": {
             "bin": {
                 "autoprefixer": "bin/autoprefixer"
             },
             "dependencies": {
                 "browserslist": "^4.21.5",
                 "caniuse-lite": "^1.0.30001464",
@@ -1437,20 +1472,20 @@
                     "url": "https://github.com/sponsors/twbs"
                 },
                 {
                     "type": "opencollective",
                     "url": "https://opencollective.com/bootstrap"
                 }
             ],
-            "integrity": "sha512-cEKPM+fwb3cT8NzQZYEu4HilJ3anCrWqh3CHAok1p9jXqMPsPTBhU25fBckEJHJ/p+tTxTFTsFQGM+gaHpi3QQ==",
+            "integrity": "sha512-jzwza3Yagduci2x0rr9MeFSORjcHpt0lRZukZPZQJT1Dth5qzV7XcgGqYzi39KGAVYR8QEDVoO0ubFKOxzMG+g==",
             "peerDependencies": {
-                "@popperjs/core": "^2.11.6"
+                "@popperjs/core": "^2.11.8"
             },
-            "resolved": "https://registry.npmjs.org/bootstrap/-/bootstrap-5.2.3.tgz",
-            "version": "5.2.3"
+            "resolved": "https://registry.npmjs.org/bootstrap/-/bootstrap-5.3.1.tgz",
+            "version": "5.3.1"
         },
         "node_modules/brace-expansion": {
             "dependencies": {
                 "balanced-match": "^1.0.0",
                 "concat-map": "0.0.1"
             },
             "dev": true,
@@ -1459,36 +1494,40 @@
             "version": "1.1.11"
         },
         "node_modules/browserslist": {
             "bin": {
                 "browserslist": "cli.js"
             },
             "dependencies": {
-                "caniuse-lite": "^1.0.30001449",
-                "electron-to-chromium": "^1.4.284",
-                "node-releases": "^2.0.8",
-                "update-browserslist-db": "^1.0.10"
+                "caniuse-lite": "^1.0.30001503",
+                "electron-to-chromium": "^1.4.431",
+                "node-releases": "^2.0.12",
+                "update-browserslist-db": "^1.0.11"
             },
             "dev": true,
             "engines": {
                 "node": "^6 || ^7 || ^8 || ^9 || ^10 || ^11 || ^12 || >=13.7"
             },
             "funding": [
                 {
                     "type": "opencollective",
                     "url": "https://opencollective.com/browserslist"
                 },
                 {
                     "type": "tidelift",
                     "url": "https://tidelift.com/funding/github/npm/browserslist"
+                },
+                {
+                    "type": "github",
+                    "url": "https://github.com/sponsors/ai"
                 }
             ],
-            "integrity": "sha512-tUkiguQGW7S3IhB7N+c2MV/HZPSCPAAiYBZXLsBhFB/PCy6ZKKsZrmBayHV9fdGV/ARIfJ14NkxKzRDjvp7L6w==",
-            "resolved": "https://registry.npmjs.org/browserslist/-/browserslist-4.21.5.tgz",
-            "version": "4.21.5"
+            "integrity": "sha512-M0MFoZzbUrRU4KNfCrDLnvyE7gub+peetoTid3TBIqtunaDJyXlwhakT+/VkvSXcfIzFfK/nkCs4nmyTmxdNSg==",
+            "resolved": "https://registry.npmjs.org/browserslist/-/browserslist-4.21.9.tgz",
+            "version": "4.21.9"
         },
         "node_modules/buffer": {
             "dependencies": {
                 "base64-js": "^1.3.1",
                 "ieee754": "^1.1.13"
             },
             "dev": true,
@@ -1673,17 +1712,17 @@
                     "url": "https://tidelift.com/funding/github/npm/caniuse-lite"
                 },
                 {
                     "type": "github",
                     "url": "https://github.com/sponsors/ai"
                 }
             ],
-            "integrity": "sha512-KCqHwRnaa1InZBtqXzP98LPg0ajCVujMKjqKDhZEthIpAsJl/YEIa3YvXjGXPVqzZVguccuu7ga9KOE1J9rKPQ==",
-            "resolved": "https://registry.npmjs.org/caniuse-lite/-/caniuse-lite-1.0.30001481.tgz",
-            "version": "1.0.30001481"
+            "integrity": "sha512-Vdhm5S11DaFVLlyiKu4hiUTkpZu+y1KA/rZZqVQfOD5YdDT/eQKlkt7NaE0WGOFgX32diqt9MiP9CAiFeRklaA==",
+            "resolved": "https://registry.npmjs.org/caniuse-lite/-/caniuse-lite-1.0.30001517.tgz",
+            "version": "1.0.30001517"
         },
         "node_modules/canvas-fit": {
             "dependencies": {
                 "element-size": "^1.1.1"
             },
             "integrity": "sha512-onIcjRpz69/Hx5bB5HGbYKUF2uC6QT6Gp+pfpGm3A7mPfcluSLV5v4Zu+oflDUwLdUw0rLIBhUbi0v8hM4FJQQ==",
             "resolved": "https://registry.npmjs.org/canvas-fit/-/canvas-fit-1.5.0.tgz",
@@ -1883,26 +1922,14 @@
             "engines": {
                 "node": ">= 10"
             },
             "integrity": "sha512-QLdDLCKNV2dtoTorqgxngQCMA+gWXkM/Nwu7FpeBhk/RdkzimqC3jueb/FDmaZeXh+uby1jkBqE3xArsLBE5wQ==",
             "resolved": "https://registry.npmjs.org/compress-commons/-/compress-commons-4.1.1.tgz",
             "version": "4.1.1"
         },
-        "node_modules/compute-dims": {
-            "dependencies": {
-                "utils-copy": "^1.0.0",
-                "validate.io-array": "^1.0.6",
-                "validate.io-matrix-like": "^1.0.2",
-                "validate.io-ndarray-like": "^1.0.0",
-                "validate.io-positive-integer": "^1.0.0"
-            },
-            "integrity": "sha512-YHMiIKjH/8Eom8zATk3g8/lH3HxGCZcVQyEfEoVrfWI7od/WRpTgRGShnei3jArYSx77mQqPxZNokjGHCdLfxg==",
-            "resolved": "https://registry.npmjs.org/compute-dims/-/compute-dims-1.1.0.tgz",
-            "version": "1.1.0"
-        },
         "node_modules/concat-map": {
             "dev": true,
             "integrity": "sha512-/Srv4dswyQNBfohGpz9o6Yb3Gz3SrUDqBH5rTuhGR7ahtlbYKnVxw2bCFMRljaA7EXHaXZ8wsHdodFvbkhKmqg==",
             "resolved": "https://registry.npmjs.org/concat-map/-/concat-map-0.0.1.tgz",
             "version": "0.0.1"
         },
         "node_modules/concat-stream": {
@@ -1953,24 +1980,14 @@
         },
         "node_modules/console-control-strings": {
             "dev": true,
             "integrity": "sha512-ty/fTekppD2fIwRvnZAVdeOiGd1c7YXEixbgJTNzqcxJWKQnjJ/V1bNEEE6hygpM3WjwHFUVK6HTjWSzV4a8sQ==",
             "resolved": "https://registry.npmjs.org/console-control-strings/-/console-control-strings-1.1.0.tgz",
             "version": "1.1.0"
         },
-        "node_modules/const-max-uint32": {
-            "integrity": "sha512-T8/9bffg5RThuejasJWrwqxs3Q0fsJvyl7/33IB6svroD8JC93E7X60AuuOnDE8RlP6Jlb5FxmlrVDpl9KiU2Q==",
-            "resolved": "https://registry.npmjs.org/const-max-uint32/-/const-max-uint32-1.0.2.tgz",
-            "version": "1.0.2"
-        },
-        "node_modules/const-pinf-float64": {
-            "integrity": "sha512-wfs+V4HdSN7C3CWJWR7hVa24yTPn3mDJthwhRIObZBh6UjTjkUMUrCP3UrNGozB/HjTpcScnGXtQUNa+yjsIJQ==",
-            "resolved": "https://registry.npmjs.org/const-pinf-float64/-/const-pinf-float64-1.0.0.tgz",
-            "version": "1.0.0"
-        },
         "node_modules/core-util-is": {
             "integrity": "sha512-ZQBvi1DcpJ4GDqanjucZ2Hj3wEO5pZDS89BWbkcrvdxksJorwUDDZamX9ldFkp9aw2lmBDLgkObEA4DWNJ9FYQ==",
             "resolved": "https://registry.npmjs.org/core-util-is/-/core-util-is-1.0.3.tgz",
             "version": "1.0.3"
         },
         "node_modules/cosmiconfig": {
             "dependencies": {
@@ -1982,17 +1999,17 @@
             "dev": true,
             "engines": {
                 "node": ">=14"
             },
             "funding": {
                 "url": "https://github.com/sponsors/d-fischer"
             },
-            "integrity": "sha512-/UkO2JKI18b5jVMJUp0lvKFMpa/Gye+ZgZjKD+DGEN9y7NRcf/nK1A0sp67ONmKtnDCNMS44E6jrk0Yc3bDuUw==",
-            "resolved": "https://registry.npmjs.org/cosmiconfig/-/cosmiconfig-8.1.3.tgz",
-            "version": "8.1.3"
+            "integrity": "sha512-3rTMnFJA1tCOPwRxtgF4wd7Ab2qvDbL8jX+3smjIbS4HlZBagTlpERbdN7iAbWlrfxE3M8c27kTwTawQ7st+OQ==",
+            "resolved": "https://registry.npmjs.org/cosmiconfig/-/cosmiconfig-8.2.0.tgz",
+            "version": "8.2.0"
         },
         "node_modules/country-regex": {
             "integrity": "sha512-iSPlClZP8vX7MC3/u6s3lrDuoQyhQukh5LyABJ3hvfzbQ3Yyayd4fp04zjLnfi267B/B2FkumcWWgrbban7sSA==",
             "resolved": "https://registry.npmjs.org/country-regex/-/country-regex-1.1.0.tgz",
             "version": "1.1.0"
         },
         "node_modules/crc-32": {
@@ -2074,36 +2091,36 @@
             "integrity": "sha512-X1xgQhkZ9n94WDwntqst5D/FKkmiU0GlJSFZSV3kLvyJ1WC5VeyoXDOuleUD+SIuH9C7W05is++0Woh0CGfKjQ==",
             "resolved": "https://registry.npmjs.org/css-global-keywords/-/css-global-keywords-1.0.1.tgz",
             "version": "1.0.1"
         },
         "node_modules/css-loader": {
             "dependencies": {
                 "icss-utils": "^5.1.0",
-                "postcss": "^8.4.19",
+                "postcss": "^8.4.21",
                 "postcss-modules-extract-imports": "^3.0.0",
-                "postcss-modules-local-by-default": "^4.0.0",
+                "postcss-modules-local-by-default": "^4.0.3",
                 "postcss-modules-scope": "^3.0.0",
                 "postcss-modules-values": "^4.0.0",
                 "postcss-value-parser": "^4.2.0",
                 "semver": "^7.3.8"
             },
             "dev": true,
             "engines": {
                 "node": ">= 12.13.0"
             },
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/webpack"
             },
-            "integrity": "sha512-qhOH1KlBMnZP8FzRO6YCH9UHXQhVMcEGLyNdb7Hv2cpcmJbW0YrddO+tG1ab5nT41KpHIYGsbeHqxB9xPu1pKQ==",
+            "integrity": "sha512-xDAXtEVGlD0gJ07iclwWVkLoZOpEvAWaSyf6W18S2pOC//K8+qUDIx8IIT3D+HjnmkJPQeesOPv5aiUaJsCM2g==",
             "peerDependencies": {
                 "webpack": "^5.0.0"
             },
-            "resolved": "https://registry.npmjs.org/css-loader/-/css-loader-6.7.3.tgz",
-            "version": "6.7.3"
+            "resolved": "https://registry.npmjs.org/css-loader/-/css-loader-6.8.1.tgz",
+            "version": "6.8.1"
         },
         "node_modules/css-select": {
             "dependencies": {
                 "boolbase": "^1.0.0",
                 "css-what": "^6.0.1",
                 "domhandler": "^4.3.1",
                 "domutils": "^2.8.0",
@@ -2192,28 +2209,28 @@
                 "d3-timer": "3",
                 "d3-transition": "3",
                 "d3-zoom": "3"
             },
             "engines": {
                 "node": ">=12"
             },
-            "integrity": "sha512-q2WHStdhiBtD8DMmhDPyJmXUxr6VWRngKyiJ5EfXMxPw+tqT6BhNjhJZ4w3BHsNm3QoVfZLY8Orq/qPFczwKRA==",
-            "resolved": "https://registry.npmjs.org/d3/-/d3-7.8.4.tgz",
-            "version": "7.8.4"
+            "integrity": "sha512-JgoahDG51ncUfJu6wX/1vWQEqOflgXyl4MaHqlcSruTez7yhaRKR9i8VjjcQGeS2en/jnFivXuaIMnseMMt0XA==",
+            "resolved": "https://registry.npmjs.org/d3/-/d3-7.8.5.tgz",
+            "version": "7.8.5"
         },
         "node_modules/d3-array": {
             "dependencies": {
                 "internmap": "1 - 2"
             },
             "engines": {
                 "node": ">=12"
             },
-            "integrity": "sha512-JRHwbQQ84XuAESWhvIPaUV4/1UYTBOLiOPGWqgFDHZS1D5QN9c57FbH3QpEnQMYiOXNzKUQyGTZf+EVO7RT5TQ==",
-            "resolved": "https://registry.npmjs.org/d3-array/-/d3-array-3.2.3.tgz",
-            "version": "3.2.3"
+            "integrity": "sha512-tdQAmyA18i4J7wprpYq8ClcxZy3SC31QMeByyCFyRt7BVHdREQZ5lpzoe5mFEYZUWe+oq8HBvk9JjpibyEV4Jg==",
+            "resolved": "https://registry.npmjs.org/d3-array/-/d3-array-3.2.4.tgz",
+            "version": "3.2.4"
         },
         "node_modules/d3-axis": {
             "engines": {
                 "node": ">=12"
             },
             "integrity": "sha512-IH5tgjV4jE/GhHkRV0HiVYPDtvfjHQlQfJHs0usq7M30XcSBvOotpmH1IgkcXsO/5gEQZD43B//fc7SRT5S+xw==",
             "resolved": "https://registry.npmjs.org/d3-axis/-/d3-axis-3.0.0.tgz",
@@ -2851,17 +2868,17 @@
         "node_modules/earcut": {
             "integrity": "sha512-/pjZsA1b4RPHbeWZQn66SWS8nZZWLQQ23oE3Eam7aroEFGEvwKAsJfZ9ytiEMycfzXWpca4FA9QIOehf7PocBQ==",
             "resolved": "https://registry.npmjs.org/earcut/-/earcut-2.2.4.tgz",
             "version": "2.2.4"
         },
         "node_modules/electron-to-chromium": {
             "dev": true,
-            "integrity": "sha512-H3BYG6DW5Z+l0xcfXaicJGxrpA4kMlCxnN71+iNX+dBLkRMOdVJqFJiAmbNZZKA1zISpRg17JR03qGifXNsJtw==",
-            "resolved": "https://registry.npmjs.org/electron-to-chromium/-/electron-to-chromium-1.4.377.tgz",
-            "version": "1.4.377"
+            "integrity": "sha512-shUVy6Eawp33dFBFIoYbIwLHrX0IZ857AlH9ug2o4rvbWmpaCUdBpQ5Zw39HRrfzAFm4APJE9V+E2A/WB0YqJw==",
+            "resolved": "https://registry.npmjs.org/electron-to-chromium/-/electron-to-chromium-1.4.477.tgz",
+            "version": "1.4.477"
         },
         "node_modules/element-size": {
             "integrity": "sha512-eaN+GMOq/Q+BIWy0ybsgpcYImjGIdNLyjLFJU4XsLHXYQao5jCNb36GyN6C2qwmDDYSfIBmKpPpr4VnBdLCsPQ==",
             "resolved": "https://registry.npmjs.org/element-size/-/element-size-1.1.1.tgz",
             "version": "1.1.1"
         },
         "node_modules/elementary-circuits-directed-graph": {
@@ -2910,17 +2927,17 @@
                 "graceful-fs": "^4.2.4",
                 "tapable": "^2.2.0"
             },
             "dev": true,
             "engines": {
                 "node": ">=10.13.0"
             },
-            "integrity": "sha512-eyV8f0y1+bzyfh8xAwW/WTSZpLbjhqc4ne9eGSH4Zo2ejdyiNG9pU6mf9DG8a7+Auk6MFTlNOT4Y2y/9k8GKVg==",
-            "resolved": "https://registry.npmjs.org/enhanced-resolve/-/enhanced-resolve-5.13.0.tgz",
-            "version": "5.13.0"
+            "integrity": "sha512-LXYT42KJ7lpIKECr2mAXIaMldcNCh/7E0KBKOu4KSfkHmP+mZmSs+8V5gBAqisWBy0OO4W5Oyys0GO1Y8KtdKg==",
+            "resolved": "https://registry.npmjs.org/enhanced-resolve/-/enhanced-resolve-5.15.0.tgz",
+            "version": "5.15.0"
         },
         "node_modules/entities": {
             "dev": true,
             "engines": {
                 "node": ">=0.12"
             },
             "funding": {
@@ -2943,17 +2960,17 @@
             "bin": {
                 "envinfo": "dist/cli.js"
             },
             "dev": true,
             "engines": {
                 "node": ">=4"
             },
-            "integrity": "sha512-/o+BXHmB7ocbHEAs6F2EnG0ogybVVUdkRunTT2glZU9XAaGmhqskrvKwqXuDfNjEO0LZKWdejEEpnq8aM0tOaw==",
-            "resolved": "https://registry.npmjs.org/envinfo/-/envinfo-7.8.1.tgz",
-            "version": "7.8.1"
+            "integrity": "sha512-ZtUjZO6l5mwTHvc1L9+1q5p/R3wTopcfqMW8r5t8SJSKqeVI/LtajORwRFEKpEFuekjD0VBjwu1HMxL4UalIRw==",
+            "resolved": "https://registry.npmjs.org/envinfo/-/envinfo-7.10.0.tgz",
+            "version": "7.10.0"
         },
         "node_modules/err-code": {
             "dev": true,
             "integrity": "sha512-2bmlRpNKBxT/CRmPOlyISQpNj+qSeYvcym/uT0Jx2bMOlKLtSy1ZmLuVxSEKKyor/N5yhvp/ZiG1oE3DEYMSFA==",
             "resolved": "https://registry.npmjs.org/err-code/-/err-code-2.0.3.tgz",
             "version": "2.0.3"
         },
@@ -2965,20 +2982,21 @@
             "integrity": "sha512-7dFHNmqeFSEt2ZBsCriorKnn3Z2pj+fd9kmI6QoWw4//DL+icEBfc0U7qJCisqrTsKTjw4fNFy2pW9OqStD84g==",
             "resolved": "https://registry.npmjs.org/error-ex/-/error-ex-1.3.2.tgz",
             "version": "1.3.2"
         },
         "node_modules/es-abstract": {
             "dependencies": {
                 "array-buffer-byte-length": "^1.0.0",
+                "arraybuffer.prototype.slice": "^1.0.1",
                 "available-typed-arrays": "^1.0.5",
                 "call-bind": "^1.0.2",
                 "es-set-tostringtag": "^2.0.1",
                 "es-to-primitive": "^1.2.1",
                 "function.prototype.name": "^1.1.5",
-                "get-intrinsic": "^1.2.0",
+                "get-intrinsic": "^1.2.1",
                 "get-symbol-description": "^1.0.0",
                 "globalthis": "^1.0.3",
                 "gopd": "^1.0.1",
                 "has": "^1.0.3",
                 "has-property-descriptors": "^1.0.0",
                 "has-proto": "^1.0.1",
                 "has-symbols": "^1.0.3",
@@ -2990,39 +3008,43 @@
                 "is-shared-array-buffer": "^1.0.2",
                 "is-string": "^1.0.7",
                 "is-typed-array": "^1.1.10",
                 "is-weakref": "^1.0.2",
                 "object-inspect": "^1.12.3",
                 "object-keys": "^1.1.1",
                 "object.assign": "^4.1.4",
-                "regexp.prototype.flags": "^1.4.3",
+                "regexp.prototype.flags": "^1.5.0",
+                "safe-array-concat": "^1.0.0",
                 "safe-regex-test": "^1.0.0",
                 "string.prototype.trim": "^1.2.7",
                 "string.prototype.trimend": "^1.0.6",
                 "string.prototype.trimstart": "^1.0.6",
+                "typed-array-buffer": "^1.0.0",
+                "typed-array-byte-length": "^1.0.0",
+                "typed-array-byte-offset": "^1.0.0",
                 "typed-array-length": "^1.0.4",
                 "unbox-primitive": "^1.0.2",
-                "which-typed-array": "^1.1.9"
+                "which-typed-array": "^1.1.10"
             },
             "dev": true,
             "engines": {
                 "node": ">= 0.4"
             },
             "funding": {
                 "url": "https://github.com/sponsors/ljharb"
             },
-            "integrity": "sha512-y/B5POM2iBnIxCiernH1G7rC9qQoM77lLIMQLuob0zhp8C56Po81+2Nj0WFKnd0pNReDTnkYryc+zhOzpEIROg==",
-            "resolved": "https://registry.npmjs.org/es-abstract/-/es-abstract-1.21.2.tgz",
-            "version": "1.21.2"
+            "integrity": "sha512-ioRRcXMO6OFyRpyzV3kE1IIBd4WG5/kltnzdxSCqoP8CMGs/Li+M1uF5o7lOkZVFjDs+NLesthnF66Pg/0q0Lw==",
+            "resolved": "https://registry.npmjs.org/es-abstract/-/es-abstract-1.22.1.tgz",
+            "version": "1.22.1"
         },
         "node_modules/es-module-lexer": {
             "dev": true,
-            "integrity": "sha512-9978wrXM50Y4rTMmW5kXIC09ZdXQZqkE4mxhwkd8VbzsGkXGPgV4zWuqQJgCEzYngdo2dYDa0l8xhX4fkSwJSg==",
-            "resolved": "https://registry.npmjs.org/es-module-lexer/-/es-module-lexer-1.2.1.tgz",
-            "version": "1.2.1"
+            "integrity": "sha512-vZK7T0N2CBmBOixhmjdqx2gWVbFZ4DXZ/NyRMZVlJXPa7CyFS+/a4QQsDGDQy9ZfEzxFuNEsMLeQJnKP2p5/JA==",
+            "resolved": "https://registry.npmjs.org/es-module-lexer/-/es-module-lexer-1.3.0.tgz",
+            "version": "1.3.0"
         },
         "node_modules/es-set-tostringtag": {
             "dependencies": {
                 "get-intrinsic": "^1.1.3",
                 "has": "^1.0.3",
                 "has-tostringtag": "^1.0.0"
             },
@@ -3203,90 +3225,90 @@
         },
         "node_modules/eslint": {
             "bin": {
                 "eslint": "bin/eslint.js"
             },
             "dependencies": {
                 "@eslint-community/eslint-utils": "^4.2.0",
-                "@eslint-community/regexpp": "^4.4.0",
-                "@eslint/eslintrc": "^2.0.2",
-                "@eslint/js": "8.39.0",
-                "@humanwhocodes/config-array": "^0.11.8",
+                "@eslint-community/regexpp": "^4.6.1",
+                "@eslint/eslintrc": "^2.1.1",
+                "@eslint/js": "^8.46.0",
+                "@humanwhocodes/config-array": "^0.11.10",
                 "@humanwhocodes/module-importer": "^1.0.1",
                 "@nodelib/fs.walk": "^1.2.8",
-                "ajv": "^6.10.0",
+                "ajv": "^6.12.4",
                 "chalk": "^4.0.0",
                 "cross-spawn": "^7.0.2",
                 "debug": "^4.3.2",
                 "doctrine": "^3.0.0",
                 "escape-string-regexp": "^4.0.0",
-                "eslint-scope": "^7.2.0",
-                "eslint-visitor-keys": "^3.4.0",
-                "espree": "^9.5.1",
+                "eslint-scope": "^7.2.2",
+                "eslint-visitor-keys": "^3.4.2",
+                "espree": "^9.6.1",
                 "esquery": "^1.4.2",
                 "esutils": "^2.0.2",
                 "fast-deep-equal": "^3.1.3",
                 "file-entry-cache": "^6.0.1",
                 "find-up": "^5.0.0",
                 "glob-parent": "^6.0.2",
                 "globals": "^13.19.0",
-                "grapheme-splitter": "^1.0.4",
+                "graphemer": "^1.4.0",
                 "ignore": "^5.2.0",
-                "import-fresh": "^3.0.0",
                 "imurmurhash": "^0.1.4",
                 "is-glob": "^4.0.0",
                 "is-path-inside": "^3.0.3",
-                "js-sdsl": "^4.1.4",
                 "js-yaml": "^4.1.0",
                 "json-stable-stringify-without-jsonify": "^1.0.1",
                 "levn": "^0.4.1",
                 "lodash.merge": "^4.6.2",
                 "minimatch": "^3.1.2",
                 "natural-compare": "^1.4.0",
-                "optionator": "^0.9.1",
+                "optionator": "^0.9.3",
                 "strip-ansi": "^6.0.1",
-                "strip-json-comments": "^3.1.0",
                 "text-table": "^0.2.0"
             },
             "dev": true,
             "engines": {
                 "node": "^12.22.0 || ^14.17.0 || >=16.0.0"
             },
             "funding": {
                 "url": "https://opencollective.com/eslint"
             },
-            "integrity": "sha512-mwiok6cy7KTW7rBpo05k6+p4YVZByLNjAZ/ACB9DRCu4YDRwjXI01tWHp6KAUWelsBetTxKK/2sHB0vdS8Z2Og==",
-            "resolved": "https://registry.npmjs.org/eslint/-/eslint-8.39.0.tgz",
-            "version": "8.39.0"
+            "integrity": "sha512-cIO74PvbW0qU8e0mIvk5IV3ToWdCq5FYG6gWPHHkx6gNdjlbAYvtfHmlCMXxjcoVaIdwy/IAt3+mDkZkfvb2Dg==",
+            "resolved": "https://registry.npmjs.org/eslint/-/eslint-8.46.0.tgz",
+            "version": "8.46.0"
         },
         "node_modules/eslint-config-standard": {
             "dev": true,
+            "engines": {
+                "node": ">=12.0.0"
+            },
             "funding": [
                 {
                     "type": "github",
                     "url": "https://github.com/sponsors/feross"
                 },
                 {
                     "type": "patreon",
                     "url": "https://www.patreon.com/feross"
                 },
                 {
                     "type": "consulting",
                     "url": "https://feross.org/support"
                 }
             ],
-            "integrity": "sha512-/2ks1GKyqSOkH7JFvXJicu0iMpoojkwB+f5Du/1SC0PtBL+s8v30k9njRZ21pm2drKYm2342jFnGWzttxPmZVg==",
+            "integrity": "sha512-IwHwmaBNtDK4zDHQukFDW5u/aTb8+meQWZvNFWkiGmbWjD6bqyuSSBxxXKkCftCUzc1zwCH2m/baCNDLGmuO5Q==",
             "peerDependencies": {
                 "eslint": "^8.0.1",
                 "eslint-plugin-import": "^2.25.2",
-                "eslint-plugin-n": "^15.0.0",
+                "eslint-plugin-n": "^15.0.0 || ^16.0.0 ",
                 "eslint-plugin-promise": "^6.0.0"
             },
-            "resolved": "https://registry.npmjs.org/eslint-config-standard/-/eslint-config-standard-17.0.0.tgz",
-            "version": "17.0.0"
+            "resolved": "https://registry.npmjs.org/eslint-config-standard/-/eslint-config-standard-17.1.0.tgz",
+            "version": "17.1.0"
         },
         "node_modules/eslint-import-resolver-node": {
             "dependencies": {
                 "debug": "^3.2.7",
                 "is-core-module": "^2.11.0",
                 "resolve": "^1.22.1"
             },
@@ -3338,76 +3360,72 @@
             "dev": true,
             "engines": {
                 "node": ">=8.10.0"
             },
             "funding": {
                 "url": "https://github.com/sponsors/mysticatea"
             },
-            "integrity": "sha512-GILhQTnjYE2WorX5Jyi5i4dz5ALWxBIdQECVQavL6s7cI76IZTDWleTHkxz/QT3kvcs2QlGHvKLYsSlPOlPXnQ==",
-            "peer": true,
+            "integrity": "sha512-GUmAsJaN4Fc7Gbtl8uOBlayo2DqhwWvEzykMHSCZHU3XdJ+NSzzZcVhXh3VxX5icqQ+oQdIEawXX8xkR3mIFmQ==",
             "peerDependencies": {
                 "eslint": ">=4.19.1"
             },
-            "resolved": "https://registry.npmjs.org/eslint-plugin-es/-/eslint-plugin-es-4.1.0.tgz",
-            "version": "4.1.0"
+            "resolved": "https://registry.npmjs.org/eslint-plugin-es/-/eslint-plugin-es-3.0.1.tgz",
+            "version": "3.0.1"
         },
-        "node_modules/eslint-plugin-es/node_modules/eslint-utils": {
+        "node_modules/eslint-plugin-es-x": {
             "dependencies": {
-                "eslint-visitor-keys": "^1.1.0"
+                "@eslint-community/eslint-utils": "^4.1.2",
+                "@eslint-community/regexpp": "^4.6.0"
             },
             "dev": true,
             "engines": {
-                "node": ">=6"
+                "node": "^14.18.0 || >=16.0.0"
             },
             "funding": {
-                "url": "https://github.com/sponsors/mysticatea"
+                "url": "https://github.com/sponsors/ota-meshi"
             },
-            "integrity": "sha512-w94dQYoauyvlDc43XnGB8lU3Zt713vNChgt4EWwhXAP2XkBvndfxF0AgIqKOOasjPIPzj9JqgwkwbCYD0/V3Zg==",
+            "integrity": "sha512-9dvv5CcvNjSJPqnS5uZkqb3xmbeqRLnvXKK7iI5+oK/yTusyc46zbBZKENGsOfojm/mKfszyZb+wNqNPAPeGXA==",
             "peer": true,
-            "resolved": "https://registry.npmjs.org/eslint-utils/-/eslint-utils-2.1.0.tgz",
-            "version": "2.1.0"
-        },
-        "node_modules/eslint-plugin-es/node_modules/eslint-visitor-keys": {
-            "dev": true,
-            "engines": {
-                "node": ">=4"
+            "peerDependencies": {
+                "eslint": ">=8"
             },
-            "integrity": "sha512-6J72N8UNa462wa/KFODt/PJ3IU60SDpC3QXC1Hjc1BXXpfL2C9R5+AU7jhe0F6GREqVMh4Juu+NY7xn+6dipUQ==",
-            "peer": true,
-            "resolved": "https://registry.npmjs.org/eslint-visitor-keys/-/eslint-visitor-keys-1.3.0.tgz",
-            "version": "1.3.0"
+            "resolved": "https://registry.npmjs.org/eslint-plugin-es-x/-/eslint-plugin-es-x-7.2.0.tgz",
+            "version": "7.2.0"
         },
         "node_modules/eslint-plugin-import": {
             "dependencies": {
                 "array-includes": "^3.1.6",
+                "array.prototype.findlastindex": "^1.2.2",
                 "array.prototype.flat": "^1.3.1",
                 "array.prototype.flatmap": "^1.3.1",
                 "debug": "^3.2.7",
                 "doctrine": "^2.1.0",
                 "eslint-import-resolver-node": "^0.3.7",
-                "eslint-module-utils": "^2.7.4",
+                "eslint-module-utils": "^2.8.0",
                 "has": "^1.0.3",
-                "is-core-module": "^2.11.0",
+                "is-core-module": "^2.12.1",
                 "is-glob": "^4.0.3",
                 "minimatch": "^3.1.2",
+                "object.fromentries": "^2.0.6",
+                "object.groupby": "^1.0.0",
                 "object.values": "^1.1.6",
-                "resolve": "^1.22.1",
-                "semver": "^6.3.0",
-                "tsconfig-paths": "^3.14.1"
+                "resolve": "^1.22.3",
+                "semver": "^6.3.1",
+                "tsconfig-paths": "^3.14.2"
             },
             "dev": true,
             "engines": {
                 "node": ">=4"
             },
-            "integrity": "sha512-LmEt3GVofgiGuiE+ORpnvP+kAm3h6MLZJ4Q5HCyHADofsb4VzXFsRiWj3c0OFiV+3DWFh0qg3v9gcPlfc3zRow==",
+            "integrity": "sha512-B8s/n+ZluN7sxj9eUf7/pRFERX0r5bnFA2dCaLHy2ZeaQEAz0k+ZZkFWRFHJAqxfxQDx6KLv9LeIki7cFdwW+Q==",
             "peerDependencies": {
                 "eslint": "^2 || ^3 || ^4 || ^5 || ^6 || ^7.2.0 || ^8"
             },
-            "resolved": "https://registry.npmjs.org/eslint-plugin-import/-/eslint-plugin-import-2.27.5.tgz",
-            "version": "2.27.5"
+            "resolved": "https://registry.npmjs.org/eslint-plugin-import/-/eslint-plugin-import-2.28.0.tgz",
+            "version": "2.28.0"
         },
         "node_modules/eslint-plugin-import/node_modules/debug": {
             "dependencies": {
                 "ms": "^2.1.1"
             },
             "dev": true,
             "integrity": "sha512-CFjzYYAi4ThfiQvizrFQevTTXHtnCqWfe7x1AhgEscTz6ZbLbfoLRLPugTQyBth6f8ZERVUSyWHFD/7Wu4t1XQ==",
@@ -3427,43 +3445,43 @@
             "version": "2.1.0"
         },
         "node_modules/eslint-plugin-import/node_modules/semver": {
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
         "node_modules/eslint-plugin-n": {
             "dependencies": {
+                "@eslint-community/eslint-utils": "^4.4.0",
                 "builtins": "^5.0.1",
-                "eslint-plugin-es": "^4.1.0",
-                "eslint-utils": "^3.0.0",
-                "ignore": "^5.1.1",
-                "is-core-module": "^2.11.0",
+                "eslint-plugin-es-x": "^7.1.0",
+                "ignore": "^5.2.4",
+                "is-core-module": "^2.12.1",
                 "minimatch": "^3.1.2",
-                "resolve": "^1.22.1",
-                "semver": "^7.3.8"
+                "resolve": "^1.22.2",
+                "semver": "^7.5.3"
             },
             "dev": true,
             "engines": {
-                "node": ">=12.22.0"
+                "node": ">=16.0.0"
             },
             "funding": {
                 "url": "https://github.com/sponsors/mysticatea"
             },
-            "integrity": "sha512-jDex9s7D/Qial8AGVIHq4W7NswpUD5DPDL2RH8Lzd9EloWUuvUkHfv4FRLMipH5q2UtyurorBkPeNi1wVWNh3Q==",
+            "integrity": "sha512-CDmHegJN0OF3L5cz5tATH84RPQm9kG+Yx39wIqIwPR2C0uhBGMWfbbOtetR83PQjjidA5aXMu+LEFw1jaSwvTA==",
             "peer": true,
             "peerDependencies": {
                 "eslint": ">=7.0.0"
             },
-            "resolved": "https://registry.npmjs.org/eslint-plugin-n/-/eslint-plugin-n-15.7.0.tgz",
-            "version": "15.7.0"
+            "resolved": "https://registry.npmjs.org/eslint-plugin-n/-/eslint-plugin-n-16.0.1.tgz",
+            "version": "16.0.1"
         },
         "node_modules/eslint-plugin-node": {
             "dependencies": {
                 "eslint-plugin-es": "^3.0.0",
                 "eslint-utils": "^2.0.0",
                 "ignore": "^5.1.1",
                 "minimatch": "^3.0.4",
@@ -3477,65 +3495,22 @@
             "integrity": "sha512-oUwtPJ1W0SKD0Tr+wqu92c5xuCeQqB3hSCHasn/ZgjFdA9iDGNkNf2Zi9ztY7X+hNuMib23LNGRm6+uN+KLE3g==",
             "peerDependencies": {
                 "eslint": ">=5.16.0"
             },
             "resolved": "https://registry.npmjs.org/eslint-plugin-node/-/eslint-plugin-node-11.1.0.tgz",
             "version": "11.1.0"
         },
-        "node_modules/eslint-plugin-node/node_modules/eslint-plugin-es": {
-            "dependencies": {
-                "eslint-utils": "^2.0.0",
-                "regexpp": "^3.0.0"
-            },
-            "dev": true,
-            "engines": {
-                "node": ">=8.10.0"
-            },
-            "funding": {
-                "url": "https://github.com/sponsors/mysticatea"
-            },
-            "integrity": "sha512-GUmAsJaN4Fc7Gbtl8uOBlayo2DqhwWvEzykMHSCZHU3XdJ+NSzzZcVhXh3VxX5icqQ+oQdIEawXX8xkR3mIFmQ==",
-            "peerDependencies": {
-                "eslint": ">=4.19.1"
-            },
-            "resolved": "https://registry.npmjs.org/eslint-plugin-es/-/eslint-plugin-es-3.0.1.tgz",
-            "version": "3.0.1"
-        },
-        "node_modules/eslint-plugin-node/node_modules/eslint-utils": {
-            "dependencies": {
-                "eslint-visitor-keys": "^1.1.0"
-            },
-            "dev": true,
-            "engines": {
-                "node": ">=6"
-            },
-            "funding": {
-                "url": "https://github.com/sponsors/mysticatea"
-            },
-            "integrity": "sha512-w94dQYoauyvlDc43XnGB8lU3Zt713vNChgt4EWwhXAP2XkBvndfxF0AgIqKOOasjPIPzj9JqgwkwbCYD0/V3Zg==",
-            "resolved": "https://registry.npmjs.org/eslint-utils/-/eslint-utils-2.1.0.tgz",
-            "version": "2.1.0"
-        },
-        "node_modules/eslint-plugin-node/node_modules/eslint-visitor-keys": {
-            "dev": true,
-            "engines": {
-                "node": ">=4"
-            },
-            "integrity": "sha512-6J72N8UNa462wa/KFODt/PJ3IU60SDpC3QXC1Hjc1BXXpfL2C9R5+AU7jhe0F6GREqVMh4Juu+NY7xn+6dipUQ==",
-            "resolved": "https://registry.npmjs.org/eslint-visitor-keys/-/eslint-visitor-keys-1.3.0.tgz",
-            "version": "1.3.0"
-        },
         "node_modules/eslint-plugin-node/node_modules/semver": {
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
         "node_modules/eslint-plugin-promise": {
             "dev": true,
             "engines": {
                 "node": "^12.22.0 || ^14.17.0 || >=16.0.0"
             },
             "integrity": "sha512-tjqWDwVZQo7UIPMeDReOpUgHCmCiH+ePnVT+5zVapL0uuHnegBUs2smM13CzOs2Xb5+MHMRFTs9v24yjba4Oig==",
@@ -3553,75 +3528,70 @@
             "dev": true,
             "engines": {
                 "node": "^12.22.0 || ^14.17.0 || >=16.0.0"
             },
             "funding": {
                 "url": "https://opencollective.com/eslint"
             },
-            "integrity": "sha512-DYj5deGlHBfMt15J7rdtyKNq/Nqlv5KfU4iodrQ019XESsRnwXH9KAE0y3cwtUHDo2ob7CypAnCqefh6vioWRw==",
-            "resolved": "https://registry.npmjs.org/eslint-scope/-/eslint-scope-7.2.0.tgz",
-            "version": "7.2.0"
+            "integrity": "sha512-dOt21O7lTMhDM+X9mB4GX+DZrZtCUJPL/wlcTqxyrx5IvO0IYtILdtrQGQp+8n5S0gwSVmOf9NQrjMOgfQZlIg==",
+            "resolved": "https://registry.npmjs.org/eslint-scope/-/eslint-scope-7.2.2.tgz",
+            "version": "7.2.2"
         },
         "node_modules/eslint-utils": {
             "dependencies": {
-                "eslint-visitor-keys": "^2.0.0"
+                "eslint-visitor-keys": "^1.1.0"
             },
             "dev": true,
             "engines": {
-                "node": "^10.0.0 || ^12.0.0 || >= 14.0.0"
+                "node": ">=6"
             },
             "funding": {
                 "url": "https://github.com/sponsors/mysticatea"
             },
-            "integrity": "sha512-uuQC43IGctw68pJA1RgbQS8/NP7rch6Cwd4j3ZBtgo4/8Flj4eGE7ZYSZRN3iq5pVUv6GPdW5Z1RFleo84uLDA==",
-            "peer": true,
-            "peerDependencies": {
-                "eslint": ">=5"
-            },
-            "resolved": "https://registry.npmjs.org/eslint-utils/-/eslint-utils-3.0.0.tgz",
-            "version": "3.0.0"
+            "integrity": "sha512-w94dQYoauyvlDc43XnGB8lU3Zt713vNChgt4EWwhXAP2XkBvndfxF0AgIqKOOasjPIPzj9JqgwkwbCYD0/V3Zg==",
+            "resolved": "https://registry.npmjs.org/eslint-utils/-/eslint-utils-2.1.0.tgz",
+            "version": "2.1.0"
         },
         "node_modules/eslint-utils/node_modules/eslint-visitor-keys": {
             "dev": true,
             "engines": {
-                "node": ">=10"
+                "node": ">=4"
             },
-            "integrity": "sha512-0rSmRBzXgDzIsD6mGdJgevzgezI534Cer5L/vyMX0kHzT/jiB43jRhd9YUlMGYLQy2zprNmoT8qasCGtY+QaKw==",
-            "peer": true,
-            "resolved": "https://registry.npmjs.org/eslint-visitor-keys/-/eslint-visitor-keys-2.1.0.tgz",
-            "version": "2.1.0"
+            "integrity": "sha512-6J72N8UNa462wa/KFODt/PJ3IU60SDpC3QXC1Hjc1BXXpfL2C9R5+AU7jhe0F6GREqVMh4Juu+NY7xn+6dipUQ==",
+            "resolved": "https://registry.npmjs.org/eslint-visitor-keys/-/eslint-visitor-keys-1.3.0.tgz",
+            "version": "1.3.0"
         },
         "node_modules/eslint-visitor-keys": {
             "dev": true,
             "engines": {
                 "node": "^12.22.0 || ^14.17.0 || >=16.0.0"
             },
             "funding": {
                 "url": "https://opencollective.com/eslint"
             },
-            "integrity": "sha512-HPpKPUBQcAsZOsHAFwTtIKcYlCje62XB7SEAcxjtmW6TD1WVpkS6i6/hOVtTZIl4zGj/mBqpFVGvaDneik+VoQ==",
-            "resolved": "https://registry.npmjs.org/eslint-visitor-keys/-/eslint-visitor-keys-3.4.0.tgz",
-            "version": "3.4.0"
+            "integrity": "sha512-8drBzUEyZ2llkpCA67iYrgEssKDUu68V8ChqqOfFupIaG/LCVPUT+CoGJpT77zJprs4T/W7p07LP7zAIMuweVw==",
+            "resolved": "https://registry.npmjs.org/eslint-visitor-keys/-/eslint-visitor-keys-3.4.2.tgz",
+            "version": "3.4.2"
         },
         "node_modules/espree": {
             "dependencies": {
-                "acorn": "^8.8.0",
+                "acorn": "^8.9.0",
                 "acorn-jsx": "^5.3.2",
-                "eslint-visitor-keys": "^3.4.0"
+                "eslint-visitor-keys": "^3.4.1"
             },
             "dev": true,
             "engines": {
                 "node": "^12.22.0 || ^14.17.0 || >=16.0.0"
             },
             "funding": {
                 "url": "https://opencollective.com/eslint"
             },
-            "integrity": "sha512-5yxtHSZXRSW5pvv3hAlXM5+/Oswi1AUFqBmbibKb5s6bp3rGIDkyXU6xCoyuuLhijr4SFwPrXRoZjz0AZDN9tg==",
-            "resolved": "https://registry.npmjs.org/espree/-/espree-9.5.1.tgz",
-            "version": "9.5.1"
+            "integrity": "sha512-oruZaFkjorTpF32kDSI5/75ViwGeZginGGy2NoOSg3Q9bnwlnmDm4HLnkl0RE3n+njDXR037aY1+x58Z/zFdwQ==",
+            "resolved": "https://registry.npmjs.org/espree/-/espree-9.6.1.tgz",
+            "version": "9.6.1"
         },
         "node_modules/esprima": {
             "bin": {
                 "esparse": "bin/esparse.js",
                 "esvalidate": "bin/esvalidate.js"
             },
             "engines": {
@@ -3830,19 +3800,14 @@
             "dependencies": {
                 "dtype": "^2.0.0"
             },
             "integrity": "sha512-BvCBFK2NZqerFTdMDgqfHBwxYWnxeCkwONsw6PvBMcUXqo8U/KDWwmXhqx1x2kLIg7DqIsJfOaJFOmlua3Lxuw==",
             "resolved": "https://registry.npmjs.org/flatten-vertex-data/-/flatten-vertex-data-1.0.2.tgz",
             "version": "1.0.2"
         },
-        "node_modules/flip-pixels": {
-            "integrity": "sha512-oXbJGbjDnfJRWPC7Va38EFhd+A8JWE5/hCiKcK8qjCdbLj9DTpsq6MEudwpRTH+V4qq+Jw7d3pUgQdSr3x3mTA==",
-            "resolved": "https://registry.npmjs.org/flip-pixels/-/flip-pixels-1.0.2.tgz",
-            "version": "1.0.2"
-        },
         "node_modules/font-atlas": {
             "dependencies": {
                 "css-font": "^1.0.0"
             },
             "integrity": "sha512-kP3AmvX+HJpW4w3d+PiPR2X6E1yvsBXt2yhuCw+yReO9F1WYhvZwx3c95DGZGwg9xYzDGrgJYa885xmVA+28Cg==",
             "resolved": "https://registry.npmjs.org/font-atlas/-/font-atlas-2.1.0.tgz",
             "version": "2.1.0"
@@ -4024,23 +3989,24 @@
             "resolved": "https://registry.npmjs.org/get-canvas-context/-/get-canvas-context-1.0.2.tgz",
             "version": "1.0.2"
         },
         "node_modules/get-intrinsic": {
             "dependencies": {
                 "function-bind": "^1.1.1",
                 "has": "^1.0.3",
+                "has-proto": "^1.0.1",
                 "has-symbols": "^1.0.3"
             },
             "dev": true,
             "funding": {
                 "url": "https://github.com/sponsors/ljharb"
             },
-            "integrity": "sha512-L049y6nFOuom5wGyRc3/gdTLO94dySVKRACj1RmJZBQXlbTMhtNIgkWkUHq+jYmZvKf14EW1EoJnnjbmoHij0Q==",
-            "resolved": "https://registry.npmjs.org/get-intrinsic/-/get-intrinsic-1.2.0.tgz",
-            "version": "1.2.0"
+            "integrity": "sha512-2DcsyfABl+gVHEfCOaTrWgyt+tb6MSEGmKq+kI5HwLbIYgjgmMcV8KQ41uaKz1xxUcn9tJtgFbQUEVcEbd0FYw==",
+            "resolved": "https://registry.npmjs.org/get-intrinsic/-/get-intrinsic-1.2.1.tgz",
+            "version": "1.2.1"
         },
         "node_modules/get-stdin": {
             "dev": true,
             "engines": {
                 "node": ">=0.10.0"
             },
             "integrity": "sha512-F5aQMywwJ2n85s4hJPTT9RPxGmubonuB10MNYo17/xph174n2MIR33HRguhzVag10O/npM7SPk73LMZNP+FaWw==",
@@ -4430,19 +4396,19 @@
             "version": "1.0.1"
         },
         "node_modules/graceful-fs": {
             "integrity": "sha512-RbJ5/jmFcNNCcDV5o9eTnBLJ/HszWV0P73bc+Ff4nS/rJj+YaS6IGyiOL0VoBYX+l1Wrl3k63h/KrH+nhJ0XvQ==",
             "resolved": "https://registry.npmjs.org/graceful-fs/-/graceful-fs-4.2.11.tgz",
             "version": "4.2.11"
         },
-        "node_modules/grapheme-splitter": {
+        "node_modules/graphemer": {
             "dev": true,
-            "integrity": "sha512-bzh50DW9kTPM00T8y4o8vQg89Di9oLJVLW/KaOGIXJWP/iqCN6WKYkbNOF04vFLJhwcpYUh9ydh/+5vpOqV4YQ==",
-            "resolved": "https://registry.npmjs.org/grapheme-splitter/-/grapheme-splitter-1.0.4.tgz",
-            "version": "1.0.4"
+            "integrity": "sha512-EtKwoO6kxCL9WO5xipiHTZlSzBm7WLT627TqC/uVRd0HKmq8NXyebnNYxDoBi7wt8eTWrUrKXCOVaFq9x1kgag==",
+            "resolved": "https://registry.npmjs.org/graphemer/-/graphemer-1.4.0.tgz",
+            "version": "1.4.0"
         },
         "node_modules/grid-index": {
             "integrity": "sha512-HZRwumpOGUrHyxO5bqKZL0B0GlUpwtCAzZ42sgxUPniu33R1LSFH5yrIcBCHjkctCAh3mtWKcKd9J4vDDdeVHA==",
             "resolved": "https://registry.npmjs.org/grid-index/-/grid-index-1.1.0.tgz",
             "version": "1.1.0"
         },
         "node_modules/hard-rejection": {
@@ -4656,20 +4622,20 @@
             "engines": {
                 "node": ">=10.13.0"
             },
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/html-webpack-plugin"
             },
-            "integrity": "sha512-cTUzZ1+NqjGEKjmVgZKLMdiFg3m9MdRXkZW2OEe69WYVi5ONLMmlnSZdXzGGMOq0C8jGDrL6EWyEDDUioHO/pA==",
+            "integrity": "sha512-6YrDKTuqaP/TquFH7h4srYWsZx+x6k6+FbsTm0ziCwGHDP78Unr1r9F/H4+sGmMbX08GQcJ+K64x55b+7VM/jg==",
             "peerDependencies": {
                 "webpack": "^5.20.0"
             },
-            "resolved": "https://registry.npmjs.org/html-webpack-plugin/-/html-webpack-plugin-5.5.1.tgz",
-            "version": "5.5.1"
+            "resolved": "https://registry.npmjs.org/html-webpack-plugin/-/html-webpack-plugin-5.5.3.tgz",
+            "version": "5.5.3"
         },
         "node_modules/html-webpack-plugin/node_modules/commander": {
             "dev": true,
             "engines": {
                 "node": ">= 12"
             },
             "integrity": "sha512-OkTL9umf+He2DZkUq8f8J9of7yL6RJKI24dVITBmNfZBmri9zYZQrKkuXiKhyfPSu8tUhnVBB1iKXevvnlR4Ww==",
@@ -4814,24 +4780,14 @@
             "engines": {
                 "node": ">= 4"
             },
             "integrity": "sha512-MAb38BcSbH0eHNBxn7ql2NH/kX33OkB3lZ1BNdh7ENeRChHTYsTvWrMubiIAMNS2llXEEgZ1MUOBtXChP3kaFQ==",
             "resolved": "https://registry.npmjs.org/ignore/-/ignore-5.2.4.tgz",
             "version": "5.2.4"
         },
-        "node_modules/image-palette": {
-            "dependencies": {
-                "color-id": "^1.1.0",
-                "pxls": "^2.0.0",
-                "quantize": "^1.0.2"
-            },
-            "integrity": "sha512-3ImSEWD26+xuQFdP0RWR4WSXadZwvgrFhjGNpMEapTG1tf2XrBFS2dlKK5hNgH4UIaSQlSUFRn1NeA+zULIWbQ==",
-            "resolved": "https://registry.npmjs.org/image-palette/-/image-palette-2.1.0.tgz",
-            "version": "2.1.0"
-        },
         "node_modules/import-fresh": {
             "dependencies": {
                 "parent-module": "^1.0.0",
                 "resolve-from": "^4.0.0"
             },
             "dev": true,
             "engines": {
@@ -4955,42 +4911,26 @@
         },
         "node_modules/is-arrayish": {
             "dev": true,
             "integrity": "sha512-zz06S8t0ozoDXMG+ube26zeCTNXcKIPJZJi8hBrF4idCLms4CG9QtK7qBl1boi5ODzFpjswb5JPmHCbMpjaYzg==",
             "resolved": "https://registry.npmjs.org/is-arrayish/-/is-arrayish-0.2.1.tgz",
             "version": "0.2.1"
         },
-        "node_modules/is-base64": {
-            "integrity": "sha512-WRRyllsGXJM7ZN7gPTCCQ/6wNPTRDwiWdPK66l5sJzcU/oOzcIcRRf0Rux8bkpox/1yjt0F6VJRsQOIG2qz5sg==",
-            "resolved": "https://registry.npmjs.org/is-base64/-/is-base64-0.1.0.tgz",
-            "version": "0.1.0"
-        },
         "node_modules/is-bigint": {
             "dependencies": {
                 "has-bigints": "^1.0.1"
             },
             "dev": true,
             "funding": {
                 "url": "https://github.com/sponsors/ljharb"
             },
             "integrity": "sha512-zB9CruMamjym81i2JZ3UMn54PKGsQzsJeo6xvN3HJJ4CAsQNB6iRutp2To77OfCNuoxspsIhzaPoO1zyCEhFOg==",
             "resolved": "https://registry.npmjs.org/is-bigint/-/is-bigint-1.0.4.tgz",
             "version": "1.0.4"
         },
-        "node_modules/is-blob": {
-            "engines": {
-                "node": ">=6"
-            },
-            "funding": {
-                "url": "https://github.com/sponsors/sindresorhus"
-            },
-            "integrity": "sha512-SZ/fTft5eUhQM6oF/ZaASFDEdbFVe89Imltn9uZr03wdKMcWNVYSMjQPFtg05QuNkt5l5c135ElvXEQG0rk4tw==",
-            "resolved": "https://registry.npmjs.org/is-blob/-/is-blob-2.1.0.tgz",
-            "version": "2.1.0"
-        },
         "node_modules/is-boolean-object": {
             "dependencies": {
                 "call-bind": "^1.0.2",
                 "has-tostringtag": "^1.0.0"
             },
             "dev": true,
             "engines": {
@@ -5004,36 +4944,14 @@
             "version": "1.1.2"
         },
         "node_modules/is-browser": {
             "integrity": "sha512-F5rTJxDQ2sW81fcfOR1GnCXT6sVJC104fCyfj+mjpwNEwaPYSn5fte5jiHmBg3DHsIoL/l8Kvw5VN5SsTRcRFQ==",
             "resolved": "https://registry.npmjs.org/is-browser/-/is-browser-2.1.0.tgz",
             "version": "2.1.0"
         },
-        "node_modules/is-buffer": {
-            "engines": {
-                "node": ">=4"
-            },
-            "funding": [
-                {
-                    "type": "github",
-                    "url": "https://github.com/sponsors/feross"
-                },
-                {
-                    "type": "patreon",
-                    "url": "https://www.patreon.com/feross"
-                },
-                {
-                    "type": "consulting",
-                    "url": "https://feross.org/support"
-                }
-            ],
-            "integrity": "sha512-i2R6zNFDwgEHJyQUtJEk0XFi1i0dPFn/oqjK3/vPCcDeJvW5NQ83V8QbicfF1SupOaB0h8ntgBC2YiE7dfyctQ==",
-            "resolved": "https://registry.npmjs.org/is-buffer/-/is-buffer-2.0.5.tgz",
-            "version": "2.0.5"
-        },
         "node_modules/is-callable": {
             "dev": true,
             "engines": {
                 "node": ">= 0.4"
             },
             "funding": {
                 "url": "https://github.com/sponsors/ljharb"
@@ -5045,17 +4963,17 @@
         "node_modules/is-core-module": {
             "dependencies": {
                 "has": "^1.0.3"
             },
             "funding": {
                 "url": "https://github.com/sponsors/ljharb"
             },
-            "integrity": "sha512-RECHCBCd/viahWmwj6enj19sKbHfJrddi/6cBDsNTKbNq0f7VeaUkBo60BqzvPqo/W54ChS62Z5qyun7cfOMqQ==",
-            "resolved": "https://registry.npmjs.org/is-core-module/-/is-core-module-2.12.0.tgz",
-            "version": "2.12.0"
+            "integrity": "sha512-Q4ZuBAe2FUsKtyQJoQHlvP8OvBERxO3jEmy1I7hcRXcJBGGHFh/aJBswbXuS9sgrDH2QUO8ilkwNPHvHMd8clg==",
+            "resolved": "https://registry.npmjs.org/is-core-module/-/is-core-module-2.12.1.tgz",
+            "version": "2.12.1"
         },
         "node_modules/is-date-object": {
             "dependencies": {
                 "has-tostringtag": "^1.0.0"
             },
             "dev": true,
             "engines": {
@@ -5092,19 +5010,14 @@
             "engines": {
                 "node": ">=0.10.0"
             },
             "integrity": "sha512-6Q9ITjvWIm0Xdqv+5U12wgOKEM2KoBw4Y926m0OFkvlCxnbG94HKAsVz8w3fWcfAS5YA2fJORXX1dLrkprCCxA==",
             "resolved": "https://registry.npmjs.org/is-firefox/-/is-firefox-1.0.3.tgz",
             "version": "1.0.3"
         },
-        "node_modules/is-float-array": {
-            "integrity": "sha512-4ew1Sx6B6kEAl3T3NOM0yB94J3NZnBdNt4paw0e8nY73yHHTeTEhyQ3Lj7EQEnv5LD+GxNTaT4L46jcKjjpLiQ==",
-            "resolved": "https://registry.npmjs.org/is-float-array/-/is-float-array-1.0.0.tgz",
-            "version": "1.0.0"
-        },
         "node_modules/is-fullwidth-code-point": {
             "dev": true,
             "engines": {
                 "node": ">=8"
             },
             "integrity": "sha512-zymm5+u+sCsSWyD9qNaejV3DFvhCKclKdizYaJUuHA83RLjb7nSuGnddCHGv0hk+KY7BMAlsWeK4Ueg6EV6XQg==",
             "resolved": "https://registry.npmjs.org/is-fullwidth-code-point/-/is-fullwidth-code-point-3.0.0.tgz",
@@ -5271,30 +5184,26 @@
             },
             "integrity": "sha512-C/CPBqKWnvdcxqIARxyOh4v1UUEOCHpgDa0WYgpKDFMszcrPcffg5uhwSgPCLD2WWxmq6isisz87tzT01tuGhg==",
             "resolved": "https://registry.npmjs.org/is-symbol/-/is-symbol-1.0.4.tgz",
             "version": "1.0.4"
         },
         "node_modules/is-typed-array": {
             "dependencies": {
-                "available-typed-arrays": "^1.0.5",
-                "call-bind": "^1.0.2",
-                "for-each": "^0.3.3",
-                "gopd": "^1.0.1",
-                "has-tostringtag": "^1.0.0"
+                "which-typed-array": "^1.1.11"
             },
             "dev": true,
             "engines": {
                 "node": ">= 0.4"
             },
             "funding": {
                 "url": "https://github.com/sponsors/ljharb"
             },
-            "integrity": "sha512-PJqgEHiWZvMpaFZ3uTc8kHPM4+4ADTlDniuQL7cU/UDA0Ql7F70yGfHph3cLNe+c9toaigv+DFzTJKhc2CtO6A==",
-            "resolved": "https://registry.npmjs.org/is-typed-array/-/is-typed-array-1.1.10.tgz",
-            "version": "1.1.10"
+            "integrity": "sha512-Z14TF2JNG8Lss5/HMqt0//T9JeHXttXy5pH/DBU4vi98ozO2btxzq9MwYDZYnKwU8nRsz/+GVFVRDq3DkVuSPg==",
+            "resolved": "https://registry.npmjs.org/is-typed-array/-/is-typed-array-1.1.12.tgz",
+            "version": "1.1.12"
         },
         "node_modules/is-weakref": {
             "dependencies": {
                 "call-bind": "^1.0.2"
             },
             "dev": true,
             "funding": {
@@ -5354,22 +5263,22 @@
             "version": "8.1.1"
         },
         "node_modules/jiti": {
             "bin": {
                 "jiti": "bin/jiti.js"
             },
             "dev": true,
-            "integrity": "sha512-QAdOptna2NYiSSpv0O/BwoHBSmz4YhpzJHyi+fnMRTXFjp7B8i/YG5Z8IfusxB1ufjcD2Sre1F3R+nX3fvy7gg==",
-            "resolved": "https://registry.npmjs.org/jiti/-/jiti-1.18.2.tgz",
-            "version": "1.18.2"
+            "integrity": "sha512-oVhqoRDaBXf7sjkll95LHVS6Myyyb1zaunVwk4Z0+WPSW4gjS0pl01zYKHScTuyEhQsFxV5L4DR5r+YqSyqyyg==",
+            "resolved": "https://registry.npmjs.org/jiti/-/jiti-1.19.1.tgz",
+            "version": "1.19.1"
         },
         "node_modules/jquery": {
-            "integrity": "sha512-v28EW9DWDFpzcD9O5iyJXg3R3+q+mET5JhnjJzQUZMHOv67bpSIHq81GEYpPNZHG+XXHsfSme3nxp/hndKEcsQ==",
-            "resolved": "https://registry.npmjs.org/jquery/-/jquery-3.6.4.tgz",
-            "version": "3.6.4"
+            "integrity": "sha512-umpJ0/k8X0MvD1ds0P9SfowREz2LenHsQaxSohMZ5OMNEU2r0tf8pdeEFTHMFxWVxKNyU9rTtK3CWzUCTKJUeQ==",
+            "resolved": "https://registry.npmjs.org/jquery/-/jquery-3.7.0.tgz",
+            "version": "3.7.0"
         },
         "node_modules/jquery-ui": {
             "dependencies": {
                 "jquery": ">=1.8.0 <4.0.0"
             },
             "integrity": "sha512-wBZPnqWs5GaYJmo1Jj0k/mrSkzdQzKDwhXNtHKcBdAcKVxMM3KNYFq+iJ2i1rwiG53Z8M4mTn3Qxrm17uH1D4Q==",
             "resolved": "https://registry.npmjs.org/jquery-ui/-/jquery-ui-1.13.2.tgz",
@@ -5377,24 +5286,14 @@
         },
         "node_modules/js-base64": {
             "dev": true,
             "integrity": "sha512-pZe//GGmwJndub7ZghVHz7vjb2LgC1m8B07Au3eYqeqv9emhESByMXxaEgkUkEqJe87oBbSniGYoQNIBklc7IQ==",
             "resolved": "https://registry.npmjs.org/js-base64/-/js-base64-2.6.4.tgz",
             "version": "2.6.4"
         },
-        "node_modules/js-sdsl": {
-            "dev": true,
-            "funding": {
-                "type": "opencollective",
-                "url": "https://opencollective.com/js-sdsl"
-            },
-            "integrity": "sha512-FfVSdx6pJ41Oa+CF7RDaFmTnCaFhua+SNYQX74riGOpl96x+2jQCqEfQ2bnXu/5DPCqlRuiqyvTJM0Qjz26IVg==",
-            "resolved": "https://registry.npmjs.org/js-sdsl/-/js-sdsl-4.4.0.tgz",
-            "version": "4.4.0"
-        },
         "node_modules/js-tokens": {
             "dev": true,
             "integrity": "sha512-RdJUflcE3cUzKiMqQgsCu06FPu9UdIJO0beYbPhHN4k6apgJtifcoCtT9bcxOpYBtpD2kCM6Sbzg4CausW/PKQ==",
             "resolved": "https://registry.npmjs.org/js-tokens/-/js-tokens-4.0.0.tgz",
             "version": "4.0.0"
         },
         "node_modules/js-yaml": {
@@ -5449,23 +5348,14 @@
             "engines": {
                 "node": ">=0.10.0"
             },
             "integrity": "sha512-dcS1ul+9tmeD95T+x28/ehLgd9mENa3LsvDTtzm3vyBEO7RPptvAD+t44WVXaUjTBRcrpFeFlC8WCruUR456hw==",
             "resolved": "https://registry.npmjs.org/kind-of/-/kind-of-6.0.3.tgz",
             "version": "6.0.3"
         },
-        "node_modules/klona": {
-            "dev": true,
-            "engines": {
-                "node": ">= 8"
-            },
-            "integrity": "sha512-dhG34DXATL5hSxJbIexCft8FChFXtmskoZYnoPWjXQuebWYCNkVeV3KkGegCK9CP1oswI/vQibS2GY7Em/sJJA==",
-            "resolved": "https://registry.npmjs.org/klona/-/klona-2.0.6.tgz",
-            "version": "2.0.6"
-        },
         "node_modules/lazystream": {
             "dependencies": {
                 "readable-stream": "^2.0.5"
             },
             "dev": true,
             "engines": {
                 "node": ">= 0.6.3"
@@ -5804,20 +5694,20 @@
             "engines": {
                 "node": ">= 12.13.0"
             },
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/webpack"
             },
-            "integrity": "sha512-9HaR++0mlgom81s95vvNjxkg52n2b5s//3ZTI1EtzFb98awsLSivs2LMsVqnQ3ay0PVhqWcGNyDaTE961FOcjQ==",
+            "integrity": "sha512-Qk7HcgaPkGG6eD77mLvZS1nmxlao3j+9PkrT9Uc7HAE1id3F41+DdBRYRYkbyfNRGzm8/YWtzhw7nVPmwhqTQw==",
             "peerDependencies": {
                 "webpack": "^5.0.0"
             },
-            "resolved": "https://registry.npmjs.org/mini-css-extract-plugin/-/mini-css-extract-plugin-2.7.5.tgz",
-            "version": "2.7.5"
+            "resolved": "https://registry.npmjs.org/mini-css-extract-plugin/-/mini-css-extract-plugin-2.7.6.tgz",
+            "version": "2.7.6"
         },
         "node_modules/mini-css-extract-plugin/node_modules/ajv": {
             "dependencies": {
                 "fast-deep-equal": "^3.1.1",
                 "json-schema-traverse": "^1.0.0",
                 "require-from-string": "^2.0.2",
                 "uri-js": "^4.2.2"
@@ -5860,17 +5750,17 @@
             "engines": {
                 "node": ">= 12.13.0"
             },
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/webpack"
             },
-            "integrity": "sha512-lELhBAAly9NowEsX0yZBlw9ahZG+sK/1RJ21EpzdYHKEs13Vku3LJ+MIPhh4sMs0oCCeufZQEQbMekiA4vuVIQ==",
-            "resolved": "https://registry.npmjs.org/schema-utils/-/schema-utils-4.0.1.tgz",
-            "version": "4.0.1"
+            "integrity": "sha512-L0jRsrPpjdckP3oPug3/VxNKt2trR8TcabrM6FOAAlvC/9Phcmm+cuAgTlxBqdBR1WJx7Naj9WHw+aOmheSVbw==",
+            "resolved": "https://registry.npmjs.org/schema-utils/-/schema-utils-4.2.0.tgz",
+            "version": "4.2.0"
         },
         "node_modules/minimatch": {
             "dependencies": {
                 "brace-expansion": "^1.1.7"
             },
             "dev": true,
             "engines": {
@@ -6357,17 +6247,17 @@
             "dev": true,
             "integrity": "sha512-zoWr9ObaxALD3DOPfjPSqxt4fnZiWblxHIgeWqW8x7UqDzEtHEQLzji2cuJYQFCU6KmoJikOYAZlrTHHebjx2w==",
             "resolved": "https://registry.npmjs.org/unique-slug/-/unique-slug-2.0.2.tgz",
             "version": "2.0.2"
         },
         "node_modules/node-releases": {
             "dev": true,
-            "integrity": "sha512-5GFldHPXVG/YZmFzJvKK2zDSzPKhEp0+ZR5SVaoSag9fsL5YgHbUHDfnG5494ISANDcK4KwPXAx2xqVEydmd7w==",
-            "resolved": "https://registry.npmjs.org/node-releases/-/node-releases-2.0.10.tgz",
-            "version": "2.0.10"
+            "integrity": "sha512-uYr7J37ae/ORWdZeQ1xxMJe3NtdmqMC/JZK+geofDrkLUApKRHPd18/TxtBOJ4A0/+uUIliorNrfYV6s1b02eQ==",
+            "resolved": "https://registry.npmjs.org/node-releases/-/node-releases-2.0.13.tgz",
+            "version": "2.0.13"
         },
         "node_modules/node-sass": {
             "bin": {
                 "node-sass": "bin/node-sass"
             },
             "dependencies": {
                 "async-foreach": "^0.1.3",
@@ -6499,14 +6389,15 @@
                 "url": "https://github.com/sponsors/ljharb"
             },
             "integrity": "sha512-geUvdk7c+eizMNUDkRpW1wJwgfOiOeHbxBR/hLXK1aT6zmVSO0jsQcs7fj6MGw89jC/cjGfLcNOrtMYtGqm81g==",
             "resolved": "https://registry.npmjs.org/object-inspect/-/object-inspect-1.12.3.tgz",
             "version": "1.12.3"
         },
         "node_modules/object-keys": {
+            "dev": true,
             "engines": {
                 "node": ">= 0.4"
             },
             "integrity": "sha512-NuAESUOUMrlIXOfHKzD6bpPu3tYt3xvjNdRIQ+FeT0lNb4K8WR70CaDxhuNguS2XG+GjkyMwOzsN5ZktImfhLA==",
             "resolved": "https://registry.npmjs.org/object-keys/-/object-keys-1.1.1.tgz",
             "version": "1.1.1"
         },
@@ -6524,14 +6415,43 @@
             "funding": {
                 "url": "https://github.com/sponsors/ljharb"
             },
             "integrity": "sha512-1mxKf0e58bvyjSCtKYY4sRe9itRk3PJpquJOjeIkz885CczcI4IvJJDLPS72oowuSh+pBxUFROpX+TU++hxhZQ==",
             "resolved": "https://registry.npmjs.org/object.assign/-/object.assign-4.1.4.tgz",
             "version": "4.1.4"
         },
+        "node_modules/object.fromentries": {
+            "dependencies": {
+                "call-bind": "^1.0.2",
+                "define-properties": "^1.1.4",
+                "es-abstract": "^1.20.4"
+            },
+            "dev": true,
+            "engines": {
+                "node": ">= 0.4"
+            },
+            "funding": {
+                "url": "https://github.com/sponsors/ljharb"
+            },
+            "integrity": "sha512-VciD13dswC4j1Xt5394WR4MzmAQmlgN72phd/riNp9vtD7tp4QQWJ0R4wvclXcafgcYK8veHRed2W6XeGBvcfg==",
+            "resolved": "https://registry.npmjs.org/object.fromentries/-/object.fromentries-2.0.6.tgz",
+            "version": "2.0.6"
+        },
+        "node_modules/object.groupby": {
+            "dependencies": {
+                "call-bind": "^1.0.2",
+                "define-properties": "^1.2.0",
+                "es-abstract": "^1.21.2",
+                "get-intrinsic": "^1.2.1"
+            },
+            "dev": true,
+            "integrity": "sha512-70MWG6NfRH9GnbZOikuhPPYzpUpof9iW2J9E4dW7FXTqPNb6rllE6u39SKwwiNh8lCwX3DDb5OgcKGiEBrTTyw==",
+            "resolved": "https://registry.npmjs.org/object.groupby/-/object.groupby-1.0.0.tgz",
+            "version": "1.0.0"
+        },
         "node_modules/object.values": {
             "dependencies": {
                 "call-bind": "^1.0.2",
                 "define-properties": "^1.1.4",
                 "es-abstract": "^1.20.4"
             },
             "dev": true,
@@ -6551,28 +6471,28 @@
             },
             "integrity": "sha512-lNaJgI+2Q5URQBkccEKHTQOPaXdUxnZZElQTZY0MFUAuaEqe1E+Nyvgdz/aIyNi6Z9MzO5dv1H8n58/GELp3+w==",
             "resolved": "https://registry.npmjs.org/once/-/once-1.4.0.tgz",
             "version": "1.4.0"
         },
         "node_modules/optionator": {
             "dependencies": {
+                "@aashutoshrathi/word-wrap": "^1.2.3",
                 "deep-is": "^0.1.3",
                 "fast-levenshtein": "^2.0.6",
                 "levn": "^0.4.1",
                 "prelude-ls": "^1.2.1",
-                "type-check": "^0.4.0",
-                "word-wrap": "^1.2.3"
+                "type-check": "^0.4.0"
             },
             "dev": true,
             "engines": {
                 "node": ">= 0.8.0"
             },
-            "integrity": "sha512-74RlY5FCnhq4jRxVUPKDaRwrVNXMqsGsiW6AJw4XK8hmtm10wC0ypZBLw5IIp85NZMr91+qd1RvvENwg7jjRFw==",
-            "resolved": "https://registry.npmjs.org/optionator/-/optionator-0.9.1.tgz",
-            "version": "0.9.1"
+            "integrity": "sha512-JjCoypp+jKn1ttEFExxhetCKeJt9zhAgAve5FXHixTvFDW/5aEktX9bufBKLRRMdU7bNtpLfcGu94B3cdEJgjg==",
+            "resolved": "https://registry.npmjs.org/optionator/-/optionator-0.9.3.tgz",
+            "version": "0.9.3"
         },
         "node_modules/p-limit": {
             "dependencies": {
                 "yocto-queue": "^0.1.0"
             },
             "dev": true,
             "engines": {
@@ -6884,28 +6804,28 @@
                 "parse-svg-path": "^0.1.2",
                 "point-in-polygon": "^1.1.0",
                 "polybooljs": "^1.2.0",
                 "probe-image-size": "^7.2.3",
                 "regl": "npm:@plotly/regl@^2.1.2",
                 "regl-error2d": "^2.0.12",
                 "regl-line2d": "^3.1.2",
-                "regl-scatter2d": "^3.2.8",
+                "regl-scatter2d": "^3.2.9",
                 "regl-splom": "^1.0.14",
                 "strongly-connected-components": "^1.0.1",
                 "superscript-text": "^1.0.0",
                 "svg-path-sdf": "^1.1.3",
                 "tinycolor2": "^1.4.2",
                 "to-px": "1.0.1",
                 "topojson-client": "^3.1.0",
                 "webgl-context": "^2.2.0",
                 "world-calendars": "^1.0.3"
             },
-            "integrity": "sha512-g+YTMnChFDx/fNUV2rqkrf87wKwKuOhqv9LIxhmPyF94RGM4v4blP0mmgwQ278qv3kXmfTMJecIUusr1gzscng==",
-            "resolved": "https://registry.npmjs.org/plotly.js/-/plotly.js-2.22.0.tgz",
-            "version": "2.22.0"
+            "integrity": "sha512-zwcXyPuofbpaWKasLdezicJQ3lbgkqQZk5D8jqDPt9ZCRDw9pgPCIDB05Dn4akSHPBGTwIpMK/2MqsDDLQOi+w==",
+            "resolved": "https://registry.npmjs.org/plotly.js/-/plotly.js-2.25.0.tgz",
+            "version": "2.25.0"
         },
         "node_modules/plotly.js/node_modules/d3-array": {
             "integrity": "sha512-KHW6M86R+FUPYGb3R5XiYjXPq7VzwxZ22buHhAEVG5ztoEcZZMLov530mmccaqA1GghZArjQV46fuc8kUqhhHw==",
             "resolved": "https://registry.npmjs.org/d3-array/-/d3-array-1.2.4.tgz",
             "version": "1.2.4"
         },
         "node_modules/plotly.js/node_modules/d3-dispatch": {
@@ -6995,40 +6915,39 @@
                     "url": "https://tidelift.com/funding/github/npm/postcss"
                 },
                 {
                     "type": "github",
                     "url": "https://github.com/sponsors/ai"
                 }
             ],
-            "integrity": "sha512-bQ3qMcpF6A/YjR55xtoTr0jGOlnPOKAIMdOWiv0EIT6HVPEaJiJB4NLljSbiHoC2RX7DN5Uvjtpbg1NPdwv1oA==",
-            "resolved": "https://registry.npmjs.org/postcss/-/postcss-8.4.23.tgz",
-            "version": "8.4.23"
+            "integrity": "sha512-gY/ACJtJPSmUFPDCHtX78+01fHa64FaU4zaaWfuh1MhGJISufJAH4cun6k/8fwsHYeK4UQmENQK+tRLCFJE8JQ==",
+            "resolved": "https://registry.npmjs.org/postcss/-/postcss-8.4.27.tgz",
+            "version": "8.4.27"
         },
         "node_modules/postcss-loader": {
             "dependencies": {
-                "cosmiconfig": "^8.1.3",
+                "cosmiconfig": "^8.2.0",
                 "jiti": "^1.18.2",
-                "klona": "^2.0.6",
                 "semver": "^7.3.8"
             },
             "dev": true,
             "engines": {
                 "node": ">= 14.15.0"
             },
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/webpack"
             },
-            "integrity": "sha512-qLAFjvR2BFNz1H930P7mj1iuWJFjGey/nVhimfOAAQ1ZyPpcClAxP8+A55Sl8mBvM+K2a9Pjgdj10KpANWrNfw==",
+            "integrity": "sha512-YgO/yhtevGO/vJePCQmTxiaEwER94LABZN0ZMT4A0vsak9TpO+RvKRs7EmJ8peIlB9xfXCsS7M8LjqncsUZ5HA==",
             "peerDependencies": {
                 "postcss": "^7.0.0 || ^8.0.1",
                 "webpack": "^5.0.0"
             },
-            "resolved": "https://registry.npmjs.org/postcss-loader/-/postcss-loader-7.3.0.tgz",
-            "version": "7.3.0"
+            "resolved": "https://registry.npmjs.org/postcss-loader/-/postcss-loader-7.3.3.tgz",
+            "version": "7.3.3"
         },
         "node_modules/postcss-modules-extract-imports": {
             "dev": true,
             "engines": {
                 "node": "^10 || ^12 || >= 14"
             },
             "integrity": "sha512-bdHleFnP3kZ4NYDhuGlVK+CMrQ/pqUm8bx/oGL93K6gVwiclvX5x0n76fYMKuIGKzlABOy13zsvqjb0f92TEXw==",
@@ -7044,20 +6963,20 @@
                 "postcss-selector-parser": "^6.0.2",
                 "postcss-value-parser": "^4.1.0"
             },
             "dev": true,
             "engines": {
                 "node": "^10 || ^12 || >= 14"
             },
-            "integrity": "sha512-sT7ihtmGSF9yhm6ggikHdV0hlziDTX7oFoXtuVWeDd3hHObNkcHRo9V3yg7vCAY7cONyxJC/XXCmmiHHcvX7bQ==",
+            "integrity": "sha512-2/u2zraspoACtrbFRnTijMiQtb4GW4BvatjaG/bCjYQo8kLTdevCUlwuBHx2sCnSyrI3x3qj4ZK1j5LQBgzmwA==",
             "peerDependencies": {
                 "postcss": "^8.1.0"
             },
-            "resolved": "https://registry.npmjs.org/postcss-modules-local-by-default/-/postcss-modules-local-by-default-4.0.0.tgz",
-            "version": "4.0.0"
+            "resolved": "https://registry.npmjs.org/postcss-modules-local-by-default/-/postcss-modules-local-by-default-4.0.3.tgz",
+            "version": "4.0.3"
         },
         "node_modules/postcss-modules-scope": {
             "dependencies": {
                 "postcss-selector-parser": "^6.0.4"
             },
             "dev": true,
             "engines": {
@@ -7090,17 +7009,17 @@
                 "cssesc": "^3.0.0",
                 "util-deprecate": "^1.0.2"
             },
             "dev": true,
             "engines": {
                 "node": ">=4"
             },
-            "integrity": "sha512-NdxGCAZdRrwVI1sy59+Wzrh+pMMHxapGnpfenDVlMEXoOcvt4pGE0JLK9YY2F5dLxcFYA/YbVQKhcGU+FtSYQg==",
-            "resolved": "https://registry.npmjs.org/postcss-selector-parser/-/postcss-selector-parser-6.0.12.tgz",
-            "version": "6.0.12"
+            "integrity": "sha512-EaV1Gl4mUEV4ddhDnv/xtj7sxwrwxdetHdWUGnT4VJQf+4d05v6lHYZr8N573k5Z0BViss7BDhfWtKS3+sfAqQ==",
+            "resolved": "https://registry.npmjs.org/postcss-selector-parser/-/postcss-selector-parser-6.0.13.tgz",
+            "version": "6.0.13"
         },
         "node_modules/postcss-value-parser": {
             "dev": true,
             "integrity": "sha512-1NNCs6uurfkVbeXG4S8JFT9t19m45ICnif8zWLd5oPSZ50QnwMfK+H3jv408d4jw/7Bttv5axS5IiHoLaVNHeQ==",
             "resolved": "https://registry.npmjs.org/postcss-value-parser/-/postcss-value-parser-4.2.0.tgz",
             "version": "4.2.0"
         },
@@ -7172,35 +7091,14 @@
             "engines": {
                 "node": ">=6"
             },
             "integrity": "sha512-rRV+zQD8tVFys26lAGR9WUuS4iUAngJScM+ZRSKtvl5tKeZ2t5bvdNFdNHBW9FWR4guGHlgmsZ1G7BSm2wTbuA==",
             "resolved": "https://registry.npmjs.org/punycode/-/punycode-2.3.0.tgz",
             "version": "2.3.0"
         },
-        "node_modules/pxls": {
-            "dependencies": {
-                "arr-flatten": "^1.1.0",
-                "compute-dims": "^1.1.0",
-                "flip-pixels": "^1.0.2",
-                "is-browser": "^2.1.0",
-                "is-buffer": "^2.0.3",
-                "to-uint8": "^1.4.1"
-            },
-            "integrity": "sha512-pQkwgbLqWPcuES5iEmGa10OlCf5xG0blkIF3dg7PpRZShbTYcvAdfFfGL03SMrkaSUaa/V0UpN9HWg40O2AIIw==",
-            "resolved": "https://registry.npmjs.org/pxls/-/pxls-2.3.2.tgz",
-            "version": "2.3.2"
-        },
-        "node_modules/quantize": {
-            "engines": {
-                "node": ">=0.10.21"
-            },
-            "integrity": "sha512-25P7wI2UoDbIQsQp50ARkt+5pwPsOq7G/BqvT5xAbapnRoNWMN8/p55H9TXd5MuENiJnm5XICB2H2aDZGwts7w==",
-            "resolved": "https://registry.npmjs.org/quantize/-/quantize-1.0.2.tgz",
-            "version": "1.0.2"
-        },
         "node_modules/queue-microtask": {
             "dev": true,
             "funding": [
                 {
                     "type": "github",
                     "url": "https://github.com/sponsors/feross"
                 },
@@ -7360,17 +7258,17 @@
             "version": "2.5.0"
         },
         "node_modules/read-pkg/node_modules/semver": {
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
         "node_modules/read-pkg/node_modules/type-fest": {
             "dev": true,
             "engines": {
                 "node": ">=8"
             },
             "integrity": "sha512-q+MB8nYR1KDLrgr4G5yemftpMC7/QLqVndBmEEdqzmNj5dcFOO4Oo8qlwZE3ULT3+Zim1F8Kq4cBnikNhlCMlg==",
@@ -7442,19 +7340,14 @@
             "engines": {
                 "node": ">=8"
             },
             "integrity": "sha512-6tDA8g98We0zd0GvVeMT9arEOnTw9qM03L9cJXaCjrip1OO764RDBLBfrB4cwzNGDj5OA5ioymC9GkizgWJDUg==",
             "resolved": "https://registry.npmjs.org/redent/-/redent-3.0.0.tgz",
             "version": "3.0.0"
         },
-        "node_modules/regex-regex": {
-            "integrity": "sha512-FPbEhFTLpxKNgHKay3zMfkHzFK2ebViAlyvsz5euO4kwekH0T6fAL4Sdo2CgQ7Y1tGB5HqQm8SBq7pW5GegvVA==",
-            "resolved": "https://registry.npmjs.org/regex-regex/-/regex-regex-1.0.0.tgz",
-            "version": "1.0.0"
-        },
         "node_modules/regexp.prototype.flags": {
             "dependencies": {
                 "call-bind": "^1.0.2",
                 "define-properties": "^1.2.0",
                 "functions-have-names": "^1.2.3"
             },
             "dev": true,
@@ -7526,25 +7419,24 @@
                 "array-rearrange": "^2.2.2",
                 "clamp": "^1.0.1",
                 "color-id": "^1.1.0",
                 "color-normalize": "^1.5.0",
                 "color-rgba": "^2.1.1",
                 "flatten-vertex-data": "^1.0.2",
                 "glslify": "^7.0.0",
-                "image-palette": "^2.1.0",
                 "is-iexplorer": "^1.0.0",
                 "object-assign": "^4.1.1",
                 "parse-rect": "^1.2.0",
                 "pick-by-alias": "^1.2.0",
                 "to-float32": "^1.1.0",
                 "update-diff": "^1.1.0"
             },
-            "integrity": "sha512-bqrqJyeHkGBa9mEfuBnRd7FUtdtZ1l+gsM2C5Ugr1U3vJG5K3mdWdVWtOAllZ5FHHyWJV/vgjVvftgFUg6CDig==",
-            "resolved": "https://registry.npmjs.org/regl-scatter2d/-/regl-scatter2d-3.2.8.tgz",
-            "version": "3.2.8"
+            "integrity": "sha512-PNrXs+xaCClKpiB2b3HZ2j3qXQXhC5kcTh/Nfgx9rLO0EpEhab0BSQDqAsbdbpdf+pSHSJvbgitB7ulbGeQ+Fg==",
+            "resolved": "https://registry.npmjs.org/regl-scatter2d/-/regl-scatter2d-3.2.9.tgz",
+            "version": "3.2.9"
         },
         "node_modules/regl-splom": {
             "dependencies": {
                 "array-bounds": "^1.0.1",
                 "array-range": "^1.0.1",
                 "color-alpha": "^1.0.4",
                 "flatten-vertex-data": "^1.0.2",
@@ -7598,24 +7490,24 @@
             "version": "2.0.2"
         },
         "node_modules/resolve": {
             "bin": {
                 "resolve": "bin/resolve"
             },
             "dependencies": {
-                "is-core-module": "^2.11.0",
+                "is-core-module": "^2.12.0",
                 "path-parse": "^1.0.7",
                 "supports-preserve-symlinks-flag": "^1.0.0"
             },
             "funding": {
                 "url": "https://github.com/sponsors/ljharb"
             },
-            "integrity": "sha512-Sb+mjNHOULsBv818T40qSPeRiuWLyaGMa5ewydRLFimneixmVy2zdivRl+AF6jaYPC8ERxGDmFSiqui6SfPd+g==",
-            "resolved": "https://registry.npmjs.org/resolve/-/resolve-1.22.2.tgz",
-            "version": "1.22.2"
+            "integrity": "sha512-P8ur/gp/AmbEzjr729bZnLjXK5Z+4P0zhIJgBgzqRih7hL7BOukHGtSTA3ACMY467GRFz3duQsi0bDZdR7DKdw==",
+            "resolved": "https://registry.npmjs.org/resolve/-/resolve-1.22.3.tgz",
+            "version": "1.22.3"
         },
         "node_modules/resolve-cwd": {
             "dependencies": {
                 "resolve-from": "^5.0.0"
             },
             "dev": true,
             "engines": {
@@ -7687,17 +7579,17 @@
                 "url": "https://github.com/sponsors/isaacs"
             },
             "integrity": "sha512-JZkJMZkAGFFPP2YqXZXPbMlMBgsxzE8ILs4lMIX/2o0L9UBw9O/Y3o6wFw/i9YLapcUJWwqbi3kdxIPdC62TIA==",
             "resolved": "https://registry.npmjs.org/rimraf/-/rimraf-3.0.2.tgz",
             "version": "3.0.2"
         },
         "node_modules/robust-predicates": {
-            "integrity": "sha512-ndEIpszUHiG4HtDsQLeIuMvRsDnn8c8rYStabochtUeCvfuvNptb5TUbVD68LRAILPX7p9nqQGh4xJgn3EHS/g==",
-            "resolved": "https://registry.npmjs.org/robust-predicates/-/robust-predicates-3.0.1.tgz",
-            "version": "3.0.1"
+            "integrity": "sha512-IXgzBWvWQwE6PrDI05OvmXUIruQTcoMDzRsOd5CDvHCVLcLHMTSYvOK5Cm46kWqlV3yAbuSpBZdJ5oP5OUoStg==",
+            "resolved": "https://registry.npmjs.org/robust-predicates/-/robust-predicates-3.0.2.tgz",
+            "version": "3.0.2"
         },
         "node_modules/run-parallel": {
             "dependencies": {
                 "queue-microtask": "^1.2.2"
             },
             "dev": true,
             "funding": [
@@ -7719,14 +7611,32 @@
             "version": "1.2.0"
         },
         "node_modules/rw": {
             "integrity": "sha512-PdhdWy89SiZogBLaw42zdeqtRJ//zFd2PgQavcICDUgJT5oW10QCRKbJ6bg4r0/UY2M6BWd5tkxuGFRvCkgfHQ==",
             "resolved": "https://registry.npmjs.org/rw/-/rw-1.3.3.tgz",
             "version": "1.3.3"
         },
+        "node_modules/safe-array-concat": {
+            "dependencies": {
+                "call-bind": "^1.0.2",
+                "get-intrinsic": "^1.2.0",
+                "has-symbols": "^1.0.3",
+                "isarray": "^2.0.5"
+            },
+            "dev": true,
+            "engines": {
+                "node": ">=0.4"
+            },
+            "funding": {
+                "url": "https://github.com/sponsors/ljharb"
+            },
+            "integrity": "sha512-9dVEFruWIsnie89yym+xWTAYASdpw3CJV7Li/6zBewGf9z2i1j31rP6jnY0pHEO4QZh6N0K11bFjWmdR8UGdPQ==",
+            "resolved": "https://registry.npmjs.org/safe-array-concat/-/safe-array-concat-1.0.0.tgz",
+            "version": "1.0.0"
+        },
         "node_modules/safe-buffer": {
             "dev": true,
             "funding": [
                 {
                     "type": "github",
                     "url": "https://github.com/sponsors/feross"
                 },
@@ -7778,29 +7688,28 @@
             },
             "integrity": "sha512-5YCfmGBmxoIRYHnKK2AKzrAkCoQ8ozO+iumT8K4tXJXRVCPf+7s1/9KxTSW3Rbvf+7Y7b4FR3mWyLnQr3PHocA==",
             "resolved": "https://registry.npmjs.org/sass-graph/-/sass-graph-4.0.1.tgz",
             "version": "4.0.1"
         },
         "node_modules/sass-loader": {
             "dependencies": {
-                "klona": "^2.0.6",
                 "neo-async": "^2.6.2"
             },
             "dev": true,
             "engines": {
                 "node": ">= 14.15.0"
             },
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/webpack"
             },
-            "integrity": "sha512-nrIdVAAte3B9icfBiGWvmMhT/D+eCDwnk+yA7VE/76dp/WkHX+i44Q/pfo71NYbwj0Ap+PGsn0ekOuU1WFJ2AA==",
+            "integrity": "sha512-CQbKl57kdEv+KDLquhC+gE3pXt74LEAzm+tzywcA0/aHZuub8wTErbjAoNI57rPUWRYRNC5WUnNl8eGJNbDdwg==",
             "peerDependencies": {
                 "fibers": ">= 3.1.0",
-                "node-sass": "^4.0.0 || ^5.0.0 || ^6.0.0 || ^7.0.0 || ^8.0.0",
+                "node-sass": "^4.0.0 || ^5.0.0 || ^6.0.0 || ^7.0.0 || ^8.0.0 || ^9.0.0",
                 "sass": "^1.3.0",
                 "sass-embedded": "*",
                 "webpack": "^5.0.0"
             },
             "peerDependenciesMeta": {
                 "fibers": {
                     "optional": true
@@ -7811,16 +7720,16 @@
                 "sass": {
                     "optional": true
                 },
                 "sass-embedded": {
                     "optional": true
                 }
             },
-            "resolved": "https://registry.npmjs.org/sass-loader/-/sass-loader-13.2.2.tgz",
-            "version": "13.2.2"
+            "resolved": "https://registry.npmjs.org/sass-loader/-/sass-loader-13.3.2.tgz",
+            "version": "13.3.2"
         },
         "node_modules/sax": {
             "integrity": "sha512-NqVDv9TpANUjFm0N8uM5GxL36UgKi9/atZw+x7YFnQ8ckwFGKrl4xX4yWtrey3UJm5nP1kUbnYgLopqWNSRhWw==",
             "resolved": "https://registry.npmjs.org/sax/-/sax-1.2.4.tgz",
             "version": "1.2.4"
         },
         "node_modules/schema-utils": {
@@ -7833,17 +7742,17 @@
             "engines": {
                 "node": ">= 10.13.0"
             },
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/webpack"
             },
-            "integrity": "sha512-pvjEHOgWc9OWA/f/DE3ohBWTD6EleVLf7iFUkoSwAxttdBhB9QUebQgxER2kWueOvRJXPHNnyrvvh9eZINB8Eg==",
-            "resolved": "https://registry.npmjs.org/schema-utils/-/schema-utils-3.1.2.tgz",
-            "version": "3.1.2"
+            "integrity": "sha512-pN/yOAvcC+5rQ5nERGuwrjLlYvLTbCibnZ1I7B1LaiAz9BRBlE9GMgE/eqV30P7aJQUf7Ddimy/RsbYO/GrVGg==",
+            "resolved": "https://registry.npmjs.org/schema-utils/-/schema-utils-3.3.0.tgz",
+            "version": "3.3.0"
         },
         "node_modules/scss-tokenizer": {
             "dependencies": {
                 "js-base64": "^2.4.9",
                 "source-map": "^0.7.3"
             },
             "dev": true,
@@ -7867,17 +7776,17 @@
             "dependencies": {
                 "lru-cache": "^6.0.0"
             },
             "dev": true,
             "engines": {
                 "node": ">=10"
             },
-            "integrity": "sha512-+XC0AD/R7Q2mPSRuy2Id0+CGTZ98+8f+KvwirxOKIEyid+XSx6HbC63p+O4IndTHuX5Z+JxQ0TghCkO5Cg/2HA==",
-            "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.0.tgz",
-            "version": "7.5.0"
+            "integrity": "sha512-1bCSESV6Pv+i21Hvpxp3Dx+pSD8lIPt8uVjRrxAUt/nbswYc+tK6Y2btiULjd4+fnq15PX+nqQDC7Oft7WkwcA==",
+            "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.4.tgz",
+            "version": "7.5.4"
         },
         "node_modules/semver/node_modules/lru-cache": {
             "dependencies": {
                 "yallist": "^4.0.0"
             },
             "dev": true,
             "engines": {
@@ -8166,23 +8075,14 @@
             "dependencies": {
                 "parenthesis": "^3.1.5"
             },
             "integrity": "sha512-KaJKY+hfpzNyet/emP81PJA9hTVSfxNLS9SFTWxdCnnW1/zOOwiV248+EfoX7IQFcBaOp4G5YE6xTJMF+pLg6A==",
             "resolved": "https://registry.npmjs.org/string-split-by/-/string-split-by-1.0.0.tgz",
             "version": "1.0.0"
         },
-        "node_modules/string-to-arraybuffer": {
-            "dependencies": {
-                "atob-lite": "^2.0.0",
-                "is-base64": "^0.1.0"
-            },
-            "integrity": "sha512-DaGZidzi93dwjQen5I2osxR9ERS/R7B1PFyufNMnzhj+fmlDQAc1DSDIJVJhgI8Oq221efIMbABUBdPHDRt43Q==",
-            "resolved": "https://registry.npmjs.org/string-to-arraybuffer/-/string-to-arraybuffer-1.0.2.tgz",
-            "version": "1.0.2"
-        },
         "node_modules/string-width": {
             "dependencies": {
                 "emoji-regex": "^8.0.0",
                 "is-fullwidth-code-point": "^3.0.0",
                 "strip-ansi": "^6.0.1"
             },
             "dev": true,
@@ -8302,20 +8202,20 @@
             "engines": {
                 "node": ">= 12.13.0"
             },
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/webpack"
             },
-            "integrity": "sha512-RHs/vcrKdQK8wZliteNK4NKzxvLBzpuHMqYmUVWeKa6MkaIQ97ZTOS0b+zapZhy6GcrgWnvWYCMHRirC3FsUmw==",
+            "integrity": "sha512-53BiGLXAcll9maCYtZi2RCQZKa8NQQai5C4horqKyRmHj9H7QmcUyucrH+4KW/gBQbXM2AsB0axoEcFZPlfPcw==",
             "peerDependencies": {
                 "webpack": "^5.0.0"
             },
-            "resolved": "https://registry.npmjs.org/style-loader/-/style-loader-3.3.2.tgz",
-            "version": "3.3.2"
+            "resolved": "https://registry.npmjs.org/style-loader/-/style-loader-3.3.3.tgz",
+            "version": "3.3.3"
         },
         "node_modules/supercluster": {
             "dependencies": {
                 "kdbush": "^3.0.0"
             },
             "integrity": "sha512-EulshI3pGUM66o6ZdH3ReiFcvHpM3vAigyK+vcxdjpJyEbIIrtbmBdY23mGgnI24uXiGFvrGq9Gkum/8U7vJWg==",
             "resolved": "https://registry.npmjs.org/supercluster/-/supercluster-7.1.5.tgz",
@@ -8394,26 +8294,26 @@
             "resolved": "https://registry.npmjs.org/tapable/-/tapable-2.2.1.tgz",
             "version": "2.2.1"
         },
         "node_modules/tar": {
             "dependencies": {
                 "chownr": "^2.0.0",
                 "fs-minipass": "^2.0.0",
-                "minipass": "^4.0.0",
+                "minipass": "^5.0.0",
                 "minizlib": "^2.1.1",
                 "mkdirp": "^1.0.3",
                 "yallist": "^4.0.0"
             },
             "dev": true,
             "engines": {
                 "node": ">=10"
             },
-            "integrity": "sha512-jdIBIN6LTIe2jqzay/2vtYLlBHa3JF42ot3h1dW8Q0PaAG4v8rm0cvpVePtau5C6OKXGGcgO9q2AMNSWxiLqKw==",
-            "resolved": "https://registry.npmjs.org/tar/-/tar-6.1.13.tgz",
-            "version": "6.1.13"
+            "integrity": "sha512-/zKt9UyngnxIT/EAGYuxaMYgOIJiP81ab9ZfkILq4oNLPFX50qyYmu7jRj9qeXoxmJHjGlbH0+cm2uy1WCs10A==",
+            "resolved": "https://registry.npmjs.org/tar/-/tar-6.1.15.tgz",
+            "version": "6.1.15"
         },
         "node_modules/tar-stream": {
             "dependencies": {
                 "bl": "^4.0.3",
                 "end-of-stream": "^1.4.1",
                 "fs-constants": "^1.0.0",
                 "inherits": "^2.0.3",
@@ -8439,69 +8339,69 @@
             "version": "4.1.0"
         },
         "node_modules/tar/node_modules/minipass": {
             "dev": true,
             "engines": {
                 "node": ">=8"
             },
-            "integrity": "sha512-fNzuVyifolSLFL4NzpF+wEF4qrgqaaKX0haXPQEdQ7NKAN+WecoKMHV09YcuL/DHxrUsYQOK3MiuDf7Ip2OXfQ==",
-            "resolved": "https://registry.npmjs.org/minipass/-/minipass-4.2.8.tgz",
-            "version": "4.2.8"
+            "integrity": "sha512-3FnjYuehv9k6ovOEbyOswadCDPX1piCfhV8ncmYtHOjuPwylVWsghTLo7rabjC3Rx5xD4HDx8Wm1xnMF7S5qFQ==",
+            "resolved": "https://registry.npmjs.org/minipass/-/minipass-5.0.0.tgz",
+            "version": "5.0.0"
         },
         "node_modules/terser": {
             "bin": {
                 "terser": "bin/terser"
             },
             "dependencies": {
-                "@jridgewell/source-map": "^0.3.2",
-                "acorn": "^8.5.0",
+                "@jridgewell/source-map": "^0.3.3",
+                "acorn": "^8.8.2",
                 "commander": "^2.20.0",
                 "source-map-support": "~0.5.20"
             },
             "dev": true,
             "engines": {
                 "node": ">=10"
             },
-            "integrity": "sha512-hVl35zClmpisy6oaoKALOpS0rDYLxRFLHhRuDlEGTKey9qHjS1w9GMORjuwIMt70Wan4lwsLYyWDVnWgF+KUEw==",
-            "resolved": "https://registry.npmjs.org/terser/-/terser-5.17.1.tgz",
-            "version": "5.17.1"
+            "integrity": "sha512-qC5+dmecKJA4cpYxRa5aVkKehYsQKc+AHeKl0Oe62aYjBL8ZA33tTljktDHJSaxxMnbI5ZYw+o/S2DxxLu8OfA==",
+            "resolved": "https://registry.npmjs.org/terser/-/terser-5.19.2.tgz",
+            "version": "5.19.2"
         },
         "node_modules/terser-webpack-plugin": {
             "dependencies": {
                 "@jridgewell/trace-mapping": "^0.3.17",
                 "jest-worker": "^27.4.5",
                 "schema-utils": "^3.1.1",
                 "serialize-javascript": "^6.0.1",
-                "terser": "^5.16.5"
+                "terser": "^5.16.8"
             },
             "dev": true,
             "engines": {
                 "node": ">= 10.13.0"
             },
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/webpack"
             },
-            "integrity": "sha512-AfKwIktyP7Cu50xNjXF/6Qb5lBNzYaWpU6YfoX3uZicTx0zTy0stDDCsvjDapKsSDvOeWo5MEq4TmdBy2cNoHw==",
+            "integrity": "sha512-ZuXsqE07EcggTWQjXUj+Aot/OMcD0bMKGgF63f7UxYcu5/AJF53aIpK1YoP5xR9l6s/Hy2b+t1AM0bLNPRuhwA==",
             "peerDependencies": {
                 "webpack": "^5.1.0"
             },
             "peerDependenciesMeta": {
                 "@swc/core": {
                     "optional": true
                 },
                 "esbuild": {
                     "optional": true
                 },
                 "uglify-js": {
                     "optional": true
                 }
             },
-            "resolved": "https://registry.npmjs.org/terser-webpack-plugin/-/terser-webpack-plugin-5.3.7.tgz",
-            "version": "5.3.7"
+            "resolved": "https://registry.npmjs.org/terser-webpack-plugin/-/terser-webpack-plugin-5.3.9.tgz",
+            "version": "5.3.9"
         },
         "node_modules/terser/node_modules/commander": {
             "dev": true,
             "integrity": "sha512-GpVkmM8vF2vQUkj2LvZmD35JxeJOLCwJ9cUkugyk2nuhbv3+mJvpLYYt+0+USMxE+oj+ey/lJEnhZw75x/OMcQ==",
             "resolved": "https://registry.npmjs.org/commander/-/commander-2.20.3.tgz",
             "version": "2.20.3"
         },
@@ -8558,49 +8458,27 @@
             "version": "1.6.0"
         },
         "node_modules/tinyqueue": {
             "integrity": "sha512-ppJZNDuKGgxzkHihX8v9v9G5f+18gzaTfrukGrq6ueg0lmH4nqVnA2IPG0AEH3jKEk2GRJCUhDoqpoiw3PHLBA==",
             "resolved": "https://registry.npmjs.org/tinyqueue/-/tinyqueue-2.0.3.tgz",
             "version": "2.0.3"
         },
-        "node_modules/to-array-buffer": {
-            "dependencies": {
-                "flatten-vertex-data": "^1.0.2",
-                "is-blob": "^2.0.1",
-                "string-to-arraybuffer": "^1.0.0"
-            },
-            "integrity": "sha512-zN33mwi0gpL+7xW1ITLfJ48CEj6ZQW0ZAP0MU+2W3kEY0PAIncyuxmD4OqkUVhPAbTP7amq9j/iwvZKYS+lzSQ==",
-            "resolved": "https://registry.npmjs.org/to-array-buffer/-/to-array-buffer-3.2.0.tgz",
-            "version": "3.2.0"
-        },
         "node_modules/to-float32": {
             "integrity": "sha512-keDnAusn/vc+R3iEiSDw8TOF7gPiTLdK1ArvWtYbJQiVfmRg6i/CAvbKq3uIS0vWroAC7ZecN3DjQKw3aSklUg==",
             "resolved": "https://registry.npmjs.org/to-float32/-/to-float32-1.1.0.tgz",
             "version": "1.1.0"
         },
         "node_modules/to-px": {
             "dependencies": {
                 "parse-unit": "^1.0.1"
             },
             "integrity": "sha512-2y3LjBeIZYL19e5gczp14/uRWFDtDUErJPVN3VU9a7SJO+RjGRtYR47aMN2bZgGlxvW4ZcEz2ddUPVHXcMfuXw==",
             "resolved": "https://registry.npmjs.org/to-px/-/to-px-1.0.1.tgz",
             "version": "1.0.1"
         },
-        "node_modules/to-uint8": {
-            "dependencies": {
-                "arr-flatten": "^1.1.0",
-                "clamp": "^1.0.1",
-                "is-base64": "^0.1.0",
-                "is-float-array": "^1.0.0",
-                "to-array-buffer": "^3.0.0"
-            },
-            "integrity": "sha512-o+ochsMlTZyucbww8It401FC2Rx+OP2RpDeYbA6h+y9HgedDl1UjdsJ9CmzKEG7AFP9es5PmJ4eDWeeeXihESg==",
-            "resolved": "https://registry.npmjs.org/to-uint8/-/to-uint8-1.4.1.tgz",
-            "version": "1.4.1"
-        },
         "node_modules/topojson-client": {
             "bin": {
                 "topo2geo": "bin/topo2geo",
                 "topomerge": "bin/topomerge",
                 "topoquantize": "bin/topoquantize"
             },
             "dependencies": {
@@ -8652,17 +8530,17 @@
             "dev": true,
             "integrity": "sha512-g1MWMLBiz8FKi1e4w0UyVL3w+iJceWAFBAaBnnGKOpNa5f8TLktkbre1+s6oICydWAm+HRUGTmI+//xv2hvXYA==",
             "resolved": "https://registry.npmjs.org/json5/-/json5-1.0.2.tgz",
             "version": "1.0.2"
         },
         "node_modules/tslib": {
             "dev": true,
-            "integrity": "sha512-336iVw3rtn2BUK7ORdIAHTyxHGRIHVReokCR3XjbckJMK7ms8FysBfhLR8IXnAgy7T0PTPNBWKiH514FOW/WSg==",
-            "resolved": "https://registry.npmjs.org/tslib/-/tslib-2.5.0.tgz",
-            "version": "2.5.0"
+            "integrity": "sha512-t0hLfiEKfMUoqhG+U1oid7Pva4bbDPHYfJNiB7BiIjRkj1pyC++4N3huJfqY6aRH6VTB0rvtzQwjM4K6qpfOig==",
+            "resolved": "https://registry.npmjs.org/tslib/-/tslib-2.6.1.tgz",
+            "version": "2.6.1"
         },
         "node_modules/type": {
             "integrity": "sha512-+5nt5AAniqsCnu2cEQQdpzCAh33kVx8n0VoFidKpB1dVVLAN/F+bgVOqOJqOnEnrhp222clB5p3vUlD+1QAnfg==",
             "resolved": "https://registry.npmjs.org/type/-/type-1.2.0.tgz",
             "version": "1.2.0"
         },
         "node_modules/type-check": {
@@ -8685,18 +8563,64 @@
             "funding": {
                 "url": "https://github.com/sponsors/sindresorhus"
             },
             "integrity": "sha512-Ne+eE4r0/iWnpAxD852z3A+N0Bt5RN//NjJwRd2VFHEmrywxf5vsZlh4R6lixl6B+wz/8d+maTSAkN1FIkI3LQ==",
             "resolved": "https://registry.npmjs.org/type-fest/-/type-fest-0.20.2.tgz",
             "version": "0.20.2"
         },
-        "node_modules/type-name": {
-            "integrity": "sha512-kkgkuqR/jKdKO5oh/I2SMu2dGbLXoJq0zkdgbxaqYK+hr9S9edwVVGf+tMUFTx2gH9TN2+Zu9JZ/Njonb3cjhA==",
-            "resolved": "https://registry.npmjs.org/type-name/-/type-name-2.0.2.tgz",
-            "version": "2.0.2"
+        "node_modules/typed-array-buffer": {
+            "dependencies": {
+                "call-bind": "^1.0.2",
+                "get-intrinsic": "^1.2.1",
+                "is-typed-array": "^1.1.10"
+            },
+            "dev": true,
+            "engines": {
+                "node": ">= 0.4"
+            },
+            "integrity": "sha512-Y8KTSIglk9OZEr8zywiIHG/kmQ7KWyjseXs1CbSo8vC42w7hg2HgYTxSWwP0+is7bWDc1H+Fo026CpHFwm8tkw==",
+            "resolved": "https://registry.npmjs.org/typed-array-buffer/-/typed-array-buffer-1.0.0.tgz",
+            "version": "1.0.0"
+        },
+        "node_modules/typed-array-byte-length": {
+            "dependencies": {
+                "call-bind": "^1.0.2",
+                "for-each": "^0.3.3",
+                "has-proto": "^1.0.1",
+                "is-typed-array": "^1.1.10"
+            },
+            "dev": true,
+            "engines": {
+                "node": ">= 0.4"
+            },
+            "funding": {
+                "url": "https://github.com/sponsors/ljharb"
+            },
+            "integrity": "sha512-Or/+kvLxNpeQ9DtSydonMxCx+9ZXOswtwJn17SNLvhptaXYDJvkFFP5zbfU/uLmvnBJlI4yrnXRxpdWH/M5tNA==",
+            "resolved": "https://registry.npmjs.org/typed-array-byte-length/-/typed-array-byte-length-1.0.0.tgz",
+            "version": "1.0.0"
+        },
+        "node_modules/typed-array-byte-offset": {
+            "dependencies": {
+                "available-typed-arrays": "^1.0.5",
+                "call-bind": "^1.0.2",
+                "for-each": "^0.3.3",
+                "has-proto": "^1.0.1",
+                "is-typed-array": "^1.1.10"
+            },
+            "dev": true,
+            "engines": {
+                "node": ">= 0.4"
+            },
+            "funding": {
+                "url": "https://github.com/sponsors/ljharb"
+            },
+            "integrity": "sha512-RD97prjEt9EL8YgAgpOkf3O4IF9lhJFr9g0htQkm0rchFp/Vx7LW5Q8fSXXub7BXAODyUQohRMyOc3faCPd0hg==",
+            "resolved": "https://registry.npmjs.org/typed-array-byte-offset/-/typed-array-byte-offset-1.0.0.tgz",
+            "version": "1.0.0"
         },
         "node_modules/typed-array-length": {
             "dependencies": {
                 "call-bind": "^1.0.2",
                 "for-each": "^0.3.3",
                 "is-typed-array": "^1.1.9"
             },
@@ -8817,143 +8741,24 @@
         },
         "node_modules/utila": {
             "dev": true,
             "integrity": "sha512-Z0DbgELS9/L/75wZbro8xAnT50pBVFQZ+hUEueGDU5FN51YSCYM+jdxsfCiHjwNP/4LCDD0i/graKpeBnOXKRA==",
             "resolved": "https://registry.npmjs.org/utila/-/utila-0.4.0.tgz",
             "version": "0.4.0"
         },
-        "node_modules/utils-copy": {
-            "dependencies": {
-                "const-pinf-float64": "^1.0.0",
-                "object-keys": "^1.0.9",
-                "type-name": "^2.0.0",
-                "utils-copy-error": "^1.0.0",
-                "utils-indexof": "^1.0.0",
-                "utils-regex-from-string": "^1.0.0",
-                "validate.io-array": "^1.0.3",
-                "validate.io-buffer": "^1.0.1",
-                "validate.io-nonnegative-integer": "^1.0.0"
-            },
-            "integrity": "sha512-+NhJVV+PcxjdpkMrVTqXhQHPldlFGca5XR9YnGyNn7kQ0fMi+DqNLzdnhJ4TJ1HNy/HzB7c+FPg3y+4icY99ZA==",
-            "resolved": "https://registry.npmjs.org/utils-copy/-/utils-copy-1.1.1.tgz",
-            "version": "1.1.1"
-        },
-        "node_modules/utils-copy-error": {
-            "dependencies": {
-                "object-keys": "^1.0.9",
-                "utils-copy": "^1.1.0"
-            },
-            "integrity": "sha512-RbJcGPZ6Ru2HQk9SWkvbdWNPX58pt4MO5uXsOQRu4LEGWB3LglkRrmnE/Ph1qWg6ywQ0qj95wTz1OeqQ2l8DCA==",
-            "resolved": "https://registry.npmjs.org/utils-copy-error/-/utils-copy-error-1.0.1.tgz",
-            "version": "1.0.1"
-        },
-        "node_modules/utils-indexof": {
-            "dependencies": {
-                "validate.io-array-like": "^1.0.1",
-                "validate.io-integer-primitive": "^1.0.0"
-            },
-            "integrity": "sha512-76QBfRJpn4A0P5uTO1x00x+Yog36w2Pab0n+aT9UfUvVa4l+e8k3p7YwNpDvfQ6+aKGZdxZpxcNotNS4YjFcyg==",
-            "resolved": "https://registry.npmjs.org/utils-indexof/-/utils-indexof-1.0.0.tgz",
-            "version": "1.0.0"
-        },
-        "node_modules/utils-regex-from-string": {
-            "dependencies": {
-                "regex-regex": "^1.0.0",
-                "validate.io-string-primitive": "^1.0.0"
-            },
-            "integrity": "sha512-xKfdmEF19iUu9TKxFiohQUlQTuqYdV80/CxHiudVI37iEV/OA4HHlXZoc4qvuO1B74EcBVpErBreRO/dpdLeYA==",
-            "resolved": "https://registry.npmjs.org/utils-regex-from-string/-/utils-regex-from-string-1.0.0.tgz",
-            "version": "1.0.0"
-        },
         "node_modules/validate-npm-package-license": {
             "dependencies": {
                 "spdx-correct": "^3.0.0",
                 "spdx-expression-parse": "^3.0.0"
             },
             "dev": true,
             "integrity": "sha512-DpKm2Ui/xN7/HQKCtpZxoRWBhZ9Z0kqtygG8XCgNQ8ZlDnxuQmWhj566j8fN4Cu3/JmbhsDo7fcAJq4s9h27Ew==",
             "resolved": "https://registry.npmjs.org/validate-npm-package-license/-/validate-npm-package-license-3.0.4.tgz",
             "version": "3.0.4"
         },
-        "node_modules/validate.io-array": {
-            "integrity": "sha512-DeOy7CnPEziggrOO5CZhVKJw6S3Yi7e9e65R1Nl/RTN1vTQKnzjfvks0/8kQ40FP/dsjRAOd4hxmJ7uLa6vxkg==",
-            "resolved": "https://registry.npmjs.org/validate.io-array/-/validate.io-array-1.0.6.tgz",
-            "version": "1.0.6"
-        },
-        "node_modules/validate.io-array-like": {
-            "dependencies": {
-                "const-max-uint32": "^1.0.2",
-                "validate.io-integer-primitive": "^1.0.0"
-            },
-            "integrity": "sha512-rGLiN0cvY9OWzQcWP+RtqZR/MK9RUz3gKDTCcRLtEQ/BvlanMF5PyqtVIN+CgrIBCv/ypfme9v7r4yMJPYpbNA==",
-            "resolved": "https://registry.npmjs.org/validate.io-array-like/-/validate.io-array-like-1.0.2.tgz",
-            "version": "1.0.2"
-        },
-        "node_modules/validate.io-buffer": {
-            "integrity": "sha512-6Tad+/QYOxWEXsesKYak1mHOzGdPYS4QeHFImWn7ECi4GR0x3vh7+6+1yoLKNXiklKuTFOxHLG3kZy9tPX0GvQ==",
-            "resolved": "https://registry.npmjs.org/validate.io-buffer/-/validate.io-buffer-1.0.2.tgz",
-            "version": "1.0.2"
-        },
-        "node_modules/validate.io-integer": {
-            "dependencies": {
-                "validate.io-number": "^1.0.3"
-            },
-            "integrity": "sha512-22izsYSLojN/P6bppBqhgUDjCkr5RY2jd+N2a3DCAUey8ydvrZ/OkGvFPR7qfOpwR2LC5p4Ngzxz36g5Vgr/hQ==",
-            "resolved": "https://registry.npmjs.org/validate.io-integer/-/validate.io-integer-1.0.5.tgz",
-            "version": "1.0.5"
-        },
-        "node_modules/validate.io-integer-primitive": {
-            "dependencies": {
-                "validate.io-number-primitive": "^1.0.0"
-            },
-            "integrity": "sha512-4ARGKA4FImVWJgrgttLYsYJmDGwxlhLfDCdq09gyVgohLKKRUfD3VAo1L2vTRCLt6hDhDtFKdZiuYUTWyBggwg==",
-            "resolved": "https://registry.npmjs.org/validate.io-integer-primitive/-/validate.io-integer-primitive-1.0.0.tgz",
-            "version": "1.0.0"
-        },
-        "node_modules/validate.io-matrix-like": {
-            "integrity": "sha512-86mqLUIkZCRAOVKZvpCB7sDCw1dKBjBkY+C6WO/wLo/jQx0sOqQZz3LLtDw0DCfuAKxRuhSmIpX3nzr0nWrbdw==",
-            "resolved": "https://registry.npmjs.org/validate.io-matrix-like/-/validate.io-matrix-like-1.0.2.tgz",
-            "version": "1.0.2"
-        },
-        "node_modules/validate.io-ndarray-like": {
-            "integrity": "sha512-OV85AosxraPFSXJwzv/d7Cu5/dLiyLtsHmxtHTJcHW1N0uscd0eJ2df1Zk+HdID0eUctUllW/1YuQPUJFv1pTA==",
-            "resolved": "https://registry.npmjs.org/validate.io-ndarray-like/-/validate.io-ndarray-like-1.0.0.tgz",
-            "version": "1.0.0"
-        },
-        "node_modules/validate.io-nonnegative-integer": {
-            "dependencies": {
-                "validate.io-integer": "^1.0.5"
-            },
-            "integrity": "sha512-uOMekPwcl84yg8NR7zgIZCZ9pHCtd9CK1Ri51N+ZJLTe1HyLbmdFdy7ZmfkiHkMvB1pOxeQmd1/LBjKhUD1L3A==",
-            "resolved": "https://registry.npmjs.org/validate.io-nonnegative-integer/-/validate.io-nonnegative-integer-1.0.0.tgz",
-            "version": "1.0.0"
-        },
-        "node_modules/validate.io-number": {
-            "integrity": "sha512-kRAyotcbNaSYoDnXvb4MHg/0a1egJdLwS6oJ38TJY7aw9n93Fl/3blIXdyYvPOp55CNxywooG/3BcrwNrBpcSg==",
-            "resolved": "https://registry.npmjs.org/validate.io-number/-/validate.io-number-1.0.3.tgz",
-            "version": "1.0.3"
-        },
-        "node_modules/validate.io-number-primitive": {
-            "integrity": "sha512-8rlCe7N0TRTd50dwk4WNoMXNbX/4+RdtqE3TO6Bk0GJvAgbQlfL5DGr/Pl9ZLbWR6CutMjE2cu+yOoCnFWk+Qw==",
-            "resolved": "https://registry.npmjs.org/validate.io-number-primitive/-/validate.io-number-primitive-1.0.0.tgz",
-            "version": "1.0.0"
-        },
-        "node_modules/validate.io-positive-integer": {
-            "dependencies": {
-                "validate.io-integer": "^1.0.5"
-            },
-            "integrity": "sha512-eg4LSdyqjICNUZWRilcQ5l+YayRlu6yi+GQsWw1bCmtG9yayOPmLa1fPymEHPPhbvWPAv3w0LLbCsf03pBHZkg==",
-            "resolved": "https://registry.npmjs.org/validate.io-positive-integer/-/validate.io-positive-integer-1.0.0.tgz",
-            "version": "1.0.0"
-        },
-        "node_modules/validate.io-string-primitive": {
-            "integrity": "sha512-TORbkLMdOFkEbPtfdx76FSVQGSAzyUEMxI+pBq5pfFm1ZzIesP+XiGc6eIK75aKu7RA7a8EcqUv5OrY5wfog5w==",
-            "resolved": "https://registry.npmjs.org/validate.io-string-primitive/-/validate.io-string-primitive-1.0.1.tgz",
-            "version": "1.0.1"
-        },
         "node_modules/vt-pbf": {
             "dependencies": {
                 "@mapbox/point-geometry": "0.1.0",
                 "@mapbox/vector-tile": "^1.3.1",
                 "pbf": "^3.2.1"
             },
             "integrity": "sha512-2LzDFzt0mZKZ9IpVF2r69G9bXaP2Q2sArJCmcCgvfTdCCZzSyz4aCLoQyUilu37Ll56tCblIZrXFIjNUpGIlmA==",
@@ -8993,59 +8798,59 @@
             "dependencies": {
                 "@types/eslint-scope": "^3.7.3",
                 "@types/estree": "^1.0.0",
                 "@webassemblyjs/ast": "^1.11.5",
                 "@webassemblyjs/wasm-edit": "^1.11.5",
                 "@webassemblyjs/wasm-parser": "^1.11.5",
                 "acorn": "^8.7.1",
-                "acorn-import-assertions": "^1.7.6",
+                "acorn-import-assertions": "^1.9.0",
                 "browserslist": "^4.14.5",
                 "chrome-trace-event": "^1.0.2",
-                "enhanced-resolve": "^5.13.0",
+                "enhanced-resolve": "^5.15.0",
                 "es-module-lexer": "^1.2.1",
                 "eslint-scope": "5.1.1",
                 "events": "^3.2.0",
                 "glob-to-regexp": "^0.4.1",
                 "graceful-fs": "^4.2.9",
                 "json-parse-even-better-errors": "^2.3.1",
                 "loader-runner": "^4.2.0",
                 "mime-types": "^2.1.27",
                 "neo-async": "^2.6.2",
-                "schema-utils": "^3.1.2",
+                "schema-utils": "^3.2.0",
                 "tapable": "^2.1.1",
                 "terser-webpack-plugin": "^5.3.7",
                 "watchpack": "^2.4.0",
                 "webpack-sources": "^3.2.3"
             },
             "dev": true,
             "engines": {
                 "node": ">=10.13.0"
             },
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/webpack"
             },
-            "integrity": "sha512-AAjaJ9S4hYCVODKLQTgG5p5e11hiMawBwV2v8MYLE0C/6UAGLuAF4n1qa9GOwdxnicaP+5k6M5HrLmD4+gIB8Q==",
+            "integrity": "sha512-JmcgNZ1iKj+aiR0OvTYtWQqJwq37Pf683dY9bVORwVbUrDhLhdn/PlO2sHsFHPkj7sHNQF3JwaAkp49V+Sq1tQ==",
             "peerDependenciesMeta": {
                 "webpack-cli": {
                     "optional": true
                 }
             },
-            "resolved": "https://registry.npmjs.org/webpack/-/webpack-5.81.0.tgz",
-            "version": "5.81.0"
+            "resolved": "https://registry.npmjs.org/webpack/-/webpack-5.88.2.tgz",
+            "version": "5.88.2"
         },
         "node_modules/webpack-cli": {
             "bin": {
                 "webpack-cli": "bin/cli.js"
             },
             "dependencies": {
                 "@discoveryjs/json-ext": "^0.5.0",
-                "@webpack-cli/configtest": "^2.0.1",
-                "@webpack-cli/info": "^2.0.1",
-                "@webpack-cli/serve": "^2.0.2",
+                "@webpack-cli/configtest": "^2.1.1",
+                "@webpack-cli/info": "^2.0.2",
+                "@webpack-cli/serve": "^2.0.5",
                 "colorette": "^2.0.14",
                 "commander": "^10.0.1",
                 "cross-spawn": "^7.0.3",
                 "envinfo": "^7.7.3",
                 "fastest-levenshtein": "^1.0.12",
                 "import-local": "^3.0.2",
                 "interpret": "^3.1.1",
@@ -9056,31 +8861,31 @@
             "engines": {
                 "node": ">=14.15.0"
             },
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/webpack"
             },
-            "integrity": "sha512-4y3W5Dawri5+8dXm3+diW6Mn1Ya+Dei6eEVAdIduAmYNLzv1koKVAqsfgrrc9P2mhrYHQphx5htnGkcNwtubyQ==",
+            "integrity": "sha512-pIDJHIEI9LR0yxHXQ+Qh95k2EvXpWzZ5l+d+jIo+RdSm9MiHfzazIxwwni/p7+x4eJZuvG1AJwgC4TNQ7NRgsg==",
             "peerDependencies": {
                 "webpack": "5.x.x"
             },
             "peerDependenciesMeta": {
                 "@webpack-cli/generators": {
                     "optional": true
                 },
                 "webpack-bundle-analyzer": {
                     "optional": true
                 },
                 "webpack-dev-server": {
                     "optional": true
                 }
             },
-            "resolved": "https://registry.npmjs.org/webpack-cli/-/webpack-cli-5.0.2.tgz",
-            "version": "5.0.2"
+            "resolved": "https://registry.npmjs.org/webpack-cli/-/webpack-cli-5.1.4.tgz",
+            "version": "5.1.4"
         },
         "node_modules/webpack-cli/node_modules/commander": {
             "dev": true,
             "engines": {
                 "node": ">=14"
             },
             "integrity": "sha512-y4Mg2tXshplEbSGzx7amzPwKKOCGuoSRP/CjEdwwk0FOGlUbq6lKuoyDZTNZkmxHdJtp54hdfY/JUrdL7Xfdug==",
@@ -9092,17 +8897,17 @@
                 "clone-deep": "^4.0.1",
                 "wildcard": "^2.0.0"
             },
             "dev": true,
             "engines": {
                 "node": ">=10.0.0"
             },
-            "integrity": "sha512-/SaI7xY0831XwP6kzuwhKWVKDP9t1QY1h65lAFLbZqMPIuYcD9QAW4u9STIbU9kaJbPBB/geU/gLr1wDjOhQ+Q==",
-            "resolved": "https://registry.npmjs.org/webpack-merge/-/webpack-merge-5.8.0.tgz",
-            "version": "5.8.0"
+            "integrity": "sha512-6NbRQw4+Sy50vYNTw7EyOn41OZItPiXB8GNv3INSoe3PSFaHJEz3SHTrYVaRm2LilNGnFUzh0FAwqPEmU/CwDg==",
+            "resolved": "https://registry.npmjs.org/webpack-merge/-/webpack-merge-5.9.0.tgz",
+            "version": "5.9.0"
         },
         "node_modules/webpack-sources": {
             "dev": true,
             "engines": {
                 "node": ">=10.13.0"
             },
             "integrity": "sha512-/DyMEOrDgLKKIG0fmvtz+4dUX/3Ghozwgm6iPp8KRhvn+eQf9+Q7GWxVNMk3+uCPWfdXYC4ExGBckIXdFEfH1w==",
@@ -9164,27 +8969,26 @@
         },
         "node_modules/which-typed-array": {
             "dependencies": {
                 "available-typed-arrays": "^1.0.5",
                 "call-bind": "^1.0.2",
                 "for-each": "^0.3.3",
                 "gopd": "^1.0.1",
-                "has-tostringtag": "^1.0.0",
-                "is-typed-array": "^1.1.10"
+                "has-tostringtag": "^1.0.0"
             },
             "dev": true,
             "engines": {
                 "node": ">= 0.4"
             },
             "funding": {
                 "url": "https://github.com/sponsors/ljharb"
             },
-            "integrity": "sha512-w9c4xkx6mPidwp7180ckYWfMmvxpjlZuIudNtDf4N/tTAUB8VJbX25qZoAsrtGuYNnGw3pa0AXgbGKRB8/EceA==",
-            "resolved": "https://registry.npmjs.org/which-typed-array/-/which-typed-array-1.1.9.tgz",
-            "version": "1.1.9"
+            "integrity": "sha512-qe9UWWpkeG5yzZ0tNYxDmd7vo58HDBc39mZ0xWWpolAGADdFOzkfamWLDxkOWcvHQKVmdTyQdLD4NOfjLWTKew==",
+            "resolved": "https://registry.npmjs.org/which-typed-array/-/which-typed-array-1.1.11.tgz",
+            "version": "1.1.11"
         },
         "node_modules/wide-align": {
             "dependencies": {
                 "string-width": "^1.0.2 || 2 || 3 || 4"
             },
             "dev": true,
             "integrity": "sha512-eDMORYaPNZ4sQIuuYPDHdQvf4gyCF9rEEV/yPxGfwPkRodwEgiMUUXTx/dex+Me0wxx53S+NgUHaP7y3MGlDmg==",
@@ -9197,17 +9001,17 @@
             "resolved": "https://registry.npmjs.org/wildcard/-/wildcard-2.0.1.tgz",
             "version": "2.0.1"
         },
         "node_modules/word-wrap": {
             "engines": {
                 "node": ">=0.10.0"
             },
-            "integrity": "sha512-Hz/mrNwitNRh/HUAtM/VT/5VH+ygD6DV7mYKZAtHOrbs8U7lvPS6xf7EJKMF0uW1KJCl0H701g3ZGus+muE5vQ==",
-            "resolved": "https://registry.npmjs.org/word-wrap/-/word-wrap-1.2.3.tgz",
-            "version": "1.2.3"
+            "integrity": "sha512-BN22B5eaMMI9UMtjrGd5g5eCYPpCPDUy0FJXbYsaT5zYxjFOckS53SQDE3pWkVoWpHXVb3BrYcEN4Twa55B5cA==",
+            "resolved": "https://registry.npmjs.org/word-wrap/-/word-wrap-1.2.5.tgz",
+            "version": "1.2.5"
         },
         "node_modules/world-calendars": {
             "dependencies": {
                 "object-assign": "^4.1.0"
             },
             "integrity": "sha512-sAjLZkBnsbHkHWVhrsCU5Sa/EVuf9QqgvrN8zyJ2L/F9FR9Oc6CvVK0674+PGAtmmmYQMH98tCUSO4QLQv3/TQ==",
             "resolved": "https://registry.npmjs.org/world-calendars/-/world-calendars-1.0.3.tgz",
```

### Comparing `munin-plot-1.6/package.json` & `munin-plot-1.7/package.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9722222222222221%*

 * *Differences: {"'dependencies'": "{'bootstrap': '^5.3.1', 'd3': '^7.8.5', 'jquery': '^3.7.0', 'plotly.js': "*

 * *                   "'^2.25.0'}",*

 * * "'devDependencies'": "{'css-loader': '^6.8.1', 'eslint': '^8.46.0', 'eslint-config-standard': "*

 * *                      "'^17.1.0', 'eslint-plugin-import': '^2.28.0', 'html-webpack-plugin': "*

 * *                      "'^5.5.3', 'mini-css-extract-plugin': '^2.7.6', 'postcss-loader': '^7.3.3', "*

 * *                      "'sass-loader': '^13.3.2', 'style-loader': '^3.3.3', 'webpack': '^5.88. […]*

```diff
@@ -1,39 +1,39 @@
 {
     "author": "Arthur de Jong <arthur@arthurdejong.org> (https://arthurdejong.org/)",
     "dependencies": {
         "@fortawesome/fontawesome-free": "^6.4.0",
-        "bootstrap": "^5.2.3",
-        "d3": "^7.8.4",
+        "bootstrap": "^5.3.1",
+        "d3": "^7.8.5",
         "daterangepicker": "^3.1.0",
-        "jquery": "^3.6.4",
+        "jquery": "^3.7.0",
         "jquery-ui": "^1.13.2",
         "pako": "^2.1.0",
-        "plotly.js": "^2.22.0"
+        "plotly.js": "^2.25.0"
     },
     "description": "Alternative web front-end for Munin",
     "devDependencies": {
         "archiver": "^5.3.1",
         "autoprefixer": "^10.4.14",
-        "css-loader": "^6.7.3",
-        "eslint": "^8.39.0",
-        "eslint-config-standard": "^17.0.0",
-        "eslint-plugin-import": "^2.27.5",
+        "css-loader": "^6.8.1",
+        "eslint": "^8.46.0",
+        "eslint-config-standard": "^17.1.0",
+        "eslint-plugin-import": "^2.28.0",
         "eslint-plugin-node": "^11.1.0",
         "eslint-plugin-promise": "^6.1.1",
         "file-loader": "^6.2.0",
         "html-loader": "^4.2.0",
-        "html-webpack-plugin": "^5.5.1",
-        "mini-css-extract-plugin": "^2.7.5",
+        "html-webpack-plugin": "^5.5.3",
+        "mini-css-extract-plugin": "^2.7.6",
         "node-sass": "^8.0.0",
-        "postcss-loader": "^7.3.0",
-        "sass-loader": "^13.2.2",
-        "style-loader": "^3.3.2",
-        "webpack": "^5.81.0",
-        "webpack-cli": "^5.0.2"
+        "postcss-loader": "^7.3.3",
+        "sass-loader": "^13.3.2",
+        "style-loader": "^3.3.3",
+        "webpack": "^5.88.2",
+        "webpack-cli": "^5.1.4"
     },
     "homepage": "https://arthurdejong.org/munin-plot/",
     "license": "MIT",
     "name": "@arthurdejong/munin-plot",
     "private": true,
     "scripts": {
         "build": "webpack --mode production",
```

### Comparing `munin-plot-1.6/setup.cfg` & `munin-plot-1.7/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [metadata]
 name = munin-plot
-version = 1.6
+version = 1.7
 description = Alternative web front-end for Munin
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Arthur de Jong
 author_email = arthur@arthurdejong.org
 url = https://arthurdejong.org/munin-plot/
 license = MIT
-license_file = COPYING
+license_files = COPYING
 classifiers = 
 	Development Status :: 3 - Alpha
 	Environment :: Web Environment
 	Intended Audience :: Developers
 	Intended Audience :: System Administrators
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
```

### Comparing `munin-plot-1.6/setup.py` & `munin-plot-1.7/setup.py`

 * *Files identical despite different names*

### Comparing `munin-plot-1.6/src/apple-touch-icon.png` & `munin-plot-1.7/src/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `munin-plot-1.6/src/favicon-32x32.png` & `munin-plot-1.7/src/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `munin-plot-1.6/src/favicon-64x64.png` & `munin-plot-1.7/src/favicon-64x64.png`

 * *Files identical despite different names*

### Comparing `munin-plot-1.6/src/favicon.ico` & `munin-plot-1.7/src/favicon.ico`

 * *Files identical despite different names*

### Comparing `munin-plot-1.6/src/index.html` & `munin-plot-1.7/src/index.html`

 * *Files 4% similar despite different names*

```diff
@@ -75,15 +75,22 @@
               <span class="sizesm sizeactive" title="small graph"></span>
               <span class="sizemd" title="medium graph"></span>
               <span class="sizelg" title="large graph"></span>
               <span class="closegraph" title="close"><i class="fa fa-window-close"></i></span>
             </div>
             <div class="card-rightbody">
               <div class="container-fluid px-0">
-                <div class="row graphtitle small"></div>
+                <div class="row small">
+                  <div class="col graphtitle"></div>
+                  <div class="col text-end">
+                    <span class="selectall mx-2" title="Select all"><i class="fa-solid fa-circle-check fa-xs"></i></span>
+                    <span class="selecttoggle mx-2" title="Toggle selection"><i class="fa-solid fa-circle-half-stroke fa-xs"></i></span>
+                    <span class="selectnone mx-2" title="Select none"><i class="fa-regular fa-circle fa-xs"></i></span>
+                  </div>
+                </div>
                 <div class="row">
                   <div class="myplot col col-8">
                     <div class="loading loading-small"></div>
                   </div>
                   <div class="mylegend col col-4">
                     <table class="table table-sm table-hover">
                       <thead>
```

#### html2text {}

```diff
@@ -7,14 +7,15 @@
   [munin-plot] munin-plot
 
   Dashboards
 
 
 **** LOADING ****
     *
+
 [                    ] [One of: All hosts] [One of: All categories]
 ** Load dashboard **
 [File]
 Load
 ** Save dashboard **
 Name
 [                    ]
```

### Comparing `munin-plot-1.6/src/logo.png` & `munin-plot-1.7/src/logo.png`

 * *Files identical despite different names*

### Comparing `munin-plot-1.6/src/munin-plot.css` & `munin-plot-1.7/src/munin-plot.css`

 * *Files identical despite different names*

### Comparing `munin-plot-1.6/src/munin-plot.js` & `munin-plot-1.7/src/munin-plot.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -345,17 +345,17 @@
     // add a graph to the list of graphs
     function addGraph(graph, size = 'sm') {
         const clone = $('#template>:first-child').clone()
         const plot = clone.find('.myplot')[0]
         const legend = clone.find('.mylegend')
         plot.graph = graph
         // update graph title
-        clone.find('.graphtitle').append($('<div>').addClass('col').text(graph.host + ' / ')
+        clone.find('.graphtitle').text(graph.host + ' / ')
             .append($('<b>').text(graph.graph_title))
-            .attr('title', graph.graph_info || ''))
+            .attr('title', graph.graph_info || '')
         // set the size changing actions
         clone.find('.sizesm').click(function() {
             clone.find('.sizeactive').removeClass('sizeactive')
             $(this).addClass('sizeactive')
             $(plot).addClass('plot-sm').removeClass('plot-md plot-lg')
             legend.addClass('legend-sm').removeClass('legend-md legend-lg')
             Plotly.relayout(plot, {})
@@ -382,14 +382,70 @@
             clone.hide(400, function() {
                 Plotly.purge(plot)
                 $(this).remove()
                 // after any changes, save the current list of graphs
                 saveCurrentGraphs()
             })
         })
+        // set the selection changing actions
+        clone.find('.selectall').click(function() {
+            if (plot.data) {
+                traces.slice().reverse().forEach(function(trace) {
+                    if (trace.showlegend !== false) {
+                        plot.legendbyfield[trace.field_name].style.opacity = 1
+                        plot.data.forEach(function(t) {
+                            if (t.field_name === trace.field_name) {
+                                t.visible = true
+                            }
+                        })
+                    }
+                })
+                saveCurrentGraphs()
+                Plotly.newPlot(plot, plot.data, plot.layout, plot.config)
+            }
+        })
+        clone.find('.selecttoggle').click(function() {
+            if (plot.data) {
+                traces.slice().reverse().forEach(function(trace) {
+                    if (trace.showlegend !== false) {
+                        const visible = (trace.visible === false)
+                        plot.legendbyfield[trace.field_name].style.opacity = visible ? 1 : 0.2
+                        plot.data.forEach(function(t) {
+                            if (t.field_name === trace.field_name) {
+                                t.visible = visible
+                            }
+                        })
+                    }
+                })
+                saveCurrentGraphs()
+                Plotly.newPlot(plot, plot.data, plot.layout, plot.config)
+            }
+        })
+        clone.find('.selectnone').click(function() {
+            if (plot.data) {
+                traces.slice().reverse().forEach(function(trace) {
+                    if (trace.field_name === 'idle') {
+                        console.log(trace)
+                        console.log(trace.name, trace.field_name, trace.visible)
+                    }
+                })
+                traces.slice().reverse().forEach(function(trace) {
+                    if (trace.showlegend !== false) {
+                        plot.legendbyfield[trace.field_name].style.opacity = 0.2
+                        plot.data.forEach(function(t) {
+                            if (t.field_name === trace.field_name) {
+                                t.visible = false
+                            }
+                        })
+                    }
+                })
+                saveCurrentGraphs()
+                Plotly.newPlot(plot, plot.data, plot.layout, plot.config)
+            }
+        })
         // set the wanted size
         $(plot).addClass('plot-' + size)
         legend.addClass('legend-' + size)
         clone.find('.sizeactive').removeClass('sizeactive')
         clone.find('.size' + size).addClass('sizeactive')
         // prepare the graph configuration
         const layout = JSON.parse(JSON.stringify(baseLayout))
@@ -477,15 +533,15 @@
         })
         // if there are too many traces only hover on the nearest
         if (traces.filter(trace => trace.showlegend !== false).length > 6) {
             layout.hovermode = 'closest'
         }
         // build the legend
         plot.legendbyfield = {}
-        traces.slice().reverse().forEach(function(trace) {
+        traces.slice().forEach(function(trace) {
             if (trace.showlegend !== false) {
                 const legendrow = $('<tr></tr>')
                 legendrow.append($('<td style="width: 20px;"><svg height="10" width="10"><line x1="0" y1="5" x2="10" y2="5"></svg></td>'))
                 legendrow.append($('<td><span></span></td>'))
                 legendrow.append($('<td></td>'))
                 legendrow.append($('<td></td>'))
                 legendrow.append($('<td></td>'))
@@ -504,15 +560,34 @@
                         $(this).css('opacity', visible ? 1 : 0.2)
                         plot.data.forEach(function(t) {
                             if (t.field_name === trace.field_name) {
                                 t.visible = visible
                             }
                         })
                         saveCurrentGraphs()
-                        Plotly.redraw(plot)
+                        Plotly.newPlot(plot, plot.data, plot.layout, plot.config)
+                    }
+                })
+                // hide all other traces on double click
+                legendrow.on('dblclick', function() {
+                    if (plot.data) {
+                        const selected = trace
+                        traces.slice().forEach(function(trace) {
+                            if (trace.showlegend !== false) {
+                                const visible = (trace.field_name === selected.field_name)
+                                plot.legendbyfield[trace.field_name].style.opacity = visible ? 1 : 0.2
+                                plot.data.forEach(function(t) {
+                                    if (t.field_name === trace.field_name) {
+                                        t.visible = visible
+                                    }
+                                })
+                            }
+                        })
+                        saveCurrentGraphs()
+                        Plotly.newPlot(plot, plot.data, plot.layout, plot.config)
                     }
                 })
                 // highlight the trace by lowering the opacity of the others traces
                 legendrow.mouseover(function() {
                     if (plot.data) {
                         Plotly.restyle(plot, 'opacity', plot.data.map(
                             t => t.field_name === trace.field_name ? 1 : 0.1))
```

### Comparing `munin-plot-1.6/tox.ini` & `munin-plot-1.7/tox.ini`

 * *Files identical despite different names*

### Comparing `munin-plot-1.6/webpack-plugins/zip-plugin.js` & `munin-plot-1.7/webpack-plugins/zip-plugin.js`

 * *Files identical despite different names*

### Comparing `munin-plot-1.6/webpack.config.js` & `munin-plot-1.7/webpack.config.js`

 * *Files identical despite different names*

