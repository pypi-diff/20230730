# Comparing `tmp/idendrogram_streamlit_component-0.2.2.tar.gz` & `tmp/idendrogram_streamlit_component-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idendrogram_streamlit_component-0.2.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "idendrogram_streamlit_component-0.2.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `idendrogram_streamlit_component-0.2.2.tar` & `idendrogram_streamlit_component-0.2.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0       24 2023-07-29 21:45:58.528315 idendrogram_streamlit_component-0.2.2/.gitignore
--rw-r--r--   0        0        0     1063 2023-07-08 23:56:47.273350 idendrogram_streamlit_component-0.2.2/LICENSE
--rw-r--r--   0        0        0       66 2023-07-23 18:39:02.909803 idendrogram_streamlit_component-0.2.2/MANIFEST.in
--rw-r--r--   0        0        0      930 2023-07-24 00:09:06.953233 idendrogram_streamlit_component-0.2.2/README.md
--rw-r--r--   0        0        0     2122 2023-07-29 22:36:21.255104 idendrogram_streamlit_component-0.2.2/idendrogram_streamlit_component/__init__.py
--rw-r--r--   0        0        0      180 2022-09-15 02:28:00.058747 idendrogram_streamlit_component-0.2.2/idendrogram_streamlit_component/frontend/.env
--rw-r--r--   0        0        0       67 2022-09-15 02:28:00.058747 idendrogram_streamlit_component-0.2.2/idendrogram_streamlit_component/frontend/.prettierrc
--rw-r--r--   0        0        0     1047 2023-07-29 21:38:19.855928 idendrogram_streamlit_component-0.2.2/idendrogram_streamlit_component/frontend/build/asset-manifest.json
--rw-r--r--   0        0        0   197459 2023-07-29 21:38:11.319263 idendrogram_streamlit_component-0.2.2/idendrogram_streamlit_component/frontend/build/bootstrap.min.css
--rw-r--r--   0        0        0     2177 2023-07-29 21:38:19.855928 idendrogram_streamlit_component-0.2.2/idendrogram_streamlit_component/frontend/build/index.html
--rw-r--r--   0        0        0      663 2023-07-29 21:38:19.855928 idendrogram_streamlit_component-0.2.2/idendrogram_streamlit_component/frontend/build/precache-manifest.3e58ef497f3baec2986da47144229e50.js
--rw-r--r--   0        0        0     1183 2023-07-29 21:38:19.855928 idendrogram_streamlit_component-0.2.2/idendrogram_streamlit_component/frontend/build/service-worker.js
--rw-r--r--   0        0        0      306 2023-07-29 21:38:19.855928 idendrogram_streamlit_component-0.2.2/idendrogram_streamlit_component/frontend/build/static/css/main.40e50dec.chunk.css
--rw-r--r--   0        0        0      632 2023-07-29 21:38:19.866761 idendrogram_streamlit_component-0.2.2/idendrogram_streamlit_component/frontend/build/static/css/main.40e50dec.chunk.css.map
--rw-r--r--   0        0        0   524006 2023-07-29 21:38:19.866761 idendrogram_streamlit_component-0.2.2/idendrogram_streamlit_component/frontend/build/static/js/2.09402de2.chunk.js
--rw-r--r--   0        0        0     1308 2023-07-29 21:38:19.866761 idendrogram_streamlit_component-0.2.2/idendrogram_streamlit_component/frontend/build/static/js/2.09402de2.chunk.js.LICENSE.txt
--rw-r--r--   0        0        0  1506803 2023-07-29 21:38:19.866761 idendrogram_streamlit_component-0.2.2/idendrogram_streamlit_component/frontend/build/static/js/2.09402de2.chunk.js.map
--rw-r--r--   0        0        0     4738 2023-07-29 21:38:19.866761 idendrogram_streamlit_component-0.2.2/idendrogram_streamlit_component/frontend/build/static/js/main.b350a90c.chunk.js
--rw-r--r--   0        0        0    19566 2023-07-29 21:38:19.866761 idendrogram_streamlit_component-0.2.2/idendrogram_streamlit_component/frontend/build/static/js/main.b350a90c.chunk.js.map
--rw-r--r--   0        0        0     1590 2023-07-29 21:38:19.855928 idendrogram_streamlit_component-0.2.2/idendrogram_streamlit_component/frontend/build/static/js/runtime-main.ea7b20aa.js
--rw-r--r--   0        0        0     8303 2023-07-29 21:38:19.866761 idendrogram_streamlit_component-0.2.2/idendrogram_streamlit_component/frontend/build/static/js/runtime-main.ea7b20aa.js.map
--rw-r--r--   0        0        0  1351829 2023-07-29 22:05:19.373874 idendrogram_streamlit_component-0.2.2/idendrogram_streamlit_component/frontend/package-lock.json
--rw-r--r--   0        0        0      770 2023-07-29 21:37:49.490101 idendrogram_streamlit_component-0.2.2/idendrogram_streamlit_component/frontend/package.json
--rw-r--r--   0        0        0   197459 2022-09-15 02:28:00.058747 idendrogram_streamlit_component-0.2.2/idendrogram_streamlit_component/frontend/public/bootstrap.min.css
--rw-r--r--   0        0        0      499 2022-09-24 02:15:10.021300 idendrogram_streamlit_component-0.2.2/idendrogram_streamlit_component/frontend/public/index.html
--rw-r--r--   0        0        0      339 2022-10-24 00:50:29.032266 idendrogram_streamlit_component-0.2.2/idendrogram_streamlit_component/frontend/src/idendro.css
--rw-r--r--   0        0        0    12388 2023-07-29 17:23:28.905419 idendrogram_streamlit_component-0.2.2/idendrogram_streamlit_component/frontend/src/index.tsx
--rw-r--r--   0        0        0       40 2022-09-15 02:28:00.058747 idendrogram_streamlit_component-0.2.2/idendrogram_streamlit_component/frontend/src/react-app-env.d.ts
--rw-r--r--   0        0        0      459 2022-09-15 02:28:00.058747 idendrogram_streamlit_component-0.2.2/idendrogram_streamlit_component/frontend/tsconfig.json
--rw-r--r--   0        0        0      880 2023-07-23 21:24:03.480085 idendrogram_streamlit_component-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1635 1970-01-01 00:00:00.000000 idendrogram_streamlit_component-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0       24 2023-07-29 21:45:58.528315 idendrogram_streamlit_component-0.2.3/.gitignore
+-rw-r--r--   0        0        0     1063 2023-07-08 23:56:47.273350 idendrogram_streamlit_component-0.2.3/LICENSE
+-rw-r--r--   0        0        0       66 2023-07-23 18:39:02.909803 idendrogram_streamlit_component-0.2.3/MANIFEST.in
+-rw-r--r--   0        0        0     1095 2023-07-29 22:49:48.067418 idendrogram_streamlit_component-0.2.3/README.md
+-rw-r--r--   0        0        0     2122 2023-07-29 22:50:47.249904 idendrogram_streamlit_component-0.2.3/idendrogram_streamlit_component/__init__.py
+-rw-r--r--   0        0        0      180 2022-09-15 02:28:00.058747 idendrogram_streamlit_component-0.2.3/idendrogram_streamlit_component/frontend/.env
+-rw-r--r--   0        0        0       67 2022-09-15 02:28:00.058747 idendrogram_streamlit_component-0.2.3/idendrogram_streamlit_component/frontend/.prettierrc
+-rw-r--r--   0        0        0     1047 2023-07-29 21:38:19.855928 idendrogram_streamlit_component-0.2.3/idendrogram_streamlit_component/frontend/build/asset-manifest.json
+-rw-r--r--   0        0        0   197459 2023-07-29 21:38:11.319263 idendrogram_streamlit_component-0.2.3/idendrogram_streamlit_component/frontend/build/bootstrap.min.css
+-rw-r--r--   0        0        0     2177 2023-07-29 21:38:19.855928 idendrogram_streamlit_component-0.2.3/idendrogram_streamlit_component/frontend/build/index.html
+-rw-r--r--   0        0        0      663 2023-07-29 21:38:19.855928 idendrogram_streamlit_component-0.2.3/idendrogram_streamlit_component/frontend/build/precache-manifest.3e58ef497f3baec2986da47144229e50.js
+-rw-r--r--   0        0        0     1183 2023-07-29 21:38:19.855928 idendrogram_streamlit_component-0.2.3/idendrogram_streamlit_component/frontend/build/service-worker.js
+-rw-r--r--   0        0        0      306 2023-07-29 21:38:19.855928 idendrogram_streamlit_component-0.2.3/idendrogram_streamlit_component/frontend/build/static/css/main.40e50dec.chunk.css
+-rw-r--r--   0        0        0      632 2023-07-29 21:38:19.866761 idendrogram_streamlit_component-0.2.3/idendrogram_streamlit_component/frontend/build/static/css/main.40e50dec.chunk.css.map
+-rw-r--r--   0        0        0   524006 2023-07-29 21:38:19.866761 idendrogram_streamlit_component-0.2.3/idendrogram_streamlit_component/frontend/build/static/js/2.09402de2.chunk.js
+-rw-r--r--   0        0        0     1308 2023-07-29 21:38:19.866761 idendrogram_streamlit_component-0.2.3/idendrogram_streamlit_component/frontend/build/static/js/2.09402de2.chunk.js.LICENSE.txt
+-rw-r--r--   0        0        0  1506803 2023-07-29 21:38:19.866761 idendrogram_streamlit_component-0.2.3/idendrogram_streamlit_component/frontend/build/static/js/2.09402de2.chunk.js.map
+-rw-r--r--   0        0        0     4738 2023-07-29 21:38:19.866761 idendrogram_streamlit_component-0.2.3/idendrogram_streamlit_component/frontend/build/static/js/main.b350a90c.chunk.js
+-rw-r--r--   0        0        0    19566 2023-07-29 21:38:19.866761 idendrogram_streamlit_component-0.2.3/idendrogram_streamlit_component/frontend/build/static/js/main.b350a90c.chunk.js.map
+-rw-r--r--   0        0        0     1590 2023-07-29 21:38:19.855928 idendrogram_streamlit_component-0.2.3/idendrogram_streamlit_component/frontend/build/static/js/runtime-main.ea7b20aa.js
+-rw-r--r--   0        0        0     8303 2023-07-29 21:38:19.866761 idendrogram_streamlit_component-0.2.3/idendrogram_streamlit_component/frontend/build/static/js/runtime-main.ea7b20aa.js.map
+-rw-r--r--   0        0        0  1351829 2023-07-29 22:05:19.373874 idendrogram_streamlit_component-0.2.3/idendrogram_streamlit_component/frontend/package-lock.json
+-rw-r--r--   0        0        0      770 2023-07-29 21:37:49.490101 idendrogram_streamlit_component-0.2.3/idendrogram_streamlit_component/frontend/package.json
+-rw-r--r--   0        0        0   197459 2022-09-15 02:28:00.058747 idendrogram_streamlit_component-0.2.3/idendrogram_streamlit_component/frontend/public/bootstrap.min.css
+-rw-r--r--   0        0        0      499 2022-09-24 02:15:10.021300 idendrogram_streamlit_component-0.2.3/idendrogram_streamlit_component/frontend/public/index.html
+-rw-r--r--   0        0        0      339 2022-10-24 00:50:29.032266 idendrogram_streamlit_component-0.2.3/idendrogram_streamlit_component/frontend/src/idendro.css
+-rw-r--r--   0        0        0    12388 2023-07-29 17:23:28.905419 idendrogram_streamlit_component-0.2.3/idendrogram_streamlit_component/frontend/src/index.tsx
+-rw-r--r--   0        0        0       40 2022-09-15 02:28:00.058747 idendrogram_streamlit_component-0.2.3/idendrogram_streamlit_component/frontend/src/react-app-env.d.ts
+-rw-r--r--   0        0        0      459 2022-09-15 02:28:00.058747 idendrogram_streamlit_component-0.2.3/idendrogram_streamlit_component/frontend/tsconfig.json
+-rw-r--r--   0        0        0      880 2023-07-23 21:24:03.480085 idendrogram_streamlit_component-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1800 1970-01-01 00:00:00.000000 idendrogram_streamlit_component-0.2.3/PKG-INFO
```

### Comparing `idendrogram_streamlit_component-0.2.2/LICENSE` & `idendrogram_streamlit_component-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `idendrogram_streamlit_component-0.2.2/README.md` & `idendrogram_streamlit_component-0.2.3/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # idendrogram-streamlit-component
 
 A D3-powered bi-directional Streamlit component for idendrogram library that visualizes dendrograms created by hierarchical clustering algorithms (SciPy, scikit-learn and hdbscan compatible).
 
-Demo [TBD]
+Demo available at https://idendrogram.streamlit.app/. 
 
 Docs @ https://kamicollo.github.io/idendrogram/
 
 ## Customizing the component
 
 If you would like to go beyond customization supported by this component out of the box (e.g. do some **_really fancy_** tooltips), you'll need:
 
 * To be familiar with [bi-directional Streamlit component development](https://docs.streamlit.io/library/components/components-api#create-a-bi-directional-component)
 * Clone this repo
-* Adjust the release flag in `idendrogram_streamlit_component/__init__.py` file to `False`, so it runs against the local development server
-* Make adjustments! The D3 component is written in a single file (`index.tsx`), and the tooltip creation is part of `draw_nodes()` function. 
+* Make adjustments! The D3 component is written in a single file (`index.tsx`), and the tooltip creation is part of `draw_nodes()` function. 
+* Run the npm server locally with `npm run start`
+* In your Streamlit app, [use the `StreamlitConverter(release=False)`](https://kamicollo.github.io/idendrogram/streamlit/#customizing-streamlit-dendrograms) to get idendrogram to look for the local NPM server.
```

### Comparing `idendrogram_streamlit_component-0.2.2/idendrogram_streamlit_component/__init__.py` & `idendrogram_streamlit_component-0.2.3/idendrogram_streamlit_component/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Bi-directional Streamlit component for creating interactive dendrograms"""
 
-__version__ = "0.2.2"
+__version__ = "0.2.3"
 
 
 import json
 import os
 from typing import Optional, Dict
 import streamlit.components.v1 as components
 from idendrogram.containers import ClusterNode, Dendrogram
```

### Comparing `idendrogram_streamlit_component-0.2.2/idendrogram_streamlit_component/frontend/build/asset-manifest.json` & `idendrogram_streamlit_component-0.2.3/idendrogram_streamlit_component/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `idendrogram_streamlit_component-0.2.2/idendrogram_streamlit_component/frontend/build/bootstrap.min.css` & `idendrogram_streamlit_component-0.2.3/idendrogram_streamlit_component/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `idendrogram_streamlit_component-0.2.2/idendrogram_streamlit_component/frontend/build/index.html` & `idendrogram_streamlit_component-0.2.3/idendrogram_streamlit_component/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `idendrogram_streamlit_component-0.2.2/idendrogram_streamlit_component/frontend/build/precache-manifest.3e58ef497f3baec2986da47144229e50.js` & `idendrogram_streamlit_component-0.2.3/idendrogram_streamlit_component/frontend/build/precache-manifest.3e58ef497f3baec2986da47144229e50.js`

 * *Files identical despite different names*

### Comparing `idendrogram_streamlit_component-0.2.2/idendrogram_streamlit_component/frontend/build/service-worker.js` & `idendrogram_streamlit_component-0.2.3/idendrogram_streamlit_component/frontend/build/service-worker.js`

 * *Files identical despite different names*

### Comparing `idendrogram_streamlit_component-0.2.2/idendrogram_streamlit_component/frontend/build/static/css/main.40e50dec.chunk.css.map` & `idendrogram_streamlit_component-0.2.3/idendrogram_streamlit_component/frontend/build/static/css/main.40e50dec.chunk.css.map`

 * *Files identical despite different names*

### Comparing `idendrogram_streamlit_component-0.2.2/idendrogram_streamlit_component/frontend/build/static/js/2.09402de2.chunk.js` & `idendrogram_streamlit_component-0.2.3/idendrogram_streamlit_component/frontend/build/static/js/2.09402de2.chunk.js`

 * *Files identical despite different names*

### Comparing `idendrogram_streamlit_component-0.2.2/idendrogram_streamlit_component/frontend/build/static/js/2.09402de2.chunk.js.LICENSE.txt` & `idendrogram_streamlit_component-0.2.3/idendrogram_streamlit_component/frontend/build/static/js/2.09402de2.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `idendrogram_streamlit_component-0.2.2/idendrogram_streamlit_component/frontend/build/static/js/2.09402de2.chunk.js.map` & `idendrogram_streamlit_component-0.2.3/idendrogram_streamlit_component/frontend/build/static/js/2.09402de2.chunk.js.map`

 * *Files identical despite different names*

### Comparing `idendrogram_streamlit_component-0.2.2/idendrogram_streamlit_component/frontend/build/static/js/main.b350a90c.chunk.js` & `idendrogram_streamlit_component-0.2.3/idendrogram_streamlit_component/frontend/build/static/js/main.b350a90c.chunk.js`

 * *Files identical despite different names*

### Comparing `idendrogram_streamlit_component-0.2.2/idendrogram_streamlit_component/frontend/build/static/js/main.b350a90c.chunk.js.map` & `idendrogram_streamlit_component-0.2.3/idendrogram_streamlit_component/frontend/build/static/js/main.b350a90c.chunk.js.map`

 * *Files identical despite different names*

### Comparing `idendrogram_streamlit_component-0.2.2/idendrogram_streamlit_component/frontend/build/static/js/runtime-main.ea7b20aa.js` & `idendrogram_streamlit_component-0.2.3/idendrogram_streamlit_component/frontend/build/static/js/runtime-main.ea7b20aa.js`

 * *Files identical despite different names*

### Comparing `idendrogram_streamlit_component-0.2.2/idendrogram_streamlit_component/frontend/build/static/js/runtime-main.ea7b20aa.js.map` & `idendrogram_streamlit_component-0.2.3/idendrogram_streamlit_component/frontend/build/static/js/runtime-main.ea7b20aa.js.map`

 * *Files identical despite different names*

### Comparing `idendrogram_streamlit_component-0.2.2/idendrogram_streamlit_component/frontend/package-lock.json` & `idendrogram_streamlit_component-0.2.3/idendrogram_streamlit_component/frontend/package-lock.json`

 * *Files identical despite different names*

### Comparing `idendrogram_streamlit_component-0.2.2/idendrogram_streamlit_component/frontend/package.json` & `idendrogram_streamlit_component-0.2.3/idendrogram_streamlit_component/frontend/package.json`

 * *Files identical despite different names*

### Comparing `idendrogram_streamlit_component-0.2.2/idendrogram_streamlit_component/frontend/public/bootstrap.min.css` & `idendrogram_streamlit_component-0.2.3/idendrogram_streamlit_component/frontend/public/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `idendrogram_streamlit_component-0.2.2/idendrogram_streamlit_component/frontend/src/index.tsx` & `idendrogram_streamlit_component-0.2.3/idendrogram_streamlit_component/frontend/src/index.tsx`

 * *Files identical despite different names*

### Comparing `idendrogram_streamlit_component-0.2.2/pyproject.toml` & `idendrogram_streamlit_component-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `idendrogram_streamlit_component-0.2.2/PKG-INFO` & `idendrogram_streamlit_component-0.2.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idendrogram-streamlit-component
-Version: 0.2.2
+Version: 0.2.3
 Summary: Bi-directional Streamlit component for creating interactive dendrograms
 Keywords: dendrogram,hierarchical clustering,clustering,streamlit,D3
 Author: Aurimas Racas
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -15,19 +15,20 @@
 Project-URL: Home, https://github.com/kamicollo/idendrogram-streamlit
 Provides-Extra: full
 
 # idendrogram-streamlit-component
 
 A D3-powered bi-directional Streamlit component for idendrogram library that visualizes dendrograms created by hierarchical clustering algorithms (SciPy, scikit-learn and hdbscan compatible).
 
-Demo [TBD]
+Demo available at https://idendrogram.streamlit.app/. 
 
 Docs @ https://kamicollo.github.io/idendrogram/
 
 ## Customizing the component
 
 If you would like to go beyond customization supported by this component out of the box (e.g. do some **_really fancy_** tooltips), you'll need:
 
 * To be familiar with [bi-directional Streamlit component development](https://docs.streamlit.io/library/components/components-api#create-a-bi-directional-component)
 * Clone this repo
-* Adjust the release flag in `idendrogram_streamlit_component/__init__.py` file to `False`, so it runs against the local development server
 * Make adjustments! The D3 component is written in a single file (`index.tsx`), and the tooltip creation is part of `draw_nodes()` function. 
+* Run the npm server locally with `npm run start`
+* In your Streamlit app, [use the `StreamlitConverter(release=False)`](https://kamicollo.github.io/idendrogram/streamlit/#customizing-streamlit-dendrograms) to get idendrogram to look for the local NPM server.
```

