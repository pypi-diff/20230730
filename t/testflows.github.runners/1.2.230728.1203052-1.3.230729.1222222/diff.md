# Comparing `tmp/testflows.github.runners-1.2.230728.1203052.tar.gz` & `tmp/testflows.github.runners-1.3.230729.1222222.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testflows.github.runners-1.2.230728.1203052.tar", last modified: Fri Jul 28 20:30:52 2023, max compression
+gzip compressed data, was "testflows.github.runners-1.3.230729.1222222.tar", last modified: Sat Jul 29 22:22:22 2023, max compression
```

## Comparing `testflows.github.runners-1.2.230728.1203052.tar` & `testflows.github.runners-1.3.230729.1222222.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 20:30:52.474443 testflows.github.runners-1.2.230728.1203052/
--rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-24 01:44:49.000000 testflows.github.runners-1.2.230728.1203052/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)    39717 2023-07-28 20:30:52.474443 testflows.github.runners-1.2.230728.1203052/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    39125 2023-07-28 20:30:27.000000 testflows.github.runners-1.2.230728.1203052/README.rst
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-28 20:30:52.474443 testflows.github.runners-1.2.230728.1203052/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-28 20:30:52.000000 testflows.github.runners-1.2.230728.1203052/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 20:30:52.470443 testflows.github.runners-1.2.230728.1203052/testflows/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 20:30:52.470443 testflows.github.runners-1.2.230728.1203052/testflows/github/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 20:30:52.470443 testflows.github.runners-1.2.230728.1203052/testflows/github/runners/
--rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-28 20:30:52.000000 testflows.github.runners-1.2.230728.1203052/testflows/github/runners/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1615 2023-07-28 12:15:47.000000 testflows.github.runners-1.2.230728.1203052/testflows/github/runners/actions.py
--rw-rw-r--   0 user      (1000) user      (1000)     3011 2023-07-27 02:43:16.000000 testflows.github.runners-1.2.230728.1203052/testflows/github/runners/args.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 20:30:52.470443 testflows.github.runners-1.2.230728.1203052/testflows/github/runners/bin/
--rwxrwxr-x   0 user      (1000) user      (1000)    22684 2023-07-28 12:17:00.000000 testflows.github.runners-1.2.230728.1203052/testflows/github/runners/bin/github-runners
--rw-rw-r--   0 user      (1000) user      (1000)    12755 2023-07-28 15:03:49.000000 testflows.github.runners-1.2.230728.1203052/testflows/github/runners/cloud.py
--rw-rw-r--   0 user      (1000) user      (1000)     1463 2023-07-28 14:48:45.000000 testflows.github.runners-1.2.230728.1203052/testflows/github/runners/config.py
--rw-rw-r--   0 user      (1000) user      (1000)      726 2023-07-28 12:15:58.000000 testflows.github.runners-1.2.230728.1203052/testflows/github/runners/logger.py
--rw-rw-r--   0 user      (1000) user      (1000)     1894 2023-07-26 15:00:13.000000 testflows.github.runners-1.2.230728.1203052/testflows/github/runners/request.py
--rw-rw-r--   0 user      (1000) user      (1000)     9760 2023-07-28 16:35:01.000000 testflows.github.runners-1.2.230728.1203052/testflows/github/runners/scale_down.py
--rw-rw-r--   0 user      (1000) user      (1000)    12069 2023-07-28 19:51:52.000000 testflows.github.runners-1.2.230728.1203052/testflows/github/runners/scale_up.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 20:30:52.470443 testflows.github.runners-1.2.230728.1203052/testflows/github/runners/scripts/
--rw-rw-r--   0 user      (1000) user      (1000)     1061 2023-07-26 23:10:10.000000 testflows.github.runners-1.2.230728.1203052/testflows/github/runners/scripts/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 20:30:52.474443 testflows.github.runners-1.2.230728.1203052/testflows/github/runners/scripts/deploy/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-24 22:39:23.000000 testflows.github.runners-1.2.230728.1203052/testflows/github/runners/scripts/deploy/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      519 2023-07-27 00:03:37.000000 testflows.github.runners-1.2.230728.1203052/testflows/github/runners/scripts/deploy/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      260 2023-07-27 02:16:34.000000 testflows.github.runners-1.2.230728.1203052/testflows/github/runners/scripts/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-26 20:22:42.000000 testflows.github.runners-1.2.230728.1203052/testflows/github/runners/scripts/startup_arm64.sh
--rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-26 20:23:06.000000 testflows.github.runners-1.2.230728.1203052/testflows/github/runners/scripts/startup_x64.sh
--rw-rw-r--   0 user      (1000) user      (1000)     2522 2023-07-27 15:03:46.000000 testflows.github.runners-1.2.230728.1203052/testflows/github/runners/server.py
--rw-rw-r--   0 user      (1000) user      (1000)     4921 2023-07-26 22:31:47.000000 testflows.github.runners-1.2.230728.1203052/testflows/github/runners/service.py
--rw-rw-r--   0 user      (1000) user      (1000)     1483 2023-07-26 15:50:50.000000 testflows.github.runners-1.2.230728.1203052/testflows/github/runners/shell.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 20:30:52.470443 testflows.github.runners-1.2.230728.1203052/testflows.github.runners.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    39717 2023-07-28 20:30:52.000000 testflows.github.runners-1.2.230728.1203052/testflows.github.runners.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1070 2023-07-28 20:30:52.000000 testflows.github.runners-1.2.230728.1203052/testflows.github.runners.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-28 20:30:52.000000 testflows.github.runners-1.2.230728.1203052/testflows.github.runners.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 17:57:22.000000 testflows.github.runners-1.2.230728.1203052/testflows.github.runners.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-28 20:30:52.000000 testflows.github.runners-1.2.230728.1203052/testflows.github.runners.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-28 20:30:52.000000 testflows.github.runners-1.2.230728.1203052/testflows.github.runners.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-29 22:22:22.906553 testflows.github.runners-1.3.230729.1222222/
+-rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230729.1222222/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)    46741 2023-07-29 22:22:22.906553 testflows.github.runners-1.3.230729.1222222/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    46149 2023-07-29 22:19:05.000000 testflows.github.runners-1.3.230729.1222222/README.rst
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-29 22:22:22.906553 testflows.github.runners-1.3.230729.1222222/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-29 22:22:22.000000 testflows.github.runners-1.3.230729.1222222/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-29 22:22:22.902553 testflows.github.runners-1.3.230729.1222222/testflows/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-29 22:22:22.902553 testflows.github.runners-1.3.230729.1222222/testflows/github/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-29 22:22:22.906553 testflows.github.runners-1.3.230729.1222222/testflows/github/runners/
+-rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-29 22:22:22.000000 testflows.github.runners-1.3.230729.1222222/testflows/github/runners/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1615 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230729.1222222/testflows/github/runners/actions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2491 2023-07-29 22:10:17.000000 testflows.github.runners-1.3.230729.1222222/testflows/github/runners/args.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-29 22:22:22.906553 testflows.github.runners-1.3.230729.1222222/testflows/github/runners/bin/
+-rwxrwxr-x   0 user      (1000) user      (1000)    22712 2023-07-29 21:42:45.000000 testflows.github.runners-1.3.230729.1222222/testflows/github/runners/bin/github-runners
+-rw-rw-r--   0 user      (1000) user      (1000)    13607 2023-07-29 20:55:15.000000 testflows.github.runners-1.3.230729.1222222/testflows/github/runners/cloud.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3995 2023-07-29 22:12:50.000000 testflows.github.runners-1.3.230729.1222222/testflows/github/runners/config.py
+-rw-rw-r--   0 user      (1000) user      (1000)      726 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230729.1222222/testflows/github/runners/logger.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1894 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230729.1222222/testflows/github/runners/request.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10527 2023-07-29 20:55:15.000000 testflows.github.runners-1.3.230729.1222222/testflows/github/runners/scale_down.py
+-rw-rw-r--   0 user      (1000) user      (1000)    16705 2023-07-29 20:55:15.000000 testflows.github.runners-1.3.230729.1222222/testflows/github/runners/scale_up.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-29 22:22:22.906553 testflows.github.runners-1.3.230729.1222222/testflows/github/runners/scripts/
+-rw-rw-r--   0 user      (1000) user      (1000)     1061 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230729.1222222/testflows/github/runners/scripts/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-29 22:22:22.906553 testflows.github.runners-1.3.230729.1222222/testflows/github/runners/scripts/deploy/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230729.1222222/testflows/github/runners/scripts/deploy/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      519 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230729.1222222/testflows/github/runners/scripts/deploy/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      260 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230729.1222222/testflows/github/runners/scripts/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230729.1222222/testflows/github/runners/scripts/startup_arm64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230729.1222222/testflows/github/runners/scripts/startup_x64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     2522 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230729.1222222/testflows/github/runners/server.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5122 2023-07-29 20:55:15.000000 testflows.github.runners-1.3.230729.1222222/testflows/github/runners/service.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1483 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230729.1222222/testflows/github/runners/shell.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-29 22:22:22.902553 testflows.github.runners-1.3.230729.1222222/testflows.github.runners.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    46741 2023-07-29 22:22:22.000000 testflows.github.runners-1.3.230729.1222222/testflows.github.runners.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1070 2023-07-29 22:22:22.000000 testflows.github.runners-1.3.230729.1222222/testflows.github.runners.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-29 22:22:22.000000 testflows.github.runners-1.3.230729.1222222/testflows.github.runners.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-29 01:22:42.000000 testflows.github.runners-1.3.230729.1222222/testflows.github.runners.egg-info/not-zip-safe
+-rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-29 22:22:22.000000 testflows.github.runners-1.3.230729.1222222/testflows.github.runners.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-29 22:22:22.000000 testflows.github.runners-1.3.230729.1222222/testflows.github.runners.egg-info/top_level.txt
```

### Comparing `testflows.github.runners-1.2.230728.1203052/LICENSE` & `testflows.github.runners-1.3.230729.1222222/LICENSE`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1203052/PKG-INFO` & `testflows.github.runners-1.3.230729.1222222/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.2.230728.1203052
+Version: 1.3.230729.1222222
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -28,14 +28,16 @@
 :License:
    `Apache-2.0 <https://github.com/testflows/TestFlows-GitHub-Runners/blob/main/LICENSE>`_
 
 ======================================================
 Autoscaling GitHub Actions Runners Using Hetzner Cloud
 ======================================================
 
+A simple alternative to Github's `Recommended autoscaling solutions <https://docs.github.com/en/actions/hosting-your-own-runners/managing-self-hosted-runners/autoscaling-with-self-hosted-runners#recommended-autoscaling-solutions>`_.
+
 The **github-runners** service program starts and monitors queued up jobs for GitHub Actions workflows.
 When a new job is queued up, it creates a new Hetzner Cloud server instance
 that provides an ephemeral GitHub Actions runner. Each server instance is automatically
 powered off when job completes and then powered off servers are
 automatically deleted. Both **x64** and **arm64** runners are supported.
 
 :❗Warning:
@@ -47,30 +49,33 @@
 to avoid any cleanup. Server instances are not shared between any jobs.
 
 :✋ Note:
    Currently Hetzner Cloud server instances are billed on hourly basis. So a job that takes 1 min will be billed
    the same way as for a job that takes 59 minutes. Therefore, the minimal cost
    for any job is the cost of the server for 1 hour plus the cost for one public IPv4 address.
 
+----
 
-.. contents:: Read more about:
-   :backlinks: top
-   :depth: 4
+:🔍 Tip:
+   You can easily navigate this documentation page by clicking on any title to jump to the `Table of Contents`_.
+   Try it out, and remember, if you get lost just click any title!
 
 ----
 
 --------
 Features
 --------
 
-* very cost efficient on-demand runners using Hetzner Cloud
-* supports both x64 and ARM64 runners
+* cost efficient on-demand runners using `Hetzner Cloud <https://www.hetzner.com/cloud>`_
+* simple configuration, no Webhooks, no need for AWS lambdas, and no need to setup any GitHub application
 * supports specifying custom runner server types, images, and locations using job labels
-* simple configuration
-* self-contained and it can deploy, redeploy, and manage itself on a cloud instance
+* self-contained program that you can use to deploy, redeploy, and manage the service on a cloud instance
+* supports both x64 and ARM64 runners
+* supports auto-replenishable fixed standby runner pools for jobs to be picked up immediately
+* simpler alternative to what GitHub lists in `Recommended autoscaling solutions <https://docs.github.com/en/actions/hosting-your-own-runners/managing-self-hosted-runners/autoscaling-with-self-hosted-runners#recommended-autoscaling-solutions>`_
 
 ----
 
 -----------
 Limitations
 -----------
 
@@ -78,17 +83,23 @@
 
   However, you can run individual services for each repository using different Hetzner Cloud projects.
 
 * *Unique Hetzner Cloud project must be used for each repository*
 
   However, unique projects allow to easily keep track of runner costs per repository.
 
-* *Idle runner pool is not supported*
+----
 
-  Given that runner servers are created for each job, currently, idle runner pool is not supported.. 
+-------------
+Prerequisites
+-------------
+
+* Python >= 3.7
+* `Hetzner Cloud <https://www.hetzner.com/cloud>`_ account
+* GitHub API token with admin privileges to manage self-hosted runners
 
 ----
 
 ------------
 Installation
 ------------
 
@@ -308,14 +319,199 @@
 :command:
    .. code-block:: bash
 
       github-runners --setup-script ./custom_setup.sh
 
 ----
 
+--------------------------
+Specifying Standby Runners
+--------------------------
+
+You can define standby runner groups to be always ready to pick your jobs using a custom configuration file.
+
+:✋ Note:
+   Standby runner groups can only be defined using a configuration file.
+   See `Using Configuration File`_ for more details.
+
+Standby runners are always active and allow the jobs to be picked up immediately.
+
+More than one standby runner group can be specified in the **standby_runners**. Each group is defined using the **standby_runner** object
+that has *labels*, *count*, and *replenish_immediately* attributes.
+
+:schema:
+   * **standby_runners: list[standby_runner]**
+      * **labels: list[str]**
+      * **count: count**
+      * **replenish_immediately: bool**
+
+where
+
+* **labels** specifies a list of labels with which standby runners in this group should be created
+* **count** specifies how many runners should be created for the group
+* **replenish_immediately** specifies if the sandby runners should be replenished as soon as any become busy after picking up a job
+
+For example,
+
+:config.py:
+   .. code-block:: python3
+
+      from testflows.github.runners.config import *
+
+      config = Config(
+         standby_runners=[
+            standby_runner(
+                  labels=["type-cx21"],
+                  count=2,
+                  replenish_immediately=True,
+            )
+         ],
+      )
+
+----
+
+-------------------------------
+Specifying Logger Configuration
+-------------------------------
+
+You can specify custom logger configuration using a configuration file.
+
+:✋ Note:
+   Custom logger configuration can only be specified using a configuration file.
+   See `Using Configuration File`_ for more details.
+
+The logger configuration is specified by passing a dictionary as the value to the **logger_config** attribute of the `Config class`_.
+See for information about the logger configuration dictionary, see `Configuration dictionary schema <https://docs.python.org/3/library/logging.config.html#logging-config-dictschema>`_ in Python documentation.
+
+For example,
+
+:config.py:
+   .. code-block:: python3
+
+      from testflows.github.runners.config import *
+
+      config = Config(
+         logger_config = {
+             "version": 1,
+             "disable_existing_loggers": False,
+             "formatters": {
+                 "standard": {
+                     "format": "%(asctime)s %(levelname)8s %(threadName)16s %(funcName)15s %(message)s",
+                     "datefmt": "%m/%d/%Y %I:%M:%S %p",
+                 },
+             },
+             "handlers": {
+                 "default": {
+                     "level": "INFO",
+                     "formatter": "standard",
+                     "class": "logging.StreamHandler",
+                     "stream": "ext://sys.stdout",
+                 },
+             },
+             "loggers": {
+                 "testflows.github.runners": {"level": "INFO", "handlers": ["default"]},
+             },
+         }
+     )
+
+------------------------
+Using Configuration File
+------------------------
+
+Instead of passing configuration options using command line arguments, you can use
+configuration file. The configuration file is Python file that must define the **config**
+object of the `Config class`_.
+
+:✋ Note:
+   When you mix command line options and custom configuration file,
+   explicit command line options take precedence over the values that are defined
+   for the same parameters in the configuration file.
+
+:✨ Why:
+   Defining configuration file in Python instead of YAML or something else
+   has a few advantages. For example, you can edit it with
+   any Python IDE that provides a convenience of autocompletion and hints.
+
+For example,
+
+:config.py:
+
+   Simple configuration file. You can find a complete example in `examples/config.py <https://github.com/testflows/TestFlows-GitHub-Runners/blob/main/examples/config.py>`_.
+
+   .. code-block:: python3
+
+      from testflows.github.runners.config import *
+
+      config = Config(
+         github_token=os.getenv("GITHUB_TOKEN"),
+         github_repository=os.getenv("GITHUB_REPOSITORY"),
+         hetzner_token=os.getenv("HETZNER_TOKEN"),
+         default_server_type=server_type("cx11"),
+         cloud=cloud(server_name="my-github-runners-service"),
+         standby_runners=[
+            standby_runner(
+                  labels=["type-cx21"],
+                  count=2,
+                  replenish_immediately=True,
+            )
+         ],
+      )
+
+You can sanity check your configuration file by executing it directly:
+
+.. code-block:: bash
+
+   python3 config.py
+
+You can pass your custom configuration file using the *-c path, --config path** command line option.
+
+.. code-block:: bash
+
+   github-runners -c config.py
+
+Configuration Schema
+=====================
+
+The `Config class`_ has the following schema:
+
+:schema:
+   * **github_token: str**
+   * **github_repository: str**
+   * **hetzner_token: str**
+   * **ssh_key: str**
+   * **max_runners**
+   * **default_image: image**
+   * **default_server_type: server_type**
+   * **default_location: location**
+   * **workers: count**
+   * **setup_script: path**
+   * **startup_x64_script: path**
+   * **startup_arm64_script: path**
+   * **max_powered_off_time: count**
+   * **max_unused_runner_time: count**
+   * **max_runner_registration_time: count**
+   * **max_server_ready_time: count**
+   * **scale_up_interval: count**
+   * **scale_down_interval: count**
+   * **debug: bool**
+   * **logger_config: dict**
+   * **cloud: cloud**
+      * **server_name: str**
+      * **deploy: deploy**
+         * **server_type: server_type**
+         * **image: image**
+         * **location: location**
+         * **setup_script: path**
+   * **standby_runners: list[standby_runner]**
+      * **labels: list[str]**
+      * **count: count**
+      * **replenish_immediately: bool**
+
+----
+
 -------
 SSH Key
 -------
 
 All server instances that are created are accessed via SSH using the **ssh** utility and therefore you must provide a valid SSH key
 using the **--ssh-key** option. If the **--ssh-key** option is no specified, then the *~/.ssh/id_rsa.pub* default key path will be used.
 
@@ -388,15 +584,15 @@
       User=1000
       Group=1000
       Type=simple
       Restart=always
       Environment=GITHUB_TOKEN=ghp_...
       Environment=GITHUB_REPOSITORY=testflows/github-runners
       Environment=HETZNER_TOKEN=GJ..
-      ExecStart=/home/user/.local/lib/python3.10/site-packages/testflows/github/runners/bin/github-runners --workers 10 --max-powered-off-time 20 --max-idle-runner-time 120 --max-runner-registration-time 60 --scale-up-interval 10 --scale-down-interval 10
+      ExecStart=/home/user/.local/lib/python3.10/site-packages/testflows/github/runners/bin/github-runners --workers 10 --max-powered-off-time 20 --max-unused-runner-time 120 --max-runner-registration-time 60 --scale-up-interval 10 --scale-down-interval 10
       [Install]
       WantedBy=multi-user.target
 
 ----
 
 Modifying Program Options
 =========================
@@ -431,15 +627,15 @@
            Loaded: loaded (/etc/systemd/system/github-runners.service; enabled; vendor preset: enabled)
            Active: active (running) since Mon 2023-07-24 14:38:33 EDT; 1h 31min ago
          Main PID: 66188 (python3)
             Tasks: 3 (limit: 37566)
            Memory: 28.8M
               CPU: 8.274s
            CGroup: /system.slice/github-runners.service
-                   └─66188 python3 /usr/local/bin/github-runners --workers 10 --max-powered-off-time 20 --max-idle-runner-time 120 --max->
+                   └─66188 python3 /usr/local/bin/github-runners --workers 10 --max-powered-off-time 20 --max-unused-runner-time 120 --max->
 
       Jul 24 14:38:33 user-node systemd[1]: Started Autoscaling GitHub Actions Runners.
       Jul 24 14:38:33 user-node github-runners[66188]: 07/24/2023 02:38:33 PM   INFO MainThread            main 🍀 Logging in to Hetzner >
       Jul 24 14:38:33 user-node github-runners[66188]: 07/24/2023 02:38:33 PM   INFO MainThread            main 🍀 Logging in to GitHub
       Jul 24 14:38:33 user-node github-runners[66188]: 07/24/2023 02:38:33 PM   INFO MainThread            main 🍀 Getting repository vza>
       Jul 24 14:38:33 user-node github-runners[66188]: 07/24/2023 02:38:33 PM   INFO MainThread            main 🍀 Creating scale up serv>
       Jul 24 14:38:33 user-node github-runners[66188]: 07/24/2023 02:38:33 PM   INFO MainThread            main 🍀 Creating scale down se>
@@ -845,16 +1041,16 @@
 For each such job, a corresponding Hetzner Cloud server instance is created with the following name:
 
 ::
 
    github-runner-{job.run_id}-{job.id}
 
 The server is configured using default **setup** and **startup** scripts. The runner name is set
-to be the same as the server name so that servers can be deleted for any idle runner that for some reason
-does not pick up a job for which it was created within the **max-idle-runner-time** period.
+to be the same as the server name so that servers can be deleted for any unused runner that for some reason
+does not pick up a job for which it was created within the **max-unused-runner-time** period.
 
 :Note:
    Given that the server name is fixed and specific for each *job.run_id, job.id* tuple, if multiple `github-runners` are running in parallel then
    only 1 server will be created for a given `job` and any other attempts to create a server with the same name will be rejected
    by the Hetzner Cloud.
 
 Also,
@@ -1000,21 +1196,21 @@
 
 The program scales down runners by first cleaning up powered off servers. The scale down service relies on the fact
 that the `startup <#the-start-up-script>`_ script starts an ephemeral runner which will pick up only 1 job and then will power itself off after the job is complete.
 
 The powered off servers are deleted after the **max-powered-off-time** interval which
 can be specified using the **--max-powered-off-time** option which by default is set to *20* sec.
 
-Idle Runners
-============
+Unused Runners
+==============
 
-The scale down service also monitors all the runners that have **idle** status and tries to delete any servers associated with such
-runners if the runner is **idle** for more than the **max-idle-runner-time** period. This is needed in case a runner never gets a job
+The scale down service also monitors all the runners that have **unused** status and tries to delete any servers associated with such
+runners if the runner is **unused** for more than the **max-unused-runner-time** period. This is needed in case a runner never gets a job
 assigned to it and the server will stay in the power on state. This cycle relies on the fact that the runner's name
-is the same as server's name. The **max-idle-runner-time** can be specified using the **--max-idle-runner-time** option which by default
+is the same as server's name. The **max-unused-runner-time** can be specified using the **--max-unused-runner-time** option which by default
 is set to *120* sec.
 
 Zombie Servers
 ==============
 
 The scale down service will delete any zombie servers. A zombie server is defined as as any server that fails to register its runner within
 the **max-runner-registration-time**. The **max-runner-registration-time** can be specified using the **--max-runner-registration-time** option
@@ -1038,15 +1234,15 @@
 :The *./run.sh* Command Fails:
    The server will be powered off by the **startup** script and will be deleted by the scale down service.
 
 :Creating Server For Queued Job Fails:
    If creation of the server fails for some reason then the scale up service will retry the operation in the next interval as the job's status will remain **queued**.
 
 :Runner Never Gets a Job Assigned:
-   If the runner never gets a job assigned, then the scale down service will remove the runner and delete its server after the **max-idle-runner-time** period.
+   If the runner never gets a job assigned, then the scale down service will remove the runner and delete its server after the **max-unused-runner-time** period.
 
 :Runner Created With a Mismatched Labels:
    The behavior will be the same as for the **Runner Never Gets a Job Assigned** case above.
 
 ----
 
 ---------------
@@ -1060,14 +1256,17 @@
 
 * **-v, --version**
   show program's version number and exit
 
 * **--license**
   show program's license and exit
 
+* **-c path, --config path**
+  program configuration file
+
 * **--github-token GITHUB_TOKEN**
   GitHub token, default: *$GITHUB_TOKEN* environment variable
 
 * **--github-repository GITHUB_REPOSITORY**
   GitHub repository, default: *$GITHUB_REPOSITORY* environment variable
 
 * **--hetzner-token HETZNER_TOKEN**
@@ -1089,31 +1288,28 @@
 
 * **-m count, --max-runners count**
   maximum number of active runners, default: *10*
 
 * **-w count, --workers count**
   number of concurrent workers, default: *10*
 
-* **--logger-config path**
-  custom logger configuration file
-
 * **--setup-script path**
   path to custom server setup script
 
 * **--startup-x64-script path**
   path to custom server startup script
 
 * **--startup-arm64-script path**
   path to custom ARM64 server startup script
 
 * **--max-powered-off-time sec**
   maximum time after which a powered off server is deleted, default: *60* sec
 
-* **--max-idle-runner-time sec**
-  maximum time after which an idle runner is removed and its server deleted, default: *120* sec
+* **--max-unused-runner-time sec**
+  maximum time after which an unused runner is removed and its server deleted, default: *120* sec
 
 * **--max-runner-registration-time**
   maximum time after which the server will be deleted if its runner is not registered with GitHub, default: *120* sec
 
 * **--max-server-ready-time sec**
   maximum time to wait for the server to be in the running state, default: *120* sec
 
@@ -1225,7 +1421,17 @@
           follow logs journal, default: *False*
 
       * **start**
         start service
 
       * **stop**
         stop service
+
+-----------------
+Table of Contents
+-----------------
+
+.. contents:: Index:
+   :backlinks: top
+   :depth: 4
+
+.. _Config class: https://github.com/testflows/TestFlows-GitHub-Runners/blob/main/testflows/github/runners/config.py#L45
```

### Comparing `testflows.github.runners-1.2.230728.1203052/README.rst` & `testflows.github.runners-1.3.230729.1222222/testflows.github.runners.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: testflows.github.runners
+Version: 1.3.230729.1222222
+Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
+Home-page: https://github.com/testflows/github-runners
+Author: Vitaliy Zakaznikov
+Author-email: vzakaznikov@testflows.com
+License: Apache-2.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: POSIX :: Linux
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
+Provides-Extra: dev
+License-File: LICENSE
+
 .. image:: https://raw.githubusercontent.com/testflows/TestFlows-ArtWork/master/images/logo.png
    :width: 20%
    :align: left
    :target: https://testflows.com
    :alt: TestFlows Open-source Testing Framework
 
 ----
@@ -11,14 +28,16 @@
 :License:
    `Apache-2.0 <https://github.com/testflows/TestFlows-GitHub-Runners/blob/main/LICENSE>`_
 
 ======================================================
 Autoscaling GitHub Actions Runners Using Hetzner Cloud
 ======================================================
 
+A simple alternative to Github's `Recommended autoscaling solutions <https://docs.github.com/en/actions/hosting-your-own-runners/managing-self-hosted-runners/autoscaling-with-self-hosted-runners#recommended-autoscaling-solutions>`_.
+
 The **github-runners** service program starts and monitors queued up jobs for GitHub Actions workflows.
 When a new job is queued up, it creates a new Hetzner Cloud server instance
 that provides an ephemeral GitHub Actions runner. Each server instance is automatically
 powered off when job completes and then powered off servers are
 automatically deleted. Both **x64** and **arm64** runners are supported.
 
 :❗Warning:
@@ -30,30 +49,33 @@
 to avoid any cleanup. Server instances are not shared between any jobs.
 
 :✋ Note:
    Currently Hetzner Cloud server instances are billed on hourly basis. So a job that takes 1 min will be billed
    the same way as for a job that takes 59 minutes. Therefore, the minimal cost
    for any job is the cost of the server for 1 hour plus the cost for one public IPv4 address.
 
+----
 
-.. contents:: Read more about:
-   :backlinks: top
-   :depth: 4
+:🔍 Tip:
+   You can easily navigate this documentation page by clicking on any title to jump to the `Table of Contents`_.
+   Try it out, and remember, if you get lost just click any title!
 
 ----
 
 --------
 Features
 --------
 
-* very cost efficient on-demand runners using Hetzner Cloud
-* supports both x64 and ARM64 runners
+* cost efficient on-demand runners using `Hetzner Cloud <https://www.hetzner.com/cloud>`_
+* simple configuration, no Webhooks, no need for AWS lambdas, and no need to setup any GitHub application
 * supports specifying custom runner server types, images, and locations using job labels
-* simple configuration
-* self-contained and it can deploy, redeploy, and manage itself on a cloud instance
+* self-contained program that you can use to deploy, redeploy, and manage the service on a cloud instance
+* supports both x64 and ARM64 runners
+* supports auto-replenishable fixed standby runner pools for jobs to be picked up immediately
+* simpler alternative to what GitHub lists in `Recommended autoscaling solutions <https://docs.github.com/en/actions/hosting-your-own-runners/managing-self-hosted-runners/autoscaling-with-self-hosted-runners#recommended-autoscaling-solutions>`_
 
 ----
 
 -----------
 Limitations
 -----------
 
@@ -61,17 +83,23 @@
 
   However, you can run individual services for each repository using different Hetzner Cloud projects.
 
 * *Unique Hetzner Cloud project must be used for each repository*
 
   However, unique projects allow to easily keep track of runner costs per repository.
 
-* *Idle runner pool is not supported*
+----
 
-  Given that runner servers are created for each job, currently, idle runner pool is not supported.. 
+-------------
+Prerequisites
+-------------
+
+* Python >= 3.7
+* `Hetzner Cloud <https://www.hetzner.com/cloud>`_ account
+* GitHub API token with admin privileges to manage self-hosted runners
 
 ----
 
 ------------
 Installation
 ------------
 
@@ -291,14 +319,199 @@
 :command:
    .. code-block:: bash
 
       github-runners --setup-script ./custom_setup.sh
 
 ----
 
+--------------------------
+Specifying Standby Runners
+--------------------------
+
+You can define standby runner groups to be always ready to pick your jobs using a custom configuration file.
+
+:✋ Note:
+   Standby runner groups can only be defined using a configuration file.
+   See `Using Configuration File`_ for more details.
+
+Standby runners are always active and allow the jobs to be picked up immediately.
+
+More than one standby runner group can be specified in the **standby_runners**. Each group is defined using the **standby_runner** object
+that has *labels*, *count*, and *replenish_immediately* attributes.
+
+:schema:
+   * **standby_runners: list[standby_runner]**
+      * **labels: list[str]**
+      * **count: count**
+      * **replenish_immediately: bool**
+
+where
+
+* **labels** specifies a list of labels with which standby runners in this group should be created
+* **count** specifies how many runners should be created for the group
+* **replenish_immediately** specifies if the sandby runners should be replenished as soon as any become busy after picking up a job
+
+For example,
+
+:config.py:
+   .. code-block:: python3
+
+      from testflows.github.runners.config import *
+
+      config = Config(
+         standby_runners=[
+            standby_runner(
+                  labels=["type-cx21"],
+                  count=2,
+                  replenish_immediately=True,
+            )
+         ],
+      )
+
+----
+
+-------------------------------
+Specifying Logger Configuration
+-------------------------------
+
+You can specify custom logger configuration using a configuration file.
+
+:✋ Note:
+   Custom logger configuration can only be specified using a configuration file.
+   See `Using Configuration File`_ for more details.
+
+The logger configuration is specified by passing a dictionary as the value to the **logger_config** attribute of the `Config class`_.
+See for information about the logger configuration dictionary, see `Configuration dictionary schema <https://docs.python.org/3/library/logging.config.html#logging-config-dictschema>`_ in Python documentation.
+
+For example,
+
+:config.py:
+   .. code-block:: python3
+
+      from testflows.github.runners.config import *
+
+      config = Config(
+         logger_config = {
+             "version": 1,
+             "disable_existing_loggers": False,
+             "formatters": {
+                 "standard": {
+                     "format": "%(asctime)s %(levelname)8s %(threadName)16s %(funcName)15s %(message)s",
+                     "datefmt": "%m/%d/%Y %I:%M:%S %p",
+                 },
+             },
+             "handlers": {
+                 "default": {
+                     "level": "INFO",
+                     "formatter": "standard",
+                     "class": "logging.StreamHandler",
+                     "stream": "ext://sys.stdout",
+                 },
+             },
+             "loggers": {
+                 "testflows.github.runners": {"level": "INFO", "handlers": ["default"]},
+             },
+         }
+     )
+
+------------------------
+Using Configuration File
+------------------------
+
+Instead of passing configuration options using command line arguments, you can use
+configuration file. The configuration file is Python file that must define the **config**
+object of the `Config class`_.
+
+:✋ Note:
+   When you mix command line options and custom configuration file,
+   explicit command line options take precedence over the values that are defined
+   for the same parameters in the configuration file.
+
+:✨ Why:
+   Defining configuration file in Python instead of YAML or something else
+   has a few advantages. For example, you can edit it with
+   any Python IDE that provides a convenience of autocompletion and hints.
+
+For example,
+
+:config.py:
+
+   Simple configuration file. You can find a complete example in `examples/config.py <https://github.com/testflows/TestFlows-GitHub-Runners/blob/main/examples/config.py>`_.
+
+   .. code-block:: python3
+
+      from testflows.github.runners.config import *
+
+      config = Config(
+         github_token=os.getenv("GITHUB_TOKEN"),
+         github_repository=os.getenv("GITHUB_REPOSITORY"),
+         hetzner_token=os.getenv("HETZNER_TOKEN"),
+         default_server_type=server_type("cx11"),
+         cloud=cloud(server_name="my-github-runners-service"),
+         standby_runners=[
+            standby_runner(
+                  labels=["type-cx21"],
+                  count=2,
+                  replenish_immediately=True,
+            )
+         ],
+      )
+
+You can sanity check your configuration file by executing it directly:
+
+.. code-block:: bash
+
+   python3 config.py
+
+You can pass your custom configuration file using the *-c path, --config path** command line option.
+
+.. code-block:: bash
+
+   github-runners -c config.py
+
+Configuration Schema
+=====================
+
+The `Config class`_ has the following schema:
+
+:schema:
+   * **github_token: str**
+   * **github_repository: str**
+   * **hetzner_token: str**
+   * **ssh_key: str**
+   * **max_runners**
+   * **default_image: image**
+   * **default_server_type: server_type**
+   * **default_location: location**
+   * **workers: count**
+   * **setup_script: path**
+   * **startup_x64_script: path**
+   * **startup_arm64_script: path**
+   * **max_powered_off_time: count**
+   * **max_unused_runner_time: count**
+   * **max_runner_registration_time: count**
+   * **max_server_ready_time: count**
+   * **scale_up_interval: count**
+   * **scale_down_interval: count**
+   * **debug: bool**
+   * **logger_config: dict**
+   * **cloud: cloud**
+      * **server_name: str**
+      * **deploy: deploy**
+         * **server_type: server_type**
+         * **image: image**
+         * **location: location**
+         * **setup_script: path**
+   * **standby_runners: list[standby_runner]**
+      * **labels: list[str]**
+      * **count: count**
+      * **replenish_immediately: bool**
+
+----
+
 -------
 SSH Key
 -------
 
 All server instances that are created are accessed via SSH using the **ssh** utility and therefore you must provide a valid SSH key
 using the **--ssh-key** option. If the **--ssh-key** option is no specified, then the *~/.ssh/id_rsa.pub* default key path will be used.
 
@@ -371,15 +584,15 @@
       User=1000
       Group=1000
       Type=simple
       Restart=always
       Environment=GITHUB_TOKEN=ghp_...
       Environment=GITHUB_REPOSITORY=testflows/github-runners
       Environment=HETZNER_TOKEN=GJ..
-      ExecStart=/home/user/.local/lib/python3.10/site-packages/testflows/github/runners/bin/github-runners --workers 10 --max-powered-off-time 20 --max-idle-runner-time 120 --max-runner-registration-time 60 --scale-up-interval 10 --scale-down-interval 10
+      ExecStart=/home/user/.local/lib/python3.10/site-packages/testflows/github/runners/bin/github-runners --workers 10 --max-powered-off-time 20 --max-unused-runner-time 120 --max-runner-registration-time 60 --scale-up-interval 10 --scale-down-interval 10
       [Install]
       WantedBy=multi-user.target
 
 ----
 
 Modifying Program Options
 =========================
@@ -414,15 +627,15 @@
            Loaded: loaded (/etc/systemd/system/github-runners.service; enabled; vendor preset: enabled)
            Active: active (running) since Mon 2023-07-24 14:38:33 EDT; 1h 31min ago
          Main PID: 66188 (python3)
             Tasks: 3 (limit: 37566)
            Memory: 28.8M
               CPU: 8.274s
            CGroup: /system.slice/github-runners.service
-                   └─66188 python3 /usr/local/bin/github-runners --workers 10 --max-powered-off-time 20 --max-idle-runner-time 120 --max->
+                   └─66188 python3 /usr/local/bin/github-runners --workers 10 --max-powered-off-time 20 --max-unused-runner-time 120 --max->
 
       Jul 24 14:38:33 user-node systemd[1]: Started Autoscaling GitHub Actions Runners.
       Jul 24 14:38:33 user-node github-runners[66188]: 07/24/2023 02:38:33 PM   INFO MainThread            main 🍀 Logging in to Hetzner >
       Jul 24 14:38:33 user-node github-runners[66188]: 07/24/2023 02:38:33 PM   INFO MainThread            main 🍀 Logging in to GitHub
       Jul 24 14:38:33 user-node github-runners[66188]: 07/24/2023 02:38:33 PM   INFO MainThread            main 🍀 Getting repository vza>
       Jul 24 14:38:33 user-node github-runners[66188]: 07/24/2023 02:38:33 PM   INFO MainThread            main 🍀 Creating scale up serv>
       Jul 24 14:38:33 user-node github-runners[66188]: 07/24/2023 02:38:33 PM   INFO MainThread            main 🍀 Creating scale down se>
@@ -828,16 +1041,16 @@
 For each such job, a corresponding Hetzner Cloud server instance is created with the following name:
 
 ::
 
    github-runner-{job.run_id}-{job.id}
 
 The server is configured using default **setup** and **startup** scripts. The runner name is set
-to be the same as the server name so that servers can be deleted for any idle runner that for some reason
-does not pick up a job for which it was created within the **max-idle-runner-time** period.
+to be the same as the server name so that servers can be deleted for any unused runner that for some reason
+does not pick up a job for which it was created within the **max-unused-runner-time** period.
 
 :Note:
    Given that the server name is fixed and specific for each *job.run_id, job.id* tuple, if multiple `github-runners` are running in parallel then
    only 1 server will be created for a given `job` and any other attempts to create a server with the same name will be rejected
    by the Hetzner Cloud.
 
 Also,
@@ -983,21 +1196,21 @@
 
 The program scales down runners by first cleaning up powered off servers. The scale down service relies on the fact
 that the `startup <#the-start-up-script>`_ script starts an ephemeral runner which will pick up only 1 job and then will power itself off after the job is complete.
 
 The powered off servers are deleted after the **max-powered-off-time** interval which
 can be specified using the **--max-powered-off-time** option which by default is set to *20* sec.
 
-Idle Runners
-============
+Unused Runners
+==============
 
-The scale down service also monitors all the runners that have **idle** status and tries to delete any servers associated with such
-runners if the runner is **idle** for more than the **max-idle-runner-time** period. This is needed in case a runner never gets a job
+The scale down service also monitors all the runners that have **unused** status and tries to delete any servers associated with such
+runners if the runner is **unused** for more than the **max-unused-runner-time** period. This is needed in case a runner never gets a job
 assigned to it and the server will stay in the power on state. This cycle relies on the fact that the runner's name
-is the same as server's name. The **max-idle-runner-time** can be specified using the **--max-idle-runner-time** option which by default
+is the same as server's name. The **max-unused-runner-time** can be specified using the **--max-unused-runner-time** option which by default
 is set to *120* sec.
 
 Zombie Servers
 ==============
 
 The scale down service will delete any zombie servers. A zombie server is defined as as any server that fails to register its runner within
 the **max-runner-registration-time**. The **max-runner-registration-time** can be specified using the **--max-runner-registration-time** option
@@ -1021,15 +1234,15 @@
 :The *./run.sh* Command Fails:
    The server will be powered off by the **startup** script and will be deleted by the scale down service.
 
 :Creating Server For Queued Job Fails:
    If creation of the server fails for some reason then the scale up service will retry the operation in the next interval as the job's status will remain **queued**.
 
 :Runner Never Gets a Job Assigned:
-   If the runner never gets a job assigned, then the scale down service will remove the runner and delete its server after the **max-idle-runner-time** period.
+   If the runner never gets a job assigned, then the scale down service will remove the runner and delete its server after the **max-unused-runner-time** period.
 
 :Runner Created With a Mismatched Labels:
    The behavior will be the same as for the **Runner Never Gets a Job Assigned** case above.
 
 ----
 
 ---------------
@@ -1043,14 +1256,17 @@
 
 * **-v, --version**
   show program's version number and exit
 
 * **--license**
   show program's license and exit
 
+* **-c path, --config path**
+  program configuration file
+
 * **--github-token GITHUB_TOKEN**
   GitHub token, default: *$GITHUB_TOKEN* environment variable
 
 * **--github-repository GITHUB_REPOSITORY**
   GitHub repository, default: *$GITHUB_REPOSITORY* environment variable
 
 * **--hetzner-token HETZNER_TOKEN**
@@ -1072,31 +1288,28 @@
 
 * **-m count, --max-runners count**
   maximum number of active runners, default: *10*
 
 * **-w count, --workers count**
   number of concurrent workers, default: *10*
 
-* **--logger-config path**
-  custom logger configuration file
-
 * **--setup-script path**
   path to custom server setup script
 
 * **--startup-x64-script path**
   path to custom server startup script
 
 * **--startup-arm64-script path**
   path to custom ARM64 server startup script
 
 * **--max-powered-off-time sec**
   maximum time after which a powered off server is deleted, default: *60* sec
 
-* **--max-idle-runner-time sec**
-  maximum time after which an idle runner is removed and its server deleted, default: *120* sec
+* **--max-unused-runner-time sec**
+  maximum time after which an unused runner is removed and its server deleted, default: *120* sec
 
 * **--max-runner-registration-time**
   maximum time after which the server will be deleted if its runner is not registered with GitHub, default: *120* sec
 
 * **--max-server-ready-time sec**
   maximum time to wait for the server to be in the running state, default: *120* sec
 
@@ -1208,7 +1421,17 @@
           follow logs journal, default: *False*
 
       * **start**
         start service
 
       * **stop**
         stop service
+
+-----------------
+Table of Contents
+-----------------
+
+.. contents:: Index:
+   :backlinks: top
+   :depth: 4
+
+.. _Config class: https://github.com/testflows/TestFlows-GitHub-Runners/blob/main/testflows/github/runners/config.py#L45
```

### Comparing `testflows.github.runners-1.2.230728.1203052/setup.py` & `testflows.github.runners-1.3.230729.1222222/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 with open("README.rst", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 
 setup(
     name="testflows.github.runners",
-    version="1.2.230728.1203052",
+    version="1.3.230729.1222222",
     description="Autoscaling GitHub Actions Runners Using Hetzner Cloud ",
     author="Vitaliy Zakaznikov",
     author_email="vzakaznikov@testflows.com",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/testflows/github-runners",
     classifiers=[
@@ -45,10 +45,10 @@
     package_data={
         "testflows.github.runners.scripts": ["*.sh"],
         "testflows.github.runners.scripts.deploy": ["*.sh"],
         "testflows.github.runners.bin": ["github-runners"],
     },
     scripts=["testflows/github/runners/bin/github-runners"],
     zip_safe=False,
-    install_requires=["PyGithub==1.59.0", "hcloud==1.25.0"],
+    install_requires=["PyGithub==1.59.0", "hcloud==1.26.0"],
     extras_require={"dev": []},
 )
```

### Comparing `testflows.github.runners-1.2.230728.1203052/testflows/github/runners/__init__.py` & `testflows.github.runners-1.3.230729.1222222/testflows/github/runners/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 __author__ = "Vitaliy Zakaznikov"
-__version__ = "1.2.230728.1203052"
+__version__ = "1.3.230729.1222222"
 __license__ = f"""
 Copyright 2023 Katteli Inc.
 TestFlows.com Open-Source Software Testing Framework (http://testflows.com)
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `testflows.github.runners-1.2.230728.1203052/testflows/github/runners/actions.py` & `testflows.github.runners-1.3.230729.1222222/testflows/github/runners/actions.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1203052/testflows/github/runners/bin/github-runners` & `testflows.github.runners-1.3.230729.1222222/testflows/github/runners/bin/github-runners`

 * *Files 5% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import os
 import sys
 import time
 import hashlib
 import logging
 import threading
+import logging.config
 
 from concurrent.futures import ThreadPoolExecutor, Future
 
 from hcloud import Client
 from hcloud.ssh_keys.domain import SSHKey
 
 from github import Github
@@ -32,21 +32,20 @@
 
 from testflows.github.runners import __version__, __license__
 from testflows.github.runners.actions import Action
 from testflows.github.runners.scale_up import scale_up
 from testflows.github.runners.scale_down import scale_down
 from testflows.github.runners.scripts import Scripts, scripts
 from testflows.github.runners.logger import logger
+from testflows.github.runners.config import Config, check_image
 
 import testflows.github.runners.args as args
 import testflows.github.runners.cloud as cloud
 import testflows.github.runners.service as service
 
-check_args = args.check
-check_image = args.check_image
 
 description = """Auto-scaling GitHub Actions runners service using Hetzner Cloud.
 
     Service that starts and monitors queued up GitHub Actions workflows.
     When a new job is queued up, it creates new Hetzner Cloud server instance
     that provides an ephemeral GitHub Actions runner. Server is automatically
     powered off when job completes and then powered off servers are
@@ -73,69 +72,73 @@
         "--license",
         action="version",
         help="show program's license and exit",
         version=f"{__license__}",
     )
 
     parser.add_argument(
+        "-c",
+        "--config",
+        metavar="path",
+        dest="config_file",
+        type=args.config_type,
+        help="program configuration file",
+        default=None,
+    )
+
+    parser.add_argument(
         "--github-token",
-        type=args.env_var_type("GITHUB_TOKEN"),
+        type=str,
         help="GitHub token, default: $GITHUB_TOKEN environment variable",
-        default="",
     )
 
     parser.add_argument(
         "--github-repository",
-        type=args.env_var_type("GITHUB_REPOSITORY"),
+        type=str,
         help="GitHub repository, default: $GITHUB_REPOSITORY environment variable",
-        default="",
     )
 
     parser.add_argument(
         "--hetzner-token",
-        type=args.env_var_type("HETZNER_TOKEN"),
+        type=str,
         help="Hetzner Cloud token, default: $HETZNER_TOKEN environment variable",
-        default="",
     )
 
     parser.add_argument(
         "--ssh-key",
         metavar="path",
         type=str,
         help="path to public SSH key, default: ~/.ssh/id_rsa.pub",
-        default=os.path.expanduser("~/.ssh/id_rsa.pub"),
     )
 
     parser.add_argument(
         "-m",
         "--max-runners",
         metavar="count",
         type=args.count_type,
         help="maximum number of active runners, default: 10",
-        default=10,
     )
 
     parser.add_argument(
         "--default-image",
         metavar="type:name_or_description",
         type=args.image_type,
         help=(
             "default runner server image type and name or description,\n"
             "where the type is either: 'system','snapshot','backup','app',\n"
             "default: system:ubuntu-22.04"
         ),
-        default="system:ubuntu-22.04",
     )
 
     parser.add_argument(
         "--default-type",
+        dest="default_server_type",
         metavar="name",
         type=args.server_type,
         help=("default runner server type name, default: cx11"),
-        default="cx11",
     )
 
     parser.add_argument(
         "--default-location",
         metavar="name",
         type=args.location_type,
         help=("default runner server location name, by default not specified"),
@@ -143,22 +146,14 @@
 
     parser.add_argument(
         "-w",
         "--workers",
         metavar="count",
         type=args.count_type,
         help="number of concurrent workers, default: 10",
-        default=10,
-    )
-
-    parser.add_argument(
-        "--logger-config",
-        metavar="path",
-        type=args.path_type,
-        help="custom logger configuration file",
     )
 
     parser.add_argument(
         "--setup-script",
         metavar="path",
         type=args.path_type,
         help="path to custom server setup script",
@@ -179,62 +174,55 @@
     )
 
     parser.add_argument(
         "--max-powered-off-time",
         metavar="sec",
         type=args.count_type,
         help="maximum time after which a powered off server is deleted, default: 60 sec",
-        default=60,
     )
 
     parser.add_argument(
-        "--max-idle-runner-time",
+        "--max-unused-runner-time",
         metavar="sec",
         type=args.count_type,
-        help="maximum time after which an idle runner is removed and its server deleted, default: 120 sec",
-        default=120,
+        help="maximum time after which an unused runner is removed and its server deleted, default: 120 sec",
     )
 
     parser.add_argument(
         "--max-runner-registration-time",
         metavar="sec",
         type=args.count_type,
         help="maximum time after which the server will be deleted if it fails to register a runner, default: 120 sec",
-        default=120,
     )
 
     parser.add_argument(
         "--max-server-ready-time",
         metavar="sec",
         type=args.count_type,
         help="maximum time to wait for the server to be in the running state, default: 120 sec",
-        default=120,
     )
 
     parser.add_argument(
         "--scale-up-interval",
         metavar="sec",
         type=args.count_type,
         help="scale up service interval, default: 15 sec",
-        default=15,
     )
 
     parser.add_argument(
         "--scale-down-interval",
         metavar="sec",
         type=args.count_type,
         help="scale down service interval, default: 15 sec",
-        default=15,
     )
 
     parser.add_argument(
         "--debug",
         action="store_true",
         help="enable debugging mode, default: False",
-        default=False,
     )
 
     commands = parser.add_subparsers(
         title="commands", metavar="command", description=None, help=None
     )
 
     cloud_parser = commands.add_parser(
@@ -244,18 +232,17 @@
         formatter_class=RawTextHelpFormatter,
     )
 
     cloud_parser.add_argument(
         "-n",
         "--name",
         metavar="server",
-        dest="server_name",
+        dest="cloud_server_name",
         type=str,
         help="deployment server name, default: github-runners",
-        default="github-runners",
     )
 
     cloud_commands = cloud_parser.add_subparsers(
         title="commands", metavar="command", description=None, help=None
     )
 
     cloud_commands.required = True
@@ -284,45 +271,45 @@
         ),
     )
 
     deploy_cloud_parser.add_argument(
         "-l",
         "--location",
         metavar="name",
+        dest="cloud_deploy_location",
         type=args.location_type,
-        help="deployment server location, default: ash",
-        default="ash",
+        help="deployment server location",
     )
 
     deploy_cloud_parser.add_argument(
         "-t",
         "--type",
         metavar="name",
+        dest="cloud_deploy_server_type",
         type=args.server_type,
         help="deployment server type, default: cpx11",
-        default="cpx11",
     )
 
     deploy_cloud_parser.add_argument(
         "-i",
         "--image",
         metavar="type:name_or_description",
+        dest="cloud_deploy_image",
         type=args.image_type,
         help=(
             "deployment server image type and name or description,\n"
             "where the type is either: 'system','snapshot','backup','app',\n"
             "default: system:ubuntu-22.04"
         ),
-        default="system:ubuntu-22.04",
     )
 
     deploy_cloud_parser.add_argument(
         "--setup-script",
         metavar="path",
-        dest="deploy_setup_script",
+        dest="cloud_deploy_setup_script",
         type=args.path_type,
         help="path to custom deployment server setup script",
     )
 
     deploy_cloud_parser.set_defaults(func=cloud.deploy)
 
     redeploy_cloud_parser = cloud_commands.add_parser(
@@ -564,34 +551,38 @@
         help="follow the logs journal",
     )
     logs_service_parser.set_defaults(func=service.logs)
 
     return parser
 
 
-def main(args, scripts: Scripts, worker_pool: ThreadPoolExecutor, terminate_timeout=30):
+def main(
+    config, scripts: Scripts, worker_pool: ThreadPoolExecutor, terminate_timeout=30
+):
     """Auto-scale runners service."""
 
     terminate = threading.Event()
 
     try:
         with Action("Logging in to Hetzner Cloud"):
-            client = Client(token=args.hetzner_token)
+            client = Client(token=config.hetzner_token)
 
         with Action("Logging in to GitHub"):
-            github = Github(login_or_token=args.github_token)
+            github = Github(login_or_token=config.github_token)
 
-        with Action(f"Getting repository {args.github_repository}"):
-            repo: Repository = github.get_repo(args.github_repository)
+        with Action(f"Getting repository {config.github_repository}"):
+            repo: Repository = github.get_repo(config.github_repository)
 
         with Action("Checking if default image exists"):
-            args.default_image = check_image(client=client, image=args.default_image)
+            config.default_image = check_image(
+                client=client, image=config.default_image
+            )
 
         with Action(f"Checking if SSH key exists"):
-            with open(args.ssh_key, "r", encoding="utf-8") as ssh_key_file:
+            with open(config.ssh_key, "r", encoding="utf-8") as ssh_key_file:
                 public_key = ssh_key_file.read()
             key_name = hashlib.md5(public_key.encode("utf-8")).hexdigest()
             ssh_key = SSHKey(name=key_name, public_key=public_key)
 
             if not client.ssh_keys.get_by_name(name=ssh_key.name):
                 with Action(f"Creating SSH key {ssh_key.name}"):
                     client.ssh_keys.create(
@@ -603,37 +594,39 @@
                 scale_up_service: Future = worker_pool.submit(
                     scale_up,
                     terminate=terminate,
                     repo=repo,
                     client=client,
                     scripts=scripts,
                     ssh_key=ssh_key,
-                    default_type=args.default_type,
-                    default_image=args.default_image,
-                    default_location=args.default_location,
+                    default_server_type=config.default_server_type,
+                    default_image=config.default_image,
+                    default_location=config.default_location,
                     worker_pool=worker_pool,
-                    github_token=args.github_token,
-                    github_repository=args.github_repository,
-                    interval=args.scale_up_interval,
-                    max_servers=args.max_runners,
-                    max_server_ready_time=args.max_server_ready_time,
-                    debug=args.debug,
+                    github_token=config.github_token,
+                    github_repository=config.github_repository,
+                    interval=config.scale_up_interval,
+                    max_servers=config.max_runners,
+                    max_server_ready_time=config.max_server_ready_time,
+                    debug=config.debug,
+                    standby_runners=config.standby_runners,
                 )
 
             with Action("Creating scale down service"):
                 scale_down_service: Future = worker_pool.submit(
                     scale_down,
                     terminate=terminate,
                     repo=repo,
                     client=client,
-                    max_powered_off_time=args.max_powered_off_time,
-                    max_idle_runner_time=args.max_idle_runner_time,
-                    max_runner_registration_time=args.max_runner_registration_time,
-                    interval=args.scale_down_interval,
-                    debug=args.debug,
+                    max_powered_off_time=config.max_powered_off_time,
+                    max_unused_runner_time=config.max_unused_runner_time,
+                    max_runner_registration_time=config.max_runner_registration_time,
+                    interval=config.scale_down_interval,
+                    debug=config.debug,
+                    standby_runners=config.standby_runners,
                 )
 
             while True:
                 time.sleep(1)
 
                 if scale_up_service.done():
                     raise RuntimeError("scale-up service exited")
@@ -653,69 +646,77 @@
             with Action(
                 "Waiting for scale down service to terminate", ignore_fail=True
             ):
                 scale_up_service.result(timeout=terminate_timeout)
 
     except KeyboardInterrupt as exc:
         msg = "❗ KeyboardInterrupt"
-        if args.debug:
+        if config.debug:
             logger.exception(f"{msg}\n{exc}")
         else:
             logger.error(msg)
         sys.exit(1)
+
     except Exception as exc:
         msg = f"❗ Error: {type(exc).__name__} {exc}"
-        if args.debug:
+        if config.debug:
             logger.exception(f"{msg}\n{exc}")
         else:
             logger.error(msg)
         sys.exit(1)
 
 
 if __name__ == "__main__":
     args = argparser().parse_args()
 
     logging_level = logging.INFO
 
-    if args.debug:
+    if args.config_file:
+        config = args.config_file
+    else:
+        config = Config()
+
+    config.update(args)
+
+    if config.debug:
         Action.debug = True
         logging_level = logging.DEBUG
 
-    if args.logger_config:
-        logging.config.fileConfig(args.logger_config)
+    if config.logger_config:
+        logging.config.dictConfig(config.logger_config)
     else:
         logger.setLevel(logging_level)
         handler = logging.StreamHandler(sys.stdout)
         formatter = logging.Formatter(
             "%(asctime)s %(levelname)8s %(threadName)16s %(funcName)15s %(message)s",
             datefmt="%m/%d/%Y %I:%M:%S %p",
         )
         handler.setFormatter(formatter)
         logger.addHandler(handler)
 
-    if args.setup_script:
-        scripts.setup = args.setup_script
+    if config.setup_script:
+        scripts.setup = config.setup_script
 
-    if args.startup_x64_script:
-        scripts.startup_x64 = args.startup_x64_script
+    if config.startup_x64_script:
+        scripts.startup_x64 = config.startup_x64_script
 
-    if args.startup_arm64_script:
-        scripts.startup_arm64 = args.startup_arm64_script
+    if config.startup_arm64_script:
+        scripts.startup_arm64 = config.startup_arm64_script
 
     if hasattr(args, "func"):
         try:
-            args.func(args=args)
+            args.func(args=args, config=config)
         except KeyboardInterrupt:
-            if args.debug:
+            if config.debug:
                 raise
         except BaseException as exc:
-            if args.debug:
+            if config.debug:
                 raise
             logger.fatal(f"❗ Error: {exc}")
 
     else:
-        check_args(args)
+        config.check()
 
         with ThreadPoolExecutor(
-            max_workers=args.workers + 2, thread_name_prefix="worker"
+            max_workers=config.workers + 2, thread_name_prefix="worker"
         ) as worker_pool:
-            main(args=args, scripts=scripts, worker_pool=worker_pool)
+            main(config=config, scripts=scripts, worker_pool=worker_pool)
```

### Comparing `testflows.github.runners-1.2.230728.1203052/testflows/github/runners/cloud.py` & `testflows.github.runners-1.3.230729.1222222/testflows/github/runners/cloud.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,105 +9,107 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
+import sys
 import hashlib
 
 from hcloud import Client
 from hcloud.ssh_keys.domain import SSHKey
-from hcloud.server_types.domain import ServerType
 from hcloud.servers.client import BoundServer
-from hcloud.images.domain import Image
-from hcloud.locations.domain import Location
 
 from .actions import Action
-from .args import check, check_image
+from .config import Config, check_image
 from . import __version__
 
 from .server import wait_ready, wait_ssh, ssh, scp, ip_address, ssh_command
 from .service import command_options
 
 current_dir = os.path.dirname(__file__)
 deploy_scripts_folder = "/home/ubuntu/.github-runners/scripts/"
 deploy_configs_folder = "/home/ubuntu/.github-runners/configs/"
 
 
-def deploy(args, redeploy=False):
+def deploy(args, config: Config, redeploy=False):
     """Deploy or redeploy github-runners as a service to a
     new Hetzner server instance."""
-    check(args)
-
+    config.check()
     version = args.version or __version__
-
-    server_name = args.server_name
+    server_name = config.cloud.server_name
 
     with Action("Logging in to Hetzner Cloud"):
-        client = Client(token=args.hetzner_token)
+        client = Client(token=config.hetzner_token)
 
     if redeploy:
         with Action(f"Getting server {server_name}"):
             server: BoundServer = client.servers.get_by_name(server_name)
 
-        uninstall(args=args, server=server)
+        uninstall(args=args, config=config, server=server)
 
         with Action("Cleaning copied scripts"):
             ssh(server, f"rm -rf {deploy_scripts_folder}*")
 
         with Action("Cleaning copied configs"):
             ssh(server, f"rm -rf {deploy_configs_folder}*")
 
     else:
-        deploy_setup_script = args.deploy_setup_script or os.path.join(
+        deploy_setup_script = config.cloud.deploy.setup_script or os.path.join(
             current_dir, "scripts", "deploy", "setup.sh"
         )
 
         if args.force:
             with Action(
                 f"Checking if server {server_name} already exists", ignore_fail=True
             ):
                 server: BoundServer = client.servers.get_by_name(server_name)
                 with Action(f"Deleting server {server_name}"):
                     server.delete()
 
         with Action("Checking if default image exists"):
-            args.default_image = check_image(client=client, image=args.default_image)
+            config.default_image = check_image(
+                client=client, image=config.default_image
+            )
 
         with Action("Checking if server image exists"):
-            args.image = check_image(client=client, image=args.image)
+            config.cloud.deploy.image = check_image(
+                client=client, image=config.cloud.deploy.image
+            )
 
         with Action(f"Checking if SSH key exists"):
-            with open(args.ssh_key, "r", encoding="utf-8") as ssh_key_file:
+            with open(config.ssh_key, "r", encoding="utf-8") as ssh_key_file:
                 public_key = ssh_key_file.read()
             key_name = hashlib.md5(public_key.encode("utf-8")).hexdigest()
             ssh_key = SSHKey(name=key_name, public_key=public_key)
 
             if not client.ssh_keys.get_by_name(name=ssh_key.name):
                 with Action(f"Creating SSH key {ssh_key.name}"):
                     client.ssh_keys.create(
                         name=ssh_key.name, public_key=ssh_key.public_key
                     )
 
         with Action(f"Creating new server"):
             response = client.servers.create(
                 name=server_name,
-                server_type=args.type,
-                image=args.image,
-                location=args.location,
+                server_type=config.cloud.deploy.server_type,
+                image=config.cloud.deploy.image,
+                location=config.cloud.deploy.location,
                 ssh_keys=[ssh_key],
             )
             server: BoundServer = response.server
 
         with Action(f"Waiting for server to be ready") as action:
-            wait_ready(server=server, timeout=args.max_server_ready_time, action=action)
+            wait_ready(
+                server=server, timeout=config.max_server_ready_time, action=action
+            )
 
         with Action("Wait for SSH connection to be ready"):
-            wait_ssh(server=server, timeout=args.max_server_ready_time)
+            wait_ssh(server=server, timeout=config.max_server_ready_time)
 
         with Action("Executing setup.sh script"):
             ssh(
                 server,
                 f"bash -s  < {deploy_setup_script}",
             )
 
@@ -120,172 +122,177 @@
                 command.replace("pip3 install", "pip3 install --upgrade")
 
         ssh(server, command)
 
     with Action("Copying any custom scripts"):
         ip = ip_address(server)
 
-        if args.setup_script:
-            with Action(f"Copying custom setup script {args.setup_script}"):
+        if config.setup_script:
+            with Action(f"Copying custom setup script {config.setup_script}"):
                 scp(
-                    source=args.setup_script,
+                    source=config.setup_script,
                     destination=f"root@{ip}:{deploy_scripts_folder}.",
                 )
-                args.setup_script = os.path.join(
+                config.setup_script = os.path.join(
                     deploy_scripts_folder,
-                    os.path.basename(args.setup_script),
+                    os.path.basename(config.setup_script),
                 )
 
-        if args.startup_x64_script:
-            with Action(f"Copying custom startup x64 script {args.startup_x64_script}"):
+        if config.startup_x64_script:
+            with Action(
+                f"Copying custom startup x64 script {config.startup_x64_script}"
+            ):
                 scp(
-                    source=args.startup_x64_script,
+                    source=config.startup_x64_script,
                     destination=f"root@{ip}:{deploy_scripts_folder}.",
                 )
-                args.startup_x64_script = os.path.join(
+                config.startup_x64_script = os.path.join(
                     deploy_scripts_folder,
-                    os.path.basename(args.startup_x64_script),
+                    os.path.basename(config.startup_x64_script),
                 )
 
-        if args.startup_arm64_script:
+        if config.startup_arm64_script:
             with Action(
-                f"Copying custom startup ARM64 script {args.startup_arm64_script}"
+                f"Copying custom startup ARM64 script {config.startup_arm64_script}"
             ):
                 scp(
-                    source=args.startup_arm64_script,
+                    source=config.startup_arm64_script,
                     destination=f"root@{ip}:{deploy_scripts_folder}.",
                 )
-                args.startup_arm64_script = os.path.join(
+                config.startup_arm64_script = os.path.join(
                     deploy_scripts_folder,
-                    os.path.basename(args.startup_arm64_script),
+                    os.path.basename(config.startup_arm64_script),
                 )
 
     with Action("Fixing ownership of any copied scripts"):
         ssh(server, f"chown -R ubuntu:ubuntu {deploy_scripts_folder}")
 
-    if args.logger_config:
-        with Action(f"Copying custom logger config {args.logger_config}"):
+    if config.config_file:
+        with Action(f"Copying config file {config.config_file}"):
             scp(
-                source=args.logger_config,
+                source=config.config_file,
                 destination=f"root@{ip}:{deploy_configs_folder}.",
             )
-            args.logger_config = os.path.join(
+            config.config_file = os.path.join(
                 deploy_configs_folder,
-                os.path.basename(args.logger_config),
+                os.path.basename(config.config_file),
             )
 
     with Action("Fixing ownership of any copied configs"):
         ssh(server, f"chown -R ubuntu:ubuntu {deploy_configs_folder}")
 
-    install(args, server=server)
+    install(args, config=config, server=server)
 
 
-def redeploy(args):
+def redeploy(args, config: Config):
     """Redeploy service on a existing cloud instance."""
-    deploy(args=args, redeploy=True)
+    deploy(args=args, config=config, redeploy=True)
 
 
-def install(args, server: BoundServer = None):
+def install(args, config: Config, server: BoundServer = None):
     """Install service on a cloud instance."""
     if server is None:
-        check(args)
-
-        server_name = args.server_name
+        config.check()
+        server_name = config.cloud.server_name
 
         with Action("Logging in to Hetzner Cloud"):
-            client = Client(token=args.hetzner_token)
+            client = Client(token=config.hetzner_token)
 
         with Action(f"Getting server {server_name}"):
             server: BoundServer = client.servers.get_by_name(server_name)
 
     with Action("Installing service"):
         command = f"\"su - ubuntu -c '"
-        command += f"GITHUB_TOKEN={args.github_token} "
-        command += f"GITHUB_REPOSITORY={args.github_repository} "
-        command += f"HETZNER_TOKEN={args.hetzner_token} "
+        command += f"GITHUB_TOKEN={config.github_token} "
+        command += f"GITHUB_REPOSITORY={config.github_repository} "
+        command += f"HETZNER_TOKEN={config.hetzner_token} "
 
         command += "github-runners"
-        command += command_options(args)
+        command += command_options(config)
         command += " service install -f'\""
 
         ssh(server, command)
 
 
-def upgrade(args):
+def upgrade(args, config: Config):
     """Upgrade github-runners application on a cloud instance."""
-    server_name = args.server_name
+    config.check("hetzner_token")
+    server_name = config.cloud.server_name
     upgrade_version = args.upgrade_version
 
     with Action("Logging in to Hetzner Cloud"):
-        client = Client(token=args.hetzner_token)
+        client = Client(token=config.hetzner_token)
 
     with Action(f"Getting server {server_name}"):
         server: BoundServer = client.servers.get_by_name(server_name)
 
-    stop(args, server=server)
+    stop(args, config=config, server=server)
 
     if upgrade_version:
         with Action(f"Upgrading github-runners to version {upgrade_version}"):
             ssh(
                 server,
                 f"'sudo -u ubuntu pip3 install testflows.github.runners=={upgrade_version}'",
             )
     else:
         with Action(f"Upgrading github-runners the latest version"):
             ssh(
                 server,
                 f"'sudo -u ubuntu pip3 install --upgrade testflows.github.runners'",
             )
 
-    start(args, server=server)
+    start(args, config=config, server=server)
 
 
-def uninstall(args, server: BoundServer = None):
+def uninstall(args, config: Config, server: BoundServer = None):
     """Uninstall github-runners service from a cloud instance."""
     if server is None:
-        server_name = args.server_name
+        config.check("hetzner_token")
+        server_name = config.cloud.server_name
 
         with Action("Logging in to Hetzner Cloud"):
-            client = Client(token=args.hetzner_token)
+            client = Client(token=config.hetzner_token)
 
         with Action(f"Getting server {server_name}"):
             server: BoundServer = client.servers.get_by_name(server_name)
 
     with Action("Uninstalling service"):
         command = f"\"su - ubuntu -c 'github-runners service uninstall'\""
         ssh(server, command)
 
 
-def delete(args):
+def delete(args, config: Config):
     """Delete github-runners service running
     on Hetzner server instance by stopping the service
     and deleting the server."""
-    server_name = args.server_name
+    config.check("hetzner_token")
+    server_name = config.cloud.server_name
 
     with Action("Logging in to Hetzner Cloud"):
-        client = Client(token=args.hetzner_token)
+        client = Client(token=config.hetzner_token)
 
     with Action(f"Getting server {server_name}"):
         server: BoundServer = client.servers.get_by_name(server_name)
 
     with Action("Uninstalling service"):
         command = f"\"su - ubuntu -c 'github-runners service uninstall'\""
         ssh(server, command)
 
     with Action(f"Deleting server {server_name}"):
         server.delete()
 
 
-def logs(args, server: BoundServer = None):
+def logs(args, config: Config, server: BoundServer = None):
     """Get cloud server service logs."""
     if server is None:
-        server_name = args.server_name
+        config.check("hetzner_token")
+        server_name = config.cloud.server_name
 
         with Action("Logging in to Hetzner Cloud"):
-            client = Client(token=args.hetzner_token)
+            client = Client(token=config.hetzner_token)
 
         with Action(f"Getting server {server_name}"):
             server: BoundServer = client.servers.get_by_name(server_name)
 
     if server is None:
         raise ValueError("server not found")
 
@@ -293,80 +300,85 @@
         f"\"su - ubuntu -c 'github-runners service logs"
         + (" -f" if args.follow else "")
         + "'\""
     )
     ssh(server, command, use_logger=False)
 
 
-def status(args, server: BoundServer = None):
+def status(args, config: Config, server: BoundServer = None):
     """Get cloud server service status."""
     if server is None:
-        server_name = args.server_name
+        config.check("hetzner_token")
+        server_name = config.cloud.server_name
 
         with Action("Logging in to Hetzner Cloud"):
-            client = Client(token=args.hetzner_token)
+            client = Client(token=config.hetzner_token)
 
         with Action(f"Getting server {server_name}"):
             server = client.servers.get_by_name(server_name)
 
     with Action("Getting status"):
         command = f"\"su - ubuntu -c 'github-runners service status'\""
         ssh(server, command)
 
 
-def start(args, server: BoundServer = None):
+def start(args, config: Config, server: BoundServer = None):
     """Start cloud server service."""
     if server is None:
-        server_name = args.server_name
+        config.check("hetzner_token")
+        server_name = config.cloud.server_name
 
         with Action("Logging in to Hetzner Cloud"):
-            client = Client(token=args.hetzner_token)
+            client = Client(token=config.hetzner_token)
 
         with Action(f"Getting server {server_name}"):
             server = client.servers.get_by_name(server_name)
 
     with Action("Starting service"):
         command = f"\"su - ubuntu -c 'github-runners service start'\""
         ssh(server, command)
 
 
-def stop(args, server: BoundServer = None):
+def stop(args, config: Config, server: BoundServer = None):
     """Stop cloud server service."""
     if server is None:
-        server_name = args.server_name
+        config.check("hetzner_token")
+        server_name = config.cloud.server_name
 
         with Action("Logging in to Hetzner Cloud"):
-            client = Client(token=args.hetzner_token)
+            client = Client(token=config.hetzner_token)
 
         with Action(f"Getting server {server_name}"):
             server = client.servers.get_by_name(server_name)
 
     with Action("Stopping service"):
         command = f"\"su - ubuntu -c 'github-runners service stop'\""
         ssh(server, command)
 
 
-def ssh_client(args):
+def ssh_client(args, config: Config):
     """Open ssh client to github-runners service running
     on Hetzner server instance.
     """
-    server_name = args.server_name
+    config.check("hetzner_token")
+    server_name = config.cloud.server_name
 
     with Action("Logging in to Hetzner Cloud"):
-        client = Client(token=args.hetzner_token)
+        client = Client(token=config.hetzner_token)
 
     with Action(f"Getting server {server_name}"):
         server: BoundServer = client.servers.get_by_name(server_name)
 
     with Action("Opening SSH client"):
         os.system(ssh_command(server=server))
 
 
-def ssh_client_command(args):
+def ssh_client_command(args, config: Config):
     """Return ssh command to connect to github-runners service running
     on Hetzner server instance.
     """
-    server_name = args.server_name
+    config.check("hetzner_token")
+    server_name = config.cloud.server_name
 
-    client = Client(token=args.hetzner_token)
+    client = Client(token=config.hetzner_token)
     server: BoundServer = client.servers.get_by_name(server_name)
-    print(ssh_command(server=server))
+    print(ssh_command(server=server), file=sys.stdout)
```

### Comparing `testflows.github.runners-1.2.230728.1203052/testflows/github/runners/logger.py` & `testflows.github.runners-1.3.230729.1222222/testflows/github/runners/logger.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1203052/testflows/github/runners/request.py` & `testflows.github.runners-1.3.230729.1222222/testflows/github/runners/request.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1203052/testflows/github/runners/scale_down.py` & `testflows.github.runners-1.3.230729.1222222/testflows/github/runners/scale_down.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,15 +15,20 @@
 import time
 import logging
 import threading
 
 from dataclasses import dataclass
 
 from .actions import Action
-from .scale_up import server_name_prefix, runner_name_prefix
+from .scale_up import (
+    server_name_prefix,
+    runner_name_prefix,
+    standby_runner_name_prefix,
+    StandbyRunner,
+)
 from .logger import logger
 
 from github.Repository import Repository
 from github.SelfHostedActionsRunner import SelfHostedActionsRunner
 
 from hcloud import Client
 from hcloud.servers.client import BoundServer
@@ -44,38 +49,39 @@
 
     time: float
     server: BoundServer
     observed_interval: float
 
 
 @dataclass
-class IdleRunner:
-    """Idle self-hosted runner."""
+class UnusedRunner:
+    """Unused self-hosted runner."""
 
     time: float
     runner: SelfHostedActionsRunner
     observed_interval: float
 
 
 def scale_down(
     terminate: threading.Event,
     repo: Repository,
     client: Client,
     max_powered_off_time: int,
-    max_idle_runner_time: int,
+    max_unused_runner_time: int,
     max_runner_registration_time: int,
     interval: int,
     debug: bool = False,
+    standby_runners: list[StandbyRunner] = None,
 ):
     """Scale down service by deleting any powered off server,
-    any server that has stale idle runner, or any server that failed to register its
+    any server that has unused runner, or any server that failed to register its
     runner (zombie server).
     """
     powered_off_servers: dict[str, PoweredOffServer] = {}
-    idle_runners: dict[str, IdleRunner] = {}
+    unused_runners: dict[str, UnusedRunner] = {}
     zombie_servers: dict[str, ZombieServer] = {}
 
     while True:
         current_interval = time.time()
 
         if terminate.is_set():
             with Action("Terminating scale down service"):
@@ -125,27 +131,40 @@
                             zombie_servers[
                                 server.name
                             ].observed_interval = current_interval
 
                         else:
                             zombie_servers.pop(server.name, None)
 
-            with Action("Looking for idle runners", level=logging.DEBUG):
+            with Action("Looking for unused runners", level=logging.DEBUG):
                 for runner in runners:
                     if runner.status == "online" and not runner.busy:
                         if runner.name.startswith(runner_name_prefix):
-                            if runner.name not in idle_runners:
-                                with Action(f"Found new idle runner {runner.name}"):
-                                    idle_runners[runner.name] = IdleRunner(
+                            # skip any specified standby runners
+                            if runner.name.startswith(standby_runner_name_prefix):
+                                found = False
+                                for standby_runner in standby_runners:
+                                    if set(standby_runner.labels).issubset(
+                                        set(
+                                            [label["name"] for label in runner.labels()]
+                                        )
+                                    ):
+                                        found = True
+                                        break
+                                if found:
+                                    continue
+                            if runner.name not in unused_runners:
+                                with Action(f"Found new unused runner {runner.name}"):
+                                    unused_runners[runner.name] = UnusedRunner(
                                         time=time.time(),
                                         runner=runner,
                                         observed_interval=current_interval,
                                     )
-                            idle_runners[runner.name].runner = runner
-                            idle_runners[
+                            unused_runners[runner.name].runner = runner
+                            unused_runners[
                                 runner.name
                             ].observed_interval = current_interval
 
             with Action(
                 "Checking which powered off servers need to be deleted",
                 level=logging.DEBUG,
             ):
@@ -186,51 +205,50 @@
                                 f"Deleting zombie server {server_name}",
                                 ignore_fail=True,
                             ) as action:
                                 zombie_server.server.delete()
                                 zombie_servers.pop(server_name)
 
             with Action(
-                "Checking which idle runners need to be removed and their servers deleted",
+                "Checking which unused runners need to be removed",
                 level=logging.DEBUG,
             ):
 
-                for idle_runner_name in list(idle_runners.keys()):
-                    idle_runner = idle_runners[idle_runner_name]
+                for runner_name in list(unused_runners.keys()):
+                    unused_runner = unused_runners[runner_name]
 
-                    if idle_runner.observed_interval != current_interval:
-                        with Action(f"Forgetting about idle runner {idle_runner_name}"):
-                            idle_runners.pop(idle_runner_name)
+                    if unused_runner.observed_interval != current_interval:
+                        with Action(f"Forgetting about unused runner {runner_name}"):
+                            unused_runners.pop(runner_name)
 
                     else:
-                        if time.time() - idle_runner.time > max_idle_runner_time:
+                        if time.time() - unused_runner.time > max_unused_runner_time:
                             runner_server = None
 
                             with Action(
-                                f"Try to find server for the runner {idle_runner_name}",
+                                f"Try to find server for the runner {runner_name}",
                                 ignore_fail=True,
                             ):
-                                runner_server = client.servers.get_by_name(
-                                    idle_runner_name
-                                )
+                                runner_server = client.servers.get_by_name(runner_name)
 
                             if runner_server is not None:
                                 with Action(
-                                    f"Deleting idle runner server {runner_server.name}",
+                                    f"Deleting unused runner server {runner_server.name}",
                                     ignore_fail=True,
                                 ):
                                     runner_server.delete()
                                     runner_server = None
 
                             if runner_server is None:
                                 with Action(
-                                    f"Removing self-hosted runner {idle_runner_name}",
+                                    f"Removing self-hosted runner {runner_name}",
                                     ignore_fail=True,
                                 ):
-                                    repo.remove_self_hosted_runner(idle_runner.runner)
+                                    repo.remove_self_hosted_runner(unused_runner.runner)
+
         except Exception as exc:
             msg = f"❗ Error: {type(exc).__name__} {exc}"
             if debug:
                 logger.exception(f"{msg}\n{exc}")
             else:
                 logger.error(msg)
```

### Comparing `testflows.github.runners-1.2.230728.1203052/testflows/github/runners/scale_up.py` & `testflows.github.runners-1.3.230729.1222222/testflows/github/runners/scale_up.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,41 +10,58 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
 import time
+import uuid
 import logging
 import threading
 
+from dataclasses import dataclass
+
 from .actions import Action
 from .scripts import Scripts
 from .request import request
-from .args import image_type, check_image
+from .args import image_type
 from .logger import logger
+from .config import check_image
+from .config import standby_runner as StandbyRunner
 
 from .server import wait_ssh, ssh, wait_ready
 
-from hcloud import Client, APIException
+from hcloud import Client
 from hcloud.ssh_keys.domain import SSHKey
 from hcloud.server_types.domain import ServerType
 from hcloud.locations.domain import Location
 from hcloud.servers.client import BoundServer
+from hcloud.servers.domain import Server
 from hcloud.images.domain import Image
+from hcloud.helpers.labels import LabelValidator
 
 from github.Repository import Repository
 from github.WorkflowJob import WorkflowJob
 from github.WorkflowRun import WorkflowRun
 from github.SelfHostedActionsRunner import SelfHostedActionsRunner
 
 from concurrent.futures import ThreadPoolExecutor, Future
 
 server_name_prefix = "github-runner-"
 runner_name_prefix = server_name_prefix
+standby_server_name_prefix = f"{server_name_prefix}standby-"
+standby_runner_name_prefix = standby_server_name_prefix
+
+
+@dataclass
+class RunnerServer:
+    name: str
+    labels: set[str]
+    server_status: str = Server.STATUS_STARTING
+    status: str = "initializing"  # busy, ready
 
 
 def server_setup(
     server: BoundServer,
     setup_script: str,
     startup_script: str,
     github_token: str,
@@ -83,101 +100,58 @@
             f'GITHUB_RUNNER_TOKEN="{GITHUB_RUNNER_TOKEN}" '
             f"GITHUB_RUNNER_GROUP=Default "
             f'GITHUB_RUNNER_LABELS="{runner_labels}" '
             f"bash -s' < {startup_script}",
         )
 
 
-def create_server(
-    setup_worker_pool: ThreadPoolExecutor,
-    client: Client,
-    job: WorkflowJob,
-    labels: list[str],
-    name: str,
-    server_type: ServerType,
-    server_location: Location,
-    server_image: Image,
-    setup_script: str,
-    startup_script: str,
-    github_token: str,
-    github_repository: str,
-    ssh_key: SSHKey,
-    timeout=60,
-):
-    """Create specified number of server instances."""
-
-    with Action("Create server"):
-        response = client.servers.create(
-            name=name,
-            server_type=server_type,
-            location=server_location,
-            image=server_image,
-            ssh_keys=[ssh_key],
-        )
-        server: BoundServer = response.server
-
-    with Action(f"Waiting for server {server.name} to be ready") as action:
-        wait_ready(server=server, timeout=timeout, action=action)
-
-    setup_worker_pool.submit(
-        server_setup,
-        server=response.server,
-        setup_script=setup_script,
-        startup_script=startup_script,
-        github_token=github_token,
-        github_repository=github_repository,
-        runner_labels=",".join(labels),
-        timeout=timeout,
-    )
-
-
-def get_server_type(job: WorkflowJob, default: ServerType, label_prefix="type-"):
+def get_server_type(labels: set[str], default: ServerType, label_prefix="type-"):
     """Get server type for the specified job."""
     server_type = None
 
     if server_type is None:
-        for label in job.raw_data["labels"]:
+        for label in labels:
             if label.startswith(label_prefix):
                 server_type_name = label.split(label_prefix, 1)[-1].lower()
                 server_type = ServerType(name=server_type_name)
 
     if server_type is None:
         server_type = default
 
     return server_type
 
 
-def get_server_location(job: WorkflowJob, default: Location = None, label_prefix="in-"):
+def get_server_location(labels: set[str], default: Location = None, label_prefix="in-"):
     """Get preferred server location for the specified job.
 
     By default, location is set to `None` to avoid server type mismatching
     the location as some server types are not available at some locations.
     """
     server_location: Location = None
 
     if server_location is None:
-        for label in job.raw_data["labels"]:
+        for label in labels:
             if label.startswith(label_prefix):
                 server_location_name = label.split(label_prefix, 1)[-1].lower()
                 server_location = Location(name=server_location_name)
 
     if server_location is None and default:
         server_location = default
 
     return server_location
 
 
 def get_server_image(
-    client: Client, job: WorkflowJob, default: Image, label_prefix="image-"
+    client: Client, labels: set[str], default: Image, label_prefix="image-"
 ):
     """Get preferred server image for the specified job."""
     server_image: Image = None
 
     if server_image is None:
-        for label in job.raw_data["labels"]:
+        for label in labels:
             if label.startswith(label_prefix):
                 server_image = check_image(
                     client,
                     image_type(label.split(label_prefix, 1)[-1].lower(), separator="-"),
                 )
 
     if server_image is None:
@@ -194,33 +168,156 @@
     """
     if server_type.name.lower().startswith("ca"):
         return scripts.startup_arm64
 
     return scripts.startup_x64
 
 
+def create_server(
+    setup_worker_pool: ThreadPoolExecutor,
+    client: Client,
+    labels: set[str],
+    name: str,
+    default_server_type: ServerType,
+    default_location: Location,
+    default_image: Image,
+    scripts: Scripts,
+    github_token: str,
+    github_repository: str,
+    ssh_key: SSHKey,
+    timeout=60,
+):
+    """Create specified number of server instances."""
+
+    server_type = get_server_type(labels=labels, default=default_server_type)
+    server_location = get_server_location(labels=labels, default=default_location)
+    server_image = get_server_image(client=client, labels=labels, default=default_image)
+    startup_script = get_startup_script(server_type=server_type, scripts=scripts)
+
+    server_labels = {
+        f"github-runner-label-{i}": value for i, value in enumerate(labels)
+    }
+
+    with Action("Validating server labels"):
+        valid, error_msg = LabelValidator.validate_verbose(labels=server_labels)
+        if not valid:
+            raise ValueError(f"invalid server labels {server_labels}: {error_msg}")
+
+    with Action(f"Creating server {name} with labels {labels}"):
+        response = client.servers.create(
+            name=name,
+            server_type=server_type,
+            location=server_location,
+            image=server_image,
+            ssh_keys=[ssh_key],
+            labels=server_labels,
+        )
+        server: BoundServer = response.server
+
+    with Action(f"Waiting for server {server.name} to be ready") as action:
+        wait_ready(server=server, timeout=timeout, action=action)
+
+    setup_worker_pool.submit(
+        server_setup,
+        server=response.server,
+        setup_script=scripts.setup,
+        startup_script=startup_script,
+        github_token=github_token,
+        github_repository=github_repository,
+        runner_labels=",".join(labels),
+        timeout=timeout,
+    )
+
+
+def count_available(servers: list[RunnerServer], labels: set[str]):
+    """Return number of available servers that match
+    that match labels (subset).
+    """
+    count = 0
+
+    for runner_server in servers:
+        if runner_server.server_status == Server.STATUS_OFF:
+            continue
+        if labels.issubset(runner_server.labels):
+            if runner_server.status in ("initializing", "ready"):
+                count += 1
+
+    return count
+
+
+def count_present(servers: list[RunnerServer], labels: set[str]):
+    """Return number of present servers that match
+    that match labels (subset).
+    """
+    count = 0
+
+    for runner_server in servers:
+        if runner_server.server_status == Server.STATUS_OFF:
+            continue
+        if labels.issubset(runner_server.labels):
+            count += 1
+
+    return count
+
+
 def scale_up(
     terminate: threading.Event,
     repo: Repository,
     client: Client,
     scripts: Scripts,
     worker_pool: ThreadPoolExecutor,
     github_token: str,
     github_repository: str,
     ssh_key: SSHKey,
-    default_type: ServerType,
+    default_server_type: ServerType,
     default_location: Location,
     default_image: Image,
     interval: int,
     max_servers: int,
     max_server_ready_time: int,
     debug: bool = False,
+    standby_runners: list[StandbyRunner] = None,
 ):
     """Scale up service."""
 
+    def create_runner_server(
+        name: str,
+        labels: set[str],
+        setup_worker_pool: ThreadPoolExecutor,
+        futures: list[Future],
+        servers: list[RunnerServer],
+    ):
+        """Create new server that would provide a runner with given labels."""
+        if max_servers is not None:
+            if len(servers) >= max_servers:
+                with Action(
+                    f"Maximum number of servers {max_servers} has been reached"
+                ):
+                    raise StopIteration("maximum number of servers reached")
+
+        future = worker_pool.submit(
+            create_server,
+            setup_worker_pool=setup_worker_pool,
+            client=client,
+            labels=labels,
+            name=name,
+            default_server_type=default_server_type,
+            default_location=default_location,
+            default_image=default_image,
+            scripts=scripts,
+            github_token=github_token,
+            github_repository=github_repository,
+            ssh_key=ssh_key,
+            timeout=max_server_ready_time,
+        )
+        future.server_name = name
+
+        futures.append(future)
+        servers.append(RunnerServer(name=name, labels=labels))
+
     with ThreadPoolExecutor(
         max_workers=worker_pool._max_workers, thread_name_prefix=f"setup-worker"
     ) as setup_worker_pool:
 
         while True:
             if terminate.is_set():
                 with Action("Terminating scale up service"):
@@ -228,93 +325,123 @@
 
             try:
                 with Action("Getting workflow runs", level=logging.DEBUG):
                     workflow_runs = repo.get_workflow_runs(status="queued")
 
                 futures: list[Future] = []
 
-                with Action("Looking for jobs", level=logging.DEBUG) as action:
-                    for run in workflow_runs:
-                        for job in run.jobs():
-                            labels = job.raw_data["labels"]
-
-                            with Action("Getting list of servers", level=logging.DEBUG):
-                                servers: list[BoundServer] = client.servers.get_all()
-                                servers = [
-                                    server
-                                    for server in servers
-                                    if server.name.startswith(server_name_prefix)
+                with Action("Getting list of servers", level=logging.DEBUG):
+                    servers = [
+                        RunnerServer(
+                            name=server.name,
+                            server_status=server.status,
+                            labels=set(
+                                [
+                                    value
+                                    for name, value in server.labels.items()
+                                    if name.startswith("github-runner-label")
                                 ]
+                            ),
+                        )
+                        for server in client.servers.get_all()
+                        if server.name.startswith(server_name_prefix)
+                    ]
+
+                with Action("Getting list of self-hosted runners", level=logging.DEBUG):
+                    runners: list[SelfHostedActionsRunner] = [
+                        runner
+                        for runner in repo.get_self_hosted_runners()
+                        if runner.name.startswith(runner_name_prefix)
+                    ]
+
+                with Action("Setting status of servers based on the runner status"):
+                    for runner in runners:
+                        for server in servers:
+                            if server.name == runner.name:
+                                if runner.status == "online":
+                                    server.status = "busy" if runner.busy else "ready"
+
+                with Action("Looking for queued jobs", level=logging.DEBUG):
+                    try:
+                        for run in workflow_runs:
+                            for job in run.jobs():
+                                labels = set(job.raw_data["labels"])
+
+                                server_name = f"{server_name_prefix}{job.id}"
+
+                                if job.status != "completed":
+                                    if server_name in [
+                                        server.name for server in servers
+                                    ]:
+                                        with Action(
+                                            f"Server already exists for {job.status} {job}",
+                                            level=logging.DEBUG,
+                                        ):
+                                            continue
+
+                                    if job.status == "in_progress":
+                                        # check we job is running on a standby runner
+                                        if job.raw_data["runner_name"].startswith(
+                                            standby_runner_name_prefix
+                                        ):
+                                            continue
+
+                                        with Action(
+                                            f"Finding labels for the job from which {job} stole the runner"
+                                        ):
+                                            labels = set(
+                                                [
+                                                    label["name"]
+                                                    for label in repo.get_self_hosted_runner(
+                                                        job.raw_data["runner_id"]
+                                                    ).labels()
+                                                ]
+                                            )
 
-                            server_name = f"{server_name_prefix}{job.run_id}-{job.id}"
+                                    with Action(f"Creating new server for {job}"):
+                                        create_runner_server(
+                                            name=server_name,
+                                            labels=labels,
+                                            setup_worker_pool=setup_worker_pool,
+                                            futures=futures,
+                                            servers=servers,
+                                        )
+                    except StopIteration:
+                        pass
 
-                            if job.status != "completed":
-                                if server_name in [server.name for server in servers]:
-                                    with Action(
-                                        f"Server already exists for {job.status} {job}",
-                                        level=logging.DEBUG,
-                                    ):
-                                        continue
+                with Action("Checking standby runner pool"):
+                    for standby_runner in standby_runners:
+                        labels = set(standby_runner.labels)
+                        replenish_immediately = standby_runner.replenish_immediately
+                        if replenish_immediately:
+                            available = count_available(servers=servers, labels=labels)
+                        else:
+                            available = count_present(server=servers, labels=labels)
 
-                                if job.status == "in_progress":
+                        if available < standby_runner.count:
+                            for _ in range(standby_runner.count - available):
+                                try:
                                     with Action(
-                                        f"Finding labels for the job from which {job} stole the runner"
+                                        f"Replenishing{' immediately' if replenish_immediately else ''} standby server with {labels}"
                                     ):
-                                        labels = repo.get_self_hosted_runner(
-                                            job.raw_data["runner_id"]
-                                        ).labels()
-
-                                with Action(
-                                    f"Found job for which server was not created {job}"
-                                ):
-                                    server_type = get_server_type(
-                                        job=job, default=default_type
-                                    )
-                                    server_location = get_server_location(
-                                        job=job, default=default_location
-                                    )
-                                    server_image = get_server_image(
-                                        client=client, job=job, default=default_image
-                                    )
-                                    startup_script = get_startup_script(
-                                        server_type=server_type, scripts=scripts
-                                    )
-
-                                    if max_servers is not None:
-                                        if len(servers) >= max_servers:
-                                            with Action(
-                                                f"Maximum number of servers {max_servers} has been reached"
-                                            ):
-                                                break
-
-                                    futures.append(
-                                        worker_pool.submit(
-                                            create_server,
-                                            setup_worker_pool=setup_worker_pool,
-                                            client=client,
-                                            job=job,
+                                        create_runner_server(
+                                            name=f"{standby_server_name_prefix}{str(uuid.uuid1()).replace('-','')}",
                                             labels=labels,
-                                            name=server_name,
-                                            server_type=server_type,
-                                            server_location=server_location,
-                                            server_image=server_image,
-                                            setup_script=scripts.setup,
-                                            startup_script=startup_script,
-                                            github_token=github_token,
-                                            github_repository=github_repository,
-                                            ssh_key=ssh_key,
-                                            timeout=max_server_ready_time,
+                                            setup_worker_pool=setup_worker_pool,
+                                            futures=futures,
+                                            servers=servers,
                                         )
-                                    )
-                        else:
-                            continue
-                        break
+                                except StopIteration:
+                                    break
 
                 for future in futures:
-                    with Action("Waiting to finish creating servers", ignore_fail=True):
+                    with Action(
+                        f"Waiting to finish creating server {future.server_name}",
+                        ignore_fail=True,
+                    ):
                         future.result()
 
             except Exception as exc:
                 msg = f"❗ Error: {type(exc).__name__} {exc}"
                 if debug:
                     logger.exception(f"{msg}\n{exc}")
                 else:
```

### Comparing `testflows.github.runners-1.2.230728.1203052/testflows/github/runners/scripts/__init__.py` & `testflows.github.runners-1.3.230729.1222222/testflows/github/runners/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1203052/testflows/github/runners/scripts/deploy/__init__.py` & `testflows.github.runners-1.3.230729.1222222/testflows/github/runners/scripts/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1203052/testflows/github/runners/scripts/deploy/setup.sh` & `testflows.github.runners-1.3.230729.1222222/testflows/github/runners/scripts/deploy/setup.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1203052/testflows/github/runners/scripts/startup_arm64.sh` & `testflows.github.runners-1.3.230729.1222222/testflows/github/runners/scripts/startup_arm64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1203052/testflows/github/runners/scripts/startup_x64.sh` & `testflows.github.runners-1.3.230729.1222222/testflows/github/runners/scripts/startup_x64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1203052/testflows/github/runners/server.py` & `testflows.github.runners-1.3.230729.1222222/testflows/github/runners/server.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1203052/testflows/github/runners/service.py` & `testflows.github.runners-1.3.230729.1222222/testflows/github/runners/service.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,66 +15,66 @@
 import os
 import sys
 
 NAME = "github-runners"
 SERVICE = f"/etc/systemd/system/{NAME}.service"
 
 from .actions import Action
-from .args import check
 
 
-def command_options(args):
+def command_options(config):
     """Build service install command options not including:
 
     --github-token
     --github-repository
     --hetzner-token
     --ssh-key
     """
     command = ""
-    command += f" --workers {args.workers}"
-    command += f" --default-type {args.default_type.name}"
+    command += f" --github-token $GITHUB_TOKEN"
+    command += f" --github-repository $GITHUB_REPOSITORY"
+    command += f" --hetzner-token $HETZNER_TOKEN"
+    command += f" --config {config.config_file}" if config.config_file else ""
+    command += f" --workers {config.workers}"
+    command += f" --default-type {config.default_server_type.name}"
     command += (
-        f" --default-location {args.default_location.name}"
-        if args.default_location
+        f" --default-location {config.default_location.name}"
+        if config.default_location
         else ""
     )
-    command += f" --default-image {args.default_image.type}:{args.default_image.name or args.default_image.description}"
-    command += f" --max-runners {args.max_runners}" if args.max_runners else ""
-    command += f" --logger-config {args.logger_config}" if args.logger_config else ""
-    command += f" --setup-script {args.setup_script}" if args.setup_script else ""
+    command += f" --default-image {config.default_image.type}:{config.default_image.name or config.default_image.description}"
+    command += f" --max-runners {config.max_runners}" if config.max_runners else ""
+    command += f" --setup-script {config.setup_script}" if config.setup_script else ""
     command += (
-        f" --startup-x64-script {args.startup_x64_script}"
-        if args.startup_x64_script
+        f" --startup-x64-script {config.startup_x64_script}"
+        if config.startup_x64_script
         else ""
     )
     command += (
-        f" --startup-arm64-script {args.startup_arm64_script}"
-        if args.startup_arm64_script
+        f" --startup-arm64-script {config.startup_arm64_script}"
+        if config.startup_arm64_script
         else ""
     )
     command += (
-        f" --max-powered-off-time {args.max_powered_off_time}"
-        f" --max-idle-runner-time {args.max_idle_runner_time}"
-        f" --max-runner-registration-time {args.max_runner_registration_time}"
-        f" --max-server-ready-time {args.max_server_ready_time}"
-        f" --scale-up-interval {args.scale_up_interval}"
-        f" --scale-down-interval {args.scale_down_interval}"
+        f" --max-powered-off-time {config.max_powered_off_time}"
+        f" --max-unused-runner-time {config.max_unused_runner_time}"
+        f" --max-runner-registration-time {config.max_runner_registration_time}"
+        f" --max-server-ready-time {config.max_server_ready_time}"
+        f" --scale-up-interval {config.scale_up_interval}"
+        f" --scale-down-interval {config.scale_down_interval}"
     )
-    command += f" --debug" if args.debug else ""
+    command += f" --debug" if config.debug else ""
 
     return command
 
 
-def install(args):
+def install(args, config):
     """Install service."""
-    check(args)
-
+    config.check()
     force = args.force
-
     current_dir = os.path.dirname(__file__)
 
     with Action("Checking if service is already installed"):
         if os.path.exists(SERVICE):
             if not force:
                 raise ValueError("service has already been installed")
             with Action("Stopping service"):
@@ -87,22 +87,21 @@
             "Description=Autoscaling GitHub Actions Runners\n"
             "After=multi-user.target\n"
             "[Service]\n"
             f"User={os.getuid()}\n"
             f"Group={os.getgid()}\n"
             "Type=simple\n"
             "Restart=always\n"
-            f"Environment=GITHUB_TOKEN={args.github_token}\n"
-            f"Environment=GITHUB_REPOSITORY={args.github_repository}\n"
-            f"Environment=HETZNER_TOKEN={args.hetzner_token}\n"
+            f"Environment=GITHUB_TOKEN={config.github_token}\n"
+            f"Environment=GITHUB_REPOSITORY={config.github_repository}\n"
+            f"Environment=HETZNER_TOKEN={config.hetzner_token}\n"
             f"ExecStart={binary}"
-            f" --workers {args.workers}"
         )
-        contents += f" --ssh-key {args.ssh_key}"
-        contents += command_options(args)
+        contents += f" --ssh-key {config.ssh_key}"
+        contents += command_options(config)
         contents += "\n" "[Install]\n" "WantedBy=multi-user.target\n"
 
         os.system(f"sudo bash -c \"cat > {SERVICE}\" <<'EOF'\n{contents}\nEOF")
         os.system(f"sudo chmod 700 {SERVICE}")
 
     with Action("Reloading systemd"):
         os.system("sudo systemctl daemon-reload")
@@ -110,46 +109,44 @@
     with Action("Enabling service"):
         os.system(f"sudo systemctl enable {NAME}.service")
 
     with Action("Starting service"):
         os.system(f"sudo service {NAME} start")
 
 
-def uninstall(args):
+def uninstall(args, config=None):
     """Uninstall service."""
-    force = args.force
-
     with Action("Stopping service"):
         os.system(f"sudo service {NAME} stop")
 
     with Action("Disabling service"):
         os.system(f"sudo systemctl disable {NAME}.service")
 
     with Action(f"Removing {SERVICE}"):
         os.system(f"sudo rm -f {SERVICE}")
 
     with Action("Reloading systemd"):
         os.system("sudo systemctl daemon-reload")
 
 
-def logs(args):
+def logs(args, config=None):
     """Get service logs."""
     os.system(
         f'sudo bash -c "journalctl -u {NAME}.service'
         + (" -f" if args.follow else "")
         + ' | tee"'
     )
 
 
-def start(args):
+def start(args, config=None):
     """Start service."""
     os.system(f"sudo service {NAME} start")
 
 
-def stop(args):
+def stop(args, config=None):
     """Stop service."""
     os.system(f"sudo service {NAME} stop")
 
 
-def status(args):
+def status(args, config=None):
     """Get service status."""
     os.system(f"sudo service {NAME} status")
```

### Comparing `testflows.github.runners-1.2.230728.1203052/testflows/github/runners/shell.py` & `testflows.github.runners-1.3.230729.1222222/testflows/github/runners/shell.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1203052/testflows.github.runners.egg-info/PKG-INFO` & `testflows.github.runners-1.3.230729.1222222/README.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: testflows.github.runners
-Version: 1.2.230728.1203052
-Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
-Home-page: https://github.com/testflows/github-runners
-Author: Vitaliy Zakaznikov
-Author-email: vzakaznikov@testflows.com
-License: Apache-2.0
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.8
-Description-Content-Type: text/x-rst
-Provides-Extra: dev
-License-File: LICENSE
-
 .. image:: https://raw.githubusercontent.com/testflows/TestFlows-ArtWork/master/images/logo.png
    :width: 20%
    :align: left
    :target: https://testflows.com
    :alt: TestFlows Open-source Testing Framework
 
 ----
@@ -28,14 +11,16 @@
 :License:
    `Apache-2.0 <https://github.com/testflows/TestFlows-GitHub-Runners/blob/main/LICENSE>`_
 
 ======================================================
 Autoscaling GitHub Actions Runners Using Hetzner Cloud
 ======================================================
 
+A simple alternative to Github's `Recommended autoscaling solutions <https://docs.github.com/en/actions/hosting-your-own-runners/managing-self-hosted-runners/autoscaling-with-self-hosted-runners#recommended-autoscaling-solutions>`_.
+
 The **github-runners** service program starts and monitors queued up jobs for GitHub Actions workflows.
 When a new job is queued up, it creates a new Hetzner Cloud server instance
 that provides an ephemeral GitHub Actions runner. Each server instance is automatically
 powered off when job completes and then powered off servers are
 automatically deleted. Both **x64** and **arm64** runners are supported.
 
 :❗Warning:
@@ -47,30 +32,33 @@
 to avoid any cleanup. Server instances are not shared between any jobs.
 
 :✋ Note:
    Currently Hetzner Cloud server instances are billed on hourly basis. So a job that takes 1 min will be billed
    the same way as for a job that takes 59 minutes. Therefore, the minimal cost
    for any job is the cost of the server for 1 hour plus the cost for one public IPv4 address.
 
+----
 
-.. contents:: Read more about:
-   :backlinks: top
-   :depth: 4
+:🔍 Tip:
+   You can easily navigate this documentation page by clicking on any title to jump to the `Table of Contents`_.
+   Try it out, and remember, if you get lost just click any title!
 
 ----
 
 --------
 Features
 --------
 
-* very cost efficient on-demand runners using Hetzner Cloud
-* supports both x64 and ARM64 runners
+* cost efficient on-demand runners using `Hetzner Cloud <https://www.hetzner.com/cloud>`_
+* simple configuration, no Webhooks, no need for AWS lambdas, and no need to setup any GitHub application
 * supports specifying custom runner server types, images, and locations using job labels
-* simple configuration
-* self-contained and it can deploy, redeploy, and manage itself on a cloud instance
+* self-contained program that you can use to deploy, redeploy, and manage the service on a cloud instance
+* supports both x64 and ARM64 runners
+* supports auto-replenishable fixed standby runner pools for jobs to be picked up immediately
+* simpler alternative to what GitHub lists in `Recommended autoscaling solutions <https://docs.github.com/en/actions/hosting-your-own-runners/managing-self-hosted-runners/autoscaling-with-self-hosted-runners#recommended-autoscaling-solutions>`_
 
 ----
 
 -----------
 Limitations
 -----------
 
@@ -78,17 +66,23 @@
 
   However, you can run individual services for each repository using different Hetzner Cloud projects.
 
 * *Unique Hetzner Cloud project must be used for each repository*
 
   However, unique projects allow to easily keep track of runner costs per repository.
 
-* *Idle runner pool is not supported*
+----
 
-  Given that runner servers are created for each job, currently, idle runner pool is not supported.. 
+-------------
+Prerequisites
+-------------
+
+* Python >= 3.7
+* `Hetzner Cloud <https://www.hetzner.com/cloud>`_ account
+* GitHub API token with admin privileges to manage self-hosted runners
 
 ----
 
 ------------
 Installation
 ------------
 
@@ -308,14 +302,199 @@
 :command:
    .. code-block:: bash
 
       github-runners --setup-script ./custom_setup.sh
 
 ----
 
+--------------------------
+Specifying Standby Runners
+--------------------------
+
+You can define standby runner groups to be always ready to pick your jobs using a custom configuration file.
+
+:✋ Note:
+   Standby runner groups can only be defined using a configuration file.
+   See `Using Configuration File`_ for more details.
+
+Standby runners are always active and allow the jobs to be picked up immediately.
+
+More than one standby runner group can be specified in the **standby_runners**. Each group is defined using the **standby_runner** object
+that has *labels*, *count*, and *replenish_immediately* attributes.
+
+:schema:
+   * **standby_runners: list[standby_runner]**
+      * **labels: list[str]**
+      * **count: count**
+      * **replenish_immediately: bool**
+
+where
+
+* **labels** specifies a list of labels with which standby runners in this group should be created
+* **count** specifies how many runners should be created for the group
+* **replenish_immediately** specifies if the sandby runners should be replenished as soon as any become busy after picking up a job
+
+For example,
+
+:config.py:
+   .. code-block:: python3
+
+      from testflows.github.runners.config import *
+
+      config = Config(
+         standby_runners=[
+            standby_runner(
+                  labels=["type-cx21"],
+                  count=2,
+                  replenish_immediately=True,
+            )
+         ],
+      )
+
+----
+
+-------------------------------
+Specifying Logger Configuration
+-------------------------------
+
+You can specify custom logger configuration using a configuration file.
+
+:✋ Note:
+   Custom logger configuration can only be specified using a configuration file.
+   See `Using Configuration File`_ for more details.
+
+The logger configuration is specified by passing a dictionary as the value to the **logger_config** attribute of the `Config class`_.
+See for information about the logger configuration dictionary, see `Configuration dictionary schema <https://docs.python.org/3/library/logging.config.html#logging-config-dictschema>`_ in Python documentation.
+
+For example,
+
+:config.py:
+   .. code-block:: python3
+
+      from testflows.github.runners.config import *
+
+      config = Config(
+         logger_config = {
+             "version": 1,
+             "disable_existing_loggers": False,
+             "formatters": {
+                 "standard": {
+                     "format": "%(asctime)s %(levelname)8s %(threadName)16s %(funcName)15s %(message)s",
+                     "datefmt": "%m/%d/%Y %I:%M:%S %p",
+                 },
+             },
+             "handlers": {
+                 "default": {
+                     "level": "INFO",
+                     "formatter": "standard",
+                     "class": "logging.StreamHandler",
+                     "stream": "ext://sys.stdout",
+                 },
+             },
+             "loggers": {
+                 "testflows.github.runners": {"level": "INFO", "handlers": ["default"]},
+             },
+         }
+     )
+
+------------------------
+Using Configuration File
+------------------------
+
+Instead of passing configuration options using command line arguments, you can use
+configuration file. The configuration file is Python file that must define the **config**
+object of the `Config class`_.
+
+:✋ Note:
+   When you mix command line options and custom configuration file,
+   explicit command line options take precedence over the values that are defined
+   for the same parameters in the configuration file.
+
+:✨ Why:
+   Defining configuration file in Python instead of YAML or something else
+   has a few advantages. For example, you can edit it with
+   any Python IDE that provides a convenience of autocompletion and hints.
+
+For example,
+
+:config.py:
+
+   Simple configuration file. You can find a complete example in `examples/config.py <https://github.com/testflows/TestFlows-GitHub-Runners/blob/main/examples/config.py>`_.
+
+   .. code-block:: python3
+
+      from testflows.github.runners.config import *
+
+      config = Config(
+         github_token=os.getenv("GITHUB_TOKEN"),
+         github_repository=os.getenv("GITHUB_REPOSITORY"),
+         hetzner_token=os.getenv("HETZNER_TOKEN"),
+         default_server_type=server_type("cx11"),
+         cloud=cloud(server_name="my-github-runners-service"),
+         standby_runners=[
+            standby_runner(
+                  labels=["type-cx21"],
+                  count=2,
+                  replenish_immediately=True,
+            )
+         ],
+      )
+
+You can sanity check your configuration file by executing it directly:
+
+.. code-block:: bash
+
+   python3 config.py
+
+You can pass your custom configuration file using the *-c path, --config path** command line option.
+
+.. code-block:: bash
+
+   github-runners -c config.py
+
+Configuration Schema
+=====================
+
+The `Config class`_ has the following schema:
+
+:schema:
+   * **github_token: str**
+   * **github_repository: str**
+   * **hetzner_token: str**
+   * **ssh_key: str**
+   * **max_runners**
+   * **default_image: image**
+   * **default_server_type: server_type**
+   * **default_location: location**
+   * **workers: count**
+   * **setup_script: path**
+   * **startup_x64_script: path**
+   * **startup_arm64_script: path**
+   * **max_powered_off_time: count**
+   * **max_unused_runner_time: count**
+   * **max_runner_registration_time: count**
+   * **max_server_ready_time: count**
+   * **scale_up_interval: count**
+   * **scale_down_interval: count**
+   * **debug: bool**
+   * **logger_config: dict**
+   * **cloud: cloud**
+      * **server_name: str**
+      * **deploy: deploy**
+         * **server_type: server_type**
+         * **image: image**
+         * **location: location**
+         * **setup_script: path**
+   * **standby_runners: list[standby_runner]**
+      * **labels: list[str]**
+      * **count: count**
+      * **replenish_immediately: bool**
+
+----
+
 -------
 SSH Key
 -------
 
 All server instances that are created are accessed via SSH using the **ssh** utility and therefore you must provide a valid SSH key
 using the **--ssh-key** option. If the **--ssh-key** option is no specified, then the *~/.ssh/id_rsa.pub* default key path will be used.
 
@@ -388,15 +567,15 @@
       User=1000
       Group=1000
       Type=simple
       Restart=always
       Environment=GITHUB_TOKEN=ghp_...
       Environment=GITHUB_REPOSITORY=testflows/github-runners
       Environment=HETZNER_TOKEN=GJ..
-      ExecStart=/home/user/.local/lib/python3.10/site-packages/testflows/github/runners/bin/github-runners --workers 10 --max-powered-off-time 20 --max-idle-runner-time 120 --max-runner-registration-time 60 --scale-up-interval 10 --scale-down-interval 10
+      ExecStart=/home/user/.local/lib/python3.10/site-packages/testflows/github/runners/bin/github-runners --workers 10 --max-powered-off-time 20 --max-unused-runner-time 120 --max-runner-registration-time 60 --scale-up-interval 10 --scale-down-interval 10
       [Install]
       WantedBy=multi-user.target
 
 ----
 
 Modifying Program Options
 =========================
@@ -431,15 +610,15 @@
            Loaded: loaded (/etc/systemd/system/github-runners.service; enabled; vendor preset: enabled)
            Active: active (running) since Mon 2023-07-24 14:38:33 EDT; 1h 31min ago
          Main PID: 66188 (python3)
             Tasks: 3 (limit: 37566)
            Memory: 28.8M
               CPU: 8.274s
            CGroup: /system.slice/github-runners.service
-                   └─66188 python3 /usr/local/bin/github-runners --workers 10 --max-powered-off-time 20 --max-idle-runner-time 120 --max->
+                   └─66188 python3 /usr/local/bin/github-runners --workers 10 --max-powered-off-time 20 --max-unused-runner-time 120 --max->
 
       Jul 24 14:38:33 user-node systemd[1]: Started Autoscaling GitHub Actions Runners.
       Jul 24 14:38:33 user-node github-runners[66188]: 07/24/2023 02:38:33 PM   INFO MainThread            main 🍀 Logging in to Hetzner >
       Jul 24 14:38:33 user-node github-runners[66188]: 07/24/2023 02:38:33 PM   INFO MainThread            main 🍀 Logging in to GitHub
       Jul 24 14:38:33 user-node github-runners[66188]: 07/24/2023 02:38:33 PM   INFO MainThread            main 🍀 Getting repository vza>
       Jul 24 14:38:33 user-node github-runners[66188]: 07/24/2023 02:38:33 PM   INFO MainThread            main 🍀 Creating scale up serv>
       Jul 24 14:38:33 user-node github-runners[66188]: 07/24/2023 02:38:33 PM   INFO MainThread            main 🍀 Creating scale down se>
@@ -845,16 +1024,16 @@
 For each such job, a corresponding Hetzner Cloud server instance is created with the following name:
 
 ::
 
    github-runner-{job.run_id}-{job.id}
 
 The server is configured using default **setup** and **startup** scripts. The runner name is set
-to be the same as the server name so that servers can be deleted for any idle runner that for some reason
-does not pick up a job for which it was created within the **max-idle-runner-time** period.
+to be the same as the server name so that servers can be deleted for any unused runner that for some reason
+does not pick up a job for which it was created within the **max-unused-runner-time** period.
 
 :Note:
    Given that the server name is fixed and specific for each *job.run_id, job.id* tuple, if multiple `github-runners` are running in parallel then
    only 1 server will be created for a given `job` and any other attempts to create a server with the same name will be rejected
    by the Hetzner Cloud.
 
 Also,
@@ -1000,21 +1179,21 @@
 
 The program scales down runners by first cleaning up powered off servers. The scale down service relies on the fact
 that the `startup <#the-start-up-script>`_ script starts an ephemeral runner which will pick up only 1 job and then will power itself off after the job is complete.
 
 The powered off servers are deleted after the **max-powered-off-time** interval which
 can be specified using the **--max-powered-off-time** option which by default is set to *20* sec.
 
-Idle Runners
-============
+Unused Runners
+==============
 
-The scale down service also monitors all the runners that have **idle** status and tries to delete any servers associated with such
-runners if the runner is **idle** for more than the **max-idle-runner-time** period. This is needed in case a runner never gets a job
+The scale down service also monitors all the runners that have **unused** status and tries to delete any servers associated with such
+runners if the runner is **unused** for more than the **max-unused-runner-time** period. This is needed in case a runner never gets a job
 assigned to it and the server will stay in the power on state. This cycle relies on the fact that the runner's name
-is the same as server's name. The **max-idle-runner-time** can be specified using the **--max-idle-runner-time** option which by default
+is the same as server's name. The **max-unused-runner-time** can be specified using the **--max-unused-runner-time** option which by default
 is set to *120* sec.
 
 Zombie Servers
 ==============
 
 The scale down service will delete any zombie servers. A zombie server is defined as as any server that fails to register its runner within
 the **max-runner-registration-time**. The **max-runner-registration-time** can be specified using the **--max-runner-registration-time** option
@@ -1038,15 +1217,15 @@
 :The *./run.sh* Command Fails:
    The server will be powered off by the **startup** script and will be deleted by the scale down service.
 
 :Creating Server For Queued Job Fails:
    If creation of the server fails for some reason then the scale up service will retry the operation in the next interval as the job's status will remain **queued**.
 
 :Runner Never Gets a Job Assigned:
-   If the runner never gets a job assigned, then the scale down service will remove the runner and delete its server after the **max-idle-runner-time** period.
+   If the runner never gets a job assigned, then the scale down service will remove the runner and delete its server after the **max-unused-runner-time** period.
 
 :Runner Created With a Mismatched Labels:
    The behavior will be the same as for the **Runner Never Gets a Job Assigned** case above.
 
 ----
 
 ---------------
@@ -1060,14 +1239,17 @@
 
 * **-v, --version**
   show program's version number and exit
 
 * **--license**
   show program's license and exit
 
+* **-c path, --config path**
+  program configuration file
+
 * **--github-token GITHUB_TOKEN**
   GitHub token, default: *$GITHUB_TOKEN* environment variable
 
 * **--github-repository GITHUB_REPOSITORY**
   GitHub repository, default: *$GITHUB_REPOSITORY* environment variable
 
 * **--hetzner-token HETZNER_TOKEN**
@@ -1089,31 +1271,28 @@
 
 * **-m count, --max-runners count**
   maximum number of active runners, default: *10*
 
 * **-w count, --workers count**
   number of concurrent workers, default: *10*
 
-* **--logger-config path**
-  custom logger configuration file
-
 * **--setup-script path**
   path to custom server setup script
 
 * **--startup-x64-script path**
   path to custom server startup script
 
 * **--startup-arm64-script path**
   path to custom ARM64 server startup script
 
 * **--max-powered-off-time sec**
   maximum time after which a powered off server is deleted, default: *60* sec
 
-* **--max-idle-runner-time sec**
-  maximum time after which an idle runner is removed and its server deleted, default: *120* sec
+* **--max-unused-runner-time sec**
+  maximum time after which an unused runner is removed and its server deleted, default: *120* sec
 
 * **--max-runner-registration-time**
   maximum time after which the server will be deleted if its runner is not registered with GitHub, default: *120* sec
 
 * **--max-server-ready-time sec**
   maximum time to wait for the server to be in the running state, default: *120* sec
 
@@ -1225,7 +1404,17 @@
           follow logs journal, default: *False*
 
       * **start**
         start service
 
       * **stop**
         stop service
+
+-----------------
+Table of Contents
+-----------------
+
+.. contents:: Index:
+   :backlinks: top
+   :depth: 4
+
+.. _Config class: https://github.com/testflows/TestFlows-GitHub-Runners/blob/main/testflows/github/runners/config.py#L45
```

### Comparing `testflows.github.runners-1.2.230728.1203052/testflows.github.runners.egg-info/SOURCES.txt` & `testflows.github.runners-1.3.230729.1222222/testflows.github.runners.egg-info/SOURCES.txt`

 * *Files identical despite different names*

