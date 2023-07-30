# Comparing `tmp/i18nice-0.6.2.tar.gz` & `tmp/i18nice-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "i18nice-0.6.2.tar", last modified: Mon Mar 27 14:15:46 2023, max compression
+gzip compressed data, was "i18nice-0.7.0.tar", last modified: Sun Jul 30 20:35:59 2023, max compression
```

## Comparing `i18nice-0.6.2.tar` & `i18nice-0.7.0.tar`

### file list

```diff
@@ -1,33 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-27 14:15:46.778915 i18nice-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-03-27 14:15:38.000000 i18nice-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-03-27 14:15:38.000000 i18nice-0.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     7075 2023-03-27 14:15:46.778915 i18nice-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6378 2023-03-27 14:15:38.000000 i18nice-0.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-27 14:15:46.774915 i18nice-0.6.2/i18n/
--rw-r--r--   0 runner    (1001) docker     (122)      371 2023-03-27 14:15:38.000000 i18nice-0.6.2/i18n/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1508 2023-03-27 14:15:38.000000 i18nice-0.6.2/i18n/config.py
--rw-r--r--   0 runner    (1001) docker     (122)      429 2023-03-27 14:15:38.000000 i18nice-0.6.2/i18n/custom_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-27 14:15:46.774915 i18nice-0.6.2/i18n/loaders/
--rw-r--r--   0 runner    (1001) docker     (122)      252 2023-03-27 14:15:38.000000 i18nice-0.6.2/i18n/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      404 2023-03-27 14:15:38.000000 i18nice-0.6.2/i18n/loaders/json_loader.py
--rw-r--r--   0 runner    (1001) docker     (122)     1947 2023-03-27 14:15:38.000000 i18nice-0.6.2/i18n/loaders/loader.py
--rw-r--r--   0 runner    (1001) docker     (122)      774 2023-03-27 14:15:38.000000 i18nice-0.6.2/i18n/loaders/python_loader.py
--rw-r--r--   0 runner    (1001) docker     (122)      446 2023-03-27 14:15:38.000000 i18nice-0.6.2/i18n/loaders/yaml_loader.py
--rw-r--r--   0 runner    (1001) docker     (122)     4582 2023-03-27 14:15:38.000000 i18nice-0.6.2/i18n/resource_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-27 14:15:46.774915 i18nice-0.6.2/i18n/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-27 14:15:38.000000 i18nice-0.6.2/i18n/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       37 2023-03-27 14:15:38.000000 i18nice-0.6.2/i18n/tests/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14643 2023-03-27 14:15:38.000000 i18nice-0.6.2/i18n/tests/loader_tests.py
--rw-r--r--   0 runner    (1001) docker     (122)     1766 2023-03-27 14:15:38.000000 i18nice-0.6.2/i18n/tests/run_tests.py
--rw-r--r--   0 runner    (1001) docker     (122)     8027 2023-03-27 14:15:38.000000 i18nice-0.6.2/i18n/tests/translation_tests.py
--rw-r--r--   0 runner    (1001) docker     (122)      581 2023-03-27 14:15:38.000000 i18nice-0.6.2/i18n/translations.py
--rw-r--r--   0 runner    (1001) docker     (122)     4033 2023-03-27 14:15:38.000000 i18nice-0.6.2/i18n/translator.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-27 14:15:46.778915 i18nice-0.6.2/i18nice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     7075 2023-03-27 14:15:46.000000 i18nice-0.6.2/i18nice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      602 2023-03-27 14:15:46.000000 i18nice-0.6.2/i18nice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-27 14:15:46.000000 i18nice-0.6.2/i18nice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-03-27 14:15:46.000000 i18nice-0.6.2/i18nice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-03-27 14:15:46.000000 i18nice-0.6.2/i18nice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-27 14:15:46.000000 i18nice-0.6.2/i18nice.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-27 14:15:46.778915 i18nice-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      985 2023-03-27 14:15:38.000000 i18nice-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 20:35:59.126722 i18nice-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-07-30 20:35:51.000000 i18nice-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-07-30 20:35:51.000000 i18nice-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     8100 2023-07-30 20:35:59.126722 i18nice-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7301 2023-07-30 20:35:51.000000 i18nice-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 20:35:59.122722 i18nice-0.7.0/i18n/
+-rw-r--r--   0 runner    (1001) docker     (122)      427 2023-07-30 20:35:51.000000 i18nice-0.7.0/i18n/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1389 2023-07-30 20:35:51.000000 i18nice-0.7.0/i18n/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)      429 2023-07-30 20:35:51.000000 i18nice-0.7.0/i18n/custom_functions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      250 2023-07-30 20:35:51.000000 i18nice-0.7.0/i18n/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4807 2023-07-30 20:35:51.000000 i18nice-0.7.0/i18n/formatters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 20:35:59.122722 i18nice-0.7.0/i18n/loaders/
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2023-07-30 20:35:51.000000 i18nice-0.7.0/i18n/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      404 2023-07-30 20:35:51.000000 i18nice-0.7.0/i18n/loaders/json_loader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1836 2023-07-30 20:35:51.000000 i18nice-0.7.0/i18n/loaders/loader.py
+-rw-r--r--   0 runner    (1001) docker     (122)      774 2023-07-30 20:35:51.000000 i18nice-0.7.0/i18n/loaders/python_loader.py
+-rw-r--r--   0 runner    (1001) docker     (122)      446 2023-07-30 20:35:51.000000 i18nice-0.7.0/i18n/loaders/yaml_loader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4759 2023-07-30 20:35:51.000000 i18nice-0.7.0/i18n/resource_loader.py
+-rw-r--r--   0 runner    (1001) docker     (122)      581 2023-07-30 20:35:51.000000 i18nice-0.7.0/i18n/translations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2674 2023-07-30 20:35:51.000000 i18nice-0.7.0/i18n/translator.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 20:35:59.126722 i18nice-0.7.0/i18nice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8100 2023-07-30 20:35:59.000000 i18nice-0.7.0/i18nice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      507 2023-07-30 20:35:59.000000 i18nice-0.7.0/i18nice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-30 20:35:59.000000 i18nice-0.7.0/i18nice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-07-30 20:35:59.000000 i18nice-0.7.0/i18nice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-30 20:35:59.000000 i18nice-0.7.0/i18nice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-30 20:35:58.000000 i18nice-0.7.0/i18nice.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-30 20:35:59.126722 i18nice-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1048 2023-07-30 20:35:51.000000 i18nice-0.7.0/setup.py
```

### Comparing `i18nice-0.6.2/LICENSE` & `i18nice-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `i18nice-0.6.2/PKG-INFO` & `i18nice-0.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: i18nice
-Version: 0.6.2
+Version: 0.7.0
 Summary: Translation library for Python
 Home-page: https://github.com/Krutyi-4el/i18nice
 Download-URL: https://github.com/Krutyi-4el/i18nice/archive/master.zip
 Author: Daniel Perez
 Author-email: tuvistavie@gmail.com
+Maintainer: Krutyi 4el
 License: MIT
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Internationalization
 Description-Content-Type: text/markdown
 Provides-Extra: YAML
 License-File: LICENSE
 
 # i18nice [![tests](https://github.com/Krutyi-4el/i18nice/actions/workflows/ci.yml/badge.svg)](https://github.com/Krutyi-4el/i18nice/actions/workflows/ci.yml) [![Coverage Status](https://coveralls.io/repos/github/Krutyi-4el/i18nice/badge.svg)](https://coveralls.io/github/Krutyi-4el/i18nice)
 
 
@@ -126,14 +128,38 @@
     }
 
 However we would like to use this i18n .json file in our Python sub-project or micro service as base file for translations.
 `i18nice` has special configuration that is skipping locale eg. `en` root data element from the file.
 
     i18n.set('skip_locale_root_data', True)
 
+### Static references
+
+Static references allow you to refer to other translation values. This can be useful to avoid repetition. To create a static reference, simply put a key prefixed with namespace delimiter to a placeholder. For example:
+
+    {
+      "en": {
+        "progname": "Program Name",
+        "welcome": "Welcome to %{.progname}!"
+      }
+    }
+
+Note that you don't need to specify the absolute key:
+
+    {
+      "en": {
+        "interface": {
+          "progname": "Program Name",
+          "ref": "%{.progname} and %{.interface.progname} refer to the same value"
+        }
+      }
+    }
+
+To be exact, keys are searched from top to bottom. For example, if you referred to `.c.my_key` in `a.b.c.d`, the library will first check for `c.my_key`, then `a.c.my_key`, and finally find `a.b.c.my_key` if it's present. If not, it'll try to search `c.my_key` in other files and throw an exception if that also fails.
+
 ### Error handling
 
 There are three config options for handling different situations.
 Setting it to `None` disables handling (default), `"error"` enables error throwing.
 You can also set your custom handlers:
 
 `on_missing_translation(key, locale, **kwargs)`
```

### Comparing `i18nice-0.6.2/README.md` & `i18nice-0.7.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -106,14 +106,38 @@
     }
 
 However we would like to use this i18n .json file in our Python sub-project or micro service as base file for translations.
 `i18nice` has special configuration that is skipping locale eg. `en` root data element from the file.
 
     i18n.set('skip_locale_root_data', True)
 
+### Static references
+
+Static references allow you to refer to other translation values. This can be useful to avoid repetition. To create a static reference, simply put a key prefixed with namespace delimiter to a placeholder. For example:
+
+    {
+      "en": {
+        "progname": "Program Name",
+        "welcome": "Welcome to %{.progname}!"
+      }
+    }
+
+Note that you don't need to specify the absolute key:
+
+    {
+      "en": {
+        "interface": {
+          "progname": "Program Name",
+          "ref": "%{.progname} and %{.interface.progname} refer to the same value"
+        }
+      }
+    }
+
+To be exact, keys are searched from top to bottom. For example, if you referred to `.c.my_key` in `a.b.c.d`, the library will first check for `c.my_key`, then `a.c.my_key`, and finally find `a.b.c.my_key` if it's present. If not, it'll try to search `c.my_key` in other files and throw an exception if that also fails.
+
 ### Error handling
 
 There are three config options for handling different situations.
 Setting it to `None` disables handling (default), `"error"` enables error throwing.
 You can also set your custom handlers:
 
 `on_missing_translation(key, locale, **kwargs)`
```

### Comparing `i18nice-0.6.2/i18n/config.py` & `i18nice-0.7.0/i18n/config.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from importlib import reload as _reload
+
 try:
     __import__("yaml")
     yaml_available = True
 except ImportError:
     yaml_available = False
 
 try:
@@ -36,22 +38,21 @@
     'enable_memoization': False,
     'argument_delimiter': '|'
 }
 
 def set(key, value):
     if key not in settings:
         raise KeyError("Invalid setting: {0}".format(key))
-    if key == 'placeholder_delimiter':
-        # hacky trick to reload formatter's configuration
-        from .translator import TranslationFormatter
-
-        TranslationFormatter.delimiter = value
-        del TranslationFormatter.pattern
-        TranslationFormatter.__init_subclass__()
     elif key == 'load_path':
         load_path.clear()
         load_path.extend(value)
         return
+
     settings[key] = value
 
+    if key in ('placeholder_delimiter', 'namespace_delimiter'):
+        from . import formatters
+
+        _reload(formatters)
+
 def get(key):
     return settings[key]
```

### Comparing `i18nice-0.6.2/i18n/loaders/loader.py` & `i18nice-0.7.0/i18n/loaders/loader.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,12 @@
-from .. import config
 import io
 import os.path
 
-
-class I18nFileLoadError(Exception):
-    def __init__(self, value):
-        self.value = value
-
-    def __str__(self):
-        return str(self.value)
+from .. import config
+from ..errors import I18nFileLoadError
 
 
 class Loader(object):
     """Base class to load resources"""
 
     loaded_files = {}
```

### Comparing `i18nice-0.6.2/i18n/loaders/python_loader.py` & `i18nice-0.7.0/i18n/loaders/python_loader.py`

 * *Files identical despite different names*

### Comparing `i18nice-0.6.2/i18n/resource_loader.py` & `i18nice-0.7.0/i18n/resource_loader.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os.path
 
 from . import config
 from .loaders import Loader, I18nFileLoadError
-from . import translations
+from . import translations, formatters
 
 loaders = {}
 
 PLURALS = {"zero", "one", "few", "many"}
 
 
 def register_loader(loader_class, supported_extensions):
@@ -73,30 +73,35 @@
         locale = config.get('locale')
     skip_locale_root_data = config.get('skip_locale_root_data')
     root_data = None if skip_locale_root_data else locale
     # if the file isn't dedicated to one locale and may contain other `root_data`s
     remember_content = "{locale}" not in config.get("filename_format") and root_data
     translations_dic = load_resource(os.path.join(base_directory, filename), root_data, remember_content)
     namespace = get_namespace_from_filepath(filename)
-    load_translation_dic(translations_dic, namespace, locale)
+    loaded = load_translation_dic(translations_dic, namespace, locale)
+    formatters.expand_static_refs(loaded, locale)
 
 
 def reload_everything():
     translations.clear()
     Loader.loaded_files.clear()
 
 
 def load_translation_dic(dic, namespace, locale):
+    loaded = set()
     if namespace:
         namespace += config.get('namespace_delimiter')
     for key, value in dic.items():
+        full_key = namespace + key
         if type(value) == dict and len(PLURALS.intersection(value)) < 2:
-            load_translation_dic(value, namespace + key, locale)
+            loaded.update(load_translation_dic(value, full_key, locale))
         else:
-            translations.add(namespace + key, value, locale)
+            translations.add(full_key, value, locale)
+            loaded.add(full_key)
+    return loaded
 
 
 def load_directory(directory, locale):
     for f in os.listdir(directory):
         path = os.path.join(directory, f)
         if os.path.isfile(path) and path.endswith(config.get('file_format')):
             if '{locale}' in config.get('filename_format') and not locale in f:
```

### Comparing `i18nice-0.6.2/i18n/translations.py` & `i18nice-0.7.0/i18n/translations.py`

 * *Files identical despite different names*

### Comparing `i18nice-0.6.2/i18nice.egg-info/PKG-INFO` & `i18nice-0.7.0/i18nice.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: i18nice
-Version: 0.6.2
+Version: 0.7.0
 Summary: Translation library for Python
 Home-page: https://github.com/Krutyi-4el/i18nice
 Download-URL: https://github.com/Krutyi-4el/i18nice/archive/master.zip
 Author: Daniel Perez
 Author-email: tuvistavie@gmail.com
+Maintainer: Krutyi 4el
 License: MIT
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Internationalization
 Description-Content-Type: text/markdown
 Provides-Extra: YAML
 License-File: LICENSE
 
 # i18nice [![tests](https://github.com/Krutyi-4el/i18nice/actions/workflows/ci.yml/badge.svg)](https://github.com/Krutyi-4el/i18nice/actions/workflows/ci.yml) [![Coverage Status](https://coveralls.io/repos/github/Krutyi-4el/i18nice/badge.svg)](https://coveralls.io/github/Krutyi-4el/i18nice)
 
 
@@ -126,14 +128,38 @@
     }
 
 However we would like to use this i18n .json file in our Python sub-project or micro service as base file for translations.
 `i18nice` has special configuration that is skipping locale eg. `en` root data element from the file.
 
     i18n.set('skip_locale_root_data', True)
 
+### Static references
+
+Static references allow you to refer to other translation values. This can be useful to avoid repetition. To create a static reference, simply put a key prefixed with namespace delimiter to a placeholder. For example:
+
+    {
+      "en": {
+        "progname": "Program Name",
+        "welcome": "Welcome to %{.progname}!"
+      }
+    }
+
+Note that you don't need to specify the absolute key:
+
+    {
+      "en": {
+        "interface": {
+          "progname": "Program Name",
+          "ref": "%{.progname} and %{.interface.progname} refer to the same value"
+        }
+      }
+    }
+
+To be exact, keys are searched from top to bottom. For example, if you referred to `.c.my_key` in `a.b.c.d`, the library will first check for `c.my_key`, then `a.c.my_key`, and finally find `a.b.c.my_key` if it's present. If not, it'll try to search `c.my_key` in other files and throw an exception if that also fails.
+
 ### Error handling
 
 There are three config options for handling different situations.
 Setting it to `None` disables handling (default), `"error"` enables error throwing.
 You can also set your custom handlers:
 
 `on_missing_translation(key, locale, **kwargs)`
```

