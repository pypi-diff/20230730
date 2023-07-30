# Comparing `tmp/dcicutils-7.6.0.2b7.tar.gz` & `tmp/dcicutils-7.6.0.2b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcicutils-7.6.0.2b7.tar", max compression
+gzip compressed data, was "dcicutils-7.6.0.2b8.tar", max compression
```

## Comparing `dcicutils-7.6.0.2b7.tar` & `dcicutils-7.6.0.2b8.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0     1103 2023-07-28 21:14:31.449372 dcicutils-7.6.0.2b7/LICENSE.txt
--rw-r--r--   0        0        0     1166 2023-07-28 21:14:31.449372 dcicutils-7.6.0.2b7/README.rst
--rw-r--r--   0        0        0        0 2023-07-28 21:14:31.449372 dcicutils-7.6.0.2b7/dcicutils/__init__.py
--rw-r--r--   0        0        0     5115 2023-07-28 21:14:31.449372 dcicutils-7.6.0.2b7/dcicutils/base.py
--rwxr-xr-x   0        0        0    51434 2023-07-28 21:14:31.449372 dcicutils-7.6.0.2b7/dcicutils/beanstalk_utils.py
--rw-r--r--   0        0        0    13786 2023-07-28 21:14:31.449372 dcicutils-7.6.0.2b7/dcicutils/cloudformation_utils.py
--rw-r--r--   0        0        0     1155 2023-07-28 21:14:31.449372 dcicutils-7.6.0.2b7/dcicutils/codebuild_utils.py
--rw-r--r--   0        0        0    15285 2023-07-28 21:14:31.449372 dcicutils-7.6.0.2b7/dcicutils/command_utils.py
--rw-r--r--   0        0        0     3763 2023-07-28 21:14:31.449372 dcicutils-7.6.0.2b7/dcicutils/common.py
--rw-r--r--   0        0        0     2015 2023-07-28 21:14:31.449372 dcicutils-7.6.0.2b7/dcicutils/contribution_scripts.py
--rw-r--r--   0        0        0    23914 2023-07-28 21:14:31.449372 dcicutils-7.6.0.2b7/dcicutils/contribution_utils.py
--rw-r--r--   0        0        0    11113 2023-07-28 21:14:31.449372 dcicutils-7.6.0.2b7/dcicutils/creds_utils.py
--rw-r--r--   0        0        0     3098 2023-07-28 21:14:31.449372 dcicutils-7.6.0.2b7/dcicutils/data_utils.py
--rw-r--r--   0        0        0    68885 2023-07-28 21:14:31.449372 dcicutils-7.6.0.2b7/dcicutils/deployment_utils.py
--rw-r--r--   0        0        0     8118 2023-07-28 21:14:31.449372 dcicutils-7.6.0.2b7/dcicutils/diff_utils.py
--rw-r--r--   0        0        0     1747 2023-07-28 21:14:31.449372 dcicutils-7.6.0.2b7/dcicutils/docker_utils.py
--rw-r--r--   0        0        0    19474 2023-07-28 21:14:31.449372 dcicutils-7.6.0.2b7/dcicutils/ecr_scripts.py
--rw-r--r--   0        0        0    13079 2023-07-28 21:14:31.449372 dcicutils-7.6.0.2b7/dcicutils/ecr_utils.py
--rw-r--r--   0        0        0     3590 2023-07-28 21:14:31.449372 dcicutils-7.6.0.2b7/dcicutils/ecs_utils.py
--rw-r--r--   0        0        0     6356 2023-07-28 21:14:31.449372 dcicutils-7.6.0.2b7/dcicutils/env_base.py
--rw-r--r--   0        0        0     9444 2023-07-28 21:14:31.449372 dcicutils-7.6.0.2b7/dcicutils/env_manager.py
--rw-r--r--   0        0        0     3909 2023-07-28 21:14:31.449372 dcicutils-7.6.0.2b7/dcicutils/env_scripts.py
--rw-r--r--   0        0        0    46970 2023-07-28 21:14:31.449372 dcicutils-7.6.0.2b7/dcicutils/env_utils.py
--rw-r--r--   0        0        0    29032 2023-07-28 21:14:31.449372 dcicutils-7.6.0.2b7/dcicutils/env_utils_legacy.py
--rw-r--r--   0        0        0     7541 2023-07-28 21:14:31.449372 dcicutils-7.6.0.2b7/dcicutils/es_utils.py
--rw-r--r--   0        0        0     9931 2023-07-28 21:14:31.449372 dcicutils-7.6.0.2b7/dcicutils/exceptions.py
--rw-r--r--   0        0        0    36918 2023-07-28 21:14:31.449372 dcicutils-7.6.0.2b7/dcicutils/ff_mocks.py
--rw-r--r--   0        0        0    66453 2023-07-28 21:14:31.449372 dcicutils-7.6.0.2b7/dcicutils/ff_utils.py
--rw-r--r--   0        0        0    10026 2023-07-28 21:14:31.449372 dcicutils-7.6.0.2b7/dcicutils/function_cache_decorator.py
--rw-r--r--   0        0        0    33704 2023-07-28 21:14:31.453372 dcicutils-7.6.0.2b7/dcicutils/glacier_utils.py
--rw-r--r--   0        0        0    11502 2023-07-28 21:14:31.453372 dcicutils-7.6.0.2b7/dcicutils/jh_utils.py
--rw-r--r--   0        0        0    16225 2023-07-28 21:14:31.453372 dcicutils-7.6.0.2b7/dcicutils/kibana/dashboards.json
--rw-r--r--   0        0        0     2164 2023-07-28 21:14:31.453372 dcicutils-7.6.0.2b7/dcicutils/kibana/readme.md
--rw-r--r--   0        0        0    27797 2023-07-28 21:14:31.453372 dcicutils-7.6.0.2b7/dcicutils/lang_utils.py
--rw-r--r--   0        0        0    38497 2023-07-28 21:14:31.453372 dcicutils-7.6.0.2b7/dcicutils/license_utils.py
--rw-r--r--   0        0        0    10883 2023-07-28 21:14:31.453372 dcicutils-7.6.0.2b7/dcicutils/log_utils.py
--rw-r--r--   0        0        0    90749 2023-07-28 21:14:31.453372 dcicutils-7.6.0.2b7/dcicutils/misc_utils.py
--rw-r--r--   0        0        0     5963 2023-07-28 21:14:31.453372 dcicutils-7.6.0.2b7/dcicutils/obfuscation_utils.py
--rw-r--r--   0        0        0     1017 2023-07-28 21:14:31.453372 dcicutils-7.6.0.2b7/dcicutils/opensearch_utils.py
--rw-r--r--   0        0        0    30631 2023-07-28 21:14:31.453372 dcicutils-7.6.0.2b7/dcicutils/project_utils.py
--rw-r--r--   0        0        0    20511 2023-07-28 21:14:31.453372 dcicutils-7.6.0.2b7/dcicutils/qa_checkers.py
--rw-r--r--   0        0        0   156269 2023-07-28 21:14:31.453372 dcicutils-7.6.0.2b7/dcicutils/qa_utils.py
--rw-r--r--   0        0        0     6509 2023-07-28 21:14:31.453372 dcicutils-7.6.0.2b7/dcicutils/redis_tools.py
--rw-r--r--   0        0        0     6462 2023-07-28 21:14:31.453372 dcicutils-7.6.0.2b7/dcicutils/redis_utils.py
--rw-r--r--   0        0        0    28852 2023-07-28 21:14:31.453372 dcicutils-7.6.0.2b7/dcicutils/s3_utils.py
--rw-r--r--   0        0        0    13576 2023-07-28 21:14:31.453372 dcicutils-7.6.0.2b7/dcicutils/scripts/publish_to_pypi.py
--rw-r--r--   0        0        0    19745 2023-07-28 21:14:31.453372 dcicutils-7.6.0.2b7/dcicutils/secrets_utils.py
--rw-r--r--   0        0        0    22961 2023-07-28 21:14:31.453372 dcicutils-7.6.0.2b7/dcicutils/snapshot_utils.py
--rw-r--r--   0        0        0     9707 2023-07-28 21:14:31.453372 dcicutils-7.6.0.2b7/dcicutils/ssl_certificate_utils.py
--rw-r--r--   0        0        0     8082 2023-07-28 21:14:31.453372 dcicutils-7.6.0.2b7/dcicutils/task_utils.py
--rw-r--r--   0        0        0     1769 2023-07-28 21:14:31.453372 dcicutils-7.6.0.2b7/dcicutils/trace_utils.py
--rw-r--r--   0        0        0     4387 2023-07-28 21:14:31.457372 dcicutils-7.6.0.2b7/pyproject.toml
--rw-r--r--   0        0        0     2762 1970-01-01 00:00:00.000000 dcicutils-7.6.0.2b7/setup.py
--rw-r--r--   0        0        0     3002 1970-01-01 00:00:00.000000 dcicutils-7.6.0.2b7/PKG-INFO
+-rw-r--r--   0        0        0     1103 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/LICENSE.txt
+-rw-r--r--   0        0        0     1166 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/README.rst
+-rw-r--r--   0        0        0        0 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/dcicutils/__init__.py
+-rw-r--r--   0        0        0     5115 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/dcicutils/base.py
+-rwxr-xr-x   0        0        0    51434 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/dcicutils/beanstalk_utils.py
+-rw-r--r--   0        0        0    13786 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/dcicutils/cloudformation_utils.py
+-rw-r--r--   0        0        0     1155 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/dcicutils/codebuild_utils.py
+-rw-r--r--   0        0        0    15285 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/dcicutils/command_utils.py
+-rw-r--r--   0        0        0     3763 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/dcicutils/common.py
+-rw-r--r--   0        0        0     2015 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/dcicutils/contribution_scripts.py
+-rw-r--r--   0        0        0    25653 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/dcicutils/contribution_utils.py
+-rw-r--r--   0        0        0    11113 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/dcicutils/creds_utils.py
+-rw-r--r--   0        0        0     3098 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/dcicutils/data_utils.py
+-rw-r--r--   0        0        0    68885 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/dcicutils/deployment_utils.py
+-rw-r--r--   0        0        0     8118 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/dcicutils/diff_utils.py
+-rw-r--r--   0        0        0     1747 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/dcicutils/docker_utils.py
+-rw-r--r--   0        0        0    19474 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/dcicutils/ecr_scripts.py
+-rw-r--r--   0        0        0    13079 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/dcicutils/ecr_utils.py
+-rw-r--r--   0        0        0     3590 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/dcicutils/ecs_utils.py
+-rw-r--r--   0        0        0     6356 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/dcicutils/env_base.py
+-rw-r--r--   0        0        0     9444 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/dcicutils/env_manager.py
+-rw-r--r--   0        0        0     3909 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/dcicutils/env_scripts.py
+-rw-r--r--   0        0        0    46970 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/dcicutils/env_utils.py
+-rw-r--r--   0        0        0    29032 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/dcicutils/env_utils_legacy.py
+-rw-r--r--   0        0        0     7541 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/dcicutils/es_utils.py
+-rw-r--r--   0        0        0     9931 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/dcicutils/exceptions.py
+-rw-r--r--   0        0        0    36918 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/dcicutils/ff_mocks.py
+-rw-r--r--   0        0        0    66453 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/dcicutils/ff_utils.py
+-rw-r--r--   0        0        0    10026 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/dcicutils/function_cache_decorator.py
+-rw-r--r--   0        0        0    33704 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/dcicutils/glacier_utils.py
+-rw-r--r--   0        0        0    11502 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/dcicutils/jh_utils.py
+-rw-r--r--   0        0        0    16225 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/dcicutils/kibana/dashboards.json
+-rw-r--r--   0        0        0     2164 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/dcicutils/kibana/readme.md
+-rw-r--r--   0        0        0    27797 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/dcicutils/lang_utils.py
+-rw-r--r--   0        0        0    38497 2023-07-30 13:17:35.703076 dcicutils-7.6.0.2b8/dcicutils/license_utils.py
+-rw-r--r--   0        0        0    10883 2023-07-30 13:17:35.703076 dcicutils-7.6.0.2b8/dcicutils/log_utils.py
+-rw-r--r--   0        0        0    90749 2023-07-30 13:17:35.703076 dcicutils-7.6.0.2b8/dcicutils/misc_utils.py
+-rw-r--r--   0        0        0     5963 2023-07-30 13:17:35.703076 dcicutils-7.6.0.2b8/dcicutils/obfuscation_utils.py
+-rw-r--r--   0        0        0     1017 2023-07-30 13:17:35.703076 dcicutils-7.6.0.2b8/dcicutils/opensearch_utils.py
+-rw-r--r--   0        0        0    30631 2023-07-30 13:17:35.703076 dcicutils-7.6.0.2b8/dcicutils/project_utils.py
+-rw-r--r--   0        0        0    20511 2023-07-30 13:17:35.703076 dcicutils-7.6.0.2b8/dcicutils/qa_checkers.py
+-rw-r--r--   0        0        0   156269 2023-07-30 13:17:35.703076 dcicutils-7.6.0.2b8/dcicutils/qa_utils.py
+-rw-r--r--   0        0        0     6509 2023-07-30 13:17:35.703076 dcicutils-7.6.0.2b8/dcicutils/redis_tools.py
+-rw-r--r--   0        0        0     6462 2023-07-30 13:17:35.703076 dcicutils-7.6.0.2b8/dcicutils/redis_utils.py
+-rw-r--r--   0        0        0    28852 2023-07-30 13:17:35.703076 dcicutils-7.6.0.2b8/dcicutils/s3_utils.py
+-rw-r--r--   0        0        0    13576 2023-07-30 13:17:35.703076 dcicutils-7.6.0.2b8/dcicutils/scripts/publish_to_pypi.py
+-rw-r--r--   0        0        0    19745 2023-07-30 13:17:35.703076 dcicutils-7.6.0.2b8/dcicutils/secrets_utils.py
+-rw-r--r--   0        0        0    22961 2023-07-30 13:17:35.703076 dcicutils-7.6.0.2b8/dcicutils/snapshot_utils.py
+-rw-r--r--   0        0        0     9707 2023-07-30 13:17:35.703076 dcicutils-7.6.0.2b8/dcicutils/ssl_certificate_utils.py
+-rw-r--r--   0        0        0     8082 2023-07-30 13:17:35.703076 dcicutils-7.6.0.2b8/dcicutils/task_utils.py
+-rw-r--r--   0        0        0     1769 2023-07-30 13:17:35.703076 dcicutils-7.6.0.2b8/dcicutils/trace_utils.py
+-rw-r--r--   0        0        0     4387 2023-07-30 13:17:35.703076 dcicutils-7.6.0.2b8/pyproject.toml
+-rw-r--r--   0        0        0     2762 1970-01-01 00:00:00.000000 dcicutils-7.6.0.2b8/setup.py
+-rw-r--r--   0        0        0     3002 1970-01-01 00:00:00.000000 dcicutils-7.6.0.2b8/PKG-INFO
```

### Comparing `dcicutils-7.6.0.2b7/LICENSE.txt` & `dcicutils-7.6.0.2b8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b7/README.rst` & `dcicutils-7.6.0.2b8/README.rst`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b7/dcicutils/base.py` & `dcicutils-7.6.0.2b8/dcicutils/base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b7/dcicutils/beanstalk_utils.py` & `dcicutils-7.6.0.2b8/dcicutils/beanstalk_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b7/dcicutils/cloudformation_utils.py` & `dcicutils-7.6.0.2b8/dcicutils/cloudformation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b7/dcicutils/codebuild_utils.py` & `dcicutils-7.6.0.2b8/dcicutils/codebuild_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b7/dcicutils/command_utils.py` & `dcicutils-7.6.0.2b8/dcicutils/command_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b7/dcicutils/common.py` & `dcicutils-7.6.0.2b8/dcicutils/common.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b7/dcicutils/contribution_scripts.py` & `dcicutils-7.6.0.2b8/dcicutils/contribution_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b7/dcicutils/contribution_utils.py` & `dcicutils-7.6.0.2b8/dcicutils/contribution_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import datetime
 import git
 import io
 import json
 import os
 import re
+import warnings
 
 from collections import defaultdict
 from dcicutils.diff_utils import DiffManager
 from dcicutils.lang_utils import n_of
 from dcicutils.misc_utils import PRINT, ignored, environ_bool
 from typing import Dict, List, Optional, Set, Type
 
@@ -30,17 +31,21 @@
     def git_commits(cls, repo_name) -> List[git.Commit]:
         repo = cls.find_repo(repo_name)
         commit: git.Commit
         for commit in repo.iter_commits():
             yield cls.json_for_commit(commit)
 
     @classmethod
+    def author_name(cls, actor: git.Actor) -> str:
+        return actor.name or actor.email.split('@')[0]
+
+    @classmethod
     def json_for_actor(cls, actor: git.Actor) -> Dict:
         return {
-            "name": actor.name,
+            "name": cls.author_name(actor),
             "email": actor.email,
         }
 
     @classmethod
     def json_for_commit(cls, commit: git.Commit) -> Dict:
         return {
             'commit': commit.hexsha,
@@ -51,15 +56,15 @@
         }
 
 
 class Contributor:
 
     @classmethod
     def create(cls, *, author: git.Actor) -> 'Contributor':
-        return Contributor(email=author.email, name=author.name)
+        return Contributor(email=author.email, name=GitAnalysis.author_name(author))
 
     def __init__(self, *, email: Optional[str] = None, name: Optional[str] = None,
                  emails: Optional[Set[str]] = None, names: Optional[Set[str]] = None,
                  primary_name: Optional[str] = None):
         # Both email and name are required keyword arguments, though name is allowed to be None,
         # even though email is not. The primary_name is not required, and defaults to None, so will
         # be heuristically computed based on available names.
@@ -111,22 +116,20 @@
         data = {
             "emails": sorted(self.emails),
             "names": sorted(self.names),
         }
         return data
 
     @classmethod
-    def from_dict(cls, data: Dict, *, key: Optional[str] = None) -> 'Contributor':
+    def from_dict(cls, data: Dict) -> 'Contributor':
         emails = data["emails"]
         names = data["names"]
         contributor = Contributor(email=emails[0], name=names[0])
         contributor.emails = set(emails)
         contributor.names = set(names)
-        if key:
-            contributor.set_primary_name(key)
         return contributor
 
     @classmethod
     def name_variation_spelling_sort_key(cls, name):
         return (
             ' ' in name,  # we prefer names like 'jane doe' over jdoe123
             len(name),  # longer names are usually more formal; william smith vs will smith
@@ -138,28 +141,25 @@
 
 
 class BasicContributions(GitAnalysis):
 
     VERBOSE = False
 
     def __init__(self, *, repo: Optional[str] = None,
-                 exclude_fork: Optional[str] = None,
                  verbose: Optional[bool] = None):
         self.email_timestamps: Dict[str, datetime.datetime] = {}
         self.name_timestamps: Dict[str, datetime.datetime] = {}
-        self.exclude_fork: Optional[str] = exclude_fork
         if not repo:
             # Doing it this way gets around an ambiguity about '/foo/' vs '/foo' since both
             # os.path.join('/foo/', 'bar') and os.path.join('/foo', 'bar') yield '/foo/bar',
             # and from there one can do os.path.basename(os.path.dirname(...)) to get 'foo' out.
             cache_file = os.path.join(os.path.abspath(os.path.curdir), self.CONTRIBUTORS_CACHE_FILE)
             dir = os.path.dirname(cache_file)
             repo = os.path.basename(dir)
         self.repo: str = repo
-        self.excluded_contributions = None
         self.forked_at: Optional[datetime.datetime] = None
         self.contributors_by_name: Optional[ContributorIndex] = None
         self.contributors_by_email: Optional[ContributorIndex] = None
         self.pre_fork_contributors_by_email: Optional[ContributorIndex] = None
         self.pre_fork_contributors_by_name: Optional[ContributorIndex] = None
         self.loaded_contributor_data = None
         self.cache_discrepancies: Optional[dict] = None
@@ -205,33 +205,42 @@
         else:
             return {
                 key: contributor.as_dict()
                 for key, contributor in contributor_index.items()
             }
 
     @classmethod
-    def contributor_values_as_objects(cls, contributor_index: Optional[Dict]):
+    def contributor_values_as_objects(cls, contributor_index: Optional[Dict]) -> Optional[ContributorIndex]:
         if contributor_index is None:
             return None
         else:
             return {
-                key: Contributor.from_dict(value, key=key)
+                key: Contributor.from_dict(value)
                 for key, value in contributor_index.items()
             }
 
     def checkpoint_state(self):
         return self.as_dict()
 
     def as_dict(self):
-        data = {
-            "forked_at": self.forked_at.isoformat() if self.forked_at else None,
-            "excluded_fork": self.exclude_fork,
-            "pre_fork_contributors_by_name": self.contributor_values_as_dicts(self.pre_fork_contributors_by_name),
-            "contributors_by_name": self.contributor_values_as_dicts(self.contributors_by_name),
-        }
+
+        data = {}
+
+        forked_at = self.forked_at.isoformat() if self.forked_at else None
+        if forked_at is not None:
+            data["forked_at"] = forked_at
+
+        pre_fork_contributors_by_name = self.contributor_values_as_dicts(self.pre_fork_contributors_by_name)
+        if pre_fork_contributors_by_name is not None:
+            data["pre_fork_contributors_by_name"] = pre_fork_contributors_by_name
+
+        contributors_by_name = self.contributor_values_as_dicts(self.contributors_by_name)
+        if contributors_by_name is not None:
+            data["contributors_by_name"] = contributors_by_name
+
         return data
 
     def save_contributor_data(self, filename: Optional[str] = None) -> str:
         if filename is None:
             filename = self.contributors_json_file()
         with io.open(filename, 'w') as fp:
             PRINT(json.dumps(self.as_dict(), indent=2), file=fp)
@@ -240,14 +249,37 @@
     def repo_contributor_names(self, with_email=False):
         for name, contributor in self.contributors_by_name.items():
             if with_email:
                 yield f"{name} ({', '.join([self.pretty_email(email) for email in contributor.emails])})"
             else:
                 yield name
 
+    def show_repo_contributors(self, analyze_discrepancies: bool = True, with_email: bool = True,
+                               error_class: Optional[Type[BaseException]] = None):
+        for author_name in self.repo_contributor_names(with_email=with_email):
+            PRINT(author_name)
+        if analyze_discrepancies:
+            file = self.existing_contributors_json_file()
+            if not file:
+                message = f"Need to create a {self.CONTRIBUTORS_CACHE_FILE} file for {self.repo}."
+                if error_class:
+                    raise error_class(message)
+                else:
+                    PRINT(message)
+            elif self.cache_discrepancies:
+                message = "There are contributor cache discrepancies."
+                PRINT(f"===== {message.rstrip('.').upper()} =====")
+                for action, items in self.cache_discrepancies.items():
+                    action: str
+                    PRINT(f"{action.replace('_', ' ').title()}:")
+                    for item in items:
+                        PRINT(f" * {item}")
+                if error_class:
+                    raise error_class(message)
+
     @classmethod
     def pretty_email(cls, email):
         m = GITHUB_USER_REGEXP.match(email)
         if m:
             user_name = m.group(1)
             return f"{user_name}@github"
         else:
@@ -259,192 +291,261 @@
             with io.open(filename, 'r') as fp:
                 data = json.load(fp)
         except Exception:
             PRINT(f"Error while reading data from {filename!r}.")
             raise
         return data
 
+    @classmethod
+    def contributor_index_by_primary_name(cls, contributors_by_name: ContributorIndex) -> ContributorIndex:
+        """
+        Given a by-name contributor index:
+
+        * Makes sure that all contributors have only one name, indexed by the contributor's primary name
+        * Sorts the resulting index using a case-insensitive alphabetic sort
+
+        and then returns the result.
+
+        :param contributors_by_name: a contributor index indexed by human name
+        :return: a contributor index
+        """
+        seen = set()
+        nicknames_seen = set()
+        contributor_items = []
+        contributors = {}
+        for name, contributor in contributors_by_name.items():
+            if contributor not in seen:
+                for nickname in contributor.names:
+                    if nickname in nicknames_seen:
+                        raise Exception(f"Name improperly shared between {contributor}"
+                                        f" and {contributors_by_name[nickname]}")
+                    nicknames_seen.add(nickname)
+                contributor_items.append((contributor.primary_name, contributor))
+                seen.add(contributor)
+        for name, contributor in sorted(contributor_items,
+                                        # Having selected the longest names, now sort names ignoring case
+                                        key=lambda pair: pair[0].lower()):
+            contributors[name] = contributor
+        return contributors
+
+    @classmethod
+    def by_email_from_by_name(cls, contributors_by_name_json):
+        result = {}
+        seen = set()
+        for name_key, entry in contributors_by_name_json.items():
+            ignored(name_key)
+            seen_key = id(entry)
+            if seen_key in seen:
+                continue
+            seen.add(seen_key)
+            for email in entry.get("emails", []) if isinstance(entry, dict) else entry.emails:
+                if result.get(email):
+                    raise Exception(f"email address {email} is used more than once.")
+                result[email] = entry
+        return result
+
+    @classmethod
+    def set_keys_as_primary_names(cls, contributors_by_name: Optional[ContributorIndex]):
+        if contributors_by_name is not None:
+            for key, contributor in contributors_by_name.items():
+                contributor.set_primary_name(key)
+
 
 class Contributions(BasicContributions):
 
     def __init__(self, *, repo: Optional[str] = None,
                  exclude_fork: Optional[str] = None,
                  verbose: Optional[bool] = None):
-        super().__init__(repo=repo, exclude_fork=exclude_fork, verbose=verbose)
+        super().__init__(repo=repo, verbose=verbose)
         existing_contributor_data_file = self.existing_contributors_json_file()
         if existing_contributor_data_file:
             # This will set .loaded_contributor_data and other values from CONTRIBUTORS.json
             self.load_contributors_from_json_file_cache(existing_contributor_data_file)
 
-        if exclude_fork and not self.excluded_contributions:
-            self.excluded_contributions = Contributions(repo=exclude_fork)
         checkpoint1 = self.checkpoint_state()
-        self.reconcile_contributors_with_github_log()
+        self.reconcile_contributors_with_github_log(exclude_fork=exclude_fork)
         checkpoint2 = self.checkpoint_state()
 
         def list_to_dict_normalizer(*, label, item):
             ignored(label)
             if isinstance(item, list):
                 return {elem: elem for elem in item}
             else:
                 return item
 
         if existing_contributor_data_file:
             diff_manager = DiffManager(label="contributors")
             contributors1 = checkpoint1['contributors_by_name']
             contributors2 = checkpoint2['contributors_by_name']
             diffs = diff_manager.diffs(contributors1, contributors2, normalizer=list_to_dict_normalizer)
-            added = diffs.get('added')
-            changed = diffs.get('changed')
-            removed = diffs.get('removed')
-            self.cache_discrepancies = cache_discrepancies = {}
-            if added:
-                cache_discrepancies['to_add'] = added
-            if changed:
-                cache_discrepancies['to_change'] = changed
-            if removed:
-                cache_discrepancies['to_remove'] = removed
+            self.cache_discrepancies = self.resummarize_discrepancies(diffs)
+
+    @classmethod
+    def resummarize_discrepancies(cls, diffs: Dict) -> Dict:
+        """
+        Reformats the dictionary result from DiffManager.diffs in a way that's more appropriate to our situation.
+        In particular:
+
+        * the "added" key is renamed to "to add"
+        * the "changed" key is renamed to "to_change"
+        * the "removed" key is renamed to "to_remove"
+
+        This tense change is necessary because the labels are cues to the user about actions that need to be done
+        in the future, not actions already done.
+        """
+        added = diffs.get('added')
+        changed = diffs.get('changed')
+        removed = diffs.get('removed')
+        cache_discrepancies = {}
+        if added:
+            cache_discrepancies['to_add'] = added
+        if changed:
+            cache_discrepancies['to_change'] = changed
+        if removed:
+            cache_discrepancies['to_remove'] = removed
+        return cache_discrepancies
 
     def load_contributors_from_json_file_cache(self, filename):
         self.loaded_contributor_data = data = self.get_contributors_json_from_file_cache(filename)
         self.load_from_dict(data)
 
         if DEBUG_CONTRIBUTIONS:  # pragma: no cover - debugging only
             PRINT("After load_contributors_from_json_file_cache...")
             PRINT(f"{n_of(self.pre_fork_contributors_by_name, 'pre-fork contributor by name')}")
             PRINT(f"{n_of(self.pre_fork_contributors_by_email, 'pre-fork contributor by email')}")
             PRINT(f"{n_of(self.contributors_by_name, 'contributor by name')}")
             PRINT(f"{n_of(self.contributors_by_email, 'contributor by email')}")
 
-    def reconcile_contributors_with_github_log(self):
+    def load_from_dict(self, data: Dict):
+        forked_at: Optional[str] = data.get('forked_at')
+        self.forked_at: Optional[datetime.datetime] = (None
+                                                       if forked_at is None
+                                                       else datetime.datetime.fromisoformat(forked_at))
+
+        if 'excluded_fork' in data:
+            # We originally implemented this, but it isn't needed and supporting it leads to problems. -kmp 30-Jul-2023
+            raise ValueError('"excluded_fork" is no longer supported.')
+
+        pre_fork_contributors_by_name_json = data.get('pre_fork_contributors_by_name') or {}
+        pre_fork_contributors_by_name = self.contributor_values_as_objects(pre_fork_contributors_by_name_json)
+        self.set_keys_as_primary_names(pre_fork_contributors_by_name)
+        self.pre_fork_contributors_by_name = pre_fork_contributors_by_name
+
+        if 'pre_fork_contributors_by_email' in data:
+            # We originally implemented this, but supporting it is unnecessarily complex
+            # because of redundancies of implementation and the possibility of ambiguities if both
+            # markers are present. -kmp 30-Jul-2023
+            raise ValueError('"pre_fork_contributors_by_email" is no longer supported.')
+        pre_fork_contributors_by_email = self.by_email_from_by_name(pre_fork_contributors_by_name)
+        self.pre_fork_contributors_by_email = pre_fork_contributors_by_email
+
+        contributors_by_name_json = data.get('contributors_by_name') or {}
+        contributors_by_name = self.contributor_values_as_objects(contributors_by_name_json)
+        self.set_keys_as_primary_names(contributors_by_name)
+        self.contributors_by_name = contributors_by_name
+
+        if 'contributors_by_email' in data:
+            # We originally implemented this, but supporting it is unnecessarily complex
+            # because of redundancies of implementation and the possibility of ambiguities if both
+            # markers are present. -kmp 30-Jul-2023
+            raise ValueError('"contributors_by_email" is no longer supported.')
+        contributors_by_email = self.by_email_from_by_name(contributors_by_name)
+        self.contributors_by_email = contributors_by_email
+
+    def reconcile_contributors_with_github_log(self, exclude_fork=None):
         """
         Rummages the GitHub log entries for contributors we don't know about.
         That data is merged against our existing structures.
         """
         if DEBUG_CONTRIBUTIONS:  # pragma: no cover - debugging only
             PRINT("Reconciling with git log.")
-        excluded_fork_contributors_by_email = (self.excluded_contributions.contributors_by_email
-                                               if self.excluded_contributions
-                                               else {})
-        # excluded_fork_contributors_by_name = (self.excluded_contributions.contributors_by_name
-        #                                       if self.excluded_contributions
-        #                                       else {})
-        fork_contributor_emails = set(excluded_fork_contributors_by_email.keys())
 
-        post_fork_contributors_seen = defaultdict(lambda: [])
+        if self.loaded_contributor_data:
+            pre_fork_contributor_emails = set(self.pre_fork_contributors_by_email.keys())
+        elif exclude_fork:
+            excluded_contributions = Contributions(repo=exclude_fork)
+            self.pre_fork_contributors_by_email = excluded_contributions.contributors_by_email
+            self.pre_fork_contributors_by_name = excluded_contributions.contributors_by_name
+            pre_fork_contributor_emails = set(self.pre_fork_contributors_by_email.keys())
+        else:
+            pre_fork_contributor_emails = set()
+
+        post_fork_contributors_seen = defaultdict(lambda: [])  # pragma: no cover - for debugging only
 
         contributors_by_email: ContributorIndex = self.contributors_by_email or {}
         git_repo = self.find_repo(repo_name=self.repo)
 
+        n = 0
+
         def notice_author(*, author: git.Actor, date: datetime.datetime):
             if self.forked_at:
                 if date < self.forked_at:
                     return
                     # raise Exception("Commits are out of order.")
-            elif author.email not in fork_contributor_emails:
-                PRINT(f"Forked {self.repo} at {date} by {author.email}")
+            elif author.email not in pre_fork_contributor_emails:
+                action = "Created" if n == 1 else (f"Forked {exclude_fork} as" if exclude_fork else "Forked")
+                PRINT(f"{action} {self.repo} at {date} by {author.email}")
                 self.forked_at = date
 
             if self.forked_at and date >= self.forked_at:
-                if author.email in fork_contributor_emails:
-                    # PRINT(f"Post-fork contribution from {author.email} ({date})")
-                    post_fork_contributors_seen[author.email].append(date)
+                if DEBUG_CONTRIBUTIONS:  # pragma: no cover - debugging only
+                    if author.email in pre_fork_contributor_emails:  # pragma: no cover - this is for debugging
+                        # PRINT(f"Post-fork contribution from {author.email} ({date})")
+                        post_fork_contributors_seen[author.email].append(date)
                 self.notice_reference_time(key=author.email, timestamp=date, timestamps=self.email_timestamps)
-                self.notice_reference_time(key=author.name, timestamp=date, timestamps=self.name_timestamps)
+                self.notice_reference_time(key=GitAnalysis.author_name(author), timestamp=date,
+                                           timestamps=self.name_timestamps)
 
                 contributor_by_email = contributors_by_email.get(author.email)
                 if contributor_by_email:  # already exists, so update it
-                    contributor_by_email.notice_mention_as(email=author.email, name=author.name)
+                    contributor_by_email.notice_mention_as(email=author.email, name=GitAnalysis.author_name(author))
                 else:  # need to create it new
                     contributor_by_email = Contributor.create(author=author)
                     contributors_by_email[author.email] = contributor_by_email
             else:
                 # print("skipped")
                 pass
 
-        n = 0
         for commit in reversed(list(git_repo.iter_commits())):
             n += 1
             commit_date = commit.committed_datetime
             notice_author(author=commit.author, date=commit_date)
             for co_author in commit.co_authors:
                 notice_author(author=co_author, date=commit_date)
-        if DEBUG_CONTRIBUTIONS:
+        if DEBUG_CONTRIBUTIONS:  # pragma: no cover - debugging only
             PRINT(f"{n_of(n, 'commit')} processed.")
-
-        for email, dates in post_fork_contributors_seen.items():
-            when = str(dates[0].date())
-            if len(dates) > 1:
-                when += f" to {dates[-1].date()}"
-            PRINT(f"{n_of(dates, 'post-fork commit')} seen for {email} ({when}).")
+            for email, dates in post_fork_contributors_seen.items():
+                when = str(dates[0].date())
+                if len(dates) > 1:
+                    when += f" to {dates[-1].date()}"
+                PRINT(f"{n_of(dates, 'post-fork commit')} seen for {email} ({when}).")
 
         contributors_by_name: ContributorIndex = {}
 
         for contributor_by_email in contributors_by_email.values():
             self.traverse(root=contributor_by_email,
                           cursor=contributor_by_email,
                           contributors_by_email=contributors_by_email,
                           contributors_by_name=contributors_by_name)
             for name in list(contributor_by_email.names):
                 contributors_by_name[name] = contributor_by_email
             for email in list(contributor_by_email.emails):
                 contributors_by_email[email] = contributor_by_email
 
-        # Note that the name table is somewhat unified, merging related cells, but the email table isn't.
-        # In part that's because I was lazy, but also we don't really need the email table to be so careful.
-        # It's the human names that really matter.
-        # if not self.pre_fork_contributors_by_name:
-        #     self.pre_fork_contributors_by_name = excluded_fork_contributors_by_name
-
-        # if not self.pre_fork_contributors_by_email:
-        #     self.pre_fork_contributors_by_email = excluded_fork_contributors_by_email
-
         self.contributors_by_name = self.contributor_index_by_primary_name(contributors_by_name)
-        self.contributors_by_email = contributors_by_email
+        self.contributors_by_email = self.by_email_from_by_name(self.contributors_by_name)  # contributors_by_email
 
         if DEBUG_CONTRIBUTIONS:  # pragma: no cover - debugging only
             PRINT("After reconcile_contributors_with_github_log...")
             PRINT(f"{n_of(self.pre_fork_contributors_by_name, 'pre-fork contributor by name')}")
             PRINT(f"{n_of(self.pre_fork_contributors_by_email, 'pre-fork contributor by email')}")
             PRINT(f"{n_of(self.contributors_by_name, 'contributor by name')}")
             PRINT(f"{n_of(self.contributors_by_email, 'contributor by email')}")
 
     @classmethod
-    def contributor_index_by_primary_name(cls, contributors_by_name: ContributorIndex) -> ContributorIndex:
-        """
-        Given a by-name contributor index:
-
-        * Makes sure that all contributors have only one name, indexed by the contributor's primary name
-        * Sorts the resulting index using a case-insensitive alphabetic sort
-
-        and then returns the result.
-
-        :param contributors_by_name: a contributor index indexed by human name
-        :return: a contributor index
-        """
-        seen = set()
-        nicknames_seen = set()
-        contributor_items = []
-        contributors = {}
-        for name, contributor in contributors_by_name.items():
-            if contributor not in seen:
-                for nickname in contributor.names:
-                    if nickname in nicknames_seen:
-                        raise Exception(f"Name improperly shared between {contributor}"
-                                        f" and {contributors_by_name[nickname]}")
-                    nicknames_seen.add(nickname)
-                contributor_items.append((contributor.primary_name, contributor))
-                seen.add(contributor)
-        for name, contributor in sorted(contributor_items,
-                                        # Having selected the longest names, now sort names ignoring case
-                                        key=lambda pair: pair[0].lower()):
-            contributors[name] = contributor
-        return contributors
-
-    @classmethod
     def traverse(cls,
                  root: Contributor,
                  cursor: Optional[Contributor],
                  contributors_by_email: ContributorIndex,
                  contributors_by_name: ContributorIndex,
                  seen: Optional[Set[Contributor]] = None):
         if seen is None:
@@ -459,74 +560,11 @@
         for name in list(cursor.names):
             contributor = contributors_by_name.get(name)
             if contributor and contributor not in seen:
                 cls.traverse(root=root, cursor=contributor, contributors_by_email=contributors_by_email,
                              contributors_by_name=contributors_by_name, seen=seen)
         for email in list(cursor.emails):
             contributor = contributors_by_email.get(email)
-            if contributor and contributor not in seen:
+            if contributor and contributor not in seen:  # pragma: no cover - shouldn't happen, included 'just in case'
+                warnings.warn(f"Unexpected stray email seen: {email}")
                 cls.traverse(root=root, cursor=contributor, contributors_by_email=contributors_by_email,
                              contributors_by_name=contributors_by_name, seen=seen)
-
-    def load_from_dict(self, data: Dict):
-        forked_at: Optional[str] = data.get('forked_at')
-        excluded_fork = data.get('excluded_fork')
-        self.forked_at: Optional[datetime.datetime] = (None
-                                                       if forked_at is None
-                                                       else datetime.datetime.fromisoformat(forked_at))
-        self.exclude_fork = excluded_fork
-
-        fork_contributors_by_name_json = data.get('pre_fork_contributors_by_name') or {}
-        fork_contributors_by_name = self.contributor_values_as_objects(fork_contributors_by_name_json)
-        self.pre_fork_contributors_by_name = fork_contributors_by_name
-        fork_contributors_by_email_json = data.get('pre_fork_contributors_by_email') or {}
-        if fork_contributors_by_email_json:
-            self.pre_fork_contributors_by_email = self.contributor_values_as_objects(fork_contributors_by_email_json)
-        else:
-            self.pre_fork_contributors_by_email = self.by_email_from_by_name(fork_contributors_by_name)
-
-        contributors_by_name_json = data.get('contributors_by_name', {})
-        self.contributors_by_name = contributors_by_name = self.contributor_values_as_objects(contributors_by_name_json)
-        contributors_by_email_json = data.get('contributors_by_email', {})
-        if contributors_by_email_json:
-            self.contributors_by_email = self.contributor_values_as_objects(contributors_by_email_json)
-        else:
-            self.contributors_by_email = self.by_email_from_by_name(contributors_by_name)
-
-    @classmethod
-    def by_email_from_by_name(cls, contributors_by_email_json):
-        result = {}
-        seen = set()
-        for email_key, entry in contributors_by_email_json.items():
-            ignored(email_key)
-            seen_key = id(entry)
-            if seen_key in seen:
-                continue
-            seen.add(seen_key)
-            for email in entry.get("emails", []) if isinstance(entry, dict) else entry.emails:
-                if result.get(email):
-                    raise Exception(f"email address {email} is used more than once.")
-                result[email] = entry
-        return result
-
-    def show_repo_contributors(self, analyze_discrepancies: bool = True, with_email: bool = True,
-                               error_class: Optional[Type[BaseException]] = None):
-        for author_name in self.repo_contributor_names(with_email=with_email):
-            PRINT(author_name)
-        if analyze_discrepancies:
-            file = self.existing_contributors_json_file()
-            if not file:
-                message = f"Need to create a {self.CONTRIBUTORS_CACHE_FILE} file for {self.repo}."
-                if error_class:
-                    raise error_class(message)
-                else:
-                    PRINT(message)
-            elif self.cache_discrepancies:
-                message = "There are contributor cache discrepancies."
-                PRINT(f"===== {message.rstrip('.').upper()} =====")
-                for action, items in self.cache_discrepancies.items():
-                    action: str
-                    PRINT(f"{action.replace('_', ' ').title()}:")
-                    for item in items:
-                        PRINT(f" * {item}")
-                if error_class:
-                    raise error_class(message)
```

### Comparing `dcicutils-7.6.0.2b7/dcicutils/creds_utils.py` & `dcicutils-7.6.0.2b8/dcicutils/creds_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b7/dcicutils/data_utils.py` & `dcicutils-7.6.0.2b8/dcicutils/data_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b7/dcicutils/deployment_utils.py` & `dcicutils-7.6.0.2b8/dcicutils/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b7/dcicutils/diff_utils.py` & `dcicutils-7.6.0.2b8/dcicutils/diff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b7/dcicutils/docker_utils.py` & `dcicutils-7.6.0.2b8/dcicutils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b7/dcicutils/ecr_scripts.py` & `dcicutils-7.6.0.2b8/dcicutils/ecr_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b7/dcicutils/ecr_utils.py` & `dcicutils-7.6.0.2b8/dcicutils/ecr_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b7/dcicutils/ecs_utils.py` & `dcicutils-7.6.0.2b8/dcicutils/ecs_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b7/dcicutils/env_base.py` & `dcicutils-7.6.0.2b8/dcicutils/env_base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b7/dcicutils/env_manager.py` & `dcicutils-7.6.0.2b8/dcicutils/env_manager.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b7/dcicutils/env_scripts.py` & `dcicutils-7.6.0.2b8/dcicutils/env_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b7/dcicutils/env_utils.py` & `dcicutils-7.6.0.2b8/dcicutils/env_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b7/dcicutils/env_utils_legacy.py` & `dcicutils-7.6.0.2b8/dcicutils/env_utils_legacy.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b7/dcicutils/es_utils.py` & `dcicutils-7.6.0.2b8/dcicutils/es_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b7/dcicutils/exceptions.py` & `dcicutils-7.6.0.2b8/dcicutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b7/dcicutils/ff_mocks.py` & `dcicutils-7.6.0.2b8/dcicutils/ff_mocks.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b7/dcicutils/ff_utils.py` & `dcicutils-7.6.0.2b8/dcicutils/ff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b7/dcicutils/function_cache_decorator.py` & `dcicutils-7.6.0.2b8/dcicutils/function_cache_decorator.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b7/dcicutils/glacier_utils.py` & `dcicutils-7.6.0.2b8/dcicutils/glacier_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b7/dcicutils/jh_utils.py` & `dcicutils-7.6.0.2b8/dcicutils/jh_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b7/dcicutils/kibana/dashboards.json` & `dcicutils-7.6.0.2b8/dcicutils/kibana/dashboards.json`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b7/dcicutils/kibana/readme.md` & `dcicutils-7.6.0.2b8/dcicutils/kibana/readme.md`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b7/dcicutils/lang_utils.py` & `dcicutils-7.6.0.2b8/dcicutils/lang_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b7/dcicutils/license_utils.py` & `dcicutils-7.6.0.2b8/dcicutils/license_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b7/dcicutils/log_utils.py` & `dcicutils-7.6.0.2b8/dcicutils/log_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b7/dcicutils/misc_utils.py` & `dcicutils-7.6.0.2b8/dcicutils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b7/dcicutils/obfuscation_utils.py` & `dcicutils-7.6.0.2b8/dcicutils/obfuscation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b7/dcicutils/opensearch_utils.py` & `dcicutils-7.6.0.2b8/dcicutils/opensearch_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b7/dcicutils/project_utils.py` & `dcicutils-7.6.0.2b8/dcicutils/project_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b7/dcicutils/qa_checkers.py` & `dcicutils-7.6.0.2b8/dcicutils/qa_checkers.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b7/dcicutils/qa_utils.py` & `dcicutils-7.6.0.2b8/dcicutils/qa_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b7/dcicutils/redis_tools.py` & `dcicutils-7.6.0.2b8/dcicutils/redis_tools.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b7/dcicutils/redis_utils.py` & `dcicutils-7.6.0.2b8/dcicutils/redis_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b7/dcicutils/s3_utils.py` & `dcicutils-7.6.0.2b8/dcicutils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b7/dcicutils/scripts/publish_to_pypi.py` & `dcicutils-7.6.0.2b8/dcicutils/scripts/publish_to_pypi.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b7/dcicutils/secrets_utils.py` & `dcicutils-7.6.0.2b8/dcicutils/secrets_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b7/dcicutils/snapshot_utils.py` & `dcicutils-7.6.0.2b8/dcicutils/snapshot_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b7/dcicutils/ssl_certificate_utils.py` & `dcicutils-7.6.0.2b8/dcicutils/ssl_certificate_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b7/dcicutils/task_utils.py` & `dcicutils-7.6.0.2b8/dcicutils/task_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b7/dcicutils/trace_utils.py` & `dcicutils-7.6.0.2b8/dcicutils/trace_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b7/pyproject.toml` & `dcicutils-7.6.0.2b8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dcicutils"
-version = "7.6.0.2b7"
+version = "7.6.0.2b8"
 description = "Utility package for interacting with the 4DN Data Portal and other 4DN resources"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/4dn-dcic/utils"
 repository = "https://github.com/4dn-dcic/utils"
 packages = [
```

### Comparing `dcicutils-7.6.0.2b7/setup.py` & `dcicutils-7.6.0.2b8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 entry_points = \
 {'console_scripts': ['publish-to-pypi = dcicutils.scripts.publish_to_pypi:main',
                      'show-contributors = '
                      'dcicutils.contribution_scripts:show_contributors_main']}
 
 setup_kwargs = {
     'name': 'dcicutils',
-    'version': '7.6.0.2b7',
+    'version': '7.6.0.2b8',
     'description': 'Utility package for interacting with the 4DN Data Portal and other 4DN resources',
     'long_description': '=====\nutils\n=====\n\nCheck out our full documentation `here <https://dcic-utils.readthedocs.io/en/latest/>`_\n\nThis repository contains various utility modules shared amongst several projects in the 4DN-DCIC. It is meant to be used internally by the DCIC team and externally as a Python API to `Fourfront <https://data.4dnucleome.org>`_\\ , the 4DN data portal.\n\npip installable as the ``dcicutils`` package with: ``pip install dcicutils``\n\nSee `this document <https://dcic-utils.readthedocs.io/en/latest/getting_started.html>`_ for tips on getting started. `Go here <https://dcic-utils.readthedocs.io/en/latest/examples.html>`_ for examples of some of the most useful functions.\n\n\n.. image:: https://travis-ci.org/4dn-dcic/utils.svg?branch=master\n   :target: https://travis-ci.org/4dn-dcic/utils\n   :alt: Build Status\n\n\n.. image:: https://coveralls.io/repos/github/4dn-dcic/utils/badge.svg?branch=master\n   :target: https://coveralls.io/github/4dn-dcic/utils?branch=master\n   :alt: Coverage\n\n.. image:: https://readthedocs.org/projects/dcic-utils/badge/?version=latest\n   :target: https://dcic-utils.readthedocs.io/en/latest/?badge=latest\n   :alt: Documentation Status\n',
     'author': '4DN-DCIC Team',
     'author_email': 'support@4dnucleome.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/4dn-dcic/utils',
```

### Comparing `dcicutils-7.6.0.2b7/PKG-INFO` & `dcicutils-7.6.0.2b8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcicutils
-Version: 7.6.0.2b7
+Version: 7.6.0.2b8
 Summary: Utility package for interacting with the 4DN Data Portal and other 4DN resources
 Home-page: https://github.com/4dn-dcic/utils
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7,<3.10
 Classifier: Development Status :: 4 - Beta
```

