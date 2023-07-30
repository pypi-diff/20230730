# Comparing `tmp/statprocon-0.0.9.tar.gz` & `tmp/statprocon-0.1.0.tar.gz`

## Comparing `statprocon-0.0.9.tar` & `statprocon-0.1.0.tar`

### file list

```diff
@@ -1,24 +1,28 @@
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 statprocon-0.0.9/CHANGELOG.md
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 statprocon-0.0.9/CODEOWNERS
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 statprocon-0.0.9/requirements-dev.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 statprocon-0.0.9/.idea/.gitignore
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 statprocon-0.0.9/.idea/dataSources.local.xml
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 statprocon-0.0.9/.idea/misc.xml
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 statprocon-0.0.9/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 statprocon-0.0.9/.idea/vcs.xml
--rw-r--r--   0        0        0     5863 2020-02-02 00:00:00.000000 statprocon-0.0.9/.idea/workspace.xml
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 statprocon-0.0.9/.idea/xmr.iml
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 statprocon-0.0.9/.idea/codeStyles/codeStyleConfig.xml
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 statprocon-0.0.9/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 statprocon-0.0.9/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 statprocon-0.0.9/statprocon/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 statprocon-0.0.9/statprocon/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 statprocon-0.0.9/statprocon/charts/__init__.py
--rw-r--r--   0        0        0    10005 2020-02-02 00:00:00.000000 statprocon-0.0.9/statprocon/charts/xmr.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 statprocon-0.0.9/tests/__init__.py
--rw-r--r--   0        0        0     9292 2020-02-02 00:00:00.000000 statprocon-0.0.9/tests/test_xmr.py
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 statprocon-0.0.9/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 statprocon-0.0.9/LICENSE
--rw-r--r--   0        0        0     4334 2020-02-02 00:00:00.000000 statprocon-0.0.9/README.md
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 statprocon-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     5116 2020-02-02 00:00:00.000000 statprocon-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 statprocon-0.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 statprocon-0.1.0/CODEOWNERS
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 statprocon-0.1.0/requirements-dev.txt
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 statprocon-0.1.0/tox.ini
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 statprocon-0.1.0/.idea/.gitignore
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 statprocon-0.1.0/.idea/dataSources.local.xml
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 statprocon-0.1.0/.idea/misc.xml
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 statprocon-0.1.0/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 statprocon-0.1.0/.idea/vcs.xml
+-rw-r--r--   0        0        0     6269 2020-02-02 00:00:00.000000 statprocon-0.1.0/.idea/workspace.xml
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 statprocon-0.1.0/.idea/xmr.iml
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 statprocon-0.1.0/.idea/codeStyles/codeStyleConfig.xml
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 statprocon-0.1.0/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 statprocon-0.1.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 statprocon-0.1.0/statprocon/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 statprocon-0.1.0/statprocon/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 statprocon-0.1.0/statprocon/charts/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 statprocon-0.1.0/statprocon/charts/xmr/__init__.py
+-rw-r--r--   0        0        0    11948 2020-02-02 00:00:00.000000 statprocon-0.1.0/statprocon/charts/xmr/base.py
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 statprocon-0.1.0/statprocon/charts/xmr/constants.py
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 statprocon-0.1.0/statprocon/charts/xmr/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 statprocon-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     9942 2020-02-02 00:00:00.000000 statprocon-0.1.0/tests/test_xmr.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 statprocon-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 statprocon-0.1.0/LICENSE
+-rw-r--r--   0        0        0     4514 2020-02-02 00:00:00.000000 statprocon-0.1.0/README.md
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 statprocon-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5353 2020-02-02 00:00:00.000000 statprocon-0.1.0/PKG-INFO
```

### Comparing `statprocon-0.0.9/requirements-dev.txt` & `statprocon-0.1.0/requirements-dev.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,47 @@
 bleach==6.0.0
 build==0.10.0
+cachetools==5.3.1
 certifi==2023.5.7
 cffi==1.15.1
+chardet==5.1.0
 charset-normalizer==3.2.0
+colorama==0.4.6
 cryptography==41.0.1
+distlib==0.3.7
 docutils==0.20.1
+filelock==3.12.2
 idna==3.4
 importlib-metadata==6.8.0
 jaraco.classes==3.3.0
 jeepney==0.8.0
 keyring==24.2.0
 markdown-it-py==3.0.0
 mdurl==0.1.2
 more-itertools==9.1.0
 mypy==1.4.1
 mypy-extensions==1.0.0
 packaging==23.1
 pkginfo==1.9.6
+platformdirs==3.9.1
+pluggy==1.2.0
 pycparser==2.21
 Pygments==2.15.1
+pyproject-api==1.5.3
 pyproject_hooks==1.0.0
 readme-renderer==40.0
 requests==2.31.0
 requests-toolbelt==1.0.0
 rfc3986==2.0.0
 rich==13.4.2
 SecretStorage==3.3.3
 six==1.16.0
 statprocon @ file:///home/matt/projects/statprocon
 tomli==2.0.1
+tox==4.6.4
 twine==4.0.2
 types-docutils==0.20.0.1
 typing_extensions==4.7.1
 urllib3==2.0.3
+virtualenv==20.24.2
 webencodings==0.5.1
 zipp==3.16.0
```

### Comparing `statprocon-0.0.9/.idea/workspace.xml` & `statprocon-0.1.0/.idea/workspace.xml`

 * *Files 4% similar despite different names*

#### Comparing `statprocon-0.0.9/.idea/workspace.xml` & `statprocon-0.1.0/.idea/workspace.xml`

```diff
@@ -1,15 +1,15 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
     <list default="true" id="6b007249-c07a-402d-ab76-cd0adebb4623" name="Default Changelist" comment="">
-      <change beforePath="$PROJECT_DIR$/statprocon/charts/xmr.py" beforeDir="false" afterPath="$PROJECT_DIR$/statprocon/charts/xmr.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="FileTemplateManagerImpl">
@@ -90,27 +90,40 @@
       <created>1688827023388</created>
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
       <updated>1688827023388</updated>
       <workItem from="1688827024910" duration="1917000"/>
       <workItem from="1688848868641" duration="17704000"/>
       <workItem from="1688944372544" duration="17391000"/>
-      <workItem from="1690054614395" duration="20831000"/>
+      <workItem from="1690054614395" duration="31231000"/>
+      <workItem from="1690685043590" duration="11931000"/>
     </task>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
   <component name="Vcs.Log.Tabs.Properties">
     <option name="TAB_STATES">
       <map>
         <entry key="MAIN">
           <value>
-            <State/>
+            <State>
+              <option name="FILTERS">
+                <map>
+                  <entry key="branch">
+                    <value>
+                      <list>
+                        <option value="trended-limits"/>
+                      </list>
+                    </value>
+                  </entry>
+                </map>
+              </option>
+            </State>
           </value>
         </entry>
       </map>
     </option>
     <option name="oldMeFiltersMigrated" value="true"/>
   </component>
   <component name="com.intellij.coverage.CoverageDataManagerImpl">
```

### Comparing `statprocon-0.0.9/.idea/xmr.iml` & `statprocon-0.1.0/.idea/xmr.iml`

 * *Files 13% similar despite different names*

#### Comparing `statprocon-0.0.9/.idea/xmr.iml` & `statprocon-0.1.0/.idea/xmr.iml`

```diff
@@ -1,12 +1,13 @@
 <?xml version="1.0" encoding="utf-8"?>
 <module type="PYTHON_MODULE" version="4">
   <component name="NewModuleRootManager">
     <content url="file://$MODULE_DIR$">
       <excludeFolder url="file://$MODULE_DIR$/venv"/>
       <excludeFolder url="file://$MODULE_DIR$/.mypy_cache"/>
       <excludeFolder url="file://$MODULE_DIR$/dist"/>
+      <excludeFolder url="file://$MODULE_DIR$/.tox"/>
     </content>
     <orderEntry type="jdk" jdkName="Python 3.10 (statprocon)" jdkType="Python SDK"/>
     <orderEntry type="sourceFolder" forTests="false"/>
   </component>
 </module>
```

### Comparing `statprocon-0.0.9/statprocon/charts/xmr.py` & `statprocon-0.1.0/statprocon/charts/xmr/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,73 @@
 import csv
 import io
+import statistics
 
 from decimal import Decimal
-from typing import cast, Union, Optional, Sequence, TypeAlias
+from typing import cast, List, Optional, Sequence, Union
 
-TYPE_COUNT_VALUE: TypeAlias = Decimal | int
-TYPE_MOVING_RANGE_VALUE: TypeAlias = Decimal | int | None
+from .constants import ROUNDING
+from .types import (
+    TYPE_COUNTS,
+    TYPE_COUNTS_INPUT,
+    TYPE_MOVING_RANGE_VALUE,
+    TYPE_MOVING_RANGES,
+    TYPE_NUMERIC_INPUTS,
+)
+
+
+AVERAGE = 'average'
+MEDIAN = 'median'
+
+# Scaling Factors (SF)
+SF_LIMITS = {
+    AVERAGE: Decimal('2.660'),
+    MEDIAN: Decimal('3.145'),
+}
+
+SF_RANGES = {
+    AVERAGE: Decimal('3.268'),
+    MEDIAN: Decimal('3.865'),
+}
 
-TYPE_COUNTS: TypeAlias = Sequence[TYPE_COUNT_VALUE | float]
-TYPE_MOVING_RANGES: TypeAlias = Sequence[TYPE_MOVING_RANGE_VALUE]
-
-
-class XmR:
-    ROUNDING = 3
 
+class Base:
     def __init__(
             self,
-            counts: TYPE_COUNTS,
+            counts: TYPE_COUNTS_INPUT,
+            x_central_line_uses: str = AVERAGE,
+            moving_range_uses: str = AVERAGE,
             subset_start_index: int = 0,
             subset_end_index: Optional[int] = None,
     ):
         """
 
-        :param counts: TYPE_COUNTS list of data to be used by the X chart
+        :param counts: list of data to be used by the X chart
+        :param x_central_line_uses: Whether to use the 'average' or 'median' for computing the X
+            central line.  Defaults to average.
+        :param moving_range_uses: Whether to use the 'average' or 'median' moving range.
+            Defaults to average.
         :param subset_start_index: Optional starting index of counts to calculate limits from
         :param subset_end_index: Optional ending index of counts to calculate limits to
         """
-        self.counts = [Decimal(str(x)) for x in counts]
+        assert x_central_line_uses in [AVERAGE, MEDIAN]
+        assert moving_range_uses in [AVERAGE, MEDIAN]
+
+        self.counts = cast(TYPE_COUNTS, self.to_decimal_list(counts))
         self._mr: TYPE_MOVING_RANGES = []
         self.i = max(0, subset_start_index)
         self.j = len(counts)
         if subset_end_index:
             self.j = min(self.j, subset_end_index)
 
         assert self.i <= self.j
 
+        self._x_central_line_uses = x_central_line_uses
+        self._moving_range_uses = moving_range_uses
+
     def __repr__(self) -> str:
         result = ''
         for k, v in self.to_dict().items():
             k_format = '{0: <9}'.format(k)
             if isinstance(v, list):
                 values = '[' + ', '.join(map(str, v)) + ']'
             else:
@@ -103,52 +132,74 @@
             return self._mr
 
         result: list[TYPE_MOVING_RANGE_VALUE] = []
         for i, c in enumerate(self.counts):
             if i == 0:
                 result.append(None)
             else:
-                value = cast(Union[Decimal | int], abs(c - self.counts[i - 1]))
+                value = cast(Union[Decimal, int], abs(c - self.counts[i - 1]))
                 result.append(value)
         self._mr = result
         return self._mr
 
     def x_central_line(self) -> Sequence[Decimal]:
-        avg = self.mean(self.counts[self.i:self.j])
-        return [self.round(avg)] * len(self.counts)
+        if self._x_central_line_uses == AVERAGE:
+            value = self._mean(self.counts[self.i:self.j])
+        elif self._x_central_line_uses == MEDIAN:
+            raise NotImplemented
+
+        return [round(value, ROUNDING)] * len(self.counts)
 
     def mr_central_line(self) -> Sequence[Decimal]:
         mr = self.moving_ranges()
         assert mr[0] is None
-        valid_values = cast(TYPE_COUNTS, mr[self.i+1:self.j])
-        avg = self.mean(valid_values)
-        return [self.round(avg)] * len(mr)
+        valid_values = cast(TYPE_COUNTS, mr[self.i + 1:self.j])
+
+        if self._moving_range_uses == AVERAGE:
+            value = self._mean(valid_values)
+        elif self._moving_range_uses == MEDIAN:
+            # mypy gives the error:
+            #   Value of type variable "_NumberT" of "median" cannot be "Decimal | int"
+            # However, the [statistics library](https://docs.python.org/3/library/statistics.html)
+            # says that the functions support int and Decimal
+            # When ignoring type-var, an assignment error appears:
+            #   Incompatible types in assignment (expression has type "Decimal | int", variable has type "Decimal")
+            # But the variable can be int and not necessarily Decimal
+            value = statistics.median(valid_values)  # type: ignore[type-var,assignment]
+
+        return [round(value, ROUNDING)] * len(mr)
 
     def upper_range_limit(self) -> Sequence[Decimal]:
+        sf = SF_RANGES[self._moving_range_uses]
         mr_cl = self.mr_central_line()
-        limit = Decimal('3.268') * mr_cl[0]
-        return [self.round(limit)] * len(mr_cl)
+        limit = sf * mr_cl[0]
+        value = round(limit, ROUNDING)
+        return [value] * len(mr_cl)
 
     def upper_natural_process_limit(self) -> Sequence[Decimal]:
-        limit = self.x_central_line()[0] + (Decimal('2.660') * self.mr_central_line()[0])
-        return [self.round(limit)] * len(self.counts)
+        sf = SF_LIMITS[self._moving_range_uses]
+        limit = self.x_central_line()[0] + (sf * self.mr_central_line()[0])
+        value = round(limit, ROUNDING)
+        return [value] * len(self.counts)
 
     def lower_natural_process_limit(self) -> Sequence[Decimal]:
         """
         LNPL can be negative.
         It's the caller's responsibility to take max(LNPL, 0) if a negative LNPL does not make sense
         """
-        limit = self.x_central_line()[0] - (Decimal('2.660') * self.mr_central_line()[0])
-        return [self.round(limit)] * len(self.counts)
+        sf = SF_LIMITS[self._moving_range_uses]
+        limit = self.x_central_line()[0] - (sf * self.mr_central_line()[0])
+        value = round(limit, ROUNDING)
+        return [value] * len(self.counts)
 
     def rule_1_x_indices_beyond_limits(
             self,
             upper_limit: Optional[Decimal] = None,
-            lower_limit: Optional[Decimal] = None
-    ) -> list[bool]:
+            lower_limit: Optional[Decimal] = None,
+    ) -> List[bool]:
         """
         Points Outside the Limits
 
         A single point outside the computed limits
         on either the X Chart, or the mR Chart,
         should be interpreted as an indication of
         the presence of an assignable cause which has a *dominant* effect.
@@ -166,29 +217,29 @@
 
         lower = self.lower_natural_process_limit()
         if lower_limit:
             lower = [lower_limit] * n
 
         return self._points_beyond_limits(self.counts, upper, lower)
 
-    def rule_1_mr_indices_beyond_limits(self) -> list[bool]:
+    def rule_1_mr_indices_beyond_limits(self) -> List[bool]:
         """
         Points Outside the Limits
 
         A single point outside the computed limits
         on either the X Chart, or the mR Chart,
         should be interpreted as an indication of
         the presence of an assignable cause which has a *dominant* effect.
 
         :return: list[bool] A list of boolean values of length(self.moving_ranges())
             True at index i means that self.moving_ranges()[i] is above the Upper Range Limit
         """
         return self._points_beyond_limits(self.moving_ranges(), self.upper_range_limit())
 
-    def rule_2_runs_about_central_line(self) -> list[bool]:
+    def rule_2_runs_about_central_line(self) -> List[bool]:
         """
         Runs About the Central Line
 
         Eight successive values,
         all on the same side of the central line on the X Chart
         may be interpreted as an indication of
         the presence of an assignable cause which has a *weak* but sustained effect.
@@ -197,38 +248,36 @@
             True at index i means that self.counts[i] is above the line and part of a run of eight successive values
         """
 
         result = [False] * len(self.counts)
 
         # positive is number of consecutive points above the line
         # negative is number of consecutive points below the line
-        central_line = 0
-
-        avg = self.mean(self.counts)
-        for i, x in enumerate(self.counts):
-            if x > avg:
-                if central_line < 0:
-                    central_line = 1
+        run = 0
+        for i, (x, cl) in enumerate(zip(self.counts, self.x_central_line())):
+            if x > cl:
+                if run < 0:
+                    run = 1
                 else:
-                    central_line += 1
-            elif x < avg:
-                if central_line > 0:
-                    central_line = -1
+                    run += 1
+            elif x < cl:
+                if run > 0:
+                    run = -1
                 else:
-                    central_line -= 1
+                    run -= 1
 
-            if abs(central_line) == 8:
+            if abs(run) == 8:
                 for j in range(8):
                     result[i - j] = True
-            elif abs(central_line) > 8:
+            elif abs(run) > 8:
                 result[i] = True
 
         return result
 
-    def rule_3_runs_near_limits(self) -> list[bool]:
+    def rule_3_runs_near_limits(self) -> List[bool]:
         """
         Runs Near the Limits
 
         Three out of four successive values on the X Chart
         all within the upper 25% of the region between the limits, or
         all within the lower 25% of the region between the limits,
         may be interpreted as an indication of the presence
@@ -254,23 +303,20 @@
                 successive_values = near_limits[i - 3:i + 1]
                 if abs(sum(successive_values)) >= 3:
                     for j in range(i - 3, i + 1):
                         result[j] = True
 
         return result
 
-    def round(self, value: Decimal) -> Decimal:
-        return round(value, self.ROUNDING)
-
     @staticmethod
     def _points_beyond_limits(
-            data: TYPE_COUNTS | TYPE_MOVING_RANGES,
+            data: TYPE_MOVING_RANGES,
             upper_limits: Sequence[Decimal],
             lower_limits: Optional[Sequence[Decimal]] = None
-    ) -> list[bool]:
+    ) -> List[bool]:
         result = [False] * len(data)
 
         if lower_limits is None:
             lower_limits = [Decimal('-Inf')] * len(upper_limits)
 
         for i, (x, w, y) in enumerate(zip(data, lower_limits, upper_limits)):
             if x is None:  # first index of Moving Ranges
@@ -278,11 +324,21 @@
 
             if not w <= x <= y:
                 result[i] = True
 
         return result
 
     @staticmethod
-    def mean(nums: TYPE_COUNTS) -> Decimal:
+    def _mean(nums: TYPE_COUNTS) -> Decimal:
         s = sum(nums)
         n = len(nums)
         return Decimal(str(s)) / Decimal(str(n))
+
+    @staticmethod
+    def to_decimal_list(values: TYPE_NUMERIC_INPUTS) -> TYPE_MOVING_RANGES:
+        result: List[Union[Decimal, None]] = []
+        for x in values:
+            if x is None:
+                result.append(None)
+            else:
+                result.append(Decimal(str(x)))
+        return result
```

### Comparing `statprocon-0.0.9/tests/test_xmr.py` & `statprocon-0.1.0/tests/test_xmr.py`

 * *Files 9% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         mr = xmr.moving_ranges()
         self.assertEqual(mr, [None, Decimal('9.74'), Decimal('5.99')])
 
     def test_float_input(self):
         counts = [5.4, 3.8, 8.75, 3.6, 3, 6, 7.4, 10, 5.8, 6.6, 3, 8.8]
         xmr = XmR(counts)
         mr = xmr.moving_ranges()
-        expected = [None, Decimal('1.6'), Decimal('4.95'), Decimal('5.15'), Decimal('0.6'), Decimal('3'), Decimal('1.4'), Decimal('2.6'), Decimal('4.2'), Decimal('0.8'), Decimal('3.6'), Decimal('5.8')]
+        expected = xmr.to_decimal_list([None, 1.6, 4.95, 5.15, 0.6, 3, 1.4, 2.6, 4.2, 0.8, 3.6, 5.8])
         self.assertListEqual(mr, expected)
 
     def test_upper_range_limit(self):
         counts = [1,51, 100, 50]
         xmr = XmR(counts)
         self._assert_line_equals(xmr, 'upper_range_limit', Decimal('162.312'))
 
@@ -78,20 +78,17 @@
 
     def test_limits_with_subsets(self):
         counts = [1] * 25
         counts[1] = 10
         counts[2] = 100
         counts[3] = 50
 
-        xmr = XmR(counts, subset_end_index=24)
-        self._assert_line_equals(xmr, 'upper_natural_process_limit', Decimal('30.442'))
-        self._assert_line_equals(xmr, 'upper_range_limit', Decimal('28.134'))
-
-        # Adjust manually so that all subset values should be 1
-        xmr.i = 4
+        xmr = XmR(counts, subset_start_index=4, subset_end_index=24)
+        self._assert_line_equals(xmr, 'upper_natural_process_limit', Decimal('1.000'))
+        self._assert_line_equals(xmr, 'upper_range_limit', Decimal('0'))
         self._assert_line_equals(xmr, 'x_central_line', 1)
         self.assertEqual(xmr.lower_natural_process_limit(), xmr.upper_natural_process_limit())
 
     def test_rule_1_points_beyond_upper_limits(self):
         """
         This test dataset comes from Table 9.1: Accident Rates in Making Sense of Data
         """
@@ -125,18 +122,17 @@
     def test_rule_1_points_beyond_both_limits(self):
         """
         This test dataset comes from Table 9.2: Accounts Receivable for Years One and Two in Making Sense of Data
         """
 
         ar_pct_sales = [
             '55.6', '54.7', '54.9', '54.8', '56.9', '55.7', '53.8', '54.8', '53.4', '57.0', '59.4', '63.2',
-            '60.9', '60.7', '58.6', '57.3', '56.9', '58.1', '58.3', '50.9', '53.3', '52.5', '50.8', '52.9'
+            '60.9', '60.7', '58.6', '57.3', '56.9', '58.1', '58.3', '50.9', '53.3', '52.5', '50.8', '52.9',
         ]
-        counts_dec = list(map(lambda x: Decimal(x), ar_pct_sales))
-        xmr = XmR(counts_dec)
+        xmr = XmR(ar_pct_sales)
 
         upper_limit = Decimal('60.7')
         expected = [False] * len(ar_pct_sales)
         for i in [11, 12, 19, 22]:
             expected[i] = True
 
         actual = xmr.rule_1_x_indices_beyond_limits(upper_limit=upper_limit)
@@ -145,18 +141,19 @@
         # Point 13 is detected in the chart in the book because the actual percentage is slightly lower than the limit
         self.assertFalse(actual[13], 'Point 13 equals the limit and should not be detected')
 
     def test_rule_1_point_beyond_upper_range_limit(self):
         """
         This test dataset also comes from Table 9.2
         """
-        ar_pct_sales = ['55.6', '54.7', '54.9', '54.8', '56.9', '55.7', '53.8', '54.8', '53.4', '57.0', '59.4', '63.2',
-                        '60.9', '60.7', '58.6', '57.3', '56.9', '58.1', '58.3', '50.9', '53.3', '52.5', '50.8', '52.9']
-        counts_dec = list(map(lambda x: Decimal(x), ar_pct_sales))
-        xmr = XmR(counts_dec)
+        ar_pct_sales = [
+            '55.6', '54.7', '54.9', '54.8', '56.9', '55.7', '53.8', '54.8', '53.4', '57.0', '59.4', '63.2',
+            '60.9', '60.7', '58.6', '57.3', '56.9', '58.1', '58.3', '50.9', '53.3', '52.5', '50.8', '52.9',
+        ]
+        xmr = XmR(ar_pct_sales)
 
         expected = [False] * len(ar_pct_sales)
         expected[19] = True
         self.assertListEqual(xmr.rule_1_mr_indices_beyond_limits(), expected)
 
     def test_rule_2(self):
         """
@@ -176,16 +173,14 @@
         """
         Data comes from pg 130 of "Making Sense of Data"
         Figure 9.9 XmR Chart for AM Premedication Peak Flow Rates for Days 1 to 18
         @see test_peak_flow_rates
         """
 
         x_values = [120, 140, 100, 150, 260, 150, 100, 120, 300, 300, 275, 300, 140, 1750, 150, 150, 190, 180]
-        unpl = Decimal('322.5')
-        lnpl = Decimal('43.7')
 
         xmr = XmR(x_values)
 
         expected = [False] * len(x_values)
         for i in range(8, 4):
             expected[i] = True
         self.assertListEqual(xmr.rule_3_runs_near_limits(), expected)
@@ -203,41 +198,61 @@
         lnpl = Decimal('3188.72')
         unpl = Decimal('5082.28')
         url = Decimal('1163.19')
 
         xmr = XmR(counts)
 
         self.assertListEqual(xmr.moving_ranges(), moving_ranges)
-        self.assertEqual(x_avg, xmr.mean(counts))
+        self.assertEqual(x_avg, xmr.x_central_line()[0])
         self.assertEqual(mr_avg, round(xmr.mr_central_line()[0], 2))
         self.assertEqual(lnpl, round(xmr.lower_natural_process_limit()[0], 2))
         self.assertEqual(unpl, round(xmr.upper_natural_process_limit()[0], 2))
         self.assertEqual(url, round(xmr.upper_range_limit()[0], 2))
 
     def test_peak_flow_rates(self):
         """
         Data comes from pg 130 of "Making Sense of Data"
         Figure 9.9 XmR Chart for AM Premedication Peak Flow Rates for Days 1 to 18
         """
 
         x_values = [120, 140, 100, 150, 260, 150, 100, 120, 300, 300, 275, 300, 140, 170, 150, 150, 190, 180]
         mr_values = [None, 20, 40, 50, 110, 110, 50, 20, 180, 0, 25, 25, 160, 30, 20, 0, 40, 10]
-        x_avg = Decimal('183.1')
-        mr_avg = Decimal('52.4')
+        x_cl = Decimal('183.1')
+        mr_cl = Decimal('52.4')
 
         # changes are due to rounding
         unpl = Decimal('322.3')  # 322.5 in book
         lnpl = Decimal('43.8')  # 43.7 in book
         url = Decimal('171.1')  # 171.3 in book
 
         xmr = XmR(x_values)
 
         self.assertListEqual(xmr.moving_ranges(), mr_values)
-        self.assertEqual(x_avg, round(xmr.mean(x_values), 1))
-        self.assertEqual(mr_avg, round(xmr.mr_central_line()[0], 1))
+        self.assertEqual(x_cl, round(xmr.x_central_line()[0], 1))
+        self.assertEqual(mr_cl, round(xmr.mr_central_line()[0], 1))
         self.assertEqual(lnpl, round(xmr.lower_natural_process_limit()[0], 1))
         self.assertEqual(unpl, round(xmr.upper_natural_process_limit()[0], 1))
         self.assertEqual(url, round(xmr.upper_range_limit()[0], 1))
 
+    def test_median_moving_range(self):
+        # Data comes from pg. 145 of Making Sense of Data
+        # Section 10.2 Using the Median Moving Range
+        x_values = [2.5, 2.3, 16.3, 6.3, 7.6, 16.3, 7.1, 7.8, 7.8, 9.9, 10.5, -4.8]
+        mr_values = [None, 0.2, 14, 10, 1.3, 8.7, 9.2, 0.7, 0, 2.1, 0.6, 15.3]
+        x_cl = Decimal('7.467')  # 7.47 in book
+        mr_cl = Decimal('2.10')
+        unpl = Decimal('14.072')  # 14.07 in book
+        lnpl = Decimal('0.862')  # 0.87 in book
+        url = Decimal('8.116')  # 8.12 in book
+
+        xmr = XmR(x_values, moving_range_uses='median')
+
+        self.assertListEqual(xmr.moving_ranges(), xmr.to_decimal_list(mr_values))
+        self.assertEqual(x_cl, xmr.x_central_line()[0])
+        self.assertEqual(mr_cl, xmr.mr_central_line()[0])
+        self.assertEqual(lnpl, xmr.lower_natural_process_limit()[0])
+        self.assertEqual(unpl, xmr.upper_natural_process_limit()[0])
+        self.assertEqual(url, xmr.upper_range_limit()[0])
+
     def _assert_line_equals(self, xmr, func, value):
         actual = getattr(xmr, func)()
         self.assertListEqual(actual, [value] * len(xmr.counts))
```

### Comparing `statprocon-0.0.9/LICENSE` & `statprocon-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `statprocon-0.0.9/README.md` & `statprocon-0.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -80,14 +80,22 @@
 1. Click the 3 dot menu on the right next to `LNPL`
 1. Click `Remove`
 
 The LNPL line will be removed from the X Chart.
 
 ## Advanced Usage
 
+### Use the Median Moving Range
+
+If your data contains extreme outliers, it may be better to compute the limits using the median moving range.
+
+```python
+xmr = XmR(counts, moving_range_uses='median')
+```
+
 ### Calculate Limits from Subset of Counts
 
 The central lines and limits calculations can be restricted to a subset of the count data.
 Use the `subset_start_index` and `subset_end_index` parameters when instantiating the XmR object:
 
 ```python
 xmr = XmR(counts, subset_start_index=10, subset_end_index=34)  # 24 points of data starting at index 10
@@ -136,9 +144,9 @@
 [Install package from source](https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/#installing-from-source)
 ```shell
 python3 -m pip install .
 ```
 
 Run tests
 ```shell
-python3 -m unittest discover
+tox
 ```
```

### Comparing `statprocon-0.0.9/pyproject.toml` & `statprocon-0.1.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "statprocon"
-version = "0.0.9"
+version = "0.1.0"
 authors = [
   { name="Matt McCormick", email="mattmccor@gmail.com" },
 ]
 description = "A Python helper library for generating Process Behaviour Charts"
 readme = "README.md"
-requires-python = ">=3.10"
+requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 keywords = ["Statistical Process Control", "SPC", "Quality Control Chart", "QCC", "Process Behaviour Chart", "Process Behavior Chart", "XmR", "Shewhart", "Wheeler"]
+dependencies = [
+    "packaging",
+    "typing_extensions",
+]
 
 [project.urls]
 "Homepage" = "https://github.com/mattmccormick/statprocon"
 "Bug Tracker" = "https://github.com/mattmccormick/statprocon/issues"
 "Changelog" = "https://github.com/mattmccormick/statprocon/blob/main/CHANGELOG.md"
```

### Comparing `statprocon-0.0.9/PKG-INFO` & `statprocon-0.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: statprocon
-Version: 0.0.9
+Version: 0.1.0
 Summary: A Python helper library for generating Process Behaviour Charts
 Project-URL: Homepage, https://github.com/mattmccormick/statprocon
 Project-URL: Bug Tracker, https://github.com/mattmccormick/statprocon/issues
 Project-URL: Changelog, https://github.com/mattmccormick/statprocon/blob/main/CHANGELOG.md
 Author-email: Matt McCormick <mattmccor@gmail.com>
 License-File: LICENSE
 Keywords: Process Behavior Chart,Process Behaviour Chart,QCC,Quality Control Chart,SPC,Shewhart,Statistical Process Control,Wheeler,XmR
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10
+Requires-Python: >=3.7
+Requires-Dist: packaging
+Requires-Dist: typing-extensions
 Description-Content-Type: text/markdown
 
 # statprocon
 
 **statprocon** is a Python helper library for generating data for use in **Stat**istical **Pro**cess **Con**trol charts.
 SPC charts are also known as Process Behaviour Charts, Control charts or Shewhart charts.
 
@@ -96,14 +98,22 @@
 1. Click the 3 dot menu on the right next to `LNPL`
 1. Click `Remove`
 
 The LNPL line will be removed from the X Chart.
 
 ## Advanced Usage
 
+### Use the Median Moving Range
+
+If your data contains extreme outliers, it may be better to compute the limits using the median moving range.
+
+```python
+xmr = XmR(counts, moving_range_uses='median')
+```
+
 ### Calculate Limits from Subset of Counts
 
 The central lines and limits calculations can be restricted to a subset of the count data.
 Use the `subset_start_index` and `subset_end_index` parameters when instantiating the XmR object:
 
 ```python
 xmr = XmR(counts, subset_start_index=10, subset_end_index=34)  # 24 points of data starting at index 10
@@ -152,9 +162,9 @@
 [Install package from source](https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/#installing-from-source)
 ```shell
 python3 -m pip install .
 ```
 
 Run tests
 ```shell
-python3 -m unittest discover
+tox
 ```
```

