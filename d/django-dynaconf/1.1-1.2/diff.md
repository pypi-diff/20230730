# Comparing `tmp/django-dynaconf-1.1.tar.gz` & `tmp/django-dynaconf-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-dynaconf-1.1.tar", last modified: Wed Apr 13 13:04:47 2022, max compression
+gzip compressed data, was "django-dynaconf-1.2.tar", last modified: Sun Jul 30 17:23:56 2023, max compression
```

## Comparing `django-dynaconf-1.1.tar` & `django-dynaconf-1.2.tar`

### file list

```diff
@@ -1,23 +1,26 @@
-drwxr-xr-x   0 hassansiddiqui   (502) staff       (20)        0 2022-04-13 13:04:47.000000 django-dynaconf-1.1/
--rw-r--r--   0 hassansiddiqui   (502) staff       (20)     1067 2022-02-14 21:11:11.000000 django-dynaconf-1.1/LICENSE
--rw-r--r--   0 hassansiddiqui   (502) staff       (20)     3915 2022-04-13 13:04:47.000000 django-dynaconf-1.1/PKG-INFO
--rw-r--r--   0 hassansiddiqui   (502) staff       (20)     2409 2022-04-13 12:55:57.000000 django-dynaconf-1.1/README.md
-drwxr-xr-x   0 hassansiddiqui   (502) staff       (20)        0 2022-04-13 13:04:47.000000 django-dynaconf-1.1/django_dynaconf/
--rw-r--r--   0 hassansiddiqui   (502) staff       (20)      153 2022-04-13 12:59:24.000000 django-dynaconf-1.1/django_dynaconf/__init__.py
--rw-r--r--   0 hassansiddiqui   (502) staff       (20)      431 2022-02-25 15:18:21.000000 django-dynaconf-1.1/django_dynaconf/admin.py
--rw-r--r--   0 hassansiddiqui   (502) staff       (20)      169 2022-04-13 12:47:17.000000 django-dynaconf-1.1/django_dynaconf/apps.py
--rw-r--r--   0 hassansiddiqui   (502) staff       (20)     2444 2022-04-13 12:51:08.000000 django-dynaconf-1.1/django_dynaconf/configs.py
-drwxr-xr-x   0 hassansiddiqui   (502) staff       (20)        0 2022-04-13 13:04:47.000000 django-dynaconf-1.1/django_dynaconf/migrations/
--rw-r--r--   0 hassansiddiqui   (502) staff       (20)     1365 2022-02-15 20:02:49.000000 django-dynaconf-1.1/django_dynaconf/migrations/0001_initial.py
--rw-r--r--   0 hassansiddiqui   (502) staff       (20)        0 2022-02-13 07:20:46.000000 django-dynaconf-1.1/django_dynaconf/migrations/__init__.py
--rw-r--r--   0 hassansiddiqui   (502) staff       (20)     4672 2022-02-25 15:15:16.000000 django-dynaconf-1.1/django_dynaconf/models.py
--rw-r--r--   0 hassansiddiqui   (502) staff       (20)      125 2022-02-13 07:20:46.000000 django-dynaconf-1.1/django_dynaconf/tests.py
-drwxr-xr-x   0 hassansiddiqui   (502) staff       (20)        0 2022-04-13 13:04:47.000000 django-dynaconf-1.1/django_dynaconf.egg-info/
--rw-r--r--   0 hassansiddiqui   (502) staff       (20)     3915 2022-04-13 13:04:45.000000 django-dynaconf-1.1/django_dynaconf.egg-info/PKG-INFO
--rw-r--r--   0 hassansiddiqui   (502) staff       (20)      495 2022-04-13 13:04:47.000000 django-dynaconf-1.1/django_dynaconf.egg-info/SOURCES.txt
--rw-r--r--   0 hassansiddiqui   (502) staff       (20)        1 2022-04-13 13:04:45.000000 django-dynaconf-1.1/django_dynaconf.egg-info/dependency_links.txt
--rw-r--r--   0 hassansiddiqui   (502) staff       (20)        1 2022-02-25 16:05:49.000000 django-dynaconf-1.1/django_dynaconf.egg-info/not-zip-safe
--rw-r--r--   0 hassansiddiqui   (502) staff       (20)       50 2022-04-13 13:04:46.000000 django-dynaconf-1.1/django_dynaconf.egg-info/requires.txt
--rw-r--r--   0 hassansiddiqui   (502) staff       (20)       16 2022-04-13 13:04:46.000000 django-dynaconf-1.1/django_dynaconf.egg-info/top_level.txt
--rw-r--r--   0 hassansiddiqui   (502) staff       (20)       38 2022-04-13 13:04:47.000000 django-dynaconf-1.1/setup.cfg
--rw-r--r--   0 hassansiddiqui   (502) staff       (20)     2335 2022-04-13 12:47:17.000000 django-dynaconf-1.1/setup.py
+drwxr-xr-x   0 hassan.siddiqui   (502) staff       (20)        0 2023-07-30 17:23:56.731256 django-dynaconf-1.2/
+-rw-r--r--   0 hassan.siddiqui   (502) staff       (20)     1067 2023-07-30 10:04:07.000000 django-dynaconf-1.2/LICENSE
+-rw-r--r--   0 hassan.siddiqui   (502) staff       (20)     4204 2023-07-30 17:23:56.730996 django-dynaconf-1.2/PKG-INFO
+-rw-r--r--   0 hassan.siddiqui   (502) staff       (20)     2629 2023-07-30 17:08:11.000000 django-dynaconf-1.2/README.md
+drwxr-xr-x   0 hassan.siddiqui   (502) staff       (20)        0 2023-07-30 17:23:56.725812 django-dynaconf-1.2/django_dynaconf/
+-rw-r--r--   0 hassan.siddiqui   (502) staff       (20)      153 2023-07-30 15:33:08.000000 django-dynaconf-1.2/django_dynaconf/__init__.py
+-rw-r--r--   0 hassan.siddiqui   (502) staff       (20)      439 2023-07-30 15:11:03.000000 django-dynaconf-1.2/django_dynaconf/admin.py
+-rw-r--r--   0 hassan.siddiqui   (502) staff       (20)      169 2023-07-30 10:04:07.000000 django-dynaconf-1.2/django_dynaconf/apps.py
+-rw-r--r--   0 hassan.siddiqui   (502) staff       (20)     2771 2023-07-30 16:36:42.000000 django-dynaconf-1.2/django_dynaconf/configs.py
+drwxr-xr-x   0 hassan.siddiqui   (502) staff       (20)        0 2023-07-30 17:23:56.729586 django-dynaconf-1.2/django_dynaconf/migrations/
+-rw-r--r--   0 hassan.siddiqui   (502) staff       (20)     1365 2023-07-30 10:04:07.000000 django-dynaconf-1.2/django_dynaconf/migrations/0001_initial.py
+-rw-r--r--   0 hassan.siddiqui   (502) staff       (20)      577 2023-07-30 16:32:04.000000 django-dynaconf-1.2/django_dynaconf/migrations/0002_auto_20230730_1449.py
+-rw-r--r--   0 hassan.siddiqui   (502) staff       (20)        0 2023-07-30 10:04:07.000000 django-dynaconf-1.2/django_dynaconf/migrations/__init__.py
+-rw-r--r--   0 hassan.siddiqui   (502) staff       (20)     4942 2023-07-30 16:32:04.000000 django-dynaconf-1.2/django_dynaconf/models.py
+drwxr-xr-x   0 hassan.siddiqui   (502) staff       (20)        0 2023-07-30 17:23:56.728404 django-dynaconf-1.2/django_dynaconf.egg-info/
+-rw-r--r--   0 hassan.siddiqui   (502) staff       (20)     4204 2023-07-30 17:23:56.000000 django-dynaconf-1.2/django_dynaconf.egg-info/PKG-INFO
+-rw-r--r--   0 hassan.siddiqui   (502) staff       (20)      562 2023-07-30 17:23:56.000000 django-dynaconf-1.2/django_dynaconf.egg-info/SOURCES.txt
+-rw-r--r--   0 hassan.siddiqui   (502) staff       (20)        1 2023-07-30 17:23:56.000000 django-dynaconf-1.2/django_dynaconf.egg-info/dependency_links.txt
+-rw-r--r--   0 hassan.siddiqui   (502) staff       (20)        1 2023-07-30 12:33:05.000000 django-dynaconf-1.2/django_dynaconf.egg-info/not-zip-safe
+-rw-r--r--   0 hassan.siddiqui   (502) staff       (20)       50 2023-07-30 17:23:56.000000 django-dynaconf-1.2/django_dynaconf.egg-info/requires.txt
+-rw-r--r--   0 hassan.siddiqui   (502) staff       (20)       16 2023-07-30 17:23:56.000000 django-dynaconf-1.2/django_dynaconf.egg-info/top_level.txt
+-rw-r--r--   0 hassan.siddiqui   (502) staff       (20)       38 2023-07-30 17:23:56.731297 django-dynaconf-1.2/setup.cfg
+-rw-r--r--   0 hassan.siddiqui   (502) staff       (20)     2403 2023-07-30 17:23:00.000000 django-dynaconf-1.2/setup.py
+drwxr-xr-x   0 hassan.siddiqui   (502) staff       (20)        0 2023-07-30 17:23:56.730431 django-dynaconf-1.2/tests/
+-rw-r--r--   0 hassan.siddiqui   (502) staff       (20)     1201 2023-07-30 10:04:07.000000 django-dynaconf-1.2/tests/test_settings.py
+-rw-r--r--   0 hassan.siddiqui   (502) staff       (20)     7869 2023-07-30 16:47:40.000000 django-dynaconf-1.2/tests/tests.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-dynaconf-1.1/LICENSE` & `django-dynaconf-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-dynaconf-1.1/PKG-INFO` & `django-dynaconf-1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-dynaconf
-Version: 1.1
+Version: 1.2
 Summary: Dynamic Configuration for your Django project
 Home-page: https://github.com/mhsiddiqui/django-dynaconf
 Author: Muhammad Hassan Siddiqui
 Author-email: mhassan.eeng@gmail.com
 License: MIT
 Keywords: django,dynamic-configuration,dynamic-settings,django-settings-from-admin
 Platform: any
@@ -12,25 +12,27 @@
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 1.10
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 Provides-Extra: django
 Provides-Extra: dateutil
@@ -129,8 +131,16 @@
 from django_dynaconf.configs import configs
 
 print(configs.KEY_OF_YOUR_CONFIGURATION)
 ```
 
 At any time, when you will change your config value or add a new value, it will be available to use in you code.
 
+## Grouping (v1.2)
 
+You can group configurations. Configurations of a perticular group can be accessed like this.
+
+```python
+from django_dynaconf.configs import configs
+
+print(configs.grouped(group='NAME_OF_GROUP'))
+```
```

### Comparing `django-dynaconf-1.1/README.md` & `django-dynaconf-1.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -90,7 +90,17 @@
 ```python
 from django_dynaconf.configs import configs
 
 print(configs.KEY_OF_YOUR_CONFIGURATION)
 ```
 
 At any time, when you will change your config value or add a new value, it will be available to use in you code.
+
+## Grouping (v1.2)
+
+You can group configurations. Configurations of a perticular group can be accessed like this.
+
+```python
+from django_dynaconf.configs import configs
+
+print(configs.grouped(group='NAME_OF_GROUP'))
+```
```

### Comparing `django-dynaconf-1.1/django_dynaconf/configs.py` & `django-dynaconf-1.2/django_dynaconf/configs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from collections import defaultdict
 from django.utils.functional import LazyObject, empty
 
 from .models import Configuration
 
 
 class Configs(object):
     """
@@ -80,9 +81,18 @@
     @property
     def configured(self):
         """
         Returns True if the configuration have already been configured.
         """
         return self._wrapped is not empty
 
+    def grouped(self, group):
+        """
+        Return grouped configurations
+        """
+        configurations = Configuration.objects.filter(group=group, is_active=True)
+        if configurations.exists():
+            return Configs(configurations=configurations)
+        return empty
+
 
 configs = LazyConfigs()
```

### Comparing `django-dynaconf-1.1/django_dynaconf/migrations/0001_initial.py` & `django-dynaconf-1.2/django_dynaconf/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-dynaconf-1.1/django_dynaconf/models.py` & `django-dynaconf-1.2/django_dynaconf/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     STRING = 'string'
     NUMBER = 'number'
     BOOLEAN = 'boolean'
     JSON = 'json'
     DATE = 'date'
     DATETIME = 'datetime'
     TIME = 'time'
-    DEFAULT_GROUP = 'default'
+    DEFAULT_GROUP = 'DEFAULT'
     VALUE_TYPE = (
         (STRING, _('String')),
         (NUMBER, _('Number')),
         (BOOLEAN, _('Boolean')),
         (JSON, _('Json')),
         (DATE, _('Date')),
         (DATETIME, _('Datetime')),
@@ -61,14 +61,22 @@
     )
     key = models.CharField(max_length=100, unique=True, validators=[
         RegexValidator(
             regex=r"[A-Z\d_]+",
             message=_('Key can only contains uppercase letters, numbers and _')
         )
     ])
+    group = models.CharField(
+        max_length=100, default=DEFAULT_GROUP, validators=[
+            RegexValidator(
+                regex=r"[A-Z\d_]+",
+                message=_('Group can only contains uppercase letters, numbers and _')
+            )
+        ]
+    )
     description = models.CharField(
         max_length=200, null=True, blank=True, help_text=_('Description of configuration')
     )
     value = models.TextField()
     type = models.CharField(choices=VALUE_TYPE, max_length=20, default=STRING)
     is_active = models.BooleanField(default=True)
     created = models.DateTimeField(auto_now_add=True)
```

### Comparing `django-dynaconf-1.1/django_dynaconf.egg-info/PKG-INFO` & `django-dynaconf-1.2/django_dynaconf.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-dynaconf
-Version: 1.1
+Version: 1.2
 Summary: Dynamic Configuration for your Django project
 Home-page: https://github.com/mhsiddiqui/django-dynaconf
 Author: Muhammad Hassan Siddiqui
 Author-email: mhassan.eeng@gmail.com
 License: MIT
 Keywords: django,dynamic-configuration,dynamic-settings,django-settings-from-admin
 Platform: any
@@ -12,25 +12,27 @@
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 1.10
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 Provides-Extra: django
 Provides-Extra: dateutil
@@ -129,8 +131,16 @@
 from django_dynaconf.configs import configs
 
 print(configs.KEY_OF_YOUR_CONFIGURATION)
 ```
 
 At any time, when you will change your config value or add a new value, it will be available to use in you code.
 
+## Grouping (v1.2)
 
+You can group configurations. Configurations of a perticular group can be accessed like this.
+
+```python
+from django_dynaconf.configs import configs
+
+print(configs.grouped(group='NAME_OF_GROUP'))
+```
```

### Comparing `django-dynaconf-1.1/setup.py` & `django-dynaconf-1.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -37,25 +37,27 @@
         'Environment :: Web Environment',
         'Framework :: Django',
         'Framework :: Django :: 1.10',
         'Framework :: Django :: 2.2',
         'Framework :: Django :: 3.0',
         'Framework :: Django :: 3.1',
         'Framework :: Django :: 3.2',
+        'Framework :: Django :: 4.0',
+        'Framework :: Django :: 4.1',
+        'Framework :: Django :: 4.2',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy',
         'Topic :: Utilities',
     ],
     packages=find_packages(exclude=['tests']),
     include_package_data=True,
     zip_safe=False,
```

