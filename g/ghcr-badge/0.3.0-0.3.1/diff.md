# Comparing `tmp/ghcr_badge-0.3.0.tar.gz` & `tmp/ghcr_badge-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghcr_badge-0.3.0.tar", max compression
+gzip compressed data, was "ghcr_badge-0.3.1.tar", max compression
```

## Comparing `ghcr_badge-0.3.0.tar` & `ghcr_badge-0.3.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1049 2023-07-30 16:35:59.907051 ghcr_badge-0.3.0/LICENSE.txt
--rw-r--r--   0        0        0     3802 2023-07-30 16:35:59.907051 ghcr_badge-0.3.0/README.md
--rw-r--r--   0        0        0      125 2023-07-30 16:35:59.907051 ghcr_badge-0.3.0/ghcr_badge/__init__.py
--rw-r--r--   0        0        0     1282 2023-07-30 16:35:59.907051 ghcr_badge-0.3.0/ghcr_badge/dicts.py
--rw-r--r--   0        0        0    13055 2023-07-30 16:35:59.907051 ghcr_badge-0.3.0/ghcr_badge/generate.py
--rw-r--r--   0        0        0     2859 2023-07-30 16:35:59.907051 ghcr_badge-0.3.0/ghcr_badge/main.py
--rw-r--r--   0        0        0        0 2023-07-30 16:35:59.911051 ghcr_badge-0.3.0/ghcr_badge/py.typed
--rw-r--r--   0        0        0     7454 2023-07-30 16:35:59.911051 ghcr_badge-0.3.0/ghcr_badge/server.py
--rw-r--r--   0        0        0      721 2023-07-30 16:35:59.911051 ghcr_badge-0.3.0/ghcr_badge/svg/mark-github.svg
--rw-r--r--   0        0        0      540 2023-07-30 16:35:59.911051 ghcr_badge-0.3.0/ghcr_badge/svg/package-16.svg
--rw-r--r--   0        0        0     6014 2023-07-30 16:35:59.911051 ghcr_badge-0.3.0/ghcr_badge/templates/index.j2
--rw-r--r--   0        0        0     1798 2023-07-30 16:35:59.911051 ghcr_badge-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     5033 1970-01-01 00:00:00.000000 ghcr_badge-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1049 2023-07-30 17:40:00.717092 ghcr_badge-0.3.1/LICENSE.txt
+-rw-r--r--   0        0        0     3802 2023-07-30 17:40:00.717092 ghcr_badge-0.3.1/README.md
+-rw-r--r--   0        0        0      125 2023-07-30 17:40:00.721093 ghcr_badge-0.3.1/ghcr_badge/__init__.py
+-rw-r--r--   0        0        0     1282 2023-07-30 17:40:00.721093 ghcr_badge-0.3.1/ghcr_badge/dicts.py
+-rw-r--r--   0        0        0    13055 2023-07-30 17:40:00.721093 ghcr_badge-0.3.1/ghcr_badge/generate.py
+-rw-r--r--   0        0        0     2859 2023-07-30 17:40:00.721093 ghcr_badge-0.3.1/ghcr_badge/main.py
+-rw-r--r--   0        0        0        0 2023-07-30 17:40:00.721093 ghcr_badge-0.3.1/ghcr_badge/py.typed
+-rw-r--r--   0        0        0     7454 2023-07-30 17:40:00.721093 ghcr_badge-0.3.1/ghcr_badge/server.py
+-rw-r--r--   0        0        0      721 2023-07-30 17:40:00.721093 ghcr_badge-0.3.1/ghcr_badge/svg/mark-github.svg
+-rw-r--r--   0        0        0      540 2023-07-30 17:40:00.721093 ghcr_badge-0.3.1/ghcr_badge/svg/package-16.svg
+-rw-r--r--   0        0        0     5966 2023-07-30 17:40:00.721093 ghcr_badge-0.3.1/ghcr_badge/templates/index.j2
+-rw-r--r--   0        0        0     1798 2023-07-30 17:40:00.721093 ghcr_badge-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     5033 1970-01-01 00:00:00.000000 ghcr_badge-0.3.1/PKG-INFO
```

### Comparing `ghcr_badge-0.3.0/LICENSE.txt` & `ghcr_badge-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ghcr_badge-0.3.0/README.md` & `ghcr_badge-0.3.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -37,27 +37,27 @@
 
 - <https://ghcr-badge.deta.dev/>
   - [![Website](https://img.shields.io/website?label=deta.dev&url=https%3A%2F%2Fghcr-badge.deta.dev)](https://ghcr-badge.deta.dev)
 
 ## Available paths
 
 - `/<package_owner>/<package_name>/tags?color=...&ignore=...&n=...&label=...&trim=...`
-  - defaults: `color=#e05d44`, `ignore=latest`, `n=3`, `label=image tags`
+  - defaults: `color=#44cc11`, `ignore=latest`, `n=3`, `label=image tags`
   - <https://ghcr-badge.egpl.dev/eggplants/ghcr-badge/tags?trim=major>
   - 👉: ![1]
 - `/<package_owner>/<package_name>/latest_tag?color=...&ignore=...&label=...&trim=...`
-  - defaults: `color=#e05d44`, `ignore=latest`, `label=version`
+  - defaults: `color=#44cc11`, `ignore=latest`, `label=version`
   - <https://ghcr-badge.egpl.dev/eggplants/ghcr-badge/latest_tag?trim=major&label=latest>
   - 👉: ![2]
 - `/<package_owner>/<package_name>/develop_tag?color=...&label=...`
-  - defaults: `color=#e05d44`, `label=develop`
+  - defaults: `color=#44cc11`, `label=develop`
   - <https://ghcr-badge.egpl.dev/ptr727/plexcleaner/develop_tag>
   - 👉: ![3]
 - `/<package_owner>/<package_name>/size?color=...&tag=...&label=...&trim=...`
-  - defaults: `color=#e05d44`, `tag=latest`, `label=image size`
+  - defaults: `color=#44cc11`, `tag=latest`, `label=image size`
   - <https://ghcr-badge.egpl.dev/eggplants/ghcr-badge/size>
   - 👉: ![4]
 
 ## Common parameters
 
 ### `label` parameter
```

### Comparing `ghcr_badge-0.3.0/ghcr_badge/dicts.py` & `ghcr_badge-0.3.1/ghcr_badge/dicts.py`

 * *Files identical despite different names*

### Comparing `ghcr_badge-0.3.0/ghcr_badge/generate.py` & `ghcr_badge-0.3.1/ghcr_badge/generate.py`

 * *Files identical despite different names*

### Comparing `ghcr_badge-0.3.0/ghcr_badge/main.py` & `ghcr_badge-0.3.1/ghcr_badge/main.py`

 * *Files identical despite different names*

### Comparing `ghcr_badge-0.3.0/ghcr_badge/server.py` & `ghcr_badge-0.3.1/ghcr_badge/server.py`

 * *Files identical despite different names*

### Comparing `ghcr_badge-0.3.0/ghcr_badge/svg/mark-github.svg` & `ghcr_badge-0.3.1/ghcr_badge/svg/mark-github.svg`

 * *Files identical despite different names*

### Comparing `ghcr_badge-0.3.0/ghcr_badge/svg/package-16.svg` & `ghcr_badge-0.3.1/ghcr_badge/svg/package-16.svg`

 * *Files identical despite different names*

### Comparing `ghcr_badge-0.3.0/ghcr_badge/templates/index.j2` & `ghcr_badge-0.3.1/ghcr_badge/templates/index.j2`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,14 @@
         const name = encodeURIComponent(document.getElementById("name").value);
         if (!(owner || name)) return;
 
         const imgElms = document.querySelectorAll("main > img");
         Array.from(imgElms).filter((e) =>
           targetId === undefined || targetId === e.id
         ).forEach((e) => {
-          console.log(`${targetId} -- ${e.id}`)
           const url = new URL(`${window.location.origin}/${owner}/${name}/${e.id}`);
 
           const optionElms = document.querySelectorAll(`div[id="${e.id}-options"] > input`);
           Array.from(optionElms).forEach((o) => {
             url.searchParams.set(o.className, o.value);
           });
           e.src = url.toString();
```

### Comparing `ghcr_badge-0.3.0/pyproject.toml` & `ghcr_badge-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 description = "Generate ghcr.io container's status badge"
 keywords = ["github-container-registry", "badge", "ghcr"]
 name = "ghcr_badge"
 packages = [{include = "ghcr_badge"}]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/eggplants/ghcr-badge"
-version = "0.3.0"
+version = "0.3.1"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 anybadge="^1.9.0"
 flask="^2.1.2"
 gunicorn=">=20.1,<22.0"
 humanfriendly="^10.0"
```

### Comparing `ghcr_badge-0.3.0/PKG-INFO` & `ghcr_badge-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghcr-badge
-Version: 0.3.0
+Version: 0.3.1
 Summary: Generate ghcr.io container's status badge
 Home-page: https://github.com/eggplants/ghcr-badge
 License: MIT
 Keywords: github-container-registry,badge,ghcr
 Author: eggplants
 Author-email: w10776e8w@yahoo.co.jp
 Requires-Python: >=3.8,<3.12
@@ -67,27 +67,27 @@
 
 - <https://ghcr-badge.deta.dev/>
   - [![Website](https://img.shields.io/website?label=deta.dev&url=https%3A%2F%2Fghcr-badge.deta.dev)](https://ghcr-badge.deta.dev)
 
 ## Available paths
 
 - `/<package_owner>/<package_name>/tags?color=...&ignore=...&n=...&label=...&trim=...`
-  - defaults: `color=#e05d44`, `ignore=latest`, `n=3`, `label=image tags`
+  - defaults: `color=#44cc11`, `ignore=latest`, `n=3`, `label=image tags`
   - <https://ghcr-badge.egpl.dev/eggplants/ghcr-badge/tags?trim=major>
   - 👉: ![1]
 - `/<package_owner>/<package_name>/latest_tag?color=...&ignore=...&label=...&trim=...`
-  - defaults: `color=#e05d44`, `ignore=latest`, `label=version`
+  - defaults: `color=#44cc11`, `ignore=latest`, `label=version`
   - <https://ghcr-badge.egpl.dev/eggplants/ghcr-badge/latest_tag?trim=major&label=latest>
   - 👉: ![2]
 - `/<package_owner>/<package_name>/develop_tag?color=...&label=...`
-  - defaults: `color=#e05d44`, `label=develop`
+  - defaults: `color=#44cc11`, `label=develop`
   - <https://ghcr-badge.egpl.dev/ptr727/plexcleaner/develop_tag>
   - 👉: ![3]
 - `/<package_owner>/<package_name>/size?color=...&tag=...&label=...&trim=...`
-  - defaults: `color=#e05d44`, `tag=latest`, `label=image size`
+  - defaults: `color=#44cc11`, `tag=latest`, `label=image size`
   - <https://ghcr-badge.egpl.dev/eggplants/ghcr-badge/size>
   - 👉: ![4]
 
 ## Common parameters
 
 ### `label` parameter
```

