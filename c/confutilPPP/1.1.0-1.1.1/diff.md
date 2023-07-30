# Comparing `tmp/confutilPPP-1.1.0.tar.gz` & `tmp/confutilPPP-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "confutilPPP-1.1.0.tar", last modified: Fri Jul 28 08:54:49 2023, max compression
+gzip compressed data, was "confutilPPP-1.1.1.tar", last modified: Sun Jul 30 11:12:15 2023, max compression
```

## Comparing `confutilPPP-1.1.0.tar` & `confutilPPP-1.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 08:54:49.796743 confutilPPP-1.1.0/
--rw-rw-rw-   0        0        0     1003 2023-07-28 08:54:49.796743 confutilPPP-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      610 2023-07-28 08:54:38.000000 confutilPPP-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-28 08:54:49.781153 confutilPPP-1.1.0/confutilPPP.egg-info/
--rw-rw-rw-   0        0        0     1003 2023-07-28 08:54:49.000000 confutilPPP-1.1.0/confutilPPP.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2023-07-28 08:54:49.000000 confutilPPP-1.1.0/confutilPPP.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 08:54:49.000000 confutilPPP-1.1.0/confutilPPP.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-07-28 08:54:49.000000 confutilPPP-1.1.0/confutilPPP.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-28 08:54:49.000000 confutilPPP-1.1.0/confutilPPP.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-28 08:54:49.796743 confutilPPP-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      814 2023-07-28 07:23:26.000000 confutilPPP-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-28 08:54:49.781153 confutilPPP-1.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-28 08:54:49.796743 confutilPPP-1.1.0/src/confutilPPP/
--rw-rw-rw-   0        0        0     2272 2023-07-28 08:51:55.000000 confutilPPP-1.1.0/src/confutilPPP/__confutil__.py
--rw-rw-rw-   0        0        0      245 2023-07-28 08:48:44.000000 confutilPPP-1.1.0/src/confutilPPP/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:12:15.659235 confutilPPP-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-07-30 11:12:15.659235 confutilPPP-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-30 11:12:03.000000 confutilPPP-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:12:15.655235 confutilPPP-1.1.1/confutilPPP.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-07-30 11:12:15.000000 confutilPPP-1.1.1/confutilPPP.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-30 11:12:15.000000 confutilPPP-1.1.1/confutilPPP.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 11:12:15.000000 confutilPPP-1.1.1/confutilPPP.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-30 11:12:15.000000 confutilPPP-1.1.1/confutilPPP.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-30 11:12:15.000000 confutilPPP-1.1.1/confutilPPP.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 11:12:15.659235 confutilPPP-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-30 11:12:03.000000 confutilPPP-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:12:15.655235 confutilPPP-1.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:12:15.655235 confutilPPP-1.1.1/src/confutilPPP/
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-07-30 11:12:03.000000 confutilPPP-1.1.1/src/confutilPPP/__confutil__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-30 11:12:03.000000 confutilPPP-1.1.1/src/confutilPPP/__init__.py
```

### Comparing `confutilPPP-1.1.0/PKG-INFO` & `confutilPPP-1.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-Metadata-Version: 2.1
-Name: confutilPPP
-Version: 1.1.0
-Summary: A simple configuration file tool
-Home-page: https://github.com/Aurorax-own/confutilPPP
-Author: Aurorax-own
-Author-email: 15047150695@163.com
-Project-URL: Source, https://github.com/Aurorax-own/confutilPPP
-Project-URL: Tracker, https://github.com/Aurorax-own/confutilPPP/issues
-Description-Content-Type: text/markdown
-
-# confutilPPP
-
-## 1.安装
-
-```
-pip install confutilPPP
-```
-
-## 2.导入并使用
-
-```
-import confutilPPP
-
-# 此项设置为 False 时，日志不会带颜色（默认为 True）
-confutilPPP.LOG_IS_COLOR = True
-
-
-def test():
-    # _object : dict, 包含配置对象
-    # _filename : str, 配置文件名 默认为 config
-    # return : dict, 配置字典
-    # 首次当前位置生成 *.yml 文件，之后直接读取
-    # *.yaml也可用
-    CONFIG = {
-        'test': 'test'
-    }
-    conf = confutilPPP.check_config(_object=CONFIG, _filename='config')
-    print(conf)
-```
-
+Metadata-Version: 2.1
+Name: confutilPPP
+Version: 1.1.1
+Summary: A simple configuration file tool
+Home-page: https://github.com/Aurorax-own/confutilPPP
+Author: Aurorax-own
+Author-email: 15047150695@163.com
+Project-URL: Source, https://github.com/Aurorax-own/confutilPPP
+Project-URL: Tracker, https://github.com/Aurorax-own/confutilPPP/issues
+Description-Content-Type: text/markdown
+
+# confutilPPP
+
+## 1.安装
+
+```
+pip install confutilPPP
+```
+
+## 2.导入并使用
+
+```
+import confutilPPP
+
+# 此项设置为 False 时，日志不会带颜色（默认为 True）
+confutilPPP.LOG_IS_COLOR = True
+
+
+def test():
+    # _object : dict, 包含配置对象
+    # _filename : str, 配置文件名 默认为 config
+    # return : dict, 配置字典
+    # 首次当前位置生成 *.yml 文件，之后直接读取
+    # *.yaml也可用
+    CONFIG = {
+        'test': 'test'
+    }
+    conf = confutilPPP.check_config(_object=CONFIG, _filename='config')
+    print(conf)
+```
+
```

### Comparing `confutilPPP-1.1.0/confutilPPP.egg-info/PKG-INFO` & `confutilPPP-1.1.1/confutilPPP.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-Metadata-Version: 2.1
-Name: confutilPPP
-Version: 1.1.0
-Summary: A simple configuration file tool
-Home-page: https://github.com/Aurorax-own/confutilPPP
-Author: Aurorax-own
-Author-email: 15047150695@163.com
-Project-URL: Source, https://github.com/Aurorax-own/confutilPPP
-Project-URL: Tracker, https://github.com/Aurorax-own/confutilPPP/issues
-Description-Content-Type: text/markdown
-
-# confutilPPP
-
-## 1.安装
-
-```
-pip install confutilPPP
-```
-
-## 2.导入并使用
-
-```
-import confutilPPP
-
-# 此项设置为 False 时，日志不会带颜色（默认为 True）
-confutilPPP.LOG_IS_COLOR = True
-
-
-def test():
-    # _object : dict, 包含配置对象
-    # _filename : str, 配置文件名 默认为 config
-    # return : dict, 配置字典
-    # 首次当前位置生成 *.yml 文件，之后直接读取
-    # *.yaml也可用
-    CONFIG = {
-        'test': 'test'
-    }
-    conf = confutilPPP.check_config(_object=CONFIG, _filename='config')
-    print(conf)
-```
-
+Metadata-Version: 2.1
+Name: confutilPPP
+Version: 1.1.1
+Summary: A simple configuration file tool
+Home-page: https://github.com/Aurorax-own/confutilPPP
+Author: Aurorax-own
+Author-email: 15047150695@163.com
+Project-URL: Source, https://github.com/Aurorax-own/confutilPPP
+Project-URL: Tracker, https://github.com/Aurorax-own/confutilPPP/issues
+Description-Content-Type: text/markdown
+
+# confutilPPP
+
+## 1.安装
+
+```
+pip install confutilPPP
+```
+
+## 2.导入并使用
+
+```
+import confutilPPP
+
+# 此项设置为 False 时，日志不会带颜色（默认为 True）
+confutilPPP.LOG_IS_COLOR = True
+
+
+def test():
+    # _object : dict, 包含配置对象
+    # _filename : str, 配置文件名 默认为 config
+    # return : dict, 配置字典
+    # 首次当前位置生成 *.yml 文件，之后直接读取
+    # *.yaml也可用
+    CONFIG = {
+        'test': 'test'
+    }
+    conf = confutilPPP.check_config(_object=CONFIG, _filename='config')
+    print(conf)
+```
+
```

### Comparing `confutilPPP-1.1.0/src/confutilPPP/__confutil__.py` & `confutilPPP-1.1.1/src/confutilPPP/__confutil__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,57 +1,60 @@
-import argparse
-import os
-
-import logPPP
-import yaml
-
-LOG_IS_COLOR = True
-
-
-class confutil:
-    def __init__(self):
-        pass
-
-    # 获取参数
-    @staticmethod
-    def _parse_arguments():
-        parser = argparse.ArgumentParser()
-        default_config_path = os.path.join(os.getcwd(), 'config.yaml')
-        parser.add_argument("--configpath", "-c", default=default_config_path, nargs=1, help="配置文件")
-        return parser.parse_args()
-
-    # 检查解析参数
-    @staticmethod
-    def check_config(_object=None, _filename='config'):
-        try:
-            # 解析参数
-            config_path = confutil._parse_arguments().configpath
-            # 如果*.yaml文件不存在或者为空
-            if not os.path.isfile(config_path) or os.path.getsize(config_path) == 0:
-                # 使用os.path模块获取文件名和文件路径
-                file_name = os.path.basename(config_path)
-                file_path = os.path.dirname(config_path)
-                # 检查文件名是否以.yaml结尾
-                if file_name.endswith('.yaml'):
-                    # 生成新的文件路径
-                    config_path = os.path.join(file_path, file_name[:-5] + '.yml')
-        except Exception:
-            logPPP.error('构建配置文件路径失败！', is_color=LOG_IS_COLOR)
-            return None
-
-        # 如果文件不存在或者为空，创建文件并写入
-        try:
-            if not os.path.isfile(config_path) or os.path.getsize(config_path) == 0:
-                with open(config_path, 'w', encoding='utf_8') as f:
-                    f.write(yaml.dump(_object, allow_unicode=True, sort_keys=False, default_flow_style=False))
-        except Exception:
-            logPPP.error('创建配置文件失败！', is_color=LOG_IS_COLOR)
-            return None
-
-        # 读取YAML文件
-        try:
-            with open(config_path, 'r', encoding='utf_8') as f:
-                logPPP.info("配置文件:", config_path, is_color=LOG_IS_COLOR)
-                return yaml.safe_load(f)
-        except Exception:
-            logPPP.error("读取配置文件失败,检查配置文件格式是否正确！", is_color=LOG_IS_COLOR)
-            return None
+import argparse
+import os
+
+import logPPP
+import yaml
+
+LOG_IS_COLOR = True
+
+
+class confutil:
+    def __init__(self):
+        pass
+
+    # 获取参数
+    @staticmethod
+    def _parse_arguments():
+        parser = argparse.ArgumentParser()
+        default_config_path = os.path.join(os.getcwd(), 'config.yaml')
+        parser.add_argument("--configpath", "-c", default=default_config_path, nargs=1, help="配置文件")
+        return parser.parse_args()
+
+    # 检查解析参数
+    @staticmethod
+    def check_config(_object=None, _filename='config'):
+        try:
+            # 解析参数
+            config_path = confutil._parse_arguments().configpath[0]
+            if not os.path.isabs(config_path):
+                config_path = os.path.abspath(config_path)
+            # 如果*.yaml文件不存在或者为空
+            if not os.path.exists(config_path) or os.path.getsize(config_path) == 0:
+                # 使用os.path模块获取文件名和文件路径
+                file_name = os.path.basename(config_path)
+                file_path = os.path.dirname(config_path)
+                # 检查文件名是否以.yaml结尾
+                if file_name.endswith('.yaml'):
+                    # 生成新的文件路径
+                    config_path = os.path.join(file_path, file_name[:-5] + '.yml')
+        except Exception:
+            logPPP.error('构建配置文件路径失败！', is_color=LOG_IS_COLOR)
+            return None
+
+        # 如果文件不存在或者为空，创建文件并写入
+        try:
+            if not os.path.exists(config_path) or os.path.getsize(config_path) == 0:
+                os.makedirs(file_path, exist_ok=True)
+                with open(config_path, 'w', encoding='utf_8') as f:
+                    f.write(yaml.dump(_object, allow_unicode=True, sort_keys=False, default_flow_style=False))
+        except Exception as e:
+            logPPP.error('创建配置文件失败！', e, is_color=LOG_IS_COLOR)
+            return None
+
+        # 读取YAML文件
+        try:
+            with open(config_path, 'r', encoding='utf_8') as f:
+                logPPP.info("配置文件:", config_path, is_color=LOG_IS_COLOR)
+                return yaml.safe_load(f)
+        except Exception:
+            logPPP.error("读取配置文件失败,检查配置文件格式是否正确！", is_color=LOG_IS_COLOR)
+            return None
```

