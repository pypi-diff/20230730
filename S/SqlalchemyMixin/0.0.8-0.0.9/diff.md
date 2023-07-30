# Comparing `tmp/SqlalchemyMixin-0.0.8.tar.gz` & `tmp/SqlalchemyMixin-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SqlalchemyMixin-0.0.8.tar", last modified: Fri Oct 28 22:24:58 2022, max compression
+gzip compressed data, was "SqlalchemyMixin-0.0.9.tar", last modified: Fri Oct 28 22:53:04 2022, max compression
```

## Comparing `SqlalchemyMixin-0.0.8.tar` & `SqlalchemyMixin-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2022-10-28 22:24:58.851619 SqlalchemyMixin-0.0.8/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1071 2022-10-16 19:39:29.000000 SqlalchemyMixin-0.0.8/LICENSE
--rw-r--r--   0 yasarozyurt   (501) staff       (20)    13822 2022-10-28 22:24:58.851479 SqlalchemyMixin-0.0.8/PKG-INFO
--rw-r--r--   0 yasarozyurt   (501) staff       (20)    13094 2022-10-28 19:30:20.000000 SqlalchemyMixin-0.0.8/README.md
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2022-10-28 22:24:58.846759 SqlalchemyMixin-0.0.8/SqlalchemyMixin.egg-info/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)    13822 2022-10-28 22:24:58.000000 SqlalchemyMixin-0.0.8/SqlalchemyMixin.egg-info/PKG-INFO
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      610 2022-10-28 22:24:58.000000 SqlalchemyMixin-0.0.8/SqlalchemyMixin.egg-info/SOURCES.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        1 2022-10-28 22:24:58.000000 SqlalchemyMixin-0.0.8/SqlalchemyMixin.egg-info/dependency_links.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)       60 2022-10-28 22:24:58.000000 SqlalchemyMixin-0.0.8/SqlalchemyMixin.egg-info/requires.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)       18 2022-10-28 22:24:58.000000 SqlalchemyMixin-0.0.8/SqlalchemyMixin.egg-info/top_level.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)       38 2022-10-28 22:24:58.851662 SqlalchemyMixin-0.0.8/setup.cfg
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1248 2022-10-28 22:24:36.000000 SqlalchemyMixin-0.0.8/setup.py
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2022-10-28 22:24:58.851116 SqlalchemyMixin-0.0.8/sqlalchemy_mixins/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      405 2022-10-28 10:07:29.000000 SqlalchemyMixin-0.0.8/sqlalchemy_mixins/__init__.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      341 2022-10-28 22:02:26.000000 SqlalchemyMixin-0.0.8/sqlalchemy_mixins/active_record.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     5009 2022-10-28 22:24:36.000000 SqlalchemyMixin-0.0.8/sqlalchemy_mixins/crud_mixin.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1725 2022-10-27 19:06:09.000000 SqlalchemyMixin-0.0.8/sqlalchemy_mixins/date_mixin.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     3935 2022-10-27 17:52:38.000000 SqlalchemyMixin-0.0.8/sqlalchemy_mixins/eager_load.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      305 2022-10-27 17:54:04.000000 SqlalchemyMixin-0.0.8/sqlalchemy_mixins/image_mixin.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1819 2022-10-27 17:48:30.000000 SqlalchemyMixin-0.0.8/sqlalchemy_mixins/inspection_mixin.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1538 2022-10-27 17:45:12.000000 SqlalchemyMixin-0.0.8/sqlalchemy_mixins/repr_mixin.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      780 2022-10-27 17:38:37.000000 SqlalchemyMixin-0.0.8/sqlalchemy_mixins/session_mixin.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)    16505 2022-10-27 17:57:03.000000 SqlalchemyMixin-0.0.8/sqlalchemy_mixins/smart_query.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      320 2022-10-27 19:46:38.000000 SqlalchemyMixin-0.0.8/sqlalchemy_mixins/user_mixin.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     2545 2022-10-28 19:25:41.000000 SqlalchemyMixin-0.0.8/sqlalchemy_mixins/util.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2022-10-28 22:53:04.642600 SqlalchemyMixin-0.0.9/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1071 2022-10-16 19:39:29.000000 SqlalchemyMixin-0.0.9/LICENSE
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)    13822 2022-10-28 22:53:04.642424 SqlalchemyMixin-0.0.9/PKG-INFO
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)    13094 2022-10-28 19:30:20.000000 SqlalchemyMixin-0.0.9/README.md
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2022-10-28 22:53:04.637478 SqlalchemyMixin-0.0.9/SqlalchemyMixin.egg-info/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)    13822 2022-10-28 22:53:04.000000 SqlalchemyMixin-0.0.9/SqlalchemyMixin.egg-info/PKG-INFO
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      610 2022-10-28 22:53:04.000000 SqlalchemyMixin-0.0.9/SqlalchemyMixin.egg-info/SOURCES.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        1 2022-10-28 22:53:04.000000 SqlalchemyMixin-0.0.9/SqlalchemyMixin.egg-info/dependency_links.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)       75 2022-10-28 22:53:04.000000 SqlalchemyMixin-0.0.9/SqlalchemyMixin.egg-info/requires.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)       18 2022-10-28 22:53:04.000000 SqlalchemyMixin-0.0.9/SqlalchemyMixin.egg-info/top_level.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)       38 2022-10-28 22:53:04.642649 SqlalchemyMixin-0.0.9/setup.cfg
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1274 2022-10-28 22:52:32.000000 SqlalchemyMixin-0.0.9/setup.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2022-10-28 22:53:04.642048 SqlalchemyMixin-0.0.9/sqlalchemy_mixins/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      405 2022-10-28 10:07:29.000000 SqlalchemyMixin-0.0.9/sqlalchemy_mixins/__init__.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      561 2022-10-28 22:42:38.000000 SqlalchemyMixin-0.0.9/sqlalchemy_mixins/active_record.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     5002 2022-10-28 22:44:23.000000 SqlalchemyMixin-0.0.9/sqlalchemy_mixins/crud_mixin.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1725 2022-10-27 19:06:09.000000 SqlalchemyMixin-0.0.9/sqlalchemy_mixins/date_mixin.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     3935 2022-10-27 17:52:38.000000 SqlalchemyMixin-0.0.9/sqlalchemy_mixins/eager_load.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      305 2022-10-27 17:54:04.000000 SqlalchemyMixin-0.0.9/sqlalchemy_mixins/image_mixin.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1819 2022-10-27 17:48:30.000000 SqlalchemyMixin-0.0.9/sqlalchemy_mixins/inspection_mixin.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1538 2022-10-27 17:45:12.000000 SqlalchemyMixin-0.0.9/sqlalchemy_mixins/repr_mixin.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      780 2022-10-27 17:38:37.000000 SqlalchemyMixin-0.0.9/sqlalchemy_mixins/session_mixin.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)    16505 2022-10-27 17:57:03.000000 SqlalchemyMixin-0.0.9/sqlalchemy_mixins/smart_query.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      320 2022-10-27 19:46:38.000000 SqlalchemyMixin-0.0.9/sqlalchemy_mixins/user_mixin.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     2545 2022-10-28 19:25:41.000000 SqlalchemyMixin-0.0.9/sqlalchemy_mixins/util.py
```

### Comparing `SqlalchemyMixin-0.0.8/LICENSE` & `SqlalchemyMixin-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `SqlalchemyMixin-0.0.8/PKG-INFO` & `SqlalchemyMixin-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SqlalchemyMixin
-Version: 0.0.8
+Version: 0.0.9
 Summary: Active Record, Django-like queries, nested eager load and beauty __repr__ for SQLAlchemy
 Home-page: https://github.com/blueromans/sqlalchemy_mixin.git
 Author: Yaşar Özyurt
 Author-email: blueromans@gmail.com
 Project-URL: Bug Tracker, https://github.com/blueromans/sqlalchemy_mixin/issues
 Keywords: sqlalchemy,active record,activerecord,orm,django-like,django,eager load,eagerload,repr,__repr__,mysql,postgresql,pymysql,sqlite
 Classifier: Programming Language :: Python :: 3
```

### Comparing `SqlalchemyMixin-0.0.8/README.md` & `SqlalchemyMixin-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `SqlalchemyMixin-0.0.8/SqlalchemyMixin.egg-info/PKG-INFO` & `SqlalchemyMixin-0.0.9/SqlalchemyMixin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SqlalchemyMixin
-Version: 0.0.8
+Version: 0.0.9
 Summary: Active Record, Django-like queries, nested eager load and beauty __repr__ for SQLAlchemy
 Home-page: https://github.com/blueromans/sqlalchemy_mixin.git
 Author: Yaşar Özyurt
 Author-email: blueromans@gmail.com
 Project-URL: Bug Tracker, https://github.com/blueromans/sqlalchemy_mixin/issues
 Keywords: sqlalchemy,active record,activerecord,orm,django-like,django,eager load,eagerload,repr,__repr__,mysql,postgresql,pymysql,sqlite
 Classifier: Programming Language :: Python :: 3
```

### Comparing `SqlalchemyMixin-0.0.8/SqlalchemyMixin.egg-info/SOURCES.txt` & `SqlalchemyMixin-0.0.9/SqlalchemyMixin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SqlalchemyMixin-0.0.8/setup.py` & `SqlalchemyMixin-0.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name='SqlalchemyMixin',
-    version="0.0.8",
+    version="0.0.9",
     author="Yaşar Özyurt",
     author_email="blueromans@gmail.com",
     description='Active Record, Django-like queries, nested eager load '
                 'and beauty __repr__ for SQLAlchemy',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/blueromans/sqlalchemy_mixin.git',
@@ -21,14 +21,15 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
         "SQLAlchemy >= 1.0",
         "six",
+        "python-slugify",
         "arrow",
         "typing; python_version < '3.5'"
     ],
     keywords=['sqlalchemy', 'active record', 'activerecord', 'orm',
               'django-like', 'django', 'eager load', 'eagerload', 'repr',
               '__repr__', 'mysql', 'postgresql', 'pymysql', 'sqlite'],
     packages=['sqlalchemy_mixins'],
```

### Comparing `SqlalchemyMixin-0.0.8/sqlalchemy_mixins/crud_mixin.py` & `SqlalchemyMixin-0.0.9/sqlalchemy_mixins/crud_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
     @classmethod
     def create(cls, **kwargs):
         """Create and persist a new record for the model
         :param kwargs: attributes for the record
         :return: the new model instance
         """
-        return cls().fill(**kwargs).save()
+        return cls(**kwargs).save()
 
     def update(self, **kwargs):
         """Same as :meth:`fill` method but persists changes to database.
         """
         return self.fill(**kwargs).save()
 
     def delete(self):
```

### Comparing `SqlalchemyMixin-0.0.8/sqlalchemy_mixins/date_mixin.py` & `SqlalchemyMixin-0.0.9/sqlalchemy_mixins/date_mixin.py`

 * *Files identical despite different names*

### Comparing `SqlalchemyMixin-0.0.8/sqlalchemy_mixins/eager_load.py` & `SqlalchemyMixin-0.0.9/sqlalchemy_mixins/eager_load.py`

 * *Files identical despite different names*

### Comparing `SqlalchemyMixin-0.0.8/sqlalchemy_mixins/inspection_mixin.py` & `SqlalchemyMixin-0.0.9/sqlalchemy_mixins/inspection_mixin.py`

 * *Files identical despite different names*

### Comparing `SqlalchemyMixin-0.0.8/sqlalchemy_mixins/repr_mixin.py` & `SqlalchemyMixin-0.0.9/sqlalchemy_mixins/repr_mixin.py`

 * *Files identical despite different names*

### Comparing `SqlalchemyMixin-0.0.8/sqlalchemy_mixins/session_mixin.py` & `SqlalchemyMixin-0.0.9/sqlalchemy_mixins/session_mixin.py`

 * *Files identical despite different names*

### Comparing `SqlalchemyMixin-0.0.8/sqlalchemy_mixins/smart_query.py` & `SqlalchemyMixin-0.0.9/sqlalchemy_mixins/smart_query.py`

 * *Files identical despite different names*

### Comparing `SqlalchemyMixin-0.0.8/sqlalchemy_mixins/util.py` & `SqlalchemyMixin-0.0.9/sqlalchemy_mixins/util.py`

 * *Files identical despite different names*

