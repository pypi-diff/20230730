# Comparing `tmp/statprocon-0.1.0.tar.gz` & `tmp/statprocon-0.1.1.tar.gz`

## Comparing `statprocon-0.1.0.tar` & `statprocon-0.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 statprocon-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 statprocon-0.1.0/CODEOWNERS
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 statprocon-0.1.0/requirements-dev.txt
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 statprocon-0.1.0/tox.ini
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 statprocon-0.1.0/.idea/.gitignore
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 statprocon-0.1.0/.idea/dataSources.local.xml
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 statprocon-0.1.0/.idea/misc.xml
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 statprocon-0.1.0/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 statprocon-0.1.0/.idea/vcs.xml
--rw-r--r--   0        0        0     6269 2020-02-02 00:00:00.000000 statprocon-0.1.0/.idea/workspace.xml
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 statprocon-0.1.0/.idea/xmr.iml
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 statprocon-0.1.0/.idea/codeStyles/codeStyleConfig.xml
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 statprocon-0.1.0/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 statprocon-0.1.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 statprocon-0.1.0/statprocon/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 statprocon-0.1.0/statprocon/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 statprocon-0.1.0/statprocon/charts/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 statprocon-0.1.0/statprocon/charts/xmr/__init__.py
--rw-r--r--   0        0        0    11948 2020-02-02 00:00:00.000000 statprocon-0.1.0/statprocon/charts/xmr/base.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 statprocon-0.1.0/statprocon/charts/xmr/constants.py
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 statprocon-0.1.0/statprocon/charts/xmr/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 statprocon-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     9942 2020-02-02 00:00:00.000000 statprocon-0.1.0/tests/test_xmr.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 statprocon-0.1.0/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 statprocon-0.1.0/LICENSE
--rw-r--r--   0        0        0     4514 2020-02-02 00:00:00.000000 statprocon-0.1.0/README.md
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 statprocon-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5353 2020-02-02 00:00:00.000000 statprocon-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 statprocon-0.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 statprocon-0.1.1/CODEOWNERS
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 statprocon-0.1.1/requirements-dev.txt
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 statprocon-0.1.1/tox.ini
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 statprocon-0.1.1/.idea/.gitignore
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 statprocon-0.1.1/.idea/dataSources.local.xml
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 statprocon-0.1.1/.idea/misc.xml
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 statprocon-0.1.1/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 statprocon-0.1.1/.idea/vcs.xml
+-rw-r--r--   0        0        0     6831 2020-02-02 00:00:00.000000 statprocon-0.1.1/.idea/workspace.xml
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 statprocon-0.1.1/.idea/xmr.iml
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 statprocon-0.1.1/.idea/codeStyles/codeStyleConfig.xml
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 statprocon-0.1.1/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 statprocon-0.1.1/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 statprocon-0.1.1/statprocon/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 statprocon-0.1.1/statprocon/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 statprocon-0.1.1/statprocon/charts/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 statprocon-0.1.1/statprocon/charts/xmr/__init__.py
+-rw-r--r--   0        0        0    12222 2020-02-02 00:00:00.000000 statprocon-0.1.1/statprocon/charts/xmr/base.py
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 statprocon-0.1.1/statprocon/charts/xmr/constants.py
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 statprocon-0.1.1/statprocon/charts/xmr/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 statprocon-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0    10865 2020-02-02 00:00:00.000000 statprocon-0.1.1/tests/test_xmr.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 statprocon-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 statprocon-0.1.1/LICENSE
+-rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 statprocon-0.1.1/README.md
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 statprocon-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5906 2020-02-02 00:00:00.000000 statprocon-0.1.1/PKG-INFO
```

### Comparing `statprocon-0.1.0/CHANGELOG.md` & `statprocon-0.1.1/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Release History
 
 ---
 
+## 0.1.1
+
+- Add parameter `x_central_line_uses` to accept `median` and return the median for the X central line
+
 ## 0.1.0
 
 - Add parameter `moving_range_uses` to accept `median` and compute the limits using the median moving range
 
 ## 0.0.10
 
 - Change minimum required Python version to 3.7
```

### Comparing `statprocon-0.1.0/requirements-dev.txt` & `statprocon-0.1.1/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `statprocon-0.1.0/.idea/workspace.xml` & `statprocon-0.1.1/.idea/workspace.xml`

 * *Files 11% similar despite different names*

#### Comparing `statprocon-0.1.0/.idea/workspace.xml` & `statprocon-0.1.1/.idea/workspace.xml`

```diff
@@ -1,15 +1,19 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
     <list default="true" id="6b007249-c07a-402d-ab76-cd0adebb4623" name="Default Changelist" comment="">
+      <change beforePath="$PROJECT_DIR$/CHANGELOG.md" beforeDir="false" afterPath="$PROJECT_DIR$/CHANGELOG.md" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/README.md" beforeDir="false" afterPath="$PROJECT_DIR$/README.md" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/statprocon/charts/xmr/base.py" beforeDir="false" afterPath="$PROJECT_DIR$/statprocon/charts/xmr/base.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/tests/test_xmr.py" beforeDir="false" afterPath="$PROJECT_DIR$/tests/test_xmr.py" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="FileTemplateManagerImpl">
@@ -91,15 +95,15 @@
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
       <updated>1688827023388</updated>
       <workItem from="1688827024910" duration="1917000"/>
       <workItem from="1688848868641" duration="17704000"/>
       <workItem from="1688944372544" duration="17391000"/>
       <workItem from="1690054614395" duration="31231000"/>
-      <workItem from="1690685043590" duration="11931000"/>
+      <workItem from="1690685043590" duration="13677000"/>
     </task>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
   <component name="Vcs.Log.Tabs.Properties">
```

### Comparing `statprocon-0.1.0/.idea/xmr.iml` & `statprocon-0.1.1/.idea/xmr.iml`

 * *Files identical despite different names*

### Comparing `statprocon-0.1.0/statprocon/charts/xmr/base.py` & `statprocon-0.1.1/statprocon/charts/xmr/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,16 @@
             subset_start_index: int = 0,
             subset_end_index: Optional[int] = None,
     ):
         """
 
         :param counts: list of data to be used by the X chart
         :param x_central_line_uses: Whether to use the 'average' or 'median' for computing the X
-            central line.  Defaults to average.
+            central line.  Defaults to average.  If set to median, moving_range_uses will also be
+            set to median.
         :param moving_range_uses: Whether to use the 'average' or 'median' moving range.
             Defaults to average.
         :param subset_start_index: Optional starting index of counts to calculate limits from
         :param subset_end_index: Optional ending index of counts to calculate limits to
         """
         assert x_central_line_uses in [AVERAGE, MEDIAN]
         assert moving_range_uses in [AVERAGE, MEDIAN]
@@ -58,15 +59,18 @@
         self.j = len(counts)
         if subset_end_index:
             self.j = min(self.j, subset_end_index)
 
         assert self.i <= self.j
 
         self._x_central_line_uses = x_central_line_uses
-        self._moving_range_uses = moving_range_uses
+        if x_central_line_uses == MEDIAN:
+            self._moving_range_uses = MEDIAN
+        else:
+            self._moving_range_uses = moving_range_uses
 
     def __repr__(self) -> str:
         result = ''
         for k, v in self.to_dict().items():
             k_format = '{0: <9}'.format(k)
             if isinstance(v, list):
                 values = '[' + ', '.join(map(str, v)) + ']'
@@ -138,18 +142,19 @@
             else:
                 value = cast(Union[Decimal, int], abs(c - self.counts[i - 1]))
                 result.append(value)
         self._mr = result
         return self._mr
 
     def x_central_line(self) -> Sequence[Decimal]:
+        valid_values = self.counts[self.i:self.j]
         if self._x_central_line_uses == AVERAGE:
-            value = self._mean(self.counts[self.i:self.j])
+            value = self._mean(valid_values)
         elif self._x_central_line_uses == MEDIAN:
-            raise NotImplemented
+            value = statistics.median(valid_values)  # type: ignore[type-var,assignment]
 
         return [round(value, ROUNDING)] * len(self.counts)
 
     def mr_central_line(self) -> Sequence[Decimal]:
         mr = self.moving_ranges()
         assert mr[0] is None
         valid_values = cast(TYPE_COUNTS, mr[self.i + 1:self.j])
```

### Comparing `statprocon-0.1.0/statprocon/charts/xmr/types.py` & `statprocon-0.1.1/statprocon/charts/xmr/types.py`

 * *Files identical despite different names*

### Comparing `statprocon-0.1.0/tests/test_xmr.py` & `statprocon-0.1.1/tests/test_xmr.py`

 * *Files 3% similar despite different names*

```diff
@@ -249,10 +249,33 @@
         self.assertListEqual(xmr.moving_ranges(), xmr.to_decimal_list(mr_values))
         self.assertEqual(x_cl, xmr.x_central_line()[0])
         self.assertEqual(mr_cl, xmr.mr_central_line()[0])
         self.assertEqual(lnpl, xmr.lower_natural_process_limit()[0])
         self.assertEqual(unpl, xmr.upper_natural_process_limit()[0])
         self.assertEqual(url, xmr.upper_range_limit()[0])
 
+    def test_median_x_central_line(self):
+        # Data comes from pg. 147 of Making Sense of Data
+        # s10.2 Episode Treatment Groups
+        x_values = [
+            260, 130, 189, 1080, 175, 200, 193, 120, 33,
+            293, 195, 571, 55698, 209, 1825, 239, 290, 254,
+            93, 278, 185, 123, 9434, 408, 570, 118, 238,
+            207, 153, 209, 243, 110, 306, 343, 244,
+        ]
+        x_cl = 238
+        mr_cl = 125
+        unpl = 631.125  # 630 in book
+        lnpl = -155.125  # -154 in book
+        url = 483.125  # 482 in book
+
+        xmr = XmR(x_values, x_central_line_uses='median')
+
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

### Comparing `statprocon-0.1.0/LICENSE` & `statprocon-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `statprocon-0.1.0/README.md` & `statprocon-0.1.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 # statprocon
 
 **statprocon** is a Python helper library for generating data for use in **Stat**istical **Pro**cess **Con**trol charts.
 SPC charts are also known as Process Behaviour Charts, Control charts or Shewhart charts.
 
+SPC Charts help answer questions like:
+- How do I know a change has occurred in a process?
+- What is the expected variation in a process?
+- Is a process stable or unpredictable?
+
 ## Installation
 
 ```shell
 pip install statprocon
 ```
 
 ## Usage
@@ -24,15 +29,15 @@
 
 url = xmr.upper_range_limit()[0]  # 65.36
 mr_cl = xmr.mr_central_line()[0]  # 20
 
 ```
 
 Currently, this library only supports the data for generating an XmR chart.
-An XmR chart is the simplest type of process behaviour chart.
+An XmR chart is the most universal way of using process behaviour charts.
 XmR is short for individual values (X) and a moving range (mR).
 More chart data options can be added via pull requests.
 
 For more information, please read [Making Sense of Data by Donald Wheeler](https://www.amazon.com/Making-Sense-Data-Donald-Wheeler/dp/0945320728).
 
 ### pandas
 
@@ -88,14 +93,27 @@
 
 If your data contains extreme outliers, it may be better to compute the limits using the median moving range.
 
 ```python
 xmr = XmR(counts, moving_range_uses='median')
 ```
 
+### Use the Median for the X Central Line
+
+```python
+xmr = XmR(counts, x_central_line_uses='median')
+```
+
+Note: It's assumed that by using the median for the X central line that the median moving range should also be used.
+For example, you **cannot** do the following:
+
+```python
+xmr = XmR(counts, x_central_line_uses='median', moving_range_uses='average')
+```
+
 ### Calculate Limits from Subset of Counts
 
 The central lines and limits calculations can be restricted to a subset of the count data.
 Use the `subset_start_index` and `subset_end_index` parameters when instantiating the XmR object:
 
 ```python
 xmr = XmR(counts, subset_start_index=10, subset_end_index=34)  # 24 points of data starting at index 10
```

### Comparing `statprocon-0.1.0/pyproject.toml` & `statprocon-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "statprocon"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Matt McCormick", email="mattmccor@gmail.com" },
 ]
 description = "A Python helper library for generating Process Behaviour Charts"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `statprocon-0.1.0/PKG-INFO` & `statprocon-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statprocon
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python helper library for generating Process Behaviour Charts
 Project-URL: Homepage, https://github.com/mattmccormick/statprocon
 Project-URL: Bug Tracker, https://github.com/mattmccormick/statprocon/issues
 Project-URL: Changelog, https://github.com/mattmccormick/statprocon/blob/main/CHANGELOG.md
 Author-email: Matt McCormick <mattmccor@gmail.com>
 License-File: LICENSE
 Keywords: Process Behavior Chart,Process Behaviour Chart,QCC,Quality Control Chart,SPC,Shewhart,Statistical Process Control,Wheeler,XmR
@@ -17,14 +17,19 @@
 Description-Content-Type: text/markdown
 
 # statprocon
 
 **statprocon** is a Python helper library for generating data for use in **Stat**istical **Pro**cess **Con**trol charts.
 SPC charts are also known as Process Behaviour Charts, Control charts or Shewhart charts.
 
+SPC Charts help answer questions like:
+- How do I know a change has occurred in a process?
+- What is the expected variation in a process?
+- Is a process stable or unpredictable?
+
 ## Installation
 
 ```shell
 pip install statprocon
 ```
 
 ## Usage
@@ -42,15 +47,15 @@
 
 url = xmr.upper_range_limit()[0]  # 65.36
 mr_cl = xmr.mr_central_line()[0]  # 20
 
 ```
 
 Currently, this library only supports the data for generating an XmR chart.
-An XmR chart is the simplest type of process behaviour chart.
+An XmR chart is the most universal way of using process behaviour charts.
 XmR is short for individual values (X) and a moving range (mR).
 More chart data options can be added via pull requests.
 
 For more information, please read [Making Sense of Data by Donald Wheeler](https://www.amazon.com/Making-Sense-Data-Donald-Wheeler/dp/0945320728).
 
 ### pandas
 
@@ -106,14 +111,27 @@
 
 If your data contains extreme outliers, it may be better to compute the limits using the median moving range.
 
 ```python
 xmr = XmR(counts, moving_range_uses='median')
 ```
 
+### Use the Median for the X Central Line
+
+```python
+xmr = XmR(counts, x_central_line_uses='median')
+```
+
+Note: It's assumed that by using the median for the X central line that the median moving range should also be used.
+For example, you **cannot** do the following:
+
+```python
+xmr = XmR(counts, x_central_line_uses='median', moving_range_uses='average')
+```
+
 ### Calculate Limits from Subset of Counts
 
 The central lines and limits calculations can be restricted to a subset of the count data.
 Use the `subset_start_index` and `subset_end_index` parameters when instantiating the XmR object:
 
 ```python
 xmr = XmR(counts, subset_start_index=10, subset_end_index=34)  # 24 points of data starting at index 10
```

