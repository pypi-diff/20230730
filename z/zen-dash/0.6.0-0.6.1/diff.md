# Comparing `tmp/zen_dash-0.6.0.tar.gz` & `tmp/zen_dash-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zen_dash-0.6.0.tar", max compression
+gzip compressed data, was "zen_dash-0.6.1.tar", max compression
```

## Comparing `zen_dash-0.6.0.tar` & `zen_dash-0.6.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1070 2023-02-09 14:33:40.121808 zen_dash-0.6.0/LICENSE
--rw-r--r--   0        0        0     7781 2023-05-05 01:59:51.099742 zen_dash-0.6.0/README.md
--rw-r--r--   0        0        0     1288 2023-07-24 01:22:52.929274 zen_dash-0.6.0/pyproject.toml
--rw-r--r--   0        0        0       41 2023-04-12 05:50:21.332964 zen_dash-0.6.0/zen_dash/__init__.py
--rw-r--r--   0        0        0     1873 2023-07-22 22:55:25.435617 zen_dash-0.6.0/zen_dash/auth/__init__.py
--rw-r--r--   0        0        0        0 2023-01-07 16:56:11.285785 zen_dash-0.6.0/zen_dash/cli/__init__.py
--rw-r--r--   0        0        0      219 2023-04-14 03:33:36.095076 zen_dash-0.6.0/zen_dash/cli/main.py
--rw-r--r--   0        0        0     5879 2023-04-14 03:33:25.986936 zen_dash-0.6.0/zen_dash/cli/project_management.py
--rw-r--r--   0        0        0      203 2023-04-12 05:50:21.336964 zen_dash-0.6.0/zen_dash/flex_data.py
--rw-r--r--   0        0        0      196 2023-04-12 05:50:21.336964 zen_dash-0.6.0/zen_dash/instances.py
--rw-r--r--   0        0        0     1403 2023-07-22 15:37:24.864370 zen_dash-0.6.0/zen_dash/objects/__init__.py
--rw-r--r--   0        0        0      291 2023-04-12 05:50:21.336964 zen_dash-0.6.0/zen_dash/objects/flex_data.py
--rw-r--r--   0        0        0    13136 2023-07-24 00:51:23.343274 zen_dash-0.6.0/zen_dash/objects/instances.py
--rw-r--r--   0        0        0      255 2023-04-12 05:50:21.336964 zen_dash-0.6.0/zen_dash/objects/page.py
--rw-r--r--   0        0        0      768 2023-04-12 05:50:21.336964 zen_dash-0.6.0/zen_dash/objects/scripts.py
--rw-r--r--   0        0        0      750 2023-06-16 02:37:03.983233 zen_dash-0.6.0/zen_dash/objects/sidebar.py
--rw-r--r--   0        0        0      919 2023-04-12 05:50:21.336964 zen_dash-0.6.0/zen_dash/page.py
--rw-r--r--   0        0        0        0 2023-04-12 05:50:21.336964 zen_dash-0.6.0/zen_dash/route.py
--rw-r--r--   0        0        0      191 2023-04-12 05:50:21.336964 zen_dash-0.6.0/zen_dash/scripts.py
--rw-r--r--   0        0        0      195 2023-04-12 05:50:21.336964 zen_dash-0.6.0/zen_dash/sidebar.py
--rw-r--r--   0        0        0  1017714 2023-07-23 16:22:33.182273 zen_dash-0.6.0/zen_dash/static/275.44cd52f9d992445f.js
--rw-r--r--   0        0        0    57081 2023-07-24 00:55:40.695293 zen_dash-0.6.0/zen_dash/static/3rdpartylicenses.txt
--rw-r--r--   0        0        0   128180 2023-07-23 16:22:33.182273 zen_dash-0.6.0/zen_dash/static/MaterialIcons-Regular.196fa4a92dd6fa73.ttf
--rw-r--r--   0        0        0   143258 2023-07-23 16:22:33.182273 zen_dash-0.6.0/zen_dash/static/MaterialIcons-Regular.1e50f5c2ffa6aba4.eot
--rw-r--r--   0        0        0    44300 2023-07-23 16:22:33.182273 zen_dash-0.6.0/zen_dash/static/MaterialIcons-Regular.7ea2023eeca07427.woff2
--rw-r--r--   0        0        0    57620 2023-07-23 16:22:33.182273 zen_dash-0.6.0/zen_dash/static/MaterialIcons-Regular.db852539204b1a34.woff
--rw-r--r--   0        0        0      948 2023-07-23 16:22:33.182273 zen_dash-0.6.0/zen_dash/static/favicon.ico
--rw-r--r--   0        0        0     2137 2023-07-24 00:55:41.423305 zen_dash-0.6.0/zen_dash/static/index.html
--rw-r--r--   0        0        0    92621 2023-07-24 00:55:40.695293 zen_dash-0.6.0/zen_dash/static/main.b01efffb503d168d.js
--rw-r--r--   0        0        0    33759 2023-07-23 16:22:33.182273 zen_dash-0.6.0/zen_dash/static/polyfills.0a8881ff36766b1e.js
--rw-r--r--   0        0        0     3285 2023-07-23 16:22:33.182273 zen_dash-0.6.0/zen_dash/static/runtime.6a9b461ae5a72237.js
--rw-r--r--   0        0        0   152653 2023-07-23 16:22:33.182273 zen_dash-0.6.0/zen_dash/static/styles.362a8260c32d36d9.css
--rw-r--r--   0        0        0  3060723 2023-07-23 16:22:33.182273 zen_dash-0.6.0/zen_dash/static/vendor.3c67e76b6e4a9ca3.js
--rw-r--r--   0        0        0      621 2022-10-23 00:15:15.909625 zen_dash-0.6.0/zen_dash/support/__init__.py
--rw-r--r--   0        0        0      217 2023-04-12 05:50:21.352964 zen_dash-0.6.0/zen_dash/support/encoder.py
--rw-r--r--   0        0        0     7055 2023-05-29 16:12:36.409345 zen_dash-0.6.0/zen_dash/tag/__init__.py
--rw-r--r--   0        0        0     1513 2023-04-12 05:50:21.352964 zen_dash-0.6.0/zen_dash/websocket/__init__.py
--rw-r--r--   0        0        0     8861 1970-01-01 00:00:00.000000 zen_dash-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-02-09 14:33:40.121808 zen_dash-0.6.1/LICENSE
+-rw-r--r--   0        0        0     7781 2023-05-05 01:59:51.099742 zen_dash-0.6.1/README.md
+-rw-r--r--   0        0        0     1288 2023-07-30 20:53:03.392198 zen_dash-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0       41 2023-04-12 05:50:21.332964 zen_dash-0.6.1/zen_dash/__init__.py
+-rw-r--r--   0        0        0     1521 2023-07-30 20:54:39.317930 zen_dash-0.6.1/zen_dash/auth/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-07 16:56:11.285785 zen_dash-0.6.1/zen_dash/cli/__init__.py
+-rw-r--r--   0        0        0      219 2023-04-14 03:33:36.095076 zen_dash-0.6.1/zen_dash/cli/main.py
+-rw-r--r--   0        0        0     5879 2023-04-14 03:33:25.986936 zen_dash-0.6.1/zen_dash/cli/project_management.py
+-rw-r--r--   0        0        0      203 2023-04-12 05:50:21.336964 zen_dash-0.6.1/zen_dash/flex_data.py
+-rw-r--r--   0        0        0      196 2023-04-12 05:50:21.336964 zen_dash-0.6.1/zen_dash/instances.py
+-rw-r--r--   0        0        0     1403 2023-07-22 15:37:24.864370 zen_dash-0.6.1/zen_dash/objects/__init__.py
+-rw-r--r--   0        0        0      291 2023-04-12 05:50:21.336964 zen_dash-0.6.1/zen_dash/objects/flex_data.py
+-rw-r--r--   0        0        0    13136 2023-07-24 00:51:23.343274 zen_dash-0.6.1/zen_dash/objects/instances.py
+-rw-r--r--   0        0        0      255 2023-04-12 05:50:21.336964 zen_dash-0.6.1/zen_dash/objects/page.py
+-rw-r--r--   0        0        0      768 2023-04-12 05:50:21.336964 zen_dash-0.6.1/zen_dash/objects/scripts.py
+-rw-r--r--   0        0        0      750 2023-06-16 02:37:03.983233 zen_dash-0.6.1/zen_dash/objects/sidebar.py
+-rw-r--r--   0        0        0      919 2023-04-12 05:50:21.336964 zen_dash-0.6.1/zen_dash/page.py
+-rw-r--r--   0        0        0        0 2023-04-12 05:50:21.336964 zen_dash-0.6.1/zen_dash/route.py
+-rw-r--r--   0        0        0      191 2023-04-12 05:50:21.336964 zen_dash-0.6.1/zen_dash/scripts.py
+-rw-r--r--   0        0        0      195 2023-04-12 05:50:21.336964 zen_dash-0.6.1/zen_dash/sidebar.py
+-rw-r--r--   0        0        0  1017714 2023-07-23 16:22:33.182273 zen_dash-0.6.1/zen_dash/static/275.44cd52f9d992445f.js
+-rw-r--r--   0        0        0    57081 2023-07-24 00:55:40.695293 zen_dash-0.6.1/zen_dash/static/3rdpartylicenses.txt
+-rw-r--r--   0        0        0   128180 2023-07-23 16:22:33.182273 zen_dash-0.6.1/zen_dash/static/MaterialIcons-Regular.196fa4a92dd6fa73.ttf
+-rw-r--r--   0        0        0   143258 2023-07-23 16:22:33.182273 zen_dash-0.6.1/zen_dash/static/MaterialIcons-Regular.1e50f5c2ffa6aba4.eot
+-rw-r--r--   0        0        0    44300 2023-07-23 16:22:33.182273 zen_dash-0.6.1/zen_dash/static/MaterialIcons-Regular.7ea2023eeca07427.woff2
+-rw-r--r--   0        0        0    57620 2023-07-23 16:22:33.182273 zen_dash-0.6.1/zen_dash/static/MaterialIcons-Regular.db852539204b1a34.woff
+-rw-r--r--   0        0        0      948 2023-07-23 16:22:33.182273 zen_dash-0.6.1/zen_dash/static/favicon.ico
+-rw-r--r--   0        0        0     2137 2023-07-24 00:55:41.423305 zen_dash-0.6.1/zen_dash/static/index.html
+-rw-r--r--   0        0        0    92621 2023-07-24 00:55:40.695293 zen_dash-0.6.1/zen_dash/static/main.b01efffb503d168d.js
+-rw-r--r--   0        0        0    33759 2023-07-23 16:22:33.182273 zen_dash-0.6.1/zen_dash/static/polyfills.0a8881ff36766b1e.js
+-rw-r--r--   0        0        0     3285 2023-07-23 16:22:33.182273 zen_dash-0.6.1/zen_dash/static/runtime.6a9b461ae5a72237.js
+-rw-r--r--   0        0        0   152653 2023-07-23 16:22:33.182273 zen_dash-0.6.1/zen_dash/static/styles.362a8260c32d36d9.css
+-rw-r--r--   0        0        0  3060723 2023-07-23 16:22:33.182273 zen_dash-0.6.1/zen_dash/static/vendor.3c67e76b6e4a9ca3.js
+-rw-r--r--   0        0        0      621 2022-10-23 00:15:15.909625 zen_dash-0.6.1/zen_dash/support/__init__.py
+-rw-r--r--   0        0        0      217 2023-04-12 05:50:21.352964 zen_dash-0.6.1/zen_dash/support/encoder.py
+-rw-r--r--   0        0        0     7055 2023-05-29 16:12:36.409345 zen_dash-0.6.1/zen_dash/tag/__init__.py
+-rw-r--r--   0        0        0     1513 2023-04-12 05:50:21.352964 zen_dash-0.6.1/zen_dash/websocket/__init__.py
+-rw-r--r--   0        0        0     8861 1970-01-01 00:00:00.000000 zen_dash-0.6.1/PKG-INFO
```

### Comparing `zen_dash-0.6.0/LICENSE` & `zen_dash-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.0/README.md` & `zen_dash-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.0/pyproject.toml` & `zen_dash-0.6.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zen_dash"
-version = "0.6.0"
+version = "0.6.1"
 license = "MIT"
 description = "Simple yet scable and production ready python dashboard that is better than shiny application for business."
 readme = "README.md"
 authors = ["Zen <zenreportz@pm.me>"]
 homepage = "https://zen-reportz.github.io/zen_dash/index.html"
 repository = "https://github.com/Zen-Reportz/zen_dash"
 include = [
```

### Comparing `zen_dash-0.6.0/zen_dash/cli/project_management.py` & `zen_dash-0.6.1/zen_dash/cli/project_management.py`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.0/zen_dash/objects/__init__.py` & `zen_dash-0.6.1/zen_dash/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.0/zen_dash/objects/instances.py` & `zen_dash-0.6.1/zen_dash/objects/instances.py`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.0/zen_dash/objects/scripts.py` & `zen_dash-0.6.1/zen_dash/objects/scripts.py`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.0/zen_dash/objects/sidebar.py` & `zen_dash-0.6.1/zen_dash/objects/sidebar.py`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.0/zen_dash/page.py` & `zen_dash-0.6.1/zen_dash/page.py`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.0/zen_dash/static/275.44cd52f9d992445f.js` & `zen_dash-0.6.1/zen_dash/static/275.44cd52f9d992445f.js`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.0/zen_dash/static/3rdpartylicenses.txt` & `zen_dash-0.6.1/zen_dash/static/3rdpartylicenses.txt`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.0/zen_dash/static/MaterialIcons-Regular.196fa4a92dd6fa73.ttf` & `zen_dash-0.6.1/zen_dash/static/MaterialIcons-Regular.196fa4a92dd6fa73.ttf`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.0/zen_dash/static/MaterialIcons-Regular.1e50f5c2ffa6aba4.eot` & `zen_dash-0.6.1/zen_dash/static/MaterialIcons-Regular.1e50f5c2ffa6aba4.eot`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.0/zen_dash/static/MaterialIcons-Regular.7ea2023eeca07427.woff2` & `zen_dash-0.6.1/zen_dash/static/MaterialIcons-Regular.7ea2023eeca07427.woff2`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.0/zen_dash/static/MaterialIcons-Regular.db852539204b1a34.woff` & `zen_dash-0.6.1/zen_dash/static/MaterialIcons-Regular.db852539204b1a34.woff`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.0/zen_dash/static/favicon.ico` & `zen_dash-0.6.1/zen_dash/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.0/zen_dash/static/index.html` & `zen_dash-0.6.1/zen_dash/static/index.html`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.0/zen_dash/static/main.b01efffb503d168d.js` & `zen_dash-0.6.1/zen_dash/static/main.b01efffb503d168d.js`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.0/zen_dash/static/polyfills.0a8881ff36766b1e.js` & `zen_dash-0.6.1/zen_dash/static/polyfills.0a8881ff36766b1e.js`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.0/zen_dash/static/runtime.6a9b461ae5a72237.js` & `zen_dash-0.6.1/zen_dash/static/runtime.6a9b461ae5a72237.js`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.0/zen_dash/static/styles.362a8260c32d36d9.css` & `zen_dash-0.6.1/zen_dash/static/styles.362a8260c32d36d9.css`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.0/zen_dash/static/vendor.3c67e76b6e4a9ca3.js` & `zen_dash-0.6.1/zen_dash/static/vendor.3c67e76b6e4a9ca3.js`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.0/zen_dash/support/__init__.py` & `zen_dash-0.6.1/zen_dash/support/__init__.py`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.0/zen_dash/tag/__init__.py` & `zen_dash-0.6.1/zen_dash/tag/__init__.py`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.0/zen_dash/websocket/__init__.py` & `zen_dash-0.6.1/zen_dash/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.0/PKG-INFO` & `zen_dash-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zen-dash
-Version: 0.6.0
+Version: 0.6.1
 Summary: Simple yet scable and production ready python dashboard that is better than shiny application for business.
 Home-page: https://zen-reportz.github.io/zen_dash/index.html
 License: MIT
 Author: Zen
 Author-email: zenreportz@pm.me
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

