# Comparing `tmp/cookies_utilities-0.0.2.tar.gz` & `tmp/cookies_utilities-0.0.3.tar.gz`

## Comparing `cookies_utilities-0.0.2.tar` & `cookies_utilities-0.0.3.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/.readthedocs.yaml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/Makefile
--rwxr-xr-x   0        0        0      804 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/make.bat
--rw-r--r--   0        0        0    25667 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/doctrees/cookies_utilities.doctree
--rw-r--r--   0        0        0    59389 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/doctrees/environment.pickle
--rw-r--r--   0        0        0     5322 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/doctrees/index.doctree
--rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/doctrees/modules.doctree
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/.buildinfo
--rw-r--r--   0        0        0    17149 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/cookies_utilities.html
--rw-r--r--   0        0        0     4732 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/genindex.html
--rw-r--r--   0        0        0     5460 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/index.html
--rw-r--r--   0        0        0     4993 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/modules.html
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/objects.inv
--rw-r--r--   0        0        0     3941 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/search.html
--rw-r--r--   0        0        0     3386 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/searchindex.js
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_sources/cookies_utilities.rst.txt
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_sources/index.rst.txt
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_sources/modules.rst.txt
--rw-r--r--   0        0        0     4289 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--   0        0        0    15715 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/basic.css
--rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/doctools.js
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/documentation_options.js
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/file.png
--rw-r--r--   0        0        0    89501 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/jquery.js
--rw-r--r--   0        0        0     4957 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/language_data.js
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/minus.png
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/plus.png
--rw-r--r--   0        0        0     4892 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/pygments.css
--rw-r--r--   0        0        0    18215 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/searchtools.js
--rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/sphinx_highlight.js
--rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/css/badge_only.css
--rw-r--r--   0        0        0   135314 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/css/theme.css
--rw-r--r--   0        0        0    87624 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff
--rw-r--r--   0        0        0    67312 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
--rw-r--r--   0        0        0    86288 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff
--rw-r--r--   0        0        0    66444 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
--rw-r--r--   0        0        0   165742 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0        0        0   444379 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0        0        0   165548 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0        0        0    98024 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0        0        0    77160 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0        0        0   323344 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/lato-bold-italic.woff
--rw-r--r--   0        0        0   193308 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/lato-bold-italic.woff2
--rw-r--r--   0        0        0   309728 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/lato-bold.woff
--rw-r--r--   0        0        0   184912 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/lato-bold.woff2
--rw-r--r--   0        0        0   328412 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/lato-normal-italic.woff
--rw-r--r--   0        0        0   195704 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/lato-normal-italic.woff2
--rw-r--r--   0        0        0   309192 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/lato-normal.woff
--rw-r--r--   0        0        0   182708 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/lato-normal.woff2
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/js/badge_only.js
--rw-r--r--   0        0        0     4370 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/js/html5shiv-printshiv.min.js
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/js/html5shiv.min.js
--rw-r--r--   0        0        0     5023 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/build/html/_static/js/theme.js
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/source/conf.py
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/source/cookies_utilities.rst
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/source/index.rst
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/docs/source/modules.rst
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/src/cookies_utilities/__init__.py
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/src/cookies_utilities/stopwatch.py
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/tests/test_cookies_utilities.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/tests/test_stopwatch.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/LICENSE
--rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/README.md
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 cookies_utilities-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/.readthedocs.yaml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/docs/Makefile
+-rwxr-xr-x   0        0        0      804 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/docs/make.bat
+-rw-r--r--   0        0        0    43086 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/docs/build/doctrees/cookies_utilities.doctree
+-rw-r--r--   0        0        0    88903 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/docs/build/doctrees/environment.pickle
+-rw-r--r--   0        0        0     8899 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/docs/build/doctrees/index.doctree
+-rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/docs/build/doctrees/modules.doctree
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/docs/build/html/.buildinfo
+-rw-r--r--   0        0        0    28900 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/docs/build/html/cookies_utilities.html
+-rw-r--r--   0        0        0     5293 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/docs/build/html/genindex.html
+-rw-r--r--   0        0        0     6661 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/docs/build/html/index.html
+-rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/docs/build/html/modules.html
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/docs/build/html/objects.inv
+-rw-r--r--   0        0        0     3940 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/docs/build/html/search.html
+-rw-r--r--   0        0        0     5195 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/docs/build/html/searchindex.js
+-rw-r--r--   0        0        0     3592 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/docs/build/html/_sources/cookies_utilities.rst.txt
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/docs/build/html/_sources/index.rst.txt
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/docs/build/html/_sources/modules.rst.txt
+-rw-r--r--   0        0        0     4289 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js
+-rw-r--r--   0        0        0    15715 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/docs/build/html/_static/basic.css
+-rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/docs/build/html/_static/doctools.js
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/docs/build/html/_static/documentation_options.js
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/docs/build/html/_static/file.png
+-rw-r--r--   0        0        0    89501 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/docs/build/html/_static/jquery.js
+-rw-r--r--   0        0        0     4957 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/docs/build/html/_static/language_data.js
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/docs/build/html/_static/minus.png
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/docs/build/html/_static/plus.png
+-rw-r--r--   0        0        0     4892 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/docs/build/html/_static/pygments.css
+-rw-r--r--   0        0        0    18215 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/docs/build/html/_static/searchtools.js
+-rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/docs/build/html/_static/sphinx_highlight.js
+-rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/docs/build/html/_static/css/badge_only.css
+-rw-r--r--   0        0        0   135314 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/docs/build/html/_static/css/theme.css
+-rw-r--r--   0        0        0    87624 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-r--r--   0        0        0    67312 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-r--r--   0        0        0    86288 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-r--r--   0        0        0    66444 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-r--r--   0        0        0   165742 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/docs/build/html/_static/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0        0        0   444379 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/docs/build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0        0        0   165548 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0        0        0    98024 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/docs/build/html/_static/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0        0        0    77160 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0        0        0   323344 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/docs/build/html/_static/css/fonts/lato-bold-italic.woff
+-rw-r--r--   0        0        0   193308 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/docs/build/html/_static/css/fonts/lato-bold-italic.woff2
+-rw-r--r--   0        0        0   309728 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/docs/build/html/_static/css/fonts/lato-bold.woff
+-rw-r--r--   0        0        0   184912 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/docs/build/html/_static/css/fonts/lato-bold.woff2
+-rw-r--r--   0        0        0   328412 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/docs/build/html/_static/css/fonts/lato-normal-italic.woff
+-rw-r--r--   0        0        0   195704 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/docs/build/html/_static/css/fonts/lato-normal-italic.woff2
+-rw-r--r--   0        0        0   309192 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/docs/build/html/_static/css/fonts/lato-normal.woff
+-rw-r--r--   0        0        0   182708 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/docs/build/html/_static/css/fonts/lato-normal.woff2
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/docs/build/html/_static/js/badge_only.js
+-rw-r--r--   0        0        0     4370 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/docs/build/html/_static/js/html5shiv-printshiv.min.js
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/docs/build/html/_static/js/html5shiv.min.js
+-rw-r--r--   0        0        0     5023 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/docs/build/html/_static/js/theme.js
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/docs/source/conf.py
+-rw-r--r--   0        0        0     3592 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/docs/source/cookies_utilities.rst
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/docs/source/index.rst
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/docs/source/modules.rst
+-rw-r--r--   0        0        0     5699 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/src/cookies_utilities/__init__.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/src/cookies_utilities/stopwatch.py
+-rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/tests/test_cookies_utilities.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/tests/test_stopwatch.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/README.md
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 cookies_utilities-0.0.3/PKG-INFO
```

### Comparing `cookies_utilities-0.0.2/docs/Makefile` & `cookies_utilities-0.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.2/docs/make.bat` & `cookies_utilities-0.0.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.2/docs/build/doctrees/modules.doctree` & `cookies_utilities-0.0.3/docs/build/doctrees/modules.doctree`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.2/docs/build/html/cookies_utilities.html` & `cookies_utilities-0.0.3/docs/build/html/cookies_utilities.html`

 * *Files 25% similar despite different names*

```diff
@@ -37,22 +37,30 @@
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
 </div>
         </div><div class="wy-menu wy-menu-vertical" data-spy="affix" role="navigation" aria-label="Navigation menu">
-              <p class="caption" role="heading"><span class="caption-text">Contents:</span></p>
+              <p class="caption" role="heading"><span class="caption-text">Contents</span></p>
 <ul class="current">
 <li class="toctree-l1 current"><a class="current reference internal" href="#">Documentation</a><ul>
 <li class="toctree-l2"><a class="reference internal" href="#functions">Functions</a><ul>
+<li class="toctree-l3"><a class="reference internal" href="#cookies-utilities-copy-datetime">cookies_utilities.copy_datetime</a><ul>
+<li class="toctree-l4"><a class="reference internal" href="#cookies_utilities.copy_datetime"><code class="docutils literal notranslate"><span class="pre">copy_datetime()</span></code></a></li>
+</ul>
+</li>
 <li class="toctree-l3"><a class="reference internal" href="#cookies-utilities-get-dates">cookies_utilities.get_dates</a><ul>
 <li class="toctree-l4"><a class="reference internal" href="#cookies_utilities.get_dates"><code class="docutils literal notranslate"><span class="pre">get_dates()</span></code></a></li>
 </ul>
 </li>
+<li class="toctree-l3"><a class="reference internal" href="#cookies-utilities-convert-time-to-feature">cookies_utilities.convert_time_to_feature</a><ul>
+<li class="toctree-l4"><a class="reference internal" href="#cookies_utilities.convert_time_to_feature"><code class="docutils literal notranslate"><span class="pre">convert_time_to_feature()</span></code></a></li>
+</ul>
+</li>
 </ul>
 </li>
 <li class="toctree-l2"><a class="reference internal" href="#classes">Classes</a><ul>
 <li class="toctree-l3"><a class="reference internal" href="#cookies-utilities-stopwatch">cookies_utilities.Stopwatch</a><ul>
 <li class="toctree-l4"><a class="reference internal" href="#cookies_utilities.Stopwatch"><code class="docutils literal notranslate"><span class="pre">Stopwatch</span></code></a></li>
 </ul>
 </li>
@@ -86,29 +94,61 @@
           <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
            <div itemprop="articleBody">
              
   <section id="documentation">
 <h1>Documentation<a class="headerlink" href="#documentation" title="Permalink to this heading"></a></h1>
 <section id="functions">
 <h2>Functions<a class="headerlink" href="#functions" title="Permalink to this heading"></a></h2>
+<section id="cookies-utilities-copy-datetime">
+<h3>cookies_utilities.copy_datetime<a class="headerlink" href="#cookies-utilities-copy-datetime" title="Permalink to this heading"></a></h3>
+<dl class="py function">
+<dt class="sig sig-object py" id="cookies_utilities.copy_datetime">
+<span class="sig-prename descclassname"><span class="pre">cookies_utilities.</span></span><span class="sig-name descname"><span class="pre">copy_datetime</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">dt</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">options</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">{}</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#cookies_utilities.copy_datetime" title="Permalink to this definition"></a></dt>
+<dd><p>Create a copy of a datetime.datetime object.</p>
+<dl class="field-list simple">
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
+<dd class="field-odd"><ul class="simple">
+<li><p><strong>dt</strong> (<em>datetime.datetime</em>) – The original object.</p></li>
+<li><p><strong>options</strong> (<em>dict</em>) – If you wish to overwrite certain fields,
+please specify them using this dictionary (optional).
+The keys must be in [‘year’, ‘month’, ‘day’, ‘hour’, ‘minute’,
+‘second’, ‘microsecond’, ‘tzinfo’, ‘fold’].</p></li>
+</ul>
+</dd>
+<dt class="field-even">Return type<span class="colon">:</span></dt>
+<dd class="field-even"><p>datetime.datetime</p>
+</dd>
+</dl>
+</dd></dl>
+
+<p><strong>Example</strong></p>
+<div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="kn">import</span> <span class="nn">cookies_utilities</span> <span class="k">as</span> <span class="nn">cu</span>
+<span class="kn">import</span> <span class="nn">datetime</span>
+
+<span class="n">dt</span> <span class="o">=</span> <span class="n">datetime</span><span class="o">.</span><span class="n">datetime</span><span class="o">.</span><span class="n">strptime</span><span class="p">(</span><span class="s1">&#39;2016-07-01 02:15:00&#39;</span><span class="p">,</span> <span class="s1">&#39;%Y-%m-</span><span class="si">%d</span><span class="s1"> %H:%M:%S&#39;</span><span class="p">)</span>
+<span class="n">dt_copy</span> <span class="o">=</span> <span class="n">cu</span><span class="o">.</span><span class="n">copy_datetime</span><span class="p">(</span><span class="n">dt</span><span class="p">,</span> <span class="p">{</span><span class="s1">&#39;minute&#39;</span><span class="p">:</span> <span class="mi">0</span><span class="p">})</span>  <span class="c1"># --&gt; 2016-07-01 02:00:00</span>
+</pre></div>
+</div>
+</section>
 <section id="cookies-utilities-get-dates">
 <h3>cookies_utilities.get_dates<a class="headerlink" href="#cookies-utilities-get-dates" title="Permalink to this heading"></a></h3>
 <dl class="py function">
 <dt class="sig sig-object py" id="cookies_utilities.get_dates">
 <span class="sig-prename descclassname"><span class="pre">cookies_utilities.</span></span><span class="sig-name descname"><span class="pre">get_dates</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">start</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">'2016-07-01</span> <span class="pre">02:00:00'</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">end</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">'2016-07-02</span> <span class="pre">01:00:00'</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">format</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">'%Y-%m-%d</span> <span class="pre">%H:%M:%S'</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">delta</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">{'days':</span> <span class="pre">0,</span> <span class="pre">'hours':</span> <span class="pre">1,</span> <span class="pre">'minutes':</span> <span class="pre">0,</span> <span class="pre">'weeks':</span> <span class="pre">0}</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">geniter</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">cast_str</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">True</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">format_out</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#cookies_utilities.get_dates" title="Permalink to this definition"></a></dt>
 <dd><p>Returns a list of times from the ‘start’ time to the ‘end’ time,
-incremented by ‘delta’.</p>
+incremented by ‘delta’.
+Please ensure ‘delta’ is greater than or equal to 1 microsecond.</p>
 <p>If you’re using the result as an iterator, it is recommended to set <em>geniter=True</em>.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><strong>start</strong> (<em>string</em>) – Start time string.</p></li>
 <li><p><strong>end</strong> (<em>string</em>) – End time string (inclusive).</p></li>
 <li><p><strong>format</strong> (<em>string</em>) – Conversion format for datetime.strptime.</p></li>
-<li><p><strong>delta</strong> (<em>dict</em>) – Timedelta as args for datetime.timedelta.</p></li>
+<li><p><strong>delta</strong> (<em>dict</em>) – Timedelta as args for datetime.timedelta (&gt;= 1 microsecond).</p></li>
 <li><p><strong>geniter</strong> (<em>bool</em>) – Whether to return as a generator iterator (default <em>False</em>).</p></li>
 <li><p><strong>cast_str</strong> (<em>bool</em>) – Whether to convert output to string (default <em>True</em>).</p></li>
 <li><p><strong>format_out</strong> (<em>string</em>) – Conversion format for output (default same to <strong>format</strong>).</p></li>
 </ul>
 </dd>
 <dt class="field-even">Return type<span class="colon">:</span></dt>
 <dd class="field-even"><p>list (or generator iterator) of string (or datetime.datetime)</p>
@@ -153,14 +193,83 @@
 <div class="highlight-console notranslate"><div class="highlight"><pre><span></span><span class="go">&lt;class &#39;generator&#39;&gt;</span>
 <span class="go">2016/07/01</span>
 <span class="go">2016/07/02</span>
 <span class="go">2016/07/03</span>
 </pre></div>
 </div>
 </section>
+<section id="cookies-utilities-convert-time-to-feature">
+<h3>cookies_utilities.convert_time_to_feature<a class="headerlink" href="#cookies-utilities-convert-time-to-feature" title="Permalink to this heading"></a></h3>
+<dl class="py function">
+<dt class="sig sig-object py" id="cookies_utilities.convert_time_to_feature">
+<span class="sig-prename descclassname"><span class="pre">cookies_utilities.</span></span><span class="sig-name descname"><span class="pre">convert_time_to_feature</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">dt</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">format</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">'%Y-%m-%d</span> <span class="pre">%H:%M:%S'</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">period</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">'day'</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">ceiling</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#cookies_utilities.convert_time_to_feature" title="Permalink to this definition"></a></dt>
+<dd><p>Convert a time to a feature value between 0 and 1.
+The return feature value represents how much of a period has passed.</p>
+<p>For example, if the period is 1 day, a feature value of noon is 0.5.</p>
+<p>Note 1: When setting the period to a month, the cycle is considered as 31 days
+regardless of the actual number of days in that month. This is to ensure that
+the feature value for ‘the 5th day of any month’ is consistent.</p>
+<p>Note 2: When setting the period to a year, the cycle is considered as 366 days
+regardless of the actual number of days in that year. This is done to ensure that
+the feature value for ‘the 5th day of any year’ remains the same,
+regardless of the specific year.</p>
+<dl class="field-list simple">
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
+<dd class="field-odd"><ul class="simple">
+<li><p><strong>dt</strong> (<em>string</em>) – A time string.</p></li>
+<li><p><strong>format</strong> (<em>string</em>) – Conversion format for datetime.strptime.
+If you set this argument to None,
+we expect ‘dt’ to originally be datetime.datetime object.</p></li>
+<li><p><strong>period</strong> (<em>string</em>) – A time period to convert a time to a feature value.
+This must be in [‘year’, ‘month’, ‘week’, ‘day’, ‘hour’, ‘minute’, ‘second’].</p></li>
+<li><p><strong>ceiling</strong> (<em>string</em>) – If you want to round the time when calculating the feature value,
+specify the rounding granularity in this argument (optional).
+This must be in [‘year’, ‘month’, ‘day’, ‘hour’, ‘minute’, ‘second’].</p></li>
+</ul>
+</dd>
+<dt class="field-even">Return type<span class="colon">:</span></dt>
+<dd class="field-even"><p>float</p>
+</dd>
+</dl>
+</dd></dl>
+
+<div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="kn">import</span> <span class="nn">cookies_utilities</span> <span class="k">as</span> <span class="nn">cu</span>
+
+<span class="n">feature_value</span> <span class="o">=</span> <span class="n">cu</span><span class="o">.</span><span class="n">convert_time_to_feature</span><span class="p">(</span>
+    <span class="n">dt</span><span class="o">=</span><span class="s1">&#39;2023-01-02 03:40:50&#39;</span><span class="p">,</span> <span class="nb">format</span><span class="o">=</span><span class="s1">&#39;%Y-%m-</span><span class="si">%d</span><span class="s1"> %H:%M:%S&#39;</span><span class="p">,</span>
+    <span class="n">period</span><span class="o">=</span><span class="s1">&#39;day&#39;</span><span class="p">,</span> <span class="n">ceiling</span><span class="o">=</span><span class="s1">&#39;hour&#39;</span><span class="p">)</span>
+<span class="c1">#  --&gt; 0.125  ( 3:00 am is 12.5% of the day )</span>
+
+<span class="n">feature_value</span> <span class="o">=</span> <span class="n">cu</span><span class="o">.</span><span class="n">convert_time_to_feature</span><span class="p">(</span>
+    <span class="n">dt</span><span class="o">=</span><span class="s1">&#39;2023-01-02 03:40:50&#39;</span><span class="p">,</span> <span class="nb">format</span><span class="o">=</span><span class="s1">&#39;%Y-%m-</span><span class="si">%d</span><span class="s1"> %H:%M:%S&#39;</span><span class="p">,</span>
+    <span class="n">period</span><span class="o">=</span><span class="s1">&#39;year&#39;</span><span class="p">,</span> <span class="n">ceiling</span><span class="o">=</span><span class="s1">&#39;day&#39;</span><span class="p">)</span>
+<span class="c1">#  --&gt; 0.002732  ( 1.0 / 366.0 )</span>
+
+<span class="n">feature_value</span> <span class="o">=</span> <span class="n">cu</span><span class="o">.</span><span class="n">convert_time_to_feature</span><span class="p">(</span>
+    <span class="n">dt</span><span class="o">=</span><span class="s1">&#39;2023-01-02 03:40:50&#39;</span><span class="p">,</span> <span class="nb">format</span><span class="o">=</span><span class="s1">&#39;%Y-%m-</span><span class="si">%d</span><span class="s1"> %H:%M:%S&#39;</span><span class="p">,</span>
+    <span class="n">period</span><span class="o">=</span><span class="s1">&#39;month&#39;</span><span class="p">,</span> <span class="n">ceiling</span><span class="o">=</span><span class="s1">&#39;day&#39;</span><span class="p">)</span>
+<span class="c1">#  --&gt; 0.032258  ( 1.0 / 31.0 )</span>
+
+<span class="n">feature_value</span> <span class="o">=</span> <span class="n">cu</span><span class="o">.</span><span class="n">convert_time_to_feature</span><span class="p">(</span>
+    <span class="n">dt</span><span class="o">=</span><span class="s1">&#39;2023-01-02 03:40:50&#39;</span><span class="p">,</span> <span class="nb">format</span><span class="o">=</span><span class="s1">&#39;%Y-%m-</span><span class="si">%d</span><span class="s1"> %H:%M:%S&#39;</span><span class="p">,</span>
+    <span class="n">period</span><span class="o">=</span><span class="s1">&#39;week&#39;</span><span class="p">,</span> <span class="n">ceiling</span><span class="o">=</span><span class="s1">&#39;hour&#39;</span><span class="p">)</span>
+<span class="c1">#  --&gt; 0.017857  ( 0.125 / 7.0 )</span>
+
+<span class="n">feature_value</span> <span class="o">=</span> <span class="n">cu</span><span class="o">.</span><span class="n">convert_time_to_feature</span><span class="p">(</span>
+    <span class="n">dt</span><span class="o">=</span><span class="s1">&#39;2023-01-02 03:40:50&#39;</span><span class="p">,</span> <span class="nb">format</span><span class="o">=</span><span class="s1">&#39;%Y-%m-</span><span class="si">%d</span><span class="s1"> %H:%M:%S&#39;</span><span class="p">,</span>
+    <span class="n">period</span><span class="o">=</span><span class="s1">&#39;hour&#39;</span><span class="p">,</span> <span class="n">ceiling</span><span class="o">=</span><span class="s1">&#39;minute&#39;</span><span class="p">)</span>
+<span class="c1">#  --&gt; 0.666667  ( 40.0 / 60.0 )</span>
+
+<span class="n">feature_value</span> <span class="o">=</span> <span class="n">cu</span><span class="o">.</span><span class="n">convert_time_to_feature</span><span class="p">(</span>
+    <span class="n">dt</span><span class="o">=</span><span class="s1">&#39;2023-01-02 03:40:50&#39;</span><span class="p">,</span> <span class="nb">format</span><span class="o">=</span><span class="s1">&#39;%Y-%m-</span><span class="si">%d</span><span class="s1"> %H:%M:%S&#39;</span><span class="p">,</span>
+    <span class="n">period</span><span class="o">=</span><span class="s1">&#39;minute&#39;</span><span class="p">)</span>
+<span class="c1">#  --&gt; 0.833333  ( 50.0 / 60.0 )</span>
+</pre></div>
+</div>
+</section>
 </section>
 <section id="classes">
 <h2>Classes<a class="headerlink" href="#classes" title="Permalink to this heading"></a></h2>
 <section id="cookies-utilities-stopwatch">
 <h3>cookies_utilities.Stopwatch<a class="headerlink" href="#cookies-utilities-stopwatch" title="Permalink to this heading"></a></h3>
 <dl class="py class">
 <dt class="sig sig-object py" id="cookies_utilities.Stopwatch">
@@ -192,16 +301,16 @@
 <span class="c1"># train</span>
 <span class="n">sw</span><span class="o">.</span><span class="n">press</span><span class="p">(</span><span class="s1">&#39;train end&#39;</span><span class="p">)</span>
 <span class="c1"># test</span>
 <span class="n">sw</span><span class="o">.</span><span class="n">press</span><span class="p">(</span><span class="s1">&#39;test end&#39;</span><span class="p">)</span>
 <span class="n">sw</span><span class="o">.</span><span class="n">show</span><span class="p">()</span>
 </pre></div>
 </div>
-<div class="highlight-console notranslate"><div class="highlight"><pre><span></span><span class="go">time1(train start-train end): 2.000s</span>
-<span class="go">time2(train end-test end): 1.000s</span>
+<div class="highlight-console notranslate"><div class="highlight"><pre><span></span><span class="go">time1 (train start - train end): 2.000s</span>
+<span class="go">time2 (train end - test end): 1.000s</span>
 <span class="go">total: 3.000s</span>
 </pre></div>
 </div>
 </section>
 </section>
 </section>
```

#### html2text {}

```diff
@@ -2,41 +2,66 @@
 
 
 
 
 
 cookies_utilities
 [q                   ]
-Contents:
+Contents
     * Documentation
           o Functions
+                # cookies_utilities.copy_datetime
+                      # copy_datetime()
                 # cookies_utilities.get_dates
                       # get_dates()
+                # cookies_utilities.convert_time_to_feature
+                      # convert_time_to_feature()
           o Classes
                 # cookies_utilities.Stopwatch
                       # Stopwatch
    cookies_utilities
     * Documentation
     * View_page_source
 ===============================================================================
 ****** Documentationï ******
 ***** Functionsï *****
+**** cookies_utilities.copy_datetimeï ****
+  cookies_utilities.copy_datetime(dt, options={})ï
+      Create a copy of a datetime.datetime object.
+        Parameters:
+                * dt (datetime.datetime) â The original object.
+                * options (dict) â If you wish to overwrite certain fields,
+                  please specify them using this dictionary (optional). The
+                  keys must be in [âyearâ, âmonthâ, âdayâ,
+                  âhourâ, âminuteâ, âsecondâ, âmicrosecondâ,
+                  âtzinfoâ, âfoldâ].
+        Return type:
+            datetime.datetime
+Example
+import cookies_utilities as cu
+import datetime
+
+dt = datetime.datetime.strptime('2016-07-01 02:15:00', '%Y-%m-%d %H:%M:%S')
+dt_copy = cu.copy_datetime(dt, {'minute': 0})  # --> 2016-07-01 02:00:00
+
 **** cookies_utilities.get_datesï ****
   cookies_utilities.get_dates(start='2016-07-01 02:00:00', end='2016-07-02 01:
   00:00', format='%Y-%m-%d %H:%M:%S', delta={'days': 0, 'hours': 1, 'minutes':
   0, 'weeks': 0}, geniter=False, cast_str=True, format_out=None)ï
       Returns a list of times from the âstartâ time to the âendâ time,
-      incremented by âdeltaâ.
+      incremented by âdeltaâ. Please ensure âdeltaâ is greater than or
+      equal to 1 microsecond.
       If youâre using the result as an iterator, it is recommended to set
       geniter=True.
         Parameters:
                 * start (string) â Start time string.
                 * end (string) â End time string (inclusive).
                 * format (string) â Conversion format for datetime.strptime.
-                * delta (dict) â Timedelta as args for datetime.timedelta.
+                * delta (dict) â Timedelta as args for datetime.timedelta (>=
+                  1 microsecond).
                 * geniter (bool) â Whether to return as a generator iterator
                   (default False).
                 * cast_str (bool) â Whether to convert output to string
                   (default True).
                 * format_out (string) â Conversion format for output (default
                   same to format).
         Return type:
@@ -67,14 +92,76 @@
 for date in dates:
     print(date)
 <class 'generator'>
 2016/07/01
 2016/07/02
 2016/07/03
 
+**** cookies_utilities.convert_time_to_featureï ****
+  cookies_utilities.convert_time_to_feature(dt, format='%Y-%m-%d %H:%M:%S',
+  period='day', ceiling=None)ï
+      Convert a time to a feature value between 0 and 1. The return feature
+      value represents how much of a period has passed.
+      For example, if the period is 1 day, a feature value of noon is 0.5.
+      Note 1: When setting the period to a month, the cycle is considered as 31
+      days regardless of the actual number of days in that month. This is to
+      ensure that the feature value for âthe 5th day of any monthâ is
+      consistent.
+      Note 2: When setting the period to a year, the cycle is considered as 366
+      days regardless of the actual number of days in that year. This is done
+      to ensure that the feature value for âthe 5th day of any yearâ
+      remains the same, regardless of the specific year.
+        Parameters:
+                * dt (string) â A time string.
+                * format (string) â Conversion format for datetime.strptime.
+                  If you set this argument to None, we expect âdtâ to
+                  originally be datetime.datetime object.
+                * period (string) â A time period to convert a time to a
+                  feature value. This must be in [âyearâ, âmonthâ,
+                  âweekâ, âdayâ, âhourâ, âminuteâ,
+                  âsecondâ].
+                * ceiling (string) â If you want to round the time when
+                  calculating the feature value, specify the rounding
+                  granularity in this argument (optional). This must be in
+                  [âyearâ, âmonthâ, âdayâ, âhourâ,
+                  âminuteâ, âsecondâ].
+        Return type:
+            float
+import cookies_utilities as cu
+
+feature_value = cu.convert_time_to_feature(
+    dt='2023-01-02 03:40:50', format='%Y-%m-%d %H:%M:%S',
+    period='day', ceiling='hour')
+#  --> 0.125  ( 3:00 am is 12.5% of the day )
+
+feature_value = cu.convert_time_to_feature(
+    dt='2023-01-02 03:40:50', format='%Y-%m-%d %H:%M:%S',
+    period='year', ceiling='day')
+#  --> 0.002732  ( 1.0 / 366.0 )
+
+feature_value = cu.convert_time_to_feature(
+    dt='2023-01-02 03:40:50', format='%Y-%m-%d %H:%M:%S',
+    period='month', ceiling='day')
+#  --> 0.032258  ( 1.0 / 31.0 )
+
+feature_value = cu.convert_time_to_feature(
+    dt='2023-01-02 03:40:50', format='%Y-%m-%d %H:%M:%S',
+    period='week', ceiling='hour')
+#  --> 0.017857  ( 0.125 / 7.0 )
+
+feature_value = cu.convert_time_to_feature(
+    dt='2023-01-02 03:40:50', format='%Y-%m-%d %H:%M:%S',
+    period='hour', ceiling='minute')
+#  --> 0.666667  ( 40.0 / 60.0 )
+
+feature_value = cu.convert_time_to_feature(
+    dt='2023-01-02 03:40:50', format='%Y-%m-%d %H:%M:%S',
+    period='minute')
+#  --> 0.833333  ( 50.0 / 60.0 )
+
 ***** Classesï *****
 **** cookies_utilities.Stopwatchï ****
   classcookies_utilities.Stopwatchï
       Stopwatch for measuring processing time.
         press(key='')ï
             Press the stopwatch.
               Parameters:
@@ -86,15 +173,15 @@
 sw = cu.Stopwatch()
 sw.press('train start')
 # train
 sw.press('train end')
 # test
 sw.press('test end')
 sw.show()
-time1(train start-train end): 2.000s
-time2(train end-test end): 1.000s
+time1 (train start - train end): 2.000s
+time2 (train end - test end): 1.000s
 total: 3.000s
 
 Previous
 ===============================================================================
 © Copyright 2023, CookieBox26.
 Built with Sphinx using a theme provided by Read_the_Docs.
```

### Comparing `cookies_utilities-0.0.2/docs/build/html/genindex.html` & `cookies_utilities-0.0.3/docs/build/html/genindex.html`

 * *Files 10% similar despite different names*

```diff
@@ -35,15 +35,15 @@
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
 </div>
         </div><div class="wy-menu wy-menu-vertical" data-spy="affix" role="navigation" aria-label="Navigation menu">
-              <p class="caption" role="heading"><span class="caption-text">Contents:</span></p>
+              <p class="caption" role="heading"><span class="caption-text">Contents</span></p>
 <ul>
 <li class="toctree-l1"><a class="reference internal" href="cookies_utilities.html">Documentation</a></li>
 </ul>
 
         </div>
       </div>
     </nav>
@@ -67,19 +67,32 @@
           <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
            <div itemprop="articleBody">
              
 
 <h1 id="index">Index</h1>
 
 <div class="genindex-jumpbox">
- <a href="#G"><strong>G</strong></a>
+ <a href="#C"><strong>C</strong></a>
+ | <a href="#G"><strong>G</strong></a>
  | <a href="#P"><strong>P</strong></a>
  | <a href="#S"><strong>S</strong></a>
  
 </div>
+<h2 id="C">C</h2>
+<table style="width: 100%" class="indextable genindextable"><tr>
+  <td style="width: 33%; vertical-align: top;"><ul>
+      <li><a href="cookies_utilities.html#cookies_utilities.convert_time_to_feature">convert_time_to_feature() (in module cookies_utilities)</a>
+</li>
+  </ul></td>
+  <td style="width: 33%; vertical-align: top;"><ul>
+      <li><a href="cookies_utilities.html#cookies_utilities.copy_datetime">copy_datetime() (in module cookies_utilities)</a>
+</li>
+  </ul></td>
+</tr></table>
+
 <h2 id="G">G</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="cookies_utilities.html#cookies_utilities.get_dates">get_dates() (in module cookies_utilities)</a>
 </li>
   </ul></td>
 </tr></table>
```

#### html2text {}

```diff
@@ -1,21 +1,24 @@
 
 
 
 
 
 cookies_utilities
 [q                   ]
-Contents:
+Contents
     * Documentation
    cookies_utilities
     * Index
 ===============================================================================
 ****** Index ******
-G | P | S
+C | G | P | S
+***** C *****
+    * convert_time_to_feature()_(in_module     * copy_datetime()_(in_module
+      cookies_utilities)                         cookies_utilities)
 ***** G *****
     * get_dates()_(in_module_cookies_utilities)
 ***** P *****
     * press()_(cookies_utilities.Stopwatch_method)
 ***** S *****
     * show()_(cookies_utilities.Stopwatch     * Stopwatch_(class_in
       method)                                   cookies_utilities)
```

### Comparing `cookies_utilities-0.0.2/docs/build/html/index.html` & `cookies_utilities-0.0.3/docs/build/html/index.html`

 * *Files 11% similar despite different names*

```diff
@@ -37,15 +37,15 @@
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
 </div>
         </div><div class="wy-menu wy-menu-vertical" data-spy="affix" role="navigation" aria-label="Navigation menu">
-              <p class="caption" role="heading"><span class="caption-text">Contents:</span></p>
+              <p class="caption" role="heading"><span class="caption-text">Contents</span></p>
 <ul>
 <li class="toctree-l1"><a class="reference internal" href="cookies_utilities.html">Documentation</a></li>
 </ul>
 
         </div>
       </div>
     </nav>
@@ -68,33 +68,47 @@
   <hr/>
 </div>
           <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
            <div itemprop="articleBody">
              
   <section id="welcome-to-cookies-utilities-documentation">
 <h1>Welcome to cookies_utilities’ documentation!<a class="headerlink" href="#welcome-to-cookies-utilities-documentation" title="Permalink to this heading"></a></h1>
-<section id="links">
-<h2>Links<a class="headerlink" href="#links" title="Permalink to this heading"></a></h2>
-<ul class="simple">
-<li><p><a class="reference external" href="https://pypi.org/project/cookies-utilities/">PyPI</a></p></li>
-<li><p><a class="reference external" href="https://github.com/CookieBox26/cookies_utilities">GitHub</a></p></li>
-</ul>
+<p>This package is intended to provide useful functions and classes. Please see <a class="reference internal" href="cookies_utilities.html"><span class="doc">Documentation</span></a>.</p>
+<section id="installation">
+<h2>Installation<a class="headerlink" href="#installation" title="Permalink to this heading"></a></h2>
+<p>You can install the release version from <a class="reference external" href="https://pypi.org/project/cookies-utilities/">PyPI</a>.</p>
+<div class="highlight-console notranslate"><div class="highlight"><pre><span></span><span class="go">pip install cookies_utilities</span>
+</pre></div>
+</div>
+<p>If you want to use the latest version that has not been released, clone <a class="reference external" href="https://github.com/CookieBox26/cookies_utilities">our GitHub repository</a> and install from the local directory.</p>
+<div class="highlight-console notranslate"><div class="highlight"><pre><span></span><span class="go">git clone https://github.com/CookieBox26/cookies_utilities.git</span>
+<span class="go">cd cookies_utilities</span>
+<span class="go">pip install .</span>
+</pre></div>
+</div>
 <div class="toctree-wrapper compound">
-<p class="caption" role="heading"><span class="caption-text">Contents:</span></p>
+<p class="caption" role="heading"><span class="caption-text">Contents</span></p>
 <ul>
 <li class="toctree-l1"><a class="reference internal" href="cookies_utilities.html">Documentation</a><ul>
 <li class="toctree-l2"><a class="reference internal" href="cookies_utilities.html#functions">Functions</a></li>
 <li class="toctree-l2"><a class="reference internal" href="cookies_utilities.html#classes">Classes</a></li>
 </ul>
 </li>
 </ul>
 </div>
 </section>
-<section id="indices-and-tables">
-<h2>Indices and tables<a class="headerlink" href="#indices-and-tables" title="Permalink to this heading"></a></h2>
+<section id="links">
+<h2>Links<a class="headerlink" href="#links" title="Permalink to this heading"></a></h2>
+<ul class="simple">
+<li><p><a class="reference external" href="https://pypi.org/project/cookies-utilities/">PyPI</a></p></li>
+<li><p><a class="reference external" href="https://github.com/CookieBox26/cookies_utilities">GitHub</a> – If you want to maintain this package, please refer to the README in the GitHub repository.</p></li>
+</ul>
+</section>
+<section id="index">
+<h2>Index<a class="headerlink" href="#index" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p><a class="reference internal" href="genindex.html"><span class="std std-ref">Index</span></a></p></li>
 </ul>
 </section>
 </section>
```

#### html2text {}

```diff
@@ -2,29 +2,41 @@
 
 
 
 
 
 cookies_utilities
 [q                   ]
-Contents:
+Contents
     * Documentation
    cookies_utilities
     * Welcome to cookies_utilitiesâ documentation!
     * View_page_source
 ===============================================================================
 ****** Welcome to cookies_utilitiesâ documentation!ï ******
-***** Linksï *****
-    * PyPI
-    * GitHub
-Contents:
+This package is intended to provide useful functions and classes. Please see
+Documentation.
+***** Installationï *****
+You can install the release version from PyPI.
+pip install cookies_utilities
+If you want to use the latest version that has not been released, clone our
+GitHub_repository and install from the local directory.
+git clone https://github.com/CookieBox26/cookies_utilities.git
+cd cookies_utilities
+pip install .
+Contents
     * Documentation
           o Functions
           o Classes
 
-***** Indices and tablesï *****
+***** Linksï *****
+    * PyPI
+    * GitHub â If you want to maintain this package, please refer to the
+      README in the GitHub repository.
+
+***** Indexï *****
     * Index
 
 Next
 ===============================================================================
 © Copyright 2023, CookieBox26.
 Built with Sphinx using a theme provided by Read_the_Docs.
```

### Comparing `cookies_utilities-0.0.2/docs/build/html/modules.html` & `cookies_utilities-0.0.3/docs/build/html/modules.html`

 * *Files 19% similar despite different names*

```diff
@@ -36,15 +36,15 @@
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
 </div>
         </div><div class="wy-menu wy-menu-vertical" data-spy="affix" role="navigation" aria-label="Navigation menu">
-              <p class="caption" role="heading"><span class="caption-text">Contents:</span></p>
+              <p class="caption" role="heading"><span class="caption-text">Contents</span></p>
 <ul>
 <li class="toctree-l1"><a class="reference internal" href="cookies_utilities.html">Documentation</a></li>
 </ul>
 
         </div>
       </div>
     </nav>
@@ -71,18 +71,26 @@
              
   <section id="cookies-utilities">
 <h1>cookies_utilities<a class="headerlink" href="#cookies-utilities" title="Permalink to this heading"></a></h1>
 <div class="toctree-wrapper compound">
 <ul>
 <li class="toctree-l1"><a class="reference internal" href="cookies_utilities.html">Documentation</a><ul>
 <li class="toctree-l2"><a class="reference internal" href="cookies_utilities.html#functions">Functions</a><ul>
+<li class="toctree-l3"><a class="reference internal" href="cookies_utilities.html#cookies-utilities-copy-datetime">cookies_utilities.copy_datetime</a><ul>
+<li class="toctree-l4"><a class="reference internal" href="cookies_utilities.html#cookies_utilities.copy_datetime"><code class="docutils literal notranslate"><span class="pre">copy_datetime()</span></code></a></li>
+</ul>
+</li>
 <li class="toctree-l3"><a class="reference internal" href="cookies_utilities.html#cookies-utilities-get-dates">cookies_utilities.get_dates</a><ul>
 <li class="toctree-l4"><a class="reference internal" href="cookies_utilities.html#cookies_utilities.get_dates"><code class="docutils literal notranslate"><span class="pre">get_dates()</span></code></a></li>
 </ul>
 </li>
+<li class="toctree-l3"><a class="reference internal" href="cookies_utilities.html#cookies-utilities-convert-time-to-feature">cookies_utilities.convert_time_to_feature</a><ul>
+<li class="toctree-l4"><a class="reference internal" href="cookies_utilities.html#cookies_utilities.convert_time_to_feature"><code class="docutils literal notranslate"><span class="pre">convert_time_to_feature()</span></code></a></li>
+</ul>
+</li>
 </ul>
 </li>
 <li class="toctree-l2"><a class="reference internal" href="cookies_utilities.html#classes">Classes</a><ul>
 <li class="toctree-l3"><a class="reference internal" href="cookies_utilities.html#cookies-utilities-stopwatch">cookies_utilities.Stopwatch</a><ul>
 <li class="toctree-l4"><a class="reference internal" href="cookies_utilities.html#cookies_utilities.Stopwatch"><code class="docutils literal notranslate"><span class="pre">Stopwatch</span></code></a></li>
 </ul>
 </li>
```

#### html2text {}

```diff
@@ -1,25 +1,29 @@
 
 
 
 
 
 cookies_utilities
 [q                   ]
-Contents:
+Contents
     * Documentation
    cookies_utilities
     * cookies_utilities
     * View_page_source
 ===============================================================================
 ****** cookies_utilitiesï ******
     * Documentation
           o Functions
+                # cookies_utilities.copy_datetime
+                      # copy_datetime()
                 # cookies_utilities.get_dates
                       # get_dates()
+                # cookies_utilities.convert_time_to_feature
+                      # convert_time_to_feature()
           o Classes
                 # cookies_utilities.Stopwatch
                       # Stopwatch
 
 ===============================================================================
 © Copyright 2023, CookieBox26.
 Built with Sphinx using a theme provided by Read_the_Docs.
```

### Comparing `cookies_utilities-0.0.2/docs/build/html/search.html` & `cookies_utilities-0.0.3/docs/build/html/search.html`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
   <form id="rtd-search-form" class="wy-form" action="#" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
 </div>
         </div><div class="wy-menu wy-menu-vertical" data-spy="affix" role="navigation" aria-label="Navigation menu">
-              <p class="caption" role="heading"><span class="caption-text">Contents:</span></p>
+              <p class="caption" role="heading"><span class="caption-text">Contents</span></p>
 <ul>
 <li class="toctree-l1"><a class="reference internal" href="cookies_utilities.html">Documentation</a></li>
 </ul>
 
         </div>
       </div>
     </nav>
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
 
 
 
 
 
 cookies_utilities
 [q                   ]
-Contents:
+Contents
     * Documentation
    cookies_utilities
     * Search
 ===============================================================================
 Please activate JavaScript to enable the search functionality.
 
 ===============================================================================
```

### Comparing `cookies_utilities-0.0.2/docs/build/html/searchindex.js` & `cookies_utilities-0.0.3/docs/build/html/searchindex.js`

 * *Files 25% similar despite different names*

#### js-beautify {}

```diff
@@ -1,22 +1,22 @@
 Search.setIndex({
     "docnames": ["cookies_utilities", "index", "modules"],
     "filenames": ["cookies_utilities.rst", "index.rst", "modules.rst"],
     "titles": ["Documentation", "Welcome to cookies_utilities\u2019 documentation!", "cookies_utilities"],
     "terms": {
-        "index": 1,
+        "index": [],
         "modul": [],
         "search": [],
         "page": [],
-        "packag": [],
+        "packag": 1,
         "submodul": [],
         "stopwatch": 2,
         "content": [],
         "base": [],
-        "object": [],
+        "object": 0,
         "measur": 0,
         "process": 0,
         "time": 0,
         "press": 0,
         "kei": 0,
         "paramet": 0,
         "string": 0,
@@ -52,41 +52,41 @@
         "week": 0,
         "cast_str": 0,
         "true": 0,
         "format_out": 0,
         "none": 0,
         "return": 0,
         "list": 0,
-        "from": 0,
+        "from": [0, 1],
         "increment": 0,
         "convers": 0,
         "datetim": 0,
         "strptime": 0,
         "dict": 0,
         "arg": 0,
         "timedelta": 0,
-        "A": [],
+        "A": 0,
         "rtype": [],
         "type": 0,
         "bool": 0,
         "whether": 0,
         "convert": 0,
         "output": 0,
         "same": 0,
         "testpypi": [],
-        "http": [],
+        "http": 1,
         "test": 0,
         "pypi": 1,
         "org": [],
         "project": [],
         "cooki": [],
         "util": [],
         "github": 1,
-        "com": [],
-        "cookiebox26": [],
+        "com": 1,
+        "cookiebox26": 1,
         "import": 0,
         "cu": 0,
         "date": 0,
         "03": 0,
         "sw": 0,
         "train": 0,
         "time1": 0,
@@ -96,35 +96,135 @@
         "2": 0,
         "3": 0,
         "usag": [],
         "exampl": 0,
         "inclus": 0,
         "genit": 0,
         "fals": 0,
-        "If": 0,
-        "you": 0,
+        "If": [0, 1],
+        "you": [0, 1],
         "re": 0,
-        "us": 0,
+        "us": [0, 1],
         "result": 0,
         "an": 0,
         "iter": 0,
-        "i": 0,
+        "i": [0, 1],
         "recommend": 0,
         "set": 0,
         "gener": 0,
         "04": [],
         "20": 0,
         "print": 0,
         "40": 0,
         "one": 0,
-        "retriev": 0
+        "retriev": 0,
+        "pleas": [0, 1],
+        "ensur": 0,
+        "greater": 0,
+        "than": 0,
+        "equal": 0,
+        "microsecond": 0,
+        "thi": [0, 1],
+        "intend": 1,
+        "provid": 1,
+        "can": 1,
+        "releas": 1,
+        "version": 1,
+        "want": [0, 1],
+        "latest": 1,
+        "ha": [0, 1],
+        "been": 1,
+        "clone": 1,
+        "repositori": 1,
+        "local": 1,
+        "directori": 1,
+        "pip": 1,
+        "see": 1,
+        "git": 1,
+        "cd": 1,
+        "our": 1,
+        "maintain": 1,
+        "refer": 1,
+        "readm": 1,
+        "homepag": [],
+        "dt": 0,
+        "creat": 0,
+        "copi": 0,
+        "origin": 0,
+        "wish": 0,
+        "overwrit": 0,
+        "certain": 0,
+        "field": 0,
+        "specifi": 0,
+        "them": 0,
+        "dictionari": 0,
+        "copy_datetim": 2,
+        "must": 0,
+        "year": 0,
+        "month": 0,
+        "second": 0,
+        "tzinfo": 0,
+        "fold": 0,
+        "period": 0,
+        "ceil": 0,
+        "featur": 0,
+        "valu": 0,
+        "between": 0,
+        "repres": 0,
+        "how": 0,
+        "much": 0,
+        "pass": 0,
+        "float": 0,
+        "to_timefeatur": [],
+        "round": 0,
+        "when": 0,
+        "calcul": 0,
+        "granular": 0,
+        "argument": 0,
+        "For": 0,
+        "noon": 0,
+        "5": 0,
+        "we": 0,
+        "expect": 0,
+        "convert_time_to_featur": 2,
+        "15": 0,
+        "dt_copi": 0,
+        "feature_valu": 0,
+        "2023": 0,
+        "50": 0,
+        "125": 0,
+        "am": 0,
+        "12": 0,
+        "002732": 0,
+        "366": 0,
+        "032258": 0,
+        "31": 0,
+        "017857": 0,
+        "7": 0,
+        "666667": 0,
+        "60": 0,
+        "833333": 0,
+        "note": 0,
+        "cycl": 0,
+        "consid": 0,
+        "regardless": 0,
+        "actual": 0,
+        "number": 0,
+        "5th": 0,
+        "ani": 0,
+        "consist": 0,
+        "done": 0,
+        "remain": 0,
+        "specif": 0
     },
     "objects": {
         "cookies_utilities": [
             [0, 0, 1, "", "Stopwatch"],
+            [0, 2, 1, "", "convert_time_to_feature"],
+            [0, 2, 1, "", "copy_datetime"],
             [0, 2, 1, "", "get_dates"]
         ],
         "cookies_utilities.Stopwatch": [
             [0, 1, 1, "", "press"],
             [0, 1, 1, "", "show"]
         ]
     },
@@ -144,20 +244,25 @@
         "submodul": [],
         "stopwatch": 0,
         "modul": [],
         "content": 1,
         "welcom": 1,
         "": [],
         "document": [0, 1],
-        "indic": 1,
-        "tabl": 1,
+        "indic": [],
+        "tabl": [],
         "function": 0,
         "get_dat": 0,
         "class": 0,
-        "link": 1
+        "link": 1,
+        "instal": 1,
+        "index": 1,
+        "copy_datetim": 0,
+        "to_timefeatur": [],
+        "convert_time_to_featur": 0
     },
     "envversion": {
         "sphinx.domains.c": 2,
         "sphinx.domains.changeset": 1,
         "sphinx.domains.citation": 1,
         "sphinx.domains.cpp": 8,
         "sphinx.domains.index": 1,
@@ -165,49 +270,64 @@
         "sphinx.domains.math": 2,
         "sphinx.domains.python": 3,
         "sphinx.domains.rst": 2,
         "sphinx.domains.std": 2,
         "sphinx": 57
     },
     "alltitles": {
+        "cookies_utilities": [
+            [2, "cookies-utilities"]
+        ],
         "Welcome to cookies_utilities\u2019 documentation!": [
             [1, "welcome-to-cookies-utilities-documentation"]
         ],
-        "Links": [
-            [1, "links"]
+        "Installation": [
+            [1, "installation"]
         ],
-        "Contents:": [
+        "Contents": [
             [1, null]
         ],
-        "Indices and tables": [
-            [1, "indices-and-tables"]
+        "Links": [
+            [1, "links"]
         ],
-        "cookies_utilities": [
-            [2, "cookies-utilities"]
+        "Index": [
+            [1, "index"]
         ],
         "Documentation": [
             [0, "documentation"]
         ],
         "Functions": [
             [0, "functions"]
         ],
+        "cookies_utilities.copy_datetime": [
+            [0, "cookies-utilities-copy-datetime"]
+        ],
         "cookies_utilities.get_dates": [
             [0, "cookies-utilities-get-dates"]
         ],
+        "cookies_utilities.convert_time_to_feature": [
+            [0, "cookies-utilities-convert-time-to-feature"]
+        ],
         "Classes": [
             [0, "classes"]
         ],
         "cookies_utilities.Stopwatch": [
             [0, "cookies-utilities-stopwatch"]
         ]
     },
     "indexentries": {
         "stopwatch (class in cookies_utilities)": [
             [0, "cookies_utilities.Stopwatch"]
         ],
+        "convert_time_to_feature() (in module cookies_utilities)": [
+            [0, "cookies_utilities.convert_time_to_feature"]
+        ],
+        "copy_datetime() (in module cookies_utilities)": [
+            [0, "cookies_utilities.copy_datetime"]
+        ],
         "get_dates() (in module cookies_utilities)": [
             [0, "cookies_utilities.get_dates"]
         ],
         "press() (cookies_utilities.stopwatch method)": [
             [0, "cookies_utilities.Stopwatch.press"]
         ],
         "show() (cookies_utilities.stopwatch method)": [
```

### Comparing `cookies_utilities-0.0.2/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js` & `cookies_utilities-0.0.3/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.2/docs/build/html/_static/basic.css` & `cookies_utilities-0.0.3/docs/build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.2/docs/build/html/_static/doctools.js` & `cookies_utilities-0.0.3/docs/build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.2/docs/build/html/_static/jquery.js` & `cookies_utilities-0.0.3/docs/build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.2/docs/build/html/_static/language_data.js` & `cookies_utilities-0.0.3/docs/build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.2/docs/build/html/_static/pygments.css` & `cookies_utilities-0.0.3/docs/build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.2/docs/build/html/_static/searchtools.js` & `cookies_utilities-0.0.3/docs/build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.2/docs/build/html/_static/sphinx_highlight.js` & `cookies_utilities-0.0.3/docs/build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.2/docs/build/html/_static/css/badge_only.css` & `cookies_utilities-0.0.3/docs/build/html/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.2/docs/build/html/_static/css/theme.css` & `cookies_utilities-0.0.3/docs/build/html/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff` & `cookies_utilities-0.0.3/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2` & `cookies_utilities-0.0.3/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff` & `cookies_utilities-0.0.3/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2` & `cookies_utilities-0.0.3/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/fontawesome-webfont.eot` & `cookies_utilities-0.0.3/docs/build/html/_static/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/fontawesome-webfont.svg` & `cookies_utilities-0.0.3/docs/build/html/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf` & `cookies_utilities-0.0.3/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/fontawesome-webfont.woff` & `cookies_utilities-0.0.3/docs/build/html/_static/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2` & `cookies_utilities-0.0.3/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/lato-bold-italic.woff` & `cookies_utilities-0.0.3/docs/build/html/_static/css/fonts/lato-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/lato-bold-italic.woff2` & `cookies_utilities-0.0.3/docs/build/html/_static/css/fonts/lato-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/lato-bold.woff` & `cookies_utilities-0.0.3/docs/build/html/_static/css/fonts/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/lato-bold.woff2` & `cookies_utilities-0.0.3/docs/build/html/_static/css/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/lato-normal-italic.woff` & `cookies_utilities-0.0.3/docs/build/html/_static/css/fonts/lato-normal-italic.woff`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/lato-normal-italic.woff2` & `cookies_utilities-0.0.3/docs/build/html/_static/css/fonts/lato-normal-italic.woff2`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/lato-normal.woff` & `cookies_utilities-0.0.3/docs/build/html/_static/css/fonts/lato-normal.woff`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.2/docs/build/html/_static/css/fonts/lato-normal.woff2` & `cookies_utilities-0.0.3/docs/build/html/_static/css/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.2/docs/build/html/_static/js/badge_only.js` & `cookies_utilities-0.0.3/docs/build/html/_static/js/badge_only.js`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.2/docs/build/html/_static/js/html5shiv-printshiv.min.js` & `cookies_utilities-0.0.3/docs/build/html/_static/js/html5shiv-printshiv.min.js`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.2/docs/build/html/_static/js/html5shiv.min.js` & `cookies_utilities-0.0.3/docs/build/html/_static/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.2/docs/build/html/_static/js/theme.js` & `cookies_utilities-0.0.3/docs/build/html/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.2/docs/source/conf.py` & `cookies_utilities-0.0.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.2/src/cookies_utilities/stopwatch.py` & `cookies_utilities-0.0.3/src/cookies_utilities/stopwatch.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,12 +16,12 @@
 
     def show(self):
         """ Show lap times.
         """
         if len(self.cache) < 2:
             return
         for i in range(1, len(self.cache)):
-            k = f'{self.cache[i-1][0]}-{self.cache[i][0]}'
+            k = f'{self.cache[i-1][0]} - {self.cache[i][0]}'
             t = self.cache[i][1] - self.cache[i-1][1]
-            print(f'time{i}({k}): {t:.3f}s')
+            print(f'time{i} ({k}): {t:.3f}s')
         t = self.cache[-1][1] - self.cache[0][1]
         print(f'total: {t:.3f}s')
```

### Comparing `cookies_utilities-0.0.2/LICENSE` & `cookies_utilities-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cookies_utilities-0.0.2/README.md` & `cookies_utilities-0.0.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -5,41 +5,62 @@
 <!-- - [TestPyPI](https://test.pypi.org/project/cookies-utilities/) -->
 <!-- - [PyPI](https://pypi.org/project/cookies-utilities/) -->
 - [Documentation (released)](https://cookies-utilities.readthedocs.io/en/stable/)
 - [Documentation (main branch HEAD)](https://cookies-utilities.readthedocs.io/en/latest/)
 
 ---
 
-### Development Guide
+## Installation (for Users)
+
+You can install the release version from PyPI.
+
+```
+pip install cookies_utilities
+```
+
+If you want to use the latest version that has not been released, clone this repository and install from the local directory.
+
+```
+git clone https://github.com/CookieBox26/cookies_utilities.git
+cd cookies_utilities
+pip install .
+```
+
+## Development Guide (for Developers)
 
 Please execute the following at the root of the repository.
 
-#### Test locally
+### Test locally
 
 Please run the following commands.
 
 ```
+git clone https://github.com/CookieBox26/cookies_utilities.git
+cd cookies_utilities
+# make some changes to the code
 pip install -e .  # install the package in editable mode
 python -m unittest discover tests -v  # test
 ```
 If an error occurs, you can fix the code and rerun the tests without having to reinstall the package.
 
-#### Update documentation
+### Update documentation
 
 If you add a new function or class, please update the documentation accordingly.
 
 ```
 cd docs
 vi source/cookies_utilities.rst  # add a new function or class
 ./make.bat html  # or 'make html' (not on Windows)
 # Please open 'docs/build/html/index.html' in your browser and check the content.
 cd ..
 ```
 
-#### Build the distribution archives
+If you are not an administrator, please open a pull request at this point.
+
+### Build and upload the distribution archives (for administrator only)
 
 Please run the following commands. More details are [here](https://packaging.python.org/en/latest/tutorials/packaging-projects/#generating-distribution-archives).
 
 ```
 pip install --upgrade build  # upgrade 'build'
 python -m build
 ```
@@ -47,17 +68,15 @@
 The following files will be generated.
 
 ```
 ./dist/cookies_utilities-0.0.1.tar.gz
 ./dist/cookies_utilities-0.0.1-py3-none-any.whl
 ```
 
-#### Upload the distribution archives to TestPyPI (PyPI)
-
-Please run the following commands. More details are [here](https://packaging.python.org/en/latest/tutorials/packaging-projects/#uploading-the-distribution-archives).
+Then please run the following commands. More details are [here](https://packaging.python.org/en/latest/tutorials/packaging-projects/#uploading-the-distribution-archives).
 
 ```
 pip install --upgrade twine
 python -m twine upload --repository testpypi dist/*  # TestPyPI
 python -m twine upload dist/*  # PyPI
 ```
```

### Comparing `cookies_utilities-0.0.2/pyproject.toml` & `cookies_utilities-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cookies_utilities"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="CookieBox26", email="cookie-box@cookie-box.info" },
 ]
 description = "Utility functions."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `cookies_utilities-0.0.2/PKG-INFO` & `cookies_utilities-0.0.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cookies_utilities
-Version: 0.0.2
+Version: 0.0.3
 Summary: Utility functions.
 Project-URL: GitHub, https://github.com/CookieBox26/cookies_utilities
 Project-URL: Documentation, https://cookies-utilities.readthedocs.io/en/stable/
 Author-email: CookieBox26 <cookie-box@cookie-box.info>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -19,41 +19,62 @@
 <!-- - [TestPyPI](https://test.pypi.org/project/cookies-utilities/) -->
 <!-- - [PyPI](https://pypi.org/project/cookies-utilities/) -->
 - [Documentation (released)](https://cookies-utilities.readthedocs.io/en/stable/)
 - [Documentation (main branch HEAD)](https://cookies-utilities.readthedocs.io/en/latest/)
 
 ---
 
-### Development Guide
+## Installation (for Users)
+
+You can install the release version from PyPI.
+
+```
+pip install cookies_utilities
+```
+
+If you want to use the latest version that has not been released, clone this repository and install from the local directory.
+
+```
+git clone https://github.com/CookieBox26/cookies_utilities.git
+cd cookies_utilities
+pip install .
+```
+
+## Development Guide (for Developers)
 
 Please execute the following at the root of the repository.
 
-#### Test locally
+### Test locally
 
 Please run the following commands.
 
 ```
+git clone https://github.com/CookieBox26/cookies_utilities.git
+cd cookies_utilities
+# make some changes to the code
 pip install -e .  # install the package in editable mode
 python -m unittest discover tests -v  # test
 ```
 If an error occurs, you can fix the code and rerun the tests without having to reinstall the package.
 
-#### Update documentation
+### Update documentation
 
 If you add a new function or class, please update the documentation accordingly.
 
 ```
 cd docs
 vi source/cookies_utilities.rst  # add a new function or class
 ./make.bat html  # or 'make html' (not on Windows)
 # Please open 'docs/build/html/index.html' in your browser and check the content.
 cd ..
 ```
 
-#### Build the distribution archives
+If you are not an administrator, please open a pull request at this point.
+
+### Build and upload the distribution archives (for administrator only)
 
 Please run the following commands. More details are [here](https://packaging.python.org/en/latest/tutorials/packaging-projects/#generating-distribution-archives).
 
 ```
 pip install --upgrade build  # upgrade 'build'
 python -m build
 ```
@@ -61,17 +82,15 @@
 The following files will be generated.
 
 ```
 ./dist/cookies_utilities-0.0.1.tar.gz
 ./dist/cookies_utilities-0.0.1-py3-none-any.whl
 ```
 
-#### Upload the distribution archives to TestPyPI (PyPI)
-
-Please run the following commands. More details are [here](https://packaging.python.org/en/latest/tutorials/packaging-projects/#uploading-the-distribution-archives).
+Then please run the following commands. More details are [here](https://packaging.python.org/en/latest/tutorials/packaging-projects/#uploading-the-distribution-archives).
 
 ```
 pip install --upgrade twine
 python -m twine upload --repository testpypi dist/*  # TestPyPI
 python -m twine upload dist/*  # PyPI
 ```
```

