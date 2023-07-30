# Comparing `tmp/django_msgs-1.3.31.tar.gz` & `tmp/django_msgs-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_msgs-1.3.31.tar", last modified: Fri Jun 23 15:37:13 2023, max compression
+gzip compressed data, was "django_msgs-1.4.0.tar", last modified: Sun Jul 30 19:41:30 2023, max compression
```

## Comparing `django_msgs-1.3.31.tar` & `django_msgs-1.4.0.tar`

### file list

```diff
@@ -1,62 +1,63 @@
-drwxr-xr-x   0 alexander   (501) staff       (20)        0 2023-06-23 15:37:13.671000 django_msgs-1.3.31/
--rw-r--r--   0 alexander   (501) staff       (20)     1073 2020-12-07 15:50:01.000000 django_msgs-1.3.31/LICENSE
--rw-r--r--   0 alexander   (501) staff       (20)       17 2020-12-07 15:39:16.000000 django_msgs-1.3.31/MANIFEST.in
--rw-r--r--   0 alexander   (501) staff       (20)     3910 2023-06-23 15:37:13.671115 django_msgs-1.3.31/PKG-INFO
--rw-r--r--   0 alexander   (501) staff       (20)     3323 2021-09-23 06:41:03.000000 django_msgs-1.3.31/README.md
-drwxr-xr-x   0 alexander   (501) staff       (20)        0 2023-06-23 15:37:13.648445 django_msgs-1.3.31/config/
--rw-r--r--   0 alexander   (501) staff       (20)        0 2021-07-13 19:37:37.000000 django_msgs-1.3.31/config/__init__.py
--rw-r--r--   0 alexander   (501) staff       (20)      387 2021-07-13 21:02:06.000000 django_msgs-1.3.31/config/asgi.py
--rw-r--r--   0 alexander   (501) staff       (20)     4673 2022-05-30 08:36:00.000000 django_msgs-1.3.31/config/settings.py
--rw-r--r--   0 alexander   (501) staff       (20)      746 2021-07-13 19:50:10.000000 django_msgs-1.3.31/config/urls.py
--rw-r--r--   0 alexander   (501) staff       (20)      387 2021-07-13 21:02:06.000000 django_msgs-1.3.31/config/wsgi.py
-drwxr-xr-x   0 alexander   (501) staff       (20)        0 2023-06-23 15:37:13.649869 django_msgs-1.3.31/django_msgs.egg-info/
--rw-r--r--   0 alexander   (501) staff       (20)     3910 2023-06-23 15:37:13.000000 django_msgs-1.3.31/django_msgs.egg-info/PKG-INFO
--rw-r--r--   0 alexander   (501) staff       (20)     1512 2023-06-23 15:37:13.000000 django_msgs-1.3.31/django_msgs.egg-info/SOURCES.txt
--rw-r--r--   0 alexander   (501) staff       (20)        1 2023-06-23 15:37:13.000000 django_msgs-1.3.31/django_msgs.egg-info/dependency_links.txt
--rw-r--r--   0 alexander   (501) staff       (20)       19 2023-06-23 15:37:13.000000 django_msgs-1.3.31/django_msgs.egg-info/requires.txt
--rw-r--r--   0 alexander   (501) staff       (20)       12 2023-06-23 15:37:13.000000 django_msgs-1.3.31/django_msgs.egg-info/top_level.txt
-drwxr-xr-x   0 alexander   (501) staff       (20)        0 2023-06-23 15:37:13.655551 django_msgs-1.3.31/msgs/
--rw-r--r--   0 alexander   (501) staff       (20)       43 2021-11-07 20:03:56.000000 django_msgs-1.3.31/msgs/__init__.py
-drwxr-xr-x   0 alexander   (501) staff       (20)        0 2023-06-23 15:37:13.656925 django_msgs-1.3.31/msgs/abstract/
--rw-r--r--   0 alexander   (501) staff       (20)        0 2021-07-13 18:45:04.000000 django_msgs-1.3.31/msgs/abstract/__init__.py
--rw-r--r--   0 alexander   (501) staff       (20)      748 2022-03-28 10:36:36.000000 django_msgs-1.3.31/msgs/abstract/admin.py
--rw-r--r--   0 alexander   (501) staff       (20)     6560 2023-06-23 15:24:55.000000 django_msgs-1.3.31/msgs/abstract/models.py
--rw-r--r--   0 alexander   (501) staff       (20)      811 2021-11-07 20:06:22.000000 django_msgs-1.3.31/msgs/admin.py
--rw-r--r--   0 alexander   (501) staff       (20)      213 2021-11-07 20:03:56.000000 django_msgs-1.3.31/msgs/app.py
--rw-r--r--   0 alexander   (501) staff       (20)      201 2022-06-07 11:19:07.000000 django_msgs-1.3.31/msgs/exceptions.py
--rw-r--r--   0 alexander   (501) staff       (20)      255 2021-09-28 19:56:53.000000 django_msgs-1.3.31/msgs/helpers.py
-drwxr-xr-x   0 alexander   (501) staff       (20)        0 2023-06-23 15:37:13.665354 django_msgs-1.3.31/msgs/migrations/
--rw-r--r--   0 alexander   (501) staff       (20)     2344 2020-12-08 11:49:48.000000 django_msgs-1.3.31/msgs/migrations/0001_initial.py
--rw-r--r--   0 alexander   (501) staff       (20)      692 2021-02-20 16:00:18.000000 django_msgs-1.3.31/msgs/migrations/0002_timestamped_messages.py
--rw-r--r--   0 alexander   (501) staff       (20)      795 2021-03-03 16:57:06.000000 django_msgs-1.3.31/msgs/migrations/0003_provider_fields_and_statuses.py
--rw-r--r--   0 alexander   (501) staff       (20)      883 2021-03-26 16:56:33.000000 django_msgs-1.3.31/msgs/migrations/0004_default_templates_datamigration.py
--rw-r--r--   0 alexander   (501) staff       (20)      778 2021-07-13 18:33:23.000000 django_msgs-1.3.31/msgs/migrations/0005_tpl_name_and_type.py
--rw-r--r--   0 alexander   (501) staff       (20)      596 2021-07-13 18:33:23.000000 django_msgs-1.3.31/msgs/migrations/0006_tpl_fields_changed.py
--rw-r--r--   0 alexander   (501) staff       (20)     7855 2021-07-15 16:08:11.000000 django_msgs-1.3.31/msgs/migrations/0007_auto_20210715_1608.py
--rw-r--r--   0 alexander   (501) staff       (20)     1301 2021-08-25 12:50:02.000000 django_msgs-1.3.31/msgs/migrations/0008_auto_20210825_1250.py
--rw-r--r--   0 alexander   (501) staff       (20)     2061 2022-02-06 11:05:48.000000 django_msgs-1.3.31/msgs/migrations/0009_auto_20220206_1105.py
--rw-r--r--   0 alexander   (501) staff       (20)      719 2022-03-28 11:09:32.000000 django_msgs-1.3.31/msgs/migrations/0010_auto_20220328_1109.py
--rw-r--r--   0 alexander   (501) staff       (20)     1706 2022-06-13 09:02:27.000000 django_msgs-1.3.31/msgs/migrations/0011_auto_20220613_0857.py
--rw-r--r--   0 alexander   (501) staff       (20)      764 2023-06-22 13:29:37.000000 django_msgs-1.3.31/msgs/migrations/0012_alter_email_object_id_alter_message_object_id_and_more.py
--rw-r--r--   0 alexander   (501) staff       (20)      767 2023-06-22 15:46:47.000000 django_msgs-1.3.31/msgs/migrations/0013_email_service_context_message_service_context_and_more.py
--rw-r--r--   0 alexander   (501) staff       (20)        0 2020-07-14 09:53:30.000000 django_msgs-1.3.31/msgs/migrations/__init__.py
--rw-r--r--   0 alexander   (501) staff       (20)     1997 2022-02-06 12:18:56.000000 django_msgs-1.3.31/msgs/mixins.py
--rw-r--r--   0 alexander   (501) staff       (20)     1276 2022-02-06 14:19:53.000000 django_msgs-1.3.31/msgs/models.py
-drwxr-xr-x   0 alexander   (501) staff       (20)        0 2023-06-23 15:37:13.670582 django_msgs-1.3.31/msgs/providers/
--rw-r--r--   0 alexander   (501) staff       (20)        0 2020-10-02 08:58:26.000000 django_msgs-1.3.31/msgs/providers/__init__.py
--rw-r--r--   0 alexander   (501) staff       (20)     2698 2022-06-07 12:48:29.000000 django_msgs-1.3.31/msgs/providers/base.py
--rw-r--r--   0 alexander   (501) staff       (20)      601 2021-07-15 17:03:12.000000 django_msgs-1.3.31/msgs/providers/dummy.py
--rw-r--r--   0 alexander   (501) staff       (20)     1826 2022-06-03 11:18:00.000000 django_msgs-1.3.31/msgs/providers/plivo.py
--rw-r--r--   0 alexander   (501) staff       (20)     1724 2021-07-15 17:11:26.000000 django_msgs-1.3.31/msgs/providers/sendgrid.py
--rw-r--r--   0 alexander   (501) staff       (20)     1709 2021-11-07 20:32:25.000000 django_msgs-1.3.31/msgs/providers/sendinblue.py
--rw-r--r--   0 alexander   (501) staff       (20)     2029 2021-04-16 12:11:11.000000 django_msgs-1.3.31/msgs/providers/sendinblue_sdk.py
--rw-r--r--   0 alexander   (501) staff       (20)     2235 2021-08-25 12:13:40.000000 django_msgs-1.3.31/msgs/providers/sendpulse.py
--rw-r--r--   0 alexander   (501) staff       (20)     1822 2022-05-12 11:04:22.000000 django_msgs-1.3.31/msgs/providers/telegram.py
--rw-r--r--   0 alexander   (501) staff       (20)      482 2021-04-16 12:11:11.000000 django_msgs-1.3.31/msgs/providers/twilio.py
--rw-r--r--   0 alexander   (501) staff       (20)      589 2021-04-16 12:11:11.000000 django_msgs-1.3.31/msgs/providers/voximplant.py
--rw-r--r--   0 alexander   (501) staff       (20)     1028 2022-06-07 12:15:13.000000 django_msgs-1.3.31/msgs/signals.py
--rw-r--r--   0 alexander   (501) staff       (20)       60 2020-07-14 09:53:30.000000 django_msgs-1.3.31/msgs/tests.py
--rw-r--r--   0 alexander   (501) staff       (20)      944 2021-07-16 15:56:46.000000 django_msgs-1.3.31/msgs/utils.py
--rw-r--r--   0 alexander   (501) staff       (20)       63 2020-07-14 09:53:30.000000 django_msgs-1.3.31/msgs/views.py
--rw-r--r--   0 alexander   (501) staff       (20)       79 2023-06-23 15:37:13.671849 django_msgs-1.3.31/setup.cfg
--rw-r--r--   0 alexander   (501) staff       (20)      908 2023-06-23 15:36:59.000000 django_msgs-1.3.31/setup.py
+drwxr-xr-x   0 alexander   (501) staff       (20)        0 2023-07-30 19:41:30.374569 django_msgs-1.4.0/
+-rw-r--r--   0 alexander   (501) staff       (20)     1073 2020-12-07 15:50:01.000000 django_msgs-1.4.0/LICENSE
+-rw-r--r--   0 alexander   (501) staff       (20)       17 2020-12-07 15:39:16.000000 django_msgs-1.4.0/MANIFEST.in
+-rw-r--r--   0 alexander   (501) staff       (20)     3909 2023-07-30 19:41:30.374753 django_msgs-1.4.0/PKG-INFO
+-rw-r--r--   0 alexander   (501) staff       (20)     3323 2021-09-23 06:41:03.000000 django_msgs-1.4.0/README.md
+drwxr-xr-x   0 alexander   (501) staff       (20)        0 2023-07-30 19:41:30.343108 django_msgs-1.4.0/config/
+-rw-r--r--   0 alexander   (501) staff       (20)        0 2021-07-13 19:37:37.000000 django_msgs-1.4.0/config/__init__.py
+-rw-r--r--   0 alexander   (501) staff       (20)      387 2021-07-13 21:02:06.000000 django_msgs-1.4.0/config/asgi.py
+-rw-r--r--   0 alexander   (501) staff       (20)     4673 2022-05-30 08:36:00.000000 django_msgs-1.4.0/config/settings.py
+-rw-r--r--   0 alexander   (501) staff       (20)      746 2021-07-13 19:50:10.000000 django_msgs-1.4.0/config/urls.py
+-rw-r--r--   0 alexander   (501) staff       (20)      387 2021-07-13 21:02:06.000000 django_msgs-1.4.0/config/wsgi.py
+drwxr-xr-x   0 alexander   (501) staff       (20)        0 2023-07-30 19:41:30.344846 django_msgs-1.4.0/django_msgs.egg-info/
+-rw-r--r--   0 alexander   (501) staff       (20)     3909 2023-07-30 19:41:30.000000 django_msgs-1.4.0/django_msgs.egg-info/PKG-INFO
+-rw-r--r--   0 alexander   (501) staff       (20)     1578 2023-07-30 19:41:30.000000 django_msgs-1.4.0/django_msgs.egg-info/SOURCES.txt
+-rw-r--r--   0 alexander   (501) staff       (20)        1 2023-07-30 19:41:30.000000 django_msgs-1.4.0/django_msgs.egg-info/dependency_links.txt
+-rw-r--r--   0 alexander   (501) staff       (20)       19 2023-07-30 19:41:30.000000 django_msgs-1.4.0/django_msgs.egg-info/requires.txt
+-rw-r--r--   0 alexander   (501) staff       (20)       12 2023-07-30 19:41:30.000000 django_msgs-1.4.0/django_msgs.egg-info/top_level.txt
+drwxr-xr-x   0 alexander   (501) staff       (20)        0 2023-07-30 19:41:30.352001 django_msgs-1.4.0/msgs/
+-rw-r--r--   0 alexander   (501) staff       (20)       43 2021-11-07 20:03:56.000000 django_msgs-1.4.0/msgs/__init__.py
+drwxr-xr-x   0 alexander   (501) staff       (20)        0 2023-07-30 19:41:30.353305 django_msgs-1.4.0/msgs/abstract/
+-rw-r--r--   0 alexander   (501) staff       (20)        0 2021-07-13 18:45:04.000000 django_msgs-1.4.0/msgs/abstract/__init__.py
+-rw-r--r--   0 alexander   (501) staff       (20)      748 2022-03-28 10:36:36.000000 django_msgs-1.4.0/msgs/abstract/admin.py
+-rw-r--r--   0 alexander   (501) staff       (20)     6560 2023-06-23 15:24:55.000000 django_msgs-1.4.0/msgs/abstract/models.py
+-rw-r--r--   0 alexander   (501) staff       (20)      811 2021-11-07 20:06:22.000000 django_msgs-1.4.0/msgs/admin.py
+-rw-r--r--   0 alexander   (501) staff       (20)      213 2021-11-07 20:03:56.000000 django_msgs-1.4.0/msgs/app.py
+-rw-r--r--   0 alexander   (501) staff       (20)      201 2022-06-07 11:19:07.000000 django_msgs-1.4.0/msgs/exceptions.py
+-rw-r--r--   0 alexander   (501) staff       (20)      255 2021-09-28 19:56:53.000000 django_msgs-1.4.0/msgs/helpers.py
+drwxr-xr-x   0 alexander   (501) staff       (20)        0 2023-07-30 19:41:30.364818 django_msgs-1.4.0/msgs/migrations/
+-rw-r--r--   0 alexander   (501) staff       (20)     2344 2020-12-08 11:49:48.000000 django_msgs-1.4.0/msgs/migrations/0001_initial.py
+-rw-r--r--   0 alexander   (501) staff       (20)      692 2021-02-20 16:00:18.000000 django_msgs-1.4.0/msgs/migrations/0002_timestamped_messages.py
+-rw-r--r--   0 alexander   (501) staff       (20)      795 2021-03-03 16:57:06.000000 django_msgs-1.4.0/msgs/migrations/0003_provider_fields_and_statuses.py
+-rw-r--r--   0 alexander   (501) staff       (20)      883 2021-03-26 16:56:33.000000 django_msgs-1.4.0/msgs/migrations/0004_default_templates_datamigration.py
+-rw-r--r--   0 alexander   (501) staff       (20)      778 2021-07-13 18:33:23.000000 django_msgs-1.4.0/msgs/migrations/0005_tpl_name_and_type.py
+-rw-r--r--   0 alexander   (501) staff       (20)      596 2021-07-13 18:33:23.000000 django_msgs-1.4.0/msgs/migrations/0006_tpl_fields_changed.py
+-rw-r--r--   0 alexander   (501) staff       (20)     7855 2021-07-15 16:08:11.000000 django_msgs-1.4.0/msgs/migrations/0007_auto_20210715_1608.py
+-rw-r--r--   0 alexander   (501) staff       (20)     1301 2021-08-25 12:50:02.000000 django_msgs-1.4.0/msgs/migrations/0008_auto_20210825_1250.py
+-rw-r--r--   0 alexander   (501) staff       (20)     2061 2022-02-06 11:05:48.000000 django_msgs-1.4.0/msgs/migrations/0009_auto_20220206_1105.py
+-rw-r--r--   0 alexander   (501) staff       (20)      719 2022-03-28 11:09:32.000000 django_msgs-1.4.0/msgs/migrations/0010_auto_20220328_1109.py
+-rw-r--r--   0 alexander   (501) staff       (20)     1706 2022-06-13 09:02:27.000000 django_msgs-1.4.0/msgs/migrations/0011_auto_20220613_0857.py
+-rw-r--r--   0 alexander   (501) staff       (20)      764 2023-06-22 13:29:37.000000 django_msgs-1.4.0/msgs/migrations/0012_alter_email_object_id_alter_message_object_id_and_more.py
+-rw-r--r--   0 alexander   (501) staff       (20)      767 2023-06-22 15:46:47.000000 django_msgs-1.4.0/msgs/migrations/0013_email_service_context_message_service_context_and_more.py
+-rw-r--r--   0 alexander   (501) staff       (20)      723 2023-07-30 19:40:34.000000 django_msgs-1.4.0/msgs/migrations/0014_email_bcc_emails_email_cc_emails_and_more.py
+-rw-r--r--   0 alexander   (501) staff       (20)        0 2020-07-14 09:53:30.000000 django_msgs-1.4.0/msgs/migrations/__init__.py
+-rw-r--r--   0 alexander   (501) staff       (20)     1997 2022-02-06 12:18:56.000000 django_msgs-1.4.0/msgs/mixins.py
+-rw-r--r--   0 alexander   (501) staff       (20)     1453 2023-07-30 19:38:33.000000 django_msgs-1.4.0/msgs/models.py
+drwxr-xr-x   0 alexander   (501) staff       (20)        0 2023-07-30 19:41:30.374133 django_msgs-1.4.0/msgs/providers/
+-rw-r--r--   0 alexander   (501) staff       (20)        0 2020-10-02 08:58:26.000000 django_msgs-1.4.0/msgs/providers/__init__.py
+-rw-r--r--   0 alexander   (501) staff       (20)     2698 2022-06-07 12:48:29.000000 django_msgs-1.4.0/msgs/providers/base.py
+-rw-r--r--   0 alexander   (501) staff       (20)      601 2021-07-15 17:03:12.000000 django_msgs-1.4.0/msgs/providers/dummy.py
+-rw-r--r--   0 alexander   (501) staff       (20)     1826 2022-06-03 11:18:00.000000 django_msgs-1.4.0/msgs/providers/plivo.py
+-rw-r--r--   0 alexander   (501) staff       (20)     2254 2023-07-30 19:38:33.000000 django_msgs-1.4.0/msgs/providers/sendgrid.py
+-rw-r--r--   0 alexander   (501) staff       (20)     1709 2021-11-07 20:32:25.000000 django_msgs-1.4.0/msgs/providers/sendinblue.py
+-rw-r--r--   0 alexander   (501) staff       (20)     2029 2021-04-16 12:11:11.000000 django_msgs-1.4.0/msgs/providers/sendinblue_sdk.py
+-rw-r--r--   0 alexander   (501) staff       (20)     2235 2021-08-25 12:13:40.000000 django_msgs-1.4.0/msgs/providers/sendpulse.py
+-rw-r--r--   0 alexander   (501) staff       (20)     1822 2022-05-12 11:04:22.000000 django_msgs-1.4.0/msgs/providers/telegram.py
+-rw-r--r--   0 alexander   (501) staff       (20)      482 2021-04-16 12:11:11.000000 django_msgs-1.4.0/msgs/providers/twilio.py
+-rw-r--r--   0 alexander   (501) staff       (20)      589 2021-04-16 12:11:11.000000 django_msgs-1.4.0/msgs/providers/voximplant.py
+-rw-r--r--   0 alexander   (501) staff       (20)     1028 2022-06-07 12:15:13.000000 django_msgs-1.4.0/msgs/signals.py
+-rw-r--r--   0 alexander   (501) staff       (20)       60 2020-07-14 09:53:30.000000 django_msgs-1.4.0/msgs/tests.py
+-rw-r--r--   0 alexander   (501) staff       (20)      944 2021-07-16 15:56:46.000000 django_msgs-1.4.0/msgs/utils.py
+-rw-r--r--   0 alexander   (501) staff       (20)       63 2020-07-14 09:53:30.000000 django_msgs-1.4.0/msgs/views.py
+-rw-r--r--   0 alexander   (501) staff       (20)       79 2023-07-30 19:41:30.375487 django_msgs-1.4.0/setup.cfg
+-rw-r--r--   0 alexander   (501) staff       (20)      907 2023-07-30 19:41:26.000000 django_msgs-1.4.0/setup.py
```

### Comparing `django_msgs-1.3.31/LICENSE` & `django_msgs-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.31/PKG-INFO` & `django_msgs-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_msgs
-Version: 1.3.31
+Version: 1.4.0
 Summary: Emails and SMSs managing framework for Django
 Home-page: https://github.com/san4ezy/django_msgs
 Author: Alexander Yudkin
 Author-email: san4ezy@gmail.com
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
```

### Comparing `django_msgs-1.3.31/README.md` & `django_msgs-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.31/config/settings.py` & `django_msgs-1.4.0/config/settings.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.31/config/urls.py` & `django_msgs-1.4.0/config/urls.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.31/django_msgs.egg-info/PKG-INFO` & `django_msgs-1.4.0/django_msgs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-msgs
-Version: 1.3.31
+Version: 1.4.0
 Summary: Emails and SMSs managing framework for Django
 Home-page: https://github.com/san4ezy/django_msgs
 Author: Alexander Yudkin
 Author-email: san4ezy@gmail.com
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
```

### Comparing `django_msgs-1.3.31/django_msgs.egg-info/SOURCES.txt` & `django_msgs-1.4.0/django_msgs.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 msgs/migrations/0007_auto_20210715_1608.py
 msgs/migrations/0008_auto_20210825_1250.py
 msgs/migrations/0009_auto_20220206_1105.py
 msgs/migrations/0010_auto_20220328_1109.py
 msgs/migrations/0011_auto_20220613_0857.py
 msgs/migrations/0012_alter_email_object_id_alter_message_object_id_and_more.py
 msgs/migrations/0013_email_service_context_message_service_context_and_more.py
+msgs/migrations/0014_email_bcc_emails_email_cc_emails_and_more.py
 msgs/migrations/__init__.py
 msgs/providers/__init__.py
 msgs/providers/base.py
 msgs/providers/dummy.py
 msgs/providers/plivo.py
 msgs/providers/sendgrid.py
 msgs/providers/sendinblue.py
```

### Comparing `django_msgs-1.3.31/msgs/abstract/admin.py` & `django_msgs-1.4.0/msgs/abstract/admin.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.31/msgs/abstract/models.py` & `django_msgs-1.4.0/msgs/abstract/models.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.31/msgs/admin.py` & `django_msgs-1.4.0/msgs/admin.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.31/msgs/migrations/0001_initial.py` & `django_msgs-1.4.0/msgs/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.31/msgs/migrations/0002_timestamped_messages.py` & `django_msgs-1.4.0/msgs/migrations/0002_timestamped_messages.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.31/msgs/migrations/0003_provider_fields_and_statuses.py` & `django_msgs-1.4.0/msgs/migrations/0003_provider_fields_and_statuses.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.31/msgs/migrations/0004_default_templates_datamigration.py` & `django_msgs-1.4.0/msgs/migrations/0004_default_templates_datamigration.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.31/msgs/migrations/0005_tpl_name_and_type.py` & `django_msgs-1.4.0/msgs/migrations/0005_tpl_name_and_type.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.31/msgs/migrations/0006_tpl_fields_changed.py` & `django_msgs-1.4.0/msgs/migrations/0006_tpl_fields_changed.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.31/msgs/migrations/0007_auto_20210715_1608.py` & `django_msgs-1.4.0/msgs/migrations/0007_auto_20210715_1608.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.31/msgs/migrations/0008_auto_20210825_1250.py` & `django_msgs-1.4.0/msgs/migrations/0008_auto_20210825_1250.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.31/msgs/migrations/0009_auto_20220206_1105.py` & `django_msgs-1.4.0/msgs/migrations/0009_auto_20220206_1105.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.31/msgs/migrations/0010_auto_20220328_1109.py` & `django_msgs-1.4.0/msgs/migrations/0010_auto_20220328_1109.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.31/msgs/migrations/0011_auto_20220613_0857.py` & `django_msgs-1.4.0/msgs/migrations/0011_auto_20220613_0857.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.31/msgs/migrations/0012_alter_email_object_id_alter_message_object_id_and_more.py` & `django_msgs-1.4.0/msgs/migrations/0012_alter_email_object_id_alter_message_object_id_and_more.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.31/msgs/migrations/0013_email_service_context_message_service_context_and_more.py` & `django_msgs-1.4.0/msgs/migrations/0013_email_service_context_message_service_context_and_more.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.31/msgs/mixins.py` & `django_msgs-1.4.0/msgs/mixins.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.31/msgs/models.py` & `django_msgs-1.4.0/msgs/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Iterable
 
 from django.conf import settings
 from django.db import models
 
 from msgs.abstract.models import AbstractTemplate, AbstractMessage, AbstractAttachment
+from msgs.helpers import NULLABLE
 
 
 class SMSTemplate(AbstractTemplate):
     pass
 
 
 class EmailTemplate(AbstractTemplate):
@@ -33,14 +34,18 @@
         verbose_name_plural = 'SMS'
 
 
 class Email(AbstractMessage):
     template = models.ForeignKey(EmailTemplate, on_delete=models.CASCADE)
     attachments = models.ManyToManyField(EmailAttachment)
 
+    reply_to_emails = models.TextField(default='')
+    cc_emails = models.TextField(default='')
+    bcc_emails = models.TextField(default='')
+
     def get_provider_name(self):
         return settings.MSGS['email']
 
     def add_attachments(self, attachments: Iterable[str]):
         for item in attachments:
             attachment = EmailAttachment.objects.create(file=item)
             self.attachments.add(attachment)
```

### Comparing `django_msgs-1.3.31/msgs/providers/base.py` & `django_msgs-1.4.0/msgs/providers/base.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.31/msgs/providers/dummy.py` & `django_msgs-1.4.0/msgs/providers/dummy.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.31/msgs/providers/plivo.py` & `django_msgs-1.4.0/msgs/providers/plivo.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.31/msgs/providers/sendgrid.py` & `django_msgs-1.4.0/msgs/providers/sendgrid.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from django.conf import settings
 
 from msgs.abstract.models import AbstractMessage
-from sendgrid import SendGridAPIClient, Mail, Attachment, FileContent, FileName, FileType, Disposition, ContentId
+from sendgrid import SendGridAPIClient, Mail, Email, Attachment, FileContent, FileName, FileType, Disposition, ContentId
 
 from msgs.providers.base import BaseEmailProvider
 from msgs.mixins import TemplatingMixin
 
 
 class SendgridEmailProvider(TemplatingMixin, BaseEmailProvider):
     settings = settings.MSGS['providers']['sendgrid']['options']
@@ -21,14 +21,31 @@
         attachments = self.get_attachments(message, lang, context)
         sendgrid_message = Mail(
             from_email=self.get_sender(),
             to_emails=message.recipient,
             subject=title_html,
             html_content=body_html,
         )
+
+        reply_to_emails = message.reply_to_emails
+        if reply_to_emails:
+            sendgrid_message.reply_to = [Email(rt) for rt in reply_to_emails]
+
+        cc_emails = message.cc_emails
+        if cc_emails:
+            sendgrid_message.personalizations[0].add_cc(
+                [Email(cc) for cc in cc_emails]
+            )
+
+        bcc_emails = message.bcc_emails
+        if bcc_emails:
+            sendgrid_message.personalizations[0].add_bcc(
+                [Email(cc) for cc in bcc_emails]
+            )
+
         for attachment in attachments:
             sendgrid_message.add_attachment(attachment)
         # sendgrid_message.add_attachment(self.get_logo_attachment())  # must be removed to the child class for the library version
         response = self.client.send(sendgrid_message)
         return response
 
     def build_attachment_object(self, **kwargs):
```

### Comparing `django_msgs-1.3.31/msgs/providers/sendinblue.py` & `django_msgs-1.4.0/msgs/providers/sendinblue.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.31/msgs/providers/sendinblue_sdk.py` & `django_msgs-1.4.0/msgs/providers/sendinblue_sdk.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.31/msgs/providers/sendpulse.py` & `django_msgs-1.4.0/msgs/providers/sendpulse.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.31/msgs/providers/telegram.py` & `django_msgs-1.4.0/msgs/providers/telegram.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.31/msgs/providers/voximplant.py` & `django_msgs-1.4.0/msgs/providers/voximplant.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.31/msgs/signals.py` & `django_msgs-1.4.0/msgs/signals.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.31/msgs/utils.py` & `django_msgs-1.4.0/msgs/utils.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.31/setup.py` & `django_msgs-1.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="django_msgs",
-    version="1.3.31",
+    version="1.4.0",
     author="Alexander Yudkin",
     author_email="san4ezy@gmail.com",
     description="Emails and SMSs managing framework for Django",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/san4ezy/django_msgs",
     packages=setuptools.find_packages(),
```

