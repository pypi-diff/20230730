# Comparing `tmp/lbg-1.2.8.tar.gz` & `tmp/lbg-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lbg-1.2.8.tar", last modified: Tue Nov 29 12:04:17 2022, max compression
+gzip compressed data, was "lbg-1.2.9.tar", last modified: Thu Dec  1 03:55:29 2022, max compression
```

## Comparing `lbg-1.2.8.tar` & `lbg-1.2.9.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 zhiweizhang   (501) staff       (20)        0 2022-11-29 12:04:17.992891 lbg-1.2.8/
--rw-r--r--   0 zhiweizhang   (501) staff       (20)     1542 2022-07-21 10:13:57.000000 lbg-1.2.8/LICENSE
--rw-r--r--   0 zhiweizhang   (501) staff       (20)      206 2022-11-29 12:04:17.992726 lbg-1.2.8/PKG-INFO
--rw-r--r--   0 zhiweizhang   (501) staff       (20)    10956 2022-07-21 10:13:57.000000 lbg-1.2.8/README.md
-drwxr-xr-x   0 zhiweizhang   (501) staff       (20)        0 2022-11-29 12:04:17.983219 lbg-1.2.8/lbg.egg-info/
--rw-r--r--   0 zhiweizhang   (501) staff       (20)      206 2022-11-29 12:04:17.000000 lbg-1.2.8/lbg.egg-info/PKG-INFO
--rw-r--r--   0 zhiweizhang   (501) staff       (20)      993 2022-11-29 12:04:17.000000 lbg-1.2.8/lbg.egg-info/SOURCES.txt
--rw-r--r--   0 zhiweizhang   (501) staff       (20)        1 2022-11-29 12:04:17.000000 lbg-1.2.8/lbg.egg-info/dependency_links.txt
--rw-r--r--   0 zhiweizhang   (501) staff       (20)       80 2022-11-29 12:04:17.000000 lbg-1.2.8/lbg.egg-info/entry_points.txt
--rw-r--r--   0 zhiweizhang   (501) staff       (20)      212 2022-11-29 12:04:17.000000 lbg-1.2.8/lbg.egg-info/requires.txt
--rw-r--r--   0 zhiweizhang   (501) staff       (20)       37 2022-11-29 12:04:17.000000 lbg-1.2.8/lbg.egg-info/top_level.txt
-drwxr-xr-x   0 zhiweizhang   (501) staff       (20)        0 2022-11-29 12:04:17.984848 lbg-1.2.8/lbgcli/
--rw-r--r--   0 zhiweizhang   (501) staff       (20)       22 2022-11-29 12:03:23.000000 lbg-1.2.8/lbgcli/__init__.py
-drwxr-xr-x   0 zhiweizhang   (501) staff       (20)        0 2022-11-29 12:04:17.985265 lbg-1.2.8/lbgcli/config/
--rw-r--r--   0 zhiweizhang   (501) staff       (20)        0 2022-07-21 10:13:58.000000 lbg-1.2.8/lbgcli/config/__init__.py
--rw-r--r--   0 zhiweizhang   (501) staff       (20)     7612 2022-08-10 06:38:10.000000 lbg-1.2.8/lbgcli/config/config.py
--rw-r--r--   0 zhiweizhang   (501) staff       (20)     1017 2022-11-29 09:13:00.000000 lbg-1.2.8/lbgcli/const.py
-drwxr-xr-x   0 zhiweizhang   (501) staff       (20)        0 2022-11-29 12:04:17.985844 lbg-1.2.8/lbgcli/history/
--rw-r--r--   0 zhiweizhang   (501) staff       (20)        0 2022-07-21 10:13:58.000000 lbg-1.2.8/lbgcli/history/__init__.py
--rw-r--r--   0 zhiweizhang   (501) staff       (20)     3240 2022-07-21 10:40:34.000000 lbg-1.2.8/lbgcli/history/history.py
-drwxr-xr-x   0 zhiweizhang   (501) staff       (20)        0 2022-11-29 12:04:17.986326 lbg-1.2.8/lbgcli/image/
--rw-r--r--   0 zhiweizhang   (501) staff       (20)        0 2022-07-21 10:13:58.000000 lbg-1.2.8/lbgcli/image/__init__.py
--rw-r--r--   0 zhiweizhang   (501) staff       (20)     6480 2022-11-22 09:50:26.000000 lbg-1.2.8/lbgcli/image/image.py
-drwxr-xr-x   0 zhiweizhang   (501) staff       (20)        0 2022-11-29 12:04:17.987108 lbg-1.2.8/lbgcli/job/
--rw-r--r--   0 zhiweizhang   (501) staff       (20)        0 2022-07-21 10:13:58.000000 lbg-1.2.8/lbgcli/job/__init__.py
--rw-r--r--   0 zhiweizhang   (501) staff       (20)    15989 2022-07-21 10:13:58.000000 lbg-1.2.8/lbgcli/job/_jcc.py
--rw-r--r--   0 zhiweizhang   (501) staff       (20)    31620 2022-11-29 12:02:40.000000 lbg-1.2.8/lbgcli/job/job.py
-drwxr-xr-x   0 zhiweizhang   (501) staff       (20)        0 2022-11-29 12:04:17.987662 lbg-1.2.8/lbgcli/job_group/
--rw-r--r--   0 zhiweizhang   (501) staff       (20)        0 2022-07-21 10:13:58.000000 lbg-1.2.8/lbgcli/job_group/__init__.py
--rw-r--r--   0 zhiweizhang   (501) staff       (20)     8722 2022-11-04 03:09:05.000000 lbg-1.2.8/lbgcli/job_group/job_group.py
-drwxr-xr-x   0 zhiweizhang   (501) staff       (20)        0 2022-11-29 12:04:17.988198 lbg-1.2.8/lbgcli/machine/
--rw-r--r--   0 zhiweizhang   (501) staff       (20)        0 2022-07-21 10:40:34.000000 lbg-1.2.8/lbgcli/machine/__init__.py
--rw-r--r--   0 zhiweizhang   (501) staff       (20)     2657 2022-11-04 03:09:05.000000 lbg-1.2.8/lbgcli/machine/machine.py
--rw-r--r--   0 zhiweizhang   (501) staff       (20)    11233 2022-11-29 09:13:00.000000 lbg-1.2.8/lbgcli/main_entry.py
--rw-r--r--   0 zhiweizhang   (501) staff       (20)       44 2022-07-21 10:40:34.000000 lbg-1.2.8/lbgcli/meta.py
--rw-r--r--   0 zhiweizhang   (501) staff       (20)     3486 2022-11-29 09:13:00.000000 lbg-1.2.8/lbgcli/module_impl.py
-drwxr-xr-x   0 zhiweizhang   (501) staff       (20)        0 2022-11-29 12:04:17.988690 lbg-1.2.8/lbgcli/node/
--rw-r--r--   0 zhiweizhang   (501) staff       (20)        0 2022-07-21 10:13:58.000000 lbg-1.2.8/lbgcli/node/__init__.py
--rw-r--r--   0 zhiweizhang   (501) staff       (20)     8724 2022-11-04 03:09:05.000000 lbg-1.2.8/lbgcli/node/node.py
-drwxr-xr-x   0 zhiweizhang   (501) staff       (20)        0 2022-11-29 12:04:17.989197 lbg-1.2.8/lbgcli/program/
--rw-r--r--   0 zhiweizhang   (501) staff       (20)        0 2022-07-21 10:13:58.000000 lbg-1.2.8/lbgcli/program/__init__.py
--rw-r--r--   0 zhiweizhang   (501) staff       (20)     6804 2022-11-04 03:09:05.000000 lbg-1.2.8/lbgcli/program/program.py
--rw-r--r--   0 zhiweizhang   (501) staff       (20)     4410 2022-11-29 09:13:00.000000 lbg-1.2.8/lbgcli/util.py
-drwxr-xr-x   0 zhiweizhang   (501) staff       (20)        0 2022-11-29 12:04:17.991302 lbg-1.2.8/lbgcore/
--rw-r--r--   0 zhiweizhang   (501) staff       (20)        0 2022-07-21 10:13:58.000000 lbg-1.2.8/lbgcore/__init__.py
--rw-r--r--   0 zhiweizhang   (501) staff       (20)     3910 2022-09-26 03:21:01.000000 lbg-1.2.8/lbgcore/client.py
--rw-r--r--   0 zhiweizhang   (501) staff       (20)     1420 2022-07-21 10:40:34.000000 lbg-1.2.8/lbgcore/image.py
--rw-r--r--   0 zhiweizhang   (501) staff       (20)     4390 2022-11-29 09:13:00.000000 lbg-1.2.8/lbgcore/job.py
--rw-r--r--   0 zhiweizhang   (501) staff       (20)     2416 2022-07-21 10:40:34.000000 lbg-1.2.8/lbgcore/jobgroup.py
--rw-r--r--   0 zhiweizhang   (501) staff       (20)     1327 2022-11-04 03:09:05.000000 lbg-1.2.8/lbgcore/machine.py
--rw-r--r--   0 zhiweizhang   (501) staff       (20)     1061 2022-07-21 10:40:34.000000 lbg-1.2.8/lbgcore/program.py
--rw-r--r--   0 zhiweizhang   (501) staff       (20)     1382 2022-07-21 10:40:34.000000 lbg-1.2.8/lbgcore/server.py
--rw-r--r--   0 zhiweizhang   (501) staff       (20)        0 2022-07-21 10:13:58.000000 lbg-1.2.8/lbgcore/util.py
-drwxr-xr-x   0 zhiweizhang   (501) staff       (20)        0 2022-11-29 12:04:17.991779 lbg-1.2.8/lebesgue_sdk/
--rw-r--r--   0 zhiweizhang   (501) staff       (20)        0 2022-07-21 10:13:58.000000 lbg-1.2.8/lebesgue_sdk/__init__.py
--rw-r--r--   0 zhiweizhang   (501) staff       (20)    17163 2022-07-21 10:40:34.000000 lbg-1.2.8/lebesgue_sdk/cmd.py
--rw-r--r--   0 zhiweizhang   (501) staff       (20)    20099 2022-07-21 10:40:34.000000 lbg-1.2.8/lebesgue_sdk/lebesgue_sdk.py
--rw-r--r--   0 zhiweizhang   (501) staff       (20)       38 2022-11-29 12:04:17.992929 lbg-1.2.8/setup.cfg
--rw-r--r--   0 zhiweizhang   (501) staff       (20)     1076 2022-11-29 09:14:27.000000 lbg-1.2.8/setup.py
-drwxr-xr-x   0 zhiweizhang   (501) staff       (20)        0 2022-11-29 12:04:17.992509 lbg-1.2.8/tiefblue/
--rw-r--r--   0 zhiweizhang   (501) staff       (20)       64 2022-11-29 10:30:01.000000 lbg-1.2.8/tiefblue/__init__.py
--rw-r--r--   0 zhiweizhang   (501) staff       (20)     9260 2022-11-29 09:13:00.000000 lbg-1.2.8/tiefblue/client.py
+drwxr-xr-x   0 zhiweizhang   (501) staff       (20)        0 2022-12-01 03:55:29.358653 lbg-1.2.9/
+-rw-r--r--   0 zhiweizhang   (501) staff       (20)     1542 2022-07-21 10:13:57.000000 lbg-1.2.9/LICENSE
+-rw-r--r--   0 zhiweizhang   (501) staff       (20)      206 2022-12-01 03:55:29.358501 lbg-1.2.9/PKG-INFO
+-rw-r--r--   0 zhiweizhang   (501) staff       (20)    10956 2022-07-21 10:13:57.000000 lbg-1.2.9/README.md
+drwxr-xr-x   0 zhiweizhang   (501) staff       (20)        0 2022-12-01 03:55:29.350990 lbg-1.2.9/lbg.egg-info/
+-rw-r--r--   0 zhiweizhang   (501) staff       (20)      206 2022-12-01 03:55:29.000000 lbg-1.2.9/lbg.egg-info/PKG-INFO
+-rw-r--r--   0 zhiweizhang   (501) staff       (20)      993 2022-12-01 03:55:29.000000 lbg-1.2.9/lbg.egg-info/SOURCES.txt
+-rw-r--r--   0 zhiweizhang   (501) staff       (20)        1 2022-12-01 03:55:29.000000 lbg-1.2.9/lbg.egg-info/dependency_links.txt
+-rw-r--r--   0 zhiweizhang   (501) staff       (20)       80 2022-12-01 03:55:29.000000 lbg-1.2.9/lbg.egg-info/entry_points.txt
+-rw-r--r--   0 zhiweizhang   (501) staff       (20)      212 2022-12-01 03:55:29.000000 lbg-1.2.9/lbg.egg-info/requires.txt
+-rw-r--r--   0 zhiweizhang   (501) staff       (20)       37 2022-12-01 03:55:29.000000 lbg-1.2.9/lbg.egg-info/top_level.txt
+drwxr-xr-x   0 zhiweizhang   (501) staff       (20)        0 2022-12-01 03:55:29.352151 lbg-1.2.9/lbgcli/
+-rw-r--r--   0 zhiweizhang   (501) staff       (20)       22 2022-12-01 03:54:59.000000 lbg-1.2.9/lbgcli/__init__.py
+drwxr-xr-x   0 zhiweizhang   (501) staff       (20)        0 2022-12-01 03:55:29.352495 lbg-1.2.9/lbgcli/config/
+-rw-r--r--   0 zhiweizhang   (501) staff       (20)        0 2022-07-21 10:13:58.000000 lbg-1.2.9/lbgcli/config/__init__.py
+-rw-r--r--   0 zhiweizhang   (501) staff       (20)     7612 2022-08-10 06:38:10.000000 lbg-1.2.9/lbgcli/config/config.py
+-rw-r--r--   0 zhiweizhang   (501) staff       (20)     1017 2022-11-29 09:13:00.000000 lbg-1.2.9/lbgcli/const.py
+drwxr-xr-x   0 zhiweizhang   (501) staff       (20)        0 2022-12-01 03:55:29.352877 lbg-1.2.9/lbgcli/history/
+-rw-r--r--   0 zhiweizhang   (501) staff       (20)        0 2022-07-21 10:13:58.000000 lbg-1.2.9/lbgcli/history/__init__.py
+-rw-r--r--   0 zhiweizhang   (501) staff       (20)     3240 2022-07-21 10:40:34.000000 lbg-1.2.9/lbgcli/history/history.py
+drwxr-xr-x   0 zhiweizhang   (501) staff       (20)        0 2022-12-01 03:55:29.353204 lbg-1.2.9/lbgcli/image/
+-rw-r--r--   0 zhiweizhang   (501) staff       (20)        0 2022-07-21 10:13:58.000000 lbg-1.2.9/lbgcli/image/__init__.py
+-rw-r--r--   0 zhiweizhang   (501) staff       (20)     6480 2022-11-22 09:50:26.000000 lbg-1.2.9/lbgcli/image/image.py
+drwxr-xr-x   0 zhiweizhang   (501) staff       (20)        0 2022-12-01 03:55:29.353846 lbg-1.2.9/lbgcli/job/
+-rw-r--r--   0 zhiweizhang   (501) staff       (20)        0 2022-07-21 10:13:58.000000 lbg-1.2.9/lbgcli/job/__init__.py
+-rw-r--r--   0 zhiweizhang   (501) staff       (20)    15989 2022-07-21 10:13:58.000000 lbg-1.2.9/lbgcli/job/_jcc.py
+-rw-r--r--   0 zhiweizhang   (501) staff       (20)    31879 2022-12-01 03:54:00.000000 lbg-1.2.9/lbgcli/job/job.py
+drwxr-xr-x   0 zhiweizhang   (501) staff       (20)        0 2022-12-01 03:55:29.354356 lbg-1.2.9/lbgcli/job_group/
+-rw-r--r--   0 zhiweizhang   (501) staff       (20)        0 2022-07-21 10:13:58.000000 lbg-1.2.9/lbgcli/job_group/__init__.py
+-rw-r--r--   0 zhiweizhang   (501) staff       (20)     8722 2022-11-04 03:09:05.000000 lbg-1.2.9/lbgcli/job_group/job_group.py
+drwxr-xr-x   0 zhiweizhang   (501) staff       (20)        0 2022-12-01 03:55:29.354910 lbg-1.2.9/lbgcli/machine/
+-rw-r--r--   0 zhiweizhang   (501) staff       (20)        0 2022-07-21 10:40:34.000000 lbg-1.2.9/lbgcli/machine/__init__.py
+-rw-r--r--   0 zhiweizhang   (501) staff       (20)     2657 2022-11-04 03:09:05.000000 lbg-1.2.9/lbgcli/machine/machine.py
+-rw-r--r--   0 zhiweizhang   (501) staff       (20)    11233 2022-11-29 09:13:00.000000 lbg-1.2.9/lbgcli/main_entry.py
+-rw-r--r--   0 zhiweizhang   (501) staff       (20)       44 2022-07-21 10:40:34.000000 lbg-1.2.9/lbgcli/meta.py
+-rw-r--r--   0 zhiweizhang   (501) staff       (20)     3486 2022-11-29 09:13:00.000000 lbg-1.2.9/lbgcli/module_impl.py
+drwxr-xr-x   0 zhiweizhang   (501) staff       (20)        0 2022-12-01 03:55:29.355225 lbg-1.2.9/lbgcli/node/
+-rw-r--r--   0 zhiweizhang   (501) staff       (20)        0 2022-07-21 10:13:58.000000 lbg-1.2.9/lbgcli/node/__init__.py
+-rw-r--r--   0 zhiweizhang   (501) staff       (20)     8724 2022-11-04 03:09:05.000000 lbg-1.2.9/lbgcli/node/node.py
+drwxr-xr-x   0 zhiweizhang   (501) staff       (20)        0 2022-12-01 03:55:29.355451 lbg-1.2.9/lbgcli/program/
+-rw-r--r--   0 zhiweizhang   (501) staff       (20)        0 2022-07-21 10:13:58.000000 lbg-1.2.9/lbgcli/program/__init__.py
+-rw-r--r--   0 zhiweizhang   (501) staff       (20)     6804 2022-11-04 03:09:05.000000 lbg-1.2.9/lbgcli/program/program.py
+-rw-r--r--   0 zhiweizhang   (501) staff       (20)     4410 2022-11-29 09:13:00.000000 lbg-1.2.9/lbgcli/util.py
+drwxr-xr-x   0 zhiweizhang   (501) staff       (20)        0 2022-12-01 03:55:29.357176 lbg-1.2.9/lbgcore/
+-rw-r--r--   0 zhiweizhang   (501) staff       (20)        0 2022-07-21 10:13:58.000000 lbg-1.2.9/lbgcore/__init__.py
+-rw-r--r--   0 zhiweizhang   (501) staff       (20)     3910 2022-09-26 03:21:01.000000 lbg-1.2.9/lbgcore/client.py
+-rw-r--r--   0 zhiweizhang   (501) staff       (20)     1420 2022-07-21 10:40:34.000000 lbg-1.2.9/lbgcore/image.py
+-rw-r--r--   0 zhiweizhang   (501) staff       (20)     4390 2022-11-29 09:13:00.000000 lbg-1.2.9/lbgcore/job.py
+-rw-r--r--   0 zhiweizhang   (501) staff       (20)     2416 2022-07-21 10:40:34.000000 lbg-1.2.9/lbgcore/jobgroup.py
+-rw-r--r--   0 zhiweizhang   (501) staff       (20)     1327 2022-11-04 03:09:05.000000 lbg-1.2.9/lbgcore/machine.py
+-rw-r--r--   0 zhiweizhang   (501) staff       (20)     1061 2022-07-21 10:40:34.000000 lbg-1.2.9/lbgcore/program.py
+-rw-r--r--   0 zhiweizhang   (501) staff       (20)     1382 2022-07-21 10:40:34.000000 lbg-1.2.9/lbgcore/server.py
+-rw-r--r--   0 zhiweizhang   (501) staff       (20)        0 2022-07-21 10:13:58.000000 lbg-1.2.9/lbgcore/util.py
+drwxr-xr-x   0 zhiweizhang   (501) staff       (20)        0 2022-12-01 03:55:29.357759 lbg-1.2.9/lebesgue_sdk/
+-rw-r--r--   0 zhiweizhang   (501) staff       (20)        0 2022-07-21 10:13:58.000000 lbg-1.2.9/lebesgue_sdk/__init__.py
+-rw-r--r--   0 zhiweizhang   (501) staff       (20)    17163 2022-07-21 10:40:34.000000 lbg-1.2.9/lebesgue_sdk/cmd.py
+-rw-r--r--   0 zhiweizhang   (501) staff       (20)    20099 2022-07-21 10:40:34.000000 lbg-1.2.9/lebesgue_sdk/lebesgue_sdk.py
+-rw-r--r--   0 zhiweizhang   (501) staff       (20)       38 2022-12-01 03:55:29.358689 lbg-1.2.9/setup.cfg
+-rw-r--r--   0 zhiweizhang   (501) staff       (20)     1076 2022-11-29 09:14:27.000000 lbg-1.2.9/setup.py
+drwxr-xr-x   0 zhiweizhang   (501) staff       (20)        0 2022-12-01 03:55:29.358310 lbg-1.2.9/tiefblue/
+-rw-r--r--   0 zhiweizhang   (501) staff       (20)       64 2022-11-29 10:30:01.000000 lbg-1.2.9/tiefblue/__init__.py
+-rw-r--r--   0 zhiweizhang   (501) staff       (20)     9260 2022-11-29 09:13:00.000000 lbg-1.2.9/tiefblue/client.py
```

### Comparing `lbg-1.2.8/LICENSE` & `lbg-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lbg-1.2.8/README.md` & `lbg-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `lbg-1.2.8/lbg.egg-info/SOURCES.txt` & `lbg-1.2.9/lbg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lbg-1.2.8/lbgcli/config/config.py` & `lbg-1.2.9/lbgcli/config/config.py`

 * *Files identical despite different names*

### Comparing `lbg-1.2.8/lbgcli/const.py` & `lbg-1.2.9/lbgcli/const.py`

 * *Files identical despite different names*

### Comparing `lbg-1.2.8/lbgcli/history/history.py` & `lbg-1.2.9/lbgcli/history/history.py`

 * *Files identical despite different names*

### Comparing `lbg-1.2.8/lbgcli/image/image.py` & `lbg-1.2.9/lbgcli/image/image.py`

 * *Files identical despite different names*

### Comparing `lbg-1.2.8/lbgcli/job/_jcc.py` & `lbg-1.2.9/lbgcli/job/_jcc.py`

 * *Files identical despite different names*

### Comparing `lbg-1.2.8/lbgcli/job/job.py` & `lbg-1.2.9/lbgcli/job/job.py`

 * *Files 2% similar despite different names*

```diff
@@ -221,15 +221,15 @@
                     #     log = f"type: {t}   modify_date: {time}\n{nl.join(logs)}"
             except Exception as e:
                 traceback.print_exc()
             self.cli.print(log)
 
     def load_submit(self):
         parser_tm = self.sub_parser.add_parser('submit', help='submit job')
-        parser_tm.set_defaults(func=lambda args: self.func_submit(args))
+        parser_tm.set_defaults(func=lambda args: self.func_submit_v2(args))
         parser_tm.add_argument('-i', '--file', action='store', help='predefined file')
         parser_tm.add_argument('-p', '--input', action='store', nargs='*', help='input file location')
         parser_tm.add_argument('-jt', '--job_type', action='store', help='indicate/container')
         parser_tm.add_argument('-jgid', '--job_group_id', action='store', type=int, help='job group id')
         parser_tm.add_argument('-pjid', '--project_id', action='store', type=int,
                                help='project id, will overwrite default')
         parser_tm.add_argument('-n', '--job_name', action='store', help='name')
@@ -311,14 +311,16 @@
             data['out_files'] = args.out_files
         if args.platform:
             data['platform'] = args.platform
         if args.region:
             data['region'] = args.region
         if args.on_demand:
             data['on_demand'] = args.on_demand
+        if data.get('image_address') and not data.get('image_name'):
+            data['image_name'] = data.get('image_address')
         if args.result or 'result' in data:
             result_path = args.result if args.result else data['result']
             ep = os.path.expanduser(result_path)
             p = Path(ep).absolute().resolve()
             p = p.joinpath(str(uuid.uuid4()) + "_temp.zip")
             data['download_path'] = str(p.absolute().resolve())
             retry = 7
@@ -470,14 +472,16 @@
             data['out_files'] = args.out_files
         if args.platform:
             data['platform'] = args.platform
         if args.region:
             data['region'] = args.region
         if args.on_demand:
             data['on_demand'] = args.on_demand
+        if data.get('image_address') and not data.get('image_name'):
+            data['image_name'] = data.get('image_address')
         if args.result or 'result' in data:
             result_path = args.result if args.result else data['result']
             ep = os.path.expanduser(result_path)
             p = Path(ep).absolute().resolve()
             p = p.joinpath(str(uuid.uuid4()) + "_temp.zip")
             data['download_path'] = str(p.absolute().resolve())
             retry = 7
```

### Comparing `lbg-1.2.8/lbgcli/job_group/job_group.py` & `lbg-1.2.9/lbgcli/job_group/job_group.py`

 * *Files identical despite different names*

### Comparing `lbg-1.2.8/lbgcli/machine/machine.py` & `lbg-1.2.9/lbgcli/machine/machine.py`

 * *Files identical despite different names*

### Comparing `lbg-1.2.8/lbgcli/main_entry.py` & `lbg-1.2.9/lbgcli/main_entry.py`

 * *Files identical despite different names*

### Comparing `lbg-1.2.8/lbgcli/module_impl.py` & `lbg-1.2.9/lbgcli/module_impl.py`

 * *Files identical despite different names*

### Comparing `lbg-1.2.8/lbgcli/node/node.py` & `lbg-1.2.9/lbgcli/node/node.py`

 * *Files identical despite different names*

### Comparing `lbg-1.2.8/lbgcli/program/program.py` & `lbg-1.2.9/lbgcli/program/program.py`

 * *Files identical despite different names*

### Comparing `lbg-1.2.8/lbgcli/util.py` & `lbg-1.2.9/lbgcli/util.py`

 * *Files identical despite different names*

### Comparing `lbg-1.2.8/lbgcore/client.py` & `lbg-1.2.9/lbgcore/client.py`

 * *Files identical despite different names*

### Comparing `lbg-1.2.8/lbgcore/image.py` & `lbg-1.2.9/lbgcore/image.py`

 * *Files identical despite different names*

### Comparing `lbg-1.2.8/lbgcore/job.py` & `lbg-1.2.9/lbgcore/job.py`

 * *Files identical despite different names*

### Comparing `lbg-1.2.8/lbgcore/jobgroup.py` & `lbg-1.2.9/lbgcore/jobgroup.py`

 * *Files identical despite different names*

### Comparing `lbg-1.2.8/lbgcore/machine.py` & `lbg-1.2.9/lbgcore/machine.py`

 * *Files identical despite different names*

### Comparing `lbg-1.2.8/lbgcore/program.py` & `lbg-1.2.9/lbgcore/program.py`

 * *Files identical despite different names*

### Comparing `lbg-1.2.8/lbgcore/server.py` & `lbg-1.2.9/lbgcore/server.py`

 * *Files identical despite different names*

### Comparing `lbg-1.2.8/lebesgue_sdk/cmd.py` & `lbg-1.2.9/lebesgue_sdk/cmd.py`

 * *Files identical despite different names*

### Comparing `lbg-1.2.8/lebesgue_sdk/lebesgue_sdk.py` & `lbg-1.2.9/lebesgue_sdk/lebesgue_sdk.py`

 * *Files identical despite different names*

### Comparing `lbg-1.2.8/setup.py` & `lbg-1.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `lbg-1.2.8/tiefblue/client.py` & `lbg-1.2.9/tiefblue/client.py`

 * *Files identical despite different names*

