# Comparing `tmp/django-sequences-2.7.tar.gz` & `tmp/django_sequences-2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-sequences-2.7.tar", max compression
+gzip compressed data, was "django_sequences-2.8.tar", max compression
```

## Comparing `django-sequences-2.7.tar` & `django_sequences-2.8.tar`

### file list

```diff
@@ -1,46 +1,45 @@
--rw-r--r--   0        0        0     1543 2020-06-07 12:39:46.000000 django-sequences-2.7/LICENSE
--rw-r--r--   0        0        0    13319 2022-05-21 08:26:20.622283 django-sequences-2.7/README.rst
--rw-r--r--   0        0        0      940 2022-05-21 08:26:49.987711 django-sequences-2.7/pyproject.toml
--rw-r--r--   0        0        0     4648 2022-05-21 08:25:19.891127 django-sequences-2.7/src/sequences/__init__.py
--rw-r--r--   0        0        0      214 2022-02-19 07:18:40.270136 django-sequences-2.7/src/sequences/admin.py
--rw-r--r--   0        0        0      182 2022-02-19 07:18:40.268071 django-sequences-2.7/src/sequences/apps.py
--rw-r--r--   0        0        0      621 2020-06-07 12:39:46.000000 django-sequences-2.7/src/sequences/locale/bg/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      588 2020-06-07 12:39:46.000000 django-sequences-2.7/src/sequences/locale/bg/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      567 2020-06-07 12:39:46.000000 django-sequences-2.7/src/sequences/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      534 2020-06-07 12:39:46.000000 django-sequences-2.7/src/sequences/locale/cs/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      524 2020-06-07 12:39:46.000000 django-sequences-2.7/src/sequences/locale/da/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      491 2020-06-07 12:39:46.000000 django-sequences-2.7/src/sequences/locale/da/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      523 2020-06-07 12:39:46.000000 django-sequences-2.7/src/sequences/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      490 2020-06-07 12:39:46.000000 django-sequences-2.7/src/sequences/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      530 2020-06-07 12:39:46.000000 django-sequences-2.7/src/sequences/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      497 2020-06-07 12:39:46.000000 django-sequences-2.7/src/sequences/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      529 2020-06-07 12:39:46.000000 django-sequences-2.7/src/sequences/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      496 2020-06-07 12:39:46.000000 django-sequences-2.7/src/sequences/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      523 2020-06-07 12:39:46.000000 django-sequences-2.7/src/sequences/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      490 2020-06-07 12:39:46.000000 django-sequences-2.7/src/sequences/locale/it/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      535 2020-06-07 12:39:46.000000 django-sequences-2.7/src/sequences/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      502 2020-06-07 12:39:46.000000 django-sequences-2.7/src/sequences/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      590 2020-06-07 12:39:46.000000 django-sequences-2.7/src/sequences/locale/lt/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      560 2020-06-07 12:39:46.000000 django-sequences-2.7/src/sequences/locale/lt/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      529 2020-06-07 12:39:46.000000 django-sequences-2.7/src/sequences/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      496 2020-06-07 12:39:46.000000 django-sequences-2.7/src/sequences/locale/nl/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      531 2020-06-07 12:39:46.000000 django-sequences-2.7/src/sequences/locale/pt/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      498 2020-06-07 12:39:46.000000 django-sequences-2.7/src/sequences/locale/pt/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      478 2020-06-07 12:39:46.000000 django-sequences-2.7/src/sequences/locale/rm/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      441 2020-06-07 12:39:46.000000 django-sequences-2.7/src/sequences/locale/rm/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      769 2020-06-07 12:39:46.000000 django-sequences-2.7/src/sequences/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      742 2020-06-07 12:39:46.000000 django-sequences-2.7/src/sequences/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      563 2020-06-07 12:39:46.000000 django-sequences-2.7/src/sequences/locale/sk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      530 2020-06-07 12:39:46.000000 django-sequences-2.7/src/sequences/locale/sk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      524 2020-06-07 12:39:46.000000 django-sequences-2.7/src/sequences/locale/sv/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      491 2020-06-07 12:39:46.000000 django-sequences-2.7/src/sequences/locale/sv/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      660 2020-06-07 12:39:46.000000 django-sequences-2.7/src/sequences/locale/th/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      709 2020-06-07 12:39:46.000000 django-sequences-2.7/src/sequences/locale/th/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      594 2020-06-07 12:39:46.000000 django-sequences-2.7/src/sequences/locale/tr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      848 2020-06-07 12:39:46.000000 django-sequences-2.7/src/sequences/locale/tr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      874 2022-02-19 07:18:40.280374 django-sequences-2.7/src/sequences/migrations/0001_initial.py
--rw-r--r--   0        0        0      354 2022-05-21 08:02:39.035378 django-sequences-2.7/src/sequences/migrations/0002_alter_sequence_last.py
--rw-r--r--   0        0        0        0 2020-06-07 12:39:46.000000 django-sequences-2.7/src/sequences/migrations/__init__.py
--rw-r--r--   0        0        0      512 2022-05-21 08:02:39.035715 django-sequences-2.7/src/sequences/models.py
--rw-r--r--   0        0        0    15315 2022-05-21 08:28:02.116528 django-sequences-2.7/setup.py
--rw-r--r--   0        0        0    14340 2022-05-21 08:28:02.117009 django-sequences-2.7/PKG-INFO
+-rw-r--r--   0        0        0     1543 2020-06-07 12:39:46.000000 django_sequences-2.8/LICENSE
+-rw-r--r--   0        0        0    13942 2023-07-30 07:38:18.938075 django_sequences-2.8/README.rst
+-rw-r--r--   0        0        0     1019 2023-07-30 07:38:28.512083 django_sequences-2.8/pyproject.toml
+-rw-r--r--   0        0        0     4613 2023-05-05 06:42:53.495806 django_sequences-2.8/src/sequences/__init__.py
+-rw-r--r--   0        0        0      213 2023-05-05 06:42:53.495990 django_sequences-2.8/src/sequences/admin.py
+-rw-r--r--   0        0        0      182 2022-02-19 07:18:40.268071 django_sequences-2.8/src/sequences/apps.py
+-rw-r--r--   0        0        0      621 2020-06-07 12:39:46.000000 django_sequences-2.8/src/sequences/locale/bg/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      588 2020-06-07 12:39:46.000000 django_sequences-2.8/src/sequences/locale/bg/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      567 2020-06-07 12:39:46.000000 django_sequences-2.8/src/sequences/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      534 2020-06-07 12:39:46.000000 django_sequences-2.8/src/sequences/locale/cs/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      524 2020-06-07 12:39:46.000000 django_sequences-2.8/src/sequences/locale/da/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      491 2020-06-07 12:39:46.000000 django_sequences-2.8/src/sequences/locale/da/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      523 2020-06-07 12:39:46.000000 django_sequences-2.8/src/sequences/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      490 2020-06-07 12:39:46.000000 django_sequences-2.8/src/sequences/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      530 2020-06-07 12:39:46.000000 django_sequences-2.8/src/sequences/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      497 2020-06-07 12:39:46.000000 django_sequences-2.8/src/sequences/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      529 2020-06-07 12:39:46.000000 django_sequences-2.8/src/sequences/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      496 2020-06-07 12:39:46.000000 django_sequences-2.8/src/sequences/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      523 2020-06-07 12:39:46.000000 django_sequences-2.8/src/sequences/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      490 2020-06-07 12:39:46.000000 django_sequences-2.8/src/sequences/locale/it/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      535 2020-06-07 12:39:46.000000 django_sequences-2.8/src/sequences/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      502 2020-06-07 12:39:46.000000 django_sequences-2.8/src/sequences/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      590 2020-06-07 12:39:46.000000 django_sequences-2.8/src/sequences/locale/lt/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      560 2020-06-07 12:39:46.000000 django_sequences-2.8/src/sequences/locale/lt/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      529 2020-06-07 12:39:46.000000 django_sequences-2.8/src/sequences/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      496 2020-06-07 12:39:46.000000 django_sequences-2.8/src/sequences/locale/nl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      531 2020-06-07 12:39:46.000000 django_sequences-2.8/src/sequences/locale/pt/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      498 2020-06-07 12:39:46.000000 django_sequences-2.8/src/sequences/locale/pt/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      478 2020-06-07 12:39:46.000000 django_sequences-2.8/src/sequences/locale/rm/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      441 2020-06-07 12:39:46.000000 django_sequences-2.8/src/sequences/locale/rm/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      769 2020-06-07 12:39:46.000000 django_sequences-2.8/src/sequences/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      742 2020-06-07 12:39:46.000000 django_sequences-2.8/src/sequences/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      563 2020-06-07 12:39:46.000000 django_sequences-2.8/src/sequences/locale/sk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      530 2020-06-07 12:39:46.000000 django_sequences-2.8/src/sequences/locale/sk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      524 2020-06-07 12:39:46.000000 django_sequences-2.8/src/sequences/locale/sv/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      491 2020-06-07 12:39:46.000000 django_sequences-2.8/src/sequences/locale/sv/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      660 2020-06-07 12:39:46.000000 django_sequences-2.8/src/sequences/locale/th/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      709 2020-06-07 12:39:46.000000 django_sequences-2.8/src/sequences/locale/th/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      594 2020-06-07 12:39:46.000000 django_sequences-2.8/src/sequences/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      848 2020-06-07 12:39:46.000000 django_sequences-2.8/src/sequences/locale/tr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      873 2023-05-05 06:42:53.496167 django_sequences-2.8/src/sequences/migrations/0001_initial.py
+-rw-r--r--   0        0        0      353 2023-05-05 06:42:53.496345 django_sequences-2.8/src/sequences/migrations/0002_alter_sequence_last.py
+-rw-r--r--   0        0        0        0 2020-06-07 12:39:46.000000 django_sequences-2.8/src/sequences/migrations/__init__.py
+-rw-r--r--   0        0        0      511 2023-05-05 06:42:53.496515 django_sequences-2.8/src/sequences/models.py
+-rw-r--r--   0        0        0    15092 1970-01-01 00:00:00.000000 django_sequences-2.8/PKG-INFO
```

### Comparing `django-sequences-2.7/LICENSE` & `django_sequences-2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `django-sequences-2.7/README.rst` & `django_sequences-2.8/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -53,25 +53,26 @@
 of django-sequences apply only if you call** ``get_next_value`` **and save its
 return value to the database within the same transaction!**
 
 Table of contents
 =================
 
 * `Getting started`_
+* `API`_
 * `Database support`_
 * `Multiple databases`_
 * `Isolation levels`_
 * `Contributing`_
 * `Releasing`_
 * `Changelog`_
 
 Getting started
 ===============
 
-django-sequences is tested with Django 3.2 (LTS) and 4.0.
+django-sequences is tested with Django 3.2 (LTS), 4.0, 4.1, and 4.2.
 It is also tested with all database backends built-in to Django: MySQL/MariaDB,
 Oracle, PostgreSQL and SQLite.
 
 It is released under the BSD license, like Django itself.
 
 Install django-sequences:
 
@@ -298,14 +299,36 @@
     Sequence.get_last_value(
         self,
     )
 
 All parameters have the same meaning as in the ``get_next_value`` and
 ``get_last_value`` functions.
 
+Examples
+========
+
+Per-date sequences
+------------------
+
+If you want independent sequences per day, month, or year, use the appropriate
+date fragment in the sequence name. For example:
+
+.. code:: python
+
+    from django.utils import timezone
+    from sequences import get_next_value
+
+    # Per-day sequence
+    get_next_value(f"books-{timezone.now().date().isoformat()}")
+    # Per-year sequence
+    get_next_value(f"prototocol-{timezone.now().year}")
+
+The above calls will result in separate sequences like ``books-2023-03-15``
+or ``protocol-2022``, respectively.
+
 Database support
 ================
 
 django-sequences is tested on PostgreSQL, MariaDB / MySQL, Oracle, and SQLite.
 
 MySQL only supports the ``nowait`` parameter from version 8.0.1.
 MariaDB only supports ``nowait`` from version 10.3.
@@ -431,14 +454,19 @@
 
     $ poetry build
     $ poetry publish
 
 Changelog
 =========
 
+2.8
+---
+
+* No significant changes.
+
 2.7
 ---
 
 * Sequence values can go up to ``2 ** 63 - 1`` instead of ``2 ** 31 - 1``
   previously. The exact limit depends on the database backend.
 
   Migration ``0002_alter_sequence_last.py`` changes the field storing sequence
```

### Comparing `django-sequences-2.7/src/sequences/__init__.py` & `django_sequences-2.8/src/sequences/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,34 +70,28 @@
 
     if using is None:
         using = router.db_for_write(Sequence)
 
     connection = connections[using]
     db_table = connection.ops.quote_name(Sequence._meta.db_table)
 
-    if (
-        connection.vendor == "postgresql"
-        and reset_value is None
-        and not nowait
-    ):
-
+    if connection.vendor == "postgresql" and reset_value is None and not nowait:
         # PostgreSQL ≥ 9.5 supports "upsert".
         # This is about 3x faster as the naive implementation.
 
         with connection.cursor() as cursor:
             cursor.execute(
                 POSTGRESQL_UPSERT.format(db_table=db_table),
                 [sequence_name, initial_value],
             ),
             result = cursor.fetchone()
 
         return result[0]
 
     elif connection.vendor == "mysql" and reset_value is None and not nowait:
-
         # MySQL supports "upsert" but not "returning".
         # This is about 2x faster as the naive implementation.
 
         with transaction.atomic(using=using, savepoint=False):
             with connection.cursor() as cursor:
                 cursor.execute(
                     MYSQL_UPSERT.format(db_table=db_table),
@@ -108,15 +102,14 @@
                     [sequence_name],
                 )
                 result = cursor.fetchone()
 
         return result[0]
 
     else:
-
         # Default, ORM-based implementation for all other cases.
 
         with transaction.atomic(using=using, savepoint=False):
             sequences = Sequence.objects.select_for_update(nowait=nowait)
             sequence, created = sequences.get_or_create(
                 name=sequence_name,
                 defaults={"last": initial_value},
```

### Comparing `django-sequences-2.7/src/sequences/locale/bg/LC_MESSAGES/django.mo` & `django_sequences-2.8/src/sequences/locale/bg/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-sequences-2.7/src/sequences/locale/bg/LC_MESSAGES/django.po` & `django_sequences-2.8/src/sequences/locale/bg/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-sequences-2.7/src/sequences/locale/cs/LC_MESSAGES/django.mo` & `django_sequences-2.8/src/sequences/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-sequences-2.7/src/sequences/locale/cs/LC_MESSAGES/django.po` & `django_sequences-2.8/src/sequences/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-sequences-2.7/src/sequences/locale/da/LC_MESSAGES/django.mo` & `django_sequences-2.8/src/sequences/locale/da/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-sequences-2.7/src/sequences/locale/de/LC_MESSAGES/django.mo` & `django_sequences-2.8/src/sequences/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-sequences-2.7/src/sequences/locale/es/LC_MESSAGES/django.mo` & `django_sequences-2.8/src/sequences/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-sequences-2.7/src/sequences/locale/fr/LC_MESSAGES/django.mo` & `django_sequences-2.8/src/sequences/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-sequences-2.7/src/sequences/locale/it/LC_MESSAGES/django.mo` & `django_sequences-2.8/src/sequences/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-sequences-2.7/src/sequences/locale/ja/LC_MESSAGES/django.mo` & `django_sequences-2.8/src/sequences/locale/ja/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-sequences-2.7/src/sequences/locale/lt/LC_MESSAGES/django.mo` & `django_sequences-2.8/src/sequences/locale/lt/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-sequences-2.7/src/sequences/locale/lt/LC_MESSAGES/django.po` & `django_sequences-2.8/src/sequences/locale/lt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-sequences-2.7/src/sequences/locale/nl/LC_MESSAGES/django.mo` & `django_sequences-2.8/src/sequences/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-sequences-2.7/src/sequences/locale/pt/LC_MESSAGES/django.mo` & `django_sequences-2.8/src/sequences/locale/pt/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-sequences-2.7/src/sequences/locale/ru/LC_MESSAGES/django.mo` & `django_sequences-2.8/src/sequences/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-sequences-2.7/src/sequences/locale/ru/LC_MESSAGES/django.po` & `django_sequences-2.8/src/sequences/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-sequences-2.7/src/sequences/locale/sk/LC_MESSAGES/django.mo` & `django_sequences-2.8/src/sequences/locale/sk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-sequences-2.7/src/sequences/locale/sk/LC_MESSAGES/django.po` & `django_sequences-2.8/src/sequences/locale/sk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-sequences-2.7/src/sequences/locale/sv/LC_MESSAGES/django.mo` & `django_sequences-2.8/src/sequences/locale/sv/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-sequences-2.7/src/sequences/locale/th/LC_MESSAGES/django.mo` & `django_sequences-2.8/src/sequences/locale/th/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-sequences-2.7/src/sequences/locale/th/LC_MESSAGES/django.po` & `django_sequences-2.8/src/sequences/locale/th/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-sequences-2.7/src/sequences/locale/tr/LC_MESSAGES/django.mo` & `django_sequences-2.8/src/sequences/locale/tr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-sequences-2.7/src/sequences/locale/tr/LC_MESSAGES/django.po` & `django_sequences-2.8/src/sequences/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-sequences-2.7/src/sequences/migrations/0001_initial.py` & `django_sequences-2.8/src/sequences/migrations/0001_initial.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     initial = True
 
     dependencies = []
 
     operations = [
         migrations.CreateModel(
             name="Sequence",
```

### Comparing `django-sequences-2.7/setup.py` & `django_sequences-2.8/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,51 +1,556 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: django-sequences
+Version: 2.8
+Summary: Generate gapless sequences of integer values.
+Home-page: https://github.com/aaugustin/django-sequences
+License: BSD-3-Clause
+Author: Aymeric Augustin
+Author-email: aymeric.augustin@m4x.org
+Requires-Python: >=3.6.2
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Web Environment
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: django (>=3.2)
+Project-URL: Repository, https://github.com/aaugustin/django-sequences
+Description-Content-Type: text/x-rst
 
-package_dir = \
-{'': 'src'}
+django-sequences
+################
 
-packages = \
-['sequences', 'sequences.migrations']
+By default, Django gives each model an auto-incrementing integer primary key.
+These primary keys look like they generate a continuous sequence of integers.
 
-package_data = \
-{'': ['*'],
- 'sequences': ['locale/bg/LC_MESSAGES/*',
-               'locale/cs/LC_MESSAGES/*',
-               'locale/da/LC_MESSAGES/*',
-               'locale/de/LC_MESSAGES/*',
-               'locale/es/LC_MESSAGES/*',
-               'locale/fr/LC_MESSAGES/*',
-               'locale/it/LC_MESSAGES/*',
-               'locale/ja/LC_MESSAGES/*',
-               'locale/lt/LC_MESSAGES/*',
-               'locale/nl/LC_MESSAGES/*',
-               'locale/pt/LC_MESSAGES/*',
-               'locale/rm/LC_MESSAGES/*',
-               'locale/ru/LC_MESSAGES/*',
-               'locale/sk/LC_MESSAGES/*',
-               'locale/sv/LC_MESSAGES/*',
-               'locale/th/LC_MESSAGES/*',
-               'locale/tr/LC_MESSAGES/*']}
-
-install_requires = \
-['django>=3.2']
-
-setup_kwargs = {
-    'name': 'django-sequences',
-    'version': '2.7',
-    'description': 'Generate gapless sequences of integer values.',
-    'long_description': 'django-sequences\n################\n\nBy default, Django gives each model an auto-incrementing integer primary key.\nThese primary keys look like they generate a continuous sequence of integers.\n\nHowever, this behavior isn\'t guaranteed.\n\nIf a transaction inserts a row and then is rolled back, the sequence counter\nisn\'t rolled back for performance reasons, creating a gap in primary keys.\n\nSuch gaps may happen on all databases natively supported by Django:\n\n* `PostgreSQL <https://www.postgresql.org/docs/current/datatype-numeric.html#DATATYPE-SERIAL>`_\n* `MariaDB <https://mariadb.com/kb/en/auto_increment/#missing-values>`_ / MySQL\n* `Oracle <https://docs.oracle.com/en/database/oracle/oracle-database/21/sqlrf/CREATE-SEQUENCE.html>`_\n* `SQLite <https://sqlite.org/autoinc.html#the_autoincrement_keyword>`_\n\nThey may also happen on most databases supported via third-party backends.\n\nThis can cause compliance issues for some use cases such as accounting.\n\nThis risk isn\'t well known. Since most transactions succeed, values look\nsequential. Gaps will only be revealed by audits.\n\ndjango-sequences solves this problem with a ``get_next_value`` function\ndesigned to be used as follows:\n\n.. code:: python\n\n    from django.db import transaction\n    from sequences import get_next_value\n    from invoices.models import Invoice\n\n    with transaction.atomic():\n        Invoice.objects.create(number=get_next_value("invoice_numbers"))\n\nOr, if you\'d rather use an object-oriented API:\n\n.. code:: python\n\n    from django.db import transaction\n    from sequences import Sequence\n    from invoices.models import Invoice\n\n    invoice_numbers = Sequence("invoice_numbers")\n\n    with transaction.atomic():\n        Invoice.objects.create(number=next(invoice_numbers))\n\n``get_next_value`` relies on the database\'s transactional integrity to ensure\nthat each value is returned exactly once. As a consequence, **the guarantees\nof django-sequences apply only if you call** ``get_next_value`` **and save its\nreturn value to the database within the same transaction!**\n\nTable of contents\n=================\n\n* `Getting started`_\n* `Database support`_\n* `Multiple databases`_\n* `Isolation levels`_\n* `Contributing`_\n* `Releasing`_\n* `Changelog`_\n\nGetting started\n===============\n\ndjango-sequences is tested with Django 3.2 (LTS) and 4.0.\nIt is also tested with all database backends built-in to Django: MySQL/MariaDB,\nOracle, PostgreSQL and SQLite.\n\nIt is released under the BSD license, like Django itself.\n\nInstall django-sequences:\n\n.. code:: shell-session\n\n    $ pip install django-sequences\n\nAdd it to the list of applications in your project\'s settings:\n\n.. code:: python\n\n    INSTALLED_APPS = [\n        ...,\n        "sequences.apps.SequencesConfig",\n        ...\n    ]\n\nRun migrations:\n\n.. code:: shell-session\n\n    $ django-admin migrate\n\nAPI\n===\n\n``get_next_value``\n------------------\n\n.. code:: pycon\n\n    >>> from sequences import get_next_value\n\nThis function generates a gapless sequence of integer values:\n\n.. code:: pycon\n\n    >>> get_next_value()\n    1\n    >>> get_next_value()\n    2\n    >>> get_next_value()\n    3\n\nIt supports multiple independent sequences:\n\n.. code:: pycon\n\n    >>> get_next_value("cases")\n    1\n    >>> get_next_value("cases")\n    2\n    >>> get_next_value("invoices")\n    1\n    >>> get_next_value("invoices")\n    2\n\nThe first value defaults to 1. It can be customized:\n\n.. code:: pycon\n\n    >>> get_next_value("customers", initial_value=1000)  # pro growth hacking\n\nThe ``initial_value`` parameter only matters when ``get_next_value`` is called\nfor the first time for a given sequence — assuming the corresponding database\ntransaction gets committed; as discussed above, if the transaction is rolled\nback, the generated value isn\'t consumed. It\'s also possible to initialize a\nsequence in a data migration and not use ``initial_value`` in actual code.\n\nSequences can loop:\n\n.. code:: pycon\n\n    >>> get_next_value("seconds", initial_value=0, reset_value=60)\n\nWhen the sequence reaches ``reset_value``, it restarts at ``initial_value``.\nIn other words, it generates ``reset_value - 2``, ``reset_value - 1``,\n``initial_value``, ``initial_value + 1``, etc. In that case, each call to\n``get_next_value`` must provide ``initial_value`` when it isn\'t the default\nand ``reset_value``.\n\n**Database transactions that call** ``get_next_value`` **for a given sequence\nare serialized.** As a consequence, when you call ``get_next_value`` in a\ndatabase transaction, other callers trying to get a value from the same\nsequence block until the transaction completes, either with a commit or a\nrollback. You should keep such transactions short to minimize the impact on\nperformance.\n\nThis is why databases default to a faster behavior that may create gaps.\n\nPassing ``nowait=True`` makes ``get_next_value`` raise an exception instead of\nblocking in this scenario. This is rarely useful. Also it doesn\'t work for the\nfirst call. (This is a bug but it\'s harmless and hard to fix.)\n\nCalls to ``get_next_value`` for distinct sequences don\'t interact with one\nanother.\n\nFinally, passing ``using="..."`` allows selecting the database on which the\ncurrent sequence value is stored. When this parameter isn\'t provided, it\ndefaults to the default database for writing models of the ``sequences``\napplication. See `Multiple databases`_ for details.\n\nTo sum up, the complete signature of ``get_next_value`` is:\n\n.. code:: python\n\n    get_next_value(\n        sequence_name="default",\n        initial_value=1,\n        reset_value=None,\n        *,\n        nowait=False,\n        using=None,\n    )\n\n``get_last_value``\n------------------\n\n.. code:: pycon\n\n    >>> from sequences import get_last_value\n\nThis function returns the last value generated by a sequence:\n\n.. code:: pycon\n\n    >>> get_last_value()\n    None\n    >>> get_next_value()\n    1\n    >>> get_last_value()\n    1\n    >>> get_next_value()\n    2\n    >>> get_last_value()\n    2\n\nIf the sequence hasn\'t generated a value yet, ``get_last_value`` returns\n``None``.\n\nIt supports independent sequences like ``get_next_value``:\n\n.. code:: pycon\n\n    >>> get_next_value("cases")\n    1\n    >>> get_last_value("cases")\n    1\n    >>> get_next_value("invoices")\n    1\n    >>> get_last_value("invoices")\n    1\n\nIt accepts ``using="..."`` for selecting the database on which the current\nsequence value is stored, defaulting to the default database for reading\nmodels of the ``sequences`` application.\n\nThe complete signature of ``get_last_value`` is:\n\n.. code:: python\n\n    get_last_value(\n        sequence_name="default",\n        *,\n        using=None,\n    )\n\n``get_last_value`` **is a convenient and fast way to tell how many values a\nsequence generated but it makes no guarantees.** Concurrent calls to\n``get_next_value`` may produce unexpected results of ``get_last_value``.\n\n``Sequence``\n------------\n\n.. code:: pycon\n\n    >>> from sequences import Sequence\n\n(not to be confused with ``sequences.models.Sequence``, a private API)\n\nThis class stores parameters for a sequence and provides ``get_next_value``\nand ``get_last_value`` methods:\n\n.. code:: pycon\n\n    >>> claim_ids = Sequence("claims")\n    >>> claim_ids.get_next_value()\n    1\n    >>> claim_ids.get_next_value()\n    2\n    >>> claim_ids.get_last_value()\n    2\n\nThis reduces the risk of errors when the same sequence is used in multiple\nplaces.\n\nInstances of ``Sequence`` are also infinite iterators:\n\n.. code:: pycon\n\n    >>> next(claim_ids)\n    3\n    >>> next(claim_ids)\n    4\n\nThe complete API is:\n\n.. code:: python\n\n    Sequence(\n        sequence_name="default",\n        initial_value=1,\n        reset_value=None,\n        *,\n        using=None,\n    )\n\n    Sequence.get_next_value(\n        self,\n        *,\n        nowait=False,\n    )\n\n    Sequence.get_last_value(\n        self,\n    )\n\nAll parameters have the same meaning as in the ``get_next_value`` and\n``get_last_value`` functions.\n\nDatabase support\n================\n\ndjango-sequences is tested on PostgreSQL, MariaDB / MySQL, Oracle, and SQLite.\n\nMySQL only supports the ``nowait`` parameter from version 8.0.1.\nMariaDB only supports ``nowait`` from version 10.3.\n\nMultiple databases\n==================\n\nSince django-sequences relies on the database to guarantee transactional\nintegrity, the current value for a given sequence must be stored in the same\ndatabase as models containing generated values.\n\nIn a project that uses multiple databases, you must write a suitable database\nrouter to create tables for the ``sequences`` application on all databases\nstoring models containing sequential numbers.\n\nEach database has its own namespace: a sequence with the same name stored in\ntwo databases will have independent counters in each database.\n\nIsolation levels\n================\n\nSince django-sequences relies on the database\'s transactional integrity, using\na non-default transaction isolation level requires special care.\n\n* **read uncommitted:** django-sequences cannot work at this isolation level.\n\n  Indeed, concurrent transactions can create gaps, as in this scenario:\n\n  * Transaction A reads N and writes N + 1;\n  * Transaction B reads N + 1 (dirty read) and writes N + 2;\n  * Transaction A is rolled back;\n  * Transaction B is committed;\n  * N + 1 is a gap.\n\n  The read uncommitted isolation level doesn\'t provide sufficient guarantees.\n  It will never be supported.\n\n* **read committed:** django-sequences works best at this isolation level,\n  like Django itself.\n\n* **repeatable read:** django-sequences also works at this isolation level,\n  provided your code handles serialization failures and retries transactions.\n\n  This requirement isn\'t specific to django-sequences. It\'s generally needed\n  when running at the repeatable read isolation level.\n\n  Here\'s a scenario where only one of two concurrent transactions can\n  complete on PostgreSQL:\n\n  * Transaction A reads N and writes N + 1;\n  * Transaction B attemps to read; it must wait until transaction A completes;\n  * Transaction A is committed;\n  * Transaction B is aborted.\n\n  On PostgreSQL, serialization failures are reported as: ``OperationalError:\n  could not serialize access due to concurrent update``.\n\n  On MySQL, they result in: ``OperationalError: (1213, \'Deadlock found when\n  trying to get lock; try restarting transaction\')``.\n\n  Concurrent transactions initializing the same sequence are also vulnerable,\n  although that\'s hardly ever a problem in practice.\n\n  On PostgreSQL, this manifests as ``IntegrityError: duplicate key value\n  violates unique constraint "sequences_sequence_pkey"``.\n\n* **serializable:** the situation is identical to the repeatable read level.\n\n  SQLite always runs at the serializable isolation level. Serialization\n  failures result in: ``OperationalError: database is locked``.\n\nContributing\n============\n\nPrepare a development environment:\n\n* Install Poetry_.\n* Run ``poetry install``.\n* Run ``poetry shell`` to load the development environment.\n\nPrepare testing databases:\n\n* Install PostgreSQL, MariaDB, and Oracle.\n* Create a database called ``sequences``, owned by a user called ``sequences``\n  with password ``sequences``, with permissions to create a ``test_sequences``\n  test database. You may override these values with environment variables; see\n  ``tests/*_settings.py`` for details.\n\nMake changes:\n\n* Make changes to the code, tests, or docs.\n* Run ``make style`` and fix any flake8 violations.\n* Run ``make test`` to run the set suite on all databases.\n\nIterate until you\'re happy.\n\nCheck quality and submit your changes:\n\n* Install tox_.\n* Run ``tox`` to test on all Python and Django versions and all databases.\n* Submit a pull request.\n\n.. _Poetry: https://python-poetry.org/\n.. _tox: https://tox.readthedocs.io/\n\nReleasing\n=========\n\nIncrement version number X.Y in ``pyproject.toml``.\n\nCommit, tag, and push the change:\n\n.. code:: shell-session\n\n    $ git commit -m "Bump version number".\n    $ git tag X.Y\n    $ git push\n    $ git push --tags\n\nBuild and publish the new version:\n\n.. code:: shell-session\n\n    $ poetry build\n    $ poetry publish\n\nChangelog\n=========\n\n2.7\n---\n\n* Sequence values can go up to ``2 ** 63 - 1`` instead of ``2 ** 31 - 1``\n  previously. The exact limit depends on the database backend.\n\n  Migration ``0002_alter_sequence_last.py`` changes the field storing sequence\n  values from ``PositiveIntegerField`` to ``PositiveBigIntegerField``. Running\n  it requires an exclusive lock on the table, which prevents other operations,\n  including reads.\n\n  If you have many distinct sequences, e.g. if you create one sequence per user\n  and you have millions of users, review how the migration will affect your app\n  before running it or skip it with ``migrate --fake``.\n\n2.6\n---\n\n* Improve documentation.\n\n2.5\n---\n\n* Fix Japanese and Turkish translations.\n* Restore compatibility with Python 3.5.\n* Support relabeling the ``sequences`` app with a custom ``AppConfig``.\n\n2.4\n---\n\n* Add the ``get_last_value`` function.\n* Add the ``Sequence`` class.\n\n2.3\n---\n\n* Optimize performance on MySQL.\n* Test on MySQL, SQLite and Oracle.\n\n2.2\n---\n\n* Optimize performance on PostgreSQL ≥ 9.5.\n\n2.1\n---\n\n* Provide looping sequences with ``reset_value``.\n\n2.0\n---\n\n* Add support for multiple databases.\n* Add translations.\n* ``nowait`` becomes keyword-only argument.\n* Drop support for Python 2.\n\n1.0\n---\n\n* Initial stable release.\n',
-    'author': 'Aymeric Augustin',
-    'author_email': 'aymeric.augustin@m4x.org',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/aaugustin/django-sequences',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.6.2',
-}
+However, this behavior isn't guaranteed.
 
+If a transaction inserts a row and then is rolled back, the sequence counter
+isn't rolled back for performance reasons, creating a gap in primary keys.
+
+Such gaps may happen on all databases natively supported by Django:
+
+* `PostgreSQL <https://www.postgresql.org/docs/current/datatype-numeric.html#DATATYPE-SERIAL>`_
+* `MariaDB <https://mariadb.com/kb/en/auto_increment/#missing-values>`_ / MySQL
+* `Oracle <https://docs.oracle.com/en/database/oracle/oracle-database/21/sqlrf/CREATE-SEQUENCE.html>`_
+* `SQLite <https://sqlite.org/autoinc.html#the_autoincrement_keyword>`_
+
+They may also happen on most databases supported via third-party backends.
+
+This can cause compliance issues for some use cases such as accounting.
+
+This risk isn't well known. Since most transactions succeed, values look
+sequential. Gaps will only be revealed by audits.
+
+django-sequences solves this problem with a ``get_next_value`` function
+designed to be used as follows:
+
+.. code:: python
+
+    from django.db import transaction
+    from sequences import get_next_value
+    from invoices.models import Invoice
+
+    with transaction.atomic():
+        Invoice.objects.create(number=get_next_value("invoice_numbers"))
+
+Or, if you'd rather use an object-oriented API:
+
+.. code:: python
+
+    from django.db import transaction
+    from sequences import Sequence
+    from invoices.models import Invoice
+
+    invoice_numbers = Sequence("invoice_numbers")
+
+    with transaction.atomic():
+        Invoice.objects.create(number=next(invoice_numbers))
+
+``get_next_value`` relies on the database's transactional integrity to ensure
+that each value is returned exactly once. As a consequence, **the guarantees
+of django-sequences apply only if you call** ``get_next_value`` **and save its
+return value to the database within the same transaction!**
+
+Table of contents
+=================
+
+* `Getting started`_
+* `API`_
+* `Database support`_
+* `Multiple databases`_
+* `Isolation levels`_
+* `Contributing`_
+* `Releasing`_
+* `Changelog`_
+
+Getting started
+===============
+
+django-sequences is tested with Django 3.2 (LTS), 4.0, 4.1, and 4.2.
+It is also tested with all database backends built-in to Django: MySQL/MariaDB,
+Oracle, PostgreSQL and SQLite.
+
+It is released under the BSD license, like Django itself.
+
+Install django-sequences:
+
+.. code:: shell-session
+
+    $ pip install django-sequences
+
+Add it to the list of applications in your project's settings:
+
+.. code:: python
+
+    INSTALLED_APPS = [
+        ...,
+        "sequences.apps.SequencesConfig",
+        ...
+    ]
+
+Run migrations:
+
+.. code:: shell-session
+
+    $ django-admin migrate
+
+API
+===
+
+``get_next_value``
+------------------
+
+.. code:: pycon
+
+    >>> from sequences import get_next_value
+
+This function generates a gapless sequence of integer values:
+
+.. code:: pycon
+
+    >>> get_next_value()
+    1
+    >>> get_next_value()
+    2
+    >>> get_next_value()
+    3
+
+It supports multiple independent sequences:
+
+.. code:: pycon
+
+    >>> get_next_value("cases")
+    1
+    >>> get_next_value("cases")
+    2
+    >>> get_next_value("invoices")
+    1
+    >>> get_next_value("invoices")
+    2
+
+The first value defaults to 1. It can be customized:
+
+.. code:: pycon
+
+    >>> get_next_value("customers", initial_value=1000)  # pro growth hacking
+
+The ``initial_value`` parameter only matters when ``get_next_value`` is called
+for the first time for a given sequence — assuming the corresponding database
+transaction gets committed; as discussed above, if the transaction is rolled
+back, the generated value isn't consumed. It's also possible to initialize a
+sequence in a data migration and not use ``initial_value`` in actual code.
+
+Sequences can loop:
+
+.. code:: pycon
+
+    >>> get_next_value("seconds", initial_value=0, reset_value=60)
+
+When the sequence reaches ``reset_value``, it restarts at ``initial_value``.
+In other words, it generates ``reset_value - 2``, ``reset_value - 1``,
+``initial_value``, ``initial_value + 1``, etc. In that case, each call to
+``get_next_value`` must provide ``initial_value`` when it isn't the default
+and ``reset_value``.
+
+**Database transactions that call** ``get_next_value`` **for a given sequence
+are serialized.** As a consequence, when you call ``get_next_value`` in a
+database transaction, other callers trying to get a value from the same
+sequence block until the transaction completes, either with a commit or a
+rollback. You should keep such transactions short to minimize the impact on
+performance.
+
+This is why databases default to a faster behavior that may create gaps.
+
+Passing ``nowait=True`` makes ``get_next_value`` raise an exception instead of
+blocking in this scenario. This is rarely useful. Also it doesn't work for the
+first call. (This is a bug but it's harmless and hard to fix.)
+
+Calls to ``get_next_value`` for distinct sequences don't interact with one
+another.
+
+Finally, passing ``using="..."`` allows selecting the database on which the
+current sequence value is stored. When this parameter isn't provided, it
+defaults to the default database for writing models of the ``sequences``
+application. See `Multiple databases`_ for details.
+
+To sum up, the complete signature of ``get_next_value`` is:
+
+.. code:: python
+
+    get_next_value(
+        sequence_name="default",
+        initial_value=1,
+        reset_value=None,
+        *,
+        nowait=False,
+        using=None,
+    )
+
+``get_last_value``
+------------------
+
+.. code:: pycon
+
+    >>> from sequences import get_last_value
+
+This function returns the last value generated by a sequence:
+
+.. code:: pycon
+
+    >>> get_last_value()
+    None
+    >>> get_next_value()
+    1
+    >>> get_last_value()
+    1
+    >>> get_next_value()
+    2
+    >>> get_last_value()
+    2
+
+If the sequence hasn't generated a value yet, ``get_last_value`` returns
+``None``.
+
+It supports independent sequences like ``get_next_value``:
+
+.. code:: pycon
+
+    >>> get_next_value("cases")
+    1
+    >>> get_last_value("cases")
+    1
+    >>> get_next_value("invoices")
+    1
+    >>> get_last_value("invoices")
+    1
+
+It accepts ``using="..."`` for selecting the database on which the current
+sequence value is stored, defaulting to the default database for reading
+models of the ``sequences`` application.
+
+The complete signature of ``get_last_value`` is:
+
+.. code:: python
+
+    get_last_value(
+        sequence_name="default",
+        *,
+        using=None,
+    )
+
+``get_last_value`` **is a convenient and fast way to tell how many values a
+sequence generated but it makes no guarantees.** Concurrent calls to
+``get_next_value`` may produce unexpected results of ``get_last_value``.
+
+``Sequence``
+------------
+
+.. code:: pycon
+
+    >>> from sequences import Sequence
+
+(not to be confused with ``sequences.models.Sequence``, a private API)
+
+This class stores parameters for a sequence and provides ``get_next_value``
+and ``get_last_value`` methods:
+
+.. code:: pycon
+
+    >>> claim_ids = Sequence("claims")
+    >>> claim_ids.get_next_value()
+    1
+    >>> claim_ids.get_next_value()
+    2
+    >>> claim_ids.get_last_value()
+    2
+
+This reduces the risk of errors when the same sequence is used in multiple
+places.
+
+Instances of ``Sequence`` are also infinite iterators:
+
+.. code:: pycon
+
+    >>> next(claim_ids)
+    3
+    >>> next(claim_ids)
+    4
+
+The complete API is:
+
+.. code:: python
+
+    Sequence(
+        sequence_name="default",
+        initial_value=1,
+        reset_value=None,
+        *,
+        using=None,
+    )
+
+    Sequence.get_next_value(
+        self,
+        *,
+        nowait=False,
+    )
+
+    Sequence.get_last_value(
+        self,
+    )
+
+All parameters have the same meaning as in the ``get_next_value`` and
+``get_last_value`` functions.
+
+Examples
+========
+
+Per-date sequences
+------------------
+
+If you want independent sequences per day, month, or year, use the appropriate
+date fragment in the sequence name. For example:
+
+.. code:: python
+
+    from django.utils import timezone
+    from sequences import get_next_value
+
+    # Per-day sequence
+    get_next_value(f"books-{timezone.now().date().isoformat()}")
+    # Per-year sequence
+    get_next_value(f"prototocol-{timezone.now().year}")
+
+The above calls will result in separate sequences like ``books-2023-03-15``
+or ``protocol-2022``, respectively.
+
+Database support
+================
+
+django-sequences is tested on PostgreSQL, MariaDB / MySQL, Oracle, and SQLite.
+
+MySQL only supports the ``nowait`` parameter from version 8.0.1.
+MariaDB only supports ``nowait`` from version 10.3.
+
+Multiple databases
+==================
+
+Since django-sequences relies on the database to guarantee transactional
+integrity, the current value for a given sequence must be stored in the same
+database as models containing generated values.
+
+In a project that uses multiple databases, you must write a suitable database
+router to create tables for the ``sequences`` application on all databases
+storing models containing sequential numbers.
+
+Each database has its own namespace: a sequence with the same name stored in
+two databases will have independent counters in each database.
+
+Isolation levels
+================
+
+Since django-sequences relies on the database's transactional integrity, using
+a non-default transaction isolation level requires special care.
+
+* **read uncommitted:** django-sequences cannot work at this isolation level.
+
+  Indeed, concurrent transactions can create gaps, as in this scenario:
+
+  * Transaction A reads N and writes N + 1;
+  * Transaction B reads N + 1 (dirty read) and writes N + 2;
+  * Transaction A is rolled back;
+  * Transaction B is committed;
+  * N + 1 is a gap.
+
+  The read uncommitted isolation level doesn't provide sufficient guarantees.
+  It will never be supported.
+
+* **read committed:** django-sequences works best at this isolation level,
+  like Django itself.
+
+* **repeatable read:** django-sequences also works at this isolation level,
+  provided your code handles serialization failures and retries transactions.
+
+  This requirement isn't specific to django-sequences. It's generally needed
+  when running at the repeatable read isolation level.
+
+  Here's a scenario where only one of two concurrent transactions can
+  complete on PostgreSQL:
+
+  * Transaction A reads N and writes N + 1;
+  * Transaction B attemps to read; it must wait until transaction A completes;
+  * Transaction A is committed;
+  * Transaction B is aborted.
+
+  On PostgreSQL, serialization failures are reported as: ``OperationalError:
+  could not serialize access due to concurrent update``.
+
+  On MySQL, they result in: ``OperationalError: (1213, 'Deadlock found when
+  trying to get lock; try restarting transaction')``.
+
+  Concurrent transactions initializing the same sequence are also vulnerable,
+  although that's hardly ever a problem in practice.
+
+  On PostgreSQL, this manifests as ``IntegrityError: duplicate key value
+  violates unique constraint "sequences_sequence_pkey"``.
+
+* **serializable:** the situation is identical to the repeatable read level.
+
+  SQLite always runs at the serializable isolation level. Serialization
+  failures result in: ``OperationalError: database is locked``.
+
+Contributing
+============
+
+Prepare a development environment:
+
+* Install Poetry_.
+* Run ``poetry install``.
+* Run ``poetry shell`` to load the development environment.
+
+Prepare testing databases:
+
+* Install PostgreSQL, MariaDB, and Oracle.
+* Create a database called ``sequences``, owned by a user called ``sequences``
+  with password ``sequences``, with permissions to create a ``test_sequences``
+  test database. You may override these values with environment variables; see
+  ``tests/*_settings.py`` for details.
+
+Make changes:
+
+* Make changes to the code, tests, or docs.
+* Run ``make style`` and fix any flake8 violations.
+* Run ``make test`` to run the set suite on all databases.
+
+Iterate until you're happy.
+
+Check quality and submit your changes:
+
+* Install tox_.
+* Run ``tox`` to test on all Python and Django versions and all databases.
+* Submit a pull request.
+
+.. _Poetry: https://python-poetry.org/
+.. _tox: https://tox.readthedocs.io/
+
+Releasing
+=========
+
+Increment version number X.Y in ``pyproject.toml``.
+
+Commit, tag, and push the change:
+
+.. code:: shell-session
+
+    $ git commit -m "Bump version number".
+    $ git tag X.Y
+    $ git push
+    $ git push --tags
+
+Build and publish the new version:
+
+.. code:: shell-session
+
+    $ poetry build
+    $ poetry publish
+
+Changelog
+=========
+
+2.8
+---
+
+* No significant changes.
+
+2.7
+---
+
+* Sequence values can go up to ``2 ** 63 - 1`` instead of ``2 ** 31 - 1``
+  previously. The exact limit depends on the database backend.
+
+  Migration ``0002_alter_sequence_last.py`` changes the field storing sequence
+  values from ``PositiveIntegerField`` to ``PositiveBigIntegerField``. Running
+  it requires an exclusive lock on the table, which prevents other operations,
+  including reads.
+
+  If you have many distinct sequences, e.g. if you create one sequence per user
+  and you have millions of users, review how the migration will affect your app
+  before running it or skip it with ``migrate --fake``.
+
+2.6
+---
+
+* Improve documentation.
+
+2.5
+---
+
+* Fix Japanese and Turkish translations.
+* Restore compatibility with Python 3.5.
+* Support relabeling the ``sequences`` app with a custom ``AppConfig``.
+
+2.4
+---
+
+* Add the ``get_last_value`` function.
+* Add the ``Sequence`` class.
+
+2.3
+---
+
+* Optimize performance on MySQL.
+* Test on MySQL, SQLite and Oracle.
+
+2.2
+---
+
+* Optimize performance on PostgreSQL ≥ 9.5.
+
+2.1
+---
+
+* Provide looping sequences with ``reset_value``.
+
+2.0
+---
+
+* Add support for multiple databases.
+* Add translations.
+* ``nowait`` becomes keyword-only argument.
+* Drop support for Python 2.
+
+1.0
+---
+
+* Initial stable release.
 
-setup(**setup_kwargs)
```

