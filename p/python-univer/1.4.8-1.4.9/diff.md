# Comparing `tmp/python-univer-1.4.8.tar.gz` & `tmp/python-univer-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-univer-1.4.8.tar", last modified: Fri Jul 28 06:37:53 2023, max compression
+gzip compressed data, was "python-univer-1.4.9.tar", last modified: Sun Jul 30 20:31:17 2023, max compression
```

## Comparing `python-univer-1.4.8.tar` & `python-univer-1.4.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 user      (1000) user      (1001)        0 2023-07-28 06:37:53.146666 python-univer-1.4.8/
--rw-r--r--   0 user      (1000) user      (1001)        0 2023-07-18 16:09:38.000000 python-univer-1.4.8/LICENSE
--rw-r--r--   0 user      (1000) user      (1001)     1231 2023-07-28 06:37:53.146666 python-univer-1.4.8/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1001)      706 2023-07-18 16:09:38.000000 python-univer-1.4.8/README.md
-drwxr-xr-x   0 user      (1000) user      (1001)        0 2023-07-28 06:37:53.116666 python-univer-1.4.8/python_univer.egg-info/
--rw-r--r--   0 user      (1000) user      (1001)     1231 2023-07-28 06:37:52.000000 python-univer-1.4.8/python_univer.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1001)      765 2023-07-28 06:37:52.000000 python-univer-1.4.8/python_univer.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1001)        1 2023-07-28 06:37:52.000000 python-univer-1.4.8/python_univer.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1001)       18 2023-07-28 06:37:52.000000 python-univer-1.4.8/python_univer.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1001)       10 2023-07-28 06:37:52.000000 python-univer-1.4.8/python_univer.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1001)       38 2023-07-28 06:37:53.146666 python-univer-1.4.8/setup.cfg
--rw-r--r--   0 user      (1000) user      (1001)      827 2023-07-28 06:37:05.000000 python-univer-1.4.8/setup.py
-drwxr-xr-x   0 user      (1000) user      (1001)        0 2023-07-28 06:37:53.119999 python-univer-1.4.8/univer_db/
--rw-r--r--   0 user      (1000) user      (1001)        0 2023-07-18 16:09:38.000000 python-univer-1.4.8/univer_db/__init__.py
--rw-r--r--   0 user      (1000) user      (1001)      472 2023-07-18 16:09:38.000000 python-univer-1.4.8/univer_db/config.py
-drwxr-xr-x   0 user      (1000) user      (1001)        0 2023-07-28 06:37:53.143333 python-univer-1.4.8/univer_db/models/
--rw-r--r--   0 user      (1000) user      (1001)      253 2023-07-28 06:36:00.000000 python-univer-1.4.8/univer_db/models/__init__.py
--rw-r--r--   0 user      (1000) user      (1001)     9276 2023-07-25 23:49:51.000000 python-univer-1.4.8/univer_db/models/base.py
--rw-r--r--   0 user      (1000) user      (1001)     4523 2023-07-28 06:35:35.000000 python-univer-1.4.8/univer_db/models/certificates.py
--rw-r--r--   0 user      (1000) user      (1001)     8231 2023-07-18 16:09:38.000000 python-univer-1.4.8/univer_db/models/dormitories.py
--rw-r--r--   0 user      (1000) user      (1001)     1888 2023-07-25 23:43:54.000000 python-univer-1.4.8/univer_db/models/geo.py
--rw-r--r--   0 user      (1000) user      (1001)      951 2023-07-18 16:09:38.000000 python-univer-1.4.8/univer_db/models/grades.py
--rw-r--r--   0 user      (1000) user      (1001)        0 2023-07-18 16:09:38.000000 python-univer-1.4.8/univer_db/models/groups.py
--rw-r--r--   0 user      (1000) user      (1001)    35417 2023-07-25 23:50:41.000000 python-univer-1.4.8/univer_db/models/models.py
--rw-r--r--   0 user      (1000) user      (1001)     9229 2023-07-25 23:49:39.000000 python-univer-1.4.8/univer_db/models/orders.py
--rw-r--r--   0 user      (1000) user      (1001)    25491 2023-07-25 23:48:54.000000 python-univer-1.4.8/univer_db/models/roles.py
--rw-r--r--   0 user      (1000) user      (1001)     4194 2023-07-25 23:48:54.000000 python-univer-1.4.8/univer_db/models/schedule.py
--rw-r--r--   0 user      (1000) user      (1001)     3573 2023-07-25 23:48:09.000000 python-univer-1.4.8/univer_db/models/sheets.py
--rw-r--r--   0 user      (1000) user      (1001)     5071 2023-07-25 23:46:52.000000 python-univer-1.4.8/univer_db/models/structures.py
--rw-r--r--   0 user      (1000) user      (1001)      769 2023-07-18 16:09:38.000000 python-univer-1.4.8/univer_db/orm.py
-drwxr-xr-x   0 user      (1000) user      (1001)        0 2023-07-28 06:37:53.143333 python-univer-1.4.8/univer_db/tests/
--rw-r--r--   0 user      (1000) user      (1001)      264 2023-07-18 16:09:38.000000 python-univer-1.4.8/univer_db/tests/__init__.py
--rw-r--r--   0 user      (1000) user      (1001)      569 2023-07-18 16:09:38.000000 python-univer-1.4.8/univer_db/tests/geo.py
--rw-r--r--   0 user      (1000) user      (1001)     2635 2023-07-18 16:09:38.000000 python-univer-1.4.8/univer_db/tests/models.py
--rw-r--r--   0 user      (1000) user      (1001)     1136 2023-07-18 16:09:38.000000 python-univer-1.4.8/univer_db/tests/roles.py
--rw-r--r--   0 user      (1000) user      (1001)      624 2023-07-18 16:09:38.000000 python-univer-1.4.8/univer_db/tests/structures.py
+drwxr-xr-x   0 user      (1000) user      (1001)        0 2023-07-30 20:31:17.469999 python-univer-1.4.9/
+-rw-r--r--   0 user      (1000) user      (1001)        0 2023-07-18 16:09:38.000000 python-univer-1.4.9/LICENSE
+-rw-r--r--   0 user      (1000) user      (1001)     1231 2023-07-30 20:31:17.469999 python-univer-1.4.9/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1001)      706 2023-07-18 16:09:38.000000 python-univer-1.4.9/README.md
+drwxr-xr-x   0 user      (1000) user      (1001)        0 2023-07-30 20:31:17.349999 python-univer-1.4.9/python_univer.egg-info/
+-rw-r--r--   0 user      (1000) user      (1001)     1231 2023-07-30 20:31:17.000000 python-univer-1.4.9/python_univer.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1001)      765 2023-07-30 20:31:17.000000 python-univer-1.4.9/python_univer.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1001)        1 2023-07-30 20:31:17.000000 python-univer-1.4.9/python_univer.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1001)       18 2023-07-30 20:31:17.000000 python-univer-1.4.9/python_univer.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1001)       10 2023-07-30 20:31:17.000000 python-univer-1.4.9/python_univer.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1001)       38 2023-07-30 20:31:17.469999 python-univer-1.4.9/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1001)      827 2023-07-30 20:30:55.000000 python-univer-1.4.9/setup.py
+drwxr-xr-x   0 user      (1000) user      (1001)        0 2023-07-30 20:31:17.353332 python-univer-1.4.9/univer_db/
+-rw-r--r--   0 user      (1000) user      (1001)        0 2023-07-18 16:09:38.000000 python-univer-1.4.9/univer_db/__init__.py
+-rw-r--r--   0 user      (1000) user      (1001)      472 2023-07-18 16:09:38.000000 python-univer-1.4.9/univer_db/config.py
+drwxr-xr-x   0 user      (1000) user      (1001)        0 2023-07-30 20:31:17.469999 python-univer-1.4.9/univer_db/models/
+-rw-r--r--   0 user      (1000) user      (1001)      253 2023-07-28 06:36:00.000000 python-univer-1.4.9/univer_db/models/__init__.py
+-rw-r--r--   0 user      (1000) user      (1001)     9276 2023-07-25 23:49:51.000000 python-univer-1.4.9/univer_db/models/base.py
+-rw-r--r--   0 user      (1000) user      (1001)     4522 2023-07-30 20:30:44.000000 python-univer-1.4.9/univer_db/models/certificates.py
+-rw-r--r--   0 user      (1000) user      (1001)     8231 2023-07-18 16:09:38.000000 python-univer-1.4.9/univer_db/models/dormitories.py
+-rw-r--r--   0 user      (1000) user      (1001)     1888 2023-07-25 23:43:54.000000 python-univer-1.4.9/univer_db/models/geo.py
+-rw-r--r--   0 user      (1000) user      (1001)      951 2023-07-18 16:09:38.000000 python-univer-1.4.9/univer_db/models/grades.py
+-rw-r--r--   0 user      (1000) user      (1001)        0 2023-07-18 16:09:38.000000 python-univer-1.4.9/univer_db/models/groups.py
+-rw-r--r--   0 user      (1000) user      (1001)    35417 2023-07-25 23:50:41.000000 python-univer-1.4.9/univer_db/models/models.py
+-rw-r--r--   0 user      (1000) user      (1001)     9229 2023-07-25 23:49:39.000000 python-univer-1.4.9/univer_db/models/orders.py
+-rw-r--r--   0 user      (1000) user      (1001)    25491 2023-07-25 23:48:54.000000 python-univer-1.4.9/univer_db/models/roles.py
+-rw-r--r--   0 user      (1000) user      (1001)     4194 2023-07-25 23:48:54.000000 python-univer-1.4.9/univer_db/models/schedule.py
+-rw-r--r--   0 user      (1000) user      (1001)     3573 2023-07-25 23:48:09.000000 python-univer-1.4.9/univer_db/models/sheets.py
+-rw-r--r--   0 user      (1000) user      (1001)     5071 2023-07-25 23:46:52.000000 python-univer-1.4.9/univer_db/models/structures.py
+-rw-r--r--   0 user      (1000) user      (1001)      769 2023-07-18 16:09:38.000000 python-univer-1.4.9/univer_db/orm.py
+drwxr-xr-x   0 user      (1000) user      (1001)        0 2023-07-30 20:31:17.469999 python-univer-1.4.9/univer_db/tests/
+-rw-r--r--   0 user      (1000) user      (1001)      264 2023-07-18 16:09:38.000000 python-univer-1.4.9/univer_db/tests/__init__.py
+-rw-r--r--   0 user      (1000) user      (1001)      569 2023-07-18 16:09:38.000000 python-univer-1.4.9/univer_db/tests/geo.py
+-rw-r--r--   0 user      (1000) user      (1001)     2635 2023-07-18 16:09:38.000000 python-univer-1.4.9/univer_db/tests/models.py
+-rw-r--r--   0 user      (1000) user      (1001)     1136 2023-07-18 16:09:38.000000 python-univer-1.4.9/univer_db/tests/roles.py
+-rw-r--r--   0 user      (1000) user      (1001)      624 2023-07-18 16:09:38.000000 python-univer-1.4.9/univer_db/tests/structures.py
```

### Comparing `python-univer-1.4.8/PKG-INFO` & `python-univer-1.4.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-univer
-Version: 1.4.8
+Version: 1.4.9
 Summary: Данная библиотека содержит SqlAlchemy ORM для системы Univer
 Home-page: https://github.com/yessenovuniversity/python_univer
 Author: Nauryzbek Aitbayev
 Author-email: nauryzbek.aitbayev@yu.edu.kz
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `python-univer-1.4.8/README.md` & `python-univer-1.4.9/README.md`

 * *Files identical despite different names*

### Comparing `python-univer-1.4.8/python_univer.egg-info/PKG-INFO` & `python-univer-1.4.9/python_univer.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-univer
-Version: 1.4.8
+Version: 1.4.9
 Summary: Данная библиотека содержит SqlAlchemy ORM для системы Univer
 Home-page: https://github.com/yessenovuniversity/python_univer
 Author: Nauryzbek Aitbayev
 Author-email: nauryzbek.aitbayev@yu.edu.kz
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `python-univer-1.4.8/python_univer.egg-info/SOURCES.txt` & `python-univer-1.4.9/python_univer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-univer-1.4.8/setup.py` & `python-univer-1.4.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="python-univer",
-    version="1.4.8",
+    version="1.4.9",
     author="Nauryzbek Aitbayev",
     author_email="nauryzbek.aitbayev@yu.edu.kz",
     description="Данная библиотека содержит SqlAlchemy ORM для системы Univer",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/yessenovuniversity/python_univer",
     packages=setuptools.find_packages(),
```

### Comparing `python-univer-1.4.8/univer_db/models/base.py` & `python-univer-1.4.9/univer_db/models/base.py`

 * *Files identical despite different names*

### Comparing `python-univer-1.4.8/univer_db/models/certificates.py` & `python-univer-1.4.9/univer_db/models/certificates.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     """Дисциплина в сертификате"""
     __tablename__ = 'univer_certificate_subject'
 
     # Идентификатор
     id = Column('certificate_subject_id', Integer, primary_key=True)
 
     # Академический степень
-    stage_id = Column(ForeignKey('univer_stages.stage_id'))
+    stage_id = Column(ForeignKey('univer_stage.stage_id'))
     stage = relationship('Stage')
 
     # Статус
     status = Column(Integer)
 
     # Наименование дисциплины
     name_ru = Column('certificate_subject_name_ru', Unicode(100))
```

### Comparing `python-univer-1.4.8/univer_db/models/dormitories.py` & `python-univer-1.4.9/univer_db/models/dormitories.py`

 * *Files identical despite different names*

### Comparing `python-univer-1.4.8/univer_db/models/geo.py` & `python-univer-1.4.9/univer_db/models/geo.py`

 * *Files identical despite different names*

### Comparing `python-univer-1.4.8/univer_db/models/grades.py` & `python-univer-1.4.9/univer_db/models/grades.py`

 * *Files identical despite different names*

### Comparing `python-univer-1.4.8/univer_db/models/models.py` & `python-univer-1.4.9/univer_db/models/models.py`

 * *Files identical despite different names*

### Comparing `python-univer-1.4.8/univer_db/models/orders.py` & `python-univer-1.4.9/univer_db/models/orders.py`

 * *Files identical despite different names*

### Comparing `python-univer-1.4.8/univer_db/models/roles.py` & `python-univer-1.4.9/univer_db/models/roles.py`

 * *Files identical despite different names*

### Comparing `python-univer-1.4.8/univer_db/models/schedule.py` & `python-univer-1.4.9/univer_db/models/schedule.py`

 * *Files identical despite different names*

### Comparing `python-univer-1.4.8/univer_db/models/sheets.py` & `python-univer-1.4.9/univer_db/models/sheets.py`

 * *Files identical despite different names*

### Comparing `python-univer-1.4.8/univer_db/models/structures.py` & `python-univer-1.4.9/univer_db/models/structures.py`

 * *Files identical despite different names*

### Comparing `python-univer-1.4.8/univer_db/orm.py` & `python-univer-1.4.9/univer_db/orm.py`

 * *Files identical despite different names*

### Comparing `python-univer-1.4.8/univer_db/tests/geo.py` & `python-univer-1.4.9/univer_db/tests/geo.py`

 * *Files identical despite different names*

### Comparing `python-univer-1.4.8/univer_db/tests/models.py` & `python-univer-1.4.9/univer_db/tests/models.py`

 * *Files identical despite different names*

### Comparing `python-univer-1.4.8/univer_db/tests/roles.py` & `python-univer-1.4.9/univer_db/tests/roles.py`

 * *Files identical despite different names*

### Comparing `python-univer-1.4.8/univer_db/tests/structures.py` & `python-univer-1.4.9/univer_db/tests/structures.py`

 * *Files identical despite different names*

