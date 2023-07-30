# Comparing `tmp/syntaxlight-0.0.8.tar.gz` & `tmp/syntaxlight-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syntaxlight-0.0.8.tar", max compression
+gzip compressed data, was "syntaxlight-0.0.9.tar", max compression
```

## Comparing `syntaxlight-0.0.8.tar` & `syntaxlight-0.0.9.tar`

### file list

```diff
@@ -1,40 +1,41 @@
--rw-r--r--   0        0        0     1064 2023-06-08 14:13:12.759574 syntaxlight-0.0.8/LICENSE
--rw-r--r--   0        0        0      464 2023-07-29 14:40:09.550161 syntaxlight-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     2183 2023-07-22 12:55:46.842043 syntaxlight-0.0.8/README.md
--rw-r--r--   0        0        0      187 2023-07-29 14:31:45.643282 syntaxlight-0.0.8/syntaxlight/__init__.py
--rw-r--r--   0        0        0    15173 2023-07-29 13:02:30.287941 syntaxlight-0.0.8/syntaxlight/ast.py
--rw-r--r--   0        0        0     2223 2023-07-29 13:42:32.821896 syntaxlight-0.0.8/syntaxlight/css/all.css
--rw-r--r--   0        0        0      665 2023-07-22 15:03:22.184483 syntaxlight-0.0.8/syntaxlight/css/bnf.css
--rw-r--r--   0        0        0     2118 2023-07-23 15:21:29.646891 syntaxlight-0.0.8/syntaxlight/css/c.css
--rw-r--r--   0        0        0    18397 2023-06-15 07:10:53.753178 syntaxlight-0.0.8/syntaxlight/css/index.css
--rw-r--r--   0        0        0      529 2023-07-21 12:50:35.868013 syntaxlight-0.0.8/syntaxlight/css/json.css
--rw-r--r--   0        0        0     1101 2023-07-26 09:05:41.943038 syntaxlight-0.0.8/syntaxlight/css/lua.css
--rw-r--r--   0        0        0      744 2023-07-29 14:18:59.090972 syntaxlight-0.0.8/syntaxlight/css/shell.css
--rw-r--r--   0        0        0     2812 2023-07-29 14:20:16.175242 syntaxlight-0.0.8/syntaxlight/css/themes.json
--rw-r--r--   0        0        0      557 2023-07-19 08:11:34.232315 syntaxlight-0.0.8/syntaxlight/css/toml.css
--rw-r--r--   0        0        0      495 2023-07-19 08:15:19.310673 syntaxlight-0.0.8/syntaxlight/css/xml.css
--rw-r--r--   0        0        0     2428 2023-07-26 07:25:50.581952 syntaxlight-0.0.8/syntaxlight/error.py
--rw-r--r--   0        0        0     2011 2023-07-25 01:37:18.564742 syntaxlight-0.0.8/syntaxlight/example.py
--rw-r--r--   0        0        0     1666 2023-07-29 05:28:25.722849 syntaxlight-0.0.8/syntaxlight/export.py
--rw-r--r--   0        0        0     2781 2023-07-29 13:56:47.817032 syntaxlight-0.0.8/syntaxlight/gdt.py
--rw-r--r--   0        0        0      401 2023-07-24 09:03:19.313778 syntaxlight-0.0.8/syntaxlight/lexers/__init__.py
--rw-r--r--   0        0        0     1921 2023-07-26 05:57:52.779798 syntaxlight-0.0.8/syntaxlight/lexers/bnf_lexer.py
--rw-r--r--   0        0        0    12514 2023-07-29 03:41:26.897980 syntaxlight-0.0.8/syntaxlight/lexers/c_lexer.py
--rw-r--r--   0        0        0     1995 2023-07-26 05:58:05.904375 syntaxlight-0.0.8/syntaxlight/lexers/json_lexer.py
--rw-r--r--   0        0        0    22638 2023-07-29 13:36:11.005583 syntaxlight-0.0.8/syntaxlight/lexers/lexer.py
--rw-r--r--   0        0        0     8150 2023-07-26 08:57:37.822371 syntaxlight-0.0.8/syntaxlight/lexers/lua_lexer.py
--rw-r--r--   0        0        0     4077 2023-07-29 14:16:38.127889 syntaxlight-0.0.8/syntaxlight/lexers/shell_lexer.py
--rw-r--r--   0        0        0     3002 2023-07-26 02:47:58.836633 syntaxlight-0.0.8/syntaxlight/lexers/toml_lexer.py
--rw-r--r--   0        0        0     4576 2023-07-26 05:58:25.950097 syntaxlight-0.0.8/syntaxlight/lexers/xml_lexer.py
--rw-r--r--   0        0        0      275 2023-07-25 01:05:05.983118 syntaxlight-0.0.8/syntaxlight/parsers/__init__.py
--rw-r--r--   0        0        0     6950 2023-07-24 08:35:40.217597 syntaxlight-0.0.8/syntaxlight/parsers/bnf_parser.py
--rw-r--r--   0        0        0    99058 2023-07-29 03:43:10.405548 syntaxlight-0.0.8/syntaxlight/parsers/c_parser.py
--rw-r--r--   0        0        0     5758 2023-07-24 01:35:24.219886 syntaxlight-0.0.8/syntaxlight/parsers/json_parser.py
--rw-r--r--   0        0        0    35078 2023-07-26 09:03:07.504849 syntaxlight-0.0.8/syntaxlight/parsers/lua_parser.py
--rw-r--r--   0        0        0    12778 2023-07-29 14:00:12.143979 syntaxlight-0.0.8/syntaxlight/parsers/parser.py
--rw-r--r--   0        0        0     2344 2023-07-29 14:21:32.659521 syntaxlight-0.0.8/syntaxlight/parsers/shell_parser.py
--rw-r--r--   0        0        0    11810 2023-07-24 01:35:24.522506 syntaxlight-0.0.8/syntaxlight/parsers/toml_parser.py
--rw-r--r--   0        0        0     6531 2023-07-24 01:35:24.720887 syntaxlight-0.0.8/syntaxlight/parsers/xml_parser.py
--rw-r--r--   0        0        0     4277 2023-07-29 13:01:51.131206 syntaxlight-0.0.8/syntaxlight/syntax_parse.py
--rw-r--r--   0        0        0      349 2023-07-25 01:26:08.919200 syntaxlight-0.0.8/syntaxlight/template.html
--rw-r--r--   0        0        0     2825 1970-01-01 00:00:00.000000 syntaxlight-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-08 14:13:12.759574 syntaxlight-0.0.9/LICENSE
+-rw-r--r--   0        0        0      464 2023-07-29 15:18:30.018496 syntaxlight-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2183 2023-07-22 12:55:46.842043 syntaxlight-0.0.9/README.md
+-rw-r--r--   0        0        0      187 2023-07-29 14:31:45.643282 syntaxlight-0.0.9/syntaxlight/__init__.py
+-rw-r--r--   0        0        0    15173 2023-07-29 13:02:30.287941 syntaxlight-0.0.9/syntaxlight/ast.py
+-rw-r--r--   0        0        0     2223 2023-07-29 13:42:32.821896 syntaxlight-0.0.9/syntaxlight/css/all.css
+-rw-r--r--   0        0        0      665 2023-07-22 15:03:22.184483 syntaxlight-0.0.9/syntaxlight/css/bnf.css
+-rw-r--r--   0        0        0     2118 2023-07-23 15:21:29.646891 syntaxlight-0.0.9/syntaxlight/css/c.css
+-rw-r--r--   0        0        0    18397 2023-06-15 07:10:53.753178 syntaxlight-0.0.9/syntaxlight/css/index.css
+-rw-r--r--   0        0        0      529 2023-07-21 12:50:35.868013 syntaxlight-0.0.9/syntaxlight/css/json.css
+-rw-r--r--   0        0        0     1101 2023-07-26 09:05:41.943038 syntaxlight-0.0.9/syntaxlight/css/lua.css
+-rw-r--r--   0        0        0      744 2023-07-29 14:18:59.090972 syntaxlight-0.0.9/syntaxlight/css/shell.css
+-rw-r--r--   0        0        0     2812 2023-07-29 14:20:16.175242 syntaxlight-0.0.9/syntaxlight/css/themes.json
+-rw-r--r--   0        0        0      557 2023-07-19 08:11:34.232315 syntaxlight-0.0.9/syntaxlight/css/toml.css
+-rw-r--r--   0        0        0      495 2023-07-19 08:15:19.310673 syntaxlight-0.0.9/syntaxlight/css/xml.css
+-rw-r--r--   0        0        0     2428 2023-07-26 07:25:50.581952 syntaxlight-0.0.9/syntaxlight/error.py
+-rw-r--r--   0        0        0     1947 2023-07-29 15:01:42.303917 syntaxlight-0.0.9/syntaxlight/example.py
+-rw-r--r--   0        0        0     1676 2023-07-29 15:00:43.690651 syntaxlight-0.0.9/syntaxlight/export.py
+-rw-r--r--   0        0        0     2781 2023-07-29 13:56:47.817032 syntaxlight-0.0.9/syntaxlight/gdt.py
+-rw-r--r--   0        0        0     1882 2023-07-29 15:16:31.592870 syntaxlight-0.0.9/syntaxlight/language.py
+-rw-r--r--   0        0        0      401 2023-07-24 09:03:19.313778 syntaxlight-0.0.9/syntaxlight/lexers/__init__.py
+-rw-r--r--   0        0        0     1921 2023-07-26 05:57:52.779798 syntaxlight-0.0.9/syntaxlight/lexers/bnf_lexer.py
+-rw-r--r--   0        0        0    12514 2023-07-29 03:41:26.897980 syntaxlight-0.0.9/syntaxlight/lexers/c_lexer.py
+-rw-r--r--   0        0        0     1995 2023-07-26 05:58:05.904375 syntaxlight-0.0.9/syntaxlight/lexers/json_lexer.py
+-rw-r--r--   0        0        0    22638 2023-07-29 13:36:11.005583 syntaxlight-0.0.9/syntaxlight/lexers/lexer.py
+-rw-r--r--   0        0        0     8150 2023-07-26 08:57:37.822371 syntaxlight-0.0.9/syntaxlight/lexers/lua_lexer.py
+-rw-r--r--   0        0        0     4077 2023-07-29 14:16:38.127889 syntaxlight-0.0.9/syntaxlight/lexers/shell_lexer.py
+-rw-r--r--   0        0        0     3002 2023-07-26 02:47:58.836633 syntaxlight-0.0.9/syntaxlight/lexers/toml_lexer.py
+-rw-r--r--   0        0        0     4576 2023-07-26 05:58:25.950097 syntaxlight-0.0.9/syntaxlight/lexers/xml_lexer.py
+-rw-r--r--   0        0        0      275 2023-07-25 01:05:05.983118 syntaxlight-0.0.9/syntaxlight/parsers/__init__.py
+-rw-r--r--   0        0        0     6950 2023-07-24 08:35:40.217597 syntaxlight-0.0.9/syntaxlight/parsers/bnf_parser.py
+-rw-r--r--   0        0        0    99058 2023-07-29 03:43:10.405548 syntaxlight-0.0.9/syntaxlight/parsers/c_parser.py
+-rw-r--r--   0        0        0     5758 2023-07-24 01:35:24.219886 syntaxlight-0.0.9/syntaxlight/parsers/json_parser.py
+-rw-r--r--   0        0        0    35078 2023-07-26 09:03:07.504849 syntaxlight-0.0.9/syntaxlight/parsers/lua_parser.py
+-rw-r--r--   0        0        0    12778 2023-07-29 14:00:12.143979 syntaxlight-0.0.9/syntaxlight/parsers/parser.py
+-rw-r--r--   0        0        0     2344 2023-07-29 14:21:32.659521 syntaxlight-0.0.9/syntaxlight/parsers/shell_parser.py
+-rw-r--r--   0        0        0    11810 2023-07-24 01:35:24.522506 syntaxlight-0.0.9/syntaxlight/parsers/toml_parser.py
+-rw-r--r--   0        0        0     6531 2023-07-24 01:35:24.720887 syntaxlight-0.0.9/syntaxlight/parsers/xml_parser.py
+-rw-r--r--   0        0        0     2842 2023-07-29 15:18:08.408506 syntaxlight-0.0.9/syntaxlight/syntax_parse.py
+-rw-r--r--   0        0        0      349 2023-07-25 01:26:08.919200 syntaxlight-0.0.9/syntaxlight/template.html
+-rw-r--r--   0        0        0     2825 1970-01-01 00:00:00.000000 syntaxlight-0.0.9/PKG-INFO
```

### Comparing `syntaxlight-0.0.8/LICENSE` & `syntaxlight-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.8/README.md` & `syntaxlight-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.8/syntaxlight/ast.py` & `syntaxlight-0.0.9/syntaxlight/ast.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.8/syntaxlight/css/all.css` & `syntaxlight-0.0.9/syntaxlight/css/all.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.8/syntaxlight/css/bnf.css` & `syntaxlight-0.0.9/syntaxlight/css/bnf.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.8/syntaxlight/css/c.css` & `syntaxlight-0.0.9/syntaxlight/css/c.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.8/syntaxlight/css/index.css` & `syntaxlight-0.0.9/syntaxlight/css/index.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.8/syntaxlight/css/json.css` & `syntaxlight-0.0.9/syntaxlight/css/json.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.8/syntaxlight/css/lua.css` & `syntaxlight-0.0.9/syntaxlight/css/lua.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.8/syntaxlight/css/shell.css` & `syntaxlight-0.0.9/syntaxlight/css/shell.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.8/syntaxlight/css/themes.json` & `syntaxlight-0.0.9/syntaxlight/css/themes.json`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.8/syntaxlight/css/toml.css` & `syntaxlight-0.0.9/syntaxlight/css/toml.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.8/syntaxlight/error.py` & `syntaxlight-0.0.9/syntaxlight/error.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.8/syntaxlight/example.py` & `syntaxlight-0.0.9/syntaxlight/example.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,10 +46,9 @@
 
     with open(os.path.join(example_folder_name, example_html_file), "w", encoding="utf-8") as f:
         f.write(content)
 
     for file in css_files:
         shutil.copyfile(file, os.path.join(example_folder_name, file.split(os.sep)[-1]))
 
-    export_name = os.path.join(example_folder_name, f"{language}.css")
-    export_css([language], export_name, style)
+    export_css([language], example_folder_name, style)
     # print(f"open syntaxlight_example/inedx.html in browser")
```

### Comparing `syntaxlight-0.0.8/syntaxlight/export.py` & `syntaxlight-0.0.9/syntaxlight/export.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from typing import Dict, List
 import json
 
 
-def export_css(languages: List[str], export_name: str = "index.css", style: str = "vscode"):
+def export_css(languages: List[str], export_dir: str = ".", style: str = "vscode"):
     syntaxlight_path = os.path.dirname(__file__)
     json_file_path = os.path.join(syntaxlight_path, "css", "themes.json")
     with open(json_file_path, "r", encoding="utf-8") as f:
         themes: Dict[str, Dict[str, str]] = json.load(f)
 
     EXTENSION_NAME = "extension"
 
@@ -30,14 +30,14 @@
             # 使用主题颜色替换 css 文件中的对应类型
             for type_name, color in theme.items():
                 if type_name == EXTENSION_NAME:
                     continue
 
                 css_content = css_content.replace(type_name, color)
 
-            with open(export_name, "w", encoding="utf-8") as f:
+            with open(f'{export_dir}/{language}.css', "w", encoding="utf-8") as f:
                 f.write(css_content)
     else:
         print(f"unknown style {style}")
         print(f"supported style: {list(themes.keys())}")
         exit(1)
```

### Comparing `syntaxlight-0.0.8/syntaxlight/gdt.py` & `syntaxlight-0.0.9/syntaxlight/gdt.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.8/syntaxlight/lexers/bnf_lexer.py` & `syntaxlight-0.0.9/syntaxlight/lexers/bnf_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.8/syntaxlight/lexers/c_lexer.py` & `syntaxlight-0.0.9/syntaxlight/lexers/c_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.8/syntaxlight/lexers/json_lexer.py` & `syntaxlight-0.0.9/syntaxlight/lexers/json_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.8/syntaxlight/lexers/lexer.py` & `syntaxlight-0.0.9/syntaxlight/lexers/lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.8/syntaxlight/lexers/lua_lexer.py` & `syntaxlight-0.0.9/syntaxlight/lexers/lua_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.8/syntaxlight/lexers/shell_lexer.py` & `syntaxlight-0.0.9/syntaxlight/lexers/shell_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.8/syntaxlight/lexers/toml_lexer.py` & `syntaxlight-0.0.9/syntaxlight/lexers/toml_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.8/syntaxlight/lexers/xml_lexer.py` & `syntaxlight-0.0.9/syntaxlight/lexers/xml_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.8/syntaxlight/parsers/bnf_parser.py` & `syntaxlight-0.0.9/syntaxlight/parsers/bnf_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.8/syntaxlight/parsers/c_parser.py` & `syntaxlight-0.0.9/syntaxlight/parsers/c_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.8/syntaxlight/parsers/json_parser.py` & `syntaxlight-0.0.9/syntaxlight/parsers/json_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.8/syntaxlight/parsers/lua_parser.py` & `syntaxlight-0.0.9/syntaxlight/parsers/lua_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.8/syntaxlight/parsers/parser.py` & `syntaxlight-0.0.9/syntaxlight/parsers/parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.8/syntaxlight/parsers/shell_parser.py` & `syntaxlight-0.0.9/syntaxlight/parsers/shell_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.8/syntaxlight/parsers/toml_parser.py` & `syntaxlight-0.0.9/syntaxlight/parsers/toml_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.8/syntaxlight/parsers/xml_parser.py` & `syntaxlight-0.0.9/syntaxlight/parsers/xml_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.8/syntaxlight/syntax_parse.py` & `syntaxlight-0.0.9/syntaxlight/syntax_parse.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,50 +1,22 @@
 import os
 from .lexers import *
-from .error import Error
 from .parsers import *
+from .error import Error
+from .language import guess_language, SUPPORTED_SYNTAX, show_help_info, clean_language
 from .ast import display_ast
 import sys
-from typing import List, TypedDict
-
-class SyntaxDict(TypedDict):
-    lexer: Lexer
-    parser: Parser
-    suffix: List[str]
-
-SUPPORTED_SYNTAX = {
-    "json": SyntaxDict(lexer=JsonLexer, parser=JsonParser, suffix=['json']),
-    "c": SyntaxDict(lexer=CLexer, parser=CParser, suffix=["c", "h"]),
-    "lua": SyntaxDict(lexer=LuaLexer, parser=LuaParser, suffix=['lua']),
-    "bnf": SyntaxDict(lexer=BNFLexer, parser=BNFParser, suffix=['bnf']),
-    "toml": SyntaxDict(lexer=TomlLexer, parser=TomlParser, suffix=['toml']),
-    "xml": SyntaxDict(lexer=XmlLexer, parser=XmlParser, suffix=['xml']),
-    "shell": SyntaxDict(lexer=ShellLexer, parser=ShellParser, suffix=['sh']),
-    "bash": SyntaxDict(lexer=ShellLexer, parser=ShellParser, suffix=['sh'])
-}
-
-
-def is_language_support(language: str):
-    """
-    检验 syntaxlight 是否支持当前语言
-    """
-    global SUPPORTED_SYNTAX
-    language = language.lower()
-    if language in SUPPORTED_SYNTAX:
-        return True
-    else:
-        return False
 
 
 def parse(
     text: str, language=None, file_path=None, show_error_context=True, save_ast_tree=False
 ) -> str:
     if len(text) == 0:
         return ""
-
+    language = clean_language(language)
     parser = get_parser(text, language)
     parser.lexer.file_path = file_path
 
     try:
         parser.parse()
     except Error as e:
         sys.stderr.write(e.message)
@@ -61,48 +33,26 @@
         print(f"{file_path} file not exsist")
 
     with open(file_path, "r", encoding="utf-8") as f:
         text = f.read()
 
     if language is None:
         language = guess_language(file_path)
+    else:
+        language = clean_language(language)
 
     return parse(
         text,
         language=language,
         file_path=file_path,
         show_error_context=show_error_context,
         save_ast_tree=save_ast_tree,
     )
 
 
-def guess_language(file_path: str) -> str:
-    """
-    通过文件名猜测文法类型
-    """
-    suffix_name = file_path.split(os.sep)[-1].split(".")[-1]
-    for language in SUPPORTED_SYNTAX:
-        if suffix_name in SUPPORTED_SYNTAX[language]["suffix"]:
-            return language
-
-    if suffix_name in SUPPORTED_SYNTAX:
-        return suffix_name
-
-    print("fail to guess language")
-    show_help_info()
-    exit(1)
-
-
-def show_help_info():
-    print(f"supported language:")
-    for language in SUPPORTED_SYNTAX:
-        print(f"{language:>10}:", SUPPORTED_SYNTAX[language]["suffix"])
-    exit(1)
-
-
 def get_tokens(lexer: Lexer):
     token = lexer.get_next_token()
     tokens = [token]
     while token.type.value != "EOF":
         try:
             token = lexer.get_next_token()
             tokens.append(token)
@@ -138,8 +88,9 @@
             code = f.read()
 
         if language is None:
             language = guess_language(code_or_path)
     else:
         code = code_or_path
 
+    language = clean_language(language)
     return code, language
```

### Comparing `syntaxlight-0.0.8/PKG-INFO` & `syntaxlight-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syntaxlight
-Version: 0.0.8
+Version: 0.0.9
 Summary: syntax highlight based on EBNF
 Home-page: https://github.com/luzhixing12345/syntaxlight
 License: MIT
 Author: luzhixing12345
 Author-email: luzhixing12345@163.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

