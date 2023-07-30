# Comparing `tmp/zood-0.8.1.tar.gz` & `tmp/zood-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zood-0.8.1.tar", max compression
+gzip compressed data, was "zood-0.8.2.tar", max compression
```

## Comparing `zood-0.8.1.tar` & `zood-0.8.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0      566 2023-07-30 03:45:14.060768 zood-0.8.1/pyproject.toml
--rw-r--r--   0        0        0      657 2023-07-28 05:47:50.290823 zood-0.8.1/README.md
--rw-r--r--   0        0        0       24 2023-01-06 12:50:33.818825 zood-0.8.1/zood/__init__.py
--rw-r--r--   0        0        0     4975 2023-07-30 02:58:53.277878 zood-0.8.1/zood/config/_config.yml
--rw-r--r--   0        0        0      209 2022-12-30 16:25:34.984515 zood-0.8.1/zood/config/img/after_copy.png
--rw-r--r--   0        0        0      215 2022-12-30 15:33:16.742079 zood-0.8.1/zood/config/img/before_copy.png
--rw-r--r--   0        0        0     2720 2023-01-14 08:58:35.867485 zood-0.8.1/zood/config/img/enter.png
--rw-r--r--   0        0        0      247 2023-01-14 09:31:22.970712 zood-0.8.1/zood/config/img/enter.svg
--rw-r--r--   0        0        0      454 2022-12-30 16:25:01.986421 zood-0.8.1/zood/config/img/moon.png
--rw-r--r--   0        0        0      446 2023-01-13 11:27:05.445651 zood-0.8.1/zood/config/img/search.svg
--rw-r--r--   0        0        0      428 2022-12-30 16:24:58.219147 zood-0.8.1/zood/config/img/sun.png
--rw-r--r--   0        0        0    14998 2023-07-30 03:04:00.968032 zood-0.8.1/zood/config/index.css
--rw-r--r--   0        0        0     3991 2023-07-13 02:52:54.473602 zood-0.8.1/zood/config/js/change_mode.js
--rw-r--r--   0        0        0     2646 2023-07-28 00:49:18.358387 zood-0.8.1/zood/config/js/copy_code.js
--rw-r--r--   0        0        0     1251 2023-07-28 01:20:50.114459 zood-0.8.1/zood/config/js/global_js_configuration.js
--rw-r--r--   0        0        0     2154 2023-07-13 02:53:27.953277 zood-0.8.1/zood/config/js/navigator.js
--rw-r--r--   0        0        0     1000 2023-01-01 02:18:50.438286 zood-0.8.1/zood/config/js/next_front.js
--rw-r--r--   0        0        0     1064 2023-01-02 14:54:02.515677 zood-0.8.1/zood/config/js/picture_preview.js
--rw-r--r--   0        0        0      285 2023-01-02 13:48:40.110725 zood-0.8.1/zood/config/js/picture_title.js
--rw-r--r--   0        0        0     2301 2023-02-17 14:35:29.225249 zood-0.8.1/zood/config/js/prismjs/prism.css
--rw-r--r--   0        0        0    64866 2023-04-27 06:47:33.381797 zood-0.8.1/zood/config/js/prismjs/prism.js
--rw-r--r--   0        0        0     5999 2023-04-19 11:50:00.362712 zood-0.8.1/zood/config/js/search.js
--rw-r--r--   0        0        0      583 2023-07-29 15:25:41.350255 zood-0.8.1/zood/config/template.html
--rw-r--r--   0        0        0       69 2023-06-24 15:37:55.849962 zood-0.8.1/zood/extensions/__init__.py
--rw-r--r--   0        0        0     4109 2023-07-03 06:30:14.058101 zood-0.8.1/zood/extensions/poetry_update.py
--rw-r--r--   0        0        0     6699 2023-07-29 16:25:01.045516 zood-0.8.1/zood/gen_doc.py
--rw-r--r--   0        0        0     5547 2023-07-29 15:04:26.207636 zood-0.8.1/zood/main.py
--rw-r--r--   0        0        0     6809 2023-07-29 04:00:11.279113 zood-0.8.1/zood/util.py
--rw-r--r--   0        0        0     8041 2023-07-29 15:38:58.625505 zood-0.8.1/zood/zood.py
--rw-r--r--   0        0        0     1495 1970-01-01 00:00:00.000000 zood-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0      571 2023-07-30 05:35:32.843944 zood-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0      657 2023-07-28 05:47:50.290823 zood-0.8.2/README.md
+-rw-r--r--   0        0        0       24 2023-01-06 12:50:33.818825 zood-0.8.2/zood/__init__.py
+-rw-r--r--   0        0        0     4975 2023-07-30 02:58:53.277878 zood-0.8.2/zood/config/_config.yml
+-rw-r--r--   0        0        0      209 2022-12-30 16:25:34.984515 zood-0.8.2/zood/config/img/after_copy.png
+-rw-r--r--   0        0        0      215 2022-12-30 15:33:16.742079 zood-0.8.2/zood/config/img/before_copy.png
+-rw-r--r--   0        0        0     2720 2023-01-14 08:58:35.867485 zood-0.8.2/zood/config/img/enter.png
+-rw-r--r--   0        0        0      247 2023-01-14 09:31:22.970712 zood-0.8.2/zood/config/img/enter.svg
+-rw-r--r--   0        0        0      454 2022-12-30 16:25:01.986421 zood-0.8.2/zood/config/img/moon.png
+-rw-r--r--   0        0        0      446 2023-01-13 11:27:05.445651 zood-0.8.2/zood/config/img/search.svg
+-rw-r--r--   0        0        0      428 2022-12-30 16:24:58.219147 zood-0.8.2/zood/config/img/sun.png
+-rw-r--r--   0        0        0    15118 2023-07-30 05:04:04.782039 zood-0.8.2/zood/config/index.css
+-rw-r--r--   0        0        0     3991 2023-07-13 02:52:54.473602 zood-0.8.2/zood/config/js/change_mode.js
+-rw-r--r--   0        0        0     2646 2023-07-28 00:49:18.358387 zood-0.8.2/zood/config/js/copy_code.js
+-rw-r--r--   0        0        0     1251 2023-07-28 01:20:50.114459 zood-0.8.2/zood/config/js/global_js_configuration.js
+-rw-r--r--   0        0        0     2154 2023-07-13 02:53:27.953277 zood-0.8.2/zood/config/js/navigator.js
+-rw-r--r--   0        0        0     1000 2023-01-01 02:18:50.438286 zood-0.8.2/zood/config/js/next_front.js
+-rw-r--r--   0        0        0     1064 2023-01-02 14:54:02.515677 zood-0.8.2/zood/config/js/picture_preview.js
+-rw-r--r--   0        0        0      285 2023-01-02 13:48:40.110725 zood-0.8.2/zood/config/js/picture_title.js
+-rw-r--r--   0        0        0     2301 2023-02-17 14:35:29.225249 zood-0.8.2/zood/config/js/prismjs/prism.css
+-rw-r--r--   0        0        0    64866 2023-04-27 06:47:33.381797 zood-0.8.2/zood/config/js/prismjs/prism.js
+-rw-r--r--   0        0        0     5999 2023-04-19 11:50:00.362712 zood-0.8.2/zood/config/js/search.js
+-rw-r--r--   0        0        0      583 2023-07-29 15:25:41.350255 zood-0.8.2/zood/config/template.html
+-rw-r--r--   0        0        0       69 2023-06-24 15:37:55.849962 zood-0.8.2/zood/extensions/__init__.py
+-rw-r--r--   0        0        0     4109 2023-07-03 06:30:14.058101 zood-0.8.2/zood/extensions/poetry_update.py
+-rw-r--r--   0        0        0     6896 2023-07-30 05:32:50.697535 zood-0.8.2/zood/gen_doc.py
+-rw-r--r--   0        0        0     5547 2023-07-29 15:04:26.207636 zood-0.8.2/zood/main.py
+-rw-r--r--   0        0        0     6809 2023-07-29 04:00:11.279113 zood-0.8.2/zood/util.py
+-rw-r--r--   0        0        0     8041 2023-07-29 15:38:58.625505 zood-0.8.2/zood/zood.py
+-rw-r--r--   0        0        0     1512 1970-01-01 00:00:00.000000 zood-0.8.2/PKG-INFO
```

### Comparing `zood-0.8.1/pyproject.toml` & `zood-0.8.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "zood"
-version = "0.8.1"
+version = "0.8.2"
 description = "web page documentation & comment generation documentation"
 license = "MIT"
 authors = ["kamilu <luzhixing12345@163.com>"]
 readme = "README.md"
 repository = "https://github.com/luzhixing12345/zood"
 documentation = "https://luzhixing12345.github.io/zood/"
 
 
 [tool.poetry.dependencies]
 python = "^3.7"
 PyYAML = "*"
-MarkdownParser = "*"
+MarkdownParser = "^0.5.6"
 syntaxlight = '*'
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
```

### Comparing `zood-0.8.1/README.md` & `zood-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `zood-0.8.1/zood/config/_config.yml` & `zood-0.8.2/zood/config/_config.yml`

 * *Files identical despite different names*

### Comparing `zood-0.8.1/zood/config/img/enter.png` & `zood-0.8.2/zood/config/img/enter.png`

 * *Files identical despite different names*

### Comparing `zood-0.8.1/zood/config/index.css` & `zood-0.8.2/zood/config/index.css`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,25 @@
     line-height: 1.5;
     word-wrap: break-word;
     border-radius: 10px;
     box-shadow: "<%markdown_box_shadow%>";
     background-color: "<%markdown_bg_color%>";
 }
 
+.light {
+    background-color: #eee;
+    color: #3c4858;
+}
+
+.dark {
+    background-color: #181c27;
+    color: #c4c6c9;
+}
+
+
 .markdown-light {
     background-color: "<%markdown_bg_color%>";
 }
 
 .markdown-light h1,
 .markdown-light h2,
 .markdown-light h3,
@@ -725,12 +736,11 @@
     display: inline-block;
     max-width: 100%;
     overflow: hidden;
     text-overflow: ellipsis;
     white-space: nowrap;
 }
 
-pre[class^="language-"],
-pre.UNKNOWN {
+pre[class^="language-"] {
     background: #1f1f1f;
     color: white;
 }
```

### Comparing `zood-0.8.1/zood/config/js/change_mode.js` & `zood-0.8.2/zood/config/js/change_mode.js`

 * *Files identical despite different names*

### Comparing `zood-0.8.1/zood/config/js/copy_code.js` & `zood-0.8.2/zood/config/js/copy_code.js`

 * *Files identical despite different names*

### Comparing `zood-0.8.1/zood/config/js/global_js_configuration.js` & `zood-0.8.2/zood/config/js/global_js_configuration.js`

 * *Files identical despite different names*

### Comparing `zood-0.8.1/zood/config/js/navigator.js` & `zood-0.8.2/zood/config/js/navigator.js`

 * *Files identical despite different names*

### Comparing `zood-0.8.1/zood/config/js/next_front.js` & `zood-0.8.2/zood/config/js/next_front.js`

 * *Files identical despite different names*

### Comparing `zood-0.8.1/zood/config/js/picture_preview.js` & `zood-0.8.2/zood/config/js/picture_preview.js`

 * *Files identical despite different names*

### Comparing `zood-0.8.1/zood/config/js/prismjs/prism.css` & `zood-0.8.2/zood/config/js/prismjs/prism.css`

 * *Files identical despite different names*

### Comparing `zood-0.8.1/zood/config/js/prismjs/prism.js` & `zood-0.8.2/zood/config/js/prismjs/prism.js`

 * *Files identical despite different names*

### Comparing `zood-0.8.1/zood/config/js/search.js` & `zood-0.8.2/zood/config/js/search.js`

 * *Files identical despite different names*

### Comparing `zood-0.8.1/zood/config/template.html` & `zood-0.8.2/zood/config/template.html`

 * *Files identical despite different names*

### Comparing `zood-0.8.1/zood/extensions/poetry_update.py` & `zood-0.8.2/zood/extensions/poetry_update.py`

 * *Files identical despite different names*

### Comparing `zood-0.8.1/zood/gen_doc.py` & `zood-0.8.2/zood/gen_doc.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,17 +64,21 @@
     global LANGUAGE_USED
     for block in tree.sub_blocks:
         if block.block_name == "CodeBlock":
             language = block.input["language"]
             if syntaxlight.is_language_support(language):
                 language = syntaxlight.clean_language(language)
                 block.input["language"] = language
-                block.input["code"] = syntaxlight.parse(block.input["code"], language, file_path)
-                block.toHTML = types.MethodType(toHTML, block)
-                LANGUAGE_USED.add(language)
+                code = syntaxlight.parse(block.input["code"], language, file_path)
+                if code is not None:
+                    block.input["code"] = code
+                    block.toHTML = types.MethodType(toHTML, block)
+                    LANGUAGE_USED.add(language)
+                else:
+                    print("语法解析出错, 跳过该代码段高亮, 请按提示修改")
         else:
             hightlight_codeblock(block, file_path)
 
 
 
 def generate_docs(directory_tree, markdown_htmls, md_dir_name):
     config = get_zood_config()
```

### Comparing `zood-0.8.1/zood/main.py` & `zood-0.8.2/zood/main.py`

 * *Files identical despite different names*

### Comparing `zood-0.8.1/zood/util.py` & `zood-0.8.2/zood/util.py`

 * *Files identical despite different names*

### Comparing `zood-0.8.1/zood/zood.py` & `zood-0.8.2/zood/zood.py`

 * *Files identical despite different names*

### Comparing `zood-0.8.1/PKG-INFO` & `zood-0.8.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: zood
-Version: 0.8.1
+Version: 0.8.2
 Summary: web page documentation & comment generation documentation
 Home-page: https://github.com/luzhixing12345/zood
 License: MIT
 Author: kamilu
 Author-email: luzhixing12345@163.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: MarkdownParser
+Requires-Dist: MarkdownParser (>=0.5.6,<0.6.0)
 Requires-Dist: PyYAML
 Requires-Dist: syntaxlight
 Project-URL: Documentation, https://luzhixing12345.github.io/zood/
 Project-URL: Repository, https://github.com/luzhixing12345/zood
 Description-Content-Type: text/markdown
 
 # zood
```

