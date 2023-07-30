# Comparing `tmp/BukeColabProject-0.4.6.tar.gz` & `tmp/BukeColabProject-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\BukeColabProject-0.4.6.tar", last modified: Mon Jul 24 13:11:46 2023, max compression
+gzip compressed data, was "dist\BukeColabProject-1.0.0.tar", last modified: Sun Jul 30 08:54:46 2023, max compression
```

## Comparing `BukeColabProject-0.4.6.tar` & `BukeColabProject-1.0.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 13:11:46.000000 BukeColabProject-0.4.6/
-drwxrwxrwx   0        0        0        0 2023-07-24 13:11:46.000000 BukeColabProject-0.4.6/BukeColabProject/
--rw-rw-rw-   0        0        0     8961 2023-04-02 08:47:11.000000 BukeColabProject-0.4.6/BukeColabProject/Buke_S002_buy_list.py
--rw-rw-rw-   0        0        0    17411 2023-04-02 08:39:38.000000 BukeColabProject-0.4.6/BukeColabProject/Buke_S002_sell_list.py
--rw-rw-rw-   0        0        0     8974 2023-07-24 13:11:32.000000 BukeColabProject-0.4.6/BukeColabProject/Buke_S004_buy_list.py
--rw-rw-rw-   0        0        0    17297 2023-07-24 12:43:56.000000 BukeColabProject-0.4.6/BukeColabProject/Buke_S004_sell_list.py
--rw-rw-rw-   0        0        0    21693 2023-03-19 08:57:24.000000 BukeColabProject-0.4.6/BukeColabProject/function.py
--rw-rw-rw-   0        0        0     8943 2023-03-19 08:20:07.000000 BukeColabProject-0.4.6/BukeColabProject/generate_day_price.py
--rw-rw-rw-   0        0        0     4165 2023-03-19 08:06:52.000000 BukeColabProject-0.4.6/BukeColabProject/generate_index_day_price.py
--rw-rw-rw-   0        0        0     2307 2023-03-19 08:27:27.000000 BukeColabProject-0.4.6/BukeColabProject/generate_stock_list.py
--rw-rw-rw-   0        0        0     2481 2023-03-19 07:22:24.000000 BukeColabProject-0.4.6/BukeColabProject/generate_trading_days.py
--rw-rw-rw-   0        0        0    63703 2023-03-19 08:57:24.000000 BukeColabProject-0.4.6/BukeColabProject/indicator.py
--rw-rw-rw-   0        0        0      561 2021-08-12 12:11:28.000000 BukeColabProject-0.4.6/BukeColabProject/parameter.py
--rw-rw-rw-   0        0        0     4116 2023-04-23 08:45:14.000000 BukeColabProject-0.4.6/BukeColabProject/tools.py
--rw-rw-rw-   0        0        0        0 2023-03-19 07:24:19.000000 BukeColabProject-0.4.6/BukeColabProject/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 13:11:46.000000 BukeColabProject-0.4.6/BukeColabProject.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-24 13:11:46.000000 BukeColabProject-0.4.6/BukeColabProject.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      472 2023-07-24 13:11:46.000000 BukeColabProject-0.4.6/BukeColabProject.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      646 2023-07-24 13:11:46.000000 BukeColabProject-0.4.6/BukeColabProject.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       17 2023-07-24 13:11:46.000000 BukeColabProject-0.4.6/BukeColabProject.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      472 2023-07-24 13:11:46.000000 BukeColabProject-0.4.6/PKG-INFO
--rw-rw-rw-   0        0        0        9 2023-03-19 07:23:35.000000 BukeColabProject-0.4.6/README.md
--rw-rw-rw-   0        0        0       42 2023-07-24 13:11:46.000000 BukeColabProject-0.4.6/setup.cfg
--rw-rw-rw-   0        0        0      700 2023-07-24 13:11:32.000000 BukeColabProject-0.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 08:54:46.000000 BukeColabProject-1.0.0/
+drwxrwxrwx   0        0        0        0 2023-07-30 08:54:46.000000 BukeColabProject-1.0.0/BukeColabProject/
+-rw-rw-rw-   0        0        0     8961 2023-04-02 08:47:11.000000 BukeColabProject-1.0.0/BukeColabProject/Buke_S002_buy_list.py
+-rw-rw-rw-   0        0        0    17411 2023-04-02 08:39:38.000000 BukeColabProject-1.0.0/BukeColabProject/Buke_S002_sell_list.py
+-rw-rw-rw-   0        0        0     8980 2023-07-24 13:20:08.000000 BukeColabProject-1.0.0/BukeColabProject/Buke_S004_buy_list.py
+-rw-rw-rw-   0        0        0    17297 2023-07-24 12:43:56.000000 BukeColabProject-1.0.0/BukeColabProject/Buke_S004_sell_list.py
+-rw-rw-rw-   0        0        0    21693 2023-03-19 08:57:24.000000 BukeColabProject-1.0.0/BukeColabProject/function.py
+-rw-rw-rw-   0        0        0     8943 2023-03-19 08:20:07.000000 BukeColabProject-1.0.0/BukeColabProject/generate_day_price.py
+-rw-rw-rw-   0        0        0     4165 2023-03-19 08:06:52.000000 BukeColabProject-1.0.0/BukeColabProject/generate_index_day_price.py
+-rw-rw-rw-   0        0        0     2307 2023-03-19 08:27:27.000000 BukeColabProject-1.0.0/BukeColabProject/generate_stock_list.py
+-rw-rw-rw-   0        0        0     2481 2023-03-19 07:22:24.000000 BukeColabProject-1.0.0/BukeColabProject/generate_trading_days.py
+-rw-rw-rw-   0        0        0    63703 2023-03-19 08:57:24.000000 BukeColabProject-1.0.0/BukeColabProject/indicator.py
+-rw-rw-rw-   0        0        0      561 2021-08-12 12:11:28.000000 BukeColabProject-1.0.0/BukeColabProject/parameter.py
+-rw-rw-rw-   0        0        0     4116 2023-04-23 08:45:14.000000 BukeColabProject-1.0.0/BukeColabProject/tools.py
+-rw-rw-rw-   0        0        0        0 2023-03-19 07:24:19.000000 BukeColabProject-1.0.0/BukeColabProject/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-30 08:54:46.000000 BukeColabProject-1.0.0/BukeColabProject.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-30 08:54:45.000000 BukeColabProject-1.0.0/BukeColabProject.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      472 2023-07-30 08:54:45.000000 BukeColabProject-1.0.0/BukeColabProject.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      646 2023-07-30 08:54:45.000000 BukeColabProject-1.0.0/BukeColabProject.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       17 2023-07-30 08:54:45.000000 BukeColabProject-1.0.0/BukeColabProject.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      472 2023-07-30 08:54:46.000000 BukeColabProject-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0        9 2023-03-19 07:23:35.000000 BukeColabProject-1.0.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-30 08:54:46.000000 BukeColabProject-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      700 2023-07-24 13:44:22.000000 BukeColabProject-1.0.0/setup.py
```

### Comparing `BukeColabProject-0.4.6/BukeColabProject/Buke_S002_buy_list.py` & `BukeColabProject-1.0.0/BukeColabProject/Buke_S002_buy_list.py`

 * *Files identical despite different names*

### Comparing `BukeColabProject-0.4.6/BukeColabProject/Buke_S002_sell_list.py` & `BukeColabProject-1.0.0/BukeColabProject/Buke_S002_sell_list.py`

 * *Files identical despite different names*

### Comparing `BukeColabProject-0.4.6/BukeColabProject/Buke_S004_buy_list.py` & `BukeColabProject-1.0.0/BukeColabProject/Buke_S004_buy_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,16 @@
         group['순거래대금_이평선_5'] = sma(group['순거래대금'], 5)
 
         group['종가_이평선_20'] = sma(group['종가'], 20)
 
         group['스토캐스틱_fast'] = stochastic_fast_k(group['고가'], group['저가'], group['종가'], 20)
         group['스토캐스틱_slow'] = stochastic_fast_d(group['고가'], group['저가'], group['종가'], 20, 5, MovingAverage.sma)
 
-    group_list.append(group)
+        group_list.append(group)
+
     day_price = pd.concat(group_list, axis=0)
     day_price = day_price.reset_index(drop=True)
 
     group_list = []
     grouped = day_price.groupby('날짜')
     for key, group in grouped:
         group = group.reset_index(drop=True)
```

### Comparing `BukeColabProject-0.4.6/BukeColabProject/Buke_S004_sell_list.py` & `BukeColabProject-1.0.0/BukeColabProject/Buke_S004_sell_list.py`

 * *Files identical despite different names*

### Comparing `BukeColabProject-0.4.6/BukeColabProject/function.py` & `BukeColabProject-1.0.0/BukeColabProject/function.py`

 * *Files identical despite different names*

### Comparing `BukeColabProject-0.4.6/BukeColabProject/generate_day_price.py` & `BukeColabProject-1.0.0/BukeColabProject/generate_day_price.py`

 * *Files identical despite different names*

### Comparing `BukeColabProject-0.4.6/BukeColabProject/generate_index_day_price.py` & `BukeColabProject-1.0.0/BukeColabProject/generate_index_day_price.py`

 * *Files identical despite different names*

### Comparing `BukeColabProject-0.4.6/BukeColabProject/generate_stock_list.py` & `BukeColabProject-1.0.0/BukeColabProject/generate_stock_list.py`

 * *Files identical despite different names*

### Comparing `BukeColabProject-0.4.6/BukeColabProject/generate_trading_days.py` & `BukeColabProject-1.0.0/BukeColabProject/generate_trading_days.py`

 * *Files identical despite different names*

### Comparing `BukeColabProject-0.4.6/BukeColabProject/indicator.py` & `BukeColabProject-1.0.0/BukeColabProject/indicator.py`

 * *Files identical despite different names*

### Comparing `BukeColabProject-0.4.6/BukeColabProject/parameter.py` & `BukeColabProject-1.0.0/BukeColabProject/parameter.py`

 * *Files identical despite different names*

### Comparing `BukeColabProject-0.4.6/BukeColabProject/tools.py` & `BukeColabProject-1.0.0/BukeColabProject/tools.py`

 * *Files identical despite different names*

### Comparing `BukeColabProject-0.4.6/BukeColabProject.egg-info/SOURCES.txt` & `BukeColabProject-1.0.0/BukeColabProject.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `BukeColabProject-0.4.6/setup.py` & `BukeColabProject-1.0.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="BukeColabProject", # Replace with your own username
-    version="0.4.6",
+    version="1.0.0",
     author="Example Author",
     author_email="yesben214@gamil.com",
     description="A small example package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pypa/sampleproject",
     packages=setuptools.find_packages(),
```

