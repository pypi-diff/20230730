# Comparing `tmp/gtempco2-0.0.7.tar.gz` & `tmp/gtempco2-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gtempco2-0.0.7.tar", last modified: Sun Jul 30 07:40:13 2023, max compression
+gzip compressed data, was "gtempco2-0.0.8.tar", last modified: Sun Jul 30 21:10:50 2023, max compression
```

## Comparing `gtempco2-0.0.7.tar` & `gtempco2-0.0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-07-30 07:40:13.303705 gtempco2-0.0.7/
--rw-r--r--   0 yt        (1000) yt        (1000)     1780 2023-07-30 07:40:13.302281 gtempco2-0.0.7/PKG-INFO
--rw-r--r--   0 yt        (1000) yt        (1000)     1249 2023-06-12 04:59:29.000000 gtempco2-0.0.7/README.md
--rw-r--r--   0 yt        (1000) yt        (1000)       38 2023-07-30 07:40:13.303705 gtempco2-0.0.7/setup.cfg
--rw-r--r--   0 yt        (1000) yt        (1000)      951 2023-07-30 07:39:03.000000 gtempco2-0.0.7/setup.py
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-07-30 07:40:13.295396 gtempco2-0.0.7/src/
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-07-30 07:40:13.302281 gtempco2-0.0.7/src/gtempco2.egg-info/
--rw-r--r--   0 yt        (1000) yt        (1000)     1780 2023-07-30 07:40:12.000000 gtempco2-0.0.7/src/gtempco2.egg-info/PKG-INFO
--rw-r--r--   0 yt        (1000) yt        (1000)      217 2023-07-30 07:40:12.000000 gtempco2-0.0.7/src/gtempco2.egg-info/SOURCES.txt
--rw-r--r--   0 yt        (1000) yt        (1000)        1 2023-07-30 07:40:12.000000 gtempco2-0.0.7/src/gtempco2.egg-info/dependency_links.txt
--rw-r--r--   0 yt        (1000) yt        (1000)       44 2023-07-30 07:40:12.000000 gtempco2-0.0.7/src/gtempco2.egg-info/entry_points.txt
--rw-r--r--   0 yt        (1000) yt        (1000)        9 2023-07-30 07:40:12.000000 gtempco2-0.0.7/src/gtempco2.egg-info/top_level.txt
--rw-r--r--   0 yt        (1000) yt        (1000)     3240 2023-07-30 07:36:46.000000 gtempco2-0.0.7/src/gtempco2.py
+drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-07-30 21:10:50.674186 gtempco2-0.0.8/
+-rw-r--r--   0 yt        (1000) yt        (1000)     1780 2023-07-30 21:10:50.672271 gtempco2-0.0.8/PKG-INFO
+-rw-r--r--   0 yt        (1000) yt        (1000)     1249 2023-06-12 04:59:29.000000 gtempco2-0.0.8/README.md
+-rw-r--r--   0 yt        (1000) yt        (1000)       38 2023-07-30 21:10:50.674186 gtempco2-0.0.8/setup.cfg
+-rw-r--r--   0 yt        (1000) yt        (1000)      951 2023-07-30 21:09:37.000000 gtempco2-0.0.8/setup.py
+drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-07-30 21:10:50.666629 gtempco2-0.0.8/src/
+drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-07-30 21:10:50.671274 gtempco2-0.0.8/src/gtempco2.egg-info/
+-rw-r--r--   0 yt        (1000) yt        (1000)     1780 2023-07-30 21:10:50.000000 gtempco2-0.0.8/src/gtempco2.egg-info/PKG-INFO
+-rw-r--r--   0 yt        (1000) yt        (1000)      217 2023-07-30 21:10:50.000000 gtempco2-0.0.8/src/gtempco2.egg-info/SOURCES.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)        1 2023-07-30 21:10:50.000000 gtempco2-0.0.8/src/gtempco2.egg-info/dependency_links.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)       44 2023-07-30 21:10:50.000000 gtempco2-0.0.8/src/gtempco2.egg-info/entry_points.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)        9 2023-07-30 21:10:50.000000 gtempco2-0.0.8/src/gtempco2.egg-info/top_level.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)     3117 2023-07-30 21:08:29.000000 gtempco2-0.0.8/src/gtempco2.py
```

### Comparing `gtempco2-0.0.7/PKG-INFO` & `gtempco2-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gtempco2
-Version: 0.0.7
+Version: 0.0.8
 Summary: A package for displaying global temperature and co2
 Home-page: https://github.com/ytakefuji/gtempco2
 Author: yoshiyasu takefuji
 Author-email: takefuji@keio.jp
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ytakefuji/gtempco2
 Platform: UNKNOWN
```

### Comparing `gtempco2-0.0.7/README.md` & `gtempco2-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `gtempco2-0.0.7/setup.py` & `gtempco2-0.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="gtempco2",
-    version="0.0.7",
+    version="0.0.8",
     author="yoshiyasu takefuji",
     author_email="takefuji@keio.jp",
     description="A package for displaying global temperature and co2",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ytakefuji/gtempco2",
     project_urls={
```

### Comparing `gtempco2-0.0.7/src/gtempco2.egg-info/PKG-INFO` & `gtempco2-0.0.8/src/gtempco2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gtempco2
-Version: 0.0.7
+Version: 0.0.8
 Summary: A package for displaying global temperature and co2
 Home-page: https://github.com/ytakefuji/gtempco2
 Author: yoshiyasu takefuji
 Author-email: takefuji@keio.jp
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ytakefuji/gtempco2
 Platform: UNKNOWN
```

### Comparing `gtempco2-0.0.7/src/gtempco2.py` & `gtempco2-0.0.8/src/gtempco2.py`

 * *Files 8% similar despite different names*

```diff
@@ -61,21 +61,20 @@
  ax2.plot(noaa['date'].values, noaa['change'].values, color='black', linestyle='dotted')
  ax2.set_ylabel('Temperature Anomaly (C)', color='black')
  ax2.tick_params('y', colors='black')
  
  # Add regression lines
  x = np.arange(len(co2))
  slope, intercept, r_value, p_value, std_err = stats.linregress(x, co2['average'])
- ax1.plot(co2['date'].values, intercept + slope * x, 'b', label=f'CO2: y={slope:.3f}x+{intercept:.3f}, R^2={r_value**2:.3f}')
+ ax1.plot(co2['date'].values, intercept + slope * x, 'b', label=f'CO2: y={slope:.3f}x+{intercept:.3f}, R^2={r_value**2:.3f},p-value={p_value:.5f}')
  ax1.legend(loc='upper left')
  
  x = np.arange(len(noaa))
  slope, intercept, r_value, p_value, std_err = stats.linregress(x, noaa['change'])
- ax2.plot(noaa['date'].values, intercept + slope * x, 'r', label=f'T-Anomaly: y={slope:.3f}x+{intercept:.3f},R^2={r_value**2:.3f},p-value={p_value:.3f}')
-# ax2.plot(noaa['date'].values, intercept + slope * x, 'r', label=f'Temperature Anomaly: y={slope:.3f}x+{intercept:.3f}, R^2={r_value**2:.3f}')
+ ax2.plot(noaa['date'].values, intercept + slope * x, 'r', label=f'T-Anomaly: y={slope:.3f}x+{intercept:.3f},R^2={r_value**2:.3f},p-value={p_value:.5f}')
  ax2.legend(loc='lower right')
  
  ax1.xaxis.set_major_locator(MaxNLocator(7))
  ax1.set_xticklabels(ax1.get_xticklabels(), rotation=90)
  fig.tight_layout()
  plt.savefig(start+'_'+end+'.png',dpi=300,bbox_inches='tight')
  plt.show()
```

