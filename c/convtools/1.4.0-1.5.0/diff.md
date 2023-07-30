# Comparing `tmp/convtools-1.4.0.tar.gz` & `tmp/convtools-1.5.0.tar.gz`

## Comparing `convtools-1.4.0.tar` & `convtools-1.5.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 convtools-1.4.0/convtools/__init__.py
--rw-r--r--   0        0        0    51224 2020-02-02 00:00:00.000000 convtools-1.4.0/convtools/_aggregations.py
--rw-r--r--   0        0        0   108078 2020-02-02 00:00:00.000000 convtools-1.4.0/convtools/_base.py
--rw-r--r--   0        0        0     7609 2020-02-02 00:00:00.000000 convtools-1.4.0/convtools/_chunks.py
--rw-r--r--   0        0        0     5696 2020-02-02 00:00:00.000000 convtools-1.4.0/convtools/_columns.py
--rw-r--r--   0        0        0     5538 2020-02-02 00:00:00.000000 convtools-1.4.0/convtools/_conversion.py
--rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 convtools-1.4.0/convtools/_cumulative.py
--rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 convtools-1.4.0/convtools/_debug.py
--rw-r--r--   0        0        0    20223 2020-02-02 00:00:00.000000 convtools-1.4.0/convtools/_dt.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 convtools-1.4.0/convtools/_expect.py
--rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 convtools-1.4.0/convtools/_heuristics.py
--rw-r--r--   0        0        0    17783 2020-02-02 00:00:00.000000 convtools-1.4.0/convtools/_joins.py
--rw-r--r--   0        0        0     5947 2020-02-02 00:00:00.000000 convtools-1.4.0/convtools/_mutations.py
--rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 convtools-1.4.0/convtools/_unique.py
--rw-r--r--   0        0        0     8584 2020-02-02 00:00:00.000000 convtools-1.4.0/convtools/_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 convtools-1.4.0/convtools/contrib/__init__.py
--rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 convtools-1.4.0/convtools/contrib/fs.py
--rw-r--r--   0        0        0    34670 2020-02-02 00:00:00.000000 convtools-1.4.0/convtools/contrib/tables.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 convtools-1.4.0/.gitignore
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 convtools-1.4.0/LICENSE.txt
--rw-r--r--   0        0        0     4162 2020-02-02 00:00:00.000000 convtools-1.4.0/README.md
--rw-r--r--   0        0        0     2473 2020-02-02 00:00:00.000000 convtools-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     7729 2020-02-02 00:00:00.000000 convtools-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 convtools-1.5.0/convtools/__init__.py
+-rw-r--r--   0        0        0    51318 2020-02-02 00:00:00.000000 convtools-1.5.0/convtools/_aggregations.py
+-rw-r--r--   0        0        0   109878 2020-02-02 00:00:00.000000 convtools-1.5.0/convtools/_base.py
+-rw-r--r--   0        0        0     7601 2020-02-02 00:00:00.000000 convtools-1.5.0/convtools/_chunks.py
+-rw-r--r--   0        0        0     5598 2020-02-02 00:00:00.000000 convtools-1.5.0/convtools/_columns.py
+-rw-r--r--   0        0        0     5651 2020-02-02 00:00:00.000000 convtools-1.5.0/convtools/_conversion.py
+-rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 convtools-1.5.0/convtools/_cumulative.py
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 convtools-1.5.0/convtools/_debug.py
+-rw-r--r--   0        0        0    35610 2020-02-02 00:00:00.000000 convtools-1.5.0/convtools/_dt.py
+-rw-r--r--   0        0        0     3484 2020-02-02 00:00:00.000000 convtools-1.5.0/convtools/_exceptions.py
+-rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 convtools-1.5.0/convtools/_expect.py
+-rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 convtools-1.5.0/convtools/_heuristics.py
+-rw-r--r--   0        0        0    17648 2020-02-02 00:00:00.000000 convtools-1.5.0/convtools/_joins.py
+-rw-r--r--   0        0        0     5606 2020-02-02 00:00:00.000000 convtools-1.5.0/convtools/_mutations.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 convtools-1.5.0/convtools/_unique.py
+-rw-r--r--   0        0        0     9897 2020-02-02 00:00:00.000000 convtools-1.5.0/convtools/_utils.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 convtools-1.5.0/convtools/contrib/__init__.py
+-rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 convtools-1.5.0/convtools/contrib/fs.py
+-rw-r--r--   0        0        0    34888 2020-02-02 00:00:00.000000 convtools-1.5.0/convtools/contrib/tables.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 convtools-1.5.0/.gitignore
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 convtools-1.5.0/LICENSE.txt
+-rw-r--r--   0        0        0     4162 2020-02-02 00:00:00.000000 convtools-1.5.0/README.md
+-rw-r--r--   0        0        0     2473 2020-02-02 00:00:00.000000 convtools-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     7729 2020-02-02 00:00:00.000000 convtools-1.5.0/PKG-INFO
```

### Comparing `convtools-1.4.0/convtools/_aggregations.py` & `convtools-1.5.0/convtools/_aggregations.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""This module brings aggregations with various reduce functions"""
+"""Define aggregations with various reduce functions."""
 import typing as t
 import warnings
 from collections import defaultdict
 from decimal import Decimal
 from itertools import chain
 from math import ceil
 
@@ -28,15 +28,15 @@
     _none,
 )
 from ._heuristics import Weights
 from ._utils import Code
 
 
 class ReduceCode:
-    """Merges and stores code of reducers"""
+    """Merge and store code of reducers."""
 
     def __init__(self):
         self.value_to_name: "t.Dict[str, str]" = {}
         self.condition_to_child: "t.Dict[str, ReduceCode]" = {}
         self.key_to_reduce_lines = {}
 
     def add_assignment(self, value):
@@ -72,15 +72,15 @@
             prepare_first_lines,
             reduce_lines,
         )
         return var_agg_data_value
 
 
 class ReduceManager:
-    """Builds group by / aggregate code"""
+    """Build group by / aggregate code."""
 
     __slots__ = [
         "var_row",
         "var_agg_data",
         "aggregate_mode",
         "number",
         "reduce_code",
@@ -210,15 +210,15 @@
 
             code.incr_indent_level(-1)
 
         for condition, child in reduce_code.condition_to_child.items():
             checksum += self.add_group_by_code(
                 code,
                 child,
-                delegated_conditions=delegated_conditions + (condition,),
+                delegated_conditions=(*delegated_conditions, condition),
                 var_init_checksum=var_init_checksum,
             )
 
         code.indent_level = initial_indent_level
         return checksum
 
     def add_aggregate_stage2_code(
@@ -247,26 +247,26 @@
                 for line in item[2]:  # reduce_lines
                     code.add_line(line, 0)
 
         for condition, child in reduce_code.condition_to_child.items():
             checksum += self.add_aggregate_stage2_code(
                 code,
                 child,
-                delegated_conditions=delegated_conditions + (condition,),
+                delegated_conditions=(*delegated_conditions, condition),
             )
 
         if add_pass_if_line_number == len(code.lines_info):
             code.add_line("pass", -1)
 
         code.indent_level = initial_indent_level
         return checksum
 
 
 class BaseReducer(BaseConversion):
-    """Base of a reduce operation to be used during the aggregation"""
+    """Base reduce operation to be used during the aggregation."""
 
     _expressions: t.Sequence[BaseConversion]
 
     default: t.Union[_None, BaseConversion] = _none
     initial: t.Union[_None, BaseConversion] = _none
     internals_are_public: bool
     values_use_times: t.Tuple[int, ...]
@@ -313,14 +313,15 @@
         if not self.internals_are_public and not isinstance(
             self.initial, _None
         ):
             warnings.warn(
                 "2.0 will raise ValueError if initial is "
                 f"passed to {self.__class__.__name__}",
                 DeprecationWarning,
+                stacklevel=1,
             )
 
     def prepare_default_n_initial(self, default, initial):
         if default is _none:
             default = self.default
         if initial is _none:
             initial = self.initial
@@ -413,15 +414,16 @@
             kwargs[f"value{index}"] = expression_code
 
         reduce_lines = self.get_option("reduce_lines", ctx)
 
         if not isinstance(self.initial, _None) and self.internals_are_public:
             prepare_first_lines = (
                 f"%(result)s = {self.initial.gen_code_and_update_ctx(var_row, ctx)}",
-            ) + reduce_lines
+                *reduce_lines,
+            )
         else:
             prepare_first_lines = self.get_option("prepare_first_lines", ctx)
 
         new_agg_data_value = reduce_code.add_reduce_lines(
             var_agg_data_value,
             tuple(line % kwargs for line in prepare_first_lines),
             tuple(line % kwargs for line in reduce_lines),
@@ -433,14 +435,15 @@
     def check_expressions(self):
         super().check_expressions()
         if len(self.expressions) > 1:
             warnings.warn(
                 "2.0 will raise TypeError if more than 1 expression is "
                 f"passed to {self.__class__.__name__}",
                 DeprecationWarning,
+                stacklevel=1,
             )
 
 
 class SingleExpressionReducer(BaseReducer):
     def check_expressions(self):
         super().check_expressions()
         expressions_len = len(self.expressions)
@@ -448,19 +451,22 @@
             raise ValueError("expected one expression")
 
         if expressions_len > 1:
             warnings.warn(
                 "2.0 will raise TypeError if more than 1 expression is "
                 f"passed to {self.__class__.__name__}",
                 DeprecationWarning,
+                stacklevel=1,
             )
 
 
 class BaseDictReducer(BaseReducer):
-    """This reducer accepts 2 expressions:
+    """Base reducer of two expressions.
+
+    This reducer accepts 2 expressions:
 
     - the first one is used to calculate keys of the resulting dict
     - the second one is used to calculate values to be reduced and put as the
       final value, under the certain key.
 
     Effectively dict reducers allow for double grouping: the first one on the
     top level, the second one on DictReducer level.
@@ -481,34 +487,34 @@
             ):
                 self.expressions = tuple(expr.conversions)
                 return
         raise ValueError("invalid dict reducer input: two values expected")
 
 
 class SumReducer(SingleExpressionReducer):
-    """Takes a sum, None is considered as 0"""
+    """Take a sum, None is considered as 0."""
 
     default = NaiveConversion(0)
     internals_are_public = True
-    values_use_times = (1,)  # TODO set to 1 once debugged
+    values_use_times = (1,)
     works_with_not_none_only = (False,)
 
     def prepare_first_lines(self, ctx):  # pylint: disable=unused-argument
         if self.expressions[0].has_hint(BaseConversion.OutputHints.NOT_NONE):
             return ("%(result)s = %(value0)s",)
         return ("%(result)s = %(value0)s or 0",)
 
     def reduce_lines(self, ctx):  # pylint: disable=unused-argument
         if self.expressions[0].has_hint(BaseConversion.OutputHints.NOT_NONE):
             return ("%(result)s += %(value0)s",)
         return ("%(result)s += %(value0)s or 0",)
 
 
 class SumOrNoneReducer(SingleExpressionReducer):
-    """Takes a sum, if at least one None is met, the result is None"""
+    """Take a sum. If at least one None is met, the result is None."""
 
     default = NaiveConversion(None)
     internals_are_public = True
     works_with_not_none_only = (False,)
     prepare_first_lines = ("%(result)s = %(value0)s",)
 
     def values_use_times(self, ctx):  # pylint: disable=unused-argument
@@ -548,17 +554,19 @@
     reduce_lines = (
         "if %(result)s > %(value0)s:",
         "    %(result)s = %(value0)s",
     )
 
 
 class CountReducer(OptionalExpressionReducer):
-    """Counts objects. It accepts either zero or one expression as an argument and:
-    - if zero expressions passed: counts number of rows
-    - one expression: counts not None values of the evaluated expression
+    """Counts objects.
+
+    It accepts either zero or one expression as an argument:
+      - if zero expressions passed: counts number of rows
+      - one expression: counts not None values of the evaluated expression
     """
 
     default = NaiveConversion(0)
     internals_are_public = True
     values_use_times = (0,)
     prepare_first_lines = ("%(result)s = 1",)
     reduce_lines = ("%(result)s += 1",)
@@ -596,30 +604,30 @@
     values_use_times = (1,)
     works_with_not_none_only = (False,)
     prepare_first_lines = ("%(result)s = %(value0)s",)
     reduce_lines = ("%(result)s = %(value0)s",)
 
 
 class MaxRowReducer(SingleExpressionReducer):
-    """Returns a row with a max value of object, defined by the argument"""
+    """Return a row with a max value of an argument."""
 
     default = NaiveConversion(None)
     internals_are_public = False
     values_use_times = (2,)
     works_with_not_none_only = (True,)
     prepare_first_lines = ("%(result)s = (%(value0)s, %(row)s)",)
     reduce_lines = (
         "if %(result)s[0] < %(value0)s:",
         "    %(result)s = (%(value0)s, %(row)s)",
     )
     post_conversion = GetItem(1)
 
 
 class MinRowReducer(SingleExpressionReducer):
-    """Returns a row with a min value of object, defined by the argument"""
+    """Return a row with a min value of an argument."""
 
     default = NaiveConversion(None)
     internals_are_public = False
     values_use_times = (2,)
     works_with_not_none_only = (True,)
     prepare_first_lines = ("%(result)s = (%(value0)s, %(row)s)",)
     reduce_lines = (
@@ -631,29 +639,29 @@
     def check_expressions(self):
         super().check_expressions()
         if not isinstance(self.initial, _None):
             warnings.warn(
                 "2.0 will raise ValueError if initial is "
                 f"passed to {self.__class__.__name__}",
                 DeprecationWarning,
+                stacklevel=1,
             )
 
 
 class ArrayReducer(SingleExpressionReducer):
     default = NaiveConversion(None)
     internals_are_public = True
     values_use_times = (1,)
     works_with_not_none_only = (False,)
     prepare_first_lines = ("%(result)s = [%(value0)s]",)
     reduce_lines = ("%(result)s.append(%(value0)s)",)
 
 
 class ListSortedOnceWrapper:
-    """Wraps a list, exposes append method only. Once the list is filled up, it
-    is sorted (only once) in-place and is returned when get method called."""
+    """Wrap list, which is sorted only once."""
 
     __slots__ = ["list_", "append", "sorted", "key", "reverse"]
 
     def __init__(self, list_: list, key=None, reverse=False):
         self.list_ = list_
         self.append = self.list_.append
         self.sorted = False
@@ -665,15 +673,15 @@
             self.list_.sort(key=self.key, reverse=self.reverse)
             self.sorted = True
             del self.append
         return self.list_
 
 
 class SortedArrayReducer(SingleExpressionReducer):
-    """Array reducer which sorts the list just once in the end"""
+    """Reduce values to a sorted array."""
 
     default = NaiveConversion(None)
     internals_are_public = False
     values_use_times = (1,)
     works_with_not_none_only = (False,)
     reduce_lines = ("%(result)s.append(%(value0)s)",)
     post_conversion = This.call_method("get")
@@ -699,17 +707,19 @@
     works_with_not_none_only = (False,)
     prepare_first_lines = ("%(result)s = { %(value0)s: None }",)
     reduce_lines = ("%(result)s[%(value0)s] = None",)
     post_conversion = This.as_type(list)
 
 
 class DictReducer(BaseDictReducer):
-    """Aggregates values to a dict:
-    - keys: defined by the first argument
-    - values: defined by the second argument, reduced with Last."""
+    """Reduce two values to a dict.
+
+    Keys: defined by the first argument.
+    Values: defined by the second argument, reduced with Last.
+    """
 
     default = NaiveConversion(None)
     internals_are_public = False
     values_use_times = (1, 1)
     works_with_not_none_only = (False, False)
     prepare_first_lines = ("%(result)s = { %(value0)s: %(value1)s }",)
     reduce_lines = ("%(result)s[%(value0)s] = %(value1)s",)
@@ -717,34 +727,38 @@
 
 lock_default_dict_conversion = InlineExpr(
     'setattr({this_}, "default_factory", None) or {this_}'
 ).pass_args(this_=This)
 
 
 class DictArrayReducer(BaseDictReducer):
-    """Aggregates values to a dict:
-    - keys: defined by the first argument
-    - values: defined by the second argument, reduced with Array."""
+    """Reduce two values to a dict.
+
+    Keys: defined by the first argument.
+    Values: defined by the second argument, reduced with Array.
+    """
 
     default = NaiveConversion(None)
     internals_are_public = False
     values_use_times = (1, 1)
     works_with_not_none_only = (False, False)
     prepare_first_lines = (
         "%(result)s = defaultdict(list)",
         "%(result)s[%(value0)s].append(%(value1)s)",
     )
     reduce_lines = ("%(result)s[%(value0)s].append(%(value1)s)",)
     post_conversion = lock_default_dict_conversion
 
 
 class DictArrayDistinctReducer(BaseDictReducer):
-    """Aggregates values to a dict:
-    - keys: defined by the first argument
-    - values: defined by the second argument, reduced with ArrayDistinct."""
+    """Reduce two values to a dict.
+
+    Keys: defined by the first argument
+    Values: defined by the second argument, reduced with ArrayDistinct.
+    """
 
     default = NaiveConversion(None)
     internals_are_public = False
     values_use_times = (1, 1)
     works_with_not_none_only = (False, False)
     prepare_first_lines = (
         "%(result)s = defaultdict(dict)",
@@ -753,18 +767,20 @@
     reduce_lines = ("%(result)s[%(value0)s][%(value1)s] = None",)
     post_conversion = InlineExpr(
         "{{k_: list(v_) for k_, v_ in {}.items()}}"
     ).pass_args(This)
 
 
 class DictSumReducer(BaseDictReducer):
-    """Aggregates values to a dict:
-    - keys: defined by the first argument
-    - values: defined by the second argument, reduced with Sum
-       * None is considered 0"""
+    """Reduce two values to a dict.
+
+    Keys: defined by the first argument
+    Values: defined by the second argument, reduced with Sum
+       * None is considered 0
+    """
 
     default = NaiveConversion(None)
     internals_are_public = False
     values_use_times = (1, 1)
     works_with_not_none_only = (False, False)
     prepare_first_lines = (
         "%(result)s = defaultdict(int)",
@@ -775,18 +791,20 @@
     def reduce_lines(self, ctx):  # pylint: disable=unused-argument
         if self.expressions[1].has_hint(BaseConversion.OutputHints.NOT_NONE):
             return ("%(result)s[%(value0)s] += %(value1)s",)
         return ("%(result)s[%(value0)s] += (%(value1)s or 0)",)
 
 
 class DictSumOrNoneReducer(BaseDictReducer):
-    """Aggregates values to a dict:
-    - keys: defined by the first argument
-    - values: defined by the second argument, reduced with SumOrNone
-       * if at least one None is met, the result is None"""
+    """Reduce two values to a dict.
+
+    Keys: defined by the first argument
+    Values: defined by the second argument, reduced with SumOrNone
+       * if at least one None is met, the result is None
+    """
 
     default = NaiveConversion(None)
     internals_are_public = False
     works_with_not_none_only = (False, False)
     prepare_first_lines = (
         "%(result)s = defaultdict(int)",
         "%(result)s[%(value0)s] = %(value1)s",
@@ -806,17 +824,19 @@
             "    %(result)s[%(value0)s] = None",
             "elif %(result)s[%(value0)s] is not None:",
             "    %(result)s[%(value0)s] += %(value1)s",
         )
 
 
 class DictMaxReducer(BaseDictReducer):
-    """Aggregates values to a dict:
-    - keys: defined by the first argument
-    - values: defined by the second argument, reduced with Max."""
+    """Reduce two values to a dict.
+
+    Keys: defined by the first argument
+    Values: defined by the second argument, reduced with Max.
+    """
 
     default = NaiveConversion(None)
     internals_are_public = False
     values_use_times = (1, 1)
     prepare_first_lines = ("%(result)s = { %(value0)s: %(value1)s }",)
 
     def works_with_not_none_only(self, ctx):  # pylint: disable=unused-argument
@@ -828,17 +848,19 @@
         return (
             "if %(value0)s not in %(result)s or %(value1)s > %(result)s[%(value0)s]:",
             "    %(result)s[%(value0)s] = %(value1)s",
         )
 
 
 class DictMinReducer(BaseDictReducer):
-    """Aggregates values to a dict:
-    - keys: defined by the first argument
-    - values: defined by the second argument, reduced with Min."""
+    """Reduce two values to a dict.
+
+    Keys: defined by the first argument
+    Values: defined by the second argument, reduced with Min.
+    """
 
     default = NaiveConversion(None)
     internals_are_public = False
     values_use_times = (1, 1)
     prepare_first_lines = ("%(result)s = { %(value0)s: %(value1)s }",)
 
     def works_with_not_none_only(self, ctx):  # pylint: disable=unused-argument
@@ -850,19 +872,21 @@
         return (
             "if %(value0)s not in %(result)s or %(value1)s < %(result)s[%(value0)s]:",
             "    %(result)s[%(value0)s] = %(value1)s",
         )
 
 
 class DictCountReducer(BaseDictReducer):
-    """Aggregates values to a dict:
-    - keys: defined by the first argument
-    - values: defined by the second argument (optional), reduced with Count.
+    """Reduce two values to a dict.
+
+    Keys: defined by the first argument
+    Values: defined by the second argument (optional), reduced with Count.
        * counts rows if no 2nd arg is passed
-       * counts non None values if 2nd arg is passed"""
+       * counts non None values if 2nd arg is passed
+    """
 
     default = NaiveConversion(None)
     internals_are_public = False
     values_use_times = (2, 0)
     prepare_first_lines = ("%(result)s = { %(value0)s: 1 }",)
     reduce_lines = (
         "if %(value0)s not in %(result)s:",
@@ -893,17 +917,19 @@
             BaseConversion.OutputHints.NOT_NONE
         ):
             return (False, True)
         return (False, False)
 
 
 class DictCountDistinctReducer(BaseDictReducer):
-    """Aggregates values to a dict:
-    - keys: defined by the first argument
-    - values: defined by the second argument, reduced with CountDistinct."""
+    """Reduce two values to a dict.
+
+    Keys: defined by the first argument
+    Values: defined by the second argument, reduced with CountDistinct.
+    """
 
     default = NaiveConversion(None)
     internals_are_public = False
     values_use_times = (2, 1)
     works_with_not_none_only = (False, False)
     prepare_first_lines = ("%(result)s = { %(value0)s: { %(value1)s } }",)
     reduce_lines = (
@@ -914,33 +940,37 @@
     )
     post_conversion = InlineExpr(
         "{{ k_: len(v_) for k_, v_ in {}.items() }}"
     ).pass_args(This)
 
 
 class DictFirstReducer(BaseDictReducer):
-    """Aggregates values to a dict:
-    - keys: defined by the first argument
-    - values: defined by the second argument, reduced with First."""
+    """Reduce two values to a dict.
+
+    Keys: defined by the first argument
+    Values: defined by the second argument, reduced with First.
+    """
 
     default = NaiveConversion(None)
     internals_are_public = False
     values_use_times = (2, 1)
     works_with_not_none_only = (False, False)
     prepare_first_lines = ("%(result)s = { %(value0)s: %(value1)s }",)
     reduce_lines = (
         "if %(value0)s not in %(result)s:",
         "    %(result)s[%(value0)s] = %(value1)s",
     )
 
 
 class DictLastReducer(BaseDictReducer):
-    """Aggregates values to a dict:
-    - keys: defined by the first argument
-    - values: defined by the second argument, reduced with Last."""
+    """Reduce two values to a dict.
+
+    Keys: defined by the first argument
+    Values: defined by the second argument, reduced with Last.
+    """
 
     default = NaiveConversion(None)
     internals_are_public = False
     values_use_times = (1, 1)
     works_with_not_none_only = (False, False)
     prepare_first_lines = ("%(result)s = { %(value0)s: %(value1)s }",)
     reduce_lines = ("%(result)s[%(value0)s] = %(value1)s",)
@@ -948,15 +978,15 @@
 
 class ReducerDispatcher:
     def __call__(self, *args, **kwargs) -> "BaseConversion":
         raise NotImplementedError
 
 
 class AverageReducerDispatcher(ReducerDispatcher):
-    """Calculates weighted average (default weight is 0)"""
+    """Calculates weighted average (default weight is 0)."""
 
     def __call__(
         self, value, weight=1, default=None, where=None
     ) -> "BaseConversion":
         if isinstance(weight, (int, float, Decimal)) and weight == 1:
             return If(
                 CountReducer(where=where),
@@ -970,17 +1000,17 @@
                 / SumReducer(weight, where=where)
             ),
             default,
         )
 
 
 class TopReducer(DictCountReducer):
-    """
-    Returns a list of the most frequent values.
-    The resulting list is sorted in descending order of values frequency.
+    """Return a list of the most frequent values.
+
+    The resulting list is sorted in descending order of value frequency.
     """
 
     def __init__(self, k: int, key_conv, *args, **kwargs):
         if not isinstance(k, int):
             raise TypeError("K must be an integer.")
 
         if k < 1:
@@ -1002,43 +1032,46 @@
     # TODO: check how MaxRow performs here
     post_conversion = InlineExpr(
         "sorted({data}.items(), key=lambda x: x[1])[-1][0]"
     ).pass_args(data=This)
 
 
 class PercentileReducer(SortedArrayReducer):
-    """Calculates percentile (floats from 0 to 100 inclusive)
+    """Calculates percentile (float: from 0 to 100 inclusive).
 
     >>> c.ReduceFuncs.Percentile(95, c.item("amount"))
     >>> c.ReduceFuncs.Percentile(95, c.item("amount"), interpolation="lower")
 
     interpolation options:
       * "linear"
       * "lower"
       * "higher"
       * "midpoint"
       * "nearest"
     """
 
-    interpolation_to_method: "t.Dict[str, t.Callable]" = {}
+    interpolation_to_method: t.ClassVar[t.Dict[str, t.Callable]] = {}
 
     def __init__(
         self, percentile: float, conv, *args, interpolation="linear", **kwargs
     ):
-        """
+        """Init self.
 
         Args:
-         * interpolation: one of
-           #. "linear"
-           #. "lower"
-           #. "higher"
-           #. "midpoint"
-           #. "nearest"
+          percentile: 0.0-100.0 inclusive
+          conv: conversion to apply before reduce phase
+          args: unused
+          interpolation: one of:
+            * "linear"
+            * "lower"
+            * "higher"
+            * "midpoint"
+            * "nearest"
+          kwargs: can accept `where`=conversion to pre-filter reduced values
         """
-
         self.percentile = percentile
         try:
             self.method = self.interpolation_to_method[interpolation]
         except KeyError as e:
             raise ValueError("unsupported interpolation type") from e
 
         super().__init__(conv, *args, **kwargs)
@@ -1107,15 +1140,15 @@
 def MedianReducer(  # pylint:disable=invalid-name
     conv, *args, **kwargs
 ) -> BaseConversion:
     return PercentileReducer(50, conv, *args, **kwargs)
 
 
 class ReduceFuncs:
-    """Exposes the list of reduce functions"""
+    """Expose the list of reduce functions."""
 
     # pylint: disable=invalid-name
 
     #: Calculates the sum, skips false values
     Sum = SumReducer
     #: Calculates the sum, any ``None`` makes the total sum ``None``
     SumOrNone = SumOrNoneReducer
@@ -1185,36 +1218,36 @@
     #: Aggregates values into dict; dict values are first values per group
     DictFirst = DictFirstReducer
     #: Aggregates values into dict; dict values are last values per group
     DictLast = DictLastReducer
 
 
 class GroupBy:
-    """Generates the function which aggregates the data, grouping by
-    conversions, specified in `__init__` method and returns list of items in a
-    format defined by the parameter passed to ``aggregate`` method.
+    """Generates the function which implements aggregation.
 
-    If no group keys are passed, then it returns just a single value, defined
-    by the parameter passed to ``aggregate`` method.
+    Grouping is done by conversions passed to `__init__` method.
+     - if there are any, the result is a list of reduced values.
+     - if there is no keys to group by, the result is a single reduced value.
+
+    Reduced value/values is/are defined by the parameter passed to
+    ``aggregate`` method.
 
     Current optimizations:
      * piping like ``c.group_by(...).aggregate().pipe(...)`` won't run
-       the aggregation twice, this is handled as 2 statements
-     * using the same reduce clause twice (e.g. one used as an argument
-       for some function calls) won't result in calculating this reduce twice
+       the aggregation twice
+     * using the same reducer twicewon't result in double calculation
     """
 
     def __init__(self, *by):
-        """Takes any number of conversions to group by
+        """Accept keys of group by as conversions.
 
         Args:
-          by (tuple): each item is to be wrapped with
-            :py:obj:`ensure_conversion`.  Each is to resolve to a hashable
-            object to allow using such tuples as keys. If nothing is passed,
-            aggregate the input into a single object.
+          by (tuple): keys of group by as conversions. Each is to resolve to a
+            hashable object. If nothing is passed, the result is a single
+            object.
         """
         self.by = by
 
     def aggregate(
         self, reducer: t.Union[dict, list, set, tuple, BaseConversion]
     ) -> "Grouper":
         return Grouper(self.by, reducer)
@@ -1249,16 +1282,18 @@
 {code_aggregate}
 
 {code_result}
 """
 
 
 class Grouper(BaseConversion):
-    """Fully initialized GroupBy conversion, which delegates some of methods
-    like iter to its internals"""
+    """Fully initialized GroupBy conversion.
+
+    Which delegates some of methods like iter to its internals.
+    """
 
     self_content_type = (
         BaseConversion.self_content_type
         | BaseConversion.ContentTypes.AGGREGATION
         | BaseConversion.ContentTypes.NONE_USAGE
     )
 
@@ -1430,34 +1465,34 @@
             conversion
         ).gen_code_and_update_ctx(code_input, ctx)
 
 
 def Aggregate(  # pylint:disable=invalid-name
     *args, **kwargs
 ) -> BaseConversion:
-    """Shortcut for ``GroupBy().aggregate(*args, **kwargs)``"""
+    """Shortcut for `GroupBy().aggregate(*args, **kwargs)`."""
     return GroupBy().aggregate(*args, **kwargs)
 
 
 class Reduce(BaseReducer):
-    """Defines the reduce operation, which is based on a callable / expression
-    to be used during the aggregation"""
+    """Reduce operation, which is based on a callable / expression."""
 
     internals_are_public = True
 
     def __init__(
         self,
         to_call_with_2_args: t.Union[t.Callable, InlineExpr],
         *expressions: t.Tuple[t.Any, ...],
         initial: t.Union[_None, t.Callable, InlineExpr, t.Any],
         default: t.Union[_None, t.Callable, t.Any] = _none,
         unconditional_init: bool = False,
         where=None,
     ):
-        """
+        """Init self.
+
         Args:
           to_call_with_2_args: defines the reduce function/expression
           expressions: args to be passed to `to_call_with_2_args` after the
             aggregation value
           initial: defines the very first item to be passed to
             `to_call_with_2_args` item. If callable, then the result of a call
             is used. If a conversion is passed, it is resolved on the first
@@ -1466,23 +1501,26 @@
             reduce in a group (e.g. the current reduce operation has filtered
             out some rows, while an adjacent reduce operation has got
             something to reduce, forming a group). If callable, then the result
             of a call is used.  When default is not passed, initial is used if
             it doesn't depend on input data.
           unconditional_init: tells whether the first call initializes the
             aggregation value OR there is a condition for that
+          where: condition conversion to pre-filter values to be reduced.
         """
         super().__init__(
             *expressions, initial=initial, default=default, where=where
         )
 
         self.to_call_with_2_args = self.ensure_conversion(to_call_with_2_args)
         if unconditional_init:
             warnings.warn(
-                "unconditional_init is no longer needed", DeprecationWarning
+                "unconditional_init is no longer needed",
+                DeprecationWarning,
+                stacklevel=1,
             )
 
     def values_use_times(self, ctx):  # pylint: disable=unused-argument
         return (1,) * len(self.expressions)
 
     def works_with_not_none_only(self, ctx):  # pylint: disable=unused-argument
         return (False,) * len(self.expressions)
```

### Comparing `convtools-1.4.0/convtools/_base.py` & `convtools-1.5.0/convtools/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,53 +1,35 @@
-"""
-Base and basic conversions are defined here.
-"""
+"""Base and basic conversions are defined here."""
 import re
 import string
 import sys
 import typing as t
 from collections import deque
 from datetime import datetime
 from decimal import Decimal
 from itertools import chain
 from keyword import iskeyword
 from random import Random
+from typing import Any
 
-from ._dt import (
-    DayOfWeekStep,
-    MonthStep,
-    TruncModes,
-    date_parse,
-    date_trunc_to_day,
-    date_trunc_to_month,
-    datetime_parse,
-    datetime_trunc_to_day,
-    datetime_trunc_to_microsecond,
-    datetime_trunc_to_month,
-    to_step,
-)
 from ._heuristics import Weights
 from ._utils import (
     BaseCtx,
     BaseOptions,
     Code,
     CodeStorage,
     LazyModule,
     _None,
     _none,
     get_builtins_dict,
     iter_windows,
 )
 
 
-convtools_cumulative = LazyModule("convtools._cumulative")
-convtools_debug = LazyModule("convtools._debug")
-convtools_mutations = LazyModule("convtools._mutations")
 convtools_unique = LazyModule("convtools._unique")
-convtools_expect = LazyModule("convtools._expect")
 
 
 black: "t.Optional[t.Any]" = None
 try:
     import black as black_  # pragma: no cover
 
     black = black_  # pragma: no cover
@@ -60,28 +42,27 @@
 
 
 class CodeGenerationOptionsCtx(BaseCtx):
     options_cls = CodeGenerationOptions
 
 
 class ConverterOptions(BaseOptions):
-    """Converter options (+ see default values below):
+    """Converter options (+ see default values below).
 
     * ``debug = False`` - same as ``.gen_converter(debug=...)``
 
     """
 
     debug = False
 
 
 class ConverterOptionsCtx(BaseCtx):
     """Thread-safe context to manage options.
 
     Example:
-
     >>> with ConverterOptionsCtx() as options:
     >>>     options.debug = True
     >>>     # ...
 
     """
 
     options_cls = ConverterOptions
@@ -90,38 +71,42 @@
 CONVERTER_TEMPLATE = """
 def {converter_name}({code_signature}):
 {code}
 """
 
 
 def ensure_conversion(
-    conversion: t.Any, explicitly_allowed_cls=None
+    conversion: t.Any, explicitly_allowed_cls=None  # noqa: ANN401
 ) -> "BaseConversion":
-    r"""Helps to define conversions based on its type:
+    """Transforms anything to conversion.
+
+    Helps to define conversions based on its type:
         * any conversion is returned untouched
         * list/dict/set/tuple collections are wrapped with ``c.list``,
           ``c.dict``, ``c.set``, ``c.tuple`` (see below).
           If it's not desired, use ``c.naive`` instead
         * slice gets recreated, each ``slice.start, slice.stop, slice.step`` is
           wrapped with ``ensure_conversion``
         * everything else is wrapped with ``c.naive`` (see below)
 
 
     Args:
       conversion (object): any object
+      explicitly_allowed_cls: defines which conversions with
+        `explicitly_allowed_cls` flag set can be used
 
     Returns:
       BaseConversion: a conversion based on ``conversion`` type:
        * BaseConversion -> :py:class:`BaseConversion`
-       * {} -> :py:class:`Dict` (\*conversion.items())
-       * [] -> :py:class:`List` (\*conversion)
-       * () -> :py:class:`Tuple` (\*conversion)
-       * set() -> :py:class:`Set` (\*conversion)
-       * slice -> :py:obj:`InlineExpr`
-       * object -> :py:class:`NaiveConversion` (conversion)
+       * {} -> `Dict` conversion
+       * [] -> `List` conversion
+       * () -> `Tuple` conversion
+       * set() -> `Set` conversion
+       * slice -> `InlineExpr` conversion
+       * object -> `NaiveConversion` otherwise
     """
     if isinstance(conversion, BaseConversion):
         if conversion.used_in_narrow_context and (
             explicitly_allowed_cls is None
             or not isinstance(conversion, explicitly_allowed_cls)
         ):
             raise AssertionError(
@@ -152,38 +137,38 @@
 
 
 _random = Random(1)
 choice = _random.choice
 
 
 class BaseConversion(t.Generic[CT]):
-    """This is the base class  of every conversion (so you are not going to use
-    this directly).
+    """Base class of every conversion.
 
-    A conversion is a definition of some actions to be done to the input passed
-    as `data_` argument.
+    A conversion defines a transform of an input into an output before you have
+    any data at hand. You are not going to use this directly.
 
-    Conversions are nestable (iteration, calling functions) and chainable
-    (method calling or piping).
+    Conversions can be nested (iteration, calling functions) and chained via
+    piping.
 
     Every conversion has many important methods like:
       * `gen_converter`
       * `item`, `attr`, `call`, `call_methods`, `as_type`
       * `and_`, `or_`, `not_`, `is_`, `is not`, `in_`, `not_in`
       * `filter`
       * `pipe`
-      * overloaded operators"""
+      * overloaded operators
+    """
 
     _none = _none
     valid_pipe_output = True
     used_in_narrow_context = False
     trackable_dependency = False
 
     class ContentTypes:
-        """Defines types of conversion content for bitmask calculations"""
+        """Defines types of conversion content for bitmask calculations."""
 
         REDUCER = 1
         AGGREGATION = 2
         NEW_LABEL = 4
         ARG_USAGE = 8
         LABEL_USAGE = 16
         BREAKPOINT = 32
@@ -245,25 +230,27 @@
     def get_dependencies(self, types=None):
         deps: "t.Iterator[t.Any]" = chain(self._depends_on.values(), (self,))
         if types:
             deps = (dep for dep in deps if isinstance(dep, types))
         return deps
 
     def ensure_conversion(self, conversion, **kwargs) -> "BaseConversion":
-        """Runs ensure_conversion on the input object and adds the resulting
-        conversion to the list of dependencies"""
+        """Transform an object into conversion and track its dependencies."""
         conversion = ensure_conversion(conversion, **kwargs)
         self.depends_on(conversion)
         return conversion
 
     def gen_code_and_update_ctx(self, code_input, ctx) -> str:
-        """The main method which generates the code and stores necessary info
-        in the context (which will be passed as locals() and globals() on to
-        the exec function).  However you should not override this method
-        directly, please implement the `_gen_code_and_update_ctx` one.
+        """The main code generation method.
+
+        It generates code of a conversion as an expression, stores required
+        data in the context (which is passed as `locals()` and `globals()` to
+        `compile`.
+        However you should not override this method
+        directly, please implement the `_gen_code_and_update_ctx` one
         """
         return self._gen_code_and_update_ctx(code_input, ctx)
 
     def _gen_code_and_update_ctx(self, code_input, ctx) -> str:
         raise NotImplementedError
 
     def to_code(self, code_input, ctx) -> "t.Optional[Code]":
@@ -292,16 +279,18 @@
             if name not in generated_names:
                 generated_names.add(name)
                 return name
 
         raise AssertionError("failed to generate unique filename", name)
 
     def gen_name(self, prefix, ctx, item_to_hash) -> str:
-        """Generates name of variable to be used in the generated code. This
-        also ensures that same items_to_hash will yield same names."""
+        """Generates name of variable to be used in the generated code.
+
+        This also ensures that items with same items_to_hash get same names.
+        """
         prefixed_hash_to_name = ctx[self.PREFIXED_HASH_TO_NAME]
         prefixed_hash = (prefix, item_to_hash)
         try:
             if prefixed_hash in prefixed_hash_to_name:
                 return prefixed_hash_to_name[prefixed_hash]
             name = self.gen_random_name(prefix, ctx)
 
@@ -476,17 +465,17 @@
     def gen_converter(
         self,
         method=False,
         class_method=False,
         signature=None,
         debug=None,
         converter_name="converter",
+        _inner=False,
     ):
-        """Compiles a function which act according to the conversion
-        definition.
+        """Compile a function which implements the conversion.
 
         Args:
           debug (bool): If `True`, prints the generated code (formats with
             black if available). By default: None
           signature (str): Defines the signature of the function to be
             compiled.  `data_` argument is what going to be used as the input.
             e.g. ``signature="self, dt, data_, **kwargs"``
@@ -495,21 +484,31 @@
             ``signature="cls, data_"``
           converter_name (str): prefix of the name of the function to be
             compiled
 
         Returns:
           The compiled function
         """
+        if (
+            (debug or (self.contents & self.ContentTypes.BREAKPOINT))
+            and not _inner
+            and not ConverterOptionsCtx.get_option_value("debug")
+        ):
+            with ConverterOptionsCtx() as options:
+                options.debug = True
+                return self.gen_converter(
+                    method=method,
+                    class_method=class_method,
+                    signature=signature,
+                    debug=True,
+                    converter_name=converter_name,
+                    _inner=True,
+                )
         # signature should contain "data_" argument
         initial_code_input = "data_"
-        debug = (
-            debug
-            or (self.contents & self.ContentTypes.BREAKPOINT)
-            or ConverterOptionsCtx.get_option_value("debug")
-        )
         # self.ContentTypes.NEW_LABEL | self.ContentTypes.LABEL_USAGE
         has_labels = self.contents & 20
         has_none = self.contents & 128  # self.ContentTypes.NONE_USAGE
         ctx = self._init_ctx(debug=debug)
 
         args_to_skip = (
             "self",
@@ -595,53 +594,54 @@
 
         if class_method:
             return classmethod(converter)
 
         return converter
 
     def execute(self, *args, debug=None, **kwargs) -> t.Any:
-        """Shortcut for generating converter and running it"""
+        """Shortcut for `gen_converter()` and running it."""
         return self.gen_converter(
             debug=debug or ConverterOptionsCtx.get_option_value("debug")
         )(*args, **kwargs)
 
     def to_iter(self):
         return GeneratorComp(This, _none, self)
 
     def iter(self, element_conv, *, where=None) -> "BaseConversion":
-        """Shortcut for
+        """Iterate elements of self conversion.
+
+        Shortcut for
         ``self.pipe(c.generator_comp(element_conv, where=condition))``
 
         Args:
           element_conv (object): conversion to be run on each element
           where (object): condition inside the comprehension
 
         """
         return GeneratorComp(element_conv, where=where, self_conv=self)
 
     def iter_unique(self, element_conv=None, by_=None) -> "BaseConversion":
-        """
-        Creates a conversion which iterates over the input and yields unique
-        ones (supports custom uniqueness conditions)
+        """Iterate unique elements of self conversion.
 
         Args:
           element_conv: defines a conversion to be applied to each element to
             be returned; if it is None, it means `c.this`
           by_: defines a conversion to be applied to each element to check for
             uniqueness; if it is None, it means to use `element_conv` for
             uniqueness
         """
+        from convtools import _unique
+
         element_conv = This if element_conv is None else element_conv
-        return convtools_unique.IterUnique(
+        return _unique.IterUnique(
             self, element_conv, element_conv if by_ is None else by_
         )
 
     def filter(self, condition_conv, cast=None) -> "BaseConversion":
-        """Generates the code to iterate the input, taking items for which the
-        provided conversion resolves to a truth value.
+        """Filter elements of self conversion based on predicate conversion.
 
         Args:
           condition_conv (object): to be wrapped with
             :py:obj:`ensure_conversion` and used on each item of a collection
             to filter it
           cast (callable): to wrap the generator of filtered items
         Returns:
@@ -656,31 +656,38 @@
 
         if cast is not _none:
             result = result.as_type(cast)
 
         return result
 
     def iter_mut(self, *mutations: "BaseMutation") -> "BaseConversion":
-        """Conversion which results in a generator of mutated elements
+        """Mutates elements of self conversion.
 
         Args:
           mutations (BaseMutation): conversion to be run on each element
 
         """
-        return convtools_mutations.IterMutConversion(self, *mutations)
+        from convtools import _mutations
+
+        return _mutations.IterMutConversion(self, *mutations)
 
     def iter_windows(self, width, step=1):
-        """Iterates through an iterable and yields tuples, which are obtained
-        by sliding a windows of a given width, moving it by specified step
-        size"""
+        """Iterate elements of self conversion with a window of defined length.
+
+        Returns:
+          Generator[Tuple, None, None]
+        """
         return CallFunc(iter_windows, self, width, step)
 
     def flatten(self) -> "Call":
-        """Conversion which calls :py:obj:`itertools.chain.from_iterable` on
-        self. Returns iterable"""
+        """Pass self to `itertools.chain.from_iterable` to flatten it.
+
+        Returns:
+          iterable of elements.
+        """
         return CallFunc(chain.from_iterable, self)
 
     def take_while(self, condition) -> "BaseConversion":
         return self.pipe(TakeWhile(condition))
 
     def drop_while(self, condition) -> "BaseConversion":
         return self.pipe(DropWhile(condition))
@@ -705,36 +712,32 @@
 
     def call_like(self, *args, **kwargs):
         if self.is_itself_callable_like():
             return self.call(*args, **kwargs)
         raise AssertionError("unexpected callable", self)
 
     def call(self, *args, **kwargs) -> "Call":
-        """Gets compiled into the code which calls the input with params.
-        Each ``*args`` and ``**kwargs`` are wrapped with ``ensure_conversion``.
-        """
+        """Call __call__ on input, taking args & kwargs as conversions."""
         return Call(*args, self_conv=self, **kwargs)
 
     def apply(self, args, kwargs):
-        """Gets compiled into the code which calls the input with params.
-        Both ``args`` and ``kwargs`` are wrapped with ``ensure_conversion``.
-        """
+        """Call __call__ on input, taking args & kwargs as conversions."""
         return ApplyFunc(self, args, kwargs)
 
     def call_method(self, method_name: str, *args, **kwargs) -> "Call":
-        """Gets compiled into the code which calls the ``method_name`` method
-        of input with params.
-        It's a shortcut to ``(...).attr(method_name).call(*args, **kwargs)``
+        """Call method with params.
+
+        It's a shortcut to ``(...).attr(method_name).call(*args, **kwargs)``.
         """
         return self.attr(method_name).call(*args, **kwargs)
 
     def apply_method(self, method_name: str, args, kwargs) -> "Call":
-        """Gets compiled into the code which calls the ``method_name`` method
-        of input with params.
-        It's a shortcut to ``(...).attr(method_name).apply(args, kwargs)``
+        """Call method with params.
+
+        It's a shortcut to ``(...).attr(method_name).apply(args, kwargs)``.
         """
         return self.attr(method_name).apply(args, kwargs)
 
     def as_type(self, callable_) -> "Call":
         return ensure_conversion(callable_).call(self)
 
     def or_(self, *args, **kwargs) -> "Or":
@@ -895,24 +898,23 @@
         return (
             InlineExpr("{0} // {1}", Weights.MATH_SIMPLE)
             .pass_args(self, b)
             .add_hint(self.OutputHints.NOT_NONE)
         )
 
     def len(self) -> "BaseConversion":
-        """Shortcut for CallFunc(len, self)"""
+        """Shortcut for CallFunc(len, self)."""
         return CallFunc(len, self)
 
     def sort(self, key=None, reverse=False) -> "BaseConversion":
-        """Shortcut for calling :py:obj:`convtools.base.SortConversion` on
-        self"""
+        """Shortcut for CallFunc(sorted, self, key=key, reverse=reverse)."""
         return self.pipe(SortConversion(key=key, reverse=reverse))
 
     def add_label(self, label_name: t.Union[str, dict]) -> "BaseConversion":
-        """Labels data so it can be reused further:
+        """Labels input data so it can be reused in further conversions.
 
         Basic:
         >>> c.item("objects", 0).add_label("first")
 
         Advanced:
         >>> c.item("objects").add_label({
         >>>     "first": c.item(0),
@@ -927,120 +929,167 @@
             to conversions
         Returns:
           LabelConversion: the labeled conversion
         """
         return self.pipe(This, label_input=label_name)
 
     def tap(self, *mutations: "BaseMutation") -> "BaseConversion":
-        """Allows to tap into the processing of a conversion and mutate it
-        in place. Accepts multiple mutations, order matters.
+        """Apply mutation to result of self conversion. Order matters.
 
         Args:
           mutations (iterable of BaseMutation): mutations to process the
             conversion
         """
-        return convtools_mutations.TapConversion(self, *mutations)
+        from convtools import _mutations
+
+        return _mutations.TapConversion(self, *mutations)
 
     def pipe(
         self,
         next_conversion,
         *args,
         label_input=None,
         label_output=None,
         **kwargs,
     ) -> "BaseConversion":
-        """Shortcut for :py:obj:`PipeConversion`"""
+        """Pass the result of one conversion as an input to another.
+
+        If `next_conversion` is callable, it gets called with the previous result
+        passed as the first param.
+
+        Supports predicate/sorting/type casting push down (each is directly applied
+        to the ``where`` conversion.
+
+        Supports labeling both pipe input and output data (allows to apply
+        conversions before labeling).
+        """
         return PipeConversion(
             self,
             next_conversion,
             *args,
             label_input=label_input,
             label_output=label_output,
             **kwargs,
         )
 
     def breakpoint(self):
-        """Shortcut to Breakpoint(self)"""
-        return convtools_debug.Breakpoint(self)
+        """Wrap conversion with function and add breakpoint right after."""
+        from convtools import _debug
+
+        return _debug.Breakpoint(self)
 
     def and_then(self, conversion, condition=bool) -> "BaseConversion":
-        """Applies conversion if condition is true, otherwise leaves untouched.
-        Condition is :py:obj:`bool` by default"""
+        """Apply conversion if condition is true, otherwise leave it untouched."""
         if condition is bool:
             return self.pipe(And(This(), conversion))
 
         return self.pipe(
             If(
                 CallFunc(condition, This())
                 if callable(condition)
                 else condition,
                 conversion,
             )
         )
 
     def cumulative(self, prepare_first, reduce_two, label_name=None):
-        """Shortcut for :py:obj:`Cumulative`"""
-        return convtools_cumulative.Cumulative(
+        """Calculate cumulative values within iterables.
+
+        Example:
+        >>> assert (
+        >>>     c.iter(c.cumulative(c.this, c.this + c.PREV))
+        >>>     .as_type(list)
+        >>>     .execute([0, 1, 2, 3, 4])
+        >>> ) == [0, 1, 3, 6, 10]
+
+        Args:
+          prepare_first: conversion to apply to the first element
+          reduce_two: conversion to reduce two values to one
+          label_name: custom name of cumulative to be used. It is needed when
+            `c.cumulative_reset(label_name)`
+        """
+        from convtools import _cumulative
+
+        return _cumulative.Cumulative(
             self, prepare_first, reduce_two, label_name
         )
 
     def cumulative_reset(self, label_name):
-        """Shortcut for :py:obj:`CumulativeReset`"""
-        return convtools_cumulative.CumulativeReset(self, label_name)
+        """Reset cumulative value to its initial state.
+
+        >>> assert (
+        >>>     c.iter(
+        >>>         c.cumulative_reset("abc")
+        >>>         .iter(c.cumulative(c.this, c.this + c.PREV, label_name="abc"))
+        >>>         .as_type(list)
+        >>>     )
+        >>>     .as_type(list)
+        >>>     .execute([[0, 1, 2], [3, 4]])
+        >>> ) == [[0, 1, 3], [3, 7]]
+        """
+        from convtools import _cumulative
+
+        return _cumulative.CumulativeReset(self, label_name)
 
     def date_parse(self, main_format, *other_formats, default=_none):
-        """Parses str to date using `main_format` first, then tries
+        """datetime.strptime with multi-format and default support.
+
+        Parses str to date using `main_format` first, then tries
         `other_formats`, otherwise:
           - returns `default if provided
           - or raises ValueError
         """
-        if other_formats or default is not _none:
-            default = ensure_conversion(default)
-            default_is_complex = not isinstance(default, NaiveConversion)
-            conversion: "BaseConversion" = CallFunc(
-                date_parse,
-                self,
-                main_format,
-                NaiveConversion(other_formats),
-                None if default_is_complex else default,
-            )
-            if default_is_complex:
-                conversion = conversion.or_(default)
-            return conversion
+        from convtools import _dt, _exceptions
 
-        return CallFunc(datetime.strptime, self, main_format).call_method(
-            "date"
+        parse_exc_pairs = []
+        for fmt in chain((main_format,), other_formats):
+            conversion = _dt.DatetimeParse(fmt).call_method("date")
+            parse_exc_pairs.append((conversion, (ValueError, TypeError)))
+
+        return self.pipe(
+            _exceptions.try_multiple(*parse_exc_pairs, default=default)
         )
 
     def datetime_parse(self, main_format, *other_formats, default=_none):
-        """Parses str to datetime using `main_format` first, then tries
+        """datetime.strptime with multi-format and default support.
+
+        Parses str to datetime using `main_format` first, then tries
         `other_formats`, otherwise:
           - returns `default if provided
           - or raises ValueError
         """
-        if other_formats or default is not _none:
-            default = ensure_conversion(default)
-            default_is_complex = not isinstance(default, NaiveConversion)
-            conversion: "BaseConversion" = CallFunc(
-                datetime_parse,
-                self,
-                main_format,
-                NaiveConversion(other_formats),
-                None if default_is_complex else default,
-            )
-            if default_is_complex:
-                conversion = conversion.or_(default)
-            return conversion
+        from convtools import _dt, _exceptions
+
+        parse_exc_pairs = []
+        for fmt in chain((main_format,), other_formats):
+            conversion = _dt.DatetimeParse(fmt)
+            parse_exc_pairs.append((conversion, (ValueError, TypeError)))
 
-        return CallFunc(datetime.strptime, self, main_format)
+        return self.pipe(
+            _exceptions.try_multiple(*parse_exc_pairs, default=default)
+        )
 
     def date_trunc(self, step, offset=None, mode="start"):
-        """Truncates a date to periods of certain length, specified by step and
-        offset, passed as either a STEP-STRING (see below) or a
-        `datetime.timedelta`.
+        """Truncate date.
+
+        Args:
+          step: defines period length as STEP-STRING or a timedelta. If it's a
+            year, month or a day of week, it defines beginnings of periods too.
+          offset (optional): defines the shift of the expected date grid
+            relative to 0-point as STEP-STRING or a timedelta. Positive offset
+            shifts a grid to the right.
+          mode (Literal["start", "end", "end_inclusive"]): defines truncating
+            mode:
+             * "start" returns period start;
+             * "end" returns a start of the next period, complies with default
+               interval definition where start is inclusive and end is not;
+             * "end_inclusive" returns the end of the current interval
+
+        Desired datetime grid is defined by step and offset, passed as either a
+        STEP-STRING (see below) or a `datetime.timedelta`.
         It also supports multiple modes of truncating dates.
 
         >>> conversion.date_trunc("1mo")
         >>> conversion.date_trunc("3mo", "1mo")
         >>> conversion.date_trunc("3mo", "1mo", mode="end_inclusive")
 
         STEP-STRING is a string which is comprised of numbers and suffixes:
@@ -1052,68 +1101,74 @@
          - m: minute
          - s: second
          - ms: millisecond
          - us: microsecond
 
         so -2d8h10us means minus 2 days 8 hours and 10 microseconds.
 
-        WARNING:
+        Warning:
          * y/mo support only y/mo as offsets
          * days of week don't support offsets
          * as this method truncates dates, not datetimes, it accepts only whole
            number of days as steps and offsets
 
-        Args:
-          step: defines period length. If it's a year, month or a day of week,
-            it defines beginnings of periods too.
-          offset (optional): defines the shift of the expected date grid
-            relative to 0-point. Positive offset shifts a grid to the right.
-          mode (Literal["start", "end", "end_inclusive"]): defines truncating
-            mode: "start" returns period start; "end" returns a start of the
-            next period, complies with default interval definition where start
-            is inclusive and end is not; "end_inclusive" returns the end of the
-            current interval
 
         """
-        step = to_step(step)
-        mode = TruncModes.to_internal(mode)
+        from convtools import _dt
+
+        step = _dt.to_step(step)
+        mode = _dt.TruncModes.to_internal(mode)
         if offset is not None:
-            offset = to_step(offset)
-        if isinstance(step, MonthStep):
+            offset = _dt.to_step(offset)
+        if isinstance(step, _dt.MonthStep):
             return CallFunc(
-                date_trunc_to_month,
+                _dt.date_trunc_to_month,
                 self,
                 step.to_months(),
                 0 if offset is None else offset.to_months(),
                 mode,
             )
-        elif isinstance(step, DayOfWeekStep):
+        elif isinstance(step, _dt.DayOfWeekStep):
             if offset is not None:
                 raise ValueError(
                     "offsets are not applicable to day-of-week steps"
                 )
             return CallFunc(
-                date_trunc_to_day,
+                _dt.date_trunc_to_day,
                 self,
                 step.to_days(),
                 step.day_of_week_offset,
                 mode,
             )
         return CallFunc(
-            date_trunc_to_day,
+            _dt.date_trunc_to_day,
             self,
             step.to_days(),
             0 if offset is None else offset.to_days(),
             mode,
         )
 
     def datetime_trunc(self, step, offset=None, mode="start"):
-        """Truncates a date to periods of certain length, specified by step and
-        offset, passed as either a STEP-STRING (see below) or a
-        :py:obj:`datetime.timedelta`.
+        """Truncate datetime.
+
+        Args:
+          step: defines period length as STEP-STRING or a timedelta. If it's a
+            year, month or a day of week, it defines beginnings of periods too.
+          offset (optional): defines the shift of the expected date grid
+            relative to 0-point as STEP-STRING or a timedelta. Positive offset
+            shifts a grid to the right.
+          mode (Literal["start", "end", "end_inclusive"]): defines truncating
+            mode:
+             * "start" returns period start;
+             * "end" returns a start of the next period, complies with default
+               interval definition where start is inclusive and end is not;
+             * "end_inclusive" returns the end of the current interval
+
+        Desired datetime grid is defined by step and offset, passed as either a
+        STEP-STRING (see below) or a `datetime.timedelta`.
         It also supports multiple modes of truncating dates.
 
         >>> conversion.datetime_trunc("1mo")
         >>> conversion.datetime_trunc("3mo", "1mo")
         >>> conversion.datetime_trunc("3mo", "1mo", mode="end_inclusive")
 
         STEP-STRING is a string which is comprised of numbers and suffixes:
@@ -1125,94 +1180,105 @@
          - m: minute
          - s: second
          - ms: millisecond
          - us: microsecond
 
         so "-2d8h10us" means minus 2 days 8 hours and 10 microseconds.
 
-        WARNING:
+        Warning:
+        -------
          * y/mo support only y/mo as offsets
          * days of week don't support offsets
          * any steps defined as deterministic units (d, h, m, s, ms, us) can
            only be used with offsets defined by deterministic units too
 
-        Args:
-          step: defines period length. If it's a year, month or a day of week,
-            it defines beginnings of periods too.
-          offset (optional): defines the shift of the expected date grid
-            relative to 0-point. Positive offset shifts a grid to the right.
-          mode (Literal["start", "end", "end_inclusive"]): defines truncating
-            mode: "start" returns period start; "end" returns a start of the
-            next period, complies with default interval definition where start
-            is inclusive and end is not; "end_inclusive" returns the end of the
-            current interval
         """
-        step = to_step(step)
-        mode = TruncModes.to_internal(mode)
+        from convtools import _dt
+
+        step = _dt.to_step(step)
+        mode = _dt.TruncModes.to_internal(mode)
         if offset is not None:
-            offset = to_step(offset)
+            offset = _dt.to_step(offset)
 
-        if isinstance(step, MonthStep):
+        if isinstance(step, _dt.MonthStep):
             return CallFunc(
-                datetime_trunc_to_month,
+                _dt.datetime_trunc_to_month,
                 self,
                 step.to_months(),
                 0 if offset is None else offset.to_months(),
                 mode,
             )
 
-        elif isinstance(step, DayOfWeekStep):
+        elif isinstance(step, _dt.DayOfWeekStep):
             if offset is not None:
                 raise ValueError(
                     "offsets are not applicable to day-of-week steps"
                 )
             return CallFunc(
-                datetime_trunc_to_day,
+                _dt.datetime_trunc_to_day,
                 self,
                 step.to_days(),
                 step.day_of_week_offset,
                 mode,
             )
 
         if step.can_be_cast_to_days() and (
             offset is None or offset.can_be_cast_to_days()
         ):
             return CallFunc(
-                datetime_trunc_to_day,
+                _dt.datetime_trunc_to_day,
                 self,
                 step.to_days(),
                 0 if offset is None else offset.to_days(),
                 mode,
             )
 
         return CallFunc(
-            datetime_trunc_to_microsecond,
+            _dt.datetime_trunc_to_microsecond,
             self,
             step.to_us(),
             0 if offset is None else offset.to_us(),
             mode,
         )
 
+    def format_dt(self, fmt: str):
+        """datetime.strftime with certain cases optimized for speed."""
+        if fmt == "%Y-%m-%d":
+            return If(
+                CallFunc(isinstance, self, datetime),
+                self.call_method("date").call_method("isoformat"),
+                self.call_method("isoformat"),
+            )
+        from convtools import _dt
+
+        return self.pipe(_dt.DatetimeFormat(fmt))
+
     def expect(self, condition, error_msg=None):
-        """Checks condition and return the input as is. If condition is not
-        met, raises ExpectException with error_msg (can be conversion too) as
-        param"""
-        return convtools_expect.Expect(self, condition, error_msg)
+        """Check condition and return the input as is or raise ExpectException.
+
+        Args:
+          condition: conversion to evaluate as condition
+          error_msg: error message to pass to ExpectException
+        """
+        from convtools import _expect
+
+        return _expect.Expect(self, condition, error_msg)
 
 
 class BaseMutation(BaseConversion):
     used_in_narrow_context = True
     weight = Weights.FUNCTION_CALL
 
 
 class BaseMethodConversion(BaseConversion):
-    """This conversion is required to take into account method calls.  We need
-    to preserve the instance we are calling a method on.
+    """Base conversion to method calls / attr / dict lookups.
 
-    e.g. like obj['key'] OR obj.func() OR obj.attr1"""
+    We need to preserve the instance we are calling a method on.
+    e.g. like obj['key'] OR obj.func() OR obj.attr1
+    """
 
     def __init__(self, self_conv):
         super().__init__()
         self.self_conv = (
             self_conv
             if self_conv is self._none
             else self.ensure_conversion(self_conv)
@@ -1242,32 +1308,35 @@
     return s
 
 
 NOT_NONE_FUNCS = {sum, min, max, len, int, float, Decimal}
 
 
 class NaiveConversion(BaseConversion):
-    """Naive conversion gets compiled into the code, which just returns the
-    `value` it's been initialized with.  Allows to make any object available
-    inside other conversions.
+    """Make outer variable available to code, to be generated.
+
+    During code generation phase, it names a value and passes it to
+    globals/locals of the generated code. Any object is passed as is.
     """
 
     _builtin_dict = get_builtins_dict()
     self_content_type = (
         BaseConversion.self_content_type
         & ~BaseConversion.ContentTypes.FUNCTION_OF_INPUT
     )
 
     types_to_repr = {type(None), bool, int}
     weight = Weights.STEP
 
     def __init__(self, value: t.Any, name_prefix="v"):
-        """
+        """Initialize instance.
+
         Args:
-          value (object): any object
+          value: any object to be exposed to generated code
+          name_prefix (str): prefix to be used
 
         """
         super().__init__()
         self.value = value
         self.name_prefix = name_prefix
         self.code_str = None
 
@@ -1335,16 +1404,15 @@
             conversion.value
             if isinstance(conversion, NaiveConversion)
             else conversion
         )
 
 
 class EscapedString(BaseConversion):
-    """Defines the conversion which returns the result of running the
-    python code, passed to init"""
+    """Pass code as is to the resulting generated code."""
 
     self_content_type = (
         BaseConversion.self_content_type
         & ~BaseConversion.ContentTypes.FUNCTION_OF_INPUT
     )
     weight = Weights.STEP
 
@@ -1353,88 +1421,116 @@
         self.s = s
 
     def _gen_code_and_update_ctx(self, code_input, ctx):
         return self.s
 
 
 class ThisConversion(BaseConversion):
-    """Defines the conversion which just returns the input.
+    """Identity conversion (just returns the input).
 
     Also, provided that you use this inside comprehension conversions,
-    it references an item from an iterator."""
+    it references an item from an iterator.
+    """
 
     weight = 0
 
     def __call__(self) -> "ThisConversion":
-        """To allow using it as singleton"""
+        """To allow using it as singleton."""
         return self
 
     def _gen_code_and_update_ctx(self, code_input, ctx):
         return code_input
 
+    def pipe(
+        self,
+        next_conversion,
+        *args,
+        label_input=None,
+        label_output=None,
+        **kwargs,
+    ) -> "BaseConversion":
+        """Pass the result of one conversion as an input to another.
+
+        If `next_conversion` is callable, it gets called with the previous result
+        passed as the first param.
+
+        Supports predicate/sorting/type casting push down (each is directly applied
+        to the ``where`` conversion.
+
+        Supports labeling both pipe input and output data (allows to apply
+        conversions before labeling).
+        """
+        next_conversion = ensure_conversion(next_conversion)
+        if (
+            label_input is None
+            and label_output is None
+            and not args
+            and not kwargs
+            and not next_conversion.is_itself_callable()
+        ):
+            return next_conversion
+
+        return super().pipe(
+            next_conversion,
+            *args,
+            label_input=label_input,
+            label_output=label_output,
+            **kwargs,
+        )
+
 
 This = ThisConversion()
 
 
 class InputArg(BaseConversion):
-    """Allows to use arguments passed into the compiled converter.
+    """Use argument, passed into the compiled converter.
 
     Unless the `signature` argument is passed to `gen_converter` function, all
     input arguments used in the conversion definition will be expected as
-    keyword-only arguments (affecting the resulting converter signature)."""
+    keyword-only arguments (affecting the resulting converter signature).
+    """
 
     self_content_type = (
         BaseConversion.self_content_type
         | BaseConversion.ContentTypes.ARG_USAGE
     ) & ~BaseConversion.ContentTypes.FUNCTION_OF_INPUT
     trackable_dependency = True
     weight = Weights.STEP
 
     def __init__(self, name: str):
-        """
-        Args:
-          name (string): argument name of the converter to be used
-        """
         super().__init__()
         self.name = name
 
     def _gen_code_and_update_ctx(self, code_input, ctx):
         return self.name
 
 
 class LabelConversion(BaseConversion):
-    """Allows to reference a conversion result by label, after it was cached by
-    :py:obj:`PipeConversion` or :py:obj:`BaseConversion.add_label`."""
+    """Use data, previously labeled by `add_label` or `pipe`."""
 
     self_content_type = (
         BaseConversion.self_content_type
         | BaseConversion.ContentTypes.LABEL_USAGE
     ) & ~BaseConversion.ContentTypes.FUNCTION_OF_INPUT
     weight = Weights.DICT_LOOKUP
 
     labels_code_name = "_labels"
 
     def __init__(self, label_name: str):
-        """
-        Args:
-          label_name (string): label name to be referenced
-        """
         super().__init__()
         if not isinstance(label_name, str):
             raise ValueError("invalid label_name type")
         self.label_name = label_name
 
     def _gen_code_and_update_ctx(self, code_input, ctx):
         return f"{self.labels_code_name}[{repr(self.label_name)}]"
 
 
 class Namespace(BaseConversion):
-    """Wrapping conversion which isolates :py:obj:`LazyEscapedString` (parent
-    conversions won't detect them as dependencies) and defines code inputs for
-    them"""
+    """Wrap conversion to hide `LazyEscapedString` from parents."""
 
     weight = 0
     self_content_type = (
         BaseConversion.self_content_type
         & ~BaseConversion.ContentTypes.FUNCTION_OF_INPUT
     )
 
@@ -1457,24 +1553,23 @@
             and dependency.name in self.name_to_code
         ):
             return False
         return super().is_dependency_trackable(dependency)
 
 
 class FunctionCtx:
-    """Defines a code generation context for a conversion, which is to help
-    with wrapping a conversion code in a function so that all required
-    arguments are both defines as parameters and passed properly. It also helps
-    with adding additional parameters.
-
-    Another important thing is that some parameters like LazyEscapedString are
-    renamed and replaced with arguments of the new function. So it ensures (see
-    prevent_rendering_while_active) that those lazy strings are not generating
-    code while we are building inner function code (they just won't be
-    available there).
+    """Helper context to wrap generated code with a function.
+
+    It ensures required input args, label helpers and other variables are
+    correctly passed to the generated function.
+
+    It also replaces LazyEscapedString with new names (function parameters) and
+    ensures (see prevent_rendering_while_active) that those lazy strings are
+    not generating code while we are building inner function code (they are
+    just not available there).
     """
 
     def __init__(
         self,
         conversion,
         ctx,
         args_as_def_names,
@@ -1559,16 +1654,15 @@
 
     def __exit__(self, exc_type, exc_value, exc_traceback):
         self.ctx[BaseConversion.NAIVE_TO_WARM_UP] = self.prev_names_to_warm_up
         return self.namespace_ctx.__exit__(exc_type, exc_value, exc_traceback)
 
 
 class NamespaceCtx:
-    """Context manager which defines code inputs for
-    :py:obj:`LazyEscapedString`"""
+    """Context manager which defines code inputs for `LazyEscapedString`."""
 
     _name_to_code = None
     ctx = None
     active = False
 
     NAMESPACES = BaseConversion.NAMESPACES
 
@@ -1601,16 +1695,15 @@
         return ctx[cls.NAMESPACES][-1]
 
     def prevent_rendering_while_active(self, conversion):
         return NamespaceControlledUnit(self, conversion)
 
 
 class NamespaceControlledUnit(BaseConversion):
-    """Wrapping conversion which prevents the inner one from being rendered
-    while it is inside the parent NamespaceCtx"""
+    """Wrapper which conditionally prevents inner conversion from rendering."""
 
     __slots__ = ["conversion", "namespace_ctx"]
     weight = 0
 
     def __init__(self, namespace_ctx: "NamespaceCtx", conversion):
         super().__init__()
         self.namespace_ctx = namespace_ctx
@@ -1622,17 +1715,21 @@
                 "rendering prevented by parent NamespaceCtx, "
                 "move rendering out"
             )
         return self.conversion.gen_code_and_update_ctx(code_input, ctx)
 
 
 class LazyEscapedString(BaseConversion):
-    """A lazy named conversion which allows to build a conversion on the
-    outside to then generate some code around it (properly passing required
-    args, etc.)"""
+    """Lazily defined named conversion.
+
+    It allows to expose conversion primitives to the user, so the one can use
+    them define a custom conversion, which will be embedded into different
+    conversions (properly passing required args, etc.; e.g. see joins /
+    cumulative).
+    """
 
     self_content_type = (
         BaseConversion.self_content_type
         & ~BaseConversion.ContentTypes.FUNCTION_OF_INPUT
     )
     trackable_dependency = True
     weight = Weights.STEP
@@ -1651,26 +1748,27 @@
                 return code
             raise AssertionError("it's a bug")
 
         raise ValueError("LazyEscapedString is left uninitialized", self.name)
 
 
 class OrAndEqBaseConversion(BaseConversion):
-    """Base class of Or/And/Eq operator conversions"""
+    """Base class of Or/And/Eq operator conversions."""
 
     self_content_type = (
         BaseConversion.self_content_type
         & ~BaseConversion.ContentTypes.FUNCTION_OF_INPUT
     )
 
     op = ""
     weight = Weights.LOGICAL
 
     def __init__(self, *args, default=None):
-        """
+        """Initialize operator.
+
         Args:
             args: conditions
             default: defines behavior when args is empty
               - if None, empty args will raise ValueError
               - false values - results in False
               - true values - results in True
         """
@@ -1689,81 +1787,70 @@
         code = self.op.join(
             [arg.gen_code_and_update_ctx(code_input, ctx) for arg in self.args]
         )
         return f"({code})"
 
 
 class Or(OrAndEqBaseConversion):
-    """Takes any number of objects, each is to be wrapped with
-    :py:obj:`ensure_conversion` and generates the code
-    joining every argument with python ``or`` expression
+    """Join params with `or` expression; supports default.
 
     ``default`` defines behavior when args is empty
       * if None is empty will raise ValueError
       * false values - results in False
       * true values - results in True
 
     """
 
     op = " or "
 
 
 class And(OrAndEqBaseConversion):
-    """Takes any number of objects, each is to be wrapped with
-    :py:obj:`ensure_conversion` and generates the code
-    joining every argument with python ``and`` expression.
+    """Join params with `and` expression; supports default.
 
     ``default`` defines behavior when args is empty
       * if None is empty will raise ValueError
       * false values - results in False
       * true values - results in True
 
     """
 
     op = " and "
 
 
 class Eq(OrAndEqBaseConversion):
-    """Takes any number of objects, each is to be wrapped with
-    :py:obj:`ensure_conversion` and generates the code
-    joining every argument with python `` == `` operator
+    """Join params with `==` expression; supports default.
 
     ``default`` defines behavior when args is empty
       * if None is empty will raise ValueError
       * false values - results in False
       * true values - results in True
 
     """
 
     op = " == "
 
 
 class If(BaseConversion):
-    """Generates the if expression code.
-
-    Checks the code of the input, if it
-    doesn't seem to be complex, then just proceeds with it as is.
-    If it's not simple (some index/attribute lookups or function calls are
-    in there), then it caches the input for further reuse in if_true and
-    if_false clauses."""
+    """Define conditional expression."""
 
     self_content_type = (
         BaseConversion.self_content_type
         & ~BaseConversion.ContentTypes.FUNCTION_OF_INPUT
     )
     weight = Weights.STEP
 
     def __init__(
         self,
         condition=True,
         if_true=BaseConversion._none,
         if_false=BaseConversion._none,
         no_input_caching=False,
     ):
-        """
+        """Initialize conditional expression.
+
         Args:
           condition (object): condition for the IF expression. If it is left as
             True, then the input is used as the condition.
           if_true (object): the result if the condition is true
           if_false (object): the result if the condition is false
           no_input_caching (bool): if True, disables automatic decision making
             on whether result caching is needed
@@ -1799,16 +1886,15 @@
         self.conversion = self.ensure_conversion(conversion)
 
     def _gen_code_and_update_ctx(self, code_input, ctx):
         return self.conversion.gen_code_and_update_ctx(code_input, ctx)
 
 
 class IfMultiple(BaseConversion):
-    """Builds a short-circuit conversion, which evaluates multiple conversions
-    and stops at first true one:
+    """Build a short-circuit conversion, which stops at first true value.
 
     >>> converter = c.if_multiple(
     >>>     (c.this < 10, c.this / 2),
     >>>     (c.this == 10, None),
     >>>     else_=c.this * 2
     >>> ).gen_converter()
 
@@ -1824,14 +1910,21 @@
 
     self_content_type = (
         BaseConversion.self_content_type
         & ~BaseConversion.ContentTypes.FUNCTION_OF_INPUT
     )
 
     def __init__(self, *condition_to_value_pairs, else_):
+        """Initialize IfMultiple.
+
+        Args:
+          condition_to_value_pairs: sequence of tuples ({condition},
+            {result-to-return})
+          else_: default to return if no conditions evaluated to true.
+        """
         super().__init__()
         self.condition_to_value_pairs = [
             (self.ensure_conversion(condition), self.ensure_conversion(value))
             for condition, value in condition_to_value_pairs
         ]
         self.else_ = self.ensure_conversion(else_)
 
@@ -1862,15 +1955,15 @@
             )
         return function_ctx.call_with_all_args(
             conversion
         ).gen_code_and_update_ctx(code_input, ctx)
 
 
 class Not(BaseConversion):
-    """Conversion which applies not operator to its input"""
+    """Apply `not` operator."""
 
     self_content_type = (
         BaseConversion.self_content_type
         & ~BaseConversion.ContentTypes.FUNCTION_OF_INPUT
     )
     weight = Weights.LOGICAL
 
@@ -1880,30 +1973,41 @@
 
     def _gen_code_and_update_ctx(self, code_input, ctx):
         code = self.arg.gen_code_and_update_ctx(code_input, ctx)
         return f"(not {code})"
 
 
 class InlineExpr(BaseConversion):
-    """This conversion allows to avoid function call overhead.  It inlines a
-    raw python code expression into the code of resulting conversion."""
+    """str-format for code generation.
+
+    The main use case is to avoid function call overhead. It inlines a raw
+    python code expression into the code of resulting conversion.
+
+    Example:
+    c.inline_expr("[j for i in {} for j in i]").pass_args(c.this)
+    """
 
     self_content_type = (
         BaseConversion.self_content_type
         & ~BaseConversion.ContentTypes.FUNCTION_OF_INPUT
     )
 
     def __init__(
         self, code_str, weight=Weights.UNPREDICTABLE, args=None, kwargs=None
     ):
-        """
+        """Initialize InlineExpr.
+
         Args:
-          code_str (str): python code string. Supports `{}` expressions of
-            :py:obj:`str.format`, both positional and names ones.
-            To pass arguments, use :py:obj:`InlineExpr.pass_args`
+          code_str (str): python code string. Uses `str.format` syntax - `{}`,
+            both positional and names ones. To pass arguments, use
+            `InlineExpr.pass_args` method.
+          weight: do not use it
+          args: args to pass right away, without deferring to pass_args
+          kwargs: kwargs to pass right away, without deferring to pass_args
+
         """
         self.weight = weight
         super().__init__()
         self.code_str = code_str
         self.args = (
             [self.ensure_conversion(arg) for arg in args] if args else []
         )
@@ -1983,21 +2087,20 @@
         return {get_or_default_code}
     except AttributeError:
         return {default_code}
 """
 
 
 class GetItem(BaseMethodConversion):
-    """``GetItem`` gets compiled into the code which does
-    dictionary/index lookups.
-
-    If called without params, just returns the input.
+    """Any number of dict/index lookups.
 
+    If called without params, it just returns the input.
     If an index is a conversion itself, then it is being calculated
-    against an input."""
+    against an input.
+    """
 
     prefix = "item_or_default"
     weight = Weights.DICT_LOOKUP
     caching_is_possible = True
     template = GET_ITEM_OR_DEFAULT_TEMPLATE
 
     get_or_default_functions = [
@@ -2009,19 +2112,21 @@
 
     def __init__(
         self,
         *indexes,
         default=BaseConversion._none,
         self_conv=BaseConversion._none,
     ):
-        """
+        """Initialize self.
+
         Args:
-          indexes (:obj:`list` of :obj:`object`): to do lookups with
-          default (:obj:`object`, optional): to be returned on fail,
-           like ``{}.get`` method, but now applicable to arrays too
+          indexes: sequence of indexes/key
+          default (optional): obj/conversion to be returned on fail,
+            like ``{}.get`` method, but applicable to lists too.
+          self_conv: do not use it, it is populated automatically.
         """
         super().__init__(self_conv)
         self.indexes = [self.ensure_conversion(index) for index in indexes]
         self.default = (
             self.ensure_conversion(default)
             if default is not self._none
             else None
@@ -2125,15 +2230,15 @@
                 for i, index in enumerate(self.indexes):
                     var_index = f"index_{i}"
                     function_ctx.add_arg(var_index, index)
                     code_output = self.wrap_path_item(code_output, var_index)
 
             else:
                 do_caching = False
-                for i, index in enumerate(self.indexes):
+                for _, index in enumerate(self.indexes):
                     code_output = self.wrap_path_item(
                         code_output,
                         index.gen_code_and_update_ctx("data_", ctx),
                     )
 
             key = (
                 (
@@ -2163,19 +2268,20 @@
 
         return function_ctx.call_with_all_args(
             EscapedString(converter_name)
         ).gen_code_and_update_ctx(code_input, ctx)
 
 
 class GetAttr(GetItem):
-    """``GetAttr`` gets compiled into the code which runs getattr.
-    If called without params, just returns the input.
+    """Any number of attr lookups.
 
-    If an index is a conversion itself, then it is being calculated
-    against an input."""
+    If called without params, it just returns the input.
+    If an attr is a conversion itself, then it is being calculated
+    against an input.
+    """
 
     valid_attr = re.compile(r"^'[A-Za-z_][a-zA-Z0-9_]*'$")
     prefix = "attr_or_default"
     weight = Weights.ATTR_LOOKUP
     caching_is_possible = False
     template = GET_ATTR_OR_DEFAULT_TEMPLATE
 
@@ -2185,16 +2291,16 @@
         return f"getattr({code_input}, {path_item})"
 
     def get_hardcoded_version(self):
         return
 
 
 class Call(BaseMethodConversion):
-    """This conversion writes the code which takes the input code and calls it
-    as a function.
+    """Call __call__ of the input.
+
     It takes both positional and keyword arguments to be passed.
     """
 
     self_content_type = (
         BaseConversion.self_content_type
         & ~BaseConversion.ContentTypes.FUNCTION_OF_INPUT
     )
@@ -2221,39 +2327,40 @@
                 for k, v in self.kwargs.items()
             ),
         )
         return f"{code_self}({','.join(params)})"
 
 
 def CallFunc(func, *args, **kwargs) -> "Call":  # pylint:disable=invalid-name
-    """Shortcut to ``NaiveConversion(func).call(*args, **kwargs)``"""
+    """Shortcut to `c.naive(func).call(*args, **kwargs)`."""
     assert callable(func)
     return NaiveConversion(func).call(*args, **kwargs)
 
 
 def ApplyFunc(  # pylint:disable=invalid-name
     func, args, kwargs
 ) -> "InlineExpr":
-    """Shortcut to ``NaiveConversion(func).apply(args, kwargs)``"""
+    """Shortcut to `c.naive(func).apply(args, kwargs)`."""
     if args:
         if kwargs:
             return InlineExpr("{}(*{}, **{})").pass_args(func, args, kwargs)
         return InlineExpr("{}(*{})").pass_args(func, args)
 
     if kwargs:
         return InlineExpr("{}(**{})").pass_args(func, kwargs)
 
     return InlineExpr("{}()").pass_args(func)
 
 
 class SortConversion(BaseConversion):
-    """Generates the code to sort the input."""
+    """Shortcut for CallFunc(sorted, self, key=key, reverse=reverse)."""
 
     def __init__(self, key=None, reverse=False):
-        """
+        """Initialize SortConversion.
+
         Args:
           key (callable): to be passed to :py:obj:`sorted`
           reverse (bool): to be passed to :py:obj:`sorted`
         """
         super().__init__()
         self.sorted_kwargs = {}
         if key is not None:
@@ -2266,16 +2373,15 @@
             EscapedString("sorted")
             .call(EscapedString(code_input), **self.sorted_kwargs)
             .gen_code_and_update_ctx("NOT_NEEDED_OR_BUG", ctx)
         )
 
 
 class GeneratorItem:
-    """Internal use only - defines a conversion of each element of a
-    comprehension"""
+    """Internal use only: element of generator comprehension."""
 
     __slots__ = ["item", "custom_for_params"]
 
     def __init__(self, item, *custom_for_params):
         self.item = ensure_conversion(item)
         self.custom_for_params = tuple(
             ensure_conversion(param) for param in custom_for_params
@@ -2288,30 +2394,29 @@
         return cls(item)
 
     def _replace(self, item):
         return GeneratorItem(item, *self.custom_for_params)
 
 
 class BaseComp(BaseMethodConversion):
-    """Base conversion of non-dict comprehension"""
+    """Base non-dict comprehension."""
 
     def __init__(
         self,
         generator_item,
         where,
         self_conv,
     ):
-        """
+        """Initialize self.
+
         Args:
-          item (object): to be wrapped with :py:obj:`ensure_conversion`
+          generator_item (object): to be wrapped with :py:obj:`ensure_conversion`
             and used as a conversion on each item of a collection.
           where: conversion to be used in ``if`` clause of a comprehension
-
-            e.g. for ``[i * 2 for i in l if i > 0]`` an item would be
-            ``c.generator_comp(c.this * 2, where=c.this > 0)``
+          self_conv: do not use. It is populated automatically.
         """
         super().__init__(self_conv)
 
         self.generator_item = GeneratorItem.ensure_type(generator_item)
         self.depends_on(self.generator_item.item)
 
         for param in self.generator_item.custom_for_params:
@@ -2403,15 +2508,15 @@
             return SetComp(
                 self.generator_item, where=self.where, self_conv=self.self_conv
             )
         return super().as_type(callable_)
 
 
 class SetComp(BaseComp):
-    """Generates python set comprehension code (obviously non-sortable)"""
+    """Set comprehension."""
 
     base_type_to_cast = set
 
     def _gen_code_and_update_ctx(self, code_input, ctx):
         item_code, param_code = self.get_item_n_param_codes(ctx)
         code_iterable = self.get_iterable_code(code_input, ctx)
 
@@ -2424,15 +2529,15 @@
     def as_type(self, callable_):
         if NaiveConversion.get_value(callable_) is set:
             return self
         return super().as_type(callable_)
 
 
 class ListComp(BaseComp):
-    """Generates python list comprehension code."""
+    """List comprehension."""
 
     base_type_to_cast = list
 
     def _gen_code_and_update_ctx(self, code_input, ctx):
         item_code, param_code = self.get_item_n_param_codes(ctx)
         code_iterable = self.get_iterable_code(code_input, ctx)
 
@@ -2484,23 +2589,26 @@
         return self.to_iter().as_type(callable_)
 
     def sort(self, key=None, reverse=False) -> "BaseConversion":
         return self.to_iter().sort(key, reverse).as_type(tuple)
 
 
 class DictComp(BaseMethodConversion):
-    """Generates python dict comprehension code."""
+    """Dict comprehension."""
 
     def __init__(self, key, value, where, self_conv):
-        """
+        """Initialize self.
+
         Args:
           key (object): to be wrapped with :py:obj:`ensure_conversion` and
             used on each item of a collection to form keys
           value (object): to be wrapped with :py:obj:`ensure_conversion` and
             used on each item of a collection to form values
+          where: conversion to be used in ``if`` clause of a comprehension
+          self_conv: do not use. It is populated automatically.
         """
         super().__init__(self_conv)
         self.key = self.ensure_conversion(key)
         self.value = self.ensure_conversion(value)
         self.where: "t.Union[_None, BaseConversion]" = (
             _none
             if (where is None or where is _none)
@@ -2529,26 +2637,27 @@
         return self.call_method("items").filter(condition_conv, cast=dict)
 
     def sort(self, key=None, reverse=False) -> "BaseConversion":
         return self.call_method("items").sort(key, reverse).as_type(dict)
 
 
 class BaseCollectionConversion(BaseConversion):
-    """This is a base conversion of every collection"""
+    """This is a base conversion of every collection."""
 
     self_content_type = (
         BaseConversion.self_content_type
         & ~BaseConversion.ContentTypes.FUNCTION_OF_INPUT
     )
     conversions: t.Optional[t.List[BaseConversion]] = None
     pairs: t.Optional[t.List[t.Tuple[BaseConversion, BaseConversion]]] = None
     conditions: t.Optional[t.Mapping[int, BaseConversion]] = None
 
     def __init__(self, *items):
-        """
+        """Initialize self.
+
         Args:
           items (objects): items to form a collection from.
             every item gets wrapped with :py:obj:`ensure_conversion`
         """
         super().__init__()
         self._init_from_items(items)
 
@@ -2662,30 +2771,30 @@
         joined_items_code = self.gen_joined_items_code(code_input, ctx)
         return self.gen_collection_from_items_code(
             joined_items_code, code_input, ctx
         )
 
 
 class OptionalCollectionItem(BaseConversion):
-    """Wrapping conversion which makes key/value/item of a collection
-    optional."""
+    """Make collection item optional, so it conditionally disappears."""
 
     valid_pipe_output = False
 
     condition: BaseConversion
     conversion: BaseConversion
 
     def __init__(
         self,
         conversion,
         skip_value=None,
         skip_if=BaseConversion._none,
         keep_if=BaseConversion._none,
     ):
-        """
+        """Init self.
+
         Args:
           conversion (BaseConversion): conversion to be wrapped
           skip_value: value to compare with conversion result and to be
             excluded from the collection
           skip_if: a condition to be checked; if it resolves to True, then the
             item gets excluded from the collection
           keep_if: a condition to be checked; if it resolves to False, then the
@@ -2699,30 +2808,29 @@
             raise ValueError("both condition and skip_value are passed")
         self.conversion = self.ensure_conversion(conversion)
         if condition_is_passed:
             if skip_if is not self._none:
                 self.condition = Not(self.ensure_conversion(skip_if))
             if keep_if is not self._none:
                 self.condition = self.ensure_conversion(keep_if)
+        elif skip_value is None:
+            self.condition = self.conversion.is_not(None)
         else:
-            if skip_value is None:
-                self.condition = self.conversion.is_not(None)
-            else:
-                self.condition = self.conversion != self.ensure_conversion(
-                    skip_value
-                )
+            self.condition = self.conversion != self.ensure_conversion(
+                skip_value
+            )
 
     def _gen_code_and_update_ctx(self, code_input, ctx):
         raise AssertionError(
             "OptionalCollectionItem cannot be used outside of collections"
         )
 
 
 class Tuple(BaseCollectionConversion):
-    """Gets compiled into the code which generates a tuple"""
+    """Define tuple."""
 
     weight = Weights.TUPLE_INIT
 
     def gen_collection_from_items_code(
         self, joined_items_code, code_input, ctx
     ):
         if not joined_items_code:
@@ -2730,53 +2838,53 @@
         return f"({joined_items_code},)"
 
     def gen_collection_from_generator(self, generator_code, code_input, ctx):
         return f"tuple({generator_code})"
 
 
 class List(BaseCollectionConversion):
-    """Gets compiled into the code which generates a list"""
+    """Define list."""
 
     weight = Weights.LIST_INIT
 
     def gen_collection_from_items_code(
         self, joined_items_code, code_input, ctx
     ):
         return f"[{joined_items_code}]"
 
     def gen_collection_from_generator(self, generator_code, code_input, ctx):
         return f"list({generator_code})"
 
 
 class Set(BaseCollectionConversion):
-    """Gets compiled into the code which generates a set"""
+    """Define set."""
 
     weight = Weights.SET_INIT
 
     def gen_collection_from_items_code(
         self, joined_items_code, code_input, ctx
     ):
         return f"{{{joined_items_code}}}"
 
     def gen_collection_from_generator(self, generator_code, code_input, ctx):
         return f"set({generator_code})"
 
 
 class Dict(BaseCollectionConversion):
-    """Gets compiled into the code which generates a dict"""
+    """Define dict."""
 
     weight = Weights.DICT_INIT
 
     def _init_from_items(self, items):
         pairs: "t.List[t.Tuple[BaseConversion, BaseConversion]]" = []
         conditions = None
 
-        for key, value in items:
-            key = self.ensure_conversion(key)
-            value = self.ensure_conversion(value)
+        for raw_key, raw_value in items:
+            key = self.ensure_conversion(raw_key)
+            value = self.ensure_conversion(raw_value)
             condition = None
 
             if isinstance(key, OptionalCollectionItem):
                 condition = key.condition
                 key = key.conversion
 
             if isinstance(value, OptionalCollectionItem):
@@ -2811,15 +2919,15 @@
     def gen_collection_from_items_code(
         self, joined_items_code, code_input, ctx
     ):
         return f"{{{joined_items_code}}}"
 
 
 class TakeWhile(BaseConversion):
-    """convtools implementation of :py:obj:`itertools.takewhile`"""
+    """Faster `itertools.takewhile`."""
 
     def __init__(self, condition):
         super().__init__()
         self.condition = self.ensure_conversion(condition)
         self.filter_results_conditions = None
         self.cast = self._none
 
@@ -2874,15 +2982,15 @@
         conversion = function_ctx.call_with_all_args(conversion)
         if self.cast is not self._none:
             conversion = conversion.as_type(self.cast)
         return conversion.gen_code_and_update_ctx(code_input, ctx)
 
 
 class DropWhile(BaseConversion):
-    """convtools implementation of :py:obj:`itertools.dropwhile`"""
+    """Faster `itertools.dropwhile`."""
 
     def __init__(self, condition):
         super().__init__()
         self.condition = self.ensure_conversion(condition)
         self.filter_results_conditions = None
         self.cast = self._none
 
@@ -2952,43 +3060,46 @@
             return self._replace(getattr(self.where, name)(*args, **kwargs))
         return getattr(super(self.__class__, self), name)(*args, **kwargs)
 
     return method
 
 
 class PipeConversion(BaseConversion):
-    """Passes the result of one conversion as an input to another.  If
-    `next_conversion` is callable, it gets called with the previous result
+    """Pass the result of one conversion as an input to another.
+
+    If `next_conversion` is callable, it gets called with the previous result
     passed as the first param.
 
     Supports predicate/sorting/type casting push down (each is directly applied
     to the ``where`` conversion.
 
     Supports labeling both pipe input and output data (allows to apply
-    conversions before labeling)."""
+    conversions before labeling).
+    """
 
     weight = 0
     self_content_type = (
         BaseConversion.self_content_type
     ) & ~BaseConversion.ContentTypes.FUNCTION_OF_INPUT
 
     def __init__(
         self,
-        what,
-        where,
+        what: Any,
+        where: Any,
         *args,
         label_input=None,
         label_output=None,
         **kwargs,
     ):
-        """
+        """Init self.
 
         Args:
-          next_conversion (object): to be wrapped with
-            :py:obj:`ensure_conversion` and called if callable is passed
+          what: the 1st conversion, whose result is to be passed the `where`
+          where: the 2nd conversion, which accepts the output of `what`
+            conversion. If it is callable, it is called.
           args (tuple): to be wrapped with :py:obj:`ensure_conversion` and
             passed to `next_conversion` if it's callable
           kwargs (dict): to be wrapped with :py:obj:`ensure_conversion` and
             passed to `next_conversion` if it's callable
           label_input (str or dict): Labels to be put on pipe input data.
             If a ``str`` is passed, then it is used as a label name.
             If a ``dict`` is passed, keys are label names, values
```

### Comparing `convtools-1.4.0/convtools/_chunks.py` & `convtools-1.5.0/convtools/_chunks.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-"""
-Provides conversions for slicing iterables into chunks.
-"""
+"""Conversions for slicing iterables into chunks."""
 import typing as t
 
 from ._aggregations import Aggregate
 from ._base import BaseConversion, Code, LazyEscapedString, Namespace, This
 
 
 _none = BaseConversion._none
@@ -12,15 +10,15 @@
 
 class BaseChunkBy(BaseConversion):
     def aggregate(self, *args, **kwargs) -> "BaseConversion":
         return self.iter(Aggregate(*args, **kwargs))
 
 
 class ChunkBy(BaseChunkBy):
-    """Slices iterable into chunks by element values and/or size of chunks.
+    """Slice iterable into chunks by element values and/or size of chunks.
 
     >>> # simple #1
     >>> c.chunk_by(size=1000)
     >>>
     >>> # simple #2
     >>> c.chunk_by(c.item("x"))
     >>>
@@ -53,24 +51,24 @@
     >>> })
 
     It also provides a shortcut for running
     :py:obj:`convtools.aggregations.Aggregate` on chunks.
     """
 
     def __init__(self, *by, size: t.Optional[int] = None):
-        """
+        """Init self.
+
         Args:
           by: fields/conversions to use for slicing into chunks (elements with
             same values go to the same chunk)
           size: (optional) positive int to limit max size of a chunk
         """
         super().__init__()
-        if size is not None:
-            if not isinstance(size, int) or size <= 0:
-                raise ValueError("size has to be positive int or None")
+        if size is not None and (not isinstance(size, int) or size <= 0):
+            raise ValueError("size has to be positive int or None")
         if not by and not size:
             raise ValueError("pass at least one of by or size params")
 
         self.by = (
             (self.ensure_conversion(by if len(by) > 1 else by[0]))
             if by
             else None
@@ -180,16 +178,17 @@
             chunk_ = [item_]
 
     yield chunk_
 """
 
 
 class ChunkByCondition(BaseChunkBy):
-    """Slices iterable into chunks based on condition, which is a function of a
-    current chunk and a current element.
+    """Slices iterable into chunks based on condition.
+
+    Condition is a conversion of a current chunk and a current element.
 
     >>> # example #1
     >>> c.chunk_by_condition(c.CHUNK.len() < 100)
     >>>
     >>> # example #2
     >>> c.chunk_by_condition(
     >>>     c.and_(
```

### Comparing `convtools-1.4.0/convtools/_columns.py` & `convtools-1.5.0/convtools/_columns.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,16 @@
-"""
-Implements base conversions to reference and define columns in table
-conversions
-"""
+"""Base conversions to reference/define columns for tables."""
 import typing as t
 from collections import defaultdict
 
 from ._base import BaseConversion, ConversionException, GetItem
 
 
 class ColumnRef(BaseConversion):
-    """Helper conversion, which allows to reference a column of a table
-    conversion"""
+    """Table column reference."""
 
     trackable_dependency = True
 
     def __init__(self, name: str, id_=None):
         if not isinstance(name, str):
             raise ValueError("name should be str")
         super().__init__()
@@ -36,31 +32,31 @@
             )
         return GetItem(
             self.index if self.index is not None else -1
         ).gen_code_and_update_ctx(code_input, ctx)
 
 
 class ColumnDef:
-    """
-    Defines a column within a table conversion. It holds the following:
-
-     * name of the column in the output
-     * index of the column in the input in simple cases, otherwise None
-     * conversion to obtain the value from the input, None in simple cases
-
-    """
+    """Table column definition."""
 
     __slots__ = ["name", "index", "conversion"]
 
     def __init__(
         self,
         name: str,
         index: t.Optional[t.Any],
         conversion: t.Optional[BaseConversion],
     ):
+        """Init self.
+
+        Args:
+          name: of the column in the output
+          index: of the column in the input in simple cases, otherwise None
+          conversion: to obtain the value from the input, None in simple cases
+        """
         if not bool(index is not None) ^ bool(conversion is not None):
             raise ValueError("provide either index or conversion")
         self.name = name
         self.index = index
         self.conversion = conversion
 
     def as_tuple(self):
@@ -78,15 +74,15 @@
 class ColumnChanges:
     RENAME = 1
     REARRANGE = 2
     MUTATE = 4
 
 
 class MetaColumns:
-    """A helper container for naming & keeping column definitions"""
+    """Helper container many table columns."""
 
     def __init__(
         self,
         # t.Literal["raise", "keep", "drop", "mangle"]
         duplicate_columns="raise",
     ):
         self.columns: "t.List[ColumnDef]" = []
```

### Comparing `convtools-1.4.0/convtools/_conversion.py` & `convtools-1.5.0/convtools/_conversion.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-"""
-The main module exposing public API (via conversion object)
-"""
+"""The main module exposing public API."""
 from itertools import repeat
 
 from ._aggregations import (
     Aggregate,
     BaseReducer,
     GroupBy,
     Reduce,
@@ -46,26 +44,27 @@
     Tuple,
     TupleComp,
     ensure_conversion,
 )
 from ._chunks import ChunkBy, ChunkByCondition
 from ._columns import ColumnRef
 from ._cumulative import Cumulative
+from ._exceptions import try_multiple
 from ._expect import ExpectException
 from ._joins import JoinConversion, _JoinConditions
 from ._mutations import Mutations
 
 
 __all__ = ["conversion", "Conversion"]
 
 _none = BaseConversion._none
 
 
 class Conversion:
-    """The object, which exposes public API
+    """Central object, which exposes public API.
 
     >>> from convtools import conversion as c
     >>> convert = c.aggregate(
     >>>     c.ReduceFuncs.DictSum(
     >>>         c.item("name"),
     >>>         c.item("value")
     >>>     )
@@ -159,14 +158,18 @@
     PREV = Cumulative.PREV
     cumulative = This.cumulative
     cumulative_reset = This.cumulative_reset
 
     date_parse = This.date_parse
     datetime_parse = This.datetime_parse
 
+    format_dt = This.format_dt
+
+    try_multiple = staticmethod(try_multiple)
+
     def iter(self, item, *, where=None):
         return GeneratorComp(item, where, _none)
 
     generator_comp = iter
 
     def list_comp(self, item, *, where=None):
         return ListComp(item, where, _none)
@@ -203,21 +206,21 @@
             return CallFunc(zip, *args)
 
         return CallFunc(zip, *kwargs.values()).iter(
             {name: self.item(index) for index, name in enumerate(kwargs)}
         )
 
     def repeat(self, obj, times=None):
-        """shortcut to call :py:obj:`itertools.repeat`"""
+        """Shortcut for call :py:obj:`itertools.repeat`."""
         args = () if times is None else (times,)
         return CallFunc(repeat, obj, *args)
 
     def min(self, arg, *args):
-        """c.call_func(min, ...) shortcut"""
+        """Shortcut for `c.call_func(min, ...)`."""
         return CallFunc(min, arg, *args)
 
     def max(self, arg, *args):
-        """c.call_func(max, ...) shortcut"""
+        """Shortcut for `c.call_func(max, ...)`."""
         return CallFunc(max, arg, *args)
 
 
 conversion = Conversion()
```

### Comparing `convtools-1.4.0/convtools/_cumulative.py` & `convtools-1.5.0/convtools/_cumulative.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Provides cumulative conversions"""
+"""Cumulative conversions."""
 import typing as t
 from uuid import uuid4
 
 from ._base import (
     BaseConversion,
     EscapedString,
     If,
@@ -11,16 +11,15 @@
     NaiveConversion,
     Namespace,
     PipeConversion,
 )
 
 
 class CumulativeReset(BaseConversion):
-    """A conversion which resets cumulative values to their initial states. The
-    main use case is within nested iterables:
+    """Reset cumulative value to its initial state.
 
     >>> assert (
     >>>     c.iter(
     >>>         c.cumulative_reset("abc")
     >>>         .iter(c.cumulative(c.this, c.this + c.PREV, label_name="abc"))
     >>>         .as_type(list)
     >>>     )
@@ -39,17 +38,17 @@
         return (
             f"(_labels.pop({repr(self.label_name)}, None), "
             f"{self.parent.gen_code_and_update_ctx(code_input, ctx)})[1]"
         )
 
 
 class Cumulative(BaseConversion):
-    """A conversion which calculates cumulative values. The main use case is
-    using it within iterables:
+    """Calculate cumulative values within iterables.
 
+    Example:
     >>> assert (
     >>>     c.iter(c.cumulative(c.this, c.this + c.PREV))
     >>>     .as_type(list)
     >>>     .execute([0, 1, 2, 3, 4])
     >>> ) == [0, 1, 3, 6, 10]
     """
 
@@ -58,22 +57,22 @@
     def __init__(
         self,
         parent: "t.Any",
         prepare_first: "t.Any",
         reduce_two: "t.Any",
         label_name: "t.Optional[str]" = None,
     ):
-        """
+        """Initialize cumulative conversion.
+
         Args:
           parent: conversion which is used as an input
-          prepare_first: conversion which gets initial value from the first
-            element
-          reduce_two: conversion which reduces two values to one
+          prepare_first: conversion to apply to the first element
+          reduce_two: conversion to reduce two values to one
           label_name: custom name of cumulative to be used. It is needed when
-            :py:obj:`CumulativeReset`
+            `c.cumulative_reset(label_name)`
         """
         super().__init__()
         self.label_name = label_name or uuid4().hex
 
         self.parent = self.ensure_conversion(parent)
 
         label_conversion = LabelConversion(self.label_name)
```

### Comparing `convtools-1.4.0/convtools/_debug.py` & `convtools-1.5.0/convtools/_debug.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Provides conversions which simplify debug"""
+"""Provide conversions which simplify debugging."""
 import pdb
 import sys
 
 from ._base import BaseConversion, ensure_conversion
 
 
 if "pydevd" in sys.modules:  # pragma: no cover
@@ -23,16 +23,15 @@
 
     def debug_func(obj):
         breakpoint()  # pylint: disable=undefined-variable,forgotten-debug-statement # noqa: F821,E501
         return obj
 
 
 class Breakpoint(BaseConversion):
-    """Defines the conversion which wraps another one and puts a breakpoint
-    after it"""
+    """Wrap conversion with function and add breakpoint right after."""
 
     self_content_type = (
         BaseConversion.self_content_type
         | BaseConversion.ContentTypes.BREAKPOINT
     ) & ~BaseConversion.ContentTypes.FUNCTION_OF_INPUT
     debug_func = staticmethod(debug_func)
```

### Comparing `convtools-1.4.0/convtools/_expect.py` & `convtools-1.5.0/convtools/_expect.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-"""
-Provides conversion to check expected conditions or raise exception.
-"""
+"""Conversions to check expected conditions or raise exception."""
 from ._base import BaseConversion, ConversionException
 
 
 _none = BaseConversion._none
 
 EXPECT_TEMPLATE = """
 def {converter_name}({code_args}):
@@ -15,16 +13,20 @@
 
 
 class ExpectException(ConversionException):
     pass
 
 
 class Expect(BaseConversion):
-    """Checks condition and return the input as is. If condition is not met,
-    raises ExpectException with error_msg (can be conversion too) as param"""
+    """Check condition and return the input as is or raise ExpectException.
+
+    Args:
+      condition: conversion to evaluate as condition
+      error_msg: error message to pass to ExpectException
+    """
 
     def __init__(self, conversion, condition, error_msg):
         super().__init__()
         self.conversion = self.ensure_conversion(conversion)
         self.condition = self.ensure_conversion(condition)
         self.error_msg = self.ensure_conversion(
             error_msg or "condition is not met"
```

### Comparing `convtools-1.4.0/convtools/_heuristics.py` & `convtools-1.5.0/convtools/_heuristics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-"""
-This module is to contain helpers, which collect info about python code
-execution
-"""
+"""Helpers to collect info about environment."""
 import sys
 
 
 # generated by "python benchmarks/build_heuristics.py"
 
 PY_VERSION = sys.version_info[0:2]
 if PY_VERSION <= (3, 6):
```

### Comparing `convtools-1.4.0/convtools/_joins.py` & `convtools-1.5.0/convtools/_joins.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-"""
-This module brings join functionality to the library
-"""
+"""Join conversions."""
 import typing as t
 from itertools import chain, repeat
 
 from ._aggregations import Aggregate, ReduceFuncs
 from ._base import (
     And,
     BaseConversion,
@@ -45,15 +43,15 @@
 
 
 class RightJoinCondition(JoinCondition):
     NAME = "right_row"
 
 
 class _JoinConditions:
-    """A helper object to analyze join conditions"""
+    """A helper object to analyze join conditions."""
 
     LEFT = LeftJoinCondition()
     RIGHT = RightJoinCondition()
     LEFT_NAME = LEFT.name
     RIGHT_NAME = RIGHT.name
     _ANY = {LEFT_NAME, RIGHT_NAME}
 
@@ -102,18 +100,17 @@
         if self.outer_join:
             self.inner_loop_conditions.append(filter_conv)
         else:
             self.right_collection_filters.append(filter_conv)
 
     @classmethod
     def from_condition(cls, condition, how="inner") -> "_JoinConditions":
-        if how == "right":
-            join_conditions = cls(how="left", swapped=True)
-        else:
-            join_conditions = cls(how)
+        join_conditions = (
+            cls(how="left", swapped=True) if how == "right" else cls(how)
+        )
 
         if isinstance(condition, Namespace):
             condition = condition.conversion
 
         if isinstance(condition, NaiveConversion) and condition.value is True:
             return join_conditions
 
@@ -202,16 +199,15 @@
                 self.LEFT_NAME if self.swapped else self.RIGHT_NAME
             ] = right
 
         return Namespace(conversion, name_to_code)
 
 
 class JoinConversion(BaseConversion):
-    """Generates conversion which joins left_conversion and right_conversion
-    using condition. The result is a generator of joined pairs
+    """Join results of two conversions as generated of joined pairs.
 
     Args:
       left_conversion (BaseConversion): left collection to join
       right_conversion (BaseConversion): right collection to join
       condition (BaseConversion): join condition. If is True, results in cross
         join
       how (str): one of the following: ``"inner"``, ``"left"``, ``"right"``,
```

### Comparing `convtools-1.4.0/convtools/_mutations.py` & `convtools-1.5.0/convtools/_mutations.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-"""This module brings in-place mutations"""
+"""In-place mutations."""
 from ._base import BaseConversion, BaseMutation
 from ._heuristics import Weights
 from ._utils import Code
 
 
 class BaseNameValueMutation(BaseMutation):
-    """A base in-place mutation where name and value are needed to define it"""
+    """Base in-place mutation."""
 
     def __init__(self, name, value):
-        """
+        """Init self.
+
         Args:
           name: to be wrapped with :py:obj:`ensure_conversion` and used as
             a key/attr/index for a mutation
           value: to be wrapped with :py:obj:`ensure_conversion` and used as
             a value for a mutation
         """
         super().__init__()
@@ -55,23 +56,21 @@
         code = f"delattr({code_input}, {index_code})"
         if self.if_exists:
             return f"hasattr({code_input}, {index_code}) and {code}"
         return code
 
 
 class Custom(BaseMutation):
-    """Mutation to be used in conjunction with `tap` method.
-    Runs the code, defined by the conversion argument and returns the input
-    as is."""
+    """Run a conversion and return input as is."""
 
     def __init__(self, conversion):
-        """
+        """Init self.
+
         Arg:
-          conversion: to be wrapped with :py:obj:`ensure_conversion` and used
-            as a mutation code
+          conversion: conversion to be used as a mutation code
         """
         super().__init__()
         self.conversion = self.ensure_conversion(conversion)
 
     def _gen_code_and_update_ctx(self, code_input, ctx):
         return self.conversion.gen_code_and_update_ctx(code_input, ctx)
 
@@ -89,16 +88,15 @@
     del_attr = DelAttr
     #: Runs the code, defined by the conversion argument and returns the input
     #: as is.
     custom = Custom
 
 
 class TapConversion(BaseConversion):
-    """This conversion generates the code which mutates the input data
-    in-place.  TapConversion takes any number of mutations"""
+    """Apply mutations to input and return it."""
 
     weight = Weights.FUNCTION_CALL
 
     def __init__(self, obj, *mutations: BaseMutation):
         super().__init__()
         self.obj = self.ensure_conversion(obj)
         self.mutations = [
@@ -128,17 +126,18 @@
             )
         return function_ctx.call_with_all_args(
             conversion
         ).gen_code_and_update_ctx(code_input, ctx)
 
 
 class IterMutConversion(TapConversion):
-    """This conversion generates the code which iterates and mutates the
-    elements in-place. The result is a generator.
-    IterMutConversion takes any number of mutations"""
+    """Iterate input and apply mutations element-wise.
+
+    Returns: generator of mutated elements.
+    """
 
     def _gen_code_and_update_ctx(self, code_input, ctx):
         suffix = self.gen_random_name("", ctx)
         converter_name = f"iter_mut_{suffix}"
         code_item = f"item_{suffix}"
         function_ctx = self.as_function_ctx(ctx, optimize_naive=True)
         function_ctx.add_arg("data_", self.obj)
```

### Comparing `convtools-1.4.0/convtools/_unique.py` & `convtools-1.5.0/convtools/_unique.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,14 @@
-"""Provides conversions for working with unique values"""
+"""Conversions for working with unique values."""
 from ._base import BaseConversion, EscapedString
 from ._utils import Code
 
 
 class IterUnique(BaseConversion):
-    """
-    Defines a conversion which iterates over the input and yields unique ones
-    (supports custom uniqueness conditions)
-    """
+    """Iterate unique elements of self conversion."""
 
     def __init__(self, self_conv, element, by_):
         super().__init__()
         self.self_conv = self.ensure_conversion(self_conv)
         self.element = self.ensure_conversion(element)
         self.by_ = self.ensure_conversion(by_)
```

### Comparing `convtools-1.4.0/convtools/_utils.py` & `convtools-1.5.0/convtools/_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-"""Helpers live here: like:
+"""Code generation helpers.
+
+e.g.
  - recently used cache
  - options ctx manager
 """
 import os
 import sys
 import tempfile
 import threading
 import typing as t
-from collections import deque
+from collections import defaultdict, deque
 from importlib import import_module
-from typing import TYPE_CHECKING
 from weakref import finalize
 
 
-if TYPE_CHECKING:
-    from typing import Optional
-
 PY_VERSION = sys.version_info[:2]
 if PY_VERSION == (3, 6):
 
     class BaseCtxMeta(t.GenericMeta):  # type: ignore
         def __init__(
             cls, name, bases, kwargs
         ):  # pylint: disable=no-self-argument
@@ -41,21 +39,21 @@
             k: v
             for k, v in kwargs.items()
             if not k.startswith("_") and k not in {"clone", "to_defaults"}
         }
 
 
 class BaseOptions(object, metaclass=BaseOptionsMeta):
-    """Container object, which carries current options"""
+    """Container object, which carries current code-gen options."""
 
     _option_attrs: dict
 
     def clone(self):
         clone = self.__class__()
-        for option_attr in self._option_attrs.keys():
+        for option_attr in self._option_attrs:
             setattr(clone, option_attr, getattr(self, option_attr))
         return clone
 
     def to_defaults(self, option_name=None):
         if option_name:
             setattr(self, option_name, self._option_attrs[option_name])
         else:
@@ -65,15 +63,15 @@
 
 OT = t.TypeVar("OT", bound=BaseOptions)
 
 
 class BaseCtx(
     t.Generic[OT], metaclass=BaseCtxMeta
 ):  # pylint:disable=invalid-metaclass
-    """Context manager to manage option objects"""
+    """Context manager to manage option objects."""
 
     options_cls: t.Type[OT]
     _ctx: threading.local
 
     def __enter__(self) -> OT:
         self._ctx.prev_options = getattr(self._ctx, "options", None)
         if self._ctx.prev_options:
@@ -91,39 +89,26 @@
         options = getattr(cls._ctx, "options", None)
         if not options:
             options = cls.options_cls
         return getattr(options, option_name)
 
 
 class Code:
-    """A building block for generating code, which is composed of multiple
-    statements."""
+    """Code builder for multi-statement code pieces."""
 
     def __init__(self):
         self.lines_info = []
         self.indent_level = 0
-        self.expression_line = None
 
-    def add_line(
-        self,
-        line: str,
-        next_line_indent_incr: int,
-        expression_line: "Optional[str]" = None,
-    ):
+    def add_line(self, line: str, next_line_indent_incr: int):
         self.lines_info.append((self.indent_level, line))
         self.indent_level += next_line_indent_incr
-        self.expression_line = expression_line
         if self.indent_level < 0:
             raise AssertionError("negative indentation level")
 
-    def as_expression(self) -> "Optional[str]":
-        if len(self.lines_info) == 1 and self.expression_line:
-            return self.expression_line
-        return None
-
     def add_code(self, code: "Code"):
         for indent_level, line in code.lines_info:
             self.lines_info.append((indent_level + self.indent_level, line))
 
     def incr_indent_level(self, incr: int):
         self.indent_level += incr
 
@@ -137,17 +122,70 @@
     def to_string(self, base_indent_level: int, single_indent: str = "    "):
         return "\n".join(
             f"{single_indent * (base_indent_level + indent_level)}{line}"
             for indent_level, line in self.lines_info
         )
 
 
+class CodeParams:
+    """Code-gen tree-like helper to generate assignments when needed."""
+
+    def __init__(self):
+        self.name_to_uses = defaultdict(int)
+        self.name_to_code = {}
+        self.name_to_deps = defaultdict(list)
+        self.id_to_naive_code = {}
+        self.params = []
+
+    def naive_code(self, value, ctx):
+        key = id(value)
+        if key not in self.id_to_naive_code:
+            self.id_to_naive_code[key] = convtools_base.NaiveConversion(
+                value
+            ).gen_code_and_update_ctx(None, ctx)
+        return self.id_to_naive_code[key]
+
+    def create(self, code, name, used_names=()):
+        self.name_to_code[name] = code
+        for used_name in used_names:
+            self.name_to_deps[name].append(used_name)
+
+    def use_param(self, name):
+        self.name_to_uses[name] += 1
+        self.params.append(name)
+
+        names_to_check_deps = [name]
+        visited_deps = set()
+        while names_to_check_deps:
+            name_ = names_to_check_deps.pop()
+            visited_deps.add(name_)
+            for dep_ in self.name_to_deps[name_]:
+                self.name_to_uses[dep_] += 2
+                if dep_ in visited_deps:
+                    raise ValueError("cyclic dependency detected", name, dep_)
+                names_to_check_deps.insert(0, dep_)
+
+    def create_and_use_param(self, code, name):
+        self.create(code, name)
+        self.use_param(name)
+
+    def iter_assignments(self):
+        for name, code in self.name_to_code.items():
+            if self.name_to_uses[name] > 1:
+                yield f"{name} = {code}"
+
+    def get_format_args(self):
+        return tuple(
+            self.name_to_code[name] if self.name_to_uses[name] == 1 else name
+            for name in self.params
+        )
+
+
 class LazyDebugDir:
-    """Lazy instance to hold and initialize debug directory for generated code
-    sources"""
+    """Lazy debug directory to store generated code sources."""
 
     def __init__(self):
         self.debug_dir = None
         self.dir_initialized = False
 
     def get(self) -> str:
         if self.debug_dir is None:
@@ -162,15 +200,15 @@
             self.dir_initialized = True
 
 
 debug_dir = LazyDebugDir()
 
 
 class CodePiece:
-    """Piece of source code (a function at the moment)"""
+    """Piece of generated code."""
 
     __slots__ = (
         "converter_name",
         "code_parts",
         "abs_path",
         "is_dumped",
     )
@@ -179,16 +217,18 @@
         self.converter_name = converter_name
         self.code_parts = code_parts
         self.abs_path = abs_path
         self.is_dumped = is_dumped
 
 
 class CodeStorage:
-    """Container which stores generated code pieces. It allows to dump code
-    sources on disk into a debug directory."""
+    """Container which stores generated code pieces.
+
+    It allows to dump code sources on disk into a debug directory.
+    """
 
     def __init__(self):
         self.key_to_code_piece: "t.Dict[str, CodePiece]" = {}
         self.converter_names = set()
         finalize(self, drop_dumped_code, self.key_to_code_piece)
 
     def add_sources(self, converter_name, code_str):
@@ -257,19 +297,20 @@
             window.popleft()
 
 
 obj_getattribute = object.__getattribute__
 
 
 class LazyModule:
-    """Lazy import helper, which caches results of importlib.import_module"""
+    """Lazy import helper."""
 
     __slots__ = ["name", "package", "_module"]
 
     def __init__(self, name, package=None):
+        """Init self."""
         self.name = name
         self.package = package
         self._module = None
 
     def __getattribute__(self, name):
         module = obj_getattribute(self, "_module")
         if module is None:
@@ -277,24 +318,28 @@
                 obj_getattribute(self, "name"),
                 obj_getattribute(self, "package"),
             )
         return getattr(module, name)
 
 
 class _None:
-    """Custom None type for the sake of typing AND ability to tell None passed
-    instead of default value to an optional parameter"""
+    """Custom None type.
 
-    pass
+    For the sake of typing AND ability to tell None from "undefined" optional
+    parameters.
+    """
 
 
 _none = _None()
 
 
 def get_builtins_dict():
     builtins = globals()["__builtins__"]
     if isinstance(builtins, dict):
         return builtins
     # for pypy
     return {
         name: getattr(builtins, name) for name in dir(builtins)
     }  # pragma: no cover
+
+
+convtools_base = LazyModule("convtools._base")
```

### Comparing `convtools-1.4.0/convtools/contrib/fs.py` & `convtools-1.5.0/convtools/contrib/fs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-"""
+"""File system helpers.
+
 Python's native open() doesn't support custom newlines in the text mode and
 doesn't support "newlines" (delimiters) in binary mode. The following methods
 should close the gap.
 """
 
 
 def split_buffer(buffer, delimiter, chunk_size=32768):
@@ -42,16 +43,15 @@
                 yield chunk
                 break
 
 
 def split_buffer_n_decode(
     buffer, delimiter, chunk_size=32768, encoding="utf-8"
 ):
-    """Reads binary buffer, splits it by binary delimiter and yields decoded
-    chunks.
+    """Read binary buffer, yield decoded chunks, splitting by binary delimiter.
 
     Args:
       buffer: buffer to be read
       delimiter: delimiter to use for splitting
       chunk_size: chunk size to read at every iteration
       encoding: encoding to use when decoding a chunk
     """
```

### Comparing `convtools-1.4.0/convtools/contrib/tables.py` & `convtools-1.5.0/convtools/contrib/tables.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-"""
-Implements streaming operations on table-like data and csv files.
+"""Implements streaming operations on table-like data and csv files.
 
 Conversions are defined in realtime based on table headers and called methods:
  - update
  - take
  - drop
  - join
 
@@ -32,61 +31,69 @@
 from .._joins import JoinConversion, LeftJoinCondition, RightJoinCondition
 
 
 _none = BaseConversion._none
 
 
 class CloseFileIterator:
-    """
-    Utility to close the corresponding file once the iterator is exhausted
-    """
+    """Iterator wrapper, which closes file in the end."""
 
     def __init__(self, file_to_close):
+        """Init instance.
+
+        Args:
+          file_to_close: file descriptor to be closed the first time __next__
+            is called on this wrapper
+        """
         self.file_to_close = file_to_close
 
     def __iter__(self):
+        """Returns empty iterator."""
         return self
 
     def __next__(self):
+        """Stops iteration and closes the underlying file descriptor."""
         self.file_to_close.close()
         self.file_to_close = None
         raise StopIteration
 
     def __del__(self):
+        """Closes the file descriptor on garbage collection."""
+        # Consider rewriting with: weakref.finalize
         if self.file_to_close:
             self.file_to_close.close()
             self.file_to_close = None
 
 
 class CustomCsvDialect(csv.Dialect):
-    """A helper to define custom csv dialects without defining classes"""
+    """Create custom csv dialects without defining classes."""
 
     def __init__(
         self,
         delimiter=csv.excel.delimiter,
         quotechar=csv.excel.quotechar,
         escapechar=csv.excel.escapechar,
         doublequote=csv.excel.doublequote,
         skipinitialspace=csv.excel.skipinitialspace,
         lineterminator=csv.excel.lineterminator,
         quoting=csv.excel.quoting,
     ):
+        """Init self."""
         self.delimiter = delimiter
         self.quotechar = quotechar
         self.escapechar = escapechar
         self.doublequote = doublequote
         self.skipinitialspace = skipinitialspace
         self.lineterminator = lineterminator
         self.quoting = quoting
         super().__init__()
 
 
 class Table:
-    """Table conversion exposes streaming operations on table-like data and csv
-    files
+    """Streaming operations on table-like data and csv files.
 
     >>> Table.from_csv("input.csv", header=True).update(
     >>>     c=c.item("a") + c.item("b")
     >>> ).into_csv("output.csv")
 
     >>> list(
     >>>     Table.from_rows(
@@ -109,25 +116,25 @@
         row_type: "t.Optional[type]",
         rows_objects: "t.List[t.Iterable]",
         meta_columns: "MetaColumns",
         pending_changes: int,
         pipeline: "t.Optional[BaseConversion]" = None,
         file_to_close=None,
     ):
-        """It is used internally only. Use from_rows and from_csv methods."""
+        """For internal use only. Use from_rows and from_csv methods."""
         self.row_type = row_type
         self.rows_objects: "t.Optional[t.List[t.Iterable]]" = rows_objects
         self.meta_columns = meta_columns
         self.pending_changes = pending_changes
         self.pipeline = pipeline
         self.file_to_close = file_to_close
         self.row_type = row_type
 
     def get_columns(self) -> "t.List[str]":
-        """Exposes list of column names"""
+        """Return list of column names."""
         return [column.name for column in self.meta_columns.columns]
 
     columns = property(get_columns)
 
     @classmethod
     def from_rows(
         cls,
@@ -138,16 +145,15 @@
             ]
         ]""" = None,
         # t.Literal["raise", "keep", "drop", "mangle"]
         duplicate_columns: str = "raise",
         skip_rows: int = 0,
         file_to_close=None,
     ) -> "Table":
-        """A method to initialize a table conversion from an iterable of
-        rows.
+        """Initialize a table from an iterable of rows.
 
         Args:
           rows: can be either an iterable of any objects if no header inference
             is required OR an iterable of dicts, tuples or lists
           header: specifies header inference mode:
 
              * True: takes either the first tuple/list or keys of the first
@@ -172,14 +178,16 @@
             * "mangle": names of duplicate columns are mangled like: "name",
               "name_1", "name_2", etc.
 
           skip_rows: number of rows to skip at the beginning. Useful when input
             data contains a header, but you provide your own - in this case
             it's convenient to skip the heading row from the input
 
+          file_to_close: for internal use
+
         """
         columns = MetaColumns(duplicate_columns=duplicate_columns)
 
         rows = iter(rows)
 
         if skip_rows:
             for _ in range(skip_rows):
@@ -208,44 +216,41 @@
                     "first row is not sized to apply header as dict"
                 )
             if len(header) != len(first_row):
                 raise ValueError("non-matching number of columns")
             for name, index in header.items():
                 pending_changes |= columns.add(name, index, None)[1]
 
-        else:
-            # inferring a header
-            if isinstance(first_row, dict):
-                if header is False:
-                    for key in first_row:
-                        pending_changes |= columns.add(None, key, None)[1]
-                    pending_changes |= ColumnChanges.MUTATE
-                else:
-                    for key in first_row:
-                        pending_changes |= columns.add(key, key, None)[1]
+        # inferring a header
+        elif isinstance(first_row, dict):
+            if header is False:
+                for key in first_row:
+                    pending_changes |= columns.add(None, key, None)[1]
+                pending_changes |= ColumnChanges.MUTATE
+            else:
+                for key in first_row:
+                    pending_changes |= columns.add(key, key, None)[1]
 
-            elif isinstance(first_row, (tuple, list)):
-                if header is True:
-                    for index, column_name in enumerate(first_row):
-                        pending_changes |= columns.add(
-                            column_name, index, None
-                        )[1]
-                    first_row = None
+        elif isinstance(first_row, (tuple, list)):
+            if header is True:
+                for index, column_name in enumerate(first_row):
+                    pending_changes |= columns.add(column_name, index, None)[1]
+                first_row = None
 
-                else:
-                    for index in range(len(first_row)):
-                        pending_changes |= columns.add(None, index, None)[1]
+            else:
+                for index in range(len(first_row)):
+                    pending_changes |= columns.add(None, index, None)[1]
 
+        else:
+            if header is True:
+                pending_changes |= columns.add(first_row, None, This())[1]
+                first_row = None
             else:
-                if header is True:
-                    pending_changes |= columns.add(first_row, None, This())[1]
-                    first_row = None
-                else:
-                    pending_changes |= columns.add(None, None, This())[1]
-                pending_changes |= ColumnChanges.MUTATE
+                pending_changes |= columns.add(None, None, This())[1]
+            pending_changes |= ColumnChanges.MUTATE
 
         rows_objects: "t.List[t.Iterable]" = [rows]
         if first_row is not None:
             rows_objects.insert(0, (first_row,))
 
         return cls(
             row_type=row_type,
@@ -267,36 +272,35 @@
             ]
         ]""" = None,
         duplicate_columns: str = "mangle",
         skip_rows: int = 0,
         dialect: "t.Union[str, CustomCsvDialect]" = "excel",
         encoding: str = "utf-8",
     ) -> "Table":
-        """A method to initialize a table conversion from a csv-like file.
+        """Initialize a table conversion from a csv-like object.
 
         Args:
           filepath_or_buffer: a filepath or something :py:obj:`csv.reader` can
             read
-          header: specifies header inference mode:
 
+          header: specifies header inference mode:
              * True: takes either the first tuple/list or keys of the first
                dict as a header
              * False: there's no header in input data, use numbered columns
                instead: COLUMN_0, COLUMN_1, etc.
              * list/tuple of str: there's no header in input data, so this is
                the header to be used (raises ValueError if numbers of columns
                don't match)
              * dict: its keys form the header, values are str/int indices to
                take values of columns from input rows (raises ValueError if
                numbers of columns don't match)
              * None: inspects the first row and if it's a dict, then takes its
                keys as a header
 
           duplicate_columns: either of following ("mangle" by default):
-
             * "raise": ValueError is raise if a duplicate column is detected
             * "keep": duplicate columns are left as is, but when referenced the
               first one is used
             * "drop": duplicate columns are skipped
             * "mangle": names of duplicate columns are mangled like: "name",
               "name_1", "name_2", etc.
 
@@ -304,23 +308,23 @@
             data contains a header, but you provide your own - in this case
             it's convenient to skip the heading row from the input
 
           dialect: a dialect acceptable by :py:obj:`csv.reader` There's a
             helper method:
             :py:obj:`convtools.contrib.tables.Table.csv_dialect` to create
             dialects without defining classes
+
           encoding: encoding to pass to :py:obj:`open`
         """
-
         file_to_close: "t.Optional[t.TextIO]"
         buffer: "t.TextIO"
         if isinstance(filepath_or_buffer, str):
             buffer = (
                 file_to_close
-            ) = open(  # pylint: disable=consider-using-with
+            ) = open(  # pylint: disable=consider-using-with # noqa: SIM115
                 filepath_or_buffer,
                 "r",
                 encoding=encoding,
             )
         else:
             buffer = filepath_or_buffer
             file_to_close = None
@@ -335,15 +339,17 @@
             header,
             duplicate_columns,
             skip_rows=skip_rows,
             file_to_close=file_to_close,
         )
 
     def embed_conversions(self) -> "Table":
-        """There's no need in calling this directly, it's done automatically
+        """For internal use only.
+
+        There's no need in calling this directly, it's done automatically
         when you use :py:obj:`convtools.contrib.tables.Table.update` or
         :py:obj:`convtools.contrib.tables.Table.join` See the explanation
         below:
 
         Since each column is either:
           * simply taken by index (cheap)
           * or obtained by performing arbitrary convtools conversion (may be
@@ -374,16 +380,15 @@
             )
             self.pending_changes = 0
             self.row_type = tuple
 
         return self
 
     def filter(self, condition: "BaseConversion") -> "Table":
-        """Filters table-like data, keeping rows where ``condition`` resolves
-        to ``True``"""
+        """Keep rows where ``condition`` resolves to `True`."""
         condition = ensure_conversion(condition)
         column_refs = list(condition.get_dependencies(types=ColumnRef))
         name_to_column = self.meta_columns.get_name_to_column()
 
         depends_on_complex_columns = any(
             name_to_column[ref.name].conversion is not None
             for ref in column_refs
@@ -452,21 +457,23 @@
             for column in self.meta_columns.columns
         }
         return self.update(**column_to_conversion)
 
     def rename(
         self, columns: "t.Union[t.Tuple[str], t.List[str], t.Dict[str, str]]"
     ) -> "Table":
-        """Method to rename columns. The behavior depends on type of columns
-        argument.
+        """Rename columns.
+
+        The behavior depends on type of columns argument.
 
         Args:
-          columns: if tuple/list, then it defines new column names (length of
-            passed columns should match number of columns inside).  If dict,
-            then it defines a mapping from old column names to new ones.
+          columns:
+            * tuple/list: then it defines new column names (length of
+              passed columns should match number of columns inside).
+            * dict: defines a mapping from old column names to new ones.
         """
         renamed = False
         if isinstance(columns, dict):
             for column_ in self.meta_columns.columns:
                 if column_.name in columns:
                     column_.name = columns[column_.name]
                     renamed = True
@@ -485,16 +492,18 @@
 
         if renamed and self.row_type is dict:
             self.pending_changes |= ColumnChanges.MUTATE
 
         return self
 
     def take(self, *column_names: "t.Union[str, t.Any]") -> "Table":
-        """Leaves only specified columns, omitting the rest. ``...`` references
-        non-mentioned columns, so it's easy to both take a few columns:
+        """Leave only specified columns, omitting the rest.
+
+        ``...`` references non-mentioned columns, so it's easy to both take a
+        few columns:
 
         >>> table.take("a", "b")
 
         and rearrange them:
 
         >>> table.take("c", "d", ...)
 
@@ -513,16 +522,18 @@
         """
         self.meta_columns = self.meta_columns.drop(*column_names)
         if column_names:
             self.pending_changes |= ColumnChanges.REARRANGE
         return self
 
     def zip(self, table: "Table", fill_value=None) -> "Table":
-        """Zip tables one to another. Before using this method, make sure you
-        are not looking for :py:obj:`convtools.contrib.tables.Table.join`
+        """Zip tables one to another.
+
+        Before using this method, make sure you are not looking for
+        `convtools.contrib.tables.Table.join`
 
         Let's assume fill_value is set to " ":
 
         >>> Table 1      Table 2
         >>> | a | b |    | b | c |
         >>> | 1 | 2 |    | 3 | 4 |
         >>>              | 5 | 6 |
@@ -531,17 +542,16 @@
         >>>
         >>> Result:
         >>> | a | b | b | c |
         >>> | 1 | 2 | 3 | 4 |
         >>> |   |   | 5 | 6 |
 
         Args:
-         - table: table to be chained
-         - fill_value: value to use for filling gaps
-
+          table: table to be chained
+          fill_value: value to use for filling gaps
         """
         new_columns = MetaColumns(duplicate_columns="keep")
         left_columns = self.meta_columns.get_name_to_column()
         right_columns = table.meta_columns.get_name_to_column()
 
         left_fill_value = tuple(fill_value for _ in range(len(left_columns)))
         right_fill_value = tuple(fill_value for _ in range(len(right_columns)))
@@ -583,17 +593,16 @@
         >>>
         >>> Result:
         >>> | a | b | c |
         >>> | 1 | 2 |   |
         >>> |   | 3 | 4 |
 
         Args:
-         - table: table to be chained
-         - fill_value: value to use for filling gaps
-
+          table: table to be chained
+          fill_value: value to use for filling gaps
         """
         if self.rows_objects is None:
             raise AssertionError("move_rows called the 2nd time")
         if (
             self.meta_columns.is_same_as(table.meta_columns)
             and not self.pending_changes
             and not self.pipeline
@@ -655,15 +664,15 @@
     def join(
         self,
         table: "Table",
         on: "t.Union[BaseConversion, str, t.Iterable[str]]",
         how: str,
         suffixes=("_LEFT", "_RIGHT"),
     ) -> "Table":
-        """Joins the table conversion to another table conversion.
+        """Classic table join.
 
         Args:
           table: another table conversion to join to self
           on:
             * either a join conversion like
               ``c.LEFT.col("a") == c.RIGHT.col("A")``
             * or iterable of column names to join on
@@ -671,15 +680,14 @@
           how: either of these: "inner", "left", "right", "outer" (same as
             "full")
           suffixes: tuple of two strings: the first one is the suffix to be
             added to left columns, having conflicting names with right columns;
             the second one is added to conflicting right ones. When ``on`` is
             an iterable of strings, these columns are excluded from suffixing.
         """
-
         how = JoinConversion.validate_how(how)
         left = self.embed_conversions()
         right = table.embed_conversions()
         left_join_conversion = LeftJoinCondition()
         right_join_conversion = RightJoinCondition()
         left_column_name_to_column = left.meta_columns.get_name_to_column()
         right_column_name_to_column = right.meta_columns.get_name_to_column()
@@ -799,32 +807,30 @@
             row_type=tuple,
             rows_objects=[new_rows],
             meta_columns=new_columns,
             pending_changes=ColumnChanges.MUTATE,
         )
 
     def explode(self, column_name: str):
-        """Explodes a table to a long format by exploding a column with
-        iterables, e.g.:
+        """Explode a table by unnesting a column with iterables.
 
         >>> | a |   b    |
         >>> | 1 | [2, 3] |
         >>> | 4 | [5, 6] |
         >>>
         >>> table.explode("b")
         >>>
         >>> | a | b |
         >>> | 1 | 2 |
         >>> | 1 | 3 |
         >>> | 2 | 5 |
         >>> | 2 | 6 |
 
         Args:
-         - column_name: column with iterables to be exploded
-
+          column_name: column with iterables to be exploded
         """
         columns = self.columns
         try:
             index = columns.index(column_name)
         except ValueError as e:
             raise ValueError("unknown column", column_name) from e
 
@@ -850,15 +856,18 @@
             )
             .execute(self.into_iter_rows(tuple, include_header=False))
         )
 
         return Table.from_rows(new_rows, header=columns)
 
     def move_rows_objects(self) -> "t.List[t.Iterable]":
-        """Moves out rows objects including files to be closed later"""
+        """For internal use.
+
+        Moves out rows objects including files to be closed later.
+        """
         if self.rows_objects is None:
             raise AssertionError("move_rows called the 2nd time")
 
         rows_objects = self.rows_objects
         self.rows_objects = None
 
         if self.file_to_close:
@@ -867,14 +876,15 @@
         return rows_objects
 
     supported_types = (tuple, list, dict)
 
     def into_list_of_iterables(
         self, type_=tuple, include_header=None
     ) -> "t.List[t.Iterable]":
+        """For internal use."""
         if type_ not in self.supported_types:
             raise TypeError("unsupported type_", type_)
 
         no_pending_changes = (
             type_ is self.row_type and not self.pending_changes
         )
 
@@ -916,22 +926,23 @@
             rows_objects.insert(0, (header,))
 
         return rows_objects
 
     def into_iter_rows(
         self, type_=tuple, include_header=None
     ) -> "t.Iterable[t.Any]":
-        """Consumes inner rows Iterable and returns Iterable of processed rows.
+        """Return iterable of processed rows.
 
         Args:
           type_: casts output rows to the type. Accepts the following values:
 
             * :py:obj:`dict`
             * :py:obj:`tuple`
             * :py:obj:`list`
+          include_header: whether to include header row in the result or not
 
         """
         return chain.from_iterable(
             self.into_list_of_iterables(
                 type_=type_, include_header=include_header
             )
         )
@@ -939,16 +950,15 @@
     def into_csv(
         self,
         filepath_or_buffer: "t.Union[str, t.TextIO]",
         include_header: bool = True,
         dialect: "t.Union[str, CustomCsvDialect]" = "excel",
         encoding="utf-8",
     ):
-        """Consumes inner rows Iterable and writes processed rows as a csv-like
-        file.
+        """Writes rows to a file.
 
         Args:
           filepath_or_buffer: a filepath or something :py:obj:`csv.writer` can
             write to
           include_header: self-explanatory bool
           dialect: a dialect acceptable by :py:obj:`csv.writer` There's a
             helper method:
@@ -957,15 +967,17 @@
           encoding: encoding to pass to :py:obj:`open`
         """
         row_type = list if self.row_type is list else tuple
 
         f_to_close = None
         f: "t.TextIO"
         if isinstance(filepath_or_buffer, str):
-            f = f_to_close = open(  # pylint:disable=consider-using-with
+            f = (
+                f_to_close
+            ) = open(  # pylint:disable=consider-using-with  # noqa: SIM115
                 filepath_or_buffer, "w", encoding=encoding
             )
         else:
             f = filepath_or_buffer
 
         try:
             writer = csv.writer(f, dialect=dialect)
```

### Comparing `convtools-1.4.0/.gitignore` & `convtools-1.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `convtools-1.4.0/LICENSE.txt` & `convtools-1.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `convtools-1.4.0/README.md` & `convtools-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `convtools-1.4.0/pyproject.toml` & `convtools-1.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 [tool.hatch.build.targets.sdist]
 include = ["/src"]
 
 
 [project]
 name = "convtools"
-version = "1.4.0"
+version = "1.5.0"
 description = "dynamic, declarative data transformations with automatic code generation"
 
 readme = "README.md"
 requires-python = ">=3.6"
 license = {file = "LICENSE.txt"}
 keywords = ["etl", "converters", "codegen", "convtools"]
 authors = [
```

### Comparing `convtools-1.4.0/PKG-INFO` & `convtools-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: convtools
-Version: 1.4.0
+Version: 1.5.0
 Summary: dynamic, declarative data transformations with automatic code generation
 Project-URL: homepage, https://github.com/westandskif/convtools
 Project-URL: documentation, https://convtools.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/westandskif/convtools
 Project-URL: changelog, https://github.com/westandskif/convtools/blob/master/docs/CHANGELOG.md
 Author-email: Nikita Almakov <nikita.almakov@gmail.com>
 Maintainer-email: Nikita Almakov <nikita.almakov@gmail.com>
```

