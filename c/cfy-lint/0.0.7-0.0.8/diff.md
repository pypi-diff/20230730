# Comparing `tmp/cfy-lint-0.0.7.tar.gz` & `tmp/cfy-lint-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cfy-lint-0.0.7.tar", last modified: Wed Sep 14 13:02:48 2022, max compression
+gzip compressed data, was "dist/cfy-lint-0.0.8.tar", last modified: Tue Sep 20 16:56:06 2022, max compression
```

## Comparing `cfy-lint-0.0.7.tar` & `cfy-lint-0.0.8.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-14 13:02:48.000000 cfy-lint-0.0.7/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-14 13:02:48.000000 cfy-lint-0.0.7/cfy_lint/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-14 13:02:48.000000 cfy-lint-0.0.7/cfy_lint/commands/
--rw-r--r--   0 root         (0) root         (0)      627 2022-09-14 13:02:26.000000 cfy-lint-0.0.7/cfy_lint/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1728 2022-09-14 13:02:26.000000 cfy-lint-0.0.7/cfy_lint/commands/lint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-14 13:02:48.000000 cfy-lint-0.0.7/cfy_lint/yamllint_ext/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-14 13:02:48.000000 cfy-lint-0.0.7/cfy_lint/yamllint_ext/cloudify/
--rw-r--r--   0 root         (0) root         (0)      668 2022-09-14 13:02:26.000000 cfy-lint-0.0.7/cfy_lint/yamllint_ext/cloudify/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6284 2022-09-14 13:02:26.000000 cfy-lint-0.0.7/cfy_lint/yamllint_ext/cloudify/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-14 13:02:48.000000 cfy-lint-0.0.7/cfy_lint/yamllint_ext/config/
--rw-r--r--   0 root         (0) root         (0)     2005 2022-09-14 13:02:26.000000 cfy-lint-0.0.7/cfy_lint/yamllint_ext/config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1764 2022-09-14 13:02:26.000000 cfy-lint-0.0.7/cfy_lint/yamllint_ext/config/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-14 13:02:48.000000 cfy-lint-0.0.7/cfy_lint/yamllint_ext/rules/
--rw-r--r--   0 root         (0) root         (0)     1320 2022-09-14 13:02:26.000000 cfy-lint-0.0.7/cfy_lint/yamllint_ext/rules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4106 2022-09-14 13:02:26.000000 cfy-lint-0.0.7/cfy_lint/yamllint_ext/rules/capabilities.py
--rw-r--r--   0 root         (0) root         (0)    25527 2022-09-14 13:02:26.000000 cfy-lint-0.0.7/cfy_lint/yamllint_ext/rules/constants.py
--rw-r--r--   0 root         (0) root         (0)     1772 2022-09-14 13:02:26.000000 cfy-lint-0.0.7/cfy_lint/yamllint_ext/rules/dsl_definitions.py
--rw-r--r--   0 root         (0) root         (0)     2093 2022-09-14 13:02:26.000000 cfy-lint-0.0.7/cfy_lint/yamllint_ext/rules/dsl_version.py
--rw-r--r--   0 root         (0) root         (0)     3314 2022-09-14 13:02:26.000000 cfy-lint-0.0.7/cfy_lint/yamllint_ext/rules/imports.py
--rw-r--r--   0 root         (0) root         (0)     5339 2022-09-14 13:02:26.000000 cfy-lint-0.0.7/cfy_lint/yamllint_ext/rules/inputs.py
--rw-r--r--   0 root         (0) root         (0)    17211 2022-09-14 13:02:26.000000 cfy-lint-0.0.7/cfy_lint/yamllint_ext/rules/node_templates.py
--rw-r--r--   0 root         (0) root         (0)     2001 2022-09-14 13:02:26.000000 cfy-lint-0.0.7/cfy_lint/yamllint_ext/rules/node_types.py
--rw-r--r--   0 root         (0) root         (0)     7813 2022-09-14 13:02:26.000000 cfy-lint-0.0.7/cfy_lint/yamllint_ext/rules/relationships.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-14 13:02:48.000000 cfy-lint-0.0.7/cfy_lint/yamllint_ext/tests/
--rw-r--r--   0 root         (0) root         (0)     1643 2022-09-14 13:02:26.000000 cfy-lint-0.0.7/cfy_lint/yamllint_ext/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1395 2022-09-14 13:02:26.000000 cfy-lint-0.0.7/cfy_lint/yamllint_ext/tests/test_generators.py
--rw-r--r--   0 root         (0) root         (0)    11881 2022-09-14 13:02:26.000000 cfy-lint-0.0.7/cfy_lint/yamllint_ext/tests/test_rules.py
--rw-r--r--   0 root         (0) root         (0)     3982 2022-09-14 13:02:26.000000 cfy-lint-0.0.7/cfy_lint/yamllint_ext/tests/test_utils.py
--rw-r--r--   0 root         (0) root         (0)     9632 2022-09-14 13:02:26.000000 cfy-lint-0.0.7/cfy_lint/yamllint_ext/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4904 2022-09-14 13:02:26.000000 cfy-lint-0.0.7/cfy_lint/yamllint_ext/constants.py
--rw-r--r--   0 root         (0) root         (0)     5886 2022-09-14 13:02:26.000000 cfy-lint-0.0.7/cfy_lint/yamllint_ext/generators.py
--rw-r--r--   0 root         (0) root         (0)     3467 2022-09-14 13:02:26.000000 cfy-lint-0.0.7/cfy_lint/yamllint_ext/overrides.py
--rw-r--r--   0 root         (0) root         (0)    15340 2022-09-14 13:02:26.000000 cfy-lint-0.0.7/cfy_lint/yamllint_ext/utils.py
--rw-r--r--   0 root         (0) root         (0)      627 2022-09-14 13:02:26.000000 cfy-lint-0.0.7/cfy_lint/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1509 2022-09-14 13:02:26.000000 cfy-lint-0.0.7/cfy_lint/cli.py
--rw-r--r--   0 root         (0) root         (0)      871 2022-09-14 13:02:26.000000 cfy-lint-0.0.7/cfy_lint/logger.py
--rw-r--r--   0 root         (0) root         (0)      700 2022-09-14 13:02:26.000000 cfy-lint-0.0.7/cfy_lint/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-14 13:02:48.000000 cfy-lint-0.0.7/cfy_lint.egg-info/
--rw-r--r--   0 root         (0) root         (0)      205 2022-09-14 13:02:48.000000 cfy-lint-0.0.7/cfy_lint.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1275 2022-09-14 13:02:48.000000 cfy-lint-0.0.7/cfy_lint.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-14 13:02:48.000000 cfy-lint-0.0.7/cfy_lint.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2022-09-14 13:02:48.000000 cfy-lint-0.0.7/cfy_lint.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       32 2022-09-14 13:02:48.000000 cfy-lint-0.0.7/cfy_lint.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2022-09-14 13:02:48.000000 cfy-lint-0.0.7/cfy_lint.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      730 2022-09-14 13:02:26.000000 cfy-lint-0.0.7/README.md
--rw-r--r--   0 root         (0) root         (0)     1044 2022-09-14 13:02:26.000000 cfy-lint-0.0.7/setup.py
--rw-r--r--   0 root         (0) root         (0)      205 2022-09-14 13:02:48.000000 cfy-lint-0.0.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2022-09-14 13:02:48.000000 cfy-lint-0.0.7/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-20 16:56:06.000000 cfy-lint-0.0.8/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-20 16:56:06.000000 cfy-lint-0.0.8/cfy_lint/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-20 16:56:06.000000 cfy-lint-0.0.8/cfy_lint/commands/
+-rw-r--r--   0 root         (0) root         (0)      627 2022-09-20 16:55:43.000000 cfy-lint-0.0.8/cfy_lint/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1728 2022-09-20 16:55:43.000000 cfy-lint-0.0.8/cfy_lint/commands/lint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-20 16:56:06.000000 cfy-lint-0.0.8/cfy_lint/yamllint_ext/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-20 16:56:06.000000 cfy-lint-0.0.8/cfy_lint/yamllint_ext/cloudify/
+-rw-r--r--   0 root         (0) root         (0)      668 2022-09-20 16:55:43.000000 cfy-lint-0.0.8/cfy_lint/yamllint_ext/cloudify/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6284 2022-09-20 16:55:43.000000 cfy-lint-0.0.8/cfy_lint/yamllint_ext/cloudify/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-20 16:56:06.000000 cfy-lint-0.0.8/cfy_lint/yamllint_ext/config/
+-rw-r--r--   0 root         (0) root         (0)     2005 2022-09-20 16:55:43.000000 cfy-lint-0.0.8/cfy_lint/yamllint_ext/config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1764 2022-09-20 16:55:43.000000 cfy-lint-0.0.8/cfy_lint/yamllint_ext/config/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-20 16:56:06.000000 cfy-lint-0.0.8/cfy_lint/yamllint_ext/rules/
+-rw-r--r--   0 root         (0) root         (0)     1320 2022-09-20 16:55:43.000000 cfy-lint-0.0.8/cfy_lint/yamllint_ext/rules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4194 2022-09-20 16:55:43.000000 cfy-lint-0.0.8/cfy_lint/yamllint_ext/rules/capabilities.py
+-rw-r--r--   0 root         (0) root         (0)    25527 2022-09-20 16:55:43.000000 cfy-lint-0.0.8/cfy_lint/yamllint_ext/rules/constants.py
+-rw-r--r--   0 root         (0) root         (0)     1772 2022-09-20 16:55:43.000000 cfy-lint-0.0.8/cfy_lint/yamllint_ext/rules/dsl_definitions.py
+-rw-r--r--   0 root         (0) root         (0)     2093 2022-09-20 16:55:43.000000 cfy-lint-0.0.8/cfy_lint/yamllint_ext/rules/dsl_version.py
+-rw-r--r--   0 root         (0) root         (0)     3314 2022-09-20 16:55:43.000000 cfy-lint-0.0.8/cfy_lint/yamllint_ext/rules/imports.py
+-rw-r--r--   0 root         (0) root         (0)     5585 2022-09-20 16:55:43.000000 cfy-lint-0.0.8/cfy_lint/yamllint_ext/rules/inputs.py
+-rw-r--r--   0 root         (0) root         (0)    17211 2022-09-20 16:55:43.000000 cfy-lint-0.0.8/cfy_lint/yamllint_ext/rules/node_templates.py
+-rw-r--r--   0 root         (0) root         (0)     2001 2022-09-20 16:55:43.000000 cfy-lint-0.0.8/cfy_lint/yamllint_ext/rules/node_types.py
+-rw-r--r--   0 root         (0) root         (0)     7813 2022-09-20 16:55:43.000000 cfy-lint-0.0.8/cfy_lint/yamllint_ext/rules/relationships.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-20 16:56:06.000000 cfy-lint-0.0.8/cfy_lint/yamllint_ext/tests/
+-rw-r--r--   0 root         (0) root         (0)     1643 2022-09-20 16:55:43.000000 cfy-lint-0.0.8/cfy_lint/yamllint_ext/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1395 2022-09-20 16:55:43.000000 cfy-lint-0.0.8/cfy_lint/yamllint_ext/tests/test_generators.py
+-rw-r--r--   0 root         (0) root         (0)    11881 2022-09-20 16:55:43.000000 cfy-lint-0.0.8/cfy_lint/yamllint_ext/tests/test_rules.py
+-rw-r--r--   0 root         (0) root         (0)     3982 2022-09-20 16:55:43.000000 cfy-lint-0.0.8/cfy_lint/yamllint_ext/tests/test_utils.py
+-rw-r--r--   0 root         (0) root         (0)     9632 2022-09-20 16:55:43.000000 cfy-lint-0.0.8/cfy_lint/yamllint_ext/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4904 2022-09-20 16:55:43.000000 cfy-lint-0.0.8/cfy_lint/yamllint_ext/constants.py
+-rw-r--r--   0 root         (0) root         (0)     5886 2022-09-20 16:55:43.000000 cfy-lint-0.0.8/cfy_lint/yamllint_ext/generators.py
+-rw-r--r--   0 root         (0) root         (0)     3467 2022-09-20 16:55:43.000000 cfy-lint-0.0.8/cfy_lint/yamllint_ext/overrides.py
+-rw-r--r--   0 root         (0) root         (0)    15339 2022-09-20 16:55:43.000000 cfy-lint-0.0.8/cfy_lint/yamllint_ext/utils.py
+-rw-r--r--   0 root         (0) root         (0)      627 2022-09-20 16:55:43.000000 cfy-lint-0.0.8/cfy_lint/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1509 2022-09-20 16:55:43.000000 cfy-lint-0.0.8/cfy_lint/cli.py
+-rw-r--r--   0 root         (0) root         (0)      871 2022-09-20 16:55:43.000000 cfy-lint-0.0.8/cfy_lint/logger.py
+-rw-r--r--   0 root         (0) root         (0)      700 2022-09-20 16:55:43.000000 cfy-lint-0.0.8/cfy_lint/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-20 16:56:06.000000 cfy-lint-0.0.8/cfy_lint.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      205 2022-09-20 16:56:06.000000 cfy-lint-0.0.8/cfy_lint.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1275 2022-09-20 16:56:06.000000 cfy-lint-0.0.8/cfy_lint.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-20 16:56:06.000000 cfy-lint-0.0.8/cfy_lint.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2022-09-20 16:56:06.000000 cfy-lint-0.0.8/cfy_lint.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2022-09-20 16:56:06.000000 cfy-lint-0.0.8/cfy_lint.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2022-09-20 16:56:06.000000 cfy-lint-0.0.8/cfy_lint.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      730 2022-09-20 16:55:43.000000 cfy-lint-0.0.8/README.md
+-rw-r--r--   0 root         (0) root         (0)     1044 2022-09-20 16:55:43.000000 cfy-lint-0.0.8/setup.py
+-rw-r--r--   0 root         (0) root         (0)      205 2022-09-20 16:56:06.000000 cfy-lint-0.0.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-20 16:56:06.000000 cfy-lint-0.0.8/setup.cfg
```

### Comparing `cfy-lint-0.0.7/cfy_lint/commands/__init__.py` & `cfy-lint-0.0.8/cfy_lint/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `cfy-lint-0.0.7/cfy_lint/commands/lint.py` & `cfy-lint-0.0.8/cfy_lint/commands/lint.py`

 * *Files identical despite different names*

### Comparing `cfy-lint-0.0.7/cfy_lint/yamllint_ext/cloudify/__init__.py` & `cfy-lint-0.0.8/cfy_lint/yamllint_ext/cloudify/__init__.py`

 * *Files identical despite different names*

### Comparing `cfy-lint-0.0.7/cfy_lint/yamllint_ext/cloudify/models.py` & `cfy-lint-0.0.8/cfy_lint/yamllint_ext/cloudify/models.py`

 * *Files identical despite different names*

### Comparing `cfy-lint-0.0.7/cfy_lint/yamllint_ext/config/__init__.py` & `cfy-lint-0.0.8/cfy_lint/yamllint_ext/config/__init__.py`

 * *Files identical despite different names*

### Comparing `cfy-lint-0.0.7/cfy_lint/yamllint_ext/config/constants.py` & `cfy-lint-0.0.8/cfy_lint/yamllint_ext/config/constants.py`

 * *Files identical despite different names*

### Comparing `cfy-lint-0.0.7/cfy_lint/yamllint_ext/rules/__init__.py` & `cfy-lint-0.0.8/cfy_lint/yamllint_ext/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `cfy-lint-0.0.7/cfy_lint/yamllint_ext/rules/capabilities.py` & `cfy-lint-0.0.8/cfy_lint/yamllint_ext/rules/capabilities.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,14 +32,16 @@
     for item in token.node.value:
         if token.prev.node.value == 'outputs':
             output_obj = CfyOutput(item)
             if not output_obj.name and not output_obj.mapping:
                 continue
         elif token.prev.node.value == 'capabilities':
             output_obj = CfyCapability(item)
+            if not output_obj.name and not output_obj.mapping:
+                continue
         if output_obj.not_output():
             continue
         if isinstance(output_obj, CfyOutput):
             ctx['outputs'].update(output_obj.__dict__())
         else:
             ctx['capabilities'].update(output_obj.__dict__())
         desig = 'output' if token.prev.node.value == 'outputs' \
```

### Comparing `cfy-lint-0.0.7/cfy_lint/yamllint_ext/rules/constants.py` & `cfy-lint-0.0.8/cfy_lint/yamllint_ext/rules/constants.py`

 * *Files identical despite different names*

### Comparing `cfy-lint-0.0.7/cfy_lint/yamllint_ext/rules/dsl_definitions.py` & `cfy-lint-0.0.8/cfy_lint/yamllint_ext/rules/dsl_definitions.py`

 * *Files identical despite different names*

### Comparing `cfy-lint-0.0.7/cfy_lint/yamllint_ext/rules/dsl_version.py` & `cfy-lint-0.0.8/cfy_lint/yamllint_ext/rules/dsl_version.py`

 * *Files identical despite different names*

### Comparing `cfy-lint-0.0.7/cfy_lint/yamllint_ext/rules/imports.py` & `cfy-lint-0.0.8/cfy_lint/yamllint_ext/rules/imports.py`

 * *Files identical despite different names*

### Comparing `cfy-lint-0.0.7/cfy_lint/yamllint_ext/rules/inputs.py` & `cfy-lint-0.0.8/cfy_lint/yamllint_ext/rules/inputs.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,14 +31,16 @@
 
 
 @process_relevant_tokens(CfyNode, ['inputs', 'get_input'])
 def check(token=None, **_):
     if token.prev.node.value == 'inputs':
         for item in token.node.value:
             input_obj = CfyInput(item)
+            if not input_obj.name and not input_obj.mapping:
+                continue
             if input_obj.not_input():
                 continue
             ctx['inputs'].update(input_obj.__dict__())
             yield from validate_inputs(input_obj, input_obj.line or token.line)
 
     if token.prev.node.value == 'get_input':
         if isinstance(token.node.value, list):
@@ -82,21 +84,25 @@
         yield LintProblem(line, None, message)
 
 
 class CfyInput(object):
     def __init__(self, nodes):
         self._line = None
         self.name, self.mapping = self.get_input(nodes)
-        for key in list(self.mapping.keys()):
-            if key not in ['type', 'default', 'description', 'constraints']:
-                del self.mapping[key]
-        self.input_type = self.mapping.get('type')
-        self.description = self.mapping.get('description')
-        self._default = self.mapping.get('default')
-        self.constraints = self.mapping.get('constraints')
+        if self.name and self.mapping:
+            for key in list(self.mapping.keys()):
+                if key not in ['type',
+                               'default',
+                               'description',
+                               'constraints']:
+                    del self.mapping[key]
+            self.input_type = self.mapping.get('type')
+            self.description = self.mapping.get('description')
+            self._default = self.mapping.get('default')
+            self.constraints = self.mapping.get('constraints')
 
     @property
     def default(self):
         return self._default
 
     @default.setter
     def default(self, value):
```

### Comparing `cfy-lint-0.0.7/cfy_lint/yamllint_ext/rules/node_templates.py` & `cfy-lint-0.0.8/cfy_lint/yamllint_ext/rules/node_templates.py`

 * *Files identical despite different names*

### Comparing `cfy-lint-0.0.7/cfy_lint/yamllint_ext/rules/node_types.py` & `cfy-lint-0.0.8/cfy_lint/yamllint_ext/rules/node_types.py`

 * *Files identical despite different names*

### Comparing `cfy-lint-0.0.7/cfy_lint/yamllint_ext/rules/relationships.py` & `cfy-lint-0.0.8/cfy_lint/yamllint_ext/rules/relationships.py`

 * *Files identical despite different names*

### Comparing `cfy-lint-0.0.7/cfy_lint/yamllint_ext/tests/__init__.py` & `cfy-lint-0.0.8/cfy_lint/yamllint_ext/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cfy-lint-0.0.7/cfy_lint/yamllint_ext/tests/test_generators.py` & `cfy-lint-0.0.8/cfy_lint/yamllint_ext/tests/test_generators.py`

 * *Files identical despite different names*

### Comparing `cfy-lint-0.0.7/cfy_lint/yamllint_ext/tests/test_rules.py` & `cfy-lint-0.0.8/cfy_lint/yamllint_ext/tests/test_rules.py`

 * *Files identical despite different names*

### Comparing `cfy-lint-0.0.7/cfy_lint/yamllint_ext/tests/test_utils.py` & `cfy-lint-0.0.8/cfy_lint/yamllint_ext/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `cfy-lint-0.0.7/cfy_lint/yamllint_ext/__init__.py` & `cfy-lint-0.0.8/cfy_lint/yamllint_ext/__init__.py`

 * *Files identical despite different names*

### Comparing `cfy-lint-0.0.7/cfy_lint/yamllint_ext/constants.py` & `cfy-lint-0.0.8/cfy_lint/yamllint_ext/constants.py`

 * *Files identical despite different names*

### Comparing `cfy-lint-0.0.7/cfy_lint/yamllint_ext/generators.py` & `cfy-lint-0.0.8/cfy_lint/yamllint_ext/generators.py`

 * *Files identical despite different names*

### Comparing `cfy-lint-0.0.7/cfy_lint/yamllint_ext/overrides.py` & `cfy-lint-0.0.8/cfy_lint/yamllint_ext/overrides.py`

 * *Files identical despite different names*

### Comparing `cfy-lint-0.0.7/cfy_lint/yamllint_ext/utils.py` & `cfy-lint-0.0.8/cfy_lint/yamllint_ext/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -285,15 +285,14 @@
         page = urllib.request.Request(import_item,
                                       headers={'User-Agent': 'Mozilla/5.0'})
         infile = urllib.request.urlopen(page).read()
         result = yaml.safe_load(infile)
     elif import_item == 'cloudify/types/types.yaml':
         result = DEFAULT_TYPES
     elif base_path and os.path.exists(os.path.join(base_path, import_item)):
-
         with open(os.path.join(base_path, import_item), 'r') as stream:
             result = yaml.safe_load(stream)
     elif os.path.exists(import_item):
         with open(import_item, 'r') as stream:
             result = yaml.safe_load(stream)
     result = result or {}
     for k in result.keys():
```

### Comparing `cfy-lint-0.0.7/cfy_lint/__init__.py` & `cfy-lint-0.0.8/cfy_lint/__init__.py`

 * *Files identical despite different names*

### Comparing `cfy-lint-0.0.7/cfy_lint/cli.py` & `cfy-lint-0.0.8/cfy_lint/cli.py`

 * *Files identical despite different names*

### Comparing `cfy-lint-0.0.7/cfy_lint/logger.py` & `cfy-lint-0.0.8/cfy_lint/logger.py`

 * *Files identical despite different names*

### Comparing `cfy-lint-0.0.7/cfy_lint/main.py` & `cfy-lint-0.0.8/cfy_lint/main.py`

 * *Files identical despite different names*

### Comparing `cfy-lint-0.0.7/cfy_lint.egg-info/SOURCES.txt` & `cfy-lint-0.0.8/cfy_lint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cfy-lint-0.0.7/README.md` & `cfy-lint-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `cfy-lint-0.0.7/setup.py` & `cfy-lint-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from setuptools import (setup, find_packages)
 
 setup(
     name='cfy-lint',
-    version='0.0.7',
+    version='0.0.8',
     license='LICENSE',
     packages=find_packages(),
     description='Linter for Cloudify Blueprints',
     entry_points={
         "console_scripts": [
             "cfy-lint = cfy_lint.main:lint",
         ]
```

