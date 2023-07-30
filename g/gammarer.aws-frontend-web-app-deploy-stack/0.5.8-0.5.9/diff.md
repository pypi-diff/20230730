# Comparing `tmp/gammarer.aws-frontend-web-app-deploy-stack-0.5.8.tar.gz` & `tmp/gammarer.aws-frontend-web-app-deploy-stack-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammarer.aws-frontend-web-app-deploy-stack-0.5.8.tar", last modified: Wed Jul 26 19:15:16 2023, max compression
+gzip compressed data, was "gammarer.aws-frontend-web-app-deploy-stack-0.5.9.tar", last modified: Thu Jul 27 19:16:15 2023, max compression
```

## Comparing `gammarer.aws-frontend-web-app-deploy-stack-0.5.8.tar` & `gammarer.aws-frontend-web-app-deploy-stack-0.5.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:15:16.898653 gammarer.aws-frontend-web-app-deploy-stack-0.5.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-26 19:15:04.000000 gammarer.aws-frontend-web-app-deploy-stack-0.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-26 19:15:04.000000 gammarer.aws-frontend-web-app-deploy-stack-0.5.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-26 19:15:16.898653 gammarer.aws-frontend-web-app-deploy-stack-0.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-26 19:15:04.000000 gammarer.aws-frontend-web-app-deploy-stack-0.5.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-26 19:15:04.000000 gammarer.aws-frontend-web-app-deploy-stack-0.5.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 19:15:16.898653 gammarer.aws-frontend-web-app-deploy-stack-0.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-07-26 19:15:04.000000 gammarer.aws-frontend-web-app-deploy-stack-0.5.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:15:16.894653 gammarer.aws-frontend-web-app-deploy-stack-0.5.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:15:16.894653 gammarer.aws-frontend-web-app-deploy-stack-0.5.8/src/gammarer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:15:16.898653 gammarer.aws-frontend-web-app-deploy-stack-0.5.8/src/gammarer/aws_frontend_web_app_deploy_stack/
--rw-r--r--   0 runner    (1001) docker     (123)    26250 2023-07-26 19:15:04.000000 gammarer.aws-frontend-web-app-deploy-stack-0.5.8/src/gammarer/aws_frontend_web_app_deploy_stack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:15:16.898653 gammarer.aws-frontend-web-app-deploy-stack-0.5.8/src/gammarer/aws_frontend_web_app_deploy_stack/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-26 19:15:04.000000 gammarer.aws-frontend-web-app-deploy-stack-0.5.8/src/gammarer/aws_frontend_web_app_deploy_stack/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36452 2023-07-26 19:15:04.000000 gammarer.aws-frontend-web-app-deploy-stack-0.5.8/src/gammarer/aws_frontend_web_app_deploy_stack/_jsii/aws-frontend-web-app-deploy-stack@0.5.8.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 19:15:04.000000 gammarer.aws-frontend-web-app-deploy-stack-0.5.8/src/gammarer/aws_frontend_web_app_deploy_stack/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:15:16.898653 gammarer.aws-frontend-web-app-deploy-stack-0.5.8/src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-26 19:15:16.000000 gammarer.aws-frontend-web-app-deploy-stack-0.5.8/src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-26 19:15:16.000000 gammarer.aws-frontend-web-app-deploy-stack-0.5.8/src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 19:15:16.000000 gammarer.aws-frontend-web-app-deploy-stack-0.5.8/src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-26 19:15:16.000000 gammarer.aws-frontend-web-app-deploy-stack-0.5.8/src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-26 19:15:16.000000 gammarer.aws-frontend-web-app-deploy-stack-0.5.8/src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:16:15.312588 gammarer.aws-frontend-web-app-deploy-stack-0.5.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-27 19:16:03.000000 gammarer.aws-frontend-web-app-deploy-stack-0.5.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-27 19:16:03.000000 gammarer.aws-frontend-web-app-deploy-stack-0.5.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-27 19:16:15.312588 gammarer.aws-frontend-web-app-deploy-stack-0.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-27 19:16:03.000000 gammarer.aws-frontend-web-app-deploy-stack-0.5.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-27 19:16:03.000000 gammarer.aws-frontend-web-app-deploy-stack-0.5.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 19:16:15.312588 gammarer.aws-frontend-web-app-deploy-stack-0.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-27 19:16:03.000000 gammarer.aws-frontend-web-app-deploy-stack-0.5.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:16:15.308587 gammarer.aws-frontend-web-app-deploy-stack-0.5.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:16:15.308587 gammarer.aws-frontend-web-app-deploy-stack-0.5.9/src/gammarer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:16:15.312588 gammarer.aws-frontend-web-app-deploy-stack-0.5.9/src/gammarer/aws_frontend_web_app_deploy_stack/
+-rw-r--r--   0 runner    (1001) docker     (123)    26250 2023-07-27 19:16:03.000000 gammarer.aws-frontend-web-app-deploy-stack-0.5.9/src/gammarer/aws_frontend_web_app_deploy_stack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:16:15.312588 gammarer.aws-frontend-web-app-deploy-stack-0.5.9/src/gammarer/aws_frontend_web_app_deploy_stack/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-27 19:16:03.000000 gammarer.aws-frontend-web-app-deploy-stack-0.5.9/src/gammarer/aws_frontend_web_app_deploy_stack/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36454 2023-07-27 19:16:03.000000 gammarer.aws-frontend-web-app-deploy-stack-0.5.9/src/gammarer/aws_frontend_web_app_deploy_stack/_jsii/aws-frontend-web-app-deploy-stack@0.5.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 19:16:03.000000 gammarer.aws-frontend-web-app-deploy-stack-0.5.9/src/gammarer/aws_frontend_web_app_deploy_stack/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:16:15.312588 gammarer.aws-frontend-web-app-deploy-stack-0.5.9/src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-27 19:16:15.000000 gammarer.aws-frontend-web-app-deploy-stack-0.5.9/src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-27 19:16:15.000000 gammarer.aws-frontend-web-app-deploy-stack-0.5.9/src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 19:16:15.000000 gammarer.aws-frontend-web-app-deploy-stack-0.5.9/src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-27 19:16:15.000000 gammarer.aws-frontend-web-app-deploy-stack-0.5.9/src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-27 19:16:15.000000 gammarer.aws-frontend-web-app-deploy-stack-0.5.9/src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/top_level.txt
```

### Comparing `gammarer.aws-frontend-web-app-deploy-stack-0.5.8/LICENSE` & `gammarer.aws-frontend-web-app-deploy-stack-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gammarer.aws-frontend-web-app-deploy-stack-0.5.8/PKG-INFO` & `gammarer.aws-frontend-web-app-deploy-stack-0.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-frontend-web-app-deploy-stack
-Version: 0.5.8
+Version: 0.5.9
 Summary: This is an AWS CDK Construct to make deploying a Frontend Web App (SPA) deploy to S3 behind CloudFront.
 Home-page: https://github.com/yicr/aws-frontend-web-app-deploy-stack.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-frontend-web-app-deploy-stack.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-frontend-web-app-deploy-stack-0.5.8/README.md` & `gammarer.aws-frontend-web-app-deploy-stack-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `gammarer.aws-frontend-web-app-deploy-stack-0.5.8/setup.py` & `gammarer.aws-frontend-web-app-deploy-stack-0.5.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "gammarer.aws-frontend-web-app-deploy-stack",
-    "version": "0.5.8",
+    "version": "0.5.9",
     "description": "This is an AWS CDK Construct to make deploying a Frontend Web App (SPA) deploy to S3 behind CloudFront.",
     "license": "Apache-2.0",
     "url": "https://github.com/yicr/aws-frontend-web-app-deploy-stack.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,27 +22,27 @@
     },
     "packages": [
         "gammarer.aws_frontend_web_app_deploy_stack",
         "gammarer.aws_frontend_web_app_deploy_stack._jsii"
     ],
     "package_data": {
         "gammarer.aws_frontend_web_app_deploy_stack._jsii": [
-            "aws-frontend-web-app-deploy-stack@0.5.8.jsii.tgz"
+            "aws-frontend-web-app-deploy-stack@0.5.9.jsii.tgz"
         ],
         "gammarer.aws_frontend_web_app_deploy_stack": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "aws-cdk-lib>=2.62.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "gammarer.aws-secure-bucket>=0.9.9, <0.10.0",
-        "gammarer.aws-secure-cloudfront-origin-bucket>=0.6.8, <0.7.0",
-        "gammarer.aws-secure-frontend-web-app-cloudfront-distribution>=0.6.8, <0.7.0",
+        "gammarer.aws-secure-bucket>=0.10.1, <0.11.0",
+        "gammarer.aws-secure-cloudfront-origin-bucket>=0.6.9, <0.7.0",
+        "gammarer.aws-secure-frontend-web-app-cloudfront-distribution>=0.6.9, <0.7.0",
         "jsii>=1.85.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
```

### Comparing `gammarer.aws-frontend-web-app-deploy-stack-0.5.8/src/gammarer/aws_frontend_web_app_deploy_stack/__init__.py` & `gammarer.aws-frontend-web-app-deploy-stack-0.5.9/src/gammarer/aws_frontend_web_app_deploy_stack/__init__.py`

 * *Files identical despite different names*

### Comparing `gammarer.aws-frontend-web-app-deploy-stack-0.5.8/src/gammarer/aws_frontend_web_app_deploy_stack/_jsii/__init__.py` & `gammarer.aws-frontend-web-app-deploy-stack-0.5.9/src/gammarer/aws_frontend_web_app_deploy_stack/_jsii/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 import constructs._jsii
 import gammarer.aws_secure_bucket._jsii
 import gammarer.aws_secure_cloudfront_origin_bucket._jsii
 import gammarer.aws_secure_frontend_web_app_cloudfront_distribution._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "@gammarer/aws-frontend-web-app-deploy-stack",
-    "0.5.8",
+    "0.5.9",
     __name__[0:-6],
-    "aws-frontend-web-app-deploy-stack@0.5.8.jsii.tgz",
+    "aws-frontend-web-app-deploy-stack@0.5.9.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `gammarer.aws-frontend-web-app-deploy-stack-0.5.8/src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/PKG-INFO` & `gammarer.aws-frontend-web-app-deploy-stack-0.5.9/src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-frontend-web-app-deploy-stack
-Version: 0.5.8
+Version: 0.5.9
 Summary: This is an AWS CDK Construct to make deploying a Frontend Web App (SPA) deploy to S3 behind CloudFront.
 Home-page: https://github.com/yicr/aws-frontend-web-app-deploy-stack.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-frontend-web-app-deploy-stack.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-frontend-web-app-deploy-stack-0.5.8/src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/SOURCES.txt` & `gammarer.aws-frontend-web-app-deploy-stack-0.5.9/src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/SOURCES.txt
 src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/dependency_links.txt
 src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/requires.txt
 src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/top_level.txt
 src/gammarer/aws_frontend_web_app_deploy_stack/__init__.py
 src/gammarer/aws_frontend_web_app_deploy_stack/py.typed
 src/gammarer/aws_frontend_web_app_deploy_stack/_jsii/__init__.py
-src/gammarer/aws_frontend_web_app_deploy_stack/_jsii/aws-frontend-web-app-deploy-stack@0.5.8.jsii.tgz
+src/gammarer/aws_frontend_web_app_deploy_stack/_jsii/aws-frontend-web-app-deploy-stack@0.5.9.jsii.tgz
```

