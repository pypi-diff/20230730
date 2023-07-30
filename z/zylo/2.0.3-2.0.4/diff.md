# Comparing `tmp/zylo-2.0.3.tar.gz` & `tmp/zylo-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zylo-2.0.3.tar", last modified: Thu Jul 20 08:03:48 2023, max compression
+gzip compressed data, was "zylo-2.0.4.tar", last modified: Sun Jul 30 03:39:17 2023, max compression
```

## Comparing `zylo-2.0.3.tar` & `zylo-2.0.4.tar`

### file list

```diff
@@ -1,20 +1,27 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-20 08:03:48.200309 zylo-2.0.3/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5184 2023-07-20 08:03:48.200309 zylo-2.0.3/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4558 2023-07-20 07:54:02.000000 zylo-2.0.3/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-20 08:03:48.200309 zylo-2.0.3/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      930 2023-07-20 07:53:01.000000 zylo-2.0.3/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-20 08:03:48.200309 zylo-2.0.3/zylo/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7362 2023-07-17 17:19:23.000000 zylo-2.0.3/zylo/JwT.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       19 2023-07-14 10:05:50.000000 zylo-2.0.3/zylo/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6918 2023-07-20 07:51:03.000000 zylo-2.0.3/zylo/app.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2316 2023-07-17 17:30:16.000000 zylo-2.0.3/zylo/blueprint.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6341 2023-07-14 06:35:56.000000 zylo-2.0.3/zylo/chiper.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1156 2023-07-16 18:57:34.000000 zylo-2.0.3/zylo/limiter.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3003 2023-07-20 07:52:15.000000 zylo-2.0.3/zylo/mailer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1268 2023-07-16 18:47:33.000000 zylo-2.0.3/zylo/sessions.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-20 08:03:48.200309 zylo-2.0.3/zylo.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5184 2023-07-20 08:03:47.000000 zylo-2.0.3/zylo.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      279 2023-07-20 08:03:47.000000 zylo-2.0.3/zylo.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-20 08:03:47.000000 zylo-2.0.3/zylo.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       53 2023-07-20 08:03:47.000000 zylo-2.0.3/zylo.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        5 2023-07-20 08:03:47.000000 zylo-2.0.3/zylo.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-30 03:39:17.778519 zylo-2.0.4/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1980 2023-07-30 03:39:17.778519 zylo-2.0.4/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1354 2023-07-30 03:37:44.000000 zylo-2.0.4/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-30 03:39:17.778519 zylo-2.0.4/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      930 2023-07-30 03:14:31.000000 zylo-2.0.4/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-30 03:39:17.774519 zylo-2.0.4/zylo/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-30 03:14:13.000000 zylo-2.0.4/zylo/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-30 03:39:17.774519 zylo-2.0.4/zylo/components/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 11:07:00.000000 zylo-2.0.4/zylo/components/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2316 2023-07-27 11:14:32.000000 zylo-2.0.4/zylo/components/blueprint.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1268 2023-07-27 11:06:48.000000 zylo-2.0.4/zylo/components/sessions.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-30 03:39:17.774519 zylo-2.0.4/zylo/core/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 11:27:23.000000 zylo-2.0.4/zylo/core/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7531 2023-07-28 14:53:12.000000 zylo-2.0.4/zylo/core/branch.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-30 03:39:17.778519 zylo-2.0.4/zylo/mail/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 11:25:41.000000 zylo-2.0.4/zylo/mail/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3012 2023-07-28 15:15:20.000000 zylo-2.0.4/zylo/mail/zylo_mailer.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-30 03:39:17.778519 zylo-2.0.4/zylo/security/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7362 2023-07-27 11:24:02.000000 zylo-2.0.4/zylo/security/JwT.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 11:23:50.000000 zylo-2.0.4/zylo/security/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6341 2023-07-27 11:26:09.000000 zylo-2.0.4/zylo/security/chiper.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-30 03:39:17.774519 zylo-2.0.4/zylo.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1980 2023-07-30 03:39:17.000000 zylo-2.0.4/zylo.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      419 2023-07-30 03:39:17.000000 zylo-2.0.4/zylo.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-30 03:39:17.000000 zylo-2.0.4/zylo.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       53 2023-07-30 03:39:17.000000 zylo-2.0.4/zylo.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        5 2023-07-30 03:39:17.000000 zylo-2.0.4/zylo.egg-info/top_level.txt
```

### Comparing `zylo-2.0.3/setup.py` & `zylo-2.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='zylo',
-    version='2.0.3',
+    version='2.0.4',
     description='A lightweight web framework made with love',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Pawan kumar',
     author_email='control@vvfin.in',
     url='https://github.com/E491K7/zylo',
     packages=find_packages(),
```

### Comparing `zylo-2.0.3/zylo/JwT.py` & `zylo-2.0.4/zylo/security/JwT.py`

 * *Files identical despite different names*

### Comparing `zylo-2.0.3/zylo/app.py` & `zylo-2.0.4/zylo/core/branch.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,48 +1,120 @@
 import os
 import base64
-from werkzeug.wrappers import Request, Response
+from werkzeug.wrappers import Request, Response, request
 from werkzeug.routing import Map, Rule
 from werkzeug.exceptions import HTTPException, NotFound
 from werkzeug.middleware.shared_data import SharedDataMiddleware
 from werkzeug.debug import DebuggedApplication
-from jinja2 import Environment, FileSystemLoader
-from .sessions import session_manager
-from .blueprint import Blueprint
+from jinja2 import Environment, FileSystemLoader, TemplateNotFound
+from ..components.sessions import session_manager
+from ..components.blueprint import Blueprint
 from werkzeug.urls import url_encode
 from itsdangerous import URLSafeTimedSerializer
 import json
 import mimetypes
 from urllib.parse import quote as url_quote, quote_plus as url_quote_plus, urlencode as url_encode
 from werkzeug.utils import send_from_directory, safe_join
+import importlib
 
-# Create the application
 class Zylo:
     def __init__(self, __name__=None):
-        self.template_folder='views'
+        self.template_folder = 'views'
         self.url_map = Map()
         self.static_folder = "static"
         self.error_handlers = {}
         self.middlewares = []
         self.template_env = Environment(loader=FileSystemLoader(self.template_folder))
-        self.host = 'localhost'
-        self.port = 8000
-        self.debug = True
+        self.host = None
+        self.port = None
+        self.debug = None
         self.secret_key = os.urandom(24)
         self.serializer = URLSafeTimedSerializer(base64.urlsafe_b64encode(self.secret_key))
         self.blueprints = []
         self.__name__ = __name__
         self.config = {}
 
-    def add_url_rule(self, rule, endpoint, handler, methods=['GET']):
-        def view_func(request, **values):
-            return handler(request, **values)
-        self.url_map.add(Rule(rule, endpoint=endpoint, methods=methods))
-        setattr(self, endpoint, view_func)
+    def get_config(self, key, default=None):
+        return self.config.get(key, default)
 
+    def load_settings_from_module(self, module_name):
+        try:
+            module = importlib.import_module(module_name)
+            self.host = module.HOST
+            self.port = module.PORT
+            self.debug = module.DEBUG
+        except ImportError:
+            pass
+
+    def load_settings(self):
+        self.load_settings_from_module('settings')
+
+    def load_routes(self):
+        try:
+            urls_module = importlib.import_module('urls')
+            urlpatterns = getattr(urls_module, 'urlpatterns', [])
+            for route, *args in urlpatterns:
+                if callable(args[0]):
+                    view_func = args[0]
+                    methods = args[1] if len(args) > 1 else None
+                else:
+                    view_func = args[1]
+                    methods = args[2] if len(args) > 2 else None
+                self.add_url_rule(route, view_func, methods=methods)
+        except ImportError:
+            pass
+
+    def validate_backend(self, backend):
+        supported_backends = ['zylo.template.backends.DjangoTemplates']
+        if backend not in supported_backends:
+            raise ValueError(f"Zylo template engine doesn't support this backend: {backend}")
+
+    def setup_template_env(self):
+        templates = self.get_config('TEMPLATES')
+        if templates:
+            backend = templates[0].get('BACKEND')
+            dirs = templates[0].get('DIRS', [])
+        else:
+            backend = None
+            dirs = []
+
+        if backend:
+            self.validate_backend(backend)
+            if backend == 'zylo.template.backends.DjangoTemplates':
+                self.template_env = Environment(
+                    loader=FileSystemLoader(dirs),
+                    autoescape=True  # Enable autoescaping for security
+                )
+            else:
+                # Handle other custom template backends if needed
+                pass
+        else:
+            self.template_env = Environment(
+                loader=FileSystemLoader(self.template_folder),
+                autoescape=True  # Enable autoescaping for security
+            )
+            
+    def set_template_folder(self):
+        dirs = self.config.get('DIRS')
+        if dirs:
+            dirs = self.template_folder = dirs[0]
+            return dirs
+
+    def update_config(self):
+        self.load_settings()
+        self.setup_template_env()
+        self.set_template_folder()
+        self.load_routes()
+
+    def add_url_rule(self, route, view_func, methods=None):
+        methods = methods or ['GET']
+        def wrapped_view_func(request, **values):
+            return view_func(request, **values)
+        self.url_map.add(Rule(route, endpoint=view_func.__name__, methods=methods))
+        setattr(self, view_func.__name__, wrapped_view_func)
 
     def route(self, rule, methods=['GET']):
         def decorator(handler):
             self.add_url_rule(rule, handler.__name__, handler, methods)
             return handler
 
         return decorator
@@ -88,14 +160,33 @@
 
     def handle_error(self, code, error, request):
         handler = self.error_handlers.get(code)
         if handler:
             return handler(error, request)
         else:
             return error
+        
+    def runserver(self, host=None, port=None, debug=None, secret_key=None):
+        self.update_config()
+        if host is not None:
+            self.host = host
+        if port is not None:
+            self.port = port
+        if debug is not None:
+            self.debug = debug
+        if secret_key is not None:
+            self.secret_key = secret_key
+
+        if self.debug:
+            app = DebuggedApplication(self, evalex=True)
+        else:
+            app = self
+
+        from werkzeug.serving import run_simple
+        run_simple(self.host, self.port, app, use_reloader=True)
 
     def wsgi_app(self, environ, start_response):
         request = Request(environ)
         for blueprint in self.blueprints:
             if request.path.startswith(blueprint.url_prefix):
                 request.blueprint = blueprint
                 response = blueprint.wsgi_app(environ, start_response)
@@ -115,85 +206,7 @@
 
     def __call__(self, environ, start_response):
         app = self.wsgi_app
         for middleware in reversed(self.middlewares):
             app = middleware(app)
         return app(environ, start_response)
 
-    def run(self, host=None, port=None, debug=None, secret_key=None):
-        if host is not None:
-            self.host = host
-        if port is not None:
-            self.port = port
-        if debug is not None:
-            self.debug = debug
-        if secret_key is not None:
-            self.secret_key = secret_key
-
-        if self.debug:
-            app = DebuggedApplication(self, evalex=True)
-        else:
-            app = self
-
-        from werkzeug.serving import run_simple
-        run_simple(self.host, self.port, app, use_reloader=True)
-
-app = Zylo()
-
-def render_template(template_name, **kwargs):
-    template = app.template_env.get_template(template_name)
-    kwargs['url_for_static'] = app.url_for_static
-    return Response(template.render(**kwargs), mimetype='text/html')
-
-def jsonify(data):
-    json_data = json.dumps(data)
-    return Response(json_data, mimetype='application/json')
-
-def redirect(location, code=302):
-    return Response('', status=code, headers={'Location': location})
-
-def url_for(endpoint, **values):
-    return app.url_map.build(endpoint, values)
-
-def send_file(filename, mimetype):
-    with open(filename, 'rb') as f:
-        content = f.read()
-    headers = {'Content-Type': mimetype, 'Content-Disposition': f'attachment; filename={os.path.basename(filename)}'}
-    return Response(content, headers=headers)
-
-def static_engine(static_folder):
-    app.wsgi_app = SharedDataMiddleware(app.wsgi_app, {'/static': static_folder})
-
-def template_engine(template_folder):
-    app.template_env = Environment(loader=FileSystemLoader(template_folder))
-
-def save_json_file(data, filename):
-    with open(filename, 'w') as f:
-        json.dump(data, f)
-
-def redirect_args(location, **kwargs):
-    url = location
-    if kwargs:
-        query_params = url_encode(kwargs)
-        url += f'?{query_params}'
-    return Response(status=302, headers={'Location': url})
-
-def send_from_directory(directory, filename, **options):
-    return send_from_directory(directory, filename, **options)
-
-def url_map(rules):
-    return Map(rules)
-
-def stream_with_context(generator_or_function):
-    return stream_with_context(generator_or_function)
-
-def make_unique_key():
-    return base64.urlsafe_b64encode(os.urandom(32)).rstrip(b'=').decode('ascii')
-
-def url_quote(url, safe='/', encoding=None, errors=None):
-    return url_quote(url, safe=safe, encoding=encoding, errors=errors)
-
-def url_quote_plus(url, safe='/', encoding=None, errors=None):
-    return url_quote_plus(url, safe=safe, encoding=encoding, errors=errors)
-
-def safe_join(directory, *pathnames):
-    return safe_join(directory, *pathnames)
```

### Comparing `zylo-2.0.3/zylo/blueprint.py` & `zylo-2.0.4/zylo/components/blueprint.py`

 * *Files identical despite different names*

### Comparing `zylo-2.0.3/zylo/chiper.py` & `zylo-2.0.4/zylo/security/chiper.py`

 * *Files identical despite different names*

### Comparing `zylo-2.0.3/zylo/mailer.py` & `zylo-2.0.4/zylo/mail/zylo_mailer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import smtplib
 from email.mime.text import MIMEText
 from email.mime.multipart import MIMEMultipart
-from .app import Response
+from ..core.branch import Response
 
 class Mailer:
     def __init__(self):
         self.config = {
             'SMTP': '',
             'SMTP_PORT': 587,
             'SENDER_EMAIL': '',
```

### Comparing `zylo-2.0.3/zylo/sessions.py` & `zylo-2.0.4/zylo/components/sessions.py`

 * *Files identical despite different names*

