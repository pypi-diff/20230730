# Comparing `tmp/eo_styleguide-0.0.1a3.tar.gz` & `tmp/eo_styleguide-0.0.1a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eo_styleguide-0.0.1a3.tar", max compression
+gzip compressed data, was "eo_styleguide-0.0.1a4.tar", max compression
```

## Comparing `eo_styleguide-0.0.1a3.tar` & `eo_styleguide-0.0.1a4.tar`

### file list

```diff
@@ -1,18 +1,20 @@
--rw-r--r--   0        0        0     3421 2023-07-29 13:16:52.754001 eo_styleguide-0.0.1a3/README.md
--rw-r--r--   0        0        0     1291 2023-07-29 05:28:56.221950 eo_styleguide-0.0.1a3/pyeo/__init__.py
--rw-r--r--   0        0        0     1118 2023-07-23 13:29:32.046205 eo_styleguide-0.0.1a3/pyeo/features/__init__.py
--rw-r--r--   0        0        0     1307 2023-07-23 13:29:32.046339 eo_styleguide-0.0.1a3/pyeo/features/feature.py
--rw-r--r--   0        0        0     1553 2023-07-23 14:12:32.395680 eo_styleguide-0.0.1a3/pyeo/features/final_object.py
--rw-r--r--   0        0        0     2724 2023-07-29 05:28:56.222285 eo_styleguide-0.0.1a3/pyeo/features/method_has_protocol.py
--rw-r--r--   0        0        0     2639 2023-07-29 05:28:56.222616 eo_styleguide-0.0.1a3/pyeo/features/no_code_in_ctors.py
--rw-r--r--   0        0        0     1739 2023-07-25 19:51:55.626481 eo_styleguide-0.0.1a3/pyeo/features/no_er_names.py
--rw-r--r--   0        0        0     1711 2023-07-26 11:22:26.628858 eo_styleguide-0.0.1a3/pyeo/features/no_property_methods.py
--rw-r--r--   0        0        0     2495 2023-07-29 13:16:52.754226 eo_styleguide-0.0.1a3/pyeo/features/no_reflection.py
--rw-r--r--   0        0        0     1977 2023-07-29 05:28:56.222831 eo_styleguide-0.0.1a3/pyeo/features/no_setters.py
--rw-r--r--   0        0        0     1729 2023-07-29 11:19:51.010786 eo_styleguide-0.0.1a3/pyeo/features/no_staticmethods.py
--rw-r--r--   0        0        0     1768 2023-07-23 13:29:32.046560 eo_styleguide-0.0.1a3/pyeo/features/object_has_protocol.py
--rw-r--r--   0        0        0     2092 2023-07-26 10:49:44.099286 eo_styleguide-0.0.1a3/pyeo/features/protocol_method_code_free.py
--rw-r--r--   0        0        0     3089 2023-07-29 13:16:52.754447 eo_styleguide-0.0.1a3/pyeo/main.py
--rw-r--r--   0        0        0        0 2023-07-21 21:17:44.927051 eo_styleguide-0.0.1a3/pyeo/py.typed
--rw-r--r--   0        0        0      813 2023-07-29 13:17:17.336205 eo_styleguide-0.0.1a3/pyproject.toml
--rw-r--r--   0        0        0     4312 1970-01-01 00:00:00.000000 eo_styleguide-0.0.1a3/PKG-INFO
+-rw-r--r--   0        0        0     3421 2023-07-29 14:37:37.987684 eo_styleguide-0.0.1a4/README.md
+-rw-r--r--   0        0        0     1291 2023-07-29 05:28:56.221950 eo_styleguide-0.0.1a4/pyeo/__init__.py
+-rw-r--r--   0        0        0     1118 2023-07-23 13:29:32.046205 eo_styleguide-0.0.1a4/pyeo/features/__init__.py
+-rw-r--r--   0        0        0     1307 2023-07-23 13:29:32.046339 eo_styleguide-0.0.1a4/pyeo/features/feature.py
+-rw-r--r--   0        0        0     1620 2023-07-29 22:13:02.772938 eo_styleguide-0.0.1a4/pyeo/features/final_object.py
+-rw-r--r--   0        0        0     2810 2023-07-29 22:13:02.773315 eo_styleguide-0.0.1a4/pyeo/features/method_has_protocol.py
+-rw-r--r--   0        0        0     2881 2023-07-29 22:13:02.773905 eo_styleguide-0.0.1a4/pyeo/features/no_code_in_ctors.py
+-rw-r--r--   0        0        0     1739 2023-07-25 19:51:55.626481 eo_styleguide-0.0.1a4/pyeo/features/no_er_names.py
+-rw-r--r--   0        0        0     1715 2023-07-29 22:13:02.774156 eo_styleguide-0.0.1a4/pyeo/features/no_property_methods.py
+-rw-r--r--   0        0        0     2495 2023-07-29 13:16:52.754226 eo_styleguide-0.0.1a4/pyeo/features/no_reflection.py
+-rw-r--r--   0        0        0     1977 2023-07-29 05:28:56.222831 eo_styleguide-0.0.1a4/pyeo/features/no_setters.py
+-rw-r--r--   0        0        0     1794 2023-07-29 22:13:02.774412 eo_styleguide-0.0.1a4/pyeo/features/no_staticmethods.py
+-rw-r--r--   0        0        0     1768 2023-07-23 13:29:32.046560 eo_styleguide-0.0.1a4/pyeo/features/object_has_protocol.py
+-rw-r--r--   0        0        0     2128 2023-07-29 22:13:02.774645 eo_styleguide-0.0.1a4/pyeo/features/protocol_method_code_free.py
+-rw-r--r--   0        0        0     3508 2023-07-29 22:13:02.774877 eo_styleguide-0.0.1a4/pyeo/main.py
+-rw-r--r--   0        0        0        0 2023-07-21 21:17:44.927051 eo_styleguide-0.0.1a4/pyeo/py.typed
+-rw-r--r--   0        0        0        0 2023-07-29 22:13:02.774933 eo_styleguide-0.0.1a4/pyeo/utils/__init__.py
+-rw-r--r--   0        0        0      268 2023-07-29 22:13:02.775282 eo_styleguide-0.0.1a4/pyeo/utils/decorator_name.py
+-rw-r--r--   0        0        0      813 2023-07-29 22:13:14.421256 eo_styleguide-0.0.1a4/pyproject.toml
+-rw-r--r--   0        0        0     4312 1970-01-01 00:00:00.000000 eo_styleguide-0.0.1a4/PKG-INFO
```

### Comparing `eo_styleguide-0.0.1a3/README.md` & `eo_styleguide-0.0.1a4/README.md`

 * *Files identical despite different names*

### Comparing `eo_styleguide-0.0.1a3/pyeo/__init__.py` & `eo_styleguide-0.0.1a4/pyeo/__init__.py`

 * *Files identical despite different names*

### Comparing `eo_styleguide-0.0.1a3/pyeo/features/__init__.py` & `eo_styleguide-0.0.1a4/pyeo/features/__init__.py`

 * *Files identical despite different names*

### Comparing `eo_styleguide-0.0.1a3/pyeo/features/feature.py` & `eo_styleguide-0.0.1a4/pyeo/features/feature.py`

 * *Files identical despite different names*

### Comparing `eo_styleguide-0.0.1a3/pyeo/features/final_object.py` & `eo_styleguide-0.0.1a4/pyeo/features/final_object.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,22 +16,23 @@
 EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
 MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
 IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
 DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
 OR OTHER DEALINGS IN THE SOFTWARE.
 """
+from mypy.nodes import NameExpr
 
 
 class FinalClassFeature(object):
     """Checking each object method has protocol."""
 
     def analyze(self, ctx) -> bool:
         """Analyzing.
 
         :param ctx: mypy context
         :return: bool
         """
-        if 'typing.final' not in {decorator.fullname for decorator in ctx.cls.decorators}:
+        if 'typing.final' not in {decorator.fullname for decorator in ctx.cls.decorators if isinstance(decorator, NameExpr)}:
             ctx.api.fail("Class '{0}' must be final.".format(ctx.cls.name), ctx.cls)
             return False
         return True
```

### Comparing `eo_styleguide-0.0.1a3/pyeo/features/method_has_protocol.py` & `eo_styleguide-0.0.1a4/pyeo/features/method_has_protocol.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,38 +16,39 @@
 EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
 MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
 IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
 DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
 OR OTHER DEALINGS IN THE SOFTWARE.
 """
-from mypy.nodes import Decorator
+from mypy.nodes import Decorator, FuncDef
 
 
 class EachMethodHasProtocolFeature(object):
     """Checking each object method has protocol."""
 
     def analyze(self, ctx) -> bool:
         """Analyzing.
 
         :param ctx: mypy context
         :return: bool
         """
         object_methods = {
             def_body.name: def_body
             for def_body in ctx.cls.defs.body
-            if not def_body.name.startswith('_') and not self._method_is_ctor(def_body)
+            if isinstance(def_body, FuncDef) and not def_body.name.startswith('_') and not self._method_is_ctor(def_body)
         }
         if not ctx.cls.base_type_exprs:
             return False
         extra_method_names = set(object_methods.keys()) - {  # noqa: WPS224 need a refactor
             method.name
             for base_type in ctx.cls.base_type_exprs
             for node in base_type.node.mro
             for method in node.defn.defs.body
+            if isinstance(method, FuncDef)
         }
         if extra_method_names:
             failed_methods = [
                 method
                 for method_name, method in object_methods.items()
                 if method_name in extra_method_names
             ]
```

### Comparing `eo_styleguide-0.0.1a3/pyeo/features/no_code_in_ctors.py` & `eo_styleguide-0.0.1a4/pyeo/features/no_code_in_ctors.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,29 +16,33 @@
 EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
 MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
 IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
 DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
 OR OTHER DEALINGS IN THE SOFTWARE.
 """
-from mypy.nodes import AssignmentStmt, Decorator, ReturnStmt
+from mypy.nodes import AssignmentStmt, Block, Decorator, FuncDef, NameExpr, PassStmt, ReturnStmt
+
+from pyeo.utils.decorator_name import decorator_name
 
 
 class NoCodeInCtorFeature(object):
     """Checking each object method has protocol."""
 
     def analyze(self, ctx) -> bool:
         """Analyzing.
 
         :param ctx: mypy context
         :return: bool
         """
         for func in ctx.cls.defs.body:
-            if isinstance(func, Decorator) and 'classmethod' in {dec.name for dec in func.original_decorators}:
+            if isinstance(func, Decorator) and 'classmethod' in {decorator_name(dec) for dec in func.original_decorators}:
                 self._secondary_ctor_check(ctx, func)
+            elif not isinstance(func, FuncDef):
+                continue
             elif func.name == '__init__':
                 self._primary_ctor_check(ctx, func)
         return True
 
     def _secondary_ctor_check(self, ctx, func):
         for elem in func.func.body.body:
             # TODO: ReturnStmt can contain logic like list comprehension
@@ -53,12 +57,14 @@
                 ctx.api.fail(
                     'Find code in ctor {0}.{1}.'.format(ctx.cls.name, func.name),
                     ctx.cls,
                 )
 
     def _primary_ctor_check(self, ctx, func):
         for elem in func.body.body:
+            if isinstance(elem, PassStmt):
+                continue
             if not isinstance(elem, AssignmentStmt):
                 ctx.api.fail(
                     'Find code in ctor {0}.{1}.'.format(ctx.cls.name, func.name),
                     ctx.cls,
                 )
```

### Comparing `eo_styleguide-0.0.1a3/pyeo/features/no_er_names.py` & `eo_styleguide-0.0.1a4/pyeo/features/no_er_names.py`

 * *Files identical despite different names*

### Comparing `eo_styleguide-0.0.1a3/pyeo/features/no_property_methods.py` & `eo_styleguide-0.0.1a4/pyeo/features/no_property_methods.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,11 +29,11 @@
     def analyze(self, ctx) -> bool:  # noqa: WPS231 need in refactor
         """Analyzing.
 
         :param ctx: mypy context
         :return: bool
         """
         for body_item in ctx.cls.defs.body:
-            fail_args = ("Class '{0}' has property method: '{1}'".format(ctx.cls.name, body_item.name), ctx.cls)
             if isinstance(body_item, Decorator) and body_item.func.is_property:
+                fail_args = ("Class '{0}' has property method: '{1}'".format(ctx.cls.name, body_item.name), ctx.cls)
                 ctx.api.fail(*fail_args)
         return True
```

### Comparing `eo_styleguide-0.0.1a3/pyeo/features/no_reflection.py` & `eo_styleguide-0.0.1a4/pyeo/features/no_reflection.py`

 * *Files identical despite different names*

### Comparing `eo_styleguide-0.0.1a3/pyeo/features/no_setters.py` & `eo_styleguide-0.0.1a4/pyeo/features/no_setters.py`

 * *Files identical despite different names*

### Comparing `eo_styleguide-0.0.1a3/pyeo/features/no_staticmethods.py` & `eo_styleguide-0.0.1a4/pyeo/features/no_staticmethods.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,24 +18,26 @@
 IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
 DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
 OR OTHER DEALINGS IN THE SOFTWARE.
 """
 from mypy.nodes import AssignmentStmt, Decorator, ReturnStmt
 
+from pyeo.utils.decorator_name import decorator_name
+
 
 class NoStaticmethodsFeature(object):
     """Checking each object method has protocol."""
 
     def analyze(self, ctx) -> bool:
         """Analyzing.
 
         :param ctx: mypy context
         :return: bool
         """
         for func in ctx.cls.defs.body:
-            if isinstance(func, Decorator) and 'staticmethod' in {dec.name for dec in func.original_decorators}:
+            if isinstance(func, Decorator) and 'staticmethod' in {decorator_name(dec) for dec in func.original_decorators}:
                 ctx.api.fail(
                     'Find staticmethod {0}.{1}.'.format(ctx.cls.name, func.name),
                     ctx.cls,
                 )
         return True
```

### Comparing `eo_styleguide-0.0.1a3/pyeo/features/object_has_protocol.py` & `eo_styleguide-0.0.1a4/pyeo/features/object_has_protocol.py`

 * *Files identical despite different names*

### Comparing `eo_styleguide-0.0.1a3/pyeo/features/protocol_method_code_free.py` & `eo_styleguide-0.0.1a4/pyeo/features/protocol_method_code_free.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,31 +16,31 @@
 EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
 MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
 IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
 DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
 OR OTHER DEALINGS IN THE SOFTWARE.
 """
-from mypy.nodes import EllipsisExpr, FuncDef, PassStmt, StrExpr
+from mypy.nodes import AssignmentStmt, EllipsisExpr, ExpressionStmt, FuncDef, PassStmt, StrExpr
 
 
 class ProtocolMethodCodeFreeFeature(object):
     """Check protocol methods code free."""
 
     def analyze(self, ctx) -> bool:  # noqa: WPS231 need in refactor
         """Analyzing.
 
         :param ctx: mypy context
         :return: bool
         """
         for method in ctx.cls.defs.body:
-            fail_args = ("Protocol '{0}' method '{1}' has implementation".format(ctx.cls.name, method.name), ctx.cls)
             if not isinstance(method, FuncDef):
                 continue
             for body_item in method.body.body:
+                fail_args = ("Protocol '{0}' method '{1}' has implementation".format(ctx.cls.name, method.name), ctx.cls)
                 if isinstance(body_item, PassStmt):
                     continue
                 if not hasattr(body_item, 'expr'):  # noqa: WPS421 need in refactor
                     ctx.api.fail(*fail_args)
                     continue
                 if not isinstance(body_item.expr, (EllipsisExpr, StrExpr)):
                     ctx.api.fail(*fail_args)
```

### Comparing `eo_styleguide-0.0.1a3/pyeo/main.py` & `eo_styleguide-0.0.1a4/pyeo/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,35 +16,49 @@
 EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
 MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
 IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
 DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
 OR OTHER DEALINGS IN THE SOFTWARE.
 """
+from mypy.nodes import IndexExpr
 from mypy.plugin import Plugin
 
 from pyeo.features.final_object import FinalClassFeature
 from pyeo.features.method_has_protocol import EachMethodHasProtocolFeature
 from pyeo.features.no_code_in_ctors import NoCodeInCtorFeature
 from pyeo.features.no_er_names import NoErNamesFeature
 from pyeo.features.no_property_methods import NoPropertyMethodsFeature
 from pyeo.features.no_reflection import NoReflectionFeature
 from pyeo.features.no_setters import NoSettersFeature
 from pyeo.features.no_staticmethods import NoStaticmethodsFeature
 from pyeo.features.object_has_protocol import ObjectHasProtocolFeature
 from pyeo.features.protocol_method_code_free import ProtocolMethodCodeFreeFeature
 
 
+def _is_protocl(cls):
+    if not cls.removed_base_type_exprs:
+        return False
+    if isinstance(cls.removed_base_type_exprs[0], IndexExpr):
+        return cls.removed_base_type_exprs[0].base.fullname == 'typing.Protocol'
+    return cls.removed_base_type_exprs[0].fullname == 'typing.Protocol'
+
+
 def analyze(ctx):
     """Features controller.
 
     :param ctx: mypy context
     :return: bool
     """
-    if ctx.cls.removed_base_type_exprs and ctx.cls.removed_base_type_exprs[0].fullname == 'typing.Protocol':
+    # print(ctx.cls.fullname)
+    # # print(ctx.cls.removed_base_type_exprs)
+    # for x in ctx.cls.removed_base_type_exprs:
+    #     print(x)
+    # print('\n' * 3)
+    if _is_protocl(ctx.cls):
         NoPropertyMethodsFeature().analyze(ctx)
         ProtocolMethodCodeFreeFeature().analyze(ctx)
         NoSettersFeature().analyze(ctx)
         NoStaticmethodsFeature().analyze(ctx)
         return True
     if not ObjectHasProtocolFeature().analyze(ctx):
         return True
```

### Comparing `eo_styleguide-0.0.1a3/pyproject.toml` & `eo_styleguide-0.0.1a4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "eo-styleguide"
 packages = [
     {include = "pyeo"}
 ]
-version = "0.0.1-alpha3"
+version = "0.0.1-alpha4"
 description = "Pyeo is an advanced static analysis tool tailored specifically to enforce the principles advocated by Elegant Objects (elegantobjects.org) in Python projects. It serves as a quality control instrument to ensure that your Python code adheres to the core tenets of elegance, simplicity, and maintainability."
 authors = ["Almaz Ilaletdinov <a.ilaletdinov@yandex.ru>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
```

### Comparing `eo_styleguide-0.0.1a3/PKG-INFO` & `eo_styleguide-0.0.1a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eo-styleguide
-Version: 0.0.1a3
+Version: 0.0.1a4
 Summary: Pyeo is an advanced static analysis tool tailored specifically to enforce the principles advocated by Elegant Objects (elegantobjects.org) in Python projects. It serves as a quality control instrument to ensure that your Python code adheres to the core tenets of elegance, simplicity, and maintainability.
 License: MIT
 Author: Almaz Ilaletdinov
 Author-email: a.ilaletdinov@yandex.ru
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

