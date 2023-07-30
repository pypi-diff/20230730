# Comparing `tmp/ghcr_badge-0.3.1.tar.gz` & `tmp/ghcr_badge-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghcr_badge-0.3.1.tar", max compression
+gzip compressed data, was "ghcr_badge-0.3.2.tar", max compression
```

## Comparing `ghcr_badge-0.3.1.tar` & `ghcr_badge-0.3.2.tar`

### file list

```diff
@@ -1,13 +1,15 @@
--rw-r--r--   0        0        0     1049 2023-07-30 17:40:00.717092 ghcr_badge-0.3.1/LICENSE.txt
--rw-r--r--   0        0        0     3802 2023-07-30 17:40:00.717092 ghcr_badge-0.3.1/README.md
--rw-r--r--   0        0        0      125 2023-07-30 17:40:00.721093 ghcr_badge-0.3.1/ghcr_badge/__init__.py
--rw-r--r--   0        0        0     1282 2023-07-30 17:40:00.721093 ghcr_badge-0.3.1/ghcr_badge/dicts.py
--rw-r--r--   0        0        0    13055 2023-07-30 17:40:00.721093 ghcr_badge-0.3.1/ghcr_badge/generate.py
--rw-r--r--   0        0        0     2859 2023-07-30 17:40:00.721093 ghcr_badge-0.3.1/ghcr_badge/main.py
--rw-r--r--   0        0        0        0 2023-07-30 17:40:00.721093 ghcr_badge-0.3.1/ghcr_badge/py.typed
--rw-r--r--   0        0        0     7454 2023-07-30 17:40:00.721093 ghcr_badge-0.3.1/ghcr_badge/server.py
--rw-r--r--   0        0        0      721 2023-07-30 17:40:00.721093 ghcr_badge-0.3.1/ghcr_badge/svg/mark-github.svg
--rw-r--r--   0        0        0      540 2023-07-30 17:40:00.721093 ghcr_badge-0.3.1/ghcr_badge/svg/package-16.svg
--rw-r--r--   0        0        0     5966 2023-07-30 17:40:00.721093 ghcr_badge-0.3.1/ghcr_badge/templates/index.j2
--rw-r--r--   0        0        0     1798 2023-07-30 17:40:00.721093 ghcr_badge-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     5033 1970-01-01 00:00:00.000000 ghcr_badge-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1049 2023-07-30 18:13:59.886952 ghcr_badge-0.3.2/LICENSE.txt
+-rw-r--r--   0        0        0     3802 2023-07-30 18:13:59.886952 ghcr_badge-0.3.2/README.md
+-rw-r--r--   0        0        0      125 2023-07-30 18:13:59.886952 ghcr_badge-0.3.2/ghcr_badge/__init__.py
+-rw-r--r--   0        0        0     1282 2023-07-30 18:13:59.886952 ghcr_badge-0.3.2/ghcr_badge/dicts.py
+-rw-r--r--   0        0        0    13055 2023-07-30 18:13:59.886952 ghcr_badge-0.3.2/ghcr_badge/generate.py
+-rw-r--r--   0        0        0     2859 2023-07-30 18:13:59.886952 ghcr_badge-0.3.2/ghcr_badge/main.py
+-rw-r--r--   0        0        0        0 2023-07-30 18:13:59.886952 ghcr_badge-0.3.2/ghcr_badge/py.typed
+-rw-r--r--   0        0        0     7454 2023-07-30 18:13:59.886952 ghcr_badge-0.3.2/ghcr_badge/server.py
+-rw-r--r--   0        0        0    32038 2023-07-30 18:13:59.886952 ghcr_badge-0.3.2/ghcr_badge/static/favicon.ico
+-rw-r--r--   0        0        0    28398 2023-07-30 18:13:59.886952 ghcr_badge-0.3.2/ghcr_badge/static/favicon.png
+-rw-r--r--   0        0        0      721 2023-07-30 18:13:59.886952 ghcr_badge-0.3.2/ghcr_badge/svg/mark-github.svg
+-rw-r--r--   0        0        0      540 2023-07-30 18:13:59.886952 ghcr_badge-0.3.2/ghcr_badge/svg/package-16.svg
+-rw-r--r--   0        0        0     7236 2023-07-30 18:13:59.886952 ghcr_badge-0.3.2/ghcr_badge/templates/index.j2
+-rw-r--r--   0        0        0     1798 2023-07-30 18:13:59.890952 ghcr_badge-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     5033 1970-01-01 00:00:00.000000 ghcr_badge-0.3.2/PKG-INFO
```

### Comparing `ghcr_badge-0.3.1/LICENSE.txt` & `ghcr_badge-0.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ghcr_badge-0.3.1/README.md` & `ghcr_badge-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `ghcr_badge-0.3.1/ghcr_badge/dicts.py` & `ghcr_badge-0.3.2/ghcr_badge/dicts.py`

 * *Files identical despite different names*

### Comparing `ghcr_badge-0.3.1/ghcr_badge/generate.py` & `ghcr_badge-0.3.2/ghcr_badge/generate.py`

 * *Files identical despite different names*

### Comparing `ghcr_badge-0.3.1/ghcr_badge/main.py` & `ghcr_badge-0.3.2/ghcr_badge/main.py`

 * *Files identical despite different names*

### Comparing `ghcr_badge-0.3.1/ghcr_badge/server.py` & `ghcr_badge-0.3.2/ghcr_badge/server.py`

 * *Files identical despite different names*

### Comparing `ghcr_badge-0.3.1/ghcr_badge/svg/mark-github.svg` & `ghcr_badge-0.3.2/ghcr_badge/svg/mark-github.svg`

 * *Files identical despite different names*

### Comparing `ghcr_badge-0.3.1/ghcr_badge/svg/package-16.svg` & `ghcr_badge-0.3.2/ghcr_badge/svg/package-16.svg`

 * *Files identical despite different names*

### Comparing `ghcr_badge-0.3.1/ghcr_badge/templates/index.j2` & `ghcr_badge-0.3.2/ghcr_badge/templates/index.j2`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,36 @@
 <!DOCTYPE html>
-<html lang="en">
+<html lang="en" dir="ltr">
   <head>
     <title>ghcr-badge</title>
     <meta charset="UTF-8">
-    <script type="application/javascript">
+    <meta name="viewport" content="width=device-width,initial-scale=1">
+    <meta name="description"
+          content="Generate ghcr.io (GitHub Container Registory) container's status badge">
+    <meta name="format-detection" content="telephone=no">
+    <link rel="icon" href="/static/favicon.ico">
+    <link rel="apple-touch-icon" href="/static/favicon.png">
+    <meta property="og:site_name" content="ghcr-badge">
+    <meta property="og:url" content="https://ghcr-badge.egpl.dev">
+    <meta property="og:type" content="website">
+    <meta property="og:title" content="ghcr-badge">
+    <meta property="og:description"
+          content="Generate ghcr.io (GitHub Container Registory) container's status badge">
+    <meta property="og:image"
+          content="https://ghcr-badge.egpl.dev/static/favicon.png">
+    <meta property="og:image:width" content="160">
+    <meta property="og:image:height" content="160">
+    <meta property="og:locale" content="en_US">
+    <meta name="twitter:card" content="summary">
+    <meta name="twitter:site" content="@egpl0">
+    <meta name="twitter:description"
+          content="Generate ghcr.io (GitHub Container Registory) container's status badge">
+    <meta name="twitter:image:src"
+          content="https://ghcr-badge.egpl.dev/static/favicon.png">
+    <script>
       const updateImages = (targetId) => {
         const owner = encodeURIComponent(document.getElementById("owner").value);
         const name = encodeURIComponent(document.getElementById("name").value);
         if (!(owner || name)) return;
 
         const imgElms = document.querySelectorAll("main > img");
         Array.from(imgElms).filter((e) =>
```

#### html2text {}

```diff
@@ -1,7 +1,25 @@
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
 ****** ghcr-badge ******
 
 ===============================================================================
 ghcr.io/ [eggplants           ] / [ghcr-badge          ] Generate!
 ===============================================================================
 ***** tags *****
 [tags-badge]
```

### Comparing `ghcr_badge-0.3.1/pyproject.toml` & `ghcr_badge-0.3.2/pyproject.toml`

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
-version = "0.3.1"
+version = "0.3.2"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 anybadge="^1.9.0"
 flask="^2.1.2"
 gunicorn=">=20.1,<22.0"
 humanfriendly="^10.0"
```

### Comparing `ghcr_badge-0.3.1/PKG-INFO` & `ghcr_badge-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghcr-badge
-Version: 0.3.1
+Version: 0.3.2
 Summary: Generate ghcr.io container's status badge
 Home-page: https://github.com/eggplants/ghcr-badge
 License: MIT
 Keywords: github-container-registry,badge,ghcr
 Author: eggplants
 Author-email: w10776e8w@yahoo.co.jp
 Requires-Python: >=3.8,<3.12
```

