# Comparing `tmp/gaitalytics-0.1.3b0.tar.gz` & `tmp/gaitalytics-0.1.4b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaitalytics-0.1.3b0.tar", last modified: Mon Jul  3 08:11:01 2023, max compression
+gzip compressed data, was "gaitalytics-0.1.4b0.tar", last modified: Sun Jul 30 10:57:28 2023, max compression
```

## Comparing `gaitalytics-0.1.3b0.tar` & `gaitalytics-0.1.4b0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 08:11:01.782161 gaitalytics-0.1.3b0/
--rw-rw-rw-   0        0        0     1096 2023-04-25 17:34:59.000000 gaitalytics-0.1.3b0/LICENSE
--rw-rw-rw-   0        0        0     7033 2023-07-03 08:11:01.782161 gaitalytics-0.1.3b0/PKG-INFO
--rw-rw-rw-   0        0        0     6509 2023-07-01 10:26:24.000000 gaitalytics-0.1.3b0/README.md
--rw-rw-rw-   0        0        0       84 2023-06-21 07:51:06.000000 gaitalytics-0.1.3b0/pyproject.toml
--rw-rw-rw-   0        0        0      728 2023-07-03 08:11:01.782161 gaitalytics-0.1.3b0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-03 08:11:01.735602 gaitalytics-0.1.3b0/src/
-drwxrwxrwx   0        0        0        0 2023-07-03 08:11:01.767217 gaitalytics-0.1.3b0/src/gaitalytics/
--rw-rw-rw-   0        0        0        0 2023-06-21 08:57:09.000000 gaitalytics-0.1.3b0/src/gaitalytics/__init__.py
--rw-rw-rw-   0        0        0    27232 2023-07-01 08:08:36.000000 gaitalytics-0.1.3b0/src/gaitalytics/analysis.py
--rw-rw-rw-   0        0        0    14608 2023-07-01 11:36:32.000000 gaitalytics-0.1.3b0/src/gaitalytics/api.py
--rw-rw-rw-   0        0        0     3226 2023-06-28 07:52:44.000000 gaitalytics-0.1.3b0/src/gaitalytics/c3d.py
--rw-rw-rw-   0        0        0    13160 2023-07-01 08:19:58.000000 gaitalytics-0.1.3b0/src/gaitalytics/cycle.py
--rw-rw-rw-   0        0        0     3340 2023-06-20 15:51:04.000000 gaitalytics-0.1.3b0/src/gaitalytics/emg.py
--rw-rw-rw-   0        0        0    15989 2023-06-28 13:09:43.000000 gaitalytics-0.1.3b0/src/gaitalytics/events.py
--rw-rw-rw-   0        0        0     8634 2023-07-03 08:09:26.000000 gaitalytics-0.1.3b0/src/gaitalytics/modelling.py
--rw-rw-rw-   0        0        0     6139 2023-07-01 08:19:58.000000 gaitalytics-0.1.3b0/src/gaitalytics/plot.py
--rw-rw-rw-   0        0        0    14514 2023-07-01 08:19:58.000000 gaitalytics-0.1.3b0/src/gaitalytics/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-03 08:11:01.778033 gaitalytics-0.1.3b0/src/gaitalytics.egg-info/
--rw-rw-rw-   0        0        0     7033 2023-07-03 08:11:01.000000 gaitalytics-0.1.3b0/src/gaitalytics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      490 2023-07-03 08:11:01.000000 gaitalytics-0.1.3b0/src/gaitalytics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 08:11:01.000000 gaitalytics-0.1.3b0/src/gaitalytics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-07-03 08:11:01.000000 gaitalytics-0.1.3b0/src/gaitalytics.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-03 08:11:01.000000 gaitalytics-0.1.3b0/src/gaitalytics.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 10:57:28.124027 gaitalytics-0.1.4b0/
+-rw-rw-rw-   0        0        0     1096 2023-04-25 17:34:59.000000 gaitalytics-0.1.4b0/LICENSE
+-rw-rw-rw-   0        0        0     7033 2023-07-30 10:57:28.125033 gaitalytics-0.1.4b0/PKG-INFO
+-rw-rw-rw-   0        0        0     6509 2023-07-01 10:26:24.000000 gaitalytics-0.1.4b0/README.md
+-rw-rw-rw-   0        0        0       84 2023-06-21 07:51:06.000000 gaitalytics-0.1.4b0/pyproject.toml
+-rw-rw-rw-   0        0        0      728 2023-07-30 10:57:28.126033 gaitalytics-0.1.4b0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-30 10:57:28.083834 gaitalytics-0.1.4b0/src/
+drwxrwxrwx   0        0        0        0 2023-07-30 10:57:28.111028 gaitalytics-0.1.4b0/src/gaitalytics/
+-rw-rw-rw-   0        0        0        0 2023-06-21 08:57:09.000000 gaitalytics-0.1.4b0/src/gaitalytics/__init__.py
+-rw-rw-rw-   0        0        0    24923 2023-07-29 13:19:09.000000 gaitalytics-0.1.4b0/src/gaitalytics/analysis.py
+-rw-rw-rw-   0        0        0    15018 2023-07-29 13:20:11.000000 gaitalytics-0.1.4b0/src/gaitalytics/api.py
+-rw-rw-rw-   0        0        0     3226 2023-06-28 07:52:44.000000 gaitalytics-0.1.4b0/src/gaitalytics/c3d.py
+-rw-rw-rw-   0        0        0    13160 2023-07-01 08:19:58.000000 gaitalytics-0.1.4b0/src/gaitalytics/cycle.py
+-rw-rw-rw-   0        0        0     3340 2023-06-20 15:51:04.000000 gaitalytics-0.1.4b0/src/gaitalytics/emg.py
+-rw-rw-rw-   0        0        0    19091 2023-07-26 09:09:41.000000 gaitalytics-0.1.4b0/src/gaitalytics/events.py
+-rw-rw-rw-   0        0        0    11276 2023-07-29 15:25:04.000000 gaitalytics-0.1.4b0/src/gaitalytics/modelling.py
+-rw-rw-rw-   0        0        0     6139 2023-07-01 08:19:58.000000 gaitalytics-0.1.4b0/src/gaitalytics/plot.py
+-rw-rw-rw-   0        0        0    14514 2023-07-01 08:19:58.000000 gaitalytics-0.1.4b0/src/gaitalytics/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-30 10:57:28.123058 gaitalytics-0.1.4b0/src/gaitalytics.egg-info/
+-rw-rw-rw-   0        0        0     7033 2023-07-30 10:57:28.000000 gaitalytics-0.1.4b0/src/gaitalytics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      490 2023-07-30 10:57:28.000000 gaitalytics-0.1.4b0/src/gaitalytics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 10:57:28.000000 gaitalytics-0.1.4b0/src/gaitalytics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-07-30 10:57:28.000000 gaitalytics-0.1.4b0/src/gaitalytics.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-30 10:57:28.000000 gaitalytics-0.1.4b0/src/gaitalytics.egg-info/top_level.txt
```

### Comparing `gaitalytics-0.1.3b0/LICENSE` & `gaitalytics-0.1.4b0/LICENSE`

 * *Files identical despite different names*

### Comparing `gaitalytics-0.1.3b0/PKG-INFO` & `gaitalytics-0.1.4b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaitalytics
-Version: 0.1.3b0
+Version: 0.1.4b0
 Summary: Library to analyse gait data captured with a mocap system
 Home-page: https://github.com/cereneo-foundation/gaitalytics
 Author: André Böni
 Author-email: andre.boeni@cereneo.foundation
 License: MIT
 Keywords: gait,analysis,c3d,mocap
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gaitalytics-0.1.3b0/README.md` & `gaitalytics-0.1.4b0/README.md`

 * *Files identical despite different names*

### Comparing `gaitalytics-0.1.3b0/setup.cfg` & `gaitalytics-0.1.4b0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2067 6169 7461 6c79 7469 6373 0d0a   = gaitalytics..
-00000020: 7665 7273 696f 6e20 3d20 302e 312e 3362  version = 0.1.3b
+00000020: 7665 7273 696f 6e20 3d20 302e 312e 3462  version = 0.1.4b
 00000030: 6574 610d 0a61 7574 686f 7220 3d20 416e  eta..author = An
 00000040: 6472 c3a9 2042 c3b6 6e69 0d0a 6175 7468  dr.. B..ni..auth
 00000050: 6f72 5f65 6d61 696c 203d 2061 6e64 7265  or_email = andre
 00000060: 2e62 6f65 6e69 4063 6572 656e 656f 2e66  .boeni@cereneo.f
 00000070: 6f75 6e64 6174 696f 6e0d 0a75 726c 203d  oundation..url =
 00000080: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
 00000090: 636f 6d2f 6365 7265 6e65 6f2d 666f 756e  com/cereneo-foun
```

### Comparing `gaitalytics-0.1.3b0/src/gaitalytics/analysis.py` & `gaitalytics-0.1.4b0/src/gaitalytics/analysis.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 from typing import Dict
 
 import numpy as np
 from pandas import DataFrame, concat
 from scipy import signal
 
 import gaitalytics.utils
+import logging
 
-
+logger = logging.getLogger(__name__)
 class AbstractAnalysis(ABC):
     def __init__(self, data_list: Dict[str, gaitalytics.utils.BasicCyclePoint],
                  configs: gaitalytics.utils.ConfigProvider):
         self._data_list: Dict[str, gaitalytics.utils.BasicCyclePoint] = data_list
         self._configs = configs
 
     def analyse(self, **kwargs) -> DataFrame:
@@ -31,14 +32,15 @@
         pass
 
     def _filter_keys(self, key: str) -> bool:
         """ Check if its the right point data """
         return f".{self._point_data_type.name}." in key
 
     def analyse(self, **kwargs) -> DataFrame:
+        logger.info(f"analyse: {self._point_data_type}")
         by_phase = kwargs.get("by_phase", True)
         results = None
         for key in self._data_list:  # TODO change quick fix
             if self._filter_keys(key):
                 raw_point = self._data_list[key]
                 data = raw_point.data_table
                 if not by_phase:
@@ -169,17 +171,15 @@
 class CMosAnalysis(AbstractCycleAnalysis):
 
     def __init__(self, data_list: Dict, configs: gaitalytics.utils.ConfigProvider):
         super().__init__(data_list, configs, gaitalytics.utils.PointDataType.Marker)
 
     def _filter_keys(self, key: str) -> bool:
         if super()._filter_keys(key):
-            useful = self._configs.MARKER_MAPPING.right_cmos.name in key
-            useful = self._configs.MARKER_MAPPING.left_cmos.name in key or useful
-            return useful
+            return self._configs.MARKER_MAPPING.cmos.name in key
         return False
 
     def _do_analysis(self, data: DataFrame) -> DataFrame:
         results = DataFrame(index=data.index)
 
         results['cmos_mean'] = data.mean(axis=1)
         results['cmos_max'] = data.max(axis=1)
@@ -188,47 +188,18 @@
 
         return results
 
 
 class MosAnalysis(AbstractAnalysis):
 
     def analyse(self, **kwargs) -> DataFrame:
-        left_cmos_ap = self._data_list[
-            gaitalytics.utils.ConfigProvider.define_key(self._configs.MARKER_MAPPING.left_cmos,
-                                                        gaitalytics.utils.PointDataType.Marker,
-                                                        gaitalytics.utils.AxesNames.y,
-                                                        gaitalytics.utils.GaitEventContext.LEFT)]
-        left_cmos_ml = self._data_list[
-            gaitalytics.utils.ConfigProvider.define_key(self._configs.MARKER_MAPPING.left_cmos,
-                                                        gaitalytics.utils.PointDataType.Marker,
-                                                        gaitalytics.utils.AxesNames.x,
-                                                        gaitalytics.utils.GaitEventContext.LEFT)]
-
-        right_cmos_ap = self._data_list[
-            gaitalytics.utils.ConfigProvider.define_key(self._configs.MARKER_MAPPING.right_cmos,
-                                                        gaitalytics.utils.PointDataType.Marker,
-                                                        gaitalytics.utils.AxesNames.y,
-                                                        gaitalytics.utils.GaitEventContext.RIGHT)]
-        right_cmos_ml = self._data_list[
-            gaitalytics.utils.ConfigProvider.define_key(self._configs.MARKER_MAPPING.right_cmos,
-                                                        gaitalytics.utils.PointDataType.Marker,
-                                                        gaitalytics.utils.AxesNames.x,
-                                                        gaitalytics.utils.GaitEventContext.RIGHT)]
-
-        left_ap = self._extract_mos_frames(left_cmos_ap, "left", "ap")
-        left_ml = self._extract_mos_frames(left_cmos_ml, "left", "ml")
-        right_ap = self._extract_mos_frames(right_cmos_ap, "right", "ap")
-        right_ml = self._extract_mos_frames(right_cmos_ml, "right", "ml")
-        result = left_ap.merge(left_ml, on=gaitalytics.utils.BasicCyclePoint.CYCLE_NUMBER)
-        result = result.merge(right_ap, on=gaitalytics.utils.BasicCyclePoint.CYCLE_NUMBER)
-        result = result.merge(right_ml, on=gaitalytics.utils.BasicCyclePoint.CYCLE_NUMBER)
+        # TODO MOS
 
 
-        result['metric'] = "Mos"
-        return result.pivot(columns="metric")
+        return DataFrame()
 
     @staticmethod
     def _extract_mos_frames(cmos: gaitalytics.utils.BasicCyclePoint.CYCLE_NUMBER, side, direction):
         hs_label = f"{direction}_hs_{side}"
         to_label = f"{direction}_to_{side}"
         hs_contra_label = f"{direction}_hs_contra_{side}"
         to_contra_label = f"{direction}_to_contra_{side}"
```

### Comparing `gaitalytics-0.1.3b0/src/gaitalytics/api.py` & `gaitalytics-0.1.4b0/src/gaitalytics/api.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,30 @@
 from __future__ import annotations
 
+import logging
 import os
+import sys
 from typing import Dict, List
 
 from pandas import DataFrame
 
 import gaitalytics.analysis
 import gaitalytics.c3d
 import gaitalytics.cycle
 import gaitalytics.events
 import gaitalytics.modelling
 import gaitalytics.utils
 
+logging.basicConfig(level=logging.DEBUG,
+                    format='%(asctime)s %(levelname)s %(name)s - %(message)s',
+                    datefmt='%d-%b-%y %H:%M:%S',
+                    handlers=[logging.StreamHandler(sys.stdout)])
+
+logger = logging.getLogger(__name__)
+
 # constants
 CYCLE_METHOD_HEEL_STRIKE = "HS"
 CYCLE_METHOD_TOE_OFF = "TO"
 
 NORMALISE_METHODE_LINEAR = "linear"
 NORMALISE_METHODE_LIST = (NORMALISE_METHODE_LINEAR)
 
@@ -37,34 +46,36 @@
 ANALYSIS_MOS = "mos"
 ANALYSIS_LIST = (ANALYSIS_MOMENTS,
                  ANALYSIS_ANGLES,
                  ANALYSIS_POWERS,
                  ANALYSIS_FORCES,
                  ANALYSIS_SPATIO_TEMP,
                  ANALYSIS_TOE_CLEARANCE,
-                 ANALYSIS_CMOS,
-                 ANALYSIS_MOS)
+                 ANALYSIS_CMOS)
 
 MODELLING_COM = "com"
 MODELLING_CMOS = "cmos"
+MODELLING_XCOM = "xcom"
 MODELLING_LIST = [MODELLING_COM,
-                  MODELLING_CMOS]
+                  MODELLING_CMOS,
+                  MODELLING_XCOM]
 
 
 def analyse_data(cycle_data: Dict[str, gaitalytics.utils.BasicCyclePoint],
                  config: gaitalytics.utils.ConfigProvider,
                  methode: List[str] = ANALYSIS_LIST, **kwargs: dict) -> DataFrame:
     """
     Runs specified analysis and concatenates into one Dataframe
 
     :param cycle_data: full length cycle data
     :param config: configs from marker and model mapping
     :param methode: list of methods
     :return: results of analysis
     """
+    logger.info("analyse_data")
     if not all(item in ANALYSIS_LIST for item in methode):
         raise KeyError(f"{methode} are not a valid anomaly checker")
 
     methods: List[gaitalytics.analysis.AbstractAnalysis] = []
     if ANALYSIS_ANGLES in methode:
         methods.append(gaitalytics.analysis.JointAnglesCycleAnalysis(cycle_data, config))
     if ANALYSIS_MOMENTS in methode:
@@ -101,14 +112,15 @@
     with given anomaly_checker method and saves it in output_path with '*_anomaly.txt' extension
 
     :param c3d_file_path: path of c3d file with modelled filtered data '.3.c3d'
     :param output_path: path to dir to store c3d file with events
     :param anomaly_checker: list of anomaly checkers, "context" api.GAIT_EVENT_CHECKER_CONTEXT,
        "spacing" api.GAIT_EVENT_CHECKER_SPACING
     """
+    logger.info("check_gait_event")
     if not os.path.isfile(c3d_file_path):
         raise FileExistsError(f"{c3d_file_path} does not exists")
     if not os.path.isdir(output_path):
         raise FileExistsError(f"{output_path} does not exists")
     if not all(item in GAIT_EVENT_CHECKER_LIST for item in anomaly_checker):
         raise KeyError(f"{anomaly_checker} are not a valid anomaly checker")
     # read c3d
@@ -140,14 +152,15 @@
     :param output_path: path to dir to store c3d file with events
     :param configs: configs from marker and model mapping
     :param methode: methode to detect events 'Marker' api.GAIT_EVENT_METHODE_MARKER or
         'Forceplate' api.GAIT_EVENT_METHODE_FP
     :param anomaly_checker: list of anomaly checkers, "context" api.GAIT_EVENT_CHECKER_CONTEXT,
         "spacing" api.GAIT_EVENT_CHECKER_SPACING
     """
+    logger.info("detect_gait_events")
     if not os.path.isfile(c3d_file_path):
         raise FileExistsError(f"{c3d_file_path} does not exists")
     if not os.path.isdir(output_path):
         raise FileExistsError(f"{output_path} does not exists")
     if methode not in GAIT_EVENT_METHODE_LIST:
         raise KeyError(f"{methode} is not a valid methode")
     if not all(item in GAIT_EVENT_CHECKER_LIST for item in anomaly_checker):
@@ -176,14 +189,15 @@
 def _get_anomaly_checker(anomaly_checker: List[str]) -> gaitalytics.events.AbstractEventAnomalyChecker:
     """
     defines checker by list of inputs
 
     :param anomaly_checker: list of checker name
     :return: checker object
     """
+    logger.info("_get_anomaly_checker")
     checker = None
     if GAIT_EVENT_CHECKER_CONTEXT in anomaly_checker:
         checker = gaitalytics.events.ContextPatternChecker()
     if GAIT_EVENT_CHECKER_SPACING in anomaly_checker:
         checker = gaitalytics.events.EventSpacingChecker(checker)
     return checker
 
@@ -194,14 +208,15 @@
     gets normalised and full length data from buffered folder. It is needed to run api.extract_cycles as
     api.normalise_cycles with given buffer_output_path once to use this function
 
     :param buffer_output_path: path to folder
     :param configs: configs from marker and model mapping
     :return: object containing normalised and full length data lists
     """
+    logger.info("extract_cycles_buffered")
     if not os.path.isdir(buffer_output_path):
         raise FileExistsError(f"{buffer_output_path} does not exists")
 
     # load cycles
     loader = gaitalytics.cycle.CyclePointLoader(configs, buffer_output_path)
     return loader
 
@@ -220,14 +235,15 @@
     :param configs: configs from marker and model mapping
     :param methode: method to cut gait cycles either "HS" api.CYCLE_METHOD_HEEL_STRIKE or "TO" api.CYCLE_METHOD_TOE_OFF
     :param buffer_output_path: if buffering needed path to folder
     :param anomaly_checker: list of anomaly checkers, "context" api.GAIT_EVENT_CHECKER_CONTEXT,
         "spacing" api.GAIT_EVENT_CHECKER_SPACING
     :return: extracted gait cycles
     """
+    logger.info("extract_cycles")
     # check params for validity
     if not os.path.isfile(c3d_file_path):
         raise FileExistsError(f"{c3d_file_path} does not exists")
     if methode not in [CYCLE_METHOD_HEEL_STRIKE, CYCLE_METHOD_TOE_OFF]:
         raise KeyError(f"{methode} is not a valid methode")
     if buffer_output_path:
         if not os.path.isdir(buffer_output_path):
@@ -271,15 +287,15 @@
 
     :param c3d_file_path:  path of c3d file with foot_off and foot_strike events '*.4.c3d'
     :param cycle_data: full length cycle data
     :param method: method normalise "linear" api.NORMALISE_METHODE_LINEAR
     :param buffer_output_path: if buffering needed path to folder
     :return: normalised gait cycles
     """
-
+    logger.info("normalise_cycles")
     # check params for validity
     if method not in NORMALISE_METHODE_LIST:
         raise KeyError(f"{method} is not a valid methode")
     if buffer_output_path:
         if not os.path.isdir(buffer_output_path):
             raise FileExistsError(f"{buffer_output_path} does not exists")
 
@@ -308,39 +324,40 @@
 
     :param c3d_file_path: path of c3d file with modelled filtered data '.3.c3d'
     :param output_path: path to dir to store c3d file with events
     :param configs: configs from marker and model mapping
     :param methode: methode to detect events
     :keyword belt_speed: belt speed
     """
+    logger.info("model_data")
     if not methode in MODELLING_LIST:
         raise KeyError(f"{methode} is not a valid modelling methode")
     methods: List[gaitalytics.modelling.BaseOutputModeller] = []
     acq = gaitalytics.c3d.read_btk(c3d_file_path)
     subject = gaitalytics.utils.extract_subject(acq)
     if methode == MODELLING_CMOS:
         methods.append(gaitalytics.modelling.COMModeller(configs))
-        methods.append(gaitalytics.modelling.CMoSModeller(gaitalytics.utils.GaitEventContext.LEFT,
-                                                          configs,
-                                                          subject.left_leg_length,
-                                                          **kwargs))
-        methods.append(gaitalytics.modelling.CMoSModeller(gaitalytics.utils.GaitEventContext.RIGHT,
-                                                          configs,
-                                                          subject.right_leg_length,
+        methods.append(gaitalytics.modelling.XCOMModeller(configs))
+        methods.append(gaitalytics.modelling.CMoSModeller(configs,
                                                           **kwargs))
+
+    elif methode == MODELLING_XCOM:
+        methods.append(gaitalytics.modelling.COMModeller(configs))
+        methods.append(gaitalytics.modelling.XCOMModeller(configs))
     elif methode == MODELLING_COM:
         methods.append(gaitalytics.modelling.COMModeller(configs))
 
     for methode in methods:
         methode.create_point(acq, **kwargs)
     filename = os.path.basename(c3d_file_path)
     filename = filename.replace(".4.c3d", ".5.c3d")
     output_path = os.path.join(output_path, filename)
     gaitalytics.c3d.write_btk(acq, output_path)
 
 
 def _cycle_points_to_csv(cycle_data: Dict[str, gaitalytics.utils.BasicCyclePoint], dir_path: str, prefix: str):
+    logger.info("_cycle_points_to_csv")
     subject_saved = False
     for key in cycle_data:
         cycle_data[key].to_csv(dir_path, prefix)
         if not subject_saved:
             cycle_data[key].subject.to_file(dir_path)
```

### Comparing `gaitalytics-0.1.3b0/src/gaitalytics/c3d.py` & `gaitalytics-0.1.4b0/src/gaitalytics/c3d.py`

 * *Files identical despite different names*

### Comparing `gaitalytics-0.1.3b0/src/gaitalytics/cycle.py` & `gaitalytics-0.1.4b0/src/gaitalytics/cycle.py`

 * *Files identical despite different names*

### Comparing `gaitalytics-0.1.3b0/src/gaitalytics/emg.py` & `gaitalytics-0.1.4b0/src/gaitalytics/emg.py`

 * *Files identical despite different names*

### Comparing `gaitalytics-0.1.3b0/src/gaitalytics/events.py` & `gaitalytics-0.1.4b0/src/gaitalytics/events.py`

 * *Files 11% similar despite different names*

```diff
@@ -56,57 +56,120 @@
         :param acq: loaded and filtered acquisition
         :param min_distance: minimum frames between same event
         :param show_plot: plots of zenis shown
         """
         min_distance = kwargs.get("min_distance", 100)
         show_plot = kwargs.get("show_plot", False)
 
-        right_heel = acq.GetPoint(self._config.MARKER_MAPPING.right_heel.value).GetValues()
-        left_heel = acq.GetPoint(self._config.MARKER_MAPPING.left_heel.value).GetValues()
-        right_hip = acq.GetPoint(self._config.MARKER_MAPPING.right_back_hip.value).GetValues()
-        left_hip = acq.GetPoint(self._config.MARKER_MAPPING.left_back_hip.value).GetValues()
-
+        right_heel = acq.GetPoint(self._config.MARKER_MAPPING.right_heel.value).GetValues()[:,
+                     gaitalytics.utils.AxesNames.y.value]
+        left_heel = acq.GetPoint(self._config.MARKER_MAPPING.left_heel.value).GetValues()[:,
+                    gaitalytics.utils.AxesNames.y.value]
+        right_toe = acq.GetPoint(self._config.MARKER_MAPPING.right_meta_2.value).GetValues()[:,
+                    gaitalytics.utils.AxesNames.y.value]
+        left_toe = acq.GetPoint(self._config.MARKER_MAPPING.left_meta_2.value).GetValues()[:,
+                   gaitalytics.utils.AxesNames.y.value]
+        right_hip = acq.GetPoint(self._config.MARKER_MAPPING.right_back_hip.value).GetValues()[:,
+                    gaitalytics.utils.AxesNames.y.value]
+        left_hip = acq.GetPoint(self._config.MARKER_MAPPING.left_back_hip.value).GetValues()[:,
+                   gaitalytics.utils.AxesNames.y.value]
+        '''
+        left_heel, left_toe, right_heel, right_toe, right_hip, left_hip = self._move_to_plus(left_heel,
+                                                                                             left_hip,
+                                                                                             left_toe,
+                                                                                             right_heel,
+                                                                                             right_hip,
+                                                                                             right_toe)
+        '''
         sacrum = (right_hip + left_hip) / 2.0
-        right_diff_heel = right_heel - sacrum
-        left_diff_heel = left_heel - sacrum
-        right_diff_toe = right_heel - sacrum
-        left_diff_toe = left_heel - sacrum
+        right_diff_heel = (right_heel - sacrum) * -1
+        left_diff_heel = (left_heel - sacrum) * -1
+        right_diff_toe = right_toe - sacrum
+        left_diff_toe = left_toe - sacrum
+
+        if show_plot:
+            base_title = "Test"
+            self._plot_curves(right_diff_heel,
+                              right_heel,
+                              sacrum, f"{base_title}_right_heel")
+            self._plot_curves(left_diff_heel,
+                              left_heel,
+                              sacrum, f"{base_title}_left_heel")
 
         self._create_events(acq, left_diff_toe, gaitalytics.utils.GaitEventLabel.FOOT_OFF,
                             gaitalytics.utils.GaitEventContext.LEFT, min_distance, show_plot)
         self._create_events(acq, right_diff_toe, gaitalytics.utils.GaitEventLabel.FOOT_OFF,
                             gaitalytics.utils.GaitEventContext.RIGHT, min_distance, show_plot)
         self._create_events(acq, left_diff_heel, gaitalytics.utils.GaitEventLabel.FOOT_STRIKE,
                             gaitalytics.utils.GaitEventContext.LEFT, min_distance, show_plot)
         self._create_events(acq, right_diff_heel, gaitalytics.utils.GaitEventLabel.FOOT_STRIKE,
                             gaitalytics.utils.GaitEventContext.RIGHT, min_distance, show_plot)
 
+    @staticmethod
+    def _plot_curves(diff, foot, sacrum, title):
+        from_frame = 3000
+        to_frame = 3500
+        fig, host = plt.subplots(figsize=(15, 12), layout='constrained')
+        diff_short = diff[from_frame:to_frame]
+        foot_short = foot[from_frame:to_frame]
+        sacrum_short = sacrum[from_frame:to_frame]
+
+        ax2 = host.twinx()
+        ax3 = host.twinx()
+
+        host.set_xlabel("Time")
+        host.set_ylabel("Diff")
+        ax2.set_ylabel("foot")
+        ax3.set_ylabel("sacrum")
+
+        color1, color2, color3 = plt.cm.viridis([0, .5, .9])
+        p1 = host.plot(diff_short, color=color1, label="diff")
+        extremes, foo = signal.find_peaks(diff_short)
+        host.plot( extremes, diff_short[extremes], "x")
+        p2 = ax2.plot(foot_short, color=color2, label="foot")
+        p3 = ax3.plot(sacrum_short, color=color3, label="sacrum")
+
+        host.legend(handles=p1 + p2 + p3, loc='best')
+        # right, left, top, bottom
+        ax3.spines['right'].set_position(('outward', 60))
+        plt.savefig(f"./playground/{title}.png")
+        plt.show()
+
+    @staticmethod
+    def _move_to_plus(left_heel, left_hip, left_toe, right_heel, right_hip, right_toe):
+        min_value = abs(min([min(right_heel),
+                             min(right_toe),
+                             min(left_heel),
+                             min(left_toe),
+                             min(right_hip),
+                             min(left_hip)]))
+        right_heel = right_heel + min_value
+        left_heel = left_heel + min_value
+        right_toe = right_toe + min_value
+        left_toe = left_toe + min_value
+        right_hip = right_hip + min_value
+        left_hip = left_hip + min_value
+
+        return left_heel, left_toe, right_heel, right_toe, right_hip, left_hip
+
     #   gaitalytics.c3d.sort_events(acq)
 
     def _create_events(self, acq, diff, event_label: gaitalytics.utils.GaitEventLabel,
                        event_context: gaitalytics.utils.GaitEventContext,
                        min_distance: int = 100,
                        show_plot: bool = False):
-        data = diff[:, gaitalytics.utils.AxesNames.y.value]
+        data = diff
         if gaitalytics.c3d.is_progression_axes_flip(
                 acq.GetPoint(self._config.MARKER_MAPPING.left_heel.value).GetValues(),
                 acq.GetPoint(self._config.MARKER_MAPPING.left_meta_5.value).GetValues()):
             data = data * -1
-        data = gaitalytics.utils.min_max_norm(data)
 
-        if gaitalytics.utils.GaitEventLabel.FOOT_STRIKE == event_label:
-            data = [entry * -1 for entry in data]
+        data = gaitalytics.utils.min_max_norm(data)
 
         extremes, foo = signal.find_peaks(data, height=[0, 1], distance=min_distance)
-        if show_plot:
-            plt.plot(data)
-            for i in extremes:
-                plt.plot(i, data[i], 'ro')
-            plt.plot()
-            plt.show()
 
         for frame in extremes:
             acq.AppendEvent(self._create_event(acq, frame, event_label, event_context))
 
 
 class ForcePlateEventDetection(AbstractGaitEventDetector):
     """
```

### Comparing `gaitalytics-0.1.3b0/src/gaitalytics/plot.py` & `gaitalytics-0.1.4b0/src/gaitalytics/plot.py`

 * *Files identical despite different names*

### Comparing `gaitalytics-0.1.3b0/src/gaitalytics/utils.py` & `gaitalytics-0.1.4b0/src/gaitalytics/utils.py`

 * *Files identical despite different names*

### Comparing `gaitalytics-0.1.3b0/src/gaitalytics.egg-info/PKG-INFO` & `gaitalytics-0.1.4b0/src/gaitalytics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaitalytics
-Version: 0.1.3b0
+Version: 0.1.4b0
 Summary: Library to analyse gait data captured with a mocap system
 Home-page: https://github.com/cereneo-foundation/gaitalytics
 Author: André Böni
 Author-email: andre.boeni@cereneo.foundation
 License: MIT
 Keywords: gait,analysis,c3d,mocap
 Classifier: Programming Language :: Python :: 3
```

