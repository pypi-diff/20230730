# Comparing `tmp/heatmap_cli-0.2.1.tar.gz` & `tmp/heatmap_cli-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heatmap_cli-0.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "heatmap_cli-0.2.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `heatmap_cli-0.2.1.tar` & `heatmap_cli-0.2.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0      194 2023-07-26 03:15:34.005426 heatmap_cli-0.2.1/.coveragerc
--rw-r--r--   0        0        0     3101 2023-07-10 15:24:28.645268 heatmap_cli-0.2.1/.gitignore
--rw-r--r--   0        0        0     2589 2023-07-19 03:34:58.303707 heatmap_cli-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0       13 2023-07-10 15:24:28.645268 heatmap_cli-0.2.1/.prettierignore
--rw-r--r--   0        0        0       29 2023-07-10 15:24:28.645268 heatmap_cli-0.2.1/.python-version
--rw-r--r--   0        0        0     1570 2023-07-28 02:24:37.938195 heatmap_cli-0.2.1/CHANGELOG.md
--rw-r--r--   0        0        0     1967 2023-07-22 05:51:16.547471 heatmap_cli-0.2.1/CONTRIBUTING.md
--rw-r--r--   0        0        0    31956 2023-07-10 15:24:28.645268 heatmap_cli-0.2.1/LICENSE.md
--rw-r--r--   0        0        0      509 2023-07-21 00:25:50.551442 heatmap_cli-0.2.1/Pipfile
--rw-r--r--   0        0        0   126618 2023-07-24 03:36:11.870630 heatmap_cli-0.2.1/Pipfile.lock
--rw-r--r--   0        0        0     2154 2023-07-19 10:02:05.708726 heatmap_cli-0.2.1/README.md
--rw-r--r--   0        0        0      638 2023-07-10 15:24:28.645268 heatmap_cli-0.2.1/docs/Makefile
--rw-r--r--   0        0        0      804 2023-07-10 15:24:28.645268 heatmap_cli-0.2.1/docs/make.bat
-lrwxr-xr-x   0        0        0        0 2023-07-10 15:24:28.645268 heatmap_cli-0.2.1/docs/source/CHANGELOG.md -> ../../CHANGELOG.md
-lrwxr-xr-x   0        0        0        0 2023-07-10 15:24:28.645268 heatmap_cli-0.2.1/docs/source/CONTRIBUTING.md -> ../../CONTRIBUTING.md
-lrwxr-xr-x   0        0        0        0 2023-07-10 15:24:28.645268 heatmap_cli-0.2.1/docs/source/LICENSE.md -> ../../LICENSE.md
-lrwxr-xr-x   0        0        0        0 2023-07-10 15:24:28.645268 heatmap_cli-0.2.1/docs/source/README.md -> ../../README.md
--rw-r--r--   0        0        0    14202 2023-07-10 15:24:28.645268 heatmap_cli-0.2.1/docs/source/_static/logo.jpg
--rw-r--r--   0        0        0     1555 2023-07-10 15:24:28.645268 heatmap_cli-0.2.1/docs/source/conf.py
--rw-r--r--   0        0        0      172 2023-07-10 15:24:28.645268 heatmap_cli-0.2.1/docs/source/index.rst
--rw-r--r--   0        0        0      779 2023-07-28 02:24:49.394119 heatmap_cli-0.2.1/heatmap_cli/__init__.py
--rw-r--r--   0        0        0      837 2023-07-10 15:24:28.649268 heatmap_cli-0.2.1/heatmap_cli/__main__.py
--rw-r--r--   0        0        0     6921 2023-07-27 03:36:02.562136 heatmap_cli-0.2.1/heatmap_cli/cli.py
--rw-r--r--   0        0        0     1077 2023-07-17 23:52:03.000872 heatmap_cli-0.2.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-10 15:24:28.649268 heatmap_cli-0.2.1/tests/__init__.py
--rw-r--r--   0        0        0      845 2023-07-10 15:24:28.649268 heatmap_cli-0.2.1/tests/conftest.py
--rw-r--r--   0        0        0     5810 2023-07-10 15:24:28.649268 heatmap_cli-0.2.1/tests/fixtures/sample.csv
--rw-r--r--   0        0        0      358 2023-07-19 03:58:00.025209 heatmap_cli-0.2.1/tests/test_debug_flag.py
--rw-r--r--   0        0        0      326 2023-07-10 15:24:28.649268 heatmap_cli-0.2.1/tests/test_help_flag.py
--rw-r--r--   0        0        0      545 2023-07-10 15:24:28.649268 heatmap_cli-0.2.1/tests/test_verbose_flag.py
--rw-r--r--   0        0        0      306 2023-07-10 15:24:28.649268 heatmap_cli-0.2.1/tests/test_version_flag.py
--rw-r--r--   0        0        0      306 2023-07-19 23:00:14.071564 heatmap_cli-0.2.1/tests/test_week_flag.py
--rw-r--r--   0        0        0      516 2023-07-19 03:33:39.924975 heatmap_cli-0.2.1/tests/test_year_flag.py
--rw-r--r--   0        0        0      661 2023-07-26 03:15:49.357516 heatmap_cli-0.2.1/tox.ini
--rw-r--r--   0        0        0     3152 1970-01-01 00:00:00.000000 heatmap_cli-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      198 2023-07-29 11:03:01.033125 heatmap_cli-0.2.2/.coveragerc
+-rw-r--r--   0        0        0     3101 2023-07-10 15:24:28.645268 heatmap_cli-0.2.2/.gitignore
+-rw-r--r--   0        0        0     2589 2023-07-19 03:34:58.303707 heatmap_cli-0.2.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       13 2023-07-10 15:24:28.645268 heatmap_cli-0.2.2/.prettierignore
+-rw-r--r--   0        0        0       29 2023-07-10 15:24:28.645268 heatmap_cli-0.2.2/.python-version
+-rw-r--r--   0        0        0     1872 2023-07-30 05:28:45.121770 heatmap_cli-0.2.2/CHANGELOG.md
+-rw-r--r--   0        0        0     1967 2023-07-22 05:51:16.547471 heatmap_cli-0.2.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0    31956 2023-07-10 15:24:28.645268 heatmap_cli-0.2.2/LICENSE.md
+-rw-r--r--   0        0        0      509 2023-07-21 00:25:50.551442 heatmap_cli-0.2.2/Pipfile
+-rw-r--r--   0        0        0   126618 2023-07-24 03:36:11.870630 heatmap_cli-0.2.2/Pipfile.lock
+-rw-r--r--   0        0        0     2214 2023-07-29 11:33:39.226367 heatmap_cli-0.2.2/README.md
+-rw-r--r--   0        0        0      638 2023-07-10 15:24:28.645268 heatmap_cli-0.2.2/docs/Makefile
+-rw-r--r--   0        0        0      804 2023-07-10 15:24:28.645268 heatmap_cli-0.2.2/docs/make.bat
+lrwxr-xr-x   0        0        0        0 2023-07-10 15:24:28.645268 heatmap_cli-0.2.2/docs/source/CHANGELOG.md -> ../../CHANGELOG.md
+lrwxr-xr-x   0        0        0        0 2023-07-10 15:24:28.645268 heatmap_cli-0.2.2/docs/source/CONTRIBUTING.md -> ../../CONTRIBUTING.md
+lrwxr-xr-x   0        0        0        0 2023-07-10 15:24:28.645268 heatmap_cli-0.2.2/docs/source/LICENSE.md -> ../../LICENSE.md
+lrwxr-xr-x   0        0        0        0 2023-07-10 15:24:28.645268 heatmap_cli-0.2.2/docs/source/README.md -> ../../README.md
+-rw-r--r--   0        0        0    14202 2023-07-10 15:24:28.645268 heatmap_cli-0.2.2/docs/source/_static/logo.jpg
+-rw-r--r--   0        0        0     1555 2023-07-10 15:24:28.645268 heatmap_cli-0.2.2/docs/source/conf.py
+-rw-r--r--   0        0        0      172 2023-07-10 15:24:28.645268 heatmap_cli-0.2.2/docs/source/index.rst
+-rw-r--r--   0        0        0      779 2023-07-30 05:28:28.369639 heatmap_cli-0.2.2/heatmap_cli/__init__.py
+-rw-r--r--   0        0        0      837 2023-07-10 15:24:28.649268 heatmap_cli-0.2.2/heatmap_cli/__main__.py
+-rw-r--r--   0        0        0     8735 2023-07-29 12:52:57.238708 heatmap_cli-0.2.2/heatmap_cli/cli.py
+-rw-r--r--   0        0        0     1077 2023-07-17 23:52:03.000872 heatmap_cli-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-10 15:24:28.649268 heatmap_cli-0.2.2/tests/__init__.py
+-rw-r--r--   0        0        0      845 2023-07-10 15:24:28.649268 heatmap_cli-0.2.2/tests/conftest.py
+-rw-r--r--   0        0        0     5810 2023-07-10 15:24:28.649268 heatmap_cli-0.2.2/tests/fixtures/sample.csv
+-rw-r--r--   0        0        0      358 2023-07-19 03:58:00.025209 heatmap_cli-0.2.2/tests/test_debug_flag.py
+-rw-r--r--   0        0        0      326 2023-07-10 15:24:28.649268 heatmap_cli-0.2.2/tests/test_help_flag.py
+-rw-r--r--   0        0        0      545 2023-07-10 15:24:28.649268 heatmap_cli-0.2.2/tests/test_verbose_flag.py
+-rw-r--r--   0        0        0      306 2023-07-10 15:24:28.649268 heatmap_cli-0.2.2/tests/test_version_flag.py
+-rw-r--r--   0        0        0      306 2023-07-19 23:00:14.071564 heatmap_cli-0.2.2/tests/test_week_flag.py
+-rw-r--r--   0        0        0      516 2023-07-19 03:33:39.924975 heatmap_cli-0.2.2/tests/test_year_flag.py
+-rw-r--r--   0        0        0      678 2023-07-29 11:34:24.338632 heatmap_cli-0.2.2/tox.ini
+-rw-r--r--   0        0        0     3212 1970-01-01 00:00:00.000000 heatmap_cli-0.2.2/PKG-INFO
```

### Comparing `heatmap_cli-0.2.1/.gitignore` & `heatmap_cli-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.2.1/.pre-commit-config.yaml` & `heatmap_cli-0.2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.2.1/CHANGELOG.md` & `heatmap_cli-0.2.2/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,22 +3,38 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [0-based versioning](https://0ver.org/).
 
 ## [Unreleased]
 
+## v0.2.2 (2023-07-30)
+
+### Added
+
+- Add changelog url to help message
+- Add missing documentation for functions
+
+### Changed
+
+- Set title and png filename to year only when week is set to 52
+
+### Fixed
+
+- Fix incorrect header level in changelog
+- Fix incorrect source module in coverage config file
+
 ## v0.2.1 (2023-07-28)
 
 ### Changed
 
 - Move `coverage` config from `tox` to its own file
 - Reset Dataframe index after filtering
 
-## Fixed
+### Fixed
 
 - Show verbose log of last date of current week
 - Fix incorrect header level in changelog
 
 ## v0.2.0 (2023-07-23)
 
 ### Added
```

### Comparing `heatmap_cli-0.2.1/CONTRIBUTING.md` & `heatmap_cli-0.2.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.2.1/LICENSE.md` & `heatmap_cli-0.2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.2.1/Pipfile.lock` & `heatmap_cli-0.2.2/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.2.1/README.md` & `heatmap_cli-0.2.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -31,21 +31,22 @@
 ```console
 usage: heatmap_cli [-yr YEAR] [-wk WEEK] [-d] [-v] [-h] [-V] CSV_FILENAME
 
 A console program that generates yearly calendar heatmap.
 
   website: https://github.com/kianmeng/heatmap_cli
   issues: https://github.com/kianmeng/heatmap_cli/issues
+  changelog: https://github.com/kianmeng/heatmap_cli/issues
 
 positional arguments:
   CSV_FILENAME           csv filename
 
 optional arguments:
   -yr YEAR, --year YEAR  filter by year from the CSV file (default: '2023')
-  -wk WEEK, --week WEEK  filter until week of the year from the CSV file (default: '29')
+  -wk WEEK, --week WEEK  filter until week of the year from the CSV file (default: '30')
   -d, --debug            show debugging log and stacktrace
   -v, --verbose          show verbosity of debugging log, use -vv, -vvv for more details
   -h, --help             show this help message and exit
   -V, --version          show program's version number and exit
 ```
 
 ## Copyright and License
```

### Comparing `heatmap_cli-0.2.1/docs/Makefile` & `heatmap_cli-0.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.2.1/docs/make.bat` & `heatmap_cli-0.2.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.2.1/docs/source/_static/logo.jpg` & `heatmap_cli-0.2.2/docs/source/_static/logo.jpg`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.2.1/docs/source/conf.py` & `heatmap_cli-0.2.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.2.1/heatmap_cli/__init__.py` & `heatmap_cli-0.2.2/heatmap_cli/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <https://www.gnu.org/licenses/>.
 
 """A console program that generates yearly calendar heatmap."""
 
-__version__ = "0.2.1"
+__version__ = "0.2.2"
```

### Comparing `heatmap_cli-0.2.1/heatmap_cli/__main__.py` & `heatmap_cli-0.2.2/heatmap_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.2.1/heatmap_cli/cli.py` & `heatmap_cli-0.2.2/heatmap_cli/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 """A console program that generates yearly calendar heatmap.
 
   website: https://github.com/kianmeng/heatmap_cli
   issues: https://github.com/kianmeng/heatmap_cli/issues
+  changelog: https://github.com/kianmeng/heatmap_cli/issues
 """
 
 import argparse
 import datetime
 import logging
 import sys
 from typing import Dict, Optional, Sequence
@@ -36,15 +37,22 @@
 logging.getLogger("matplotlib").propagate = False
 _logger = logging.getLogger(__name__)
 
 
 def _build_parser(
     _args: Optional[Sequence[str]] = None,
 ) -> argparse.ArgumentParser:
-    """Build the CLI parser."""
+    """Build the CLI parser.
+
+    Args:
+        _args (List | None): Argument passed through the command line
+
+    Returns:
+        parser (argparse.ArgumentParser)
+    """
     parser = argparse.ArgumentParser(
         add_help=False,
         description=__doc__,
         formatter_class=lambda prog: argparse.RawTextHelpFormatter(
             prog,
             max_help_position=25,
         ),
@@ -110,15 +118,22 @@
         "-V", "--version", action="version", version=f"%(prog)s {__version__}"
     )
 
     return parser
 
 
 def _setup_logging(debug: bool = False) -> None:
-    """Set up logging by level."""
+    """Set up logging by level.
+
+    Args:
+        debug (boolean): Whether to toggle debugging logs
+
+    Returns:
+        None
+    """
     conf: Dict = {
         True: {
             "level": logging.DEBUG,
             "msg": "[%(asctime)s] %(levelname)s: %(name)s: %(message)s",
         },
         False: {"level": logging.INFO, "msg": "%(message)s"},
     }
@@ -128,58 +143,82 @@
         stream=sys.stdout,
         format=conf[debug]["msg"],
         datefmt="%Y-%m-%d %H:%M:%S",
     )
 
 
 def _massage_data(config: argparse.Namespace) -> pd.core.frame.DataFrame:
+    """Filter the data from CSV file.
+
+    Args:
+        config (argparse.Namespace): Config from command line arguments
+
+    Returns:
+        dataframe (pd.core.frameDataFrame): Filtered Dataframe
+    """
     dataframe = pd.read_csv(
         config.input_filename, header=None, names=["date", "count"]
     )
     dataframe["date"] = pd.to_datetime(dataframe["date"])
     dataframe["weekday"] = dataframe["date"].dt.weekday + 1
     dataframe["week"] = dataframe["date"].dt.strftime("%W")
     dataframe["count"] = round(dataframe["count"], -2) / 100
 
-    steps = dataframe[
-        (dataframe["date"].dt.year == config.year)
-        & (dataframe["week"] <= str(config.week).zfill(2))
-    ]
-    steps.reset_index(drop=True, inplace=True)
+    if config.week == 52:
+        steps = dataframe[dataframe["date"].dt.year == config.year]
+    else:
+        steps = dataframe[
+            (dataframe["date"].dt.year == config.year)
+            & (dataframe["week"] <= str(config.week).zfill(2))
+        ]
 
     if steps.empty:
         raise ValueError("no data extracted from csv file")
 
     _logger.debug(
         "last date: %s of current week: %s",
         max(steps["date"]).date(),
         config.week,
     )
-    missing_df = pd.DataFrame(
+    missing_steps = pd.DataFrame(
         {
             "date": pd.date_range(
                 start=max(steps["date"]).date() + datetime.timedelta(days=1),
                 end=f"{config.year}-12-31",
             )
         }
     )
-    missing_df["weekday"] = missing_df["date"].dt.weekday + 1
-    missing_df["week"] = missing_df["date"].dt.strftime("%W")
-    missing_df["count"] = 0
+    missing_steps["weekday"] = missing_steps["date"].dt.weekday + 1
+    missing_steps["week"] = missing_steps["date"].dt.strftime("%W")
+    missing_steps["count"] = 0
+
+    if not missing_steps.empty:
+        steps = pd.concat([steps, missing_steps], ignore_index=True)
+
+    steps.reset_index(drop=True, inplace=True)
 
-    steps = pd.concat([steps, missing_df], ignore_index=True)
     year_dataframe = steps.pivot_table(
         values="count", index=["weekday"], columns=["week"], fill_value=0
     )
     return year_dataframe
 
 
 def _generate_heatmap(
     config: argparse.Namespace, dataframe: pd.core.frame.DataFrame
 ) -> None:
+    """Generate a heatmap in PNG file.
+
+    Args:
+        config (argparse.Namespace): Config from command line arguments
+        dataframe (pd.core.frameDataFrame): Dataframe with data loaded from CSV
+        file
+
+    Returns:
+        None
+    """
     # generating matplotlib graphs without a x-server
     # see http://stackoverflow.com/a/4935945
     mpl.use("Agg")
 
     cmap = "RdYlGn_r"
     _fig, axis = plt.subplots(figsize=(8, 5))
     axis.tick_params(axis="both", which="major", labelsize=9)
@@ -196,50 +235,84 @@
         cbar_kws={
             "orientation": "horizontal",
             "label": f"colourmap: {cmap}, count: by hundred",
             "pad": 0.15,
         },
     )
 
-    png_filename = (
-        f"{config.year}_week_{config.week}_{cmap}"
-        "_annotated_heatmap_of_total_daily_walked_steps.png"
-    )
-
-    plt.title(
-        (
-            "Total Daily Walking Steps Count Up to Week "
-            f"{config.week} {config.year} (kianmeng.org)"
-        ),
-        fontsize=10,
-    )
+    png_filename = _generate_filename(config, cmap)
+    plt.title(_generate_title(config), fontsize=10)
     plt.tight_layout()
     plt.savefig(
         png_filename,
         bbox_inches="tight",
         transparent=False,
         dpi=76,
     )
     _logger.info("generate heatmap png file: %s", png_filename)
 
 
+def _generate_filename(config: argparse.Namespace, cmap: str) -> str:
+    """Generate a PNG filename.
+
+    Args:
+        config (argparse.Namespace): Config from command line arguments
+
+    Returns:
+        str: A generated file name for the PNG image
+    """
+    filename = "_annotated_heatmap_of_total_daily_walked_steps_count.png"
+    if config.week == 52:
+        return f"{config.year}_{cmap}_" + filename
+
+    return f"{config.year}_week_{config.week}_{cmap}_" + filename
+
+
+def _generate_title(config: argparse.Namespace) -> str:
+    """Run the main flow.
+
+    Args:
+        config (argparse.Namespace): Config from command line arguments
+
+    Returns:
+        str: A generated title for the heatmap title
+    """
+    title = "Total Daily Walking Steps Count "
+    if config.week == 52:
+        return title + f"for the Year {config.year} (kianmeng.org)"
+
+    return (
+        title
+        + f"Up to Week {config.week} for the Year {config.year} (kianmeng.org)"
+    )
+
+
 def _run(config: argparse.Namespace) -> None:
     """Run the main flow.
 
     Args:
-        config (argparse.Namespace): Config from command line arguments or
-        config file.
+        config (argparse.Namespace): Config from command line arguments
+
+    Returns:
+        None
     """
     _logger.debug(config)
     dataframe = _massage_data(config)
     _generate_heatmap(config, dataframe)
 
 
 def main(args: Optional[Sequence[str]] = None) -> None:
-    """Run the main program flow."""
+    """Run the main program flow.
+
+    Args:
+        args (List | None): Argument passed through the command line
+
+    Returns:
+        None
+    """
     try:
         parser = _build_parser(args)
         parsed_args = parser.parse_args(args)
         _setup_logging(parsed_args.debug)
         _run(parsed_args)
     except Exception as error:
         _logger.error(
```

### Comparing `heatmap_cli-0.2.1/pyproject.toml` & `heatmap_cli-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.2.1/tests/conftest.py` & `heatmap_cli-0.2.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.2.1/tests/fixtures/sample.csv` & `heatmap_cli-0.2.2/tests/fixtures/sample.csv`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.2.1/tests/test_verbose_flag.py` & `heatmap_cli-0.2.2/tests/test_verbose_flag.py`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.2.1/tests/test_year_flag.py` & `heatmap_cli-0.2.2/tests/test_year_flag.py`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.2.1/tox.ini` & `heatmap_cli-0.2.2/tox.ini`

 * *Files 16% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     pipenv run pytest tests
 
 [testenv:cov]
 description = generate code coverage report in html
 deps = pipenv
 commands=
     pipenv install --dev
-    pipenv run pytest tests --numprocesses auto --cov=heatmap_cli --cov-report term-missing --cov-report html {toxinidir}/tests
+    pipenv run pytest tests --numprocesses auto --cov=heatmap_cli --cov-config=.coveragerc --cov-report term --cov-report html {toxinidir}/tests
 
 [testenv:doc]
 description = generate sphinx documentation in html
 basepython = python3.11
 deps = pipenv
 commands =
     pipenv install --categories doc
```

### Comparing `heatmap_cli-0.2.1/PKG-INFO` & `heatmap_cli-0.2.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heatmap_cli
-Version: 0.2.1
+Version: 0.2.2
 Summary: A console program that generates yearly calendar heatmap.
 Keywords: heatmap,cli
 Author-email: Kian-Meng Ang <kianmeng@cpan.org>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
@@ -54,21 +54,22 @@
 ```console
 usage: heatmap_cli [-yr YEAR] [-wk WEEK] [-d] [-v] [-h] [-V] CSV_FILENAME
 
 A console program that generates yearly calendar heatmap.
 
   website: https://github.com/kianmeng/heatmap_cli
   issues: https://github.com/kianmeng/heatmap_cli/issues
+  changelog: https://github.com/kianmeng/heatmap_cli/issues
 
 positional arguments:
   CSV_FILENAME           csv filename
 
 optional arguments:
   -yr YEAR, --year YEAR  filter by year from the CSV file (default: '2023')
-  -wk WEEK, --week WEEK  filter until week of the year from the CSV file (default: '29')
+  -wk WEEK, --week WEEK  filter until week of the year from the CSV file (default: '30')
   -d, --debug            show debugging log and stacktrace
   -v, --verbose          show verbosity of debugging log, use -vv, -vvv for more details
   -h, --help             show this help message and exit
   -V, --version          show program's version number and exit
 ```
 
 ## Copyright and License
```

