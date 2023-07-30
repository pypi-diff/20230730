# Comparing `tmp/crnpy-0.5.0.tar.gz` & `tmp/crnpy-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crnpy-0.5.0.tar", last modified: Sat Jul  8 00:36:07 2023, max compression
+gzip compressed data, was "crnpy-0.5.1.tar", last modified: Sun Jul 30 03:00:44 2023, max compression
```

## Comparing `crnpy-0.5.0.tar` & `crnpy-0.5.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:36:07.013567 crnpy-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-08 00:35:54.000000 crnpy-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-07-08 00:36:07.013567 crnpy-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-07-08 00:35:54.000000 crnpy-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 00:36:07.013567 crnpy-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-08 00:35:54.000000 crnpy-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:36:07.009567 crnpy-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:36:07.013567 crnpy-0.5.0/src/crnpy/
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-08 00:35:54.000000 crnpy-0.5.0/src/crnpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    58403 2023-07-08 00:35:54.000000 crnpy-0.5.0/src/crnpy/crnpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9159 2023-07-08 00:35:54.000000 crnpy-0.5.0/src/crnpy/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:36:07.013567 crnpy-0.5.0/src/crnpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-07-08 00:36:06.000000 crnpy-0.5.0/src/crnpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-08 00:36:07.000000 crnpy-0.5.0/src/crnpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 00:36:06.000000 crnpy-0.5.0/src/crnpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-08 00:36:06.000000 crnpy-0.5.0/src/crnpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:00:44.367024 crnpy-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-30 03:00:33.000000 crnpy-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-07-30 03:00:44.367024 crnpy-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-07-30 03:00:33.000000 crnpy-0.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 03:00:44.367024 crnpy-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-30 03:00:33.000000 crnpy-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:00:44.367024 crnpy-0.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:00:44.367024 crnpy-0.5.1/src/crnpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-30 03:00:33.000000 crnpy-0.5.1/src/crnpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52969 2023-07-30 03:00:33.000000 crnpy-0.5.1/src/crnpy/crnpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9159 2023-07-30 03:00:33.000000 crnpy-0.5.1/src/crnpy/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:00:44.367024 crnpy-0.5.1/src/crnpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-07-30 03:00:44.000000 crnpy-0.5.1/src/crnpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-30 03:00:44.000000 crnpy-0.5.1/src/crnpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 03:00:44.000000 crnpy-0.5.1/src/crnpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-30 03:00:44.000000 crnpy-0.5.1/src/crnpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-30 03:00:44.000000 crnpy-0.5.1/src/crnpy.egg-info/top_level.txt
```

### Comparing `crnpy-0.5.0/setup.py` & `crnpy-0.5.1/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 # contents of setup.py
 import setuptools
 
 setuptools.setup(
     name="crnpy",
-    version="0.5.0",
+    version="0.5.1",
     packages=['crnpy'],
     package_dir = {"": "src"},
     description="A Python package for the estimation and processing of soil moisture data from cosmic-ray neutron counts.",
     include_package_data=True,
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/soilwater/crnpy",
     author="Joaquin Peraza, Andres Patrignani",
     author_email="jperaza@ksu.edu, andrespatrignani@ksu.edu",
-    license="MIT"
+    license="MIT",
+    license_files=["LICENSE"],
+    install_requires=[
+        "numpy",
+        "pandas",
+        "scipy",
+        "requests"
+    ],
 )
```

### Comparing `crnpy-0.5.0/src/crnpy/__init__.py` & `crnpy-0.5.1/src/crnpy/__init__.py`

 * *Files identical despite different names*

### Comparing `crnpy-0.5.0/src/crnpy/crnpy.py` & `crnpy-0.5.1/src/crnpy/crnpy.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,349 +4,214 @@
 
  Created by Joaquin Peraza and Andres Patrignani.
 """
 
 # Import modules
 import sys
 import warnings
+import numbers
 import numpy as np
 import pandas as pd
 import requests
-import io, datetime, os
+import io
+
+
 from scipy.signal import savgol_filter
 from scipy.interpolate import griddata
+from scipy.special import erfcinv
 import crnpy.data as data
 
 # Define python version
 python_version = (3, 7)  # tuple of (major, minor) version requirement
 python_version_str = str(python_version[0]) + "." + str(python_version[1])
 
 # produce an error message if the python version is less than required
 if sys.version_info < python_version:
     msg = "Module only runs on python version >= %s" % python_version_str
     raise Exception(msg)
 
 
-def fill_missing_timestamps(df, col='timestamp', format='%Y-%m-%d %H:%M:%S', freq='H', round_time=True):
-    """Helper function to change the format and round timestamps.
+def remove_incomplete_intervals(df, timestamp_col, integration_time, remove_first=False):
+    """Function that removes rows with incomplete integration intervals.
+    
+    Args:
+        df (pandas.DataFrame): Pandas Dataframe with data from stationary or roving CRNP devices.
+        timestamp_col (str): Name of the column with timestamps in datetime format.
+        integration_time (int): Duration of the neutron counting interval in seconds. Typical values are 60 seconds and 3600 seconds.
+        remove_first (bool, optional): Remove first row. Default is False.
+        
+    Returns:
+        (pandas.DataFrame): 
+    """
+    
+    # Check format of timestamp column
+    if df[timestamp_col].dtype != 'datetime64[ns]':
+        raise TypeError('timestamp_col must be datetime64. Use `pd.to_datetime()` to fix this issue.')
+
+    # Check if differences in timestamps are below or above the provided integration time
+    idx_delta = df[timestamp_col].diff().dt.total_seconds() != integration_time
+    
+    if remove_first:
+        idx_delta[0] = True
+        
+    # Select rows that meet the specified integration time
+    df = df[~idx_delta]
+    df.reset_index(drop=True, inplace=True)
+
+    # Notify user about the number of rows that have been removed
+    print(f"Removed a total of {sum(idx_delta)} rows.")
+    
+    return df
+
+
+def fill_missing_timestamps(df, timestamp_col='timestamp', freq='H', round_timestamp=True, verbose=False):
+    """Helper function to fill rows with missing timestamps in datetime record. Rows are filled with NaN values.
 
      Args:
-         df (pandas.DataFrame): DataFrame with timestamp in the index.
-         col (str, optional): Column with the timestamp. Default is 'timestamp'.
-         format (str, optional): Format of the timestamp. Default is '%Y-%m-%d %H:%M:%S'.
-         freq (str, optional): Rounding interval. 'H' for hourly, 'M' for minute, or None. Default is 'H'.
-         round_time (bool, optional): Whether to round timestamps to the nearest frequency. Default is True.
+         df (pandas.DataFrame): Pandas DataFrame.
+         timestamp_col (str, optional): Column with the timestamp. Must be in datetime format. Default column name is 'timestamp'.
+         freq (str, optional): Timestamp frequency. 'H' for hourly, 'M' for minute, or None. Can also use '3H' for a 3 hour frequency. Default is 'H'.
+         round_timestamp (bool, optional): Whether to round timestamps to the nearest frequency. Default is True.
+         verbose (bool, optional): Prints the missing timestamps added to the DatFrame.
 
      Returns:
-         (pandas.DataFrame): DataFrame with formatted timestamps and rounded time.
+         (pandas.DataFrame): DataFrame with filled missing timestamps.
 
-     Examples:
-            >>> from crnpy import crnpy
-            >>> import pandas as pd
-            >>> df = pd.DataFrame({'timestamp':['2020-01-01 00:00:00','2020-01-01 00:30:00','2020-01-01 01:00:00']})
-            >>> df = crnpy.format_dates_df(df, col='timestamp', format='%Y-%m-%d %H:%M:%S', freq='H', round_time=True)
-            >>> df
-                            timestamp
-            0   2020-01-01 00:00:00
-            1   2020-01-01 00:00:00
-            2   2020-01-01 01:00:00
      """
 
-    # Change format of timestamp if needed
-    if df[col].dtype != 'datetime64[ns]':
-        df[col] = pd.to_datetime(df[col], format=format)
-
-    # Round timestamps to nearest frequency
-    if round_time:
-        df[col] = df[col].dt.round(freq)
+    # Check format of timestamp column
+    if df[timestamp_col].dtype != 'datetime64[ns]':
+        raise TypeError('timestamp_col must be datetime64. Use `pd.to_datetime()` to fix this issue.')
+
+    # Round timestamps to nearest frequency. This steps must preced the filling of rows.
+    if round_timestamp:
+        df[timestamp_col] = df[timestamp_col].dt.round(freq)
 
     # Fill in rows with missing timestamps
-    start_date = df[col].iloc[0]
-    end_date = df[col].iloc[-1]
+    start_date = df[timestamp_col].iloc[0]
+    end_date = df[timestamp_col].iloc[-1]
     date_range = pd.date_range(start_date, end_date, freq=freq)
+    counter = 0
     for date in date_range:
-        if date not in df[col].values:
-            print('Adding missing date:',date)
-            new_line = pd.DataFrame({col:date}, index=[-1]) # By default fills columns with np.nan
-            source = pd.concat([df,new_line])
+        if date not in df[timestamp_col].values:
+            if verbose:
+                print('Adding missing date:',date)
+            new_line = pd.DataFrame({timestamp_col:date}, index=[-1]) # By default fills columns with np.nan
+            df = pd.concat([df,new_line])
+            counter += 1
 
-    df.sort_values(by=col, inplace=True)
+    df.sort_values(by=timestamp_col, inplace=True)
     df.reset_index(drop=True, inplace=True)
-    df.set_index(col, inplace=True)
+    
+    # Notify user about the number of rows that have been removed
+    print(f"Added a total of {counter} missing timestamps.")
+    
     return df
 
-def get_integration_time(counts=None, timestamp_col=None):
-    """Approximate counting time.
-    The function will calculate the approximate counting time for each observation by taking the difference between
-    consecutive timestamps. If counts has a DateTimeIndex, timestamp_col is not needed.
-
-    Args:
-        counts (pandas.DataFrame): DataFrame with neutron counts, might have DateTimeIndex.
-        timestamp_col (pandas.Series): Series with timestamps. If counts has a DateTimeIndex, timestamp_col is not needed.
-
-    Returns:
-        (pandas.Series): Series with the approximate counting time for each observation.
-
-    Examples:
-        Using `get_integration_time` in a console environment:
-
-        >>> df = pd.DataFrame(...)
-        >>> get_integration_time(timestamp_col=df['timestamp'])
-        0   3600.0
-        1   3600.0
-        2   3600.0
-    """
-    if timestamp_col is not None:
-        if not isinstance(timestamp_col, pd.Series):
-            raise TypeError('timestamp_col must be a pandas Series.')
-        if timestamp_col.dtype != 'datetime64[ns]':
-            raise TypeError('timestamp_col must be a pandas Series with datetime64[ns] dtype.')
-
-        integration_time = timestamp_col.diff().dt.total_seconds()
-        return integration_time
-
-    if counts is not None:
-        if not isinstance(counts, pd.DataFrame):
-            raise TypeError('counts must be a pandas DataFrame.')
-
-        if not counts.index.dtype == 'datetime64[ns]':
-            raise TypeError('counts must have a DateTimeIndex.')
-
-        integration_time = counts.index.to_series().diff().dt.total_seconds()
-        return integration_time
-
-    raise TypeError('Either counts or timestamp_col must be provided.')
-
-def fill_counts(counts, actual_integration_time=None, timestamp_col=None, expected_time=False, threshold=0.25, limit=3):
-    """Fill missing neutron counts. Observation periods shorter than threshold are discarded (replaced with NaN).
-
-    Args:
-        counts (pandas.DataFrame): DataFrame with neutron counts, might have DateTimeIndex.
-        actual_integration_time (pandas.Series or pandas.DataFrame): Counting time in seconds. If a DataFrame is provided, it must have the same number of columns as `counts`.
-        timestamp_col (pandas.Series): Series with timestamps. If counts has a DateTimeIndex, timestamp_col is not needed.
-        expected_time (int): Expected integration time in seconds. If not provided, it is calculated as the median of the counting times.
-        threshold (float): Minimum fraction of the neutron integration time. Default is 0.25.
-
-    Returns:
-        (pandas.DataFrame): DataFrame with linearly interpolated neutron counts.
-
-    Examples:
-        Using `fill_counts` in a console environment:
-
-        >>> counts = pd.DataFrame({'counts':[100,105,98,102], count_time:[3600,200,3600,3600]})
-        >>> fill_counts(counts, actual_integration_time=counts['actual_integration_time'], expected_time=3600, threshold=0.25)
-        0   100.0
-        1   NaN
-        2   98.0
-        3   102.0
-    """
-
-    counts=counts.copy()
-
-    if type(counts.index) == pd.core.indexes.datetimes.DatetimeIndex and isinstance(actual_integration_time, type(None)):
-        print("No count time columns provided. Using timestamp index to compute count time.")
-        actual_integration_time = get_integration_time(timestamp_col=counts.index.to_series())
-
-    elif not isinstance(timestamp_col, type(None)) and isinstance(actual_integration_time, type(None)):
-        if timestamp_col.dtype != 'datetime64[ns]':
-            if len(timestamp_col) != len(counts):
-                raise ValueError('Timestamp column length does not match number of readings.')
-            print("No count time columns provided. Using timestamp column to compute count time.")
-            actual_integration_time = get_integration_time(timestamp_col=timestamp_col)
-        else:
-            raise TypeError('Timestamp column must be a pandas Series with datetime64[ns] dtype.')
-
-    if type(counts.index) != pd.core.indexes.datetimes.DatetimeIndex and isinstance(actual_integration_time, type(None)) and isinstance(timestamp_col, type(None)):
-        raise ValueError('Count_times must be provided, or timestamp_col must be provided, or counts must have a DatetimeIndex.')
 
-    if len(counts) != len(actual_integration_time):
-        raise ValueError('Count times length does not match number of readings.')
-
-    if expected_time is False:
-        expected_time = actual_integration_time.median()
-        print('Using median count time as expected count time:', expected_time)
-
-    # Replace values below threshold with NaN
-    time_threshold = round(expected_time * threshold)
-
-    if type(actual_integration_time) == pd.core.frame.DataFrame:
-        if len(actual_integration_time.columns) == 1:
-            idx_nan = actual_integration_time[actual_integration_time < time_threshold].index
-            counts.loc[idx_nan] = np.nan
-        else:
-            for i in range(len(actual_integration_time.columns)):
-                idx_nan = actual_integration_time[actual_integration_time.iloc[:, i] < time_threshold].index
-                counts.iloc[:,i].loc[idx_nan] = np.nan
-    elif type(actual_integration_time) == pd.core.series.Series:
-        idx_nan = actual_integration_time[actual_integration_time < time_threshold].index
-        counts.loc[idx_nan] = np.nan
-    elif type(actual_integration_time) == np.ndarray:
-        idx_nan = np.where(actual_integration_time < time_threshold)
-        counts.loc[idx_nan] = np.nan
-
-    # Fill missing values with linear interpolation and round to nearest integer
-    counts = counts.interpolate(method='linear', limit=limit, limit_direction='both').round()
-    return counts
-
-def adjust_temporal_counts(counts, nominal_integration_time=None, actual_integration_time=None, timestamp_col=None):
-    """Adjust neutron counts for the desired integration time.
-
-    Args:
-        counts (pandas.DataFrame): Dataframe containing only the columns with neutron counts.
-        nominal_integration_time (int): Nominal intgration time in seconds.
-        actual_integration_time (pandas.Series or pandas.DataFrame): Actual integration time of each measurement in seconds. If a DataFrame is provided, it must have the same number of columns as counts.
-        timestamp_col (pandas.Series): Timestamp column, used to calculate integration time if actual_integration_time is not provided, it must have the same number of rows as counts.
-
-    Returns:
-        (pandas.DataFrame): Neutron counts adjusted for the desired integration time.
-
-    """
-
-    if actual_integration_time is None and type(counts.index) == pd.core.indexes.datetimes.DatetimeIndex:
-        print("No count_times columns provided. Using timestamp index to compute count time.")
-        actual_integration_time = counts.index.to_series().diff().dt.total_seconds()
-
-    elif actual_integration_time is None and not isinstance(timestamp_col, type(None)):
-        if len(timestamp_col) != len(counts):
-            raise ValueError('Timestamp column length does not match number of readings.')
-        print("No count_times columns provided. Using timestamp column to compute count time.")
-        if timestamp_col.dtype != 'datetime64[ns]':
-            raise TypeError('Timestamp column must be a pandas Series with datetime64[ns] dtype.')
-        actual_integration_time = get_integration_time(timestamp_col=timestamp_col)
-
-
-    if isinstance(actual_integration_time, type(None)):
-        raise ValueError('Actual integration time must be provided, or `timestamp_col` must be provided, or counts must have a DatetimeIndex.')
-
-    if len(counts) != len(actual_integration_time):
-        raise ValueError('Count times length does not match number of readings.')
-
-    #Normalize counts rounded to integer
-    if type(actual_integration_time) == pd.core.series.Series or len(actual_integration_time.columns) == 1:
-        adjusted_counts = counts.div(actual_integration_time, axis=0).mul(nominal_integration_time).round()
-        return adjusted_counts
-    else:
-        adjusted_counts = counts.copy()
-        count_times = actual_integration_time.copy()
-        for i in range(len(count_times.columns)):
-            adjusted_counts[adjusted_counts.columns[i]] = adjusted_counts.iloc[:,i].div(count_times.iloc[:,i], axis=0).mul(nominal_integration_time).round()
-        return adjusted_counts
-
-
-def compute_total_raw_counts(counts, nan_strategy=None, timestamp_col=None):
+def total_raw_counts(counts, nan_strategy=None, timestamp_col=None):
     """Compute the sum of uncorrected neutron counts for all detectors.
 
     Args:
         counts (pandas.DataFrame): Dataframe containing only the columns with neutron counts.
         nan_strategy (str): Strategy to use for NaN values. Options are 'interpolate', 'average', or None. Default is None.
 
     Returns:
         (pandas.DataFrame): Dataframe with the sum of uncorrected neutron counts for all detectors.
     """
 
-    counts=counts.copy()
-
-    if counts.isnull().values.any():
-        if nan_strategy is None:
-            raise ValueError('NaN values found. Please fill missing values or provide a strategy. See documentation for more information.')
-        elif nan_strategy == 'interpolate':
-            print('NaN values found. Interpolating missing values using fill_counts().')
-            if not isinstance(timestamp_col, type(None)):
-                if type(timestamp_col) != pd.core.series.Series:
-                    if timestamp_col.dtype != 'datetime64[ns]':
-                        raise TypeError('Timestamp column must be a pandas Series with datetime64[ns] dtype.')
-                counts = fill_counts(counts, timestamp_col)
-            elif type(counts.index) != pd.core.indexes.datetimes.DatetimeIndex:
-                raise ValueError('`timestamp_col` must be provided if `counts` does not have a DatetimeIndex.')
-            counts = fill_counts(counts)
-        elif nan_strategy == 'average':
-            if len(counts.columns) == 1:
-                raise ValueError('Only one detector found. Cannot use average strategy.')
-            print('NaN values found. Replacing missing values with average of other detectors before summing.')
-            counts = counts.apply(lambda x: x.fillna(counts.mean(axis=1)),axis=0)
-        else:
-            raise ValueError('Invalid strategy.')
+    if counts.shape[0] > 1:
+        counts = counts.apply(lambda x: x.fillna(counts.mean(axis=1)),axis=0)
 
-    #Compute sum of counts
+    # Compute sum of counts
     total_raw_counts = counts.sum(axis=1)
+    
     # Replace zeros with NaN
     total_raw_counts = total_raw_counts.replace(0, np.nan)
+    
     return total_raw_counts
 
 
-def drop_outliers(raw_counts, window=5, store_outliers=False, min_counts=None, max_counts=None):
-    """Computation of a moving modified Z-score based on the median absolute difference.
+def is_outlier(x, method, window=11, min_val=None, max_val=None):
+    """Function that tests whether values are outliers using a modified moving z-score based on the median absolute difference.
 
     Args:
-        raw_counts (pandas.DataFrame): Dataframe containing only the columns with neutron counts.
-        window (int): Window size for the moving median. Default is 11.
-        store_outliers (bool): If True, store the outliers in a new column. Default is False.
-        min_counts (int): Minimum number of counts for a reading to be considered valid. Default is None.
-        max_counts (int): Maximum number of counts for a reading to be considered valid. Default is None.
+        x (pandas.DataFrame): Variable containing only the columns with neutron counts.
+        method (str): Outlier detection method. One of: range, iqr, moviqr, zscore, movzscore, modified_zscore, and scaled_mad
+        window (int, optional): Window size for the moving central tendency. Default is 11.
+        min_val (int or float): Minimum value for a reading to be considered valid. Default is None.
+        max_val(int or float): Maximum value for a reading to be considered valid. Default is None.
 
     Returns:
-        (pandas.DataFrame): Dataframe without outliers.
-        or
-        (pandas.DataFrame, pandas.DataFrame): Dataframe without outliers and dataframe with outliers.
+        (pandas.DataFrame): Boolean indicating outliers.
 
     References:
         Iglewicz, B. and Hoaglin, D.C., 1993. How to detect and handle outliers (Vol. 16). Asq Press.
     """
+        
+    if not isinstance(x, pd.Series):
+        raise TypeError('x must of type pandas.Series')
+
+    # Separate this method to allow usage together with other methods below
+    if isinstance(min_val, numbers.Number) and isinstance(max_val, numbers.Number):
+        idx_range_outliers = (x < min_val) | (x > max_val)
+    else:
+        idx_range_outliers = np.full_like(x, False)
 
-    if min_counts is not None:
-        lower_count = np.sum(raw_counts < min_counts)
-        if lower_count > len(raw_counts) * 0.25:
-            print(f"WARNING: Discarded {lower_count} counts below {min_counts}. This is more than 25% of the total number of readings. Consider increasing the minimum counts threshold.")
-        else:
-            print(f"Discarded counts below {min_counts}: {lower_count}")
-        raw_counts = raw_counts[raw_counts >= min_counts]
-    if max_counts is not None:
-        upper_count = np.sum(raw_counts > max_counts)
-        print(f"Discarded counts above {max_counts}: {upper_count}")
-        raw_counts = raw_counts[raw_counts <= max_counts]
-
-    # Compute median absolute difference
-    median = raw_counts.rolling(window, center=True).median()
-    diff = np.abs(raw_counts - median)
-    mad = diff.rolling(window, center=True).median()
-
-    # Compute modified Z-score
-    modified_z_score = 0.6745 * diff / mad
-    outliers = raw_counts[modified_z_score > 3.5]
-    # Drop outliers
-    raw_counts = raw_counts[modified_z_score < 3.5]
-
-    if store_outliers:
-        return raw_counts, outliers
-    print(f"Discarded {len(outliers)} outliers using modified Z-score.")
-    return raw_counts
-
-
-def fill_missing_atm(cols_atm, limit=24):
-    """Fill missing values in atmospheric variables. Gap filling is performed using a
-    piecewise cubic Hermite interpolating polynomial (pchip method) that is restricted to intervals
-    of missing data with a limited number of values and surrounded by valid observations.
-    There is no interpolation at the end of the time series.
-
-    Args:
-        col_atm (pandas.Series or pandas.DataFrame): Atmospheric variables to fill.
-        limit (int): Maximum number of consecutive missing values to interpolate. Default is 24.
-
-    Returns:
-        (pandas.DataFrame): Atmospheric variables with filled missing values using a piecewise cubic Hermite polynomial.
+    # Apply other methods in addition to a range check
+    if method == 'iqr':
+        q1 = x.quantile(0.25)
+        q3 = x.quantile(0.75)
+        iqr = q3 - q1
+        high_fence = q3 + (1.5 * iqr)
+        low_fence = q1 - (1.5 * iqr)
+        idx_outliers = (x<low_fence ) | (x>high_fence )
+
+    elif method == 'moviqr':
+        q1 = x.rolling(window, center=True).quantile(0.25)
+        q3 = x.rolling(window, center=True).quantile(0.75)
+        iqr = q3 - q1
+        ub = q3 + (1.5 * iqr) # Upper boundary
+        lb = q1 - (1.5 * iqr) # Lower boundary
+        idx_outliers = (x < lb) | (x > ub)
+
+    elif method == 'zscore':
+        zscore = (x - x.mean())/x.std()
+        idx_outliers = (zscore < -3) | (zscore > 3)
+
+    elif method == 'movzscore':
+        movmean = x.rolling(window=window, center=True).mean()
+        movstd = x.rolling(window=window, center=True).std()
+        movzscore = (x - movmean)/movstd
+        idx_outliers = (movzscore < -3) | (movzscore > 3)
+
+    elif method == 'modified_zscore':
+        # Compute median absolute difference
+        movmedian = x.rolling(window, center=True).median()
+        abs_diff = np.abs(x - movmedian)
+        mad = abs_diff.rolling(window, center=True).median()
+
+        # Compute modified z-score
+        modified_z_score = 0.6745 * abs_diff / mad
+        idx_outliers = (modified_z_score < -3.5) | (modified_z_score > 3.5)
+
+    elif method == 'scaled_mad':
+        # Returns true for elements more than three scaled MAD from the median. 
+        c = -1 / (np.sqrt(2)*erfcinv(3/2))
+        median = np.nanmedian(x)
+        mad = c*np.nanmedian(np.abs(x - median))
+        idx_outliers = x > (median + 3*mad)
 
-    References:
-        https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.interpolate.html
-    """
+    else:
+        raise TypeError('Outlier detection method not found.')
 
-    # Fill missing values in atmospheric variables
-    return cols_atm.interpolate(method='pchip', limit=limit, limit_direction='both')
+    return idx_outliers | idx_range_outliers
 
 
-def pressure_correction(pressure, Pref, L):
+def correction_pressure(pressure, Pref, L):
     r"""Correction factor for atmospheric pressure.
 
     This function corrects neutron counts for atmospheric pressure using the method described in Andreasen et al. (2017).
     The correction is performed using the following equation:
 
     $$
     C_{corrected} = \frac{C_{raw}}{fp}
@@ -383,15 +248,15 @@
 
     # Compute pressure correction factor
     fp = np.exp((Pref - pressure) / L) # Zreda et al. 2017 Eq 5.
 
     return fp
 
 
-def humidity_correction(abs_humidity, Aref):
+def correction_humidity(abs_humidity, Aref):
     r"""Correction factor for absolute humidity.
 
     This function corrects neutron counts for absolute humidity using the method described in Rosolem et al. (2013) and Anderson et al. (2017). The correction is performed using the following equation:
 
     $$
     C_{corrected} = C_{raw} \cdot f_w
     $$
@@ -422,15 +287,15 @@
     References:
         M. Andreasen, K.H. Jensen, D. Desilets, T.E. Franz, M. Zreda, H.R. Bogena, and M.C. Looms. 2017. Status and perspectives on the cosmic-ray neutron method for soil moisture estimation and other environmental science applications. Vadose Zone J. 16(8). doi:10.2136/vzj2017.04.0086
     """
     A = abs_humidity
     fw = 1 + 0.0054*(A - Aref) # Zreda et al. 2017 Eq 6.
     return fw
 
-def incoming_flux_correction(incoming_neutrons, incoming_Ref=None):
+def correction_incoming_flux(incoming_neutrons, incoming_Ref=None):
     r"""Correction factor for incoming neutron flux.
 
     This function corrects neutron counts for incoming neutron flux using the method described in Anderson et al. (2017). The correction is performed using the following equation:
 
     $$
     C_{corrected} = \frac{C_{raw}}{f_i}
     $$
@@ -467,15 +332,15 @@
         warnings.warn('Reference incoming neutron flux not provided. Using first value of incoming neutron flux.')
     fi = incoming_neutrons / incoming_Ref
     fi.fillna(1.0, inplace=True)  # Use a value of 1 for days without data
 
     return fi
 
 
-def get_incoming_neutron_flux(start_date, end_date, station, utc_offset=0, expand_window = 0,  verbose=False):
+def get_incoming_neutron_flux(start_date, end_date, station, utc_offset=0, expand_window=0, verbose=False):
     """Function to retrieve neutron flux from the Neutron Monitor Database.
 
     Args:
         start_date (datetime): Start date of the time series.
         end_date (datetime): End date of the time series.
         station (str): Neutron Monitor station to retrieve data from.
         utc_offset (int): UTC offset in hours. Default is 0.
@@ -493,18 +358,17 @@
     # Template url = 'http://nest.nmdb.eu/draw_graph.php?formchk=1&stations[]=KERG&output=ascii&tabchoice=revori&dtype=corr_for_efficiency&date_choice=bydate&start_year=2009&start_month=09&start_day=01&start_hour=00&start_min=00&end_year=2009&end_month=09&end_day=05&end_hour=23&end_min=59&yunits=0'
 
 
     # Expand the time window by 1 hour to ensure an extra observation is included in the request.
     start_date -= pd.Timedelta(hours=expand_window)
     end_date += pd.Timedelta(hours=expand_window)
 
-
     # Convert local time to UTC
-    start_date = start_date - datetime.timedelta(hours=utc_offset)
-    end_date = end_date - datetime.timedelta(hours=utc_offset)
+    start_date = start_date - pd.Timedelta(hours=utc_offset)
+    end_date = end_date - pd.Timedelta(hours=utc_offset)
     date_format = '%Y-%m-%d %H:%M:%S'
     root = 'http://www.nmdb.eu/nest/draw_graph.php?'
     url_par = [ 'formchk=1',
                 'stations[]=' + station,
                 'output=ascii',
                 'tabchoice=revori',
                 'dtype=corr_for_efficiency',
@@ -520,29 +384,29 @@
                 'end_day=' + str(end_date.day),
                 'end_hour=' + str(end_date.hour),
                 'end_min=' + str(end_date.minute),
                 'yunits=0']
 
     url = root + '&'.join(url_par)
 
-    if verbose > 0:
+    if verbose:
         print(f"Retrieving data from {url}")
 
     r = requests.get(url).content.decode('utf-8')
 
     # Subtract 1 hour to restore the last date included in the request.
     end_date -= pd.Timedelta('1H')
     start = r.find("RCORR_E\n") + 8
     end = r.find('\n</code></pre><br>Total') - 1
     s = r[start:end]
     s2 = ''.join([row.replace(';',',') for row in s])
     try:
         df_flux = pd.read_csv(io.StringIO(s2), names=['timestamp','counts'])
     except:
-        if verbose > -1:
+        if verbose:
             print(f"Error retrieving data from {url}")
         return None
 
     # Check if all values from selected detector are NaN. If yes, warn the user
     if df_flux['counts'].isna().all():
         warnings.warn('Data for selected neutron detectors appears to be unavailable for the selected period')
 
@@ -552,43 +416,17 @@
 
     # Print acknowledgement to inform users about restrictions and to acknowledge the NMDB database
     acknowledgement = """Data retrieved via NMDB are the property of the individual data providers. These data are free for non commercial
 use to within the restriction imposed by the providers. If you use such data for your research or applications, please acknowledge
 the origin by a sentence like 'We acknowledge the NMDB database (www.nmdb.eu) founded under the European Union's FP7 programme 
 (contract no. 213007), and the PIs of individual neutron monitors at: IGY Jungfraujoch 
 (Physikalisches Institut, University of Bern, Switzerland)"""
-    #print(acknowledgement)
-
-    return df_flux.set_index('timestamp')
 
-def interpolate_incoming_flux(df_flux, timestamps):
-    """Function to interpolate incoming neutron flux to match the timestamps of the observations.
+    return df_flux
 
-    Args:
-        df_flux (pd.DataFrame): Dataframe returned by get_incoming_flux method.
-        timestamps (pd.series or pd.DataFrame or pd.DatetimeIndex): Timestamps to interpolate the incoming neutron flux.
-
-    Returns:
-        (pd.DataFrame): Dataframe containing interpolated incoming neutron flux.
-    """
-
-    # Check that index is datetime
-    if not isinstance(df_flux.index, pd.DatetimeIndex):
-        raise ValueError('Index of df_flux must be datetime')
-
-    for timestamp in timestamps:
-        if timestamp not in df_flux.index:
-            df_flux.loc[timestamp] = np.nan
-    df_flux = df_flux.sort_index()
-
-    # Interpolate nan values
-    df_flux = df_flux['counts'].interpolate(method='nearest', limit_direction='both')
-
-    # Retur only the values for the selected timestamps
-    return df_flux.loc[timestamps]
 
 
 def smooth_1d(values, window=5, order=3, method='moving_median'):
     """Use a Savitzky-Golay filter to smooth the signal of corrected neutron counts or another one-dimensional array (e.g. computed volumetric water content).
 
     Args:
         values (pd.DataFrame or pd.Serie): Dataframe containing the values to smooth.
@@ -623,15 +461,15 @@
                 values[col] = savgol_filter(values[col],window,order)
     else:
         raise ValueError('Invalid method. Please select a valid filtering method., options are: moving_average, moving_median, savitzky_golay')
     corrected_counts = corrected_counts.ffill(limit=window).bfill(limit=window).copy()
     return corrected_counts
 
 
-def bwe_correction(counts, bwe, r2_N0=0.05):
+def correction_bwe(counts, bwe, r2_N0=0.05):
     """Function to correct for biomass effects in neutron counts.
     following the approach described in Baatz et al., 2015.
 
     Args:
         counts (array or pd.Series or pd.DataFrame): Array of ephithermal neutron counts.
         bwe (float): Biomass water equivalent kg m-2.
         r2_N0 (float): Ratio of neutron counts with biomass to neutron counts without biomass. Default is 0.05.
@@ -663,15 +501,15 @@
         Wahbi, A., Avery, W. (2018). In Situ Destructive Sampling. In:
         Cosmic Ray Neutron Sensing: Estimation of Agricultural Crop Biomass Water Equivalent.
         Springer, Cham. https://doi.org/10.1007/978-3-319-69539-6_2
     """
     return (biomass_fresh - biomass_dry) + fWE * biomass_dry
 
 
-def road_correction(counts, theta_N, road_width, road_distance=0.0, theta_road=0.12, p0=0.42, p1=0.5, p2=1.06, p3=4, p4=0.16, p6=0.94, p7=1.10, p8=2.70, p9=0.01):
+def correction_road(counts, theta_N, road_width, road_distance=0.0, theta_road=0.12, p0=0.42, p1=0.5, p2=1.06, p3=4, p4=0.16, p6=0.94, p7=1.10, p8=2.70, p9=0.01):
     """Function to correct for road effects in neutron counts.
     following the approach described in Schrön et al., 2018.
 
     Args:
         counts (array or pd.Series or pd.DataFrame): Array of ephithermal neutron counts.
         theta_N (float): Volumetric water content of the soil estimated from the uncorrected neutron counts.
         road_width (float): Width of the road in m.
@@ -774,15 +612,15 @@
     elif method == 'Franz_2012':
         results = 5.8/(bulk_density*Wlat+vwc+0.0829)
     else:
         raise ValueError('Method not recognized. Please select either "Schron_2017" or "Franz_2012".')
 
     return results
 
-def estimate_abs_humidity(relative_humidity, temp):
+def abs_humidity(relative_humidity, temp):
     """
     Compute the actual vapor pressure (e) in g m^-3 using RH (%) and current temperature (c) observations.
 
     Args:
         relative_humidity (float): relative humidity (%)
         temp (float): temperature (Celsius)
 
@@ -874,28 +712,23 @@
     # Combined and normalized weights
     weights = Wd*W/np.nansum(Wd*W)
 
     return weights
 
 
 
-def storage(sm,T=1,Z_surface=150,Z_subsurface=1000):
+def exp_filter(sm,T=1):
     """Exponential filter to estimate soil moisture in the rootzone from surface observtions.
 
     Args:
-        sm (list or array): Soil moisture in mm of water.
+        sm (list or array): Soil moisture in mm of water for the top layer of the soil profile.
         T (float): Characteristic time length in the same units as the measurement interval.
-        Z_surface (float): Depth of surface layer in mm. This should be an intermediate value according to the
-            sensing depth computed using the D86 method.
-        Z_subsurface (float): Depth of subsurface layer in mm.
 
     Returns:
-        (tuple): tuple containing:
-            - **Surface soil water storage** (*array*): Surface soil water storage in mm of water.
-            - **Subsurface soil water storage** (*array*): Subsurface soil water storage in mm of water.
+        sm_subsurface (list or array): Subsurface soil moisture in the same units as the input.
 
     References:
         Albergel, C., Rüdiger, C., Pellarin, T., Calvet, J.C., Fritz, N., Froissard, F., Suquia, D., Petitpa, A., Piguet, B. and Martin, E., 2008.
         From near-surface to root-zone soil moisture using an exponential filter: an assessment of the method based on in-situ observations and model
         simulations. Hydrology and Earth System Sciences, 12(6), pp.1323-1337.
 
         Franz, T.E., Wahbi, A., Zhang, J., Vreugdenhil, M., Heng, L., Dercon, G., Strauss, P., Brocca, L. and Wagner, W., 2020.
@@ -906,17 +739,17 @@
     """
 
 
     # Parameters
     t_delta = 1
     sm_min = np.min(sm)
     sm_max = np.max(sm)
-    ms = (sm-sm_min)/(sm_max-sm_min)
+    ms = (sm - sm_min) / (sm_max - sm_min)
 
-    # Pre-allocate soil water index array
+    # Pre-allocate soil water index array and recursive constant K
     SWI = np.ones_like(ms)*np.nan
     K = np.ones_like(ms)*np.nan
 
     # Initial conditions
     SWI[0] = ms[0]
     K[0] = 1
 
@@ -924,21 +757,18 @@
     for n in range(1,len(SWI)):
         if ~np.isnan(ms[n]) & ~np.isnan(ms[n-1]):
             K[n] = K[n-1] / (K[n-1] + np.exp(-t_delta/T))
             SWI[n] = SWI[n-1] + K[n]*(ms[n] - SWI[n-1])
         else:
             continue
 
-    # Surface storage
-    storage_surface = sm*Z_surface
-
     # Rootzone storage
-    storage_subsurface = (SWI*(sm_max-sm_min) + sm_min)*Z_subsurface
+    sm_subsurface = SWI * (sm_max - sm_min) + sm_min
 
-    return storage_surface, storage_subsurface
+    return sm_subsurface
 
 
 def cutoff_rigidity(lat,lon):
     """Function to estimate the approximate cutoff rigidity for any point on Earth according to the
     tabulated data of Smart and Shea, 2019. The returned value can be used to select the appropriate
     neutron monitor station to estimate the cosmic-ray neutron intensity at the location of interest.
 
@@ -976,15 +806,15 @@
     points = np.array( (X.flatten(), Y.flatten()) ).T
     values = Z.flatten()
     zq = griddata(points, values, (xq,yq))
 
     return np.round(zq,2)
 
 
-def find_neutron_monitor(Rc, start_date=None, end_date=None):
+def find_neutron_monitor(Rc, start_date=None, end_date=None, verbose=False):
     """Search for potential reference neutron monitoring stations based on cutoff rigidity.
 
     Args:
         Rc (float): Cutoff rigidity in GV. Values in range 1.0 to 3.0 GV.
         start_date (datetime): Start date for the period of interest.
         end_date (datetime): End date for the period of interest.
 
@@ -1022,15 +852,15 @@
     idx_R = (stations['R'] - Rc).abs().argsort()
 
     if start_date is not None and end_date is not None:
         stations["Period available"] = False
         for i in range(10):
             station = stations.iloc[idx_R[i]]["STID"]
             try:
-                if get_incoming_neutron_flux(start_date, end_date, station, verbose=-1) is not None:
+                if get_incoming_neutron_flux(start_date, end_date, station, verbose=verbose) is not None:
                     stations.iloc[idx_R[i],-1] = True
             except:
                 pass
         if sum(stations["Period available"] == True) == 0:
             print("No stations available for the selected period!")
         else:
             stations = stations[stations["Period available"] == True]
@@ -1044,15 +874,41 @@
     print("""Select a station with an altitude similar to that of your location. For more information go to: 'https://www.nmdb.eu/nest/help.php#helpstations""")
     print('')
     print(f"Your cutoff rigidity is {Rc} GV")
     print(result)
     return result
 
 
-def estimate_lattice_water(clay_content, total_carbon=None):
+def interpolate_incoming_flux(nmdb_timestamps, nmdb_counts, crnp_timestamps):
+    """Function to interpolate incoming neutron flux to match the timestamps of the observations.
+
+    Args:
+        nmdb_timestamps (pd.Series): Series of timestamps in datetime format from the NMDB.
+        nmdb_counts (pd.Series): Series of neutron counts from the NMDB
+        crnp_timestamps (pd.Series): Series of timestamps in datetime format from the station or device.
+
+    Returns:
+        (pd.Series): Series containing interpolated incoming neutron flux. Length of Series is the same as crnp_timestamps
+    """
+    incoming_flux = np.array([])
+    for k,timestamp in enumerate(crnp_timestamps):
+        if timestamp in nmdb_timestamps.values:
+            idx = timestamp == nmdb_timestamps
+            incoming_flux = np.append(incoming_flux, nmdb_counts.loc[idx])
+        else:
+            incoming_flux = np.append(incoming_flux, np.nan)
+
+    # Interpolate nan values
+    incoming_flux = pd.Series(incoming_flux).interpolate(method='nearest', limit_direction='both')
+
+    # Return only the values for the selected timestamps
+    return incoming_flux
+
+
+def lattice_water(clay_content, total_carbon=None):
     r"""Estimate the amount of water in the lattice of clay minerals.
 
     ![img1](img/lattice_water_simple.png) | ![img2](img/lattice_water_multiple.png)
     :-------------------------:|:-------------------------:
     $\omega_{lat} = 0.097 * clay(\%)$ | $\omega_{lat} = -0.028 + 0.077 * clay(\%) + 0.459 * carbon(\%)$
     Linear regression [lattice water (%) as a function of clay (%)] done with data from Kansas Sate University - Soil Water Processes Lab. |  Multiple linear regression [lattice water (%) as a function of clay (%) and soil carbon (%)] done with data from Soil Water Processes Lab.
 
@@ -1322,15 +1178,15 @@
 
     else:
         raise f"Method {method} does not exist. Provide either 'cubic', 'linear', 'nearest', or 'idw'."
 
     return X_pred, Y_pred, Z_pred
 
 
-def estimate_locations(x, y):
+def rover_centered_coordinates(x, y):
     """Function to estimate the intermediate locations between two points, assuming the measurements were taken at a constant speed.
 
     Args:
         x (array): x coordinates.
         y (array): y coordinates.
 
     Returns:
@@ -1352,9 +1208,84 @@
     x_est = np.insert(x_est, 0, x[0])
     y_est = np.insert(y_est, 0, y[0])
 
 
     return x_est, y_est
 
 
+def uncertainty_counts(raw_counts, metric="std", fp=1, fw=1, fi=1):
+    """Function to estimate the uncertainty of raw counts.
+
+    Measurements of proportional neutron detector systems are governed by counting statistics that follow a Poissonian probability distribution (Zreda et al., 2012).
+    The expected uncertainty in the neutron count rate $N$ is defined by the standard deviation $ \sqrt{N} $ (Jakobi et al., 2020).
+    The CV% can be expressed as $ N^{-1/2} $
+
+    Args:
+        raw_counts (array): Raw neutron counts.
+        metric (str): Either 'std' or 'cv' for standard deviation or coefficient of variation.
+        fp (float): Pressure correction factor.
+        fw (float): Humidity correction factor.
+        fi (float): Incoming neutron flux correction factor.
+
+    Returns:
+        uncertainty (float): Uncertainty of raw counts.
+
+    References:
+        Jakobi J, Huisman JA, Schrön M, Fiedler J, Brogi C, Vereecken H and Bogena HR (2020) Error Estimation for Soil Moisture Measurements With
+        Cosmic Ray Neutron Sensing and Implications for Rover Surveys. Front. Water 2:10. doi: 10.3389/frwa.2020.00010
+
+        Zreda, M., Shuttleworth, W. J., Zeng, X., Zweck, C., Desilets, D., Franz, T., and Rosolem, R.: COSMOS: the COsmic-ray Soil Moisture Observing System,
+        Hydrol. Earth Syst. Sci., 16, 4079–4099, https://doi.org/10.5194/hess-16-4079-2012, 2012.
+
+    """
+
+    s = fw / (fp * fi)
+    if metric == "std":
+        uncertainty = np.sqrt(raw_counts) * s
+    elif metric == "cv":
+        uncertainty = 1 /  np.sqrt(raw_counts) * s
+    else:
+        raise f"Metric {metric} does not exist. Provide either 'std' or 'cv' for standard deviation or coefficient of variation."
+    return uncertainty
+
+
+def uncertainty_vwc(raw_counts, N0, bulk_density, fp=1, fw=1, fi=1, a0=0.0808,a1=0.372,a2=0.115):
+    r"""Function to estimate the uncertainty propagated to volumetric water content.
+
+    The uncertainty of the volumetric water content is estimated by propagating the uncertainty of the raw counts.
+    Following Eq. 10 in Jakobi et al. (2020), the uncertainty of the volumetric water content can be expressed as:
+    $$
+    \sigma_{\theta_g}(N) = \sigma_N \frac{a_0 N_0}{(N_{cor} - a_1 N_0)^4} \sqrt{(N_{cor} - a_1 N_0)^4 + 8 \sigma_N^2 (N_{cor} - a_1 N_0)^2 + 15 \sigma_N^4}
+    $$
+
+    Args:
+        raw_counts (array): Raw neutron counts.
+        N0 (float): Calibration parameter N0.
+        bulk_density (float): Bulk density in g cm-3.
+        fp (float): Pressure correction factor.
+        fw (float): Humidity correction factor.
+        fi (float): Incoming neutron flux correction factor.
+
+    Returns:
+        sigma_VWC (float): Uncertainty in terms of volumetric water content.
+
+    References:
+        Jakobi J, Huisman JA, Schrön M, Fiedler J, Brogi C, Vereecken H and Bogena HR (2020) Error Estimation for Soil Moisture Measurements With
+        Cosmic Ray Neutron Sensing and Implications for Rover Surveys. Front. Water 2:10. doi: 10.3389/frwa.2020.00010
+    """
+
+    Ncorr = raw_counts * fw / (fp * fi)
+    sigma_N = uncertainty_counts(raw_counts, metric="std", fp=fp, fw=fw, fi=fi)
+    sigma_GWC = sigma_N * ((a0*N0) / ((Ncorr - a1*N0)**4)) * np.sqrt((Ncorr - a1 * N0)**4 + 8 * sigma_N**2 * (Ncorr - a1 * N0)**2 + 15 * sigma_N**4)
+    sigma_VWC = sigma_GWC * bulk_density
+
+    return sigma_VWC
+
+
+
+
+
+
+
+
```

### Comparing `crnpy-0.5.0/src/crnpy/data.py` & `crnpy-0.5.1/src/crnpy/data.py`

 * *Files identical despite different names*

