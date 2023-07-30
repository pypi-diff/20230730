# Comparing `tmp/stockstats-0.6.1.tar.gz` & `tmp/stockstats-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stockstats-0.6.1.tar", last modified: Thu Jul 27 12:53:58 2023, max compression
+gzip compressed data, was "stockstats-0.6.2.tar", last modified: Sun Jul 30 07:07:26 2023, max compression
```

## Comparing `stockstats-0.6.1.tar` & `stockstats-0.6.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:53:58.055655 stockstats-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-27 12:53:43.000000 stockstats-0.6.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-27 12:53:43.000000 stockstats-0.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    38602 2023-07-27 12:53:58.055655 stockstats-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    37670 2023-07-27 12:53:43.000000 stockstats-0.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-27 12:53:43.000000 stockstats-0.6.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-27 12:53:58.055655 stockstats-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-07-27 12:53:43.000000 stockstats-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:53:58.055655 stockstats-0.6.1/stockstats.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    38602 2023-07-27 12:53:58.000000 stockstats-0.6.1/stockstats.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-27 12:53:58.000000 stockstats-0.6.1/stockstats.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 12:53:58.000000 stockstats-0.6.1/stockstats.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-27 12:53:58.000000 stockstats-0.6.1/stockstats.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-27 12:53:58.000000 stockstats-0.6.1/stockstats.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    65458 2023-07-27 12:53:43.000000 stockstats-0.6.1/stockstats.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-27 12:53:43.000000 stockstats-0.6.1/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 07:07:26.142691 stockstats-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-30 07:07:12.000000 stockstats-0.6.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-30 07:07:12.000000 stockstats-0.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    38602 2023-07-30 07:07:26.142691 stockstats-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    37670 2023-07-30 07:07:12.000000 stockstats-0.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-30 07:07:12.000000 stockstats-0.6.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-30 07:07:26.142691 stockstats-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-07-30 07:07:12.000000 stockstats-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 07:07:26.142691 stockstats-0.6.2/stockstats.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    38602 2023-07-30 07:07:26.000000 stockstats-0.6.2/stockstats.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-30 07:07:26.000000 stockstats-0.6.2/stockstats.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 07:07:26.000000 stockstats-0.6.2/stockstats.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-30 07:07:26.000000 stockstats-0.6.2/stockstats.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-30 07:07:26.000000 stockstats-0.6.2/stockstats.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    65549 2023-07-30 07:07:12.000000 stockstats-0.6.2/stockstats.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-30 07:07:12.000000 stockstats-0.6.2/test-requirements.txt
```

### Comparing `stockstats-0.6.1/LICENSE.txt` & `stockstats-0.6.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stockstats-0.6.1/PKG-INFO` & `stockstats-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stockstats
-Version: 0.6.1
+Version: 0.6.2
 Summary: DataFrame with inline stock statistics support.
 Home-page: https://github.com/jealous/stockstats
 Author: Cedric Zhuang
 Author-email: jealous@163.com
 License: BSD
 Keywords: stock statistics indicator
 Platform: any
@@ -25,15 +25,15 @@
 
 # Stock Statistics/Indicators Calculation Helper
 
 [![build & test](https://github.com/jealous/stockstats/actions/workflows/build-test.yml/badge.svg)](https://github.com/jealous/stockstats/actions/workflows/build-test.yml)
 [![codecov](https://codecov.io/gh/jealous/stockstats/branch/master/graph/badge.svg?token=IFMD1pVJ7T)](https://codecov.io/gh/jealous/stockstats)
 [![pypi](https://img.shields.io/pypi/v/stockstats.svg)](https://pypi.python.org/pypi/stockstats)
 
-VERSION: 0.6.1
+VERSION: 0.6.2
 
 ## Introduction
 
 Supply a wrapper ``StockDataFrame`` for ``pandas.DataFrame`` with inline stock
 statistics/indicators support.
 
 Supported statistics/indicators are:
```

### Comparing `stockstats-0.6.1/README.md` & `stockstats-0.6.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Stock Statistics/Indicators Calculation Helper
 
 [![build & test](https://github.com/jealous/stockstats/actions/workflows/build-test.yml/badge.svg)](https://github.com/jealous/stockstats/actions/workflows/build-test.yml)
 [![codecov](https://codecov.io/gh/jealous/stockstats/branch/master/graph/badge.svg?token=IFMD1pVJ7T)](https://codecov.io/gh/jealous/stockstats)
 [![pypi](https://img.shields.io/pypi/v/stockstats.svg)](https://pypi.python.org/pypi/stockstats)
 
-VERSION: 0.6.1
+VERSION: 0.6.2
 
 ## Introduction
 
 Supply a wrapper ``StockDataFrame`` for ``pandas.DataFrame`` with inline stock
 statistics/indicators support.
 
 Supported statistics/indicators are:
```

### Comparing `stockstats-0.6.1/setup.py` & `stockstats-0.6.2/setup.py`

 * *Files identical despite different names*

### Comparing `stockstats-0.6.1/stockstats.egg-info/PKG-INFO` & `stockstats-0.6.2/stockstats.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stockstats
-Version: 0.6.1
+Version: 0.6.2
 Summary: DataFrame with inline stock statistics support.
 Home-page: https://github.com/jealous/stockstats
 Author: Cedric Zhuang
 Author-email: jealous@163.com
 License: BSD
 Keywords: stock statistics indicator
 Platform: any
@@ -25,15 +25,15 @@
 
 # Stock Statistics/Indicators Calculation Helper
 
 [![build & test](https://github.com/jealous/stockstats/actions/workflows/build-test.yml/badge.svg)](https://github.com/jealous/stockstats/actions/workflows/build-test.yml)
 [![codecov](https://codecov.io/gh/jealous/stockstats/branch/master/graph/badge.svg?token=IFMD1pVJ7T)](https://codecov.io/gh/jealous/stockstats)
 [![pypi](https://img.shields.io/pypi/v/stockstats.svg)](https://pypi.python.org/pypi/stockstats)
 
-VERSION: 0.6.1
+VERSION: 0.6.2
 
 ## Introduction
 
 Supply a wrapper ``StockDataFrame`` for ``pandas.DataFrame`` with inline stock
 statistics/indicators support.
 
 Supported statistics/indicators are:
```

### Comparing `stockstats-0.6.1/stockstats.py` & `stockstats-0.6.2/stockstats.py`

 * *Files 1% similar despite different names*

```diff
@@ -355,15 +355,15 @@
         negative values meaning data in the past,
         positive values meaning data in the future.
         """
         shift = -meta.int
         self[meta.name] = self.roc(self[meta.column], shift)
 
     @staticmethod
-    def _shift(series: pd.Series, window: int):
+    def s_shift(series: pd.Series, window: int):
         """ Shift the series
 
         When window is negative, shift the past period to current.
         Fill the gap with the first data available.
 
         When window is positive, shift the future period to current.
         Fill the gap with last data available.
@@ -382,19 +382,19 @@
     def _get_s(self, meta: _Meta):
         """ Get the column shifted by periods
 
         Note this method is different to the shift method of pandas.
         negative values meaning data in the past,
         positive values meaning data in the future.
         """
-        self[meta.name] = self._shift(self[meta.column], meta.int)
+        self[meta.name] = self.s_shift(self[meta.column], meta.int)
 
     def _get_log_ret(self, _: _Meta):
         close = self['close']
-        self['log-ret'] = np.log(close / self._shift(close, -1))
+        self['log-ret'] = np.log(close / self.s_shift(close, -1))
 
     def _get_c(self, meta: _Meta) -> pd.Series:
         """ get the count of column in range (shifts)
 
         example: change_20_c
         :return: result series
         """
@@ -420,15 +420,15 @@
     def _shifted_columns(self,
                          column: pd.Series,
                          shifts: list[int]) -> pd.DataFrame:
         # initialize the column if not
         col = self.get(column)
         res = pd.DataFrame()
         for i in shifts:
-            res[int(i)] = self._shift(col, i).values
+            res[int(i)] = self.s_shift(col, i).values
         return res
 
     def _get_max(self, meta: _Meta):
         column = meta.column
         shifts = meta.ints
         cols = self._shifted_columns(column, shifts)
         self[meta.name] = cols.max(axis=1).values
@@ -534,15 +534,15 @@
 
         https://www.investopedia.com/articles/technical/02/092402.asp
         """
         window = meta.int
         single = self.ema(self[meta.column], window)
         double = self.ema(single, window)
         triple = self.ema(double, window)
-        prev_triple = self._shift(triple, -1)
+        prev_triple = self.s_shift(triple, -1)
         triple_change = self._delta(triple, -1)
         self[meta.name] = triple_change * 100 / prev_triple
 
     def _get_tema(self, meta: _Meta):
         """ Another implementation for triple ema
 
         Check the algorithm described below:
@@ -581,15 +581,15 @@
         window = meta.int
         tp = self._tp()
         tp_sma = self.sma(tp, window)
         mad = self._mad(tp, window)
         self[meta.name] = (tp - tp_sma) / (.015 * mad)
 
     def _tr(self):
-        prev_close = self._shift(self['close'], -1)
+        prev_close = self.s_shift(self['close'], -1)
         high = self['high']
         low = self['low']
         c1 = high - low
         c2 = (high - prev_close).abs()
         c3 = (low - prev_close).abs()
         return pd.concat((c1, c2, c3), axis=1).max(axis=1)
 
@@ -720,15 +720,18 @@
         * μ = the mean
         * σ = the standard deviation
         """
         window = meta.int
         col = self[meta.column]
         mean = self.sma(col, window)
         std = self.mov_std(col, window)
-        self[meta.name] = ((col - mean) / std).fillna(0.0)
+        value = (col - mean) / std
+        if len(value) > 1:
+            value.iloc[0] = value.iloc[1]
+        self[meta.name] = value
 
     def _atr(self, window):
         tr = self._tr()
         return self.smma(tr, window)
 
     def _get_atr(self, meta: _Meta):
         """ Average True Range
@@ -850,16 +853,16 @@
         https://support.futunn.com/en/topic167/?lang=en-us
         Use the relationship between the highest price, the lowest price and
         yesterday's middle price to reflect the market's willingness to buy
         and sell.
         """
         window = meta.int
         middle = self._tp()
-        last_middle = self._shift(middle, -1)
-        ym = self._shift(middle, -1)
+        last_middle = self.s_shift(middle, -1)
+        ym = self.s_shift(middle, -1)
         high = self['high']
         low = self['low']
         p1_m = pd.concat((last_middle, high), axis=1).min(axis=1)
         p2_m = pd.concat((last_middle, low), axis=1).min(axis=1)
         p1 = self.mov_sum(high - p1_m, window)
         p2 = self.mov_sum(ym - p2_m, window)
 
@@ -867,15 +870,15 @@
         self[name] = cr = p1 / p2 * 100
         self[f'{name}-ma1'] = self._shifted_cr_sma(cr, self.CR_MA[0])
         self[f'{name}-ma2'] = self._shifted_cr_sma(cr, self.CR_MA[1])
         self[f'{name}-ma3'] = self._shifted_cr_sma(cr, self.CR_MA[2])
 
     def _shifted_cr_sma(self, cr, window):
         cr_sma = self.sma(cr, window)
-        return self._shift(cr_sma, -int(window / 2.5 + 1))
+        return self.s_shift(cr_sma, -int(window / 2.5 + 1))
 
     def _tp(self):
         if 'amount' in self:
             return self['amount'] / self['volume']
         return (self['close'] + self['high'] + self['low']).divide(3.0)
 
     def _get_tp(self, meta: _Meta):
@@ -1332,15 +1335,15 @@
 
         The definition of money flow index is available at:
         https://www.investopedia.com/terms/m/mfi.asp
         """
         window = meta.int
         middle = self._tp()
         money_flow = (middle * self["volume"]).fillna(0.0)
-        shifted = self._shift(middle, -1)
+        shifted = self.s_shift(middle, -1)
         delta = (middle - shifted).fillna(0)
         pos_flow = money_flow.mask(delta < 0, 0)
         neg_flow = money_flow.mask(delta >= 0, 0)
         rolling_pos_flow = self.mov_sum(pos_flow, window)
         rolling_neg_flow = self.mov_sum(neg_flow, window)
         money_flow_ratio = rolling_pos_flow / (rolling_neg_flow + 1e-12)
         mfi = (1.0 - 1.0 / (1 + money_flow_ratio))
@@ -1403,15 +1406,15 @@
         divisor = sum_up + sum_down
         res = 100 * dividend / divisor
         res.iloc[0] = 0.0
         self[meta.name] = res
 
     def ker(self, column, window):
         col = self[column]
-        col_window_s = self._shift(col, -window)
+        col_window_s = self.s_shift(col, -window)
         window_diff = (col - col_window_s).abs()
         diff = self._col_diff(column).abs()
         volatility = self.mov_sum(diff, window)
         ret = window_diff / volatility
         ret.iloc[0] = 0
         return ret
```

