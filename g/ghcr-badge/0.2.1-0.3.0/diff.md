# Comparing `tmp/ghcr_badge-0.2.1.tar.gz` & `tmp/ghcr_badge-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghcr_badge-0.2.1.tar", max compression
+gzip compressed data, was "ghcr_badge-0.3.0.tar", max compression
```

## Comparing `ghcr_badge-0.2.1.tar` & `ghcr_badge-0.3.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1049 2023-05-07 12:23:20.181370 ghcr_badge-0.2.1/LICENSE.txt
--rw-r--r--   0        0        0     3617 2023-05-07 12:23:20.181370 ghcr_badge-0.2.1/README.md
--rw-r--r--   0        0        0      125 2023-05-07 12:23:20.181370 ghcr_badge-0.2.1/ghcr_badge/__init__.py
--rw-r--r--   0        0        0     1282 2023-05-07 12:23:20.181370 ghcr_badge-0.2.1/ghcr_badge/dicts.py
--rw-r--r--   0        0        0    13171 2023-05-07 12:23:20.181370 ghcr_badge-0.2.1/ghcr_badge/generate.py
--rw-r--r--   0        0        0     2859 2023-05-07 12:23:20.181370 ghcr_badge-0.2.1/ghcr_badge/main.py
--rw-r--r--   0        0        0        0 2023-05-07 12:23:20.181370 ghcr_badge-0.2.1/ghcr_badge/py.typed
--rw-r--r--   0        0        0     6763 2023-05-07 12:23:20.185370 ghcr_badge-0.2.1/ghcr_badge/server.py
--rw-r--r--   0        0        0      721 2023-05-07 12:23:20.185370 ghcr_badge-0.2.1/ghcr_badge/svg/mark-github.svg
--rw-r--r--   0        0        0      540 2023-05-07 12:23:20.185370 ghcr_badge-0.2.1/ghcr_badge/svg/package-16.svg
--rw-r--r--   0        0        0     1670 2023-05-07 12:23:20.185370 ghcr_badge-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     4900 1970-01-01 00:00:00.000000 ghcr_badge-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1049 2023-07-30 16:35:59.907051 ghcr_badge-0.3.0/LICENSE.txt
+-rw-r--r--   0        0        0     3802 2023-07-30 16:35:59.907051 ghcr_badge-0.3.0/README.md
+-rw-r--r--   0        0        0      125 2023-07-30 16:35:59.907051 ghcr_badge-0.3.0/ghcr_badge/__init__.py
+-rw-r--r--   0        0        0     1282 2023-07-30 16:35:59.907051 ghcr_badge-0.3.0/ghcr_badge/dicts.py
+-rw-r--r--   0        0        0    13055 2023-07-30 16:35:59.907051 ghcr_badge-0.3.0/ghcr_badge/generate.py
+-rw-r--r--   0        0        0     2859 2023-07-30 16:35:59.907051 ghcr_badge-0.3.0/ghcr_badge/main.py
+-rw-r--r--   0        0        0        0 2023-07-30 16:35:59.911051 ghcr_badge-0.3.0/ghcr_badge/py.typed
+-rw-r--r--   0        0        0     7454 2023-07-30 16:35:59.911051 ghcr_badge-0.3.0/ghcr_badge/server.py
+-rw-r--r--   0        0        0      721 2023-07-30 16:35:59.911051 ghcr_badge-0.3.0/ghcr_badge/svg/mark-github.svg
+-rw-r--r--   0        0        0      540 2023-07-30 16:35:59.911051 ghcr_badge-0.3.0/ghcr_badge/svg/package-16.svg
+-rw-r--r--   0        0        0     6014 2023-07-30 16:35:59.911051 ghcr_badge-0.3.0/ghcr_badge/templates/index.j2
+-rw-r--r--   0        0        0     1798 2023-07-30 16:35:59.911051 ghcr_badge-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5033 1970-01-01 00:00:00.000000 ghcr_badge-0.3.0/PKG-INFO
```

### Comparing `ghcr_badge-0.2.1/LICENSE.txt` & `ghcr_badge-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ghcr_badge-0.2.1/README.md` & `ghcr_badge-0.3.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -89,7 +89,13 @@
 curl -X PURGE "https://camo.githubusercontent.com/..."
 ```
 
 [1]: <https://ghcr-badge.egpl.dev/eggplants/ghcr-badge/tags?trim=major>
 [2]: <https://ghcr-badge.egpl.dev/eggplants/ghcr-badge/latest_tag?trim=major&label=latest>
 [3]: <https://ghcr-badge.egpl.dev/ptr727/plexcleaner/develop_tag>
 [4]: <https://ghcr-badge.egpl.dev/eggplants/ghcr-badge/size>
+
+## Development
+
+1. Install [`poetry`](https://python-poetry.org/docs/#installation)
+1. Run `poetry install && poetry shell && pre-commit install`
+1. Launch live server with `task dev`
```

### Comparing `ghcr_badge-0.2.1/ghcr_badge/dicts.py` & `ghcr_badge-0.3.0/ghcr_badge/dicts.py`

 * *Files identical despite different names*

### Comparing `ghcr_badge-0.2.1/ghcr_badge/generate.py` & `ghcr_badge-0.3.0/ghcr_badge/generate.py`

 * *Files 2% similar despite different names*

```diff
@@ -297,20 +297,15 @@
         token = self.__auth(package_owner, package_name)
         url = f"https://ghcr.io/v2/{package_owner}/{package_name}/manifests/{tag}"
         manifest = requests.get(
             url,
             headers={
                 "User-Agent": _USER_AGENT,
                 "Authorization": f"Bearer {token}",
-                "Accept": ", ".join(
-                    (
-                        _MEDIA_TYPE_OCI_IMAGE_INDEX_V1,
-                        _MEDIA_TYPE_OCI_IMAGE_MANIFEST_V1,
-                    ),
-                ),
+                "Accept": f"{_MEDIA_TYPE_OCI_IMAGE_INDEX_V1}, {_MEDIA_TYPE_OCI_IMAGE_MANIFEST_V1}",
             },
             timeout=_TIMEOUT,
         ).json()
 
         if manifest is None:
             msg = "manifest is empty."
             raise InvalidManifestError(msg)
```

### Comparing `ghcr_badge-0.2.1/ghcr_badge/main.py` & `ghcr_badge-0.3.0/ghcr_badge/main.py`

 * *Files identical despite different names*

### Comparing `ghcr_badge-0.2.1/ghcr_badge/server.py` & `ghcr_badge-0.3.0/ghcr_badge/server.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,23 +2,26 @@
 
 from __future__ import annotations
 
 from datetime import datetime, timedelta, timezone
 from os import environ
 from typing import TYPE_CHECKING
 
-from flask import Flask, jsonify, make_response, request
+from flask import Flask, jsonify, make_response, render_template, request
+from flask.wrappers import Response
 
 from . import __version__
 from .generate import GHCRBadgeGenerator
 
 if TYPE_CHECKING:
-    from flask.wrappers import Response
+    from typing import Literal
+
 
 _PACKAGE_PARAM_RULE = "/<package_owner>/<path:package_name>"
+_REPO_LINK = "https://github.com/eggplants/ghcr-badge"
 
 app = Flask(__name__)
 app.config["JSONIFY_PRETTYPRINT_REGULAR"] = True
 
 
 def return_svg(svg: str) -> Response:
     """Return a generated svg as `Flask.Response`.
@@ -43,20 +46,46 @@
     res.headers["Pragma"] = "no-cache"  # for HTTP 1.0
     res.headers["Expires"] = expiry_time.strftime("%a, %d %b %Y %H:%M:%S GMT")
 
     return res
 
 
 @app.route("/", methods=["GET"])
-def get_index() -> Response:
+@app.route("/index", methods=["GET"])
+@app.route("/index<any('.html', '.json'):ext>", methods=["GET"])
+def get_index(ext: Literal[".html"] | Literal[".json"] = ".html") -> Response:
     """Handle GET `/`.
 
     Returns
     -------
     Response
+        JSON or HTML
+    """
+    if ext == ".json":
+        return __get_index_json()
+    return __get_index_html()
+
+
+def __get_index_html() -> Response:
+    """Handle GET `/` and response as html.
+
+    Returns
+    -------
+    Response
+        HTML
+    """
+    return Response(render_template("index.j2", version=__version__, repo_link=_REPO_LINK))
+
+
+def __get_index_json() -> Response:
+    """Handle GET `/` and response as json.
+
+    Returns
+    -------
+    Response
         JSON
     """
     try:
         return jsonify(
             {
                 "available_paths": [
                     "/",
@@ -71,15 +100,15 @@
                     "/eggplants/ghcr-badge/latest_tag",
                     "/ptr727/plexcleaner/develop_tag",
                     "/eggplants/ghcr-badge/size",
                     "/frysztak/orpington-news/size",
                     "/tuananh/aws-cli/size",
                     "/plantuml/docker%2Fjekyll/tags",
                 ],
-                "repo": "https://github.com/eggplants/ghcr-badge",
+                "repo": _REPO_LINK,
                 "version": __version__,
             },
         )
     except Exception as err:  # noqa: BLE001
         return jsonify(exception=type(err).__name__)
```

### Comparing `ghcr_badge-0.2.1/ghcr_badge/svg/mark-github.svg` & `ghcr_badge-0.3.0/ghcr_badge/svg/mark-github.svg`

 * *Files identical despite different names*

### Comparing `ghcr_badge-0.2.1/ghcr_badge/svg/package-16.svg` & `ghcr_badge-0.3.0/ghcr_badge/svg/package-16.svg`

 * *Files identical despite different names*

### Comparing `ghcr_badge-0.2.1/pyproject.toml` & `ghcr_badge-0.3.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -3,38 +3,14 @@
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = [
   "poetry-core",
 ]
 
 [tool]
-[tool.black]
-line-length = 120
-target-version = ['py39']
-
-[tool.isort]
-profile = "black"
-
-[tool.mypy]
-pretty = true
-python_version = "3.9"
-show_error_codes = true
-strict = true
-
-[tool.ruff]
-select = ["ALL"]
-ignore = [
-  "D203", # no-blank-line-before-class
-  "D213", # multi-line-summary-second-line
-]
-line-length = 120
-
-[tool.ruff.mccabe]
-max-complexity = 18
-
 [tool.poetry]
 authors = ["eggplants <w10776e8w@yahoo.co.jp>"]
 classifiers = [
   "Development Status :: 3 - Alpha",
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3 :: Only",
@@ -43,34 +19,63 @@
 description = "Generate ghcr.io container's status badge"
 keywords = ["github-container-registry", "badge", "ghcr"]
 name = "ghcr_badge"
 packages = [{include = "ghcr_badge"}]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/eggplants/ghcr-badge"
-version = "0.2.1"
+version = "0.3.0"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 anybadge="^1.9.0"
 flask="^2.1.2"
-gunicorn="^20.1.0"
+gunicorn=">=20.1,<22.0"
 humanfriendly="^10.0"
 requests="^2.28.0"
 types-humanfriendly="^10.0"
 types-requests="^2.28.0"
 typing-extensions = "^4.5.0"
 
 [tool.poetry.group.dev.dependencies]
-mypy = ">=0.991,<1.3"
+mypy = ">=0.991,<1.5"
 pre-commit = ">=2.20,<4.0"
 taskipy = "^1.10.3"
 
 [tool.poetry.scripts]
 ghcr-badge-server = "ghcr_badge.server:main"
 ghcr-badge = "ghcr_badge.main:main"
 
+[tool.black]
+line-length = 120
+target-version = ['py39']
+
+[tool.ruff]
+select = ["ALL"]
+ignore = [
+  "D203", # no-blank-line-before-class
+  "D213", # multi-line-summary-second-line
+]
+line-length = 120
+
+[tool.ruff.mccabe]
+max-complexity = 18
+
+[tool.mypy]
+pretty = true
+python_version = "3.9"
+show_error_codes = true
+strict = true
+
+[tool.djlint]
+format_css=true
+format_js=true
+indent = 2
+css.indent_size = 2
+js.indent_size = 2
+
 [tool.poetry_bumpversion.file."ghcr_badge/__init__.py"]
 
 [tool.taskipy.tasks]
 lint = "pre-commit run -a"
 profile = "python -m cProfile"
+dev = "flask --app ghcr_badge.server run --debug --reload"
```

### Comparing `ghcr_badge-0.2.1/PKG-INFO` & `ghcr_badge-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: ghcr-badge
-Version: 0.2.1
+Version: 0.3.0
 Summary: Generate ghcr.io container's status badge
 Home-page: https://github.com/eggplants/ghcr-badge
 License: MIT
 Keywords: github-container-registry,badge,ghcr
 Author: eggplants
 Author-email: w10776e8w@yahoo.co.jp
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Dist: anybadge (>=1.9.0,<2.0.0)
 Requires-Dist: flask (>=2.1.2,<3.0.0)
-Requires-Dist: gunicorn (>=20.1.0,<21.0.0)
+Requires-Dist: gunicorn (>=20.1,<22.0)
 Requires-Dist: humanfriendly (>=10.0,<11.0)
 Requires-Dist: requests (>=2.28.0,<3.0.0)
 Requires-Dist: types-humanfriendly (>=10.0,<11.0)
 Requires-Dist: types-requests (>=2.28.0,<3.0.0)
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
 Project-URL: Repository, https://github.com/eggplants/ghcr-badge
 Description-Content-Type: text/markdown
@@ -121,7 +120,13 @@
 ```
 
 [1]: <https://ghcr-badge.egpl.dev/eggplants/ghcr-badge/tags?trim=major>
 [2]: <https://ghcr-badge.egpl.dev/eggplants/ghcr-badge/latest_tag?trim=major&label=latest>
 [3]: <https://ghcr-badge.egpl.dev/ptr727/plexcleaner/develop_tag>
 [4]: <https://ghcr-badge.egpl.dev/eggplants/ghcr-badge/size>
 
+## Development
+
+1. Install [`poetry`](https://python-poetry.org/docs/#installation)
+1. Run `poetry install && poetry shell && pre-commit install`
+1. Launch live server with `task dev`
+
```

