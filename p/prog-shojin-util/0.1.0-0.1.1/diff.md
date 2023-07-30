# Comparing `tmp/prog_shojin_util-0.1.0.tar.gz` & `tmp/prog_shojin_util-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prog_shojin_util-0.1.0.tar", max compression
+gzip compressed data, was "prog_shojin_util-0.1.1.tar", max compression
```

## Comparing `prog_shojin_util-0.1.0.tar` & `prog_shojin_util-0.1.1.tar`

### file list

```diff
@@ -1,32 +1,34 @@
--rw-r--r--   0        0        0     1069 2023-07-29 07:29:18.593820 prog_shojin_util-0.1.0/LICENSE
--rw-r--r--   0        0        0     2567 2023-07-30 03:34:39.777484 prog_shojin_util-0.1.0/README.md
--rw-r--r--   0        0        0      358 2023-07-29 10:23:09.218461 prog_shojin_util-0.1.0/prog_shojin_util/__init__.py
--rw-r--r--   0        0        0       65 2023-07-27 15:43:20.938318 prog_shojin_util-0.1.0/prog_shojin_util/__main__.py
--rw-r--r--   0        0        0     2830 2023-07-30 03:34:39.777484 prog_shojin_util-0.1.0/prog_shojin_util/cli.py
--rw-r--r--   0        0        0      304 2023-07-29 07:10:58.961822 prog_shojin_util-0.1.0/prog_shojin_util/logging_config.py
--rw-r--r--   0        0        0        0 2023-07-27 15:43:20.942318 prog_shojin_util-0.1.0/prog_shojin_util/scraper/__init__.py
--rw-r--r--   0        0        0     1089 2023-07-30 03:34:39.777484 prog_shojin_util-0.1.0/prog_shojin_util/scraper/link_collector.py
--rw-r--r--   0        0        0     1806 2023-07-30 03:34:39.777484 prog_shojin_util-0.1.0/prog_shojin_util/services/output_formatter.py
--rw-r--r--   0        0        0     1722 2023-07-29 10:23:09.218461 prog_shojin_util-0.1.0/prog_shojin_util/services/problem_finder.py
--rw-r--r--   0        0        0        0 2023-07-27 15:43:20.942318 prog_shojin_util-0.1.0/prog_shojin_util/utils/__init__.py
--rw-r--r--   0        0        0     1223 2023-07-29 10:23:09.218461 prog_shojin_util-0.1.0/prog_shojin_util/utils/cache.py
--rw-r--r--   0        0        0     1373 2023-07-29 10:23:09.218461 prog_shojin_util-0.1.0/prog_shojin_util/utils/contest_site_factory.py
--rw-r--r--   0        0        0      201 2023-07-29 10:23:09.218461 prog_shojin_util-0.1.0/prog_shojin_util/utils/contest_sites/__init__.py
--rw-r--r--   0        0        0      119 2023-07-29 10:23:09.218461 prog_shojin_util-0.1.0/prog_shojin_util/utils/contest_sites/abstract/__init__.py
--rw-r--r--   0        0        0      451 2023-07-29 10:23:09.218461 prog_shojin_util-0.1.0/prog_shojin_util/utils/contest_sites/abstract/api.py
--rw-r--r--   0        0        0      447 2023-07-29 10:23:09.218461 prog_shojin_util-0.1.0/prog_shojin_util/utils/contest_sites/abstract/matcher.py
--rw-r--r--   0        0        0      289 2023-07-29 07:10:58.965822 prog_shojin_util-0.1.0/prog_shojin_util/utils/contest_sites/abstract/parser.py
--rw-r--r--   0        0        0     1388 2023-07-29 10:23:09.218461 prog_shojin_util-0.1.0/prog_shojin_util/utils/contest_sites/api_utils.py
--rw-r--r--   0        0        0       98 2023-07-29 10:23:09.218461 prog_shojin_util-0.1.0/prog_shojin_util/utils/contest_sites/atcoder/__init__.py
--rw-r--r--   0        0        0     3043 2023-07-29 10:23:09.218461 prog_shojin_util-0.1.0/prog_shojin_util/utils/contest_sites/atcoder/api.py
--rw-r--r--   0        0        0      219 2023-07-29 07:10:58.965822 prog_shojin_util-0.1.0/prog_shojin_util/utils/contest_sites/atcoder/matcher.py
--rw-r--r--   0        0        0     1150 2023-07-29 10:23:09.218461 prog_shojin_util-0.1.0/prog_shojin_util/utils/contest_sites/atcoder/parser.py
--rw-r--r--   0        0        0      852 2023-07-29 10:23:09.218461 prog_shojin_util-0.1.0/prog_shojin_util/utils/contest_sites/classifier.py
--rw-r--r--   0        0        0       37 2023-07-27 15:43:20.942318 prog_shojin_util-0.1.0/prog_shojin_util/utils/contest_sites/topcoder/__init__.py
--rw-r--r--   0        0        0      200 2023-07-29 10:23:09.218461 prog_shojin_util-0.1.0/prog_shojin_util/utils/contest_sites/topcoder/matcher.py
--rw-r--r--   0        0        0      104 2023-07-29 10:23:09.218461 prog_shojin_util-0.1.0/prog_shojin_util/utils/contest_sites/yukicoder/__init__.py
--rw-r--r--   0        0        0     1043 2023-07-29 10:23:09.218461 prog_shojin_util-0.1.0/prog_shojin_util/utils/contest_sites/yukicoder/api.py
--rw-r--r--   0        0        0      213 2023-07-29 10:23:09.218461 prog_shojin_util-0.1.0/prog_shojin_util/utils/contest_sites/yukicoder/matcher.py
--rw-r--r--   0        0        0      633 2023-07-29 10:23:09.218461 prog_shojin_util-0.1.0/prog_shojin_util/utils/contest_sites/yukicoder/parser.py
--rw-r--r--   0        0        0     1499 2023-07-30 03:34:39.777484 prog_shojin_util-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3665 1970-01-01 00:00:00.000000 prog_shojin_util-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-30 10:12:39.842214 prog_shojin_util-0.1.1/LICENSE
+-rw-r--r--   0        0        0     5959 2023-07-30 10:12:39.842214 prog_shojin_util-0.1.1/README.md
+-rw-r--r--   0        0        0      358 2023-07-30 10:12:57.230503 prog_shojin_util-0.1.1/prog_shojin_util/__init__.py
+-rw-r--r--   0        0        0       65 2023-07-30 10:12:39.842214 prog_shojin_util-0.1.1/prog_shojin_util/__main__.py
+-rw-r--r--   0        0        0     3100 2023-07-30 10:12:39.842214 prog_shojin_util-0.1.1/prog_shojin_util/cli.py
+-rw-r--r--   0        0        0      208 2023-07-30 10:12:39.842214 prog_shojin_util-0.1.1/prog_shojin_util/cli_config.py
+-rw-r--r--   0        0        0      304 2023-07-30 10:12:39.842214 prog_shojin_util-0.1.1/prog_shojin_util/logging_config.py
+-rw-r--r--   0        0        0        0 2023-07-30 10:12:39.842214 prog_shojin_util-0.1.1/prog_shojin_util/scraper/__init__.py
+-rw-r--r--   0        0        0     1313 2023-07-30 10:12:39.842214 prog_shojin_util-0.1.1/prog_shojin_util/scraper/link_collector.py
+-rw-r--r--   0        0        0     3190 2023-07-30 10:12:39.842214 prog_shojin_util-0.1.1/prog_shojin_util/services/output_formatter.py
+-rw-r--r--   0        0        0     1722 2023-07-30 10:12:39.842214 prog_shojin_util-0.1.1/prog_shojin_util/services/problem_finder.py
+-rw-r--r--   0        0        0        0 2023-07-30 10:12:39.842214 prog_shojin_util-0.1.1/prog_shojin_util/utils/__init__.py
+-rw-r--r--   0        0        0     1223 2023-07-30 10:12:39.842214 prog_shojin_util-0.1.1/prog_shojin_util/utils/cache.py
+-rw-r--r--   0        0        0     1373 2023-07-30 10:12:39.842214 prog_shojin_util-0.1.1/prog_shojin_util/utils/contest_site_factory.py
+-rw-r--r--   0        0        0      201 2023-07-30 10:12:39.842214 prog_shojin_util-0.1.1/prog_shojin_util/utils/contest_sites/__init__.py
+-rw-r--r--   0        0        0      119 2023-07-30 10:12:39.842214 prog_shojin_util-0.1.1/prog_shojin_util/utils/contest_sites/abstract/__init__.py
+-rw-r--r--   0        0        0      451 2023-07-30 10:12:39.842214 prog_shojin_util-0.1.1/prog_shojin_util/utils/contest_sites/abstract/api.py
+-rw-r--r--   0        0        0      447 2023-07-30 10:12:39.842214 prog_shojin_util-0.1.1/prog_shojin_util/utils/contest_sites/abstract/matcher.py
+-rw-r--r--   0        0        0      289 2023-07-30 10:12:39.842214 prog_shojin_util-0.1.1/prog_shojin_util/utils/contest_sites/abstract/parser.py
+-rw-r--r--   0        0        0     1388 2023-07-30 10:12:39.842214 prog_shojin_util-0.1.1/prog_shojin_util/utils/contest_sites/api_utils.py
+-rw-r--r--   0        0        0       98 2023-07-30 10:12:39.842214 prog_shojin_util-0.1.1/prog_shojin_util/utils/contest_sites/atcoder/__init__.py
+-rw-r--r--   0        0        0     3043 2023-07-30 10:12:39.842214 prog_shojin_util-0.1.1/prog_shojin_util/utils/contest_sites/atcoder/api.py
+-rw-r--r--   0        0        0      219 2023-07-30 10:12:39.842214 prog_shojin_util-0.1.1/prog_shojin_util/utils/contest_sites/atcoder/matcher.py
+-rw-r--r--   0        0        0     1150 2023-07-30 10:12:39.842214 prog_shojin_util-0.1.1/prog_shojin_util/utils/contest_sites/atcoder/parser.py
+-rw-r--r--   0        0        0      852 2023-07-30 10:12:39.842214 prog_shojin_util-0.1.1/prog_shojin_util/utils/contest_sites/classifier.py
+-rw-r--r--   0        0        0       37 2023-07-30 10:12:39.842214 prog_shojin_util-0.1.1/prog_shojin_util/utils/contest_sites/topcoder/__init__.py
+-rw-r--r--   0        0        0      200 2023-07-30 10:12:39.842214 prog_shojin_util-0.1.1/prog_shojin_util/utils/contest_sites/topcoder/matcher.py
+-rw-r--r--   0        0        0      104 2023-07-30 10:12:39.842214 prog_shojin_util-0.1.1/prog_shojin_util/utils/contest_sites/yukicoder/__init__.py
+-rw-r--r--   0        0        0     1043 2023-07-30 10:12:39.842214 prog_shojin_util-0.1.1/prog_shojin_util/utils/contest_sites/yukicoder/api.py
+-rw-r--r--   0        0        0      213 2023-07-30 10:12:39.842214 prog_shojin_util-0.1.1/prog_shojin_util/utils/contest_sites/yukicoder/matcher.py
+-rw-r--r--   0        0        0      633 2023-07-30 10:12:39.846214 prog_shojin_util-0.1.1/prog_shojin_util/utils/contest_sites/yukicoder/parser.py
+-rw-r--r--   0        0        0      208 2023-07-30 10:12:39.846214 prog_shojin_util-0.1.1/prog_shojin_util/utils/url_tools.py
+-rw-r--r--   0        0        0     1633 2023-07-30 10:12:57.230503 prog_shojin_util-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     7057 1970-01-01 00:00:00.000000 prog_shojin_util-0.1.1/PKG-INFO
```

### Comparing `prog_shojin_util-0.1.0/LICENSE` & `prog_shojin_util-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prog_shojin_util-0.1.0/prog_shojin_util/cli.py` & `prog_shojin_util-0.1.1/prog_shojin_util/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from datetime import datetime
 
 import click
 
+from prog_shojin_util.cli_config import CliConfig
 from prog_shojin_util.logging_config import setup_logging
 from prog_shojin_util.scraper.link_collector import LinkCollector
 from prog_shojin_util.services.output_formatter import OutputFormatter
 from prog_shojin_util.services.problem_finder import ProblemFinder
 
 
 @click.command(
@@ -35,18 +36,24 @@
     default="not-ac",
     show_default=True,
     help="Filter the problems based on their AC (Accepted) status. "
     "Choose 'ac' for solved problems, 'not-ac' for unsolved problems, and 'both' for all problems.",
 )
 @click.option(
     "--output",
-    type=click.Choice(["json", "markdown", "csv"]),
+    type=click.Choice(["json", "markdown", "csv", "acc_json"]),
     default="json",
     show_default=True,
-    help="Select the desired output format for the fetched problems. Available formats are JSON, Markdown, and CSV.",
+    help=(
+        "Select the output format: "
+        "JSON (Standard format), "
+        "Markdown (Export in Markdown), "
+        "CSV (Export in CSV), "
+        "acc_json (Format used by atcoder-cli tool)."
+    ),
 )
 @click.option(
     "--since",
     type=click.DateTime(),
     default="2012-01-01",
     help="Filter problems that were available since the specified date. "
     "Provide the date in 'YYYY-MM-DD' or 'YYYY-MM-DD HH:MM:SS' format. By default, it's set to 2012-01-01.",
@@ -62,32 +69,35 @@
     target,
     status,
     output,
     since,
     verbose,
 ):
     """Competitive Programming Utility Tool for Problems Fetching."""
-
     setup_logging(verbose)
 
+    cli_config = CliConfig(
+        atcoder_user=atcoder_user,
+        yukicoder_user=yukicoder_user,
+        target=target,
+        status=status,
+        output=output,
+        since=since,
+    )
+
     contest_user_data = [
-        ("Atcoder", atcoder_user),
-        ("Yukicoder", yukicoder_user),
+        ("Atcoder", cli_config.atcoder_user),
+        ("Yukicoder", cli_config.yukicoder_user),
     ]
 
     urls = LinkCollector(target).fetch_links()
     since = int(datetime.timestamp(since))
     results = {}  # {contest: [problems]}
 
+    # コンテストごとに問題を取得
     for contest, user in contest_user_data:
         finder = ProblemFinder(contest, urls)
         problems = finder.find_problems(user, status, since, True)
         results[contest] = problems
 
-    formatter = OutputFormatter(results)
-
-    if output == "json":
-        click.echo(formatter.to_json())
-    elif output == "markdown":
-        click.echo(formatter.to_markdown())
-    elif output == "csv":
-        click.echo(formatter.to_csv())
+    formatter = OutputFormatter(results, cli_config)
+    click.echo(formatter.display())
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `prog_shojin_util-0.1.0/prog_shojin_util/scraper/link_collector.py` & `prog_shojin_util-0.1.1/prog_shojin_util/scraper/link_collector.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from typing import Optional
 
 import requests
 from bs4 import BeautifulSoup
 
+from prog_shojin_util.utils.url_tools import clean_url
+
 
 class LinkCollector:
     def __init__(self, base_url: str):
         self.base_url = base_url
 
     def fetch_links(self) -> list[str]:
         content = self._fetch_content()
@@ -27,14 +29,18 @@
     def _extract_links(self, soup: BeautifulSoup) -> list[str]:
         link_elements = soup.find_all("a")
         links = [
             link.get("href") for link in link_elements if link.get("href") is not None
         ]
         return links
 
+    def _clean_links(self, links: list[str]) -> list[str]:
+        return [clean_url(link) for link in links]
+
     def fetch_links_from_file(self, file_path: str):
         with open(file_path, "r") as f:
             content = f.read()
 
         soup = BeautifulSoup(content, "html.parser")
         links = self._extract_links(soup)
-        return links
+        cleaned_links = self._clean_links(links)
+        return cleaned_links
```

### Comparing `prog_shojin_util-0.1.0/prog_shojin_util/services/problem_finder.py` & `prog_shojin_util-0.1.1/prog_shojin_util/services/problem_finder.py`

 * *Files identical despite different names*

### Comparing `prog_shojin_util-0.1.0/prog_shojin_util/utils/cache.py` & `prog_shojin_util-0.1.1/prog_shojin_util/utils/cache.py`

 * *Files identical despite different names*

### Comparing `prog_shojin_util-0.1.0/prog_shojin_util/utils/contest_site_factory.py` & `prog_shojin_util-0.1.1/prog_shojin_util/utils/contest_site_factory.py`

 * *Files identical despite different names*

### Comparing `prog_shojin_util-0.1.0/prog_shojin_util/utils/contest_sites/api_utils.py` & `prog_shojin_util-0.1.1/prog_shojin_util/utils/contest_sites/api_utils.py`

 * *Files identical despite different names*

### Comparing `prog_shojin_util-0.1.0/prog_shojin_util/utils/contest_sites/atcoder/api.py` & `prog_shojin_util-0.1.1/prog_shojin_util/utils/contest_sites/atcoder/api.py`

 * *Files identical despite different names*

### Comparing `prog_shojin_util-0.1.0/prog_shojin_util/utils/contest_sites/atcoder/parser.py` & `prog_shojin_util-0.1.1/prog_shojin_util/utils/contest_sites/atcoder/parser.py`

 * *Files identical despite different names*

### Comparing `prog_shojin_util-0.1.0/prog_shojin_util/utils/contest_sites/classifier.py` & `prog_shojin_util-0.1.1/prog_shojin_util/utils/contest_sites/classifier.py`

 * *Files identical despite different names*

### Comparing `prog_shojin_util-0.1.0/prog_shojin_util/utils/contest_sites/yukicoder/api.py` & `prog_shojin_util-0.1.1/prog_shojin_util/utils/contest_sites/yukicoder/api.py`

 * *Files identical despite different names*

### Comparing `prog_shojin_util-0.1.0/prog_shojin_util/utils/contest_sites/yukicoder/parser.py` & `prog_shojin_util-0.1.1/prog_shojin_util/utils/contest_sites/yukicoder/parser.py`

 * *Files identical despite different names*

### Comparing `prog_shojin_util-0.1.0/pyproject.toml` & `prog_shojin_util-0.1.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 [tool.poetry]
-name = "prog-shojin-util"
-version = "0.1.0"
+name = "prog_shojin_util"
+version = "0.1.1" # using poetry-dynamic-versioning
 description = "extracting and filtering problems from AtCoder, Yukicoder, and more."
 authors = ["Kazuya Isawa <torune.summer@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/edge2992/prog_shojin_util"
 packages = [{include = "prog_shojin_util"}]
 
 [tool.poetry.scripts]
-prog-shojin-util = "prog_shojin_util.__main__:main"
+pshu = "prog_shojin_util.__main__:main"
+
+[tool.poetry-dynamic-versioning]
+enable = false
+style = "pep440"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 click = "^8.1.6"
 beautifulsoup4 = "^4.12.2"
 requests = "^2.31.0"
 pandas = "^2.0.3"
@@ -53,9 +57,9 @@
 ignore_missing_imports = true
 check_untyped_defs = true
 warn_redundant_casts = true
 warn_unused_ignores = true
 strict_optional = true
 
 [build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
+build-backend = "poetry_dynamic_versioning.backend"
```

