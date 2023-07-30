# Comparing `tmp/mkdocs_puml-1.2.2.tar.gz` & `tmp/mkdocs_puml-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_puml-1.2.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "mkdocs_puml-1.2.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `mkdocs_puml-1.2.2.tar` & `mkdocs_puml-1.2.3.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0      237 2022-09-15 12:01:38.953711 mkdocs_puml-1.2.2/.coveragerc
--rw-r--r--   0        0        0    31089 2023-01-25 09:20:39.582596 mkdocs_puml-1.2.2/.docs/logo.png
--rw-r--r--   0        0        0       43 2022-09-15 12:01:38.953802 mkdocs_puml-1.2.2/.flake8
--rw-r--r--   0        0        0      655 2023-01-25 09:42:12.642417 mkdocs_puml-1.2.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2022-11-13 12:18:46.573988 mkdocs_puml-1.2.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1298 2023-03-22 10:02:51.666715 mkdocs_puml-1.2.2/.github/workflows/checks.yml
--rw-r--r--   0        0        0     5163 2022-09-20 17:56:58.445961 mkdocs_puml-1.2.2/.gitignore
--rw-r--r--   0        0        0      404 2022-09-15 12:01:38.954254 mkdocs_puml-1.2.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1082 2022-09-15 12:01:38.954367 mkdocs_puml-1.2.2/LICENSE
--rw-r--r--   0        0        0      573 2023-06-28 09:32:47.756816 mkdocs_puml-1.2.2/Pipfile
--rw-r--r--   0        0        0    71332 2023-06-28 09:32:47.757288 mkdocs_puml-1.2.2/Pipfile.lock
--rw-r--r--   0        0        0     3881 2023-03-22 10:02:51.666879 mkdocs_puml-1.2.2/README.md
--rw-r--r--   0        0        0       68 2023-06-28 09:32:47.757628 mkdocs_puml-1.2.2/mkdocs_puml/__init__.py
--rw-r--r--   0        0        0      948 2023-02-18 11:50:55.936744 mkdocs_puml-1.2.2/mkdocs_puml/encoder.py
--rw-r--r--   0        0        0     5077 2023-06-28 09:32:47.757849 mkdocs_puml-1.2.2/mkdocs_puml/plugin.py
--rw-r--r--   0        0        0     3841 2023-03-22 10:02:51.667311 mkdocs_puml-1.2.2/mkdocs_puml/puml.py
--rw-r--r--   0        0        0      628 2023-06-28 09:32:47.758075 mkdocs_puml-1.2.2/pyproject.toml
--rw-r--r--   0        0        0        0 2022-09-15 12:01:38.956165 mkdocs_puml-1.2.2/tests/__init__.py
--rw-r--r--   0        0        0      866 2023-03-22 10:02:51.667442 mkdocs_puml-1.2.2/tests/conftest.py
--rw-r--r--   0        0        0        0 2022-09-20 17:56:58.447859 mkdocs_puml-1.2.2/tests/plugins/__init__.py
--rw-r--r--   0        0        0     2374 2023-06-28 09:10:05.717513 mkdocs_puml-1.2.2/tests/plugins/conftest.py
--rw-r--r--   0        0        0     2247 2023-06-28 09:10:05.717746 mkdocs_puml-1.2.2/tests/plugins/test_plugin.py
--rw-r--r--   0        0        0      197 2022-09-15 12:01:38.956431 mkdocs_puml-1.2.2/tests/test_encoder.py
--rw-r--r--   0        0        0      876 2023-01-25 09:21:05.750584 mkdocs_puml-1.2.2/tests/test_puml.py
--rw-r--r--   0        0        0     1074 2023-03-22 10:02:51.667954 mkdocs_puml-1.2.2/tests/testdata/markdown.md
--rw-r--r--   0        0        0      375 2022-09-20 17:56:58.448279 mkdocs_puml-1.2.2/tests/testdata/output.html
--rw-r--r--   0        0        0     2255 2022-09-15 12:01:38.956767 mkdocs_puml-1.2.2/tests/testdata/plantuml.svg
--rw-r--r--   0        0        0     4334 1970-01-01 00:00:00.000000 mkdocs_puml-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0      237 2022-09-15 12:01:38.953711 mkdocs_puml-1.2.3/.coveragerc
+-rw-r--r--   0        0        0    31089 2023-01-25 09:20:39.582596 mkdocs_puml-1.2.3/.docs/logo.png
+-rw-r--r--   0        0        0       43 2022-09-15 12:01:38.953802 mkdocs_puml-1.2.3/.flake8
+-rw-r--r--   0        0        0      655 2023-01-25 09:42:12.642417 mkdocs_puml-1.2.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2022-11-13 12:18:46.573988 mkdocs_puml-1.2.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1298 2023-03-22 10:02:51.666715 mkdocs_puml-1.2.3/.github/workflows/checks.yml
+-rw-r--r--   0        0        0     5494 2023-07-30 09:50:18.334236 mkdocs_puml-1.2.3/.gitignore
+-rw-r--r--   0        0        0      404 2022-09-15 12:01:38.954254 mkdocs_puml-1.2.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      220 2023-07-30 09:50:18.334890 mkdocs_puml-1.2.3/.vscode/settings.json
+-rw-r--r--   0        0        0     1082 2022-09-15 12:01:38.954367 mkdocs_puml-1.2.3/LICENSE
+-rw-r--r--   0        0        0      581 2023-07-30 09:50:18.335270 mkdocs_puml-1.2.3/Pipfile
+-rw-r--r--   0        0        0    72352 2023-07-30 09:50:18.336178 mkdocs_puml-1.2.3/Pipfile.lock
+-rw-r--r--   0        0        0     3881 2023-07-29 20:19:51.838589 mkdocs_puml-1.2.3/README.md
+-rw-r--r--   0        0        0       68 2023-07-30 09:50:18.336488 mkdocs_puml-1.2.3/mkdocs_puml/__init__.py
+-rw-r--r--   0        0        0      948 2023-02-18 11:50:55.936744 mkdocs_puml-1.2.3/mkdocs_puml/encoder.py
+-rw-r--r--   0        0        0     5143 2023-07-30 09:50:18.336716 mkdocs_puml-1.2.3/mkdocs_puml/plugin.py
+-rw-r--r--   0        0        0     3841 2023-03-22 10:02:51.667311 mkdocs_puml-1.2.3/mkdocs_puml/puml.py
+-rw-r--r--   0        0        0      628 2023-06-28 09:32:47.758075 mkdocs_puml-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-09-15 12:01:38.956165 mkdocs_puml-1.2.3/tests/__init__.py
+-rw-r--r--   0        0        0      866 2023-03-22 10:02:51.667442 mkdocs_puml-1.2.3/tests/conftest.py
+-rw-r--r--   0        0        0        0 2022-09-20 17:56:58.447859 mkdocs_puml-1.2.3/tests/plugins/__init__.py
+-rw-r--r--   0        0        0     2374 2023-06-28 09:10:05.717513 mkdocs_puml-1.2.3/tests/plugins/conftest.py
+-rw-r--r--   0        0        0     2247 2023-06-28 09:10:05.717746 mkdocs_puml-1.2.3/tests/plugins/test_plugin.py
+-rw-r--r--   0        0        0      197 2022-09-15 12:01:38.956431 mkdocs_puml-1.2.3/tests/test_encoder.py
+-rw-r--r--   0        0        0      876 2023-01-25 09:21:05.750584 mkdocs_puml-1.2.3/tests/test_puml.py
+-rw-r--r--   0        0        0     1074 2023-03-22 10:02:51.667954 mkdocs_puml-1.2.3/tests/testdata/markdown.md
+-rw-r--r--   0        0        0      375 2022-09-20 17:56:58.448279 mkdocs_puml-1.2.3/tests/testdata/output.html
+-rw-r--r--   0        0        0     2255 2022-09-15 12:01:38.956767 mkdocs_puml-1.2.3/tests/testdata/plantuml.svg
+-rw-r--r--   0        0        0     4334 1970-01-01 00:00:00.000000 mkdocs_puml-1.2.3/PKG-INFO
```

### Comparing `mkdocs_puml-1.2.2/.docs/logo.png` & `mkdocs_puml-1.2.3/.docs/logo.png`

 * *Files identical despite different names*

### Comparing `mkdocs_puml-1.2.2/.github/ISSUE_TEMPLATE/bug_report.md` & `mkdocs_puml-1.2.3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `mkdocs_puml-1.2.2/.github/ISSUE_TEMPLATE/feature_request.md` & `mkdocs_puml-1.2.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `mkdocs_puml-1.2.2/.github/workflows/checks.yml` & `mkdocs_puml-1.2.3/.github/workflows/checks.yml`

 * *Files identical despite different names*

### Comparing `mkdocs_puml-1.2.2/.gitignore` & `mkdocs_puml-1.2.3/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,32 @@
 # Created by https://www.toptal.com/developers/gitignore/api/python,pycharm+all
 # Edit at https://www.toptal.com/developers/gitignore?templates=python,pycharm+all
 
 .examples/
 .DS_Store
 
+### VisualStudioCode ###
+.vscode/*
+!.vscode/settings.json
+!.vscode/tasks.json
+!.vscode/launch.json
+!.vscode/extensions.json
+!.vscode/*.code-snippets
+
+# Local History for Visual Studio Code
+.history/
+
+# Built Visual Studio Code Extensions
+*.vsix
+
+### VisualStudioCode Patch ###
+# Ignore all local history of files
+.history
+.ionide
+
 ### PyCharm+all ###
 # Covers JetBrains IDEs: IntelliJ, RubyMine, PhpStorm, AppCode, PyCharm, CLion, Android Studio, WebStorm and Rider
 # Reference: https://intellij-support.jetbrains.com/hc/en-us/articles/206544839
 
 # User-specific stuff
 .idea/**/workspace.xml
 .idea/**/tasks.xml
```

### Comparing `mkdocs_puml-1.2.2/LICENSE` & `mkdocs_puml-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_puml-1.2.2/Pipfile` & `mkdocs_puml-1.2.3/Pipfile`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 url = "https://pypi.org/simple"
 verify_ssl = true
 name = "pypi"
 
 [packages]
 requests = "~= 2.31"
 flit = "~=3.7"
-mkdocs = "~=1.4"
+mkdocs = ">= 1.3, < 2.0"
 
 [dev-packages]
 mkdocs-material = "*"
 mkdocs-awesome-pages-plugin = "*"
 pytest = "*"
 pytest-cov = "*"
 flake8 = "*"
```

### Comparing `mkdocs_puml-1.2.2/Pipfile.lock` & `mkdocs_puml-1.2.3/Pipfile.lock`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9520356753812637%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'f2dd9ca97b80c220cba621d9d5ac269097f073875d581a7c4ff6157f1ad1b6e6'}}",*

 * * "'default'": "{'certifi': {'hashes': "*

 * *              "['sha256:539cc1d13202e33ca466e88b2807e29f4c13049d6d87031a3c110744495cb082', "*

 * *              "'sha256:92d6037539857d8206b8f6ae472e8b77db8058fec5937a1ef3f54304089edbb9'], "*

 * *              "'version': '==2023.7.22'}, 'charset-normalizer': {'hashes': "*

 * *              "['sha256:04e57ab9fbf9607b77f7d057974694b4f6b142da9ed4a199859d9d4d5c63fe96', […]*

```diff
@@ -1,11 +1,11 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "07c0b6f3bb841007f9906449f08e2a556ce169915f6e63a27cacc2a666d20990"
+            "sha256": "f2dd9ca97b80c220cba621d9d5ac269097f073875d581a7c4ff6157f1ad1b6e6"
         },
         "pipfile-spec": 6,
         "requires": {
             "python_version": "3.11"
         },
         "sources": [
             {
@@ -14,108 +14,108 @@
                 "verify_ssl": true
             }
         ]
     },
     "default": {
         "certifi": {
             "hashes": [
-                "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7",
-                "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"
+                "sha256:539cc1d13202e33ca466e88b2807e29f4c13049d6d87031a3c110744495cb082",
+                "sha256:92d6037539857d8206b8f6ae472e8b77db8058fec5937a1ef3f54304089edbb9"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==2023.5.7"
+            "version": "==2023.7.22"
         },
         "charset-normalizer": {
             "hashes": [
-                "sha256:04afa6387e2b282cf78ff3dbce20f0cc071c12dc8f685bd40960cc68644cfea6",
-                "sha256:04eefcee095f58eaabe6dc3cc2262f3bcd776d2c67005880894f447b3f2cb9c1",
-                "sha256:0be65ccf618c1e7ac9b849c315cc2e8a8751d9cfdaa43027d4f6624bd587ab7e",
-                "sha256:0c95f12b74681e9ae127728f7e5409cbbef9cd914d5896ef238cc779b8152373",
-                "sha256:0ca564606d2caafb0abe6d1b5311c2649e8071eb241b2d64e75a0d0065107e62",
-                "sha256:10c93628d7497c81686e8e5e557aafa78f230cd9e77dd0c40032ef90c18f2230",
-                "sha256:11d117e6c63e8f495412d37e7dc2e2fff09c34b2d09dbe2bee3c6229577818be",
-                "sha256:11d3bcb7be35e7b1bba2c23beedac81ee893ac9871d0ba79effc7fc01167db6c",
-                "sha256:12a2b561af122e3d94cdb97fe6fb2bb2b82cef0cdca131646fdb940a1eda04f0",
-                "sha256:12d1a39aa6b8c6f6248bb54550efcc1c38ce0d8096a146638fd4738e42284448",
-                "sha256:1435ae15108b1cb6fffbcea2af3d468683b7afed0169ad718451f8db5d1aff6f",
-                "sha256:1c60b9c202d00052183c9be85e5eaf18a4ada0a47d188a83c8f5c5b23252f649",
-                "sha256:1e8fcdd8f672a1c4fc8d0bd3a2b576b152d2a349782d1eb0f6b8e52e9954731d",
-                "sha256:20064ead0717cf9a73a6d1e779b23d149b53daf971169289ed2ed43a71e8d3b0",
-                "sha256:21fa558996782fc226b529fdd2ed7866c2c6ec91cee82735c98a197fae39f706",
-                "sha256:22908891a380d50738e1f978667536f6c6b526a2064156203d418f4856d6e86a",
-                "sha256:3160a0fd9754aab7d47f95a6b63ab355388d890163eb03b2d2b87ab0a30cfa59",
-                "sha256:322102cdf1ab682ecc7d9b1c5eed4ec59657a65e1c146a0da342b78f4112db23",
-                "sha256:34e0a2f9c370eb95597aae63bf85eb5e96826d81e3dcf88b8886012906f509b5",
-                "sha256:3573d376454d956553c356df45bb824262c397c6e26ce43e8203c4c540ee0acb",
-                "sha256:3747443b6a904001473370d7810aa19c3a180ccd52a7157aacc264a5ac79265e",
-                "sha256:38e812a197bf8e71a59fe55b757a84c1f946d0ac114acafaafaf21667a7e169e",
-                "sha256:3a06f32c9634a8705f4ca9946d667609f52cf130d5548881401f1eb2c39b1e2c",
-                "sha256:3a5fc78f9e3f501a1614a98f7c54d3969f3ad9bba8ba3d9b438c3bc5d047dd28",
-                "sha256:3d9098b479e78c85080c98e1e35ff40b4a31d8953102bb0fd7d1b6f8a2111a3d",
-                "sha256:3dc5b6a8ecfdc5748a7e429782598e4f17ef378e3e272eeb1340ea57c9109f41",
-                "sha256:4155b51ae05ed47199dc5b2a4e62abccb274cee6b01da5b895099b61b1982974",
-                "sha256:49919f8400b5e49e961f320c735388ee686a62327e773fa5b3ce6721f7e785ce",
-                "sha256:53d0a3fa5f8af98a1e261de6a3943ca631c526635eb5817a87a59d9a57ebf48f",
-                "sha256:5f008525e02908b20e04707a4f704cd286d94718f48bb33edddc7d7b584dddc1",
-                "sha256:628c985afb2c7d27a4800bfb609e03985aaecb42f955049957814e0491d4006d",
-                "sha256:65ed923f84a6844de5fd29726b888e58c62820e0769b76565480e1fdc3d062f8",
-                "sha256:6734e606355834f13445b6adc38b53c0fd45f1a56a9ba06c2058f86893ae8017",
-                "sha256:6baf0baf0d5d265fa7944feb9f7451cc316bfe30e8df1a61b1bb08577c554f31",
-                "sha256:6f4f4668e1831850ebcc2fd0b1cd11721947b6dc7c00bf1c6bd3c929ae14f2c7",
-                "sha256:6f5c2e7bc8a4bf7c426599765b1bd33217ec84023033672c1e9a8b35eaeaaaf8",
-                "sha256:6f6c7a8a57e9405cad7485f4c9d3172ae486cfef1344b5ddd8e5239582d7355e",
-                "sha256:7381c66e0561c5757ffe616af869b916c8b4e42b367ab29fedc98481d1e74e14",
-                "sha256:73dc03a6a7e30b7edc5b01b601e53e7fc924b04e1835e8e407c12c037e81adbd",
-                "sha256:74db0052d985cf37fa111828d0dd230776ac99c740e1a758ad99094be4f1803d",
-                "sha256:75f2568b4189dda1c567339b48cba4ac7384accb9c2a7ed655cd86b04055c795",
-                "sha256:78cacd03e79d009d95635e7d6ff12c21eb89b894c354bd2b2ed0b4763373693b",
-                "sha256:80d1543d58bd3d6c271b66abf454d437a438dff01c3e62fdbcd68f2a11310d4b",
-                "sha256:830d2948a5ec37c386d3170c483063798d7879037492540f10a475e3fd6f244b",
-                "sha256:891cf9b48776b5c61c700b55a598621fdb7b1e301a550365571e9624f270c203",
-                "sha256:8f25e17ab3039b05f762b0a55ae0b3632b2e073d9c8fc88e89aca31a6198e88f",
-                "sha256:9a3267620866c9d17b959a84dd0bd2d45719b817245e49371ead79ed4f710d19",
-                "sha256:a04f86f41a8916fe45ac5024ec477f41f886b3c435da2d4e3d2709b22ab02af1",
-                "sha256:aaf53a6cebad0eae578f062c7d462155eada9c172bd8c4d250b8c1d8eb7f916a",
-                "sha256:abc1185d79f47c0a7aaf7e2412a0eb2c03b724581139193d2d82b3ad8cbb00ac",
-                "sha256:ac0aa6cd53ab9a31d397f8303f92c42f534693528fafbdb997c82bae6e477ad9",
-                "sha256:ac3775e3311661d4adace3697a52ac0bab17edd166087d493b52d4f4f553f9f0",
-                "sha256:b06f0d3bf045158d2fb8837c5785fe9ff9b8c93358be64461a1089f5da983137",
-                "sha256:b116502087ce8a6b7a5f1814568ccbd0e9f6cfd99948aa59b0e241dc57cf739f",
-                "sha256:b82fab78e0b1329e183a65260581de4375f619167478dddab510c6c6fb04d9b6",
-                "sha256:bd7163182133c0c7701b25e604cf1611c0d87712e56e88e7ee5d72deab3e76b5",
-                "sha256:c36bcbc0d5174a80d6cccf43a0ecaca44e81d25be4b7f90f0ed7bcfbb5a00909",
-                "sha256:c3af8e0f07399d3176b179f2e2634c3ce9c1301379a6b8c9c9aeecd481da494f",
-                "sha256:c84132a54c750fda57729d1e2599bb598f5fa0344085dbde5003ba429a4798c0",
-                "sha256:cb7b2ab0188829593b9de646545175547a70d9a6e2b63bf2cd87a0a391599324",
-                "sha256:cca4def576f47a09a943666b8f829606bcb17e2bc2d5911a46c8f8da45f56755",
-                "sha256:cf6511efa4801b9b38dc5546d7547d5b5c6ef4b081c60b23e4d941d0eba9cbeb",
-                "sha256:d16fd5252f883eb074ca55cb622bc0bee49b979ae4e8639fff6ca3ff44f9f854",
-                "sha256:d2686f91611f9e17f4548dbf050e75b079bbc2a82be565832bc8ea9047b61c8c",
-                "sha256:d7fc3fca01da18fbabe4625d64bb612b533533ed10045a2ac3dd194bfa656b60",
-                "sha256:dd5653e67b149503c68c4018bf07e42eeed6b4e956b24c00ccdf93ac79cdff84",
-                "sha256:de5695a6f1d8340b12a5d6d4484290ee74d61e467c39ff03b39e30df62cf83a0",
-                "sha256:e0ac8959c929593fee38da1c2b64ee9778733cdf03c482c9ff1d508b6b593b2b",
-                "sha256:e1b25e3ad6c909f398df8921780d6a3d120d8c09466720226fc621605b6f92b1",
-                "sha256:e633940f28c1e913615fd624fcdd72fdba807bf53ea6925d6a588e84e1151531",
-                "sha256:e89df2958e5159b811af9ff0f92614dabf4ff617c03a4c1c6ff53bf1c399e0e1",
-                "sha256:ea9f9c6034ea2d93d9147818f17c2a0860d41b71c38b9ce4d55f21b6f9165a11",
-                "sha256:f645caaf0008bacf349875a974220f1f1da349c5dbe7c4ec93048cdc785a3326",
-                "sha256:f8303414c7b03f794347ad062c0516cee0e15f7a612abd0ce1e25caf6ceb47df",
-                "sha256:fca62a8301b605b954ad2e9c3666f9d97f63872aa4efcae5492baca2056b74ab"
+                "sha256:04e57ab9fbf9607b77f7d057974694b4f6b142da9ed4a199859d9d4d5c63fe96",
+                "sha256:09393e1b2a9461950b1c9a45d5fd251dc7c6f228acab64da1c9c0165d9c7765c",
+                "sha256:0b87549028f680ca955556e3bd57013ab47474c3124dc069faa0b6545b6c9710",
+                "sha256:1000fba1057b92a65daec275aec30586c3de2401ccdcd41f8a5c1e2c87078706",
+                "sha256:1249cbbf3d3b04902ff081ffbb33ce3377fa6e4c7356f759f3cd076cc138d020",
+                "sha256:1920d4ff15ce893210c1f0c0e9d19bfbecb7983c76b33f046c13a8ffbd570252",
+                "sha256:193cbc708ea3aca45e7221ae58f0fd63f933753a9bfb498a3b474878f12caaad",
+                "sha256:1a100c6d595a7f316f1b6f01d20815d916e75ff98c27a01ae817439ea7726329",
+                "sha256:1f30b48dd7fa1474554b0b0f3fdfdd4c13b5c737a3c6284d3cdc424ec0ffff3a",
+                "sha256:203f0c8871d5a7987be20c72442488a0b8cfd0f43b7973771640fc593f56321f",
+                "sha256:246de67b99b6851627d945db38147d1b209a899311b1305dd84916f2b88526c6",
+                "sha256:2dee8e57f052ef5353cf608e0b4c871aee320dd1b87d351c28764fc0ca55f9f4",
+                "sha256:2efb1bd13885392adfda4614c33d3b68dee4921fd0ac1d3988f8cbb7d589e72a",
+                "sha256:2f4ac36d8e2b4cc1aa71df3dd84ff8efbe3bfb97ac41242fbcfc053c67434f46",
+                "sha256:3170c9399da12c9dc66366e9d14da8bf7147e1e9d9ea566067bbce7bb74bd9c2",
+                "sha256:3b1613dd5aee995ec6d4c69f00378bbd07614702a315a2cf6c1d21461fe17c23",
+                "sha256:3bb3d25a8e6c0aedd251753a79ae98a093c7e7b471faa3aa9a93a81431987ace",
+                "sha256:3bb7fda7260735efe66d5107fb7e6af6a7c04c7fce9b2514e04b7a74b06bf5dd",
+                "sha256:41b25eaa7d15909cf3ac4c96088c1f266a9a93ec44f87f1d13d4a0e86c81b982",
+                "sha256:45de3f87179c1823e6d9e32156fb14c1927fcc9aba21433f088fdfb555b77c10",
+                "sha256:46fb8c61d794b78ec7134a715a3e564aafc8f6b5e338417cb19fe9f57a5a9bf2",
+                "sha256:48021783bdf96e3d6de03a6e39a1171ed5bd7e8bb93fc84cc649d11490f87cea",
+                "sha256:4957669ef390f0e6719db3613ab3a7631e68424604a7b448f079bee145da6e09",
+                "sha256:5e86d77b090dbddbe78867a0275cb4df08ea195e660f1f7f13435a4649e954e5",
+                "sha256:6339d047dab2780cc6220f46306628e04d9750f02f983ddb37439ca47ced7149",
+                "sha256:681eb3d7e02e3c3655d1b16059fbfb605ac464c834a0c629048a30fad2b27489",
+                "sha256:6c409c0deba34f147f77efaa67b8e4bb83d2f11c8806405f76397ae5b8c0d1c9",
+                "sha256:7095f6fbfaa55defb6b733cfeb14efaae7a29f0b59d8cf213be4e7ca0b857b80",
+                "sha256:70c610f6cbe4b9fce272c407dd9d07e33e6bf7b4aa1b7ffb6f6ded8e634e3592",
+                "sha256:72814c01533f51d68702802d74f77ea026b5ec52793c791e2da806a3844a46c3",
+                "sha256:7a4826ad2bd6b07ca615c74ab91f32f6c96d08f6fcc3902ceeedaec8cdc3bcd6",
+                "sha256:7c70087bfee18a42b4040bb9ec1ca15a08242cf5867c58726530bdf3945672ed",
+                "sha256:855eafa5d5a2034b4621c74925d89c5efef61418570e5ef9b37717d9c796419c",
+                "sha256:8700f06d0ce6f128de3ccdbc1acaea1ee264d2caa9ca05daaf492fde7c2a7200",
+                "sha256:89f1b185a01fe560bc8ae5f619e924407efca2191b56ce749ec84982fc59a32a",
+                "sha256:8b2c760cfc7042b27ebdb4a43a4453bd829a5742503599144d54a032c5dc7e9e",
+                "sha256:8c2f5e83493748286002f9369f3e6607c565a6a90425a3a1fef5ae32a36d749d",
+                "sha256:8e098148dd37b4ce3baca71fb394c81dc5d9c7728c95df695d2dca218edf40e6",
+                "sha256:94aea8eff76ee6d1cdacb07dd2123a68283cb5569e0250feab1240058f53b623",
+                "sha256:95eb302ff792e12aba9a8b8f8474ab229a83c103d74a750ec0bd1c1eea32e669",
+                "sha256:9bd9b3b31adcb054116447ea22caa61a285d92e94d710aa5ec97992ff5eb7cf3",
+                "sha256:9e608aafdb55eb9f255034709e20d5a83b6d60c054df0802fa9c9883d0a937aa",
+                "sha256:a103b3a7069b62f5d4890ae1b8f0597618f628b286b03d4bc9195230b154bfa9",
+                "sha256:a386ebe437176aab38c041de1260cd3ea459c6ce5263594399880bbc398225b2",
+                "sha256:a38856a971c602f98472050165cea2cdc97709240373041b69030be15047691f",
+                "sha256:a401b4598e5d3f4a9a811f3daf42ee2291790c7f9d74b18d75d6e21dda98a1a1",
+                "sha256:a7647ebdfb9682b7bb97e2a5e7cb6ae735b1c25008a70b906aecca294ee96cf4",
+                "sha256:aaf63899c94de41fe3cf934601b0f7ccb6b428c6e4eeb80da72c58eab077b19a",
+                "sha256:b0dac0ff919ba34d4df1b6131f59ce95b08b9065233446be7e459f95554c0dc8",
+                "sha256:baacc6aee0b2ef6f3d308e197b5d7a81c0e70b06beae1f1fcacffdbd124fe0e3",
+                "sha256:bf420121d4c8dce6b889f0e8e4ec0ca34b7f40186203f06a946fa0276ba54029",
+                "sha256:c04a46716adde8d927adb9457bbe39cf473e1e2c2f5d0a16ceb837e5d841ad4f",
+                "sha256:c0b21078a4b56965e2b12f247467b234734491897e99c1d51cee628da9786959",
+                "sha256:c1c76a1743432b4b60ab3358c937a3fe1341c828ae6194108a94c69028247f22",
+                "sha256:c4983bf937209c57240cff65906b18bb35e64ae872da6a0db937d7b4af845dd7",
+                "sha256:c4fb39a81950ec280984b3a44f5bd12819953dc5fa3a7e6fa7a80db5ee853952",
+                "sha256:c57921cda3a80d0f2b8aec7e25c8aa14479ea92b5b51b6876d975d925a2ea346",
+                "sha256:c8063cf17b19661471ecbdb3df1c84f24ad2e389e326ccaf89e3fb2484d8dd7e",
+                "sha256:ccd16eb18a849fd8dcb23e23380e2f0a354e8daa0c984b8a732d9cfaba3a776d",
+                "sha256:cd6dbe0238f7743d0efe563ab46294f54f9bc8f4b9bcf57c3c666cc5bc9d1299",
+                "sha256:d62e51710986674142526ab9f78663ca2b0726066ae26b78b22e0f5e571238dd",
+                "sha256:db901e2ac34c931d73054d9797383d0f8009991e723dab15109740a63e7f902a",
+                "sha256:e03b8895a6990c9ab2cdcd0f2fe44088ca1c65ae592b8f795c3294af00a461c3",
+                "sha256:e1c8a2f4c69e08e89632defbfabec2feb8a8d99edc9f89ce33c4b9e36ab63037",
+                "sha256:e4b749b9cc6ee664a3300bb3a273c1ca8068c46be705b6c31cf5d276f8628a94",
+                "sha256:e6a5bf2cba5ae1bb80b154ed68a3cfa2fa00fde979a7f50d6598d3e17d9ac20c",
+                "sha256:e857a2232ba53ae940d3456f7533ce6ca98b81917d47adc3c7fd55dad8fab858",
+                "sha256:ee4006268ed33370957f55bf2e6f4d263eaf4dc3cfc473d1d90baff6ed36ce4a",
+                "sha256:eef9df1eefada2c09a5e7a40991b9fc6ac6ef20b1372abd48d2794a316dc0449",
+                "sha256:f058f6963fd82eb143c692cecdc89e075fa0828db2e5b291070485390b2f1c9c",
+                "sha256:f25c229a6ba38a35ae6e25ca1264621cc25d4d38dca2942a7fce0b67a4efe918",
+                "sha256:f2a1d0fd4242bd8643ce6f98927cf9c04540af6efa92323e9d3124f57727bfc1",
+                "sha256:f7560358a6811e52e9c4d142d497f1a6e10103d3a6881f18d04dbce3729c0e2c",
+                "sha256:f779d3ad205f108d14e99bb3859aa7dd8e9c68874617c72354d7ecaec2a054ac",
+                "sha256:f87f746ee241d30d6ed93969de31e5ffd09a2961a051e60ae6bddde9ec3583aa"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.1.0"
+            "version": "==3.2.0"
         },
         "click": {
             "hashes": [
-                "sha256:7682dc8afb30297001674575ea00d1814d808d6a36af415a82bd481d37ba7b8e",
-                "sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48"
+                "sha256:48ee849951919527a045bfe3bf7baa8a959c423134e1a5b98c05c20ba75a1cbd",
+                "sha256:fa244bb30b3b5ee2cae3da8f55c9e5e0c0e86093306301fb418eb9dc40fbded5"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==8.1.3"
+            "version": "==8.1.6"
         },
         "docutils": {
             "hashes": [
                 "sha256:96f387a2c5562db4476f09f13bbab2192e764cac08ebbf3a34a95d9b1e4a59d6",
                 "sha256:f08a4e276c3a1583a86dce3e34aba3fe04d02bba2dd51ed16106244e8a923e3b"
             ],
             "markers": "python_version >= '3.7'",
@@ -158,19 +158,19 @@
                 "sha256:6088930bfe239f0e6710546ab9c19c9ef35e29792895fed6e6e31a023a182a61"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==3.1.2"
         },
         "markdown": {
             "hashes": [
-                "sha256:cbb516f16218e643d8e0a95b309f77eb118cb138d39a4f27851e6a63581db874",
-                "sha256:f5da449a6e1c989a4cea2631aa8ee67caa5a2ef855d551c88f9e309f4634c621"
+                "sha256:225c6123522495d4119a90b3a3ba31a1e87a70369e03f14799ea9c0d7183a3d6",
+                "sha256:a4c1b65c0957b4bd9e7d86ddc7b3c9868fb9670660f6f99f6d1bca8954d5a941"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==3.3.7"
+            "markers": "python_version >= '3.7'",
+            "version": "==3.4.4"
         },
         "markupsafe": {
             "hashes": [
                 "sha256:05fb21170423db021895e1ea1e1f3ab3adb85d1c2333cbc2310f2a26bc77272e",
                 "sha256:0a4e4a1aff6c7ac4cd55792abf96c915634c2b97e3cc1c7129578aa68ebd754e",
                 "sha256:10bbfe99883db80bdbaff2dcf681dfc6533a614f700da1287707e8a5d78a8431",
                 "sha256:134da1eca9ec0ae528110ccc9e48041e0828d79f24121a1a146161103c76e686",
@@ -230,81 +230,97 @@
                 "sha256:70775750742b25c0d8f36c55aed03d24c3384d17c951b3175d898bd778ef0307"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==1.3.4"
         },
         "mkdocs": {
             "hashes": [
-                "sha256:5955093bbd4dd2e9403c5afaf57324ad8b04f16886512a3ee6ef828956481c57",
-                "sha256:6ee46d309bda331aac915cd24aab882c179a933bd9e77b80ce7d2eaaa3f689dd"
+                "sha256:67e889f8d8ba1fe5decdfc59f5f8f21d6a8925a129339e93dede303bdea03a98",
+                "sha256:f2f323c62fffdf1b71b84849e39aef56d6852b3f0a5571552bca32cefc650209"
             ],
             "index": "pypi",
-            "version": "==1.4.3"
+            "version": "==1.5.1"
         },
         "packaging": {
             "hashes": [
                 "sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61",
                 "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==23.1"
         },
+        "pathspec": {
+            "hashes": [
+                "sha256:1d6ed233af05e679efb96b1851550ea95bbb64b7c490b0f5aa52996c11e92a20",
+                "sha256:e0d8d0ac2f12da61956eb2306b69f9469b42f4deb0f3cb6ed47b9cce9996ced3"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==0.11.2"
+        },
+        "platformdirs": {
+            "hashes": [
+                "sha256:b45696dab2d7cc691a3226759c0d3b00c47c8b6e293d96f6436f733303f77f6d",
+                "sha256:d7c24979f292f916dc9cbf8648319032f551ea8c49a4c9bf2fb556a02070ec1d"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==3.10.0"
+        },
         "python-dateutil": {
             "hashes": [
                 "sha256:0123cacc1627ae19ddf3c27a5de5bd67ee4586fbdd6440d9748f8abb483d3e86",
                 "sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==2.8.2"
         },
         "pyyaml": {
             "hashes": [
-                "sha256:01b45c0191e6d66c470b6cf1b9531a771a83c1c4208272ead47a3ae4f2f603bf",
-                "sha256:0283c35a6a9fbf047493e3a0ce8d79ef5030852c51e9d911a27badfde0605293",
-                "sha256:055d937d65826939cb044fc8c9b08889e8c743fdc6a32b33e2390f66013e449b",
-                "sha256:07751360502caac1c067a8132d150cf3d61339af5691fe9e87803040dbc5db57",
-                "sha256:0b4624f379dab24d3725ffde76559cff63d9ec94e1736b556dacdfebe5ab6d4b",
-                "sha256:0ce82d761c532fe4ec3f87fc45688bdd3a4c1dc5e0b4a19814b9009a29baefd4",
-                "sha256:1e4747bc279b4f613a09eb64bba2ba602d8a6664c6ce6396a4d0cd413a50ce07",
-                "sha256:213c60cd50106436cc818accf5baa1aba61c0189ff610f64f4a3e8c6726218ba",
-                "sha256:231710d57adfd809ef5d34183b8ed1eeae3f76459c18fb4a0b373ad56bedcdd9",
-                "sha256:277a0ef2981ca40581a47093e9e2d13b3f1fbbeffae064c1d21bfceba2030287",
-                "sha256:2cd5df3de48857ed0544b34e2d40e9fac445930039f3cfe4bcc592a1f836d513",
-                "sha256:40527857252b61eacd1d9af500c3337ba8deb8fc298940291486c465c8b46ec0",
-                "sha256:432557aa2c09802be39460360ddffd48156e30721f5e8d917f01d31694216782",
-                "sha256:473f9edb243cb1935ab5a084eb238d842fb8f404ed2193a915d1784b5a6b5fc0",
-                "sha256:48c346915c114f5fdb3ead70312bd042a953a8ce5c7106d5bfb1a5254e47da92",
-                "sha256:50602afada6d6cbfad699b0c7bb50d5ccffa7e46a3d738092afddc1f9758427f",
-                "sha256:68fb519c14306fec9720a2a5b45bc9f0c8d1b9c72adf45c37baedfcd949c35a2",
-                "sha256:77f396e6ef4c73fdc33a9157446466f1cff553d979bd00ecb64385760c6babdc",
-                "sha256:81957921f441d50af23654aa6c5e5eaf9b06aba7f0a19c18a538dc7ef291c5a1",
-                "sha256:819b3830a1543db06c4d4b865e70ded25be52a2e0631ccd2f6a47a2822f2fd7c",
-                "sha256:897b80890765f037df3403d22bab41627ca8811ae55e9a722fd0392850ec4d86",
-                "sha256:98c4d36e99714e55cfbaaee6dd5badbc9a1ec339ebfc3b1f52e293aee6bb71a4",
-                "sha256:9df7ed3b3d2e0ecfe09e14741b857df43adb5a3ddadc919a2d94fbdf78fea53c",
-                "sha256:9fa600030013c4de8165339db93d182b9431076eb98eb40ee068700c9c813e34",
-                "sha256:a80a78046a72361de73f8f395f1f1e49f956c6be882eed58505a15f3e430962b",
-                "sha256:afa17f5bc4d1b10afd4466fd3a44dc0e245382deca5b3c353d8b757f9e3ecb8d",
-                "sha256:b3d267842bf12586ba6c734f89d1f5b871df0273157918b0ccefa29deb05c21c",
-                "sha256:b5b9eccad747aabaaffbc6064800670f0c297e52c12754eb1d976c57e4f74dcb",
-                "sha256:bfaef573a63ba8923503d27530362590ff4f576c626d86a9fed95822a8255fd7",
-                "sha256:c5687b8d43cf58545ade1fe3e055f70eac7a5a1a0bf42824308d868289a95737",
-                "sha256:cba8c411ef271aa037d7357a2bc8f9ee8b58b9965831d9e51baf703280dc73d3",
-                "sha256:d15a181d1ecd0d4270dc32edb46f7cb7733c7c508857278d3d378d14d606db2d",
-                "sha256:d4b0ba9512519522b118090257be113b9468d804b19d63c71dbcf4a48fa32358",
-                "sha256:d4db7c7aef085872ef65a8fd7d6d09a14ae91f691dec3e87ee5ee0539d516f53",
-                "sha256:d4eccecf9adf6fbcc6861a38015c2a64f38b9d94838ac1810a9023a0609e1b78",
-                "sha256:d67d839ede4ed1b28a4e8909735fc992a923cdb84e618544973d7dfc71540803",
-                "sha256:daf496c58a8c52083df09b80c860005194014c3698698d1a57cbcfa182142a3a",
-                "sha256:dbad0e9d368bb989f4515da330b88a057617d16b6a8245084f1b05400f24609f",
-                "sha256:e61ceaab6f49fb8bdfaa0f92c4b57bcfbea54c09277b1b4f7ac376bfb7a7c174",
-                "sha256:f84fbc98b019fef2ee9a1cb3ce93e3187a6df0b2538a651bfb890254ba9f90b5"
+                "sha256:062582fca9fabdd2c8b54a3ef1c978d786e0f6b3a1510e0ac93ef59e0ddae2bc",
+                "sha256:1635fd110e8d85d55237ab316b5b011de701ea0f29d07611174a1b42f1444741",
+                "sha256:184c5108a2aca3c5b3d3bf9395d50893a7ab82a38004c8f61c258d4428e80206",
+                "sha256:18aeb1bf9a78867dc38b259769503436b7c72f7a1f1f4c93ff9a17de54319b27",
+                "sha256:1d4c7e777c441b20e32f52bd377e0c409713e8bb1386e1099c2415f26e479595",
+                "sha256:1e2722cc9fbb45d9b87631ac70924c11d3a401b2d7f410cc0e3bbf249f2dca62",
+                "sha256:1fe35611261b29bd1de0070f0b2f47cb6ff71fa6595c077e42bd0c419fa27b98",
+                "sha256:28c119d996beec18c05208a8bd78cbe4007878c6dd15091efb73a30e90539696",
+                "sha256:42f8152b8dbc4fe7d96729ec2b99c7097d656dc1213a3229ca5383f973a5ed6d",
+                "sha256:4fb147e7a67ef577a588a0e2c17b6db51dda102c71de36f8549b6816a96e1867",
+                "sha256:50550eb667afee136e9a77d6dc71ae76a44df8b3e51e41b77f6de2932bfe0f47",
+                "sha256:510c9deebc5c0225e8c96813043e62b680ba2f9c50a08d3724c7f28a747d1486",
+                "sha256:5773183b6446b2c99bb77e77595dd486303b4faab2b086e7b17bc6bef28865f6",
+                "sha256:596106435fa6ad000c2991a98fa58eeb8656ef2325d7e158344fb33864ed87e3",
+                "sha256:6965a7bc3cf88e5a1c3bd2e0b5c22f8d677dc88a455344035f03399034eb3007",
+                "sha256:69b023b2b4daa7548bcfbd4aa3da05b3a74b772db9e23b982788168117739938",
+                "sha256:704219a11b772aea0d8ecd7058d0082713c3562b4e271b849ad7dc4a5c90c13c",
+                "sha256:7e07cbde391ba96ab58e532ff4803f79c4129397514e1413a7dc761ccd755735",
+                "sha256:81e0b275a9ecc9c0c0c07b4b90ba548307583c125f54d5b6946cfee6360c733d",
+                "sha256:9046c58c4395dff28dd494285c82ba00b546adfc7ef001486fbf0324bc174fba",
+                "sha256:9eb6caa9a297fc2c2fb8862bc5370d0303ddba53ba97e71f08023b6cd73d16a8",
+                "sha256:a0cd17c15d3bb3fa06978b4e8958dcdc6e0174ccea823003a106c7d4d7899ac5",
+                "sha256:afd7e57eddb1a54f0f1a974bc4391af8bcce0b444685d936840f125cf046d5bd",
+                "sha256:b1275ad35a5d18c62a7220633c913e1b42d44b46ee12554e5fd39c70a243d6a3",
+                "sha256:b786eecbdf8499b9ca1d697215862083bd6d2a99965554781d0d8d1ad31e13a0",
+                "sha256:ba336e390cd8e4d1739f42dfe9bb83a3cc2e80f567d8805e11b46f4a943f5515",
+                "sha256:baa90d3f661d43131ca170712d903e6295d1f7a0f595074f151c0aed377c9b9c",
+                "sha256:bc1bf2925a1ecd43da378f4db9e4f799775d6367bdb94671027b73b393a7c42c",
+                "sha256:bd4af7373a854424dabd882decdc5579653d7868b8fb26dc7d0e99f823aa5924",
+                "sha256:bf07ee2fef7014951eeb99f56f39c9bb4af143d8aa3c21b1677805985307da34",
+                "sha256:bfdf460b1736c775f2ba9f6a92bca30bc2095067b8a9d77876d1fad6cc3b4a43",
+                "sha256:c8098ddcc2a85b61647b2590f825f3db38891662cfc2fc776415143f599bb859",
+                "sha256:d2b04aac4d386b172d5b9692e2d2da8de7bfb6c387fa4f801fbf6fb2e6ba4673",
+                "sha256:d858aa552c999bc8a8d57426ed01e40bef403cd8ccdd0fc5f6f04a00414cac2a",
+                "sha256:f003ed9ad21d6a4713f0a9b5a7a0a79e08dd0f221aff4525a2be4c346ee60aab",
+                "sha256:f22ac1c3cac4dbc50079e965eba2c1058622631e526bd9afd45fedd49ba781fa",
+                "sha256:faca3bdcf85b2fc05d06ff3fbc1f83e1391b3e724afa3feba7d13eeab355484c",
+                "sha256:fca0e3a251908a499833aa292323f32437106001d436eca0e6e7833256674585",
+                "sha256:fd1592b3fdf65fff2ad0004b5e363300ef59ced41c2e6b3a99d4089fa8c5435d",
+                "sha256:fd66fc5d0da6d9815ba2cebeb4205f95818ff4b79c3ebe268e75d961704af52f"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==6.0"
+            "version": "==6.0.1"
         },
         "pyyaml-env-tag": {
             "hashes": [
                 "sha256:70092675bda14fdec33b31ba77e7543de9ddc88f2e5b99160396572d11525bdb",
                 "sha256:af31106dec8a4d68c60207c1886031cbf839b68aa7abccdb19868200532c2069"
             ],
             "markers": "python_version >= '3.6'",
@@ -332,19 +348,19 @@
                 "sha256:f463434305e0336248cac9c2dc8076b707d8a12d019dd349f5c1e382dd1ae1b9"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==1.0.0"
         },
         "urllib3": {
             "hashes": [
-                "sha256:48e7fafa40319d358848e1bc6809b208340fafe2096f1725d05d67443d0483d1",
-                "sha256:bee28b5e56addb8226c96f7f13ac28cb4c301dd5ea8a6ca179c0b9835e032825"
+                "sha256:8d22f86aae8ef5e410d4f539fde9ce6b2113a001bb4d189e0aed70642d602b11",
+                "sha256:de7df1803967d2c2a98e4b11bb7d6bd9210474c46e8a0401514e3a42a75ebde4"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.0.3"
+            "version": "==2.0.4"
         },
         "watchdog": {
             "hashes": [
                 "sha256:0e06ab8858a76e1219e68c7573dfeba9dd1c0219476c5a44d5333b01d7e1743a",
                 "sha256:13bbbb462ee42ec3c5723e1205be8ced776f05b100e4737518c67c8325cf6100",
                 "sha256:233b5817932685d39a7896b1090353fc8efc1ef99c9c054e46c8002561252fb8",
                 "sha256:25f70b4aa53bd743729c7475d7ec41093a580528b100e9a8c5b5efe8899592fc",
@@ -383,116 +399,116 @@
                 "sha256:e7b23fc8b2cd06d3dec0692baabecb249dda94e06a617901ff03a6c56fd71693"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.3.post1"
         },
         "certifi": {
             "hashes": [
-                "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7",
-                "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"
+                "sha256:539cc1d13202e33ca466e88b2807e29f4c13049d6d87031a3c110744495cb082",
+                "sha256:92d6037539857d8206b8f6ae472e8b77db8058fec5937a1ef3f54304089edbb9"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==2023.5.7"
+            "version": "==2023.7.22"
         },
         "cfgv": {
             "hashes": [
                 "sha256:c6a0883f3917a037485059700b9e75da2464e6c27051014ad85ba6aaa5884426",
                 "sha256:f5a830efb9ce7a445376bb66ec94c638a9787422f96264c98edc6bdeed8ab736"
             ],
             "markers": "python_full_version >= '3.6.1'",
             "version": "==3.3.1"
         },
         "charset-normalizer": {
             "hashes": [
-                "sha256:04afa6387e2b282cf78ff3dbce20f0cc071c12dc8f685bd40960cc68644cfea6",
-                "sha256:04eefcee095f58eaabe6dc3cc2262f3bcd776d2c67005880894f447b3f2cb9c1",
-                "sha256:0be65ccf618c1e7ac9b849c315cc2e8a8751d9cfdaa43027d4f6624bd587ab7e",
-                "sha256:0c95f12b74681e9ae127728f7e5409cbbef9cd914d5896ef238cc779b8152373",
-                "sha256:0ca564606d2caafb0abe6d1b5311c2649e8071eb241b2d64e75a0d0065107e62",
-                "sha256:10c93628d7497c81686e8e5e557aafa78f230cd9e77dd0c40032ef90c18f2230",
-                "sha256:11d117e6c63e8f495412d37e7dc2e2fff09c34b2d09dbe2bee3c6229577818be",
-                "sha256:11d3bcb7be35e7b1bba2c23beedac81ee893ac9871d0ba79effc7fc01167db6c",
-                "sha256:12a2b561af122e3d94cdb97fe6fb2bb2b82cef0cdca131646fdb940a1eda04f0",
-                "sha256:12d1a39aa6b8c6f6248bb54550efcc1c38ce0d8096a146638fd4738e42284448",
-                "sha256:1435ae15108b1cb6fffbcea2af3d468683b7afed0169ad718451f8db5d1aff6f",
-                "sha256:1c60b9c202d00052183c9be85e5eaf18a4ada0a47d188a83c8f5c5b23252f649",
-                "sha256:1e8fcdd8f672a1c4fc8d0bd3a2b576b152d2a349782d1eb0f6b8e52e9954731d",
-                "sha256:20064ead0717cf9a73a6d1e779b23d149b53daf971169289ed2ed43a71e8d3b0",
-                "sha256:21fa558996782fc226b529fdd2ed7866c2c6ec91cee82735c98a197fae39f706",
-                "sha256:22908891a380d50738e1f978667536f6c6b526a2064156203d418f4856d6e86a",
-                "sha256:3160a0fd9754aab7d47f95a6b63ab355388d890163eb03b2d2b87ab0a30cfa59",
-                "sha256:322102cdf1ab682ecc7d9b1c5eed4ec59657a65e1c146a0da342b78f4112db23",
-                "sha256:34e0a2f9c370eb95597aae63bf85eb5e96826d81e3dcf88b8886012906f509b5",
-                "sha256:3573d376454d956553c356df45bb824262c397c6e26ce43e8203c4c540ee0acb",
-                "sha256:3747443b6a904001473370d7810aa19c3a180ccd52a7157aacc264a5ac79265e",
-                "sha256:38e812a197bf8e71a59fe55b757a84c1f946d0ac114acafaafaf21667a7e169e",
-                "sha256:3a06f32c9634a8705f4ca9946d667609f52cf130d5548881401f1eb2c39b1e2c",
-                "sha256:3a5fc78f9e3f501a1614a98f7c54d3969f3ad9bba8ba3d9b438c3bc5d047dd28",
-                "sha256:3d9098b479e78c85080c98e1e35ff40b4a31d8953102bb0fd7d1b6f8a2111a3d",
-                "sha256:3dc5b6a8ecfdc5748a7e429782598e4f17ef378e3e272eeb1340ea57c9109f41",
-                "sha256:4155b51ae05ed47199dc5b2a4e62abccb274cee6b01da5b895099b61b1982974",
-                "sha256:49919f8400b5e49e961f320c735388ee686a62327e773fa5b3ce6721f7e785ce",
-                "sha256:53d0a3fa5f8af98a1e261de6a3943ca631c526635eb5817a87a59d9a57ebf48f",
-                "sha256:5f008525e02908b20e04707a4f704cd286d94718f48bb33edddc7d7b584dddc1",
-                "sha256:628c985afb2c7d27a4800bfb609e03985aaecb42f955049957814e0491d4006d",
-                "sha256:65ed923f84a6844de5fd29726b888e58c62820e0769b76565480e1fdc3d062f8",
-                "sha256:6734e606355834f13445b6adc38b53c0fd45f1a56a9ba06c2058f86893ae8017",
-                "sha256:6baf0baf0d5d265fa7944feb9f7451cc316bfe30e8df1a61b1bb08577c554f31",
-                "sha256:6f4f4668e1831850ebcc2fd0b1cd11721947b6dc7c00bf1c6bd3c929ae14f2c7",
-                "sha256:6f5c2e7bc8a4bf7c426599765b1bd33217ec84023033672c1e9a8b35eaeaaaf8",
-                "sha256:6f6c7a8a57e9405cad7485f4c9d3172ae486cfef1344b5ddd8e5239582d7355e",
-                "sha256:7381c66e0561c5757ffe616af869b916c8b4e42b367ab29fedc98481d1e74e14",
-                "sha256:73dc03a6a7e30b7edc5b01b601e53e7fc924b04e1835e8e407c12c037e81adbd",
-                "sha256:74db0052d985cf37fa111828d0dd230776ac99c740e1a758ad99094be4f1803d",
-                "sha256:75f2568b4189dda1c567339b48cba4ac7384accb9c2a7ed655cd86b04055c795",
-                "sha256:78cacd03e79d009d95635e7d6ff12c21eb89b894c354bd2b2ed0b4763373693b",
-                "sha256:80d1543d58bd3d6c271b66abf454d437a438dff01c3e62fdbcd68f2a11310d4b",
-                "sha256:830d2948a5ec37c386d3170c483063798d7879037492540f10a475e3fd6f244b",
-                "sha256:891cf9b48776b5c61c700b55a598621fdb7b1e301a550365571e9624f270c203",
-                "sha256:8f25e17ab3039b05f762b0a55ae0b3632b2e073d9c8fc88e89aca31a6198e88f",
-                "sha256:9a3267620866c9d17b959a84dd0bd2d45719b817245e49371ead79ed4f710d19",
-                "sha256:a04f86f41a8916fe45ac5024ec477f41f886b3c435da2d4e3d2709b22ab02af1",
-                "sha256:aaf53a6cebad0eae578f062c7d462155eada9c172bd8c4d250b8c1d8eb7f916a",
-                "sha256:abc1185d79f47c0a7aaf7e2412a0eb2c03b724581139193d2d82b3ad8cbb00ac",
-                "sha256:ac0aa6cd53ab9a31d397f8303f92c42f534693528fafbdb997c82bae6e477ad9",
-                "sha256:ac3775e3311661d4adace3697a52ac0bab17edd166087d493b52d4f4f553f9f0",
-                "sha256:b06f0d3bf045158d2fb8837c5785fe9ff9b8c93358be64461a1089f5da983137",
-                "sha256:b116502087ce8a6b7a5f1814568ccbd0e9f6cfd99948aa59b0e241dc57cf739f",
-                "sha256:b82fab78e0b1329e183a65260581de4375f619167478dddab510c6c6fb04d9b6",
-                "sha256:bd7163182133c0c7701b25e604cf1611c0d87712e56e88e7ee5d72deab3e76b5",
-                "sha256:c36bcbc0d5174a80d6cccf43a0ecaca44e81d25be4b7f90f0ed7bcfbb5a00909",
-                "sha256:c3af8e0f07399d3176b179f2e2634c3ce9c1301379a6b8c9c9aeecd481da494f",
-                "sha256:c84132a54c750fda57729d1e2599bb598f5fa0344085dbde5003ba429a4798c0",
-                "sha256:cb7b2ab0188829593b9de646545175547a70d9a6e2b63bf2cd87a0a391599324",
-                "sha256:cca4def576f47a09a943666b8f829606bcb17e2bc2d5911a46c8f8da45f56755",
-                "sha256:cf6511efa4801b9b38dc5546d7547d5b5c6ef4b081c60b23e4d941d0eba9cbeb",
-                "sha256:d16fd5252f883eb074ca55cb622bc0bee49b979ae4e8639fff6ca3ff44f9f854",
-                "sha256:d2686f91611f9e17f4548dbf050e75b079bbc2a82be565832bc8ea9047b61c8c",
-                "sha256:d7fc3fca01da18fbabe4625d64bb612b533533ed10045a2ac3dd194bfa656b60",
-                "sha256:dd5653e67b149503c68c4018bf07e42eeed6b4e956b24c00ccdf93ac79cdff84",
-                "sha256:de5695a6f1d8340b12a5d6d4484290ee74d61e467c39ff03b39e30df62cf83a0",
-                "sha256:e0ac8959c929593fee38da1c2b64ee9778733cdf03c482c9ff1d508b6b593b2b",
-                "sha256:e1b25e3ad6c909f398df8921780d6a3d120d8c09466720226fc621605b6f92b1",
-                "sha256:e633940f28c1e913615fd624fcdd72fdba807bf53ea6925d6a588e84e1151531",
-                "sha256:e89df2958e5159b811af9ff0f92614dabf4ff617c03a4c1c6ff53bf1c399e0e1",
-                "sha256:ea9f9c6034ea2d93d9147818f17c2a0860d41b71c38b9ce4d55f21b6f9165a11",
-                "sha256:f645caaf0008bacf349875a974220f1f1da349c5dbe7c4ec93048cdc785a3326",
-                "sha256:f8303414c7b03f794347ad062c0516cee0e15f7a612abd0ce1e25caf6ceb47df",
-                "sha256:fca62a8301b605b954ad2e9c3666f9d97f63872aa4efcae5492baca2056b74ab"
+                "sha256:04e57ab9fbf9607b77f7d057974694b4f6b142da9ed4a199859d9d4d5c63fe96",
+                "sha256:09393e1b2a9461950b1c9a45d5fd251dc7c6f228acab64da1c9c0165d9c7765c",
+                "sha256:0b87549028f680ca955556e3bd57013ab47474c3124dc069faa0b6545b6c9710",
+                "sha256:1000fba1057b92a65daec275aec30586c3de2401ccdcd41f8a5c1e2c87078706",
+                "sha256:1249cbbf3d3b04902ff081ffbb33ce3377fa6e4c7356f759f3cd076cc138d020",
+                "sha256:1920d4ff15ce893210c1f0c0e9d19bfbecb7983c76b33f046c13a8ffbd570252",
+                "sha256:193cbc708ea3aca45e7221ae58f0fd63f933753a9bfb498a3b474878f12caaad",
+                "sha256:1a100c6d595a7f316f1b6f01d20815d916e75ff98c27a01ae817439ea7726329",
+                "sha256:1f30b48dd7fa1474554b0b0f3fdfdd4c13b5c737a3c6284d3cdc424ec0ffff3a",
+                "sha256:203f0c8871d5a7987be20c72442488a0b8cfd0f43b7973771640fc593f56321f",
+                "sha256:246de67b99b6851627d945db38147d1b209a899311b1305dd84916f2b88526c6",
+                "sha256:2dee8e57f052ef5353cf608e0b4c871aee320dd1b87d351c28764fc0ca55f9f4",
+                "sha256:2efb1bd13885392adfda4614c33d3b68dee4921fd0ac1d3988f8cbb7d589e72a",
+                "sha256:2f4ac36d8e2b4cc1aa71df3dd84ff8efbe3bfb97ac41242fbcfc053c67434f46",
+                "sha256:3170c9399da12c9dc66366e9d14da8bf7147e1e9d9ea566067bbce7bb74bd9c2",
+                "sha256:3b1613dd5aee995ec6d4c69f00378bbd07614702a315a2cf6c1d21461fe17c23",
+                "sha256:3bb3d25a8e6c0aedd251753a79ae98a093c7e7b471faa3aa9a93a81431987ace",
+                "sha256:3bb7fda7260735efe66d5107fb7e6af6a7c04c7fce9b2514e04b7a74b06bf5dd",
+                "sha256:41b25eaa7d15909cf3ac4c96088c1f266a9a93ec44f87f1d13d4a0e86c81b982",
+                "sha256:45de3f87179c1823e6d9e32156fb14c1927fcc9aba21433f088fdfb555b77c10",
+                "sha256:46fb8c61d794b78ec7134a715a3e564aafc8f6b5e338417cb19fe9f57a5a9bf2",
+                "sha256:48021783bdf96e3d6de03a6e39a1171ed5bd7e8bb93fc84cc649d11490f87cea",
+                "sha256:4957669ef390f0e6719db3613ab3a7631e68424604a7b448f079bee145da6e09",
+                "sha256:5e86d77b090dbddbe78867a0275cb4df08ea195e660f1f7f13435a4649e954e5",
+                "sha256:6339d047dab2780cc6220f46306628e04d9750f02f983ddb37439ca47ced7149",
+                "sha256:681eb3d7e02e3c3655d1b16059fbfb605ac464c834a0c629048a30fad2b27489",
+                "sha256:6c409c0deba34f147f77efaa67b8e4bb83d2f11c8806405f76397ae5b8c0d1c9",
+                "sha256:7095f6fbfaa55defb6b733cfeb14efaae7a29f0b59d8cf213be4e7ca0b857b80",
+                "sha256:70c610f6cbe4b9fce272c407dd9d07e33e6bf7b4aa1b7ffb6f6ded8e634e3592",
+                "sha256:72814c01533f51d68702802d74f77ea026b5ec52793c791e2da806a3844a46c3",
+                "sha256:7a4826ad2bd6b07ca615c74ab91f32f6c96d08f6fcc3902ceeedaec8cdc3bcd6",
+                "sha256:7c70087bfee18a42b4040bb9ec1ca15a08242cf5867c58726530bdf3945672ed",
+                "sha256:855eafa5d5a2034b4621c74925d89c5efef61418570e5ef9b37717d9c796419c",
+                "sha256:8700f06d0ce6f128de3ccdbc1acaea1ee264d2caa9ca05daaf492fde7c2a7200",
+                "sha256:89f1b185a01fe560bc8ae5f619e924407efca2191b56ce749ec84982fc59a32a",
+                "sha256:8b2c760cfc7042b27ebdb4a43a4453bd829a5742503599144d54a032c5dc7e9e",
+                "sha256:8c2f5e83493748286002f9369f3e6607c565a6a90425a3a1fef5ae32a36d749d",
+                "sha256:8e098148dd37b4ce3baca71fb394c81dc5d9c7728c95df695d2dca218edf40e6",
+                "sha256:94aea8eff76ee6d1cdacb07dd2123a68283cb5569e0250feab1240058f53b623",
+                "sha256:95eb302ff792e12aba9a8b8f8474ab229a83c103d74a750ec0bd1c1eea32e669",
+                "sha256:9bd9b3b31adcb054116447ea22caa61a285d92e94d710aa5ec97992ff5eb7cf3",
+                "sha256:9e608aafdb55eb9f255034709e20d5a83b6d60c054df0802fa9c9883d0a937aa",
+                "sha256:a103b3a7069b62f5d4890ae1b8f0597618f628b286b03d4bc9195230b154bfa9",
+                "sha256:a386ebe437176aab38c041de1260cd3ea459c6ce5263594399880bbc398225b2",
+                "sha256:a38856a971c602f98472050165cea2cdc97709240373041b69030be15047691f",
+                "sha256:a401b4598e5d3f4a9a811f3daf42ee2291790c7f9d74b18d75d6e21dda98a1a1",
+                "sha256:a7647ebdfb9682b7bb97e2a5e7cb6ae735b1c25008a70b906aecca294ee96cf4",
+                "sha256:aaf63899c94de41fe3cf934601b0f7ccb6b428c6e4eeb80da72c58eab077b19a",
+                "sha256:b0dac0ff919ba34d4df1b6131f59ce95b08b9065233446be7e459f95554c0dc8",
+                "sha256:baacc6aee0b2ef6f3d308e197b5d7a81c0e70b06beae1f1fcacffdbd124fe0e3",
+                "sha256:bf420121d4c8dce6b889f0e8e4ec0ca34b7f40186203f06a946fa0276ba54029",
+                "sha256:c04a46716adde8d927adb9457bbe39cf473e1e2c2f5d0a16ceb837e5d841ad4f",
+                "sha256:c0b21078a4b56965e2b12f247467b234734491897e99c1d51cee628da9786959",
+                "sha256:c1c76a1743432b4b60ab3358c937a3fe1341c828ae6194108a94c69028247f22",
+                "sha256:c4983bf937209c57240cff65906b18bb35e64ae872da6a0db937d7b4af845dd7",
+                "sha256:c4fb39a81950ec280984b3a44f5bd12819953dc5fa3a7e6fa7a80db5ee853952",
+                "sha256:c57921cda3a80d0f2b8aec7e25c8aa14479ea92b5b51b6876d975d925a2ea346",
+                "sha256:c8063cf17b19661471ecbdb3df1c84f24ad2e389e326ccaf89e3fb2484d8dd7e",
+                "sha256:ccd16eb18a849fd8dcb23e23380e2f0a354e8daa0c984b8a732d9cfaba3a776d",
+                "sha256:cd6dbe0238f7743d0efe563ab46294f54f9bc8f4b9bcf57c3c666cc5bc9d1299",
+                "sha256:d62e51710986674142526ab9f78663ca2b0726066ae26b78b22e0f5e571238dd",
+                "sha256:db901e2ac34c931d73054d9797383d0f8009991e723dab15109740a63e7f902a",
+                "sha256:e03b8895a6990c9ab2cdcd0f2fe44088ca1c65ae592b8f795c3294af00a461c3",
+                "sha256:e1c8a2f4c69e08e89632defbfabec2feb8a8d99edc9f89ce33c4b9e36ab63037",
+                "sha256:e4b749b9cc6ee664a3300bb3a273c1ca8068c46be705b6c31cf5d276f8628a94",
+                "sha256:e6a5bf2cba5ae1bb80b154ed68a3cfa2fa00fde979a7f50d6598d3e17d9ac20c",
+                "sha256:e857a2232ba53ae940d3456f7533ce6ca98b81917d47adc3c7fd55dad8fab858",
+                "sha256:ee4006268ed33370957f55bf2e6f4d263eaf4dc3cfc473d1d90baff6ed36ce4a",
+                "sha256:eef9df1eefada2c09a5e7a40991b9fc6ac6ef20b1372abd48d2794a316dc0449",
+                "sha256:f058f6963fd82eb143c692cecdc89e075fa0828db2e5b291070485390b2f1c9c",
+                "sha256:f25c229a6ba38a35ae6e25ca1264621cc25d4d38dca2942a7fce0b67a4efe918",
+                "sha256:f2a1d0fd4242bd8643ce6f98927cf9c04540af6efa92323e9d3124f57727bfc1",
+                "sha256:f7560358a6811e52e9c4d142d497f1a6e10103d3a6881f18d04dbce3729c0e2c",
+                "sha256:f779d3ad205f108d14e99bb3859aa7dd8e9c68874617c72354d7ecaec2a054ac",
+                "sha256:f87f746ee241d30d6ed93969de31e5ffd09a2961a051e60ae6bddde9ec3583aa"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.1.0"
+            "version": "==3.2.0"
         },
         "click": {
             "hashes": [
-                "sha256:7682dc8afb30297001674575ea00d1814d808d6a36af415a82bd481d37ba7b8e",
-                "sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48"
+                "sha256:48ee849951919527a045bfe3bf7baa8a959c423134e1a5b98c05c20ba75a1cbd",
+                "sha256:fa244bb30b3b5ee2cae3da8f55c9e5e0c0e86093306301fb418eb9dc40fbded5"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==8.1.3"
+            "version": "==8.1.6"
         },
         "colorama": {
             "hashes": [
                 "sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44",
                 "sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6'",
@@ -565,73 +581,73 @@
                 "sha256:fdec9e8cbf13a5bf63290fc6013d216a4c7232efb51548594ca3631a7f13c3a3"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==7.2.7"
         },
         "distlib": {
             "hashes": [
-                "sha256:14bad2d9b04d3a36127ac97f30b12a19268f211063d8f8ee4f47108896e11b46",
-                "sha256:f35c4b692542ca110de7ef0bea44d73981caeb34ca0b9b6b2e6d7790dda8f80e"
+                "sha256:2e24928bc811348f0feb63014e97aaae3037f2cf48712d51ae61df7fd6075057",
+                "sha256:9dafe54b34a028eafd95039d5e5d4851a13734540f1331060d31c9916e7147a8"
             ],
-            "version": "==0.3.6"
+            "version": "==0.3.7"
         },
         "exceptiongroup": {
             "hashes": [
-                "sha256:232c37c63e4f682982c8b6459f33a8981039e5fb8756b2074364e5055c498c9e",
-                "sha256:d484c3090ba2889ae2928419117447a14daf3c1231d5e30d0aae34f354f01785"
+                "sha256:12c3e887d6485d16943a309616de20ae5582633e0a2eda17f4e10fd61c1e8af5",
+                "sha256:e346e69d186172ca7cf029c8c1d16235aa0e04035e5750b4b95039e65204328f"
             ],
             "markers": "python_version < '3.11'",
-            "version": "==1.1.1"
+            "version": "==1.1.2"
         },
         "filelock": {
             "hashes": [
                 "sha256:002740518d8aa59a26b0c76e10fb8c6e15eae825d34b6fdf670333fd7b938d81",
                 "sha256:cbb791cdea2a72f23da6ac5b5269ab0a0d161e9ef0100e653b69049a7706d1ec"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==3.12.2"
         },
         "flake8": {
             "hashes": [
-                "sha256:3833794e27ff64ea4e9cf5d410082a8b97ff1a06c16aa3d2027339cd0f1195c7",
-                "sha256:c61007e76655af75e6785a931f452915b371dc48f56efd765247c8fe68f2b181"
+                "sha256:d5b3857f07c030bdb5bf41c7f53799571d75c4491748a3adcd47de929e34cd23",
+                "sha256:ffdfce58ea94c6580c77888a86506937f9a1a227dfcd15f245d694ae20a6b6e5"
             ],
             "index": "pypi",
-            "version": "==6.0.0"
+            "version": "==6.1.0"
         },
         "ghp-import": {
             "hashes": [
                 "sha256:8337dd7b50877f163d4c0289bc1f1c7f127550241988d568c1db512c4324a619",
                 "sha256:9c535c4c61193c2df8871222567d7fd7e5014d835f97dc7b7439069e2413d343"
             ],
             "version": "==2.1.0"
         },
         "identify": {
             "hashes": [
-                "sha256:0aac67d5b4812498056d28a9a512a483f5085cc28640b02b258a59dac34301d4",
-                "sha256:986dbfb38b1140e763e413e6feb44cd731faf72d1909543178aa79b0e258265d"
+                "sha256:7243800bce2f58404ed41b7c002e53d4d22bcf3ae1b7900c2d7aefd95394bf7f",
+                "sha256:c22a8ead0d4ca11f1edd6c9418c3220669b3b7533ada0a0ffa6cc0ef85cf9b54"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==2.5.24"
+            "markers": "python_version >= '3.8'",
+            "version": "==2.5.26"
         },
         "idna": {
             "hashes": [
                 "sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4",
                 "sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2"
             ],
             "markers": "python_version >= '3.5'",
             "version": "==3.4"
         },
         "importlib-metadata": {
             "hashes": [
-                "sha256:1aaf550d4f73e5d6783e7acb77aec43d49da8017410afae93822cc9cca98c4d4",
-                "sha256:cb52082e659e97afc5dac71e79de97d8681de3aa07ff18578330904a9d18e5b5"
+                "sha256:3ebb78df84a805d7698245025b975d9d67053cd94c79245ba4b3eb694abe68bb",
+                "sha256:dbace7892d8c0c4ac1ad096662232f831d4e64f4c4545bd53016a3e9d4654743"
             ],
             "markers": "python_version < '3.10'",
-            "version": "==6.7.0"
+            "version": "==6.8.0"
         },
         "iniconfig": {
             "hashes": [
                 "sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3",
                 "sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374"
             ],
             "markers": "python_version >= '3.7'",
@@ -643,19 +659,19 @@
                 "sha256:6088930bfe239f0e6710546ab9c19c9ef35e29792895fed6e6e31a023a182a61"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==3.1.2"
         },
         "markdown": {
             "hashes": [
-                "sha256:cbb516f16218e643d8e0a95b309f77eb118cb138d39a4f27851e6a63581db874",
-                "sha256:f5da449a6e1c989a4cea2631aa8ee67caa5a2ef855d551c88f9e309f4634c621"
+                "sha256:225c6123522495d4119a90b3a3ba31a1e87a70369e03f14799ea9c0d7183a3d6",
+                "sha256:a4c1b65c0957b4bd9e7d86ddc7b3c9868fb9670660f6f99f6d1bca8954d5a941"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==3.3.7"
+            "markers": "python_version >= '3.7'",
+            "version": "==3.4.4"
         },
         "markupsafe": {
             "hashes": [
                 "sha256:05fb21170423db021895e1ea1e1f3ab3adb85d1c2333cbc2310f2a26bc77272e",
                 "sha256:0a4e4a1aff6c7ac4cd55792abf96c915634c2b97e3cc1c7129578aa68ebd754e",
                 "sha256:10bbfe99883db80bdbaff2dcf681dfc6533a614f700da1287707e8a5d78a8431",
                 "sha256:134da1eca9ec0ae528110ccc9e48041e0828d79f24121a1a146161103c76e686",
@@ -723,35 +739,35 @@
                 "sha256:70775750742b25c0d8f36c55aed03d24c3384d17c951b3175d898bd778ef0307"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==1.3.4"
         },
         "mkdocs": {
             "hashes": [
-                "sha256:5955093bbd4dd2e9403c5afaf57324ad8b04f16886512a3ee6ef828956481c57",
-                "sha256:6ee46d309bda331aac915cd24aab882c179a933bd9e77b80ce7d2eaaa3f689dd"
+                "sha256:67e889f8d8ba1fe5decdfc59f5f8f21d6a8925a129339e93dede303bdea03a98",
+                "sha256:f2f323c62fffdf1b71b84849e39aef56d6852b3f0a5571552bca32cefc650209"
             ],
             "index": "pypi",
-            "version": "==1.4.3"
+            "version": "==1.5.1"
         },
         "mkdocs-awesome-pages-plugin": {
             "hashes": [
                 "sha256:be65e36444f5d991f87a90dae37de64e932562f99e362078724c27124834b90a",
                 "sha256:faf5241365f94c1f65ef3cad7ea9d6f0e7a436be7f06013c79c4045db0b2eafc"
             ],
             "index": "pypi",
             "version": "==2.9.1"
         },
         "mkdocs-material": {
             "hashes": [
-                "sha256:5a076524625047bf4ee4da1509ec90626f8fce915839dc07bdae6b59ff4f36f9",
-                "sha256:809ed68427fbab0330b0b07bc93175824c3b98f4187060a5c7b46aa8ae398a75"
+                "sha256:58bb2f11ef240632e176d6f0f7d1cff06be1d11c696a5a1b553b808b4280ed47",
+                "sha256:71940cdfca84ab296b6362889c25395b1621273fb16c93deda257adb7ff44ec8"
             ],
             "index": "pypi",
-            "version": "==9.1.17"
+            "version": "==9.1.21"
         },
         "mkdocs-material-extensions": {
             "hashes": [
                 "sha256:9c003da71e2cc2493d910237448c672e00cefc800d3d6ae93d2fc69979e3bd93",
                 "sha256:e41d9f38e4798b6617ad98ca8f7f1157b1e4385ac1459ca1e4ea219b556df945"
             ],
             "markers": "python_version >= '3.7'",
@@ -777,21 +793,29 @@
             "hashes": [
                 "sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61",
                 "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==23.1"
         },
+        "pathspec": {
+            "hashes": [
+                "sha256:1d6ed233af05e679efb96b1851550ea95bbb64b7c490b0f5aa52996c11e92a20",
+                "sha256:e0d8d0ac2f12da61956eb2306b69f9469b42f4deb0f3cb6ed47b9cce9996ced3"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==0.11.2"
+        },
         "platformdirs": {
             "hashes": [
-                "sha256:b0cabcb11063d21a0b261d557acb0a9d2126350e63b70cdf7db6347baea456dc",
-                "sha256:ca9ed98ce73076ba72e092b23d3c93ea6c4e186b3f1c3dad6edd98ff6ffcca2e"
+                "sha256:b45696dab2d7cc691a3226759c0d3b00c47c8b6e293d96f6436f733303f77f6d",
+                "sha256:d7c24979f292f916dc9cbf8648319032f551ea8c49a4c9bf2fb556a02070ec1d"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.8.0"
+            "version": "==3.10.0"
         },
         "pluggy": {
             "hashes": [
                 "sha256:c2fd55a7d7a3863cba1a013e4e2414658b1d07b6bc57b3919e0c63c9abb99849",
                 "sha256:d12f0c4b579b15f5e054301bb226ee85eeeba08ffec228092f8defbaa3a4c4b3"
             ],
             "markers": "python_version >= '3.7'",
@@ -803,43 +827,43 @@
                 "sha256:a2256f489cd913d575c145132ae196fe335da32d91a8294b7afe6622335dd023"
             ],
             "index": "pypi",
             "version": "==3.3.3"
         },
         "pycodestyle": {
             "hashes": [
-                "sha256:347187bdb476329d98f695c213d7295a846d1152ff4fe9bacb8a9590b8ee7053",
-                "sha256:8a4eaf0d0495c7395bdab3589ac2db602797d76207242c17d470186815706610"
+                "sha256:259bcc17857d8a8b3b4a2327324b79e5f020a13c16074670f9c8c8f872ea76d0",
+                "sha256:5d1013ba8dc7895b548be5afb05740ca82454fd899971563d2ef625d090326f8"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==2.10.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==2.11.0"
         },
         "pyflakes": {
             "hashes": [
-                "sha256:ec55bf7fe21fff7f1ad2f7da62363d749e2a470500eab1b555334b67aa1ef8cf",
-                "sha256:ec8b276a6b60bd80defed25add7e439881c19e64850afd9b346283d4165fd0fd"
+                "sha256:4132f6d49cb4dae6819e5379898f2b8cce3c5f23994194c24b77d5da2e36f774",
+                "sha256:a0aae034c444db0071aa077972ba4768d40c830d9539fd45bf4cd3f8f6992efc"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==3.0.1"
+            "markers": "python_version >= '3.8'",
+            "version": "==3.1.0"
         },
         "pygments": {
             "hashes": [
                 "sha256:8ace4d3c1dd481894b2005f560ead0f9f19ee64fe983366be1a21e171d12775c",
                 "sha256:db2db3deb4b4179f399a09054b023b6a586b76499d36965813c71aa8ed7b5fd1"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.15.1"
         },
         "pymdown-extensions": {
             "hashes": [
-                "sha256:ae66d84013c5d027ce055693e09a4628b67e9dec5bce05727e45b0918e36f274",
-                "sha256:b44e1093a43b8a975eae17b03c3a77aad4681b3b56fce60ce746dbef1944c8cb"
+                "sha256:508009b211373058debb8247e168de4cbcb91b1bff7b5e961b2c3e864e00b195",
+                "sha256:ef25dbbae530e8f67575d222b75ff0649b1e841e22c2ae9a20bad9472c2207dc"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==10.0.1"
+            "version": "==10.1"
         },
         "pytest": {
             "hashes": [
                 "sha256:78bf16451a2eb8c7a2ea98e32dc119fd2aa758f1d5d66dbf0a59d69a3969df32",
                 "sha256:b4bf8c45bd59934ed84001ad51e11b4ee40d40a1229d2c79f9c592b0a3f6bd8a"
             ],
             "index": "pypi",
@@ -859,57 +883,57 @@
                 "sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==2.8.2"
         },
         "pyyaml": {
             "hashes": [
-                "sha256:01b45c0191e6d66c470b6cf1b9531a771a83c1c4208272ead47a3ae4f2f603bf",
-                "sha256:0283c35a6a9fbf047493e3a0ce8d79ef5030852c51e9d911a27badfde0605293",
-                "sha256:055d937d65826939cb044fc8c9b08889e8c743fdc6a32b33e2390f66013e449b",
-                "sha256:07751360502caac1c067a8132d150cf3d61339af5691fe9e87803040dbc5db57",
-                "sha256:0b4624f379dab24d3725ffde76559cff63d9ec94e1736b556dacdfebe5ab6d4b",
-                "sha256:0ce82d761c532fe4ec3f87fc45688bdd3a4c1dc5e0b4a19814b9009a29baefd4",
-                "sha256:1e4747bc279b4f613a09eb64bba2ba602d8a6664c6ce6396a4d0cd413a50ce07",
-                "sha256:213c60cd50106436cc818accf5baa1aba61c0189ff610f64f4a3e8c6726218ba",
-                "sha256:231710d57adfd809ef5d34183b8ed1eeae3f76459c18fb4a0b373ad56bedcdd9",
-                "sha256:277a0ef2981ca40581a47093e9e2d13b3f1fbbeffae064c1d21bfceba2030287",
-                "sha256:2cd5df3de48857ed0544b34e2d40e9fac445930039f3cfe4bcc592a1f836d513",
-                "sha256:40527857252b61eacd1d9af500c3337ba8deb8fc298940291486c465c8b46ec0",
-                "sha256:432557aa2c09802be39460360ddffd48156e30721f5e8d917f01d31694216782",
-                "sha256:473f9edb243cb1935ab5a084eb238d842fb8f404ed2193a915d1784b5a6b5fc0",
-                "sha256:48c346915c114f5fdb3ead70312bd042a953a8ce5c7106d5bfb1a5254e47da92",
-                "sha256:50602afada6d6cbfad699b0c7bb50d5ccffa7e46a3d738092afddc1f9758427f",
-                "sha256:68fb519c14306fec9720a2a5b45bc9f0c8d1b9c72adf45c37baedfcd949c35a2",
-                "sha256:77f396e6ef4c73fdc33a9157446466f1cff553d979bd00ecb64385760c6babdc",
-                "sha256:81957921f441d50af23654aa6c5e5eaf9b06aba7f0a19c18a538dc7ef291c5a1",
-                "sha256:819b3830a1543db06c4d4b865e70ded25be52a2e0631ccd2f6a47a2822f2fd7c",
-                "sha256:897b80890765f037df3403d22bab41627ca8811ae55e9a722fd0392850ec4d86",
-                "sha256:98c4d36e99714e55cfbaaee6dd5badbc9a1ec339ebfc3b1f52e293aee6bb71a4",
-                "sha256:9df7ed3b3d2e0ecfe09e14741b857df43adb5a3ddadc919a2d94fbdf78fea53c",
-                "sha256:9fa600030013c4de8165339db93d182b9431076eb98eb40ee068700c9c813e34",
-                "sha256:a80a78046a72361de73f8f395f1f1e49f956c6be882eed58505a15f3e430962b",
-                "sha256:afa17f5bc4d1b10afd4466fd3a44dc0e245382deca5b3c353d8b757f9e3ecb8d",
-                "sha256:b3d267842bf12586ba6c734f89d1f5b871df0273157918b0ccefa29deb05c21c",
-                "sha256:b5b9eccad747aabaaffbc6064800670f0c297e52c12754eb1d976c57e4f74dcb",
-                "sha256:bfaef573a63ba8923503d27530362590ff4f576c626d86a9fed95822a8255fd7",
-                "sha256:c5687b8d43cf58545ade1fe3e055f70eac7a5a1a0bf42824308d868289a95737",
-                "sha256:cba8c411ef271aa037d7357a2bc8f9ee8b58b9965831d9e51baf703280dc73d3",
-                "sha256:d15a181d1ecd0d4270dc32edb46f7cb7733c7c508857278d3d378d14d606db2d",
-                "sha256:d4b0ba9512519522b118090257be113b9468d804b19d63c71dbcf4a48fa32358",
-                "sha256:d4db7c7aef085872ef65a8fd7d6d09a14ae91f691dec3e87ee5ee0539d516f53",
-                "sha256:d4eccecf9adf6fbcc6861a38015c2a64f38b9d94838ac1810a9023a0609e1b78",
-                "sha256:d67d839ede4ed1b28a4e8909735fc992a923cdb84e618544973d7dfc71540803",
-                "sha256:daf496c58a8c52083df09b80c860005194014c3698698d1a57cbcfa182142a3a",
-                "sha256:dbad0e9d368bb989f4515da330b88a057617d16b6a8245084f1b05400f24609f",
-                "sha256:e61ceaab6f49fb8bdfaa0f92c4b57bcfbea54c09277b1b4f7ac376bfb7a7c174",
-                "sha256:f84fbc98b019fef2ee9a1cb3ce93e3187a6df0b2538a651bfb890254ba9f90b5"
+                "sha256:062582fca9fabdd2c8b54a3ef1c978d786e0f6b3a1510e0ac93ef59e0ddae2bc",
+                "sha256:1635fd110e8d85d55237ab316b5b011de701ea0f29d07611174a1b42f1444741",
+                "sha256:184c5108a2aca3c5b3d3bf9395d50893a7ab82a38004c8f61c258d4428e80206",
+                "sha256:18aeb1bf9a78867dc38b259769503436b7c72f7a1f1f4c93ff9a17de54319b27",
+                "sha256:1d4c7e777c441b20e32f52bd377e0c409713e8bb1386e1099c2415f26e479595",
+                "sha256:1e2722cc9fbb45d9b87631ac70924c11d3a401b2d7f410cc0e3bbf249f2dca62",
+                "sha256:1fe35611261b29bd1de0070f0b2f47cb6ff71fa6595c077e42bd0c419fa27b98",
+                "sha256:28c119d996beec18c05208a8bd78cbe4007878c6dd15091efb73a30e90539696",
+                "sha256:42f8152b8dbc4fe7d96729ec2b99c7097d656dc1213a3229ca5383f973a5ed6d",
+                "sha256:4fb147e7a67ef577a588a0e2c17b6db51dda102c71de36f8549b6816a96e1867",
+                "sha256:50550eb667afee136e9a77d6dc71ae76a44df8b3e51e41b77f6de2932bfe0f47",
+                "sha256:510c9deebc5c0225e8c96813043e62b680ba2f9c50a08d3724c7f28a747d1486",
+                "sha256:5773183b6446b2c99bb77e77595dd486303b4faab2b086e7b17bc6bef28865f6",
+                "sha256:596106435fa6ad000c2991a98fa58eeb8656ef2325d7e158344fb33864ed87e3",
+                "sha256:6965a7bc3cf88e5a1c3bd2e0b5c22f8d677dc88a455344035f03399034eb3007",
+                "sha256:69b023b2b4daa7548bcfbd4aa3da05b3a74b772db9e23b982788168117739938",
+                "sha256:704219a11b772aea0d8ecd7058d0082713c3562b4e271b849ad7dc4a5c90c13c",
+                "sha256:7e07cbde391ba96ab58e532ff4803f79c4129397514e1413a7dc761ccd755735",
+                "sha256:81e0b275a9ecc9c0c0c07b4b90ba548307583c125f54d5b6946cfee6360c733d",
+                "sha256:9046c58c4395dff28dd494285c82ba00b546adfc7ef001486fbf0324bc174fba",
+                "sha256:9eb6caa9a297fc2c2fb8862bc5370d0303ddba53ba97e71f08023b6cd73d16a8",
+                "sha256:a0cd17c15d3bb3fa06978b4e8958dcdc6e0174ccea823003a106c7d4d7899ac5",
+                "sha256:afd7e57eddb1a54f0f1a974bc4391af8bcce0b444685d936840f125cf046d5bd",
+                "sha256:b1275ad35a5d18c62a7220633c913e1b42d44b46ee12554e5fd39c70a243d6a3",
+                "sha256:b786eecbdf8499b9ca1d697215862083bd6d2a99965554781d0d8d1ad31e13a0",
+                "sha256:ba336e390cd8e4d1739f42dfe9bb83a3cc2e80f567d8805e11b46f4a943f5515",
+                "sha256:baa90d3f661d43131ca170712d903e6295d1f7a0f595074f151c0aed377c9b9c",
+                "sha256:bc1bf2925a1ecd43da378f4db9e4f799775d6367bdb94671027b73b393a7c42c",
+                "sha256:bd4af7373a854424dabd882decdc5579653d7868b8fb26dc7d0e99f823aa5924",
+                "sha256:bf07ee2fef7014951eeb99f56f39c9bb4af143d8aa3c21b1677805985307da34",
+                "sha256:bfdf460b1736c775f2ba9f6a92bca30bc2095067b8a9d77876d1fad6cc3b4a43",
+                "sha256:c8098ddcc2a85b61647b2590f825f3db38891662cfc2fc776415143f599bb859",
+                "sha256:d2b04aac4d386b172d5b9692e2d2da8de7bfb6c387fa4f801fbf6fb2e6ba4673",
+                "sha256:d858aa552c999bc8a8d57426ed01e40bef403cd8ccdd0fc5f6f04a00414cac2a",
+                "sha256:f003ed9ad21d6a4713f0a9b5a7a0a79e08dd0f221aff4525a2be4c346ee60aab",
+                "sha256:f22ac1c3cac4dbc50079e965eba2c1058622631e526bd9afd45fedd49ba781fa",
+                "sha256:faca3bdcf85b2fc05d06ff3fbc1f83e1391b3e724afa3feba7d13eeab355484c",
+                "sha256:fca0e3a251908a499833aa292323f32437106001d436eca0e6e7833256674585",
+                "sha256:fd1592b3fdf65fff2ad0004b5e363300ef59ced41c2e6b3a99d4089fa8c5435d",
+                "sha256:fd66fc5d0da6d9815ba2cebeb4205f95818ff4b79c3ebe268e75d961704af52f"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==6.0"
+            "version": "==6.0.1"
         },
         "pyyaml-env-tag": {
             "hashes": [
                 "sha256:70092675bda14fdec33b31ba77e7543de9ddc88f2e5b99160396572d11525bdb",
                 "sha256:af31106dec8a4d68c60207c1886031cbf839b68aa7abccdb19868200532c2069"
             ],
             "markers": "python_version >= '3.6'",
@@ -1039,27 +1063,27 @@
                 "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"
             ],
             "markers": "python_version < '3.11'",
             "version": "==2.0.1"
         },
         "urllib3": {
             "hashes": [
-                "sha256:48e7fafa40319d358848e1bc6809b208340fafe2096f1725d05d67443d0483d1",
-                "sha256:bee28b5e56addb8226c96f7f13ac28cb4c301dd5ea8a6ca179c0b9835e032825"
+                "sha256:8d22f86aae8ef5e410d4f539fde9ce6b2113a001bb4d189e0aed70642d602b11",
+                "sha256:de7df1803967d2c2a98e4b11bb7d6bd9210474c46e8a0401514e3a42a75ebde4"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.0.3"
+            "version": "==2.0.4"
         },
         "virtualenv": {
             "hashes": [
-                "sha256:34da10f14fea9be20e0fd7f04aba9732f84e593dac291b757ce42e3368a39419",
-                "sha256:8ff19a38c1021c742148edc4f81cb43d7f8c6816d2ede2ab72af5b84c749ade1"
+                "sha256:43a3052be36080548bdee0b42919c88072037d50d56c28bd3f853cbe92b953ff",
+                "sha256:fd8a78f46f6b99a67b7ec5cf73f92357891a7b3a40fd97637c27f854aae3b9e0"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==20.23.1"
+            "version": "==20.24.2"
         },
         "watchdog": {
             "hashes": [
                 "sha256:0e06ab8858a76e1219e68c7573dfeba9dd1c0219476c5a44d5333b01d7e1743a",
                 "sha256:13bbbb462ee42ec3c5723e1205be8ced776f05b100e4737518c67c8325cf6100",
                 "sha256:233b5817932685d39a7896b1090353fc8efc1ef99c9c054e46c8002561252fb8",
                 "sha256:25f70b4aa53bd743729c7475d7ec41093a580528b100e9a8c5b5efe8899592fc",
@@ -1096,15 +1120,15 @@
                 "sha256:b1f042a899ea4c458b7321da1b5e3331e3e0ec781583434de1301946ceadb943"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==8.4.1"
         },
         "zipp": {
             "hashes": [
-                "sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b",
-                "sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556"
+                "sha256:679e51dd4403591b2d6838a48de3d283f3d188412a9782faadf845f298736ba0",
+                "sha256:ebc15946aa78bd63458992fc81ec3b6f7b1e92d51c35e6de1c3804e73b799147"
             ],
             "markers": "python_version < '3.10'",
-            "version": "==3.15.0"
+            "version": "==3.16.2"
         }
     }
 }
```

### Comparing `mkdocs_puml-1.2.2/README.md` & `mkdocs_puml-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_puml-1.2.2/mkdocs_puml/encoder.py` & `mkdocs_puml-1.2.3/mkdocs_puml/encoder.py`

 * *Files identical despite different names*

### Comparing `mkdocs_puml-1.2.2/mkdocs_puml/plugin.py` & `mkdocs_puml-1.2.3/mkdocs_puml/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import typing
 import re
 import uuid
 
 from mkdocs.config.config_options import Type, Config
-from mkdocs.plugins import BasePlugin, Page
+from mkdocs.plugins import BasePlugin
 
 from mkdocs_puml.puml import PlantUML
 
 
 class PlantUMLPlugin(BasePlugin):
     """MKDocs plugin that converts puml diagrams into SVG images.
 
@@ -107,15 +107,15 @@
         """
         resp = self.puml.translate(self.diagrams.values())
 
         for key, svg in zip(self.diagrams.keys(), resp):
             self.diagrams[key] = svg
         return env
 
-    def on_post_page(self, output: str, page: Page, *args, **kwargs) -> str:
+    def on_post_page(self, output: str, page, *args, **kwargs) -> str:
         """The event is fired after HTML page is rendered.
         Here, we substitute <pre> tags with uuid codes of diagrams
         with the corresponding SVG images.
 
         Args:
             output: rendered HTML in str format
             page: Page object
@@ -125,14 +125,15 @@
         """
         schemes = self.uuid_regex.findall(output)
         for v in schemes:
             output = self._replace(v, output)
             page.content = self._replace(v, page.content)
 
             # MkDocs >=1.4 doesn't have html attribute.
+            # This is required for integration with mkdocs-print-page plugin.
             # TODO: Remove the support of older versions in future releases
             if hasattr(page, 'html'):
                 page.html = self._replace(v, page.html)
 
         return output
 
     def _replace(self, key: str, content: str) -> str:
```

### Comparing `mkdocs_puml-1.2.2/mkdocs_puml/puml.py` & `mkdocs_puml-1.2.3/mkdocs_puml/puml.py`

 * *Files identical despite different names*

### Comparing `mkdocs_puml-1.2.2/pyproject.toml` & `mkdocs_puml-1.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mkdocs_puml-1.2.2/tests/conftest.py` & `mkdocs_puml-1.2.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mkdocs_puml-1.2.2/tests/plugins/conftest.py` & `mkdocs_puml-1.2.3/tests/plugins/conftest.py`

 * *Files identical despite different names*

### Comparing `mkdocs_puml-1.2.2/tests/plugins/test_plugin.py` & `mkdocs_puml-1.2.3/tests/plugins/test_plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs_puml-1.2.2/tests/test_puml.py` & `mkdocs_puml-1.2.3/tests/test_puml.py`

 * *Files identical despite different names*

### Comparing `mkdocs_puml-1.2.2/tests/testdata/markdown.md` & `mkdocs_puml-1.2.3/tests/testdata/markdown.md`

 * *Files identical despite different names*

### Comparing `mkdocs_puml-1.2.2/tests/testdata/plantuml.svg` & `mkdocs_puml-1.2.3/tests/testdata/plantuml.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_puml-1.2.2/PKG-INFO` & `mkdocs_puml-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs_puml
-Version: 1.2.2
+Version: 1.2.3
 Summary: Package that brings PlantUML to MkDocs
 Author-email: Mikhail Kravets <michkravets@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: requests >= 2.27, < 3.0
 Requires-Dist: markdown >= 3.2.1, < 4.0
```

