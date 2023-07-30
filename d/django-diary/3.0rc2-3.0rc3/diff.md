# Comparing `tmp/django-diary-3.0rc2.tar.gz` & `tmp/django-diary-3.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-diary-3.0rc2.tar", last modified: Tue Jun 30 15:23:03 2020, max compression
+gzip compressed data, was "dist/django-diary-3.0rc3.tar", last modified: Tue Jun 30 15:41:23 2020, max compression
```

## Comparing `django-diary-3.0rc2.tar` & `django-diary-3.0rc3.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2020-06-30 15:23:03.657409 django-diary-3.0rc2/
--rw-r--r--   0 bob       (1000) bob       (1000)     3339 2020-06-29 12:28:02.000000 django-diary-3.0rc2/CHANGES.txt
--rw-r--r--   0 bob       (1000) bob       (1000)     1105 2015-09-09 10:52:23.000000 django-diary-3.0rc2/LICENSE.txt
--rw-r--r--   0 bob       (1000) bob       (1000)      105 2015-09-26 10:31:45.000000 django-diary-3.0rc2/MANIFEST.in
--rw-r--r--   0 bob       (1000) bob       (1000)    27232 2020-06-30 15:23:03.657409 django-diary-3.0rc2/PKG-INFO
--rw-r--r--   0 bob       (1000) bob       (1000)    23186 2020-06-29 13:07:15.000000 django-diary-3.0rc2/README.rst
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2020-06-30 15:23:03.633409 django-diary-3.0rc2/diary/
--rw-r--r--   0 bob       (1000) bob       (1000)       23 2020-06-30 15:21:39.000000 django-diary-3.0rc2/diary/__init__.py
--rw-r--r--   0 bob       (1000) bob       (1000)     5383 2015-10-21 10:00:19.000000 django-diary-3.0rc2/diary/admin.py
--rw-r--r--   0 bob       (1000) bob       (1000)      691 2020-06-29 12:28:02.000000 django-diary-3.0rc2/diary/backends.py
--rw-r--r--   0 bob       (1000) bob       (1000)     2252 2020-06-29 12:28:02.000000 django-diary-3.0rc2/diary/forms.py
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2020-06-30 15:23:03.633409 django-diary-3.0rc2/diary/management/
--rw-r--r--   0 bob       (1000) bob       (1000)        0 2015-10-30 14:06:59.000000 django-diary-3.0rc2/diary/management/__init__.py
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2020-06-30 15:23:03.633409 django-diary-3.0rc2/diary/management/commands/
--rw-r--r--   0 bob       (1000) bob       (1000)        0 2015-10-30 14:06:59.000000 django-diary-3.0rc2/diary/management/commands/__init__.py
--rw-r--r--   0 bob       (1000) bob       (1000)     2866 2015-11-19 11:27:55.000000 django-diary-3.0rc2/diary/management/commands/email_reminder.py
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2020-06-30 15:23:03.633409 django-diary-3.0rc2/diary/migrations/
--rw-r--r--   0 bob       (1000) bob       (1000)     3547 2020-06-29 12:28:02.000000 django-diary-3.0rc2/diary/migrations/0001_initial.py
--rw-r--r--   0 bob       (1000) bob       (1000)      898 2020-06-29 12:28:02.000000 django-diary-3.0rc2/diary/migrations/0002_auto_20151010_1324.py
--rw-r--r--   0 bob       (1000) bob       (1000)      640 2015-10-11 12:07:14.000000 django-diary-3.0rc2/diary/migrations/0003_auto_20151010_1331.py
--rw-r--r--   0 bob       (1000) bob       (1000)      533 2015-10-19 13:04:03.000000 django-diary-3.0rc2/diary/migrations/0004_customer_title.py
--rw-r--r--   0 bob       (1000) bob       (1000)     1332 2015-10-19 13:04:04.000000 django-diary-3.0rc2/diary/migrations/0005_auto_20151017_1119.py
--rw-r--r--   0 bob       (1000) bob       (1000)      557 2015-10-19 13:04:04.000000 django-diary-3.0rc2/diary/migrations/0006_auto_20151017_1347.py
--rw-r--r--   0 bob       (1000) bob       (1000)     1033 2015-10-19 13:04:04.000000 django-diary-3.0rc2/diary/migrations/0007_auto_20151017_1348.py
--rw-r--r--   0 bob       (1000) bob       (1000)        0 2015-09-09 10:52:23.000000 django-diary-3.0rc2/diary/migrations/__init__.py
--rw-r--r--   0 bob       (1000) bob       (1000)    13465 2020-06-29 12:28:02.000000 django-diary-3.0rc2/diary/models.py
--rw-r--r--   0 bob       (1000) bob       (1000)     1954 2015-11-05 11:24:08.000000 django-diary-3.0rc2/diary/settings.py
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2020-06-30 15:23:03.633409 django-diary-3.0rc2/diary/static/
--rw-r--r--   0 bob       (1000) bob       (1000)      702 2015-09-23 12:09:00.000000 django-diary-3.0rc2/diary/static/ajax_csrf.js
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2020-06-30 15:23:03.633409 django-diary-3.0rc2/diary/static/diary/
--rw-r--r--   0 bob       (1000) bob       (1000)     2465 2015-10-25 11:07:28.000000 django-diary-3.0rc2/diary/static/diary/base.css
--rw-r--r--   0 bob       (1000) bob       (1000)     3296 2015-10-19 13:04:04.000000 django-diary-3.0rc2/diary/static/diary/entry_ajax_dnd.js
--rw-r--r--   0 bob       (1000) bob       (1000)     1880 2015-10-11 12:07:14.000000 django-diary-3.0rc2/diary/static/diary/entry_ajax_modal.js
--rw-r--r--   0 bob       (1000) bob       (1000)     3897 2015-09-19 16:38:13.000000 django-diary-3.0rc2/diary/static/diary/multi_col.css
--rw-r--r--   0 bob       (1000) bob       (1000)     3285 2015-09-09 10:52:23.000000 django-diary-3.0rc2/diary/static/js.cookie.js
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2020-06-30 15:23:03.629408 django-diary-3.0rc2/diary/templates/
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2020-06-30 15:23:03.637409 django-diary-3.0rc2/diary/templates/diary/
--rw-r--r--   0 bob       (1000) bob       (1000)      714 2020-06-23 11:55:46.000000 django-diary-3.0rc2/diary/templates/diary/base.html
--rw-r--r--   0 bob       (1000) bob       (1000)      504 2015-09-23 12:09:00.000000 django-diary-3.0rc2/diary/templates/diary/customer_add.html
--rw-r--r--   0 bob       (1000) bob       (1000)      325 2015-09-23 12:09:00.000000 django-diary-3.0rc2/diary/templates/diary/customer_change.html
--rw-r--r--   0 bob       (1000) bob       (1000)     2920 2015-10-19 13:04:04.000000 django-diary-3.0rc2/diary/templates/diary/day.html
--rw-r--r--   0 bob       (1000) bob       (1000)      246 2020-06-23 11:55:46.000000 django-diary-3.0rc2/diary/templates/diary/day_base.html
--rw-r--r--   0 bob       (1000) bob       (1000)     2047 2015-09-09 10:52:23.000000 django-diary-3.0rc2/diary/templates/diary/day_list.html
--rw-r--r--   0 bob       (1000) bob       (1000)      394 2015-11-05 11:33:50.000000 django-diary-3.0rc2/diary/templates/diary/email_reminder.txt
--rw-r--r--   0 bob       (1000) bob       (1000)      459 2015-10-11 12:07:14.000000 django-diary-3.0rc2/diary/templates/diary/entry.html
--rw-r--r--   0 bob       (1000) bob       (1000)     2810 2015-10-11 12:07:14.000000 django-diary-3.0rc2/diary/templates/diary/form_base.html
--rw-r--r--   0 bob       (1000) bob       (1000)     2822 2015-10-25 11:07:28.000000 django-diary-3.0rc2/diary/templates/diary/history.html
--rw-r--r--   0 bob       (1000) bob       (1000)     6425 2020-06-23 11:55:46.000000 django-diary-3.0rc2/diary/templates/diary/main_base.html
--rw-r--r--   0 bob       (1000) bob       (1000)     1336 2020-06-30 15:19:38.000000 django-diary-3.0rc2/diary/templates/diary/modal_base.html
--rw-r--r--   0 bob       (1000) bob       (1000)     5091 2020-06-11 11:12:17.000000 django-diary-3.0rc2/diary/templates/diary/modal_entry.html
--rw-r--r--   0 bob       (1000) bob       (1000)     2730 2020-06-23 11:55:46.000000 django-diary-3.0rc2/diary/templates/diary/month.html
--rw-r--r--   0 bob       (1000) bob       (1000)     4659 2015-10-19 13:04:04.000000 django-diary-3.0rc2/diary/templates/diary/multi_day.html
--rw-r--r--   0 bob       (1000) bob       (1000)      590 2015-10-26 11:18:31.000000 django-diary-3.0rc2/diary/templates/diary/reminders.html
--rw-r--r--   0 bob       (1000) bob       (1000)     1247 2015-09-19 16:38:13.000000 django-diary-3.0rc2/diary/templates/diary/year.html
--rw-r--r--   0 bob       (1000) bob       (1000)    26480 2020-06-29 12:28:02.000000 django-diary-3.0rc2/diary/tests.py
--rw-r--r--   0 bob       (1000) bob       (1000)     3579 2020-06-29 12:28:02.000000 django-diary-3.0rc2/diary/urls.py
--rw-r--r--   0 bob       (1000) bob       (1000)    25016 2020-06-29 12:30:32.000000 django-diary-3.0rc2/diary/views.py
--rw-r--r--   0 bob       (1000) bob       (1000)     1859 2020-06-29 12:28:02.000000 django-diary-3.0rc2/diary/widgets.py
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2020-06-30 15:23:03.657409 django-diary-3.0rc2/django_diary.egg-info/
--rw-r--r--   0 bob       (1000) bob       (1000)    27232 2020-06-30 15:23:03.000000 django-diary-3.0rc2/django_diary.egg-info/PKG-INFO
--rw-r--r--   0 bob       (1000) bob       (1000)     2424 2020-06-30 15:23:03.000000 django-diary-3.0rc2/django_diary.egg-info/SOURCES.txt
--rw-r--r--   0 bob       (1000) bob       (1000)        1 2020-06-30 15:23:03.000000 django-diary-3.0rc2/django_diary.egg-info/dependency_links.txt
--rw-r--r--   0 bob       (1000) bob       (1000)        1 2015-09-26 10:24:06.000000 django-diary-3.0rc2/django_diary.egg-info/not-zip-safe
--rw-r--r--   0 bob       (1000) bob       (1000)       69 2020-06-30 15:23:03.000000 django-diary-3.0rc2/django_diary.egg-info/requires.txt
--rw-r--r--   0 bob       (1000) bob       (1000)        6 2020-06-30 15:23:03.000000 django-diary-3.0rc2/django_diary.egg-info/top_level.txt
--rwxr-xr-x   0 bob       (1000) bob       (1000)    11434 2015-09-25 15:18:27.000000 django-diary-3.0rc2/ez_setup.py
--rw-r--r--   0 bob       (1000) bob       (1000)       38 2020-06-30 15:23:03.657409 django-diary-3.0rc2/setup.cfg
--rwxr-xr-x   0 bob       (1000) bob       (1000)     3204 2020-06-29 13:33:43.000000 django-diary-3.0rc2/setup.py
+drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2020-06-30 15:41:23.248698 django-diary-3.0rc3/
+-rw-r--r--   0 bob       (1000) bob       (1000)     3339 2020-06-29 12:28:02.000000 django-diary-3.0rc3/CHANGES.txt
+-rw-r--r--   0 bob       (1000) bob       (1000)     1105 2015-09-09 10:52:23.000000 django-diary-3.0rc3/LICENSE.txt
+-rw-r--r--   0 bob       (1000) bob       (1000)      105 2015-09-26 10:31:45.000000 django-diary-3.0rc3/MANIFEST.in
+-rw-r--r--   0 bob       (1000) bob       (1000)    27232 2020-06-30 15:41:23.248698 django-diary-3.0rc3/PKG-INFO
+-rw-r--r--   0 bob       (1000) bob       (1000)    23186 2020-06-29 13:07:15.000000 django-diary-3.0rc3/README.rst
+drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2020-06-30 15:41:23.240698 django-diary-3.0rc3/diary/
+-rw-r--r--   0 bob       (1000) bob       (1000)       23 2020-06-30 15:40:48.000000 django-diary-3.0rc3/diary/__init__.py
+-rw-r--r--   0 bob       (1000) bob       (1000)     5383 2015-10-21 10:00:19.000000 django-diary-3.0rc3/diary/admin.py
+-rw-r--r--   0 bob       (1000) bob       (1000)      691 2020-06-29 12:28:02.000000 django-diary-3.0rc3/diary/backends.py
+-rw-r--r--   0 bob       (1000) bob       (1000)     2252 2020-06-29 12:28:02.000000 django-diary-3.0rc3/diary/forms.py
+drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2020-06-30 15:41:23.240698 django-diary-3.0rc3/diary/management/
+-rw-r--r--   0 bob       (1000) bob       (1000)        0 2015-10-30 14:06:59.000000 django-diary-3.0rc3/diary/management/__init__.py
+drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2020-06-30 15:41:23.244698 django-diary-3.0rc3/diary/management/commands/
+-rw-r--r--   0 bob       (1000) bob       (1000)        0 2015-10-30 14:06:59.000000 django-diary-3.0rc3/diary/management/commands/__init__.py
+-rw-r--r--   0 bob       (1000) bob       (1000)     2866 2015-11-19 11:27:55.000000 django-diary-3.0rc3/diary/management/commands/email_reminder.py
+drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2020-06-30 15:41:23.244698 django-diary-3.0rc3/diary/migrations/
+-rw-r--r--   0 bob       (1000) bob       (1000)     3547 2020-06-29 12:28:02.000000 django-diary-3.0rc3/diary/migrations/0001_initial.py
+-rw-r--r--   0 bob       (1000) bob       (1000)      898 2020-06-29 12:28:02.000000 django-diary-3.0rc3/diary/migrations/0002_auto_20151010_1324.py
+-rw-r--r--   0 bob       (1000) bob       (1000)      640 2015-10-11 12:07:14.000000 django-diary-3.0rc3/diary/migrations/0003_auto_20151010_1331.py
+-rw-r--r--   0 bob       (1000) bob       (1000)      533 2015-10-19 13:04:03.000000 django-diary-3.0rc3/diary/migrations/0004_customer_title.py
+-rw-r--r--   0 bob       (1000) bob       (1000)     1332 2015-10-19 13:04:04.000000 django-diary-3.0rc3/diary/migrations/0005_auto_20151017_1119.py
+-rw-r--r--   0 bob       (1000) bob       (1000)      557 2015-10-19 13:04:04.000000 django-diary-3.0rc3/diary/migrations/0006_auto_20151017_1347.py
+-rw-r--r--   0 bob       (1000) bob       (1000)     1033 2015-10-19 13:04:04.000000 django-diary-3.0rc3/diary/migrations/0007_auto_20151017_1348.py
+-rw-r--r--   0 bob       (1000) bob       (1000)        0 2015-09-09 10:52:23.000000 django-diary-3.0rc3/diary/migrations/__init__.py
+-rw-r--r--   0 bob       (1000) bob       (1000)    13465 2020-06-29 12:28:02.000000 django-diary-3.0rc3/diary/models.py
+-rw-r--r--   0 bob       (1000) bob       (1000)     1954 2015-11-05 11:24:08.000000 django-diary-3.0rc3/diary/settings.py
+drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2020-06-30 15:41:23.244698 django-diary-3.0rc3/diary/static/
+-rw-r--r--   0 bob       (1000) bob       (1000)      702 2015-09-23 12:09:00.000000 django-diary-3.0rc3/diary/static/ajax_csrf.js
+drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2020-06-30 15:41:23.244698 django-diary-3.0rc3/diary/static/diary/
+-rw-r--r--   0 bob       (1000) bob       (1000)     2465 2015-10-25 11:07:28.000000 django-diary-3.0rc3/diary/static/diary/base.css
+-rw-r--r--   0 bob       (1000) bob       (1000)     3296 2015-10-19 13:04:04.000000 django-diary-3.0rc3/diary/static/diary/entry_ajax_dnd.js
+-rw-r--r--   0 bob       (1000) bob       (1000)     1880 2015-10-11 12:07:14.000000 django-diary-3.0rc3/diary/static/diary/entry_ajax_modal.js
+-rw-r--r--   0 bob       (1000) bob       (1000)     3897 2015-09-19 16:38:13.000000 django-diary-3.0rc3/diary/static/diary/multi_col.css
+-rw-r--r--   0 bob       (1000) bob       (1000)     3285 2015-09-09 10:52:23.000000 django-diary-3.0rc3/diary/static/js.cookie.js
+drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2020-06-30 15:41:23.240698 django-diary-3.0rc3/diary/templates/
+drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2020-06-30 15:41:23.248698 django-diary-3.0rc3/diary/templates/diary/
+-rw-r--r--   0 bob       (1000) bob       (1000)      714 2020-06-23 11:55:46.000000 django-diary-3.0rc3/diary/templates/diary/base.html
+-rw-r--r--   0 bob       (1000) bob       (1000)      504 2015-09-23 12:09:00.000000 django-diary-3.0rc3/diary/templates/diary/customer_add.html
+-rw-r--r--   0 bob       (1000) bob       (1000)      325 2015-09-23 12:09:00.000000 django-diary-3.0rc3/diary/templates/diary/customer_change.html
+-rw-r--r--   0 bob       (1000) bob       (1000)     2920 2015-10-19 13:04:04.000000 django-diary-3.0rc3/diary/templates/diary/day.html
+-rw-r--r--   0 bob       (1000) bob       (1000)      246 2020-06-23 11:55:46.000000 django-diary-3.0rc3/diary/templates/diary/day_base.html
+-rw-r--r--   0 bob       (1000) bob       (1000)     2047 2015-09-09 10:52:23.000000 django-diary-3.0rc3/diary/templates/diary/day_list.html
+-rw-r--r--   0 bob       (1000) bob       (1000)      394 2015-11-05 11:33:50.000000 django-diary-3.0rc3/diary/templates/diary/email_reminder.txt
+-rw-r--r--   0 bob       (1000) bob       (1000)      459 2015-10-11 12:07:14.000000 django-diary-3.0rc3/diary/templates/diary/entry.html
+-rw-r--r--   0 bob       (1000) bob       (1000)     2810 2015-10-11 12:07:14.000000 django-diary-3.0rc3/diary/templates/diary/form_base.html
+-rw-r--r--   0 bob       (1000) bob       (1000)     2822 2015-10-25 11:07:28.000000 django-diary-3.0rc3/diary/templates/diary/history.html
+-rw-r--r--   0 bob       (1000) bob       (1000)     6425 2020-06-23 11:55:46.000000 django-diary-3.0rc3/diary/templates/diary/main_base.html
+-rw-r--r--   0 bob       (1000) bob       (1000)     1336 2020-06-30 15:19:38.000000 django-diary-3.0rc3/diary/templates/diary/modal_base.html
+-rw-r--r--   0 bob       (1000) bob       (1000)     5091 2020-06-11 11:12:17.000000 django-diary-3.0rc3/diary/templates/diary/modal_entry.html
+-rw-r--r--   0 bob       (1000) bob       (1000)     2730 2020-06-23 11:55:46.000000 django-diary-3.0rc3/diary/templates/diary/month.html
+-rw-r--r--   0 bob       (1000) bob       (1000)     4647 2020-06-30 15:39:34.000000 django-diary-3.0rc3/diary/templates/diary/multi_day.html
+-rw-r--r--   0 bob       (1000) bob       (1000)      590 2015-10-26 11:18:31.000000 django-diary-3.0rc3/diary/templates/diary/reminders.html
+-rw-r--r--   0 bob       (1000) bob       (1000)     1247 2015-09-19 16:38:13.000000 django-diary-3.0rc3/diary/templates/diary/year.html
+-rw-r--r--   0 bob       (1000) bob       (1000)    26480 2020-06-29 12:28:02.000000 django-diary-3.0rc3/diary/tests.py
+-rw-r--r--   0 bob       (1000) bob       (1000)     3579 2020-06-29 12:28:02.000000 django-diary-3.0rc3/diary/urls.py
+-rw-r--r--   0 bob       (1000) bob       (1000)    25016 2020-06-29 12:30:32.000000 django-diary-3.0rc3/diary/views.py
+-rw-r--r--   0 bob       (1000) bob       (1000)     1859 2020-06-29 12:28:02.000000 django-diary-3.0rc3/diary/widgets.py
+drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2020-06-30 15:41:23.248698 django-diary-3.0rc3/django_diary.egg-info/
+-rw-r--r--   0 bob       (1000) bob       (1000)    27232 2020-06-30 15:41:23.000000 django-diary-3.0rc3/django_diary.egg-info/PKG-INFO
+-rw-r--r--   0 bob       (1000) bob       (1000)     2424 2020-06-30 15:41:23.000000 django-diary-3.0rc3/django_diary.egg-info/SOURCES.txt
+-rw-r--r--   0 bob       (1000) bob       (1000)        1 2020-06-30 15:41:23.000000 django-diary-3.0rc3/django_diary.egg-info/dependency_links.txt
+-rw-r--r--   0 bob       (1000) bob       (1000)        1 2015-09-26 10:24:06.000000 django-diary-3.0rc3/django_diary.egg-info/not-zip-safe
+-rw-r--r--   0 bob       (1000) bob       (1000)       69 2020-06-30 15:41:23.000000 django-diary-3.0rc3/django_diary.egg-info/requires.txt
+-rw-r--r--   0 bob       (1000) bob       (1000)        6 2020-06-30 15:41:23.000000 django-diary-3.0rc3/django_diary.egg-info/top_level.txt
+-rwxr-xr-x   0 bob       (1000) bob       (1000)    11434 2015-09-25 15:18:27.000000 django-diary-3.0rc3/ez_setup.py
+-rw-r--r--   0 bob       (1000) bob       (1000)       38 2020-06-30 15:41:23.248698 django-diary-3.0rc3/setup.cfg
+-rwxr-xr-x   0 bob       (1000) bob       (1000)     3204 2020-06-29 13:33:43.000000 django-diary-3.0rc3/setup.py
```

### Comparing `django-diary-3.0rc2/CHANGES.txt` & `django-diary-3.0rc3/CHANGES.txt`

 * *Files identical despite different names*

### Comparing `django-diary-3.0rc2/LICENSE.txt` & `django-diary-3.0rc3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-diary-3.0rc2/PKG-INFO` & `django-diary-3.0rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-diary
-Version: 3.0rc2
+Version: 3.0rc3
 Summary: A pluggable diary app for use in the Django framework.
 Home-page: http://pypi.python.org/pypi/diary/
 Author: Bob Bowles
 Author-email: bobjohnbowles@gmail.com
 License: MIT License
 Description: ============
         Django Diary
```

### Comparing `django-diary-3.0rc2/README.rst` & `django-diary-3.0rc3/README.rst`

 * *Files identical despite different names*

### Comparing `django-diary-3.0rc2/diary/admin.py` & `django-diary-3.0rc3/diary/admin.py`

 * *Files identical despite different names*

### Comparing `django-diary-3.0rc2/diary/backends.py` & `django-diary-3.0rc3/diary/backends.py`

 * *Files identical despite different names*

### Comparing `django-diary-3.0rc2/diary/forms.py` & `django-diary-3.0rc3/diary/forms.py`

 * *Files identical despite different names*

### Comparing `django-diary-3.0rc2/diary/management/commands/email_reminder.py` & `django-diary-3.0rc3/diary/management/commands/email_reminder.py`

 * *Files identical despite different names*

### Comparing `django-diary-3.0rc2/diary/migrations/0001_initial.py` & `django-diary-3.0rc3/diary/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-diary-3.0rc2/diary/migrations/0002_auto_20151010_1324.py` & `django-diary-3.0rc3/diary/migrations/0002_auto_20151010_1324.py`

 * *Files identical despite different names*

### Comparing `django-diary-3.0rc2/diary/migrations/0003_auto_20151010_1331.py` & `django-diary-3.0rc3/diary/migrations/0003_auto_20151010_1331.py`

 * *Files identical despite different names*

### Comparing `django-diary-3.0rc2/diary/migrations/0004_customer_title.py` & `django-diary-3.0rc3/diary/migrations/0004_customer_title.py`

 * *Files identical despite different names*

### Comparing `django-diary-3.0rc2/diary/migrations/0005_auto_20151017_1119.py` & `django-diary-3.0rc3/diary/migrations/0005_auto_20151017_1119.py`

 * *Files identical despite different names*

### Comparing `django-diary-3.0rc2/diary/migrations/0006_auto_20151017_1347.py` & `django-diary-3.0rc3/diary/migrations/0006_auto_20151017_1347.py`

 * *Files identical despite different names*

### Comparing `django-diary-3.0rc2/diary/migrations/0007_auto_20151017_1348.py` & `django-diary-3.0rc3/diary/migrations/0007_auto_20151017_1348.py`

 * *Files identical despite different names*

### Comparing `django-diary-3.0rc2/diary/models.py` & `django-diary-3.0rc3/diary/models.py`

 * *Files identical despite different names*

### Comparing `django-diary-3.0rc2/diary/settings.py` & `django-diary-3.0rc3/diary/settings.py`

 * *Files identical despite different names*

### Comparing `django-diary-3.0rc2/diary/static/ajax_csrf.js` & `django-diary-3.0rc3/diary/static/ajax_csrf.js`

 * *Files identical despite different names*

### Comparing `django-diary-3.0rc2/diary/static/diary/base.css` & `django-diary-3.0rc3/diary/static/diary/base.css`

 * *Files identical despite different names*

### Comparing `django-diary-3.0rc2/diary/static/diary/entry_ajax_dnd.js` & `django-diary-3.0rc3/diary/static/diary/entry_ajax_dnd.js`

 * *Files identical despite different names*

### Comparing `django-diary-3.0rc2/diary/static/diary/entry_ajax_modal.js` & `django-diary-3.0rc3/diary/static/diary/entry_ajax_modal.js`

 * *Files identical despite different names*

### Comparing `django-diary-3.0rc2/diary/static/diary/multi_col.css` & `django-diary-3.0rc3/diary/static/diary/multi_col.css`

 * *Files identical despite different names*

### Comparing `django-diary-3.0rc2/diary/static/js.cookie.js` & `django-diary-3.0rc3/diary/static/js.cookie.js`

 * *Files identical despite different names*

### Comparing `django-diary-3.0rc2/diary/templates/diary/base.html` & `django-diary-3.0rc3/diary/templates/diary/base.html`

 * *Files identical despite different names*

### Comparing `django-diary-3.0rc2/diary/templates/diary/day.html` & `django-diary-3.0rc3/diary/templates/diary/day.html`

 * *Files identical despite different names*

### Comparing `django-diary-3.0rc2/diary/templates/diary/day_list.html` & `django-diary-3.0rc3/diary/templates/diary/day_list.html`

 * *Files identical despite different names*

### Comparing `django-diary-3.0rc2/diary/templates/diary/form_base.html` & `django-diary-3.0rc3/diary/templates/diary/form_base.html`

 * *Files identical despite different names*

### Comparing `django-diary-3.0rc2/diary/templates/diary/history.html` & `django-diary-3.0rc3/diary/templates/diary/history.html`

 * *Files identical despite different names*

### Comparing `django-diary-3.0rc2/diary/templates/diary/main_base.html` & `django-diary-3.0rc3/diary/templates/diary/main_base.html`

 * *Files identical despite different names*

### Comparing `django-diary-3.0rc2/diary/templates/diary/modal_base.html` & `django-diary-3.0rc3/diary/templates/diary/modal_base.html`

 * *Files identical despite different names*

### Comparing `django-diary-3.0rc2/diary/templates/diary/modal_entry.html` & `django-diary-3.0rc3/diary/templates/diary/modal_entry.html`

 * *Files identical despite different names*

### Comparing `django-diary-3.0rc2/diary/templates/diary/month.html` & `django-diary-3.0rc3/diary/templates/diary/month.html`

 * *Files identical despite different names*

### Comparing `django-diary-3.0rc2/diary/templates/diary/multi_day.html` & `django-diary-3.0rc3/diary/templates/diary/multi_day.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 {% extends 'diary/day_base.html' %}
-{% load staticfiles %}
+{% load static %}
 
 
 {% block diary_head_extra %}
     {{ block.super }}
     <link rel="stylesheet" href="{% static 'diary/multi_col.css' %}" />
 {% endblock diary_head_extra %}
 
@@ -48,15 +48,15 @@
             <div class="row">
                 <div class="col-md-1">
                     <b>{{ label }}</b>
                 </div>
                 <div class="col-md-11">
                     <div class="row cols-{{ n_cols }}">
                         {% for datetime_slug, entries, current, trading, historic, advance, allow_dnd in day_entries %}
-                            <div 
+                            <div
                                 id="{{ datetime_slug }}"
 class="col-md-1 droptarget
 {% if current %} current{% endif %}
 {% if trading %}
 {% if historic %} historic{% elif advance%} advance{% else %} trading{% endif %}
 {% else %} admin{% endif %}"
                                 {% if request.user.is_staff or allow_dnd %}
@@ -64,32 +64,32 @@
                                     ondragleave="dragleave(event);"
                                     ondragover="dragover(event);"
                                     ondrop="drop(event);"
                                     ondragend="dragend(event);"
                                 {% endif %}
                                 >
                 {% url 'diary:entry_new' slug=datetime_slug as new_entry %}
-                                <button 
-                                    class="btn btn-link new" 
-                                    type="button" 
+                                <button
+                                    class="btn btn-link new"
+                                    type="button"
 onclick="location.href='{{ new_entry }}?next={{ request.path }}'"
                                     >
                                     <span class="glyphicon glyphicon-plus">
                                     </span>
                                 </button>
                                 {% for entry in entries %}
-                                    <div 
+                                    <div
 class="entry{% if entry.cancelled %} cancelled{% endif %}{% if entry.no_show %} no_show{% endif %}"
                                         id="{{ entry.pk }}"
                                     {% if request.user.is_staff or allow_dnd %}
                                             draggable="true"
                                             ondragstart="drag(event);"
                                     {% endif %}
                                         >
-                                        <div 
+                                        <div
                     data-href="{% url 'diary:entry_modal' pk=entry.pk %}"
                                             data-toggle="modal"
                                             data-target="#ajaxModal"
                                             >
                                             {% if entry.customer %}
                                                 <b>{{ entry.customer }}</b>
                                             {% else %}
@@ -103,8 +103,7 @@
                     </div>
                 </div>
             </div>
         {% endfor %}
     </div>
 
 {% endblock diary_content %}
-
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-{% extends 'diary/day_base.html' %} {% load staticfiles %} {% block
-diary_head_extra %} {{ block.super }}
+{% extends 'diary/day_base.html' %} {% load static %} {% block diary_head_extra
+%} {{ block.super }}
  {% endblock diary_head_extra %} {% block diary_nav %} {% url 'diary:
 multi_day_nav' slug=nav_slug change='next' as diary_nav_next %} {% url 'diary:
 multi_day_nav' slug=nav_slug change='prev' as diary_nav_prev %} {% url 'diary:
 month' year=date.year month=date.month as diary_nav_up %} {{ block.super }} {%
 endblock diary_nav %} {% block diary_title %} {{ date.year }} {
 { date_start_head }} - {{ date_end_head }} {% endblock diary_title %} {% block
 diary_content %} {{ block.super }}
```

### Comparing `django-diary-3.0rc2/diary/templates/diary/reminders.html` & `django-diary-3.0rc3/diary/templates/diary/reminders.html`

 * *Files identical despite different names*

### Comparing `django-diary-3.0rc2/diary/templates/diary/year.html` & `django-diary-3.0rc3/diary/templates/diary/year.html`

 * *Files identical despite different names*

### Comparing `django-diary-3.0rc2/diary/tests.py` & `django-diary-3.0rc3/diary/tests.py`

 * *Files identical despite different names*

### Comparing `django-diary-3.0rc2/diary/urls.py` & `django-diary-3.0rc3/diary/urls.py`

 * *Files identical despite different names*

### Comparing `django-diary-3.0rc2/diary/views.py` & `django-diary-3.0rc3/diary/views.py`

 * *Files identical despite different names*

### Comparing `django-diary-3.0rc2/diary/widgets.py` & `django-diary-3.0rc3/diary/widgets.py`

 * *Files identical despite different names*

### Comparing `django-diary-3.0rc2/django_diary.egg-info/PKG-INFO` & `django-diary-3.0rc3/django_diary.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-diary
-Version: 3.0rc2
+Version: 3.0rc3
 Summary: A pluggable diary app for use in the Django framework.
 Home-page: http://pypi.python.org/pypi/diary/
 Author: Bob Bowles
 Author-email: bobjohnbowles@gmail.com
 License: MIT License
 Description: ============
         Django Diary
```

### Comparing `django-diary-3.0rc2/django_diary.egg-info/SOURCES.txt` & `django-diary-3.0rc3/django_diary.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-diary-3.0rc2/ez_setup.py` & `django-diary-3.0rc3/ez_setup.py`

 * *Files identical despite different names*

### Comparing `django-diary-3.0rc2/setup.py` & `django-diary-3.0rc3/setup.py`

 * *Files identical despite different names*

