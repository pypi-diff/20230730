# Comparing `tmp/statute_utils-0.6.2.tar.gz` & `tmp/statute_utils-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statute_utils-0.6.2.tar", max compression
+gzip compressed data, was "statute_utils-0.6.3.tar", max compression
```

## Comparing `statute_utils-0.6.2.tar` & `statute_utils-0.6.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1491 2023-06-21 15:08:07.621911 statute_utils-0.6.2/LICENSE
--rw-r--r--   0        0        0     2640 2023-07-16 05:44:56.640061 statute_utils-0.6.2/README.md
--rw-r--r--   0        0        0     1357 2023-07-29 18:31:00.746124 statute_utils-0.6.2/pyproject.toml
--rw-r--r--   0        0        0      897 2023-07-29 18:29:16.464915 statute_utils-0.6.2/statute_utils/__init__.py
--rw-r--r--   0        0        0     3035 2023-07-29 18:21:42.065621 statute_utils-0.6.2/statute_utils/codification.py
--rw-r--r--   0        0        0      588 2023-07-16 08:01:39.314430 statute_utils-0.6.2/statute_utils/components/__init__.py
--rw-r--r--   0        0        0     6011 2023-07-29 18:29:59.938432 statute_utils-0.6.2/statute_utils/components/branch.py
--rw-r--r--   0        0        0     8323 2023-07-16 08:01:53.752165 statute_utils-0.6.2/statute_utils/components/builder.py
--rw-r--r--   0        0        0    11357 2023-07-28 03:46:47.927866 statute_utils-0.6.2/statute_utils/components/category.py
--rw-r--r--   0        0        0     2015 2023-07-01 04:37:03.664929 statute_utils-0.6.2/statute_utils/components/short.py
--rw-r--r--   0        0        0     3717 2023-07-16 05:41:42.450594 statute_utils-0.6.2/statute_utils/components/utils.py
--rw-r--r--   0        0        0     1288 2023-07-17 01:57:30.575440 statute_utils-0.6.2/statute_utils/config.py
--rw-r--r--   0        0        0     9858 2023-07-17 02:00:05.382207 statute_utils-0.6.2/statute_utils/main.py
--rw-r--r--   0        0        0     4170 2023-07-17 01:57:45.971391 statute_utils-0.6.2/statute_utils/models.py
--rw-r--r--   0        0        0     9892 2023-07-02 03:43:37.827535 statute_utils-0.6.2/statute_utils/models_names.py
--rw-r--r--   0        0        0     6699 2023-07-02 03:43:23.216281 statute_utils-0.6.2/statute_utils/models_serials.py
--rw-r--r--   0        0        0      249 2023-07-01 04:12:57.597987 statute_utils-0.6.2/statute_utils/recipes/__init__.py
--rw-r--r--   0        0        0      380 2023-06-22 05:28:27.922298 statute_utils-0.6.2/statute_utils/recipes/const.py
--rw-r--r--   0        0        0     2649 2023-06-22 05:28:27.922412 statute_utils-0.6.2/statute_utils/recipes/digits.py
--rw-r--r--   0        0        0      311 2023-06-22 05:28:27.922524 statute_utils-0.6.2/statute_utils/recipes/roc.py
--rw-r--r--   0        0        0      667 2023-06-22 05:28:27.922641 statute_utils-0.6.2/statute_utils/recipes/spain.py
--rw-r--r--   0        0        0     6640 2023-07-29 17:46:52.576680 statute_utils-0.6.2/statute_utils/statute.py
--rw-r--r--   0        0        0     1851 2023-07-16 08:51:22.676004 statute_utils-0.6.2/statute_utils/templater.py
--rw-r--r--   0        0        0      208 2023-07-16 07:34:21.108245 statute_utils-0.6.2/statute_utils/templates/crumbs.html
--rw-r--r--   0        0        0      164 2023-07-16 07:29:47.336036 statute_utils-0.6.2/statute_utils/templates/paragraph.html
--rw-r--r--   0        0        0      200 2023-07-16 07:34:28.065021 statute_utils-0.6.2/statute_utils/templates/subtree.html
--rw-r--r--   0        0        0     1117 2023-07-16 09:00:07.666662 statute_utils-0.6.2/statute_utils/templates/tree.css
--rw-r--r--   0        0        0     2416 2023-07-16 08:50:40.061466 statute_utils-0.6.2/statute_utils/templates/tree.html
--rw-r--r--   0        0        0     3567 1970-01-01 00:00:00.000000 statute_utils-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1491 2023-06-21 15:08:07.621911 statute_utils-0.6.3/LICENSE
+-rw-r--r--   0        0        0     2640 2023-07-16 05:44:56.640061 statute_utils-0.6.3/README.md
+-rw-r--r--   0        0        0     1357 2023-07-30 01:35:38.594836 statute_utils-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0      897 2023-07-29 18:29:16.464915 statute_utils-0.6.3/statute_utils/__init__.py
+-rw-r--r--   0        0        0     3113 2023-07-30 00:42:26.232929 statute_utils-0.6.3/statute_utils/codification.py
+-rw-r--r--   0        0        0      588 2023-07-16 08:01:39.314430 statute_utils-0.6.3/statute_utils/components/__init__.py
+-rw-r--r--   0        0        0     6011 2023-07-29 18:29:59.938432 statute_utils-0.6.3/statute_utils/components/branch.py
+-rw-r--r--   0        0        0     8323 2023-07-16 08:01:53.752165 statute_utils-0.6.3/statute_utils/components/builder.py
+-rw-r--r--   0        0        0    12717 2023-07-30 01:34:15.178955 statute_utils-0.6.3/statute_utils/components/category.py
+-rw-r--r--   0        0        0     2015 2023-07-01 04:37:03.664929 statute_utils-0.6.3/statute_utils/components/short.py
+-rw-r--r--   0        0        0     3717 2023-07-16 05:41:42.450594 statute_utils-0.6.3/statute_utils/components/utils.py
+-rw-r--r--   0        0        0     1288 2023-07-17 01:57:30.575440 statute_utils-0.6.3/statute_utils/config.py
+-rw-r--r--   0        0        0     9858 2023-07-17 02:00:05.382207 statute_utils-0.6.3/statute_utils/main.py
+-rw-r--r--   0        0        0     4170 2023-07-17 01:57:45.971391 statute_utils-0.6.3/statute_utils/models.py
+-rw-r--r--   0        0        0     9892 2023-07-02 03:43:37.827535 statute_utils-0.6.3/statute_utils/models_names.py
+-rw-r--r--   0        0        0     6699 2023-07-02 03:43:23.216281 statute_utils-0.6.3/statute_utils/models_serials.py
+-rw-r--r--   0        0        0      249 2023-07-01 04:12:57.597987 statute_utils-0.6.3/statute_utils/recipes/__init__.py
+-rw-r--r--   0        0        0      380 2023-06-22 05:28:27.922298 statute_utils-0.6.3/statute_utils/recipes/const.py
+-rw-r--r--   0        0        0     2649 2023-06-22 05:28:27.922412 statute_utils-0.6.3/statute_utils/recipes/digits.py
+-rw-r--r--   0        0        0      311 2023-06-22 05:28:27.922524 statute_utils-0.6.3/statute_utils/recipes/roc.py
+-rw-r--r--   0        0        0      667 2023-06-22 05:28:27.922641 statute_utils-0.6.3/statute_utils/recipes/spain.py
+-rw-r--r--   0        0        0     6696 2023-07-30 01:34:59.725837 statute_utils-0.6.3/statute_utils/statute.py
+-rw-r--r--   0        0        0     1851 2023-07-16 08:51:22.676004 statute_utils-0.6.3/statute_utils/templater.py
+-rw-r--r--   0        0        0      208 2023-07-16 07:34:21.108245 statute_utils-0.6.3/statute_utils/templates/crumbs.html
+-rw-r--r--   0        0        0      164 2023-07-16 07:29:47.336036 statute_utils-0.6.3/statute_utils/templates/paragraph.html
+-rw-r--r--   0        0        0      200 2023-07-16 07:34:28.065021 statute_utils-0.6.3/statute_utils/templates/subtree.html
+-rw-r--r--   0        0        0     1117 2023-07-16 09:00:07.666662 statute_utils-0.6.3/statute_utils/templates/tree.css
+-rw-r--r--   0        0        0     2416 2023-07-16 08:50:40.061466 statute_utils-0.6.3/statute_utils/templates/tree.html
+-rw-r--r--   0        0        0     3567 1970-01-01 00:00:00.000000 statute_utils-0.6.3/PKG-INFO
```

### Comparing `statute_utils-0.6.2/LICENSE` & `statute_utils-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.2/README.md` & `statute_utils-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.2/pyproject.toml` & `statute_utils-0.6.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "statute-utils"
-version = "0.6.2"
+version = "0.6.3"
 description = "Philippine statutory law pattern matching and unit retrieval."
 authors = ["Marcelino G. Veloso III <contact@mv3.dev>"]
 readme = "README.md"
 homepage = "https://lawsql.com"
 repository = "https://github.com/justmars/statute-utils"
 documentation = "https://justmars.github.io/statute-utils"
 classifiers = [
```

### Comparing `statute_utils-0.6.2/statute_utils/__init__.py` & `statute_utils-0.6.3/statute_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.2/statute_utils/codification.py` & `statute_utils-0.6.3/statute_utils/codification.py`

 * *Files 6% similar despite different names*

```diff
@@ -74,14 +74,16 @@
 
     def make_row(self) -> dict:
         """See same logic in Statute."""
         set_node_ids(self.units)
         units = [{"id": "1.", "units": self.units}]
         return {
             "id": self.slug,
+            "title": self.title,
+            "description": self.description,
             "cat": self.rule.cat.value,
             "num": self.rule.num,
             "date": self.date,
             "units": units,
             "html": html_tree_from_hierarchy(units),
         }
```

### Comparing `statute_utils-0.6.2/statute_utils/components/__init__.py` & `statute_utils-0.6.3/statute_utils/components/__init__.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.2/statute_utils/components/branch.py` & `statute_utils-0.6.3/statute_utils/components/branch.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.2/statute_utils/components/builder.py` & `statute_utils-0.6.3/statute_utils/components/builder.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.2/statute_utils/components/category.py` & `statute_utils-0.6.3/statute_utils/components/category.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,29 +8,32 @@
     A Rule in the Philippines involves various denominations.
     It can be referred to by its
 
     1. `official` title
     2. `serial` title
     3. `short` title
     4. `alias` titles
+    4. `searchable` titles
 
     Consider something like the _Maceda Law_ which can be dissected as follows:
 
     Category | Mandatory | Nature | Description | Example | Matching Strategy
     --:|:--:|:--:|:--|:--|--:
     `official` | yes | official | full length title | _AN ACT TO PROVIDE PROTECTION TO BUYERS OF REAL ESTATE ON INSTALLMENT PAYMENTS_ | [Statute Details][statute-details]
     `serial` | yes | official | [`Statute Category`][statute-category-model] + serial identifier. | _Republic Act No. 6552_ | [Serial Pattern][serial-pattern] regex matching
     `short`  | no | official | may be declared in body of statute | _Realty Installment Buyer Act_ | [A helper function ][extract-short-title]
     `alias`  | no | unofficial | popular, undocumented means of referring to a statute | _Maceda Law_ | [Named Pattern][named-pattern] regex matching
+    `searchables`  | no | unofficial | easy way for users to reference via search | ra 6552 | --
     """  # noqa: E501
 
     Official = auto()
     Serial = auto()
     Alias = auto()
     Short = auto()
+    Searchable = auto()
 
 
 class StatuteSerialCategory(StrEnum):
     """
     It would be difficult to identify rules if they were arbitrarily named
     without a fixed point of reference. For instance the _Civil Code of the
     Philippines_,  an arbitrary collection of letters, would be hard to find
@@ -207,14 +210,39 @@
                     )
 
             case _:
                 # no need to uppercase pure digits
                 target_digit = idx if idx.isdigit() else idx.upper()
                 return f"{uncamel(self)} No. {target_digit}"
 
+    def searchable(self, num: str) -> str:
+        """Given the value `<v>` of a category (lowercased, as saved in the database),
+        use `StatuteSerialCategory(<v>)`. This will get the proper category. Use the
+        category alongside the passed `num`.
+
+        Examples:
+            >>> civ = StatuteSerialCategory('ra')
+            >>> civ.searchable('386')
+            'ra 386'
+            >>> civ = StatuteSerialCategory('rule_am')
+            >>> civ.searchable('00-2-03-sc')
+            'am 00-2-03-sc'
+        """
+        match self:
+            case StatuteSerialCategory.AdministrativeMatter:
+                return f"am {num}"
+            case StatuteSerialCategory.BarMatter:
+                return f"bm {num}"
+            case StatuteSerialCategory.CircularOCA:
+                return f"oca cir {num}"
+            case StatuteSerialCategory.CircularSC:
+                return f"sc cir {num}"
+            case _:
+                return f"{self.value} {num}"
+
     def cite(self, num: str) -> str | None:
         """Given the value `<v>` of a category (lowercased, as saved in the database),
         use `StatuteSerialCategory(<v>)`. This will get the proper category. Use the
         category alongside the passed `num`.
 
         Examples:
             >>> civ = StatuteSerialCategory('ra')
@@ -277,21 +305,27 @@
     @classmethod
     def generate(
         cls,
         official: str | None = None,
         serial: str | None = None,
         short: str | None = None,
         aliases: list[str] | None = None,
+        searchables: list[str] | None = None,
     ):
         if official:
             yield cls(category=StatuteTitleCategory.Official, text=official)
 
         if serial:
             yield cls(category=StatuteTitleCategory.Serial, text=serial)
 
         if aliases:
             for title in aliases:
                 if title and title != "":
                     yield cls(category=StatuteTitleCategory.Alias, text=title)
 
+        if searchables:
+            for title in searchables:
+                if title and title != "":
+                    yield cls(category=StatuteTitleCategory.Searchable, text=title)
+
         if short:
             yield cls(category=StatuteTitleCategory.Short, text=short)
```

### Comparing `statute_utils-0.6.2/statute_utils/components/short.py` & `statute_utils-0.6.3/statute_utils/components/short.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.2/statute_utils/components/utils.py` & `statute_utils-0.6.3/statute_utils/components/utils.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.2/statute_utils/config.py` & `statute_utils-0.6.3/statute_utils/config.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.2/statute_utils/main.py` & `statute_utils-0.6.3/statute_utils/main.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.2/statute_utils/models.py` & `statute_utils-0.6.3/statute_utils/models.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.2/statute_utils/models_names.py` & `statute_utils-0.6.3/statute_utils/models_names.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.2/statute_utils/models_serials.py` & `statute_utils-0.6.3/statute_utils/models_serials.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.2/statute_utils/recipes/digits.py` & `statute_utils-0.6.3/statute_utils/recipes/digits.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.2/statute_utils/recipes/spain.py` & `statute_utils-0.6.3/statute_utils/recipes/spain.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.2/statute_utils/statute.py` & `statute_utils-0.6.3/statute_utils/statute.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,15 @@
     walk,
 )
 from .models import Rule
 from .templater import html_tree_from_hierarchy
 
 
 class Statute(NamedTuple):
-    """A instance is dependent on a specifically
-    formatted statute Path.
+    """A instance is dependent on a specifically formatted statute Path.
 
     The shape of the contents will be different
     from the shape of the dumpable `.yml` export."""
 
     titles: list[StatuteTitle]
     rule: Rule
     variant: int
@@ -178,10 +177,11 @@
             units=data.get("units"),
             titles=list(
                 StatuteTitle.generate(
                     official=official,
                     serial=serial,
                     short=data.get("short"),
                     aliases=data.get("aliases"),
+                    searchables=[category.searchable(num)],
                 )
             ),
         )
```

### Comparing `statute_utils-0.6.2/statute_utils/templater.py` & `statute_utils-0.6.3/statute_utils/templater.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.2/statute_utils/templates/tree.css` & `statute_utils-0.6.3/statute_utils/templates/tree.css`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.2/statute_utils/templates/tree.html` & `statute_utils-0.6.3/statute_utils/templates/tree.html`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.2/PKG-INFO` & `statute_utils-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statute-utils
-Version: 0.6.2
+Version: 0.6.3
 Summary: Philippine statutory law pattern matching and unit retrieval.
 Home-page: https://lawsql.com
 Author: Marcelino G. Veloso III
 Author-email: contact@mv3.dev
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
```

