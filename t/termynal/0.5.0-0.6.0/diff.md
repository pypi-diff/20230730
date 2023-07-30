# Comparing `tmp/termynal-0.5.0.tar.gz` & `tmp/termynal-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "termynal-0.5.0.tar", max compression
+gzip compressed data, was "termynal-0.6.0.tar", max compression
```

## Comparing `termynal-0.5.0.tar` & `termynal-0.6.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1092 2023-07-22 16:51:35.582324 termynal-0.5.0/LICENSE
--rw-r--r--   0        0        0     1758 2023-07-22 16:51:35.582324 termynal-0.5.0/README.md
--rw-r--r--   0        0        0     2415 2023-07-22 16:51:35.582324 termynal-0.5.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-22 16:51:35.582324 termynal-0.5.0/termynal/__init__.py
--rw-r--r--   0        0        0     2281 2023-07-22 16:51:35.582324 termynal-0.5.0/termynal/assets/termynal.css
--rw-r--r--   0        0        0     9704 2023-07-22 16:51:35.582324 termynal-0.5.0/termynal/assets/termynal.js
--rw-r--r--   0        0        0     5541 2023-07-22 16:51:35.582324 termynal-0.5.0/termynal/markdown.py
--rw-r--r--   0        0        0     1121 2023-07-22 16:51:35.582324 termynal-0.5.0/termynal/plugin.py
--rw-r--r--   0        0        0     2423 1970-01-01 00:00:00.000000 termynal-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-07-30 06:47:20.978323 termynal-0.6.0/LICENSE
+-rw-r--r--   0        0        0     1758 2023-07-30 06:47:20.978323 termynal-0.6.0/README.md
+-rw-r--r--   0        0        0     2461 2023-07-30 06:47:20.978323 termynal-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-30 06:47:20.978323 termynal-0.6.0/termynal/__init__.py
+-rw-r--r--   0        0        0     2303 2023-07-30 06:47:20.978323 termynal-0.6.0/termynal/assets/termynal.css
+-rw-r--r--   0        0        0     9704 2023-07-30 06:47:20.978323 termynal-0.6.0/termynal/assets/termynal.js
+-rw-r--r--   0        0        0     5643 2023-07-30 06:47:20.978323 termynal-0.6.0/termynal/markdown.py
+-rw-r--r--   0        0        0     1121 2023-07-30 06:47:20.978323 termynal-0.6.0/termynal/plugin.py
+-rw-r--r--   0        0        0     2423 1970-01-01 00:00:00.000000 termynal-0.6.0/PKG-INFO
```

### Comparing `termynal-0.5.0/LICENSE` & `termynal-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `termynal-0.5.0/README.md` & `termynal-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `termynal-0.5.0/pyproject.toml` & `termynal-0.6.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.5.0"
+version = "0.6.0"
 tag_format = "v$version"
 version_files = [
     "pyproject.toml:version"
 ]
 bump_message = "chore(release): version $current_version → $new_version"
 update_changelog_on_bump = true
 
 [tool.poetry]
 name = "termynal"
-version = "0.5.0"
+version = "0.6.0"
 description = ""
 authors = ["Danil Akhtarov <daxartio@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/daxartio/termynal"
 homepage = "https://pypi.org/project/termynal"
 keywords = []
@@ -34,17 +34,19 @@
 black = "*"
 mypy = "*"
 pytest = "*"
 pytest-asyncio = "*"
 pytest-cov = "*"
 pytest-deadfixtures = "*"
 pytest-mock = "*"
+pyyaml = "^6.0.1"
 ruff = "*"
 toml = "*"
 types-Markdown = "*"
+types-pyyaml = "^6.0.12.11"
 
 [tool.poetry.group.docs.dependencies]
 markdown-include = "^0.8.1"
 mkdocs = "*"
 mkdocs-material = "*"
 
 [tool.poetry.group.git.dependencies]
@@ -69,15 +71,15 @@
 [tool.coverage.run]
 omit = ["tests/*", "**/__main__.py", "**/.venv/*", "**/site-packages/*"]
 branch = true
 
 [tool.coverage.report]
 show_missing = true
 skip_covered = true
-fail_under = 90
+fail_under = 94
 
 [tool.pytest.ini_options]
 asyncio_mode = "strict"
 addopts = "--strict-markers --showlocals --verbosity 2"
 log_level = "DEBUG"
 
 [tool.ruff]
```

### Comparing `termynal-0.5.0/termynal/assets/termynal.css` & `termynal-0.6.0/termynal/assets/termynal.css`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,15 @@
     display: block;
     color: #aebbff;
 }
 
 [data-ty] {
     display: block;
     line-height: 2;
+    white-space: pre;
 }
 
 [data-ty]:before {
     /* Set up defaults and ensure empty lines are displayed. */
     content: '';
     display: inline-block;
     vertical-align: middle;
```

### Comparing `termynal-0.5.0/termynal/assets/termynal.js` & `termynal-0.6.0/termynal/assets/termynal.js`

 * *Files identical despite different names*

### Comparing `termynal-0.5.0/termynal/markdown.py` & `termynal-0.6.0/termynal/markdown.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,100 +1,99 @@
 import re
-from typing import TYPE_CHECKING, Dict, List
+from typing import TYPE_CHECKING, Any, Dict, Iterable, List, Tuple
 
 from markdown.extensions import Extension
 from markdown.preprocessors import Preprocessor
 
 if TYPE_CHECKING:  # pragma:no cover
     from markdown import core
 
 
 class Termynal:
     progress_literal_start = "---&gt; 100%"
     custom_literal_start = "# "
 
     def __init__(
         self,
-        prompt_literal_start: tuple = ("$ ",),
+        prompt_literal_start: Iterable[str] = ("$ ",),
         promt_in_multiline: bool = False,
     ):
-        """Initialize."""
         self.prompt_literal_start = "|".join(re.escape(p) for p in prompt_literal_start)
         self.regex_prompts = re.compile(f"^({self.prompt_literal_start})")
         self.promt_in_multiline = promt_in_multiline
 
-    def convert(self, code: str) -> List[str]:
-        code_lines = []
+    def convert(self, code: str) -> str:
+        code_lines: List[str] = []
         code_lines.append('<div class="termy" data-termynal>')
         multiline = False
         used_prompt = None
         for line in code.split("\n"):
             if match := self.regex_prompts.match(line):
                 used_prompt = match.group()
                 code_lines.append(
                     f'<span data-ty="input" data-ty-prompt="{used_prompt.strip()}">'
-                    f"{line.rsplit(used_prompt)[1].replace(' ', '&nbsp;')}</span>",
+                    f"{line.rsplit(used_prompt)[1]}</span>",
                 )
                 multiline = bool(line.endswith("\\"))
             elif multiline:
                 used_prompt = used_prompt or ""
                 if not self.promt_in_multiline:
                     used_prompt = ""
                 code_lines.append(
                     f'<span data-ty="input" data-ty-prompt="{used_prompt.strip()}">'
-                    f'{line.replace(" ", "&nbsp;")}</span>',
+                    f"{line}</span>",
                 )
                 multiline = bool(line.endswith("\\"))
 
             elif line.startswith(self.custom_literal_start):
                 code_lines.append(
                     f'<span class="termynal-comment" data-ty>{line}</span>',
                 )
             elif line.startswith(self.progress_literal_start):
                 code_lines.append('<span data-ty="progress"></span>')
             else:
                 code_lines.append(f"<span data-ty>{line}</span>")
         code_lines.append("</div>")
-        return code_lines
+        return "\n".join(code_lines)
 
 
 class TermynalPreprocessor(Preprocessor):
     rexep = re.compile("(<code.*>)((.|\n)*?)(</code>)")
     comment = "<!-- termynal -->"
     language_class = 'class="language-console"'
 
-    def __init__(self, config: dict, md: "core.Markdown"):
-        """Initialize."""
+    def __init__(self, config: Dict[str, Any], md: "core.Markdown"):
         self.prompt_literal_start = config.get("prompt_literal_start", ("$ ",))
         self.promt_in_multiline = config.get("promt_in_multiline", False)
 
         super(TermynalPreprocessor, self).__init__(md=md)
 
-    def run(self, lines: List):
+    def run(self, lines: List[str]) -> List[str]:
         content_by_placeholder = {}
         for i in range(self.md.htmlStash.html_counter):
             placeholder = self.md.htmlStash.get_placeholder(i)
             content = self.md.htmlStash.rawHtmlBlocks[i]
             content_by_placeholder[placeholder] = (content, i)
 
-        lines_by_placeholder = self._get_lines(lines, content_by_placeholder)
+        target_code_by_placeholder = self._get_lines(lines, content_by_placeholder)
 
         new_lines = []
         for line in lines:
-            new_lines.append(line)
-            if line in lines_by_placeholder:
-                new_lines.extend(lines_by_placeholder[line])
+            if line in target_code_by_placeholder:
+                new_lines.append(target_code_by_placeholder[line])
+            else:
+                new_lines.append(line)
 
         return new_lines
 
     def _get_lines(
         self,
-        lines: List,
-        content_by_placeholder: Dict,
-    ):  # pylint:disable=too-many-nested-blocks
+        lines: List[str],
+        content_by_placeholder: Dict[str, Tuple[str, int]],
+    ) -> Dict[str, str]:  # pylint:disable=too-many-nested-blocks
         termynal_obj = Termynal(
             prompt_literal_start=self.prompt_literal_start,
             promt_in_multiline=self.promt_in_multiline,
         )
         lines_by_placeholder = {}
         is_termynal_code = False
         for line in lines:
@@ -115,26 +114,25 @@
                 if self.language_class in matches.group(1):
                     is_termynal_code = True
 
                 if not is_termynal_code:
                     continue
 
                 is_termynal_code = False
-                self.md.htmlStash.rawHtmlBlocks[i] = ""
                 content = matches.group(2)
-                code_lines = termynal_obj.convert(code=content)
-                if code_lines:
-                    lines_by_placeholder[line] = code_lines
+                target_code = termynal_obj.convert(code=content)
+                if target_code:
+                    self.md.htmlStash.rawHtmlBlocks[i] = ""
+                    lines_by_placeholder[line] = target_code
 
         return lines_by_placeholder
 
 
 class TermynalExtension(Extension):
-    def __init__(self, *args, **kwargs):
-        """Initialize."""
+    def __init__(self, *args: Any, **kwargs: Any):
         self.config = {
             "prompt_literal_start": [
                 [
                     "$ ",
                 ],
                 "A list of prompt characters start to consider as console - "
                 "Default: ['$ ',]",
@@ -143,17 +141,20 @@
                 False,
                 "Default: False",
             ],
         }
 
         super(TermynalExtension, self).__init__(*args, **kwargs)
 
-    def extendMarkdown(self, md: "core.Markdown"):  # noqa:N802
+    def extendMarkdown(self, md: "core.Markdown") -> None:  # noqa:N802
         """Register the extension."""
         md.registerExtension(self)
         config = self.getConfigs()
         md.preprocessors.register(TermynalPreprocessor(config, md), "termynal", 20)
 
 
-def makeExtension(*args, **kwargs):  # noqa:N802  # pylint:disable=invalid-name
+def makeExtension(  # noqa:N802  # pylint:disable=invalid-name
+    *args: Any,
+    **kwargs: Any,
+) -> TermynalExtension:
     """Return extension."""
     return TermynalExtension(*args, **kwargs)
```

### Comparing `termynal-0.5.0/termynal/plugin.py` & `termynal-0.6.0/termynal/plugin.py`

 * *Files identical despite different names*

### Comparing `termynal-0.5.0/PKG-INFO` & `termynal-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: termynal
-Version: 0.5.0
+Version: 0.6.0
 Summary: 
 Home-page: https://pypi.org/project/termynal
 License: MIT
 Author: Danil Akhtarov
 Author-email: daxartio@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

