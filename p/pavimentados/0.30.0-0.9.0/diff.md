# Comparing `tmp/pavimentados-0.30.0.tar.gz` & `tmp/pavimentados-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pavimentados-0.30.0.tar", last modified: Sun Jul 30 21:19:07 2023, max compression
+gzip compressed data, was "dist\pavimentados-0.9.0.tar", last modified: Thu Feb  3 16:35:21 2022, max compression
```

## Comparing `pavimentados-0.30.0.tar` & `pavimentados-0.9.0.tar`

### file list

```diff
@@ -1,42 +1,44 @@
-drwxr-xr-x   0 vdurand  (644026607) 1010544492        0 2023-07-30 21:19:07.909931 pavimentados-0.30.0/
--rw-r--r--   0 vdurand  (644026607) 1010544492    11839 2023-03-28 19:27:29.000000 pavimentados-0.30.0/LICENSE.md
--rw-r--r--   0 vdurand  (644026607) 1010544492      292 2023-03-28 19:27:29.000000 pavimentados-0.30.0/MANIFEST.in
--rw-r--r--   0 vdurand  (644026607) 1010544492     6842 2023-07-30 21:19:07.909783 pavimentados-0.30.0/PKG-INFO
--rw-r--r--   0 vdurand  (644026607) 1010544492     6161 2023-03-28 19:27:29.000000 pavimentados-0.30.0/README.md
-drwxr-xr-x   0 vdurand  (644026607) 1010544492        0 2023-07-30 21:19:07.904268 pavimentados-0.30.0/pavimentados/
--rw-r--r--   0 vdurand  (644026607) 1010544492      265 2023-07-29 23:03:25.000000 pavimentados-0.30.0/pavimentados/__init__.py
-drwxr-xr-x   0 vdurand  (644026607) 1010544492        0 2023-07-30 21:19:07.905939 pavimentados-0.30.0/pavimentados/analyzers/
--rw-r--r--   0 vdurand  (644026607) 1010544492        0 2023-03-28 19:27:29.000000 pavimentados-0.30.0/pavimentados/analyzers/__init__.py
--rw-r--r--   0 vdurand  (644026607) 1010544492    10145 2023-07-29 23:03:25.000000 pavimentados-0.30.0/pavimentados/analyzers/calculators.py
--rw-r--r--   0 vdurand  (644026607) 1010544492     8009 2023-07-30 21:13:16.000000 pavimentados-0.30.0/pavimentados/analyzers/gps_sources.py
--rw-r--r--   0 vdurand  (644026607) 1010544492     3338 2023-07-29 23:03:25.000000 pavimentados-0.30.0/pavimentados/analyzers/utils.py
-drwxr-xr-x   0 vdurand  (644026607) 1010544492        0 2023-07-30 21:19:07.907693 pavimentados-0.30.0/pavimentados/configs/
--rw-r--r--   0 vdurand  (644026607) 1010544492        0 2023-03-28 19:27:29.000000 pavimentados-0.30.0/pavimentados/configs/__init__.py
--rw-r--r--   0 vdurand  (644026607) 1010544492       43 2023-03-28 19:27:29.000000 pavimentados-0.30.0/pavimentados/configs/images_processor.json
--rw-r--r--   0 vdurand  (644026607) 1010544492       38 2023-03-28 19:27:29.000000 pavimentados-0.30.0/pavimentados/configs/models_general.json
--rw-r--r--   0 vdurand  (644026607) 1010544492      406 2023-03-28 19:27:29.000000 pavimentados-0.30.0/pavimentados/configs/processor.json
--rw-r--r--   0 vdurand  (644026607) 1010544492      429 2023-03-28 19:27:29.000000 pavimentados-0.30.0/pavimentados/configs/siamese_config.json
--rw-r--r--   0 vdurand  (644026607) 1010544492       53 2023-03-28 19:27:29.000000 pavimentados-0.30.0/pavimentados/configs/state_signal_config.json
--rw-r--r--   0 vdurand  (644026607) 1010544492      201 2023-07-29 23:03:25.000000 pavimentados-0.30.0/pavimentados/configs/utils.py
--rw-r--r--   0 vdurand  (644026607) 1010544492      424 2023-03-28 19:27:29.000000 pavimentados-0.30.0/pavimentados/configs/yolo_config.json
--rw-r--r--   0 vdurand  (644026607) 1010544492     3966 2023-07-29 23:03:25.000000 pavimentados-0.30.0/pavimentados/downloader.py
-drwxr-xr-x   0 vdurand  (644026607) 1010544492        0 2023-07-30 21:19:07.908028 pavimentados-0.30.0/pavimentados/image/
--rw-r--r--   0 vdurand  (644026607) 1010544492        0 2023-03-28 19:27:29.000000 pavimentados-0.30.0/pavimentados/image/__init__.py
--rw-r--r--   0 vdurand  (644026607) 1010544492      259 2023-07-29 23:03:25.000000 pavimentados-0.30.0/pavimentados/image/utils.py
-drwxr-xr-x   0 vdurand  (644026607) 1010544492        0 2023-07-30 21:19:07.908566 pavimentados-0.30.0/pavimentados/models/
--rw-r--r--   0 vdurand  (644026607) 1010544492        0 2023-03-28 19:27:29.000000 pavimentados-0.30.0/pavimentados/models/__init__.py
--rw-r--r--   0 vdurand  (644026607) 1010544492    12899 2023-07-29 23:03:25.000000 pavimentados-0.30.0/pavimentados/models/structures.py
--rw-r--r--   0 vdurand  (644026607) 1010544492    16060 2023-07-29 23:03:25.000000 pavimentados-0.30.0/pavimentados/models/yolo.py
-drwxr-xr-x   0 vdurand  (644026607) 1010544492        0 2023-07-30 21:19:07.909533 pavimentados-0.30.0/pavimentados/processing/
--rw-r--r--   0 vdurand  (644026607) 1010544492        0 2023-03-28 19:27:29.000000 pavimentados-0.30.0/pavimentados/processing/__init__.py
--rw-r--r--   0 vdurand  (644026607) 1010544492    10333 2023-07-29 23:03:25.000000 pavimentados-0.30.0/pavimentados/processing/processors.py
--rw-r--r--   0 vdurand  (644026607) 1010544492     4051 2023-07-29 23:03:25.000000 pavimentados-0.30.0/pavimentados/processing/sources.py
--rw-r--r--   0 vdurand  (644026607) 1010544492     3451 2023-07-29 23:03:25.000000 pavimentados-0.30.0/pavimentados/processing/workflows.py
-drwxr-xr-x   0 vdurand  (644026607) 1010544492        0 2023-07-30 21:19:07.905202 pavimentados-0.30.0/pavimentados.egg-info/
--rw-r--r--   0 vdurand  (644026607) 1010544492     6842 2023-07-30 21:19:07.000000 pavimentados-0.30.0/pavimentados.egg-info/PKG-INFO
--rw-r--r--   0 vdurand  (644026607) 1010544492     1022 2023-07-30 21:19:07.000000 pavimentados-0.30.0/pavimentados.egg-info/SOURCES.txt
--rw-r--r--   0 vdurand  (644026607) 1010544492        1 2023-07-30 21:19:07.000000 pavimentados-0.30.0/pavimentados.egg-info/dependency_links.txt
--rw-r--r--   0 vdurand  (644026607) 1010544492      151 2023-07-30 21:19:07.000000 pavimentados-0.30.0/pavimentados.egg-info/requires.txt
--rw-r--r--   0 vdurand  (644026607) 1010544492       13 2023-07-30 21:19:07.000000 pavimentados-0.30.0/pavimentados.egg-info/top_level.txt
--rw-r--r--   0 vdurand  (644026607) 1010544492       38 2023-07-30 21:19:07.909993 pavimentados-0.30.0/setup.cfg
--rw-r--r--   0 vdurand  (644026607) 1010544492     1357 2023-07-29 23:08:27.000000 pavimentados-0.30.0/setup.py
+drwxrwxrwx   0        0        0        0 2022-02-03 16:35:21.000000 pavimentados-0.9.0/
+-rw-rw-rw-   0        0        0     1928 2022-01-12 04:50:35.000000 pavimentados-0.9.0/.gitignore
+-rw-rw-rw-   0        0        0     7169 2022-01-12 04:50:35.000000 pavimentados-0.9.0/LICENSE
+-rw-rw-rw-   0        0        0      297 2022-01-12 05:36:36.000000 pavimentados-0.9.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2264 2022-02-03 16:35:21.000000 pavimentados-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1349 2022-02-03 15:40:33.000000 pavimentados-0.9.0/README.md
+drwxrwxrwx   0        0        0        0 2022-02-03 16:35:21.000000 pavimentados-0.9.0/pavimentados/
+-rw-rw-rw-   0        0        0      250 2022-01-12 06:27:39.000000 pavimentados-0.9.0/pavimentados/__init__.py
+drwxrwxrwx   0        0        0        0 2022-02-03 16:35:21.000000 pavimentados-0.9.0/pavimentados/analyzers/
+-rw-rw-rw-   0        0        0        0 2022-01-12 04:54:02.000000 pavimentados-0.9.0/pavimentados/analyzers/__init__.py
+-rw-rw-rw-   0        0        0     8242 2022-01-12 05:31:21.000000 pavimentados-0.9.0/pavimentados/analyzers/calculators.py
+-rw-rw-rw-   0        0        0     6785 2022-01-12 05:31:21.000000 pavimentados-0.9.0/pavimentados/analyzers/gps_sources.py
+-rw-rw-rw-   0        0        0     3011 2022-01-12 01:57:29.000000 pavimentados-0.9.0/pavimentados/analyzers/utils.py
+drwxrwxrwx   0        0        0        0 2022-02-03 16:35:21.000000 pavimentados-0.9.0/pavimentados/configs/
+-rw-rw-rw-   0        0        0        0 2022-01-12 04:53:49.000000 pavimentados-0.9.0/pavimentados/configs/__init__.py
+-rw-rw-rw-   0        0        0       45 2022-01-10 07:47:23.000000 pavimentados-0.9.0/pavimentados/configs/images_processor.json
+-rw-rw-rw-   0        0        0       40 2022-01-10 04:01:55.000000 pavimentados-0.9.0/pavimentados/configs/models_general.json
+-rw-rw-rw-   0        0        0      440 2022-01-10 04:58:59.000000 pavimentados-0.9.0/pavimentados/configs/processor.json
+-rw-rw-rw-   0        0        0      442 2022-01-10 03:40:03.000000 pavimentados-0.9.0/pavimentados/configs/siamese_config.json
+-rw-rw-rw-   0        0        0       56 2022-01-10 03:19:31.000000 pavimentados-0.9.0/pavimentados/configs/state_signal_config.json
+-rw-rw-rw-   0        0        0      186 2022-01-10 16:07:40.000000 pavimentados-0.9.0/pavimentados/configs/utils.py
+-rw-rw-rw-   0        0        0      439 2022-01-10 05:31:47.000000 pavimentados-0.9.0/pavimentados/configs/yolo_config.json
+-rw-rw-rw-   0        0        0     3358 2022-01-12 06:46:32.000000 pavimentados-0.9.0/pavimentados/downloader.py
+drwxrwxrwx   0        0        0        0 2022-02-03 16:35:21.000000 pavimentados-0.9.0/pavimentados/image/
+-rw-rw-rw-   0        0        0        0 2022-01-12 04:53:38.000000 pavimentados-0.9.0/pavimentados/image/__init__.py
+-rw-rw-rw-   0        0        0      245 2022-01-10 07:53:24.000000 pavimentados-0.9.0/pavimentados/image/utils.py
+drwxrwxrwx   0        0        0        0 2022-02-03 16:35:21.000000 pavimentados-0.9.0/pavimentados/models/
+-rw-rw-rw-   0        0        0        0 2022-01-12 04:53:27.000000 pavimentados-0.9.0/pavimentados/models/__init__.py
+-rw-rw-rw-   0        0        0    10292 2022-01-12 05:34:06.000000 pavimentados-0.9.0/pavimentados/models/structures.py
+-rw-rw-rw-   0        0        0    16632 2022-01-12 06:12:03.000000 pavimentados-0.9.0/pavimentados/models/yolo.py
+drwxrwxrwx   0        0        0        0 2022-02-03 16:35:21.000000 pavimentados-0.9.0/pavimentados/processing/
+-rw-rw-rw-   0        0        0        0 2022-01-12 04:53:16.000000 pavimentados-0.9.0/pavimentados/processing/__init__.py
+-rw-rw-rw-   0        0        0     7287 2022-01-12 05:31:22.000000 pavimentados-0.9.0/pavimentados/processing/processors.py
+-rw-rw-rw-   0        0        0     2714 2022-01-12 05:34:06.000000 pavimentados-0.9.0/pavimentados/processing/sources.py
+-rw-rw-rw-   0        0        0     2893 2022-01-12 05:31:22.000000 pavimentados-0.9.0/pavimentados/processing/workflows.py
+drwxrwxrwx   0        0        0        0 2022-02-03 16:35:21.000000 pavimentados-0.9.0/pavimentados.egg-info/
+-rw-rw-rw-   0        0        0     2264 2022-02-03 16:35:18.000000 pavimentados-0.9.0/pavimentados.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1047 2022-02-03 16:35:21.000000 pavimentados-0.9.0/pavimentados.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-02-03 16:35:18.000000 pavimentados-0.9.0/pavimentados.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      173 2022-02-03 16:35:18.000000 pavimentados-0.9.0/pavimentados.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2022-02-03 16:35:20.000000 pavimentados-0.9.0/pavimentados.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      182 2022-01-12 06:22:23.000000 pavimentados-0.9.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2022-02-03 16:35:21.000000 pavimentados-0.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     1463 2022-01-12 06:46:36.000000 pavimentados-0.9.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `pavimentados-0.30.0/pavimentados/analyzers/utils.py` & `pavimentados-0.9.0/pavimentados/analyzers/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,114 +1,108 @@
-import numpy as np
-import pandas as pd
-
-
-def total_distance(lat1, lon1, lat2, lon2):
-    """
-    Calcula la distancia entre dos puntos (lat1, lon1) y (lat2, lon2).
-    """
-
-    R = 6373.0  # approximate radius of earth in km.
-
-    lat1 = np.radians(lat1)
-    lon1 = np.radians(lon1)
-    lat2 = np.radians(lat2)
-    lon2 = np.radians(lon2)
-
-    dlon = lon2 - lon1
-    dlat = lat2 - lat1
-
-    a = np.sin(dlat / 2) ** 2 + np.cos(lat1) * np.cos(lat2) * np.sin(dlon / 2) ** 2
-    c = 2 * np.arctan2(np.sqrt(a), np.sqrt(1 - a))
-
-    distance = R * c * 1000
-    return distance
-
-
-def area_calc(boxes, altura, base):
-    """
-    Calcula el area de la caja.
-    """
-    if len(boxes) > 0:
-        return ((boxes[2] - boxes[0]) * altura) * ((boxes[3] - boxes[1]) * base)
-    else:
-        return 0
-
-
-def box_center(boxes, altura, base):
-    """
-    Calcula el centro de la caja.
-    """
-    if len(boxes) > 0:
-        return (((boxes[3] + boxes[1]) / 2) * base), (((boxes[2] + boxes[0]) / 2) * altura)
-    else:
-        return None, None
-
-
-def box_height(boxes, altura):
-    """
-    Calcula la altura de la caja.
-    """
-    if len(boxes) > 0:
-        return (boxes[2] - boxes[0]) * altura
-    else:
-        return None
-
-
-def box_width(boxes, base):
-    """
-    Calcula la base de la caja.
-    """
-    if len(boxes) > 0:
-        return (boxes[3] - boxes[1]) * base
-    else:
-        return None
-
-
-def fail_id_generator(df, min_photogram_distance):
-    """
-    Genera un ID de fail. Esto se realiza ya que cada fail es detectada en
-    fotogramas simultaneos y es necesario identificarla como una misma fail.
-    """
-
-    df_id_fails = []
-    id_fail = 0
-    for fail in list(df.classes.unique()):
-        df_fail = df.loc[df.classes == fail].copy().reset_index(drop=True)
-        fotogramas = df_fail.fotograma
-        id_section_fail = [id_fail]
-        for i in range(len(fotogramas) - 1):
-            if (fotogramas[i + 1] - fotogramas[i]) > min_photogram_distance:
-                id_fail += 1
-            id_section_fail.append(id_fail)
-        id_section_fail = np.array(id_section_fail)
-        if len(id_section_fail) > 0:
-            df_fail["fail_id_section"] = id_section_fail
-            df_id_fails.append(df_fail)
-    df = pd.concat(df_id_fails).sort_values(["fotograma", "classes", "fail_id_section"]).reset_index(drop=True)
-    return df
-
-
-def stack_columns_dataset(df, variables, static_variables):
-    df["ind"] = df.index
-    df_resulting = df[static_variables].copy()
-    c = 0
-    for v in variables:
-        d = pd.DataFrame([[i, t] for i, T in df[["ind", v]].values for t in T], columns=["ind", v])
-        d["ind2"] = d.index
-        if c == 0:
-            df_resulting = pd.merge(df_resulting, d, on="ind", how="left")
-            c += 1
-        else:
-            df_resulting = pd.merge(df_resulting, d, on=["ind", "ind2"], how="left")
-    return df_resulting
-
-
-def assign_group_calculations(df):
-    df["area"] = df.width.values * df.distances.values
-    df["start_coordinate"] = list(map(lambda x, y: (x, y), df.latitude.values, df.longitude.values))
-    df["end_coordenate"] = list(map(lambda x, y: (x, y), df.latitude.values, df.longitude.values))
-    df["start_latitude"] = df.latitude
-    df["end_latitude"] = df.latitude
-    df["start_longitude"] = df.longitude
-    df["end_longitude"] = df.longitude
-    return df
+import numpy as np
+import pandas as pd
+
+def total_distance(lat1,lon1,lat2,lon2):
+	"""
+	Calcula la distancia entre dos puntos (lat1, lon1) y (lat2, lon2).
+	"""
+
+	R = 6373.0 # approximate radius of earth in km.
+
+	lat1 = np.radians(lat1)
+	lon1 = np.radians(lon1)
+	lat2 = np.radians(lat2)
+	lon2 = np.radians(lon2)
+
+	dlon = lon2 - lon1
+	dlat = lat2 - lat1
+
+	a = np.sin(dlat / 2)**2 + np.cos(lat1) * np.cos(lat2) * np.sin(dlon / 2)**2
+	c = 2 * np.arctan2(np.sqrt(a), np.sqrt(1 - a))
+
+	distance = R * c*1000
+	return distance
+
+def area_calc(boxes,altura, base):
+	"""
+	Calcula el area de la caja.
+	"""
+	if len(boxes)>0:
+		return ((boxes[2]-boxes[0])*altura)*((boxes[3]-boxes[1])*base)
+	else:
+		return 0
+
+def box_center(boxes, altura, base):
+	"""
+	Calcula el centro de la caja.
+	"""
+	if len(boxes)>0:
+		return (((boxes[3]+boxes[1])/2)*base),(((boxes[2]+boxes[0])/2)*altura)
+	else:
+		return None,None
+
+def box_height(boxes,altura):
+	"""
+	Calcula la altura de la caja.
+	"""
+	if len(boxes)>0:
+		return ((boxes[2]-boxes[0])*altura)
+	else:
+		return None
+
+
+def box_width(boxes,base):
+	"""
+	Calcula la base de la caja.
+	"""
+	if len(boxes)>0:
+		return ((boxes[3]-boxes[1])*base)	
+	else:
+		return None
+
+
+def fail_id_generator(df, min_photogram_distance):
+	"""
+	Genera un ID de fail. Esto se realiza ya que cada fail es detectada en 
+	fotogramas simultaneos y es necesario identificarla como una misma fail.
+	"""
+
+	df_id_fails = []
+	id_fail = 0
+	for fail in list(df.classes.unique()):
+		df_fail = df.loc[df.classes==fail].copy().reset_index(drop=True)
+		fotogramas = df_fail.fotograma
+		id_section_fail = [id_fail]
+		for i in range(len(fotogramas)-1):
+			if (fotogramas[i+1]-fotogramas[i])>min_photogram_distance:
+				id_fail +=1
+			id_section_fail.append(id_fail)
+		id_section_fail = np.array(id_section_fail)
+		if len(id_section_fail)>0:
+			df_fail['fail_id_section'] = id_section_fail
+			df_id_fails.append(df_fail)
+	df = pd.concat(df_id_fails).sort_values(['fotograma','classes','fail_id_section']).reset_index(drop=True)
+	return df
+
+def stack_columns_dataset(df, variables, static_variables):
+	df['ind'] = df.index 
+	df_resulting = df[static_variables].copy()
+	c = 0
+	for v in variables:
+		d = pd.DataFrame([[i,t] for  i,T in df[['ind',v]].values for t in T], columns=['ind',v])
+		d['ind2'] = d.index
+		if c==0:
+			df_resulting = pd.merge(df_resulting,d, on='ind', how='left')
+			c+=1
+		else:
+			df_resulting = pd.merge(df_resulting,d, on=['ind','ind2'], how='left')
+	return df_resulting	
+
+def assign_group_calculations(df):
+	df['area'] = df.width.values*df.distances.values
+	df['start_coordinate'] = list(map(lambda x,y: (x,y), df.latitude.values, df.longitude.values))
+	df['end_coordenate'] = list(map(lambda x,y: (x,y), df.latitude.values, df.longitude.values))
+	df['start_latitude'] = df.latitude
+	df['end_latitude'] = df.latitude
+	df['start_longitude'] = df.longitude
+	df['end_longitude'] = df.longitude
+	return df
```

### Comparing `pavimentados-0.30.0/pavimentados/models/yolo.py` & `pavimentados-0.9.0/pavimentados/models/yolo.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,77 +1,81 @@
-import cv2
 import numpy as np
 import tensorflow as tf
 from absl import logging
+import cv2
 
 YOLOV3_LAYER_LIST = [
-    "yolo_darknet",
-    "yolo_conv_0",
-    "yolo_output_0",
-    "yolo_conv_1",
-    "yolo_output_1",
-    "yolo_conv_2",
-    "yolo_output_2",
+    'yolo_darknet',
+    'yolo_conv_0',
+    'yolo_output_0',
+    'yolo_conv_1',
+    'yolo_output_1',
+    'yolo_conv_2',
+    'yolo_output_2',
 ]
 
 YOLOV3_TINY_LAYER_LIST = [
-    "yolo_darknet",
-    "yolo_conv_0",
-    "yolo_output_0",
-    "yolo_conv_1",
-    "yolo_output_1",
+    'yolo_darknet',
+    'yolo_conv_0',
+    'yolo_output_0',
+    'yolo_conv_1',
+    'yolo_output_1',
 ]
 
 
 def load_darknet_weights(model, weights_file, tiny=False):
-    wf = open(weights_file, "rb")
+    wf = open(weights_file, 'rb')
     major, minor, revision, seen, _ = np.fromfile(wf, dtype=np.int32, count=5)
 
     if tiny:
         layers = YOLOV3_TINY_LAYER_LIST
     else:
         layers = YOLOV3_LAYER_LIST
 
     for layer_name in layers:
         sub_model = model.get_layer(layer_name)
         for i, layer in enumerate(sub_model.layers):
-            if not layer.name.startswith("conv2d"):
+            if not layer.name.startswith('conv2d'):
                 continue
             batch_norm = None
-            if i + 1 < len(sub_model.layers) and sub_model.layers[i + 1].name.startswith("batch_norm"):
+            if i + 1 < len(sub_model.layers) and \
+                    sub_model.layers[i + 1].name.startswith('batch_norm'):
                 batch_norm = sub_model.layers[i + 1]
 
-            logging.info("{}/{} {}".format(sub_model.name, layer.name, "bn" if batch_norm else "bias"))
+            logging.info("{}/{} {}".format(
+                sub_model.name, layer.name, 'bn' if batch_norm else 'bias'))
 
             filters = layer.filters
             size = layer.kernel_size[0]
             in_dim = layer.input_shape[-1]
 
             if batch_norm is None:
                 conv_bias = np.fromfile(wf, dtype=np.float32, count=filters)
             else:
                 # darknet [beta, gamma, mean, variance]
-                bn_weights = np.fromfile(wf, dtype=np.float32, count=4 * filters)
+                bn_weights = np.fromfile(
+                    wf, dtype=np.float32, count=4 * filters)
                 # tf [gamma, beta, mean, variance]
                 bn_weights = bn_weights.reshape((4, filters))[[1, 0, 2, 3]]
 
             # darknet shape (out_dim, in_dim, height, width)
             conv_shape = (filters, in_dim, size, size)
-            conv_weights = np.fromfile(wf, dtype=np.float32, count=np.product(conv_shape))
+            conv_weights = np.fromfile(
+                wf, dtype=np.float32, count=np.product(conv_shape))
             # tf shape (height, width, in_dim, out_dim)
-            conv_weights = conv_weights.reshape(conv_shape).transpose([2, 3, 1, 0])
+            conv_weights = conv_weights.reshape(
+                conv_shape).transpose([2, 3, 1, 0])
 
             if batch_norm is None:
                 layer.set_weights([conv_weights, conv_bias])
             else:
                 layer.set_weights([conv_weights])
                 batch_norm.set_weights(bn_weights)
 
-    if len(wf.read()) == 0:
-        raise AssertionError("failed to read all data")
+    assert len(wf.read()) == 0, 'failed to read all data'
     wf.close()
 
 
 def broadcast_iou(box_1, box_2):
     # box_1: (..., (x1, y1, x2, y2))
     # box_2: (N, (x1, y1, x2, y2))
 
@@ -79,19 +83,23 @@
     box_1 = tf.expand_dims(box_1, -2)
     box_2 = tf.expand_dims(box_2, 0)
     # new_shape: (..., N, (x1, y1, x2, y2))
     new_shape = tf.broadcast_dynamic_shape(tf.shape(box_1), tf.shape(box_2))
     box_1 = tf.broadcast_to(box_1, new_shape)
     box_2 = tf.broadcast_to(box_2, new_shape)
 
-    int_w = tf.maximum(tf.minimum(box_1[..., 2], box_2[..., 2]) - tf.maximum(box_1[..., 0], box_2[..., 0]), 0)
-    int_h = tf.maximum(tf.minimum(box_1[..., 3], box_2[..., 3]) - tf.maximum(box_1[..., 1], box_2[..., 1]), 0)
+    int_w = tf.maximum(tf.minimum(box_1[..., 2], box_2[..., 2]) -
+                       tf.maximum(box_1[..., 0], box_2[..., 0]), 0)
+    int_h = tf.maximum(tf.minimum(box_1[..., 3], box_2[..., 3]) -
+                       tf.maximum(box_1[..., 1], box_2[..., 1]), 0)
     int_area = int_w * int_h
-    box_1_area = (box_1[..., 2] - box_1[..., 0]) * (box_1[..., 3] - box_1[..., 1])
-    box_2_area = (box_2[..., 2] - box_2[..., 0]) * (box_2[..., 3] - box_2[..., 1])
+    box_1_area = (box_1[..., 2] - box_1[..., 0]) * \
+        (box_1[..., 3] - box_1[..., 1])
+    box_2_area = (box_2[..., 2] - box_2[..., 0]) * \
+        (box_2[..., 3] - box_2[..., 1])
     return int_area / (box_1_area + box_2_area - int_area)
 
 
 def draw_outputs(img, outputs, class_names):
     boxes, objectness, classes, nums = outputs
     boxes, objectness, classes, nums = boxes[0], objectness[0], classes[0], nums[0]
     wh = np.flip(img.shape[0:2])
@@ -110,52 +118,56 @@
     boxes, classes = tf.split(y, (4, 1), axis=-1)
     classes = classes[..., 0]
     wh = np.flip(img.shape[0:2])
     for i in range(len(boxes)):
         x1y1 = tuple((np.array(boxes[i][0:2]) * wh).astype(np.int32))
         x2y2 = tuple((np.array(boxes[i][2:4]) * wh).astype(np.int32))
         img = cv2.rectangle(img, x1y1, x2y2, (255, 0, 0), 2)
-        img = cv2.putText(img, class_names[classes[i]], x1y1, cv2.FONT_HERSHEY_COMPLEX_SMALL, 1, (0, 0, 255), 2)
+        img = cv2.putText(img, class_names[classes[i]],
+                          x1y1, cv2.FONT_HERSHEY_COMPLEX_SMALL,
+                          1, (0, 0, 255), 2)
     return img
 
 
 def freeze_all(model, frozen=True):
     model.trainable = not frozen
     if isinstance(model, tf.keras.models.Model):
-        for layer in model.layers:
-            freeze_all(layer, frozen)
+        for l in model.layers:
+            freeze_all(l, frozen)
+
+
+
 
 
-# PARAMETROS
-yolo_max_boxes = 100  # maximum number of boxes per image.
-yolo_iou_threshold = 0.1  # iou threshold.
-yolo_score_threshold = 0.1  # score threshold.
-#
+############## PARAMETROS
+yolo_max_boxes = 100 # maximum number of boxes per image.
+yolo_iou_threshold = 0.1# iou threshold.
+yolo_score_threshold = 0.1 # score threshold.
+#########################
 
-yolo_anchors = np.array([(10, 13), (16, 30), (33, 23), (30, 61), (62, 45), (59, 119), (116, 90), (156, 198), (373, 326)], np.float32) / 416
+yolo_anchors = np.array([(10, 13), (16, 30), (33, 23), (30, 61), (62, 45),
+                         (59, 119), (116, 90), (156, 198), (373, 326)],
+                        np.float32) / 416
 yolo_anchor_masks = np.array([[6, 7, 8], [3, 4, 5], [0, 1, 2]])
 
-yolo_tiny_anchors = np.array([(10, 14), (23, 27), (37, 58), (81, 82), (135, 169), (344, 319)], np.float32) / 416
+yolo_tiny_anchors = np.array([(10, 14), (23, 27), (37, 58),
+                              (81, 82), (135, 169),  (344, 319)],
+                             np.float32) / 416
 yolo_tiny_anchor_masks = np.array([[3, 4, 5], [0, 1, 2]])
 
 
 def DarknetConv(x, filters, size, strides=1, batch_norm=True):
     if strides == 1:
-        padding = "same"
+        padding = 'same'
     else:
         x = tf.keras.layers.ZeroPadding2D(((1, 0), (1, 0)))(x)  # top left half-padding
-        padding = "valid"
-    x = tf.keras.layers.Conv2D(
-        filters=filters,
-        kernel_size=size,
-        strides=strides,
-        padding=padding,
-        use_bias=not batch_norm,
-        kernel_regularizer=tf.keras.regularizers.l2(0.0005),
-    )(x)
+        padding = 'valid'
+    x = tf.keras.layers.Conv2D(filters=filters, kernel_size=size,
+               strides=strides, padding=padding,
+               use_bias=not batch_norm, kernel_regularizer=tf.keras.regularizers.l2(0.0005))(x)
     if batch_norm:
         x = tf.keras.layers.BatchNormalization()(x)
         x = tf.keras.layers.LeakyReLU(alpha=0.1)(x)
     return x
 
 
 def DarknetResidual(x, filters):
@@ -183,25 +195,25 @@
     x = DarknetBlock(x, 1024, 4)
     return tf.keras.models.Model(inputs, (x_36, x_61, x), name=name)
 
 
 def DarknetTiny(name=None):
     x = inputs = tf.keras.layers.Input([None, None, 3])
     x = DarknetConv(x, 16, 3)
-    x = tf.keras.layers.MaxPool2D(2, 2, "same")(x)
+    x = tf.keras.layers.MaxPool2D(2, 2, 'same')(x)
     x = DarknetConv(x, 32, 3)
-    x = tf.keras.layers.MaxPool2D(2, 2, "same")(x)
+    x = tf.keras.layers.MaxPool2D(2, 2, 'same')(x)
     x = DarknetConv(x, 64, 3)
-    x = tf.keras.layers.MaxPool2D(2, 2, "same")(x)
+    x = tf.keras.layers.MaxPool2D(2, 2, 'same')(x)
     x = DarknetConv(x, 128, 3)
-    x = tf.keras.layers.MaxPool2D(2, 2, "same")(x)
+    x = tf.keras.layers.MaxPool2D(2, 2, 'same')(x)
     x = x_8 = DarknetConv(x, 256, 3)  # skip connection
-    x = tf.keras.layers.MaxPool2D(2, 2, "same")(x)
+    x = tf.keras.layers.MaxPool2D(2, 2, 'same')(x)
     x = DarknetConv(x, 512, 3)
-    x = tf.keras.layers.MaxPool2D(2, 1, "same")(x)
+    x = tf.keras.layers.MaxPool2D(2, 1, 'same')(x)
     x = DarknetConv(x, 1024, 3)
     return tf.keras.models.Model(inputs, (x_8, x), name=name)
 
 
 def YoloConv(filters, name=None):
     def yolo_conv(x_in):
         if isinstance(x_in, tuple):
@@ -217,15 +229,14 @@
 
         x = DarknetConv(x, filters, 1)
         x = DarknetConv(x, filters * 2, 3)
         x = DarknetConv(x, filters, 1)
         x = DarknetConv(x, filters * 2, 3)
         x = DarknetConv(x, filters, 1)
         return tf.keras.models.Model(inputs, x, name=name)(x_in)
-
     return yolo_conv
 
 
 def YoloConvTiny(filters, name=None):
     def yolo_conv(x_in):
         if isinstance(x_in, tuple):
             inputs = tf.keras.layers.Input(x_in[0].shape[1:]), tf.keras.layers.Input(x_in[1].shape[1:])
@@ -236,44 +247,45 @@
             x = tf.keras.layers.UpSampling2D(2)(x)
             x = tf.keras.layers.Concatenate()([x, x_skip])
         else:
             x = inputs = tf.keras.layers.Input(x_in.shape[1:])
             x = DarknetConv(x, filters, 1)
 
         return tf.keras.Model(inputs, x, name=name)(x_in)
-
     return yolo_conv
 
 
 def YoloOutput(filters, anchors, classes, name=None):
     def yolo_output(x_in):
         x = inputs = tf.keras.layers.Input(x_in.shape[1:])
         x = DarknetConv(x, filters * 2, 3)
         x = DarknetConv(x, anchors * (classes + 5), 1, batch_norm=False)
-        x = tf.keras.layers.Lambda(lambda x: tf.reshape(x, (-1, tf.shape(x)[1], tf.shape(x)[2], anchors, classes + 5)))(x)
+        x = tf.keras.layers.Lambda(lambda x: tf.reshape(x, (-1, tf.shape(x)[1], tf.shape(x)[2],
+                                            anchors, classes + 5)))(x)
         return tf.keras.models.Model(inputs, x, name=name)(x_in)
-
     return yolo_output
 
 
 def yolo_boxes(pred, anchors, classes):
     # pred: (batch_size, grid, grid, anchors, (x, y, w, h, obj, ...classes))
     grid_size = tf.shape(pred)[1]
-    box_xy, box_wh, objectness, class_probs = tf.split(pred, (2, 2, 1, classes), axis=-1)
+    box_xy, box_wh, objectness, class_probs = tf.split(
+        pred, (2, 2, 1, classes), axis=-1)
 
     box_xy = tf.sigmoid(box_xy)
     objectness = tf.sigmoid(objectness)
     class_probs = tf.sigmoid(class_probs)
     pred_box = tf.concat((box_xy, box_wh), axis=-1)  # original xywh for loss
 
     # !!! grid[x][y] == (y, x)
     grid = tf.meshgrid(tf.range(grid_size), tf.range(grid_size))
     grid = tf.expand_dims(tf.stack(grid, axis=-1), axis=2)  # [gx, gy, 1, 2]
 
-    box_xy = (box_xy + tf.cast(grid, tf.float32)) / tf.cast(grid_size, tf.float32)
+    box_xy = (box_xy + tf.cast(grid, tf.float32)) / \
+        tf.cast(grid_size, tf.float32)
     box_wh = tf.exp(box_wh) * anchors
 
     box_x1y1 = box_xy - box_wh / 2
     box_x2y2 = box_xy + box_wh / 2
     bbox = tf.concat([box_x1y1, box_x2y2], axis=-1)
 
     return bbox, objectness, class_probs, pred_box
@@ -291,121 +303,132 @@
     bbox = tf.concat(b, axis=1)
     confidence = tf.concat(c, axis=1)
     class_probs = tf.concat(t, axis=1)
 
     scores = confidence * class_probs
     boxes, scores, classes, valid_detections = tf.image.combined_non_max_suppression(
         boxes=tf.reshape(bbox, (tf.shape(bbox)[0], -1, 1, 4)),
-        scores=tf.reshape(scores, (tf.shape(scores)[0], -1, tf.shape(scores)[-1])),
+        scores=tf.reshape(
+            scores, (tf.shape(scores)[0], -1, tf.shape(scores)[-1])),
         max_output_size_per_class=yolo_max_boxes,
         max_total_size=yolo_max_boxes,
         iou_threshold=yolo_iou_threshold,
-        score_threshold=yolo_score_threshold,
+        score_threshold=yolo_score_threshold
     )
 
     return boxes, scores, classes, valid_detections
 
 
-def YoloV3(size=None, channels=3, anchors=yolo_anchors, masks=yolo_anchor_masks, classes=80, training=False, model_name="yolov3"):
-    x = inputs = tf.keras.layers.Input([size, size, channels], name="input")
+def YoloV3(size=None, channels=3, anchors=yolo_anchors,
+           masks=yolo_anchor_masks, classes=80, training=False, model_name = 'yolov3'):
+    x = inputs = tf.keras.layers.Input([size, size, channels], name='input')
 
-    x_36, x_61, x = Darknet(name="yolo_darknet")(x)
+    x_36, x_61, x = Darknet(name='yolo_darknet')(x)
 
-    x = YoloConv(512, name="yolo_conv_0")(x)
-    output_0 = YoloOutput(512, len(masks[0]), classes, name="yolo_output_0")(x)
+    x = YoloConv(512, name='yolo_conv_0')(x)
+    output_0 = YoloOutput(512, len(masks[0]), classes, name='yolo_output_0')(x)
 
-    x = YoloConv(256, name="yolo_conv_1")((x, x_61))
-    output_1 = YoloOutput(256, len(masks[1]), classes, name="yolo_output_1")(x)
+    x = YoloConv(256, name='yolo_conv_1')((x, x_61))
+    output_1 = YoloOutput(256, len(masks[1]), classes, name='yolo_output_1')(x)
 
-    x = YoloConv(128, name="yolo_conv_2")((x, x_36))
-    output_2 = YoloOutput(128, len(masks[2]), classes, name="yolo_output_2")(x)
+    x = YoloConv(128, name='yolo_conv_2')((x, x_36))
+    output_2 = YoloOutput(128, len(masks[2]), classes, name='yolo_output_2')(x)
 
     if training:
-        # todo: check this
-        return Model(inputs, (output_0, output_1, output_2), name=model_name)  # noqa: F821
+        return Model(inputs, (output_0, output_1, output_2), name=model_name)
 
-    boxes_0 = tf.keras.layers.Lambda(lambda x: yolo_boxes(x, anchors[masks[0]], classes), name="yolo_boxes_0")(output_0)
-    boxes_1 = tf.keras.layers.Lambda(lambda x: yolo_boxes(x, anchors[masks[1]], classes), name="yolo_boxes_1")(output_1)
-    boxes_2 = tf.keras.layers.Lambda(lambda x: yolo_boxes(x, anchors[masks[2]], classes), name="yolo_boxes_2")(output_2)
+    boxes_0 = tf.keras.layers.Lambda(lambda x: yolo_boxes(x, anchors[masks[0]], classes),
+                     name='yolo_boxes_0')(output_0)
+    boxes_1 = tf.keras.layers.Lambda(lambda x: yolo_boxes(x, anchors[masks[1]], classes),
+                     name='yolo_boxes_1')(output_1)
+    boxes_2 = tf.keras.layers.Lambda(lambda x: yolo_boxes(x, anchors[masks[2]], classes),
+                     name='yolo_boxes_2')(output_2)
 
-    outputs = tf.keras.layers.Lambda(lambda x: yolo_nms(x, anchors, masks, classes), name="yolo_nms")(
-        (boxes_0[:3], boxes_1[:3], boxes_2[:3])
-    )
+    outputs = tf.keras.layers.Lambda(lambda x: yolo_nms(x, anchors, masks, classes),
+                     name='yolo_nms')((boxes_0[:3], boxes_1[:3], boxes_2[:3]))
 
     return tf.keras.models.Model(inputs, outputs, name=model_name)
 
 
-def YoloV3Tiny(
-    size=None, channels=3, anchors=yolo_tiny_anchors, masks=yolo_tiny_anchor_masks, classes=80, training=False, model_name="yolov3_tiny"
-):
-    x = inputs = tf.keras.layers.Input([size, size, channels], name="input")
+def YoloV3Tiny(size=None, channels=3, anchors=yolo_tiny_anchors,
+               masks=yolo_tiny_anchor_masks, classes=80, training=False, model_name = 'yolov3_tiny'):
+    x = inputs = tf.keras.layers.Input([size, size, channels], name='input')
 
-    x_8, x = DarknetTiny(name="yolo_darknet")(x)
+    x_8, x = DarknetTiny(name='yolo_darknet')(x)
 
-    x = YoloConvTiny(256, name="yolo_conv_0")(x)
-    output_0 = YoloOutput(256, len(masks[0]), classes, name="yolo_output_0")(x)
+    x = YoloConvTiny(256, name='yolo_conv_0')(x)
+    output_0 = YoloOutput(256, len(masks[0]), classes, name='yolo_output_0')(x)
 
-    x = YoloConvTiny(128, name="yolo_conv_1")((x, x_8))
-    output_1 = YoloOutput(128, len(masks[1]), classes, name="yolo_output_1")(x)
+    x = YoloConvTiny(128, name='yolo_conv_1')((x, x_8))
+    output_1 = YoloOutput(128, len(masks[1]), classes, name='yolo_output_1')(x)
 
     if training:
-        # todo: check this
-        return Model(inputs, (output_0, output_1), name=model_name)  # noqa: F821
+        return Model(inputs, (output_0, output_1), name=model_name)
 
-    boxes_0 = tf.keras.layers.Lambda(lambda x: yolo_boxes(x, anchors[masks[0]], classes), name="yolo_boxes_0")(output_0)
-    boxes_1 = tf.keras.layers.Lambda(lambda x: yolo_boxes(x, anchors[masks[1]], classes), name="yolo_boxes_1")(output_1)
-    outputs = tf.keras.layers.Lambda(lambda x: yolo_nms(x, anchors, masks, classes), name="yolo_nms")((boxes_0[:3], boxes_1[:3]))
+    boxes_0 = tf.keras.layers.Lambda(lambda x: yolo_boxes(x, anchors[masks[0]], classes),
+                     name='yolo_boxes_0')(output_0)
+    boxes_1 = tf.keras.layers.Lambda(lambda x: yolo_boxes(x, anchors[masks[1]], classes),
+                     name='yolo_boxes_1')(output_1)
+    outputs = tf.keras.layers.Lambda(lambda x: yolo_nms(x, anchors, masks, classes),
+                     name='yolo_nms')((boxes_0[:3], boxes_1[:3]))
     return tf.keras.models.Model(inputs, outputs, name=model_name)
 
 
 def YoloLoss(anchors, classes=80, ignore_thresh=0.5):
     def yolo_loss(y_true, y_pred):
         # 1. transform all pred outputs
         # y_pred: (batch_size, grid, grid, anchors, (x, y, w, h, obj, ...cls))
-        pred_box, pred_obj, pred_class, pred_xywh = yolo_boxes(y_pred, anchors, classes)
+        pred_box, pred_obj, pred_class, pred_xywh = yolo_boxes(
+            y_pred, anchors, classes)
         pred_xy = pred_xywh[..., 0:2]
         pred_wh = pred_xywh[..., 2:4]
 
         # 2. transform all true outputs
         # y_true: (batch_size, grid, grid, anchors, (x1, y1, x2, y2, obj, cls))
-        true_box, true_obj, true_class_idx = tf.split(y_true, (4, 1, 1), axis=-1)
+        true_box, true_obj, true_class_idx = tf.split(
+            y_true, (4, 1, 1), axis=-1)
         true_xy = (true_box[..., 0:2] + true_box[..., 2:4]) / 2
         true_wh = true_box[..., 2:4] - true_box[..., 0:2]
 
         # give higher weights to small boxes
         box_loss_scale = 2 - true_wh[..., 0] * true_wh[..., 1]
 
         # 3. inverting the pred box equations
         grid_size = tf.shape(y_true)[1]
         grid = tf.meshgrid(tf.range(grid_size), tf.range(grid_size))
         grid = tf.expand_dims(tf.stack(grid, axis=-1), axis=2)
-        true_xy = true_xy * tf.cast(grid_size, tf.float32) - tf.cast(grid, tf.float32)
+        true_xy = true_xy * tf.cast(grid_size, tf.float32) - \
+            tf.cast(grid, tf.float32)
         true_wh = tf.math.log(true_wh / anchors)
-        true_wh = tf.where(tf.math.is_inf(true_wh), tf.zeros_like(true_wh), true_wh)
+        true_wh = tf.where(tf.math.is_inf(true_wh),
+                           tf.zeros_like(true_wh), true_wh)
 
         # 4. calculate all masks
         obj_mask = tf.squeeze(true_obj, -1)
         # ignore false positive when iou is over threshold
         best_iou = tf.map_fn(
-            lambda x: tf.reduce_max(broadcast_iou(x[0], tf.boolean_mask(x[1], tf.cast(x[2], tf.bool))), axis=-1),
+            lambda x: tf.reduce_max(broadcast_iou(x[0], tf.boolean_mask(
+                x[1], tf.cast(x[2], tf.bool))), axis=-1),
             (pred_box, true_box, obj_mask),
-            tf.float32,
-        )
+            tf.float32)
         ignore_mask = tf.cast(best_iou < ignore_thresh, tf.float32)
 
         # 5. calculate all losses
-        xy_loss = obj_mask * box_loss_scale * tf.reduce_sum(tf.square(true_xy - pred_xy), axis=-1)
-        wh_loss = obj_mask * box_loss_scale * tf.reduce_sum(tf.square(true_wh - pred_wh), axis=-1)
+        xy_loss = obj_mask * box_loss_scale * \
+            tf.reduce_sum(tf.square(true_xy - pred_xy), axis=-1)
+        wh_loss = obj_mask * box_loss_scale * \
+            tf.reduce_sum(tf.square(true_wh - pred_wh), axis=-1)
         obj_loss = tf.keras.losses.binary_crossentropy(true_obj, pred_obj)
-        obj_loss = obj_mask * obj_loss + (1 - obj_mask) * ignore_mask * obj_loss
+        obj_loss = obj_mask * obj_loss + \
+            (1 - obj_mask) * ignore_mask * obj_loss
         # TODO: use binary_crossentropy instead
-        class_loss = obj_mask * tf.keras.losses.sparse_categorical_crossentropy(true_class_idx, pred_class)
+        class_loss = obj_mask * tf.keras.losses.sparse_categorical_crossentropy(
+            true_class_idx, pred_class)
 
         # 6. sum over (batch, gridx, gridy, anchors) => (batch, 1)
         xy_loss = tf.reduce_sum(xy_loss, axis=(1, 2, 3))
         wh_loss = tf.reduce_sum(wh_loss, axis=(1, 2, 3))
         obj_loss = tf.reduce_sum(obj_loss, axis=(1, 2, 3))
         class_loss = tf.reduce_sum(class_loss, axis=(1, 2, 3))
 
         return xy_loss + wh_loss + obj_loss + class_loss
-
-    return yolo_loss
+    return yolo_loss
```

### Comparing `pavimentados-0.30.0/pavimentados.egg-info/SOURCES.txt` & `pavimentados-0.9.0/pavimentados.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
-LICENSE.md
+.gitignore
+LICENSE
 MANIFEST.in
 README.md
+requirements.txt
 setup.py
 pavimentados/__init__.py
 pavimentados/downloader.py
 pavimentados.egg-info/PKG-INFO
 pavimentados.egg-info/SOURCES.txt
 pavimentados.egg-info/dependency_links.txt
 pavimentados.egg-info/requires.txt
```

### Comparing `pavimentados-0.30.0/setup.py` & `pavimentados-0.9.0/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,39 +1,35 @@
-from pathlib import Path
-
-import pkg_resources
-from setuptools import find_packages, setup
-
-this_directory = Path(__file__).parent
-VERSION = "0.30.0"
-DESCRIPTION = (
-    "A python package Library which implement IA algorithims to detect cracks and failures on roads. "
-    "The package is wrapper around all the models and provides an interfaces to use them properly"
-)
-
-LONG_DESCRIPTION = (this_directory / "README.md").read_text()
-
-
-with Path("requirements.txt").open() as requirements_txt:
-    install_requires = [str(requirement) for requirement in pkg_resources.parse_requirements(requirements_txt)]
-
-setup(
-    # the name must match the folder name 'verysimplemodule'
-    name="pavimentados",
-    version=VERSION,
-    author="Jose Maria Marquez Blanco",
-    author_email="jose.marquez.blanco@gmail.com",
-    description=DESCRIPTION,
-    long_description=LONG_DESCRIPTION,
-    long_description_content_type="text/markdown",
-    packages=find_packages(),
-    install_requires=install_requires,
-    keywords=["Machine Learning", "crack detections", "computer vision", "safe road"],
-    classifiers=[
-        "Development Status :: 3 - Alpha",
-        "Programming Language :: Python :: 3",
-        "Operating System :: OS Independent",
-        "Programming Language :: Python :: 3.7",
-    ],
-    python_requires=">=3.7",
-    include_package_data=True,
-)
+from setuptools import setup, find_packages
+import pkg_resources
+from pathlib import Path
+
+this_directory = Path(__file__).parent
+VERSION = '0.9.0' 
+DESCRIPTION = 'A python package Library which implement IA algorithims to detect cracks and failures on roads. The package is wrapper around all the models and provides an interfaces to use them properly'
+
+LONG_DESCRIPTION = (this_directory / "README.md").read_text()
+
+
+with Path('requirements.txt').open() as requirements_txt:
+    install_requires = [str(requirement) for requirement in pkg_resources.parse_requirements(requirements_txt)]
+
+setup(
+       # the name must match the folder name 'verysimplemodule'
+        name="pavimentados", 
+        version=VERSION,
+        author="Jose Maria Marquez Blanco",
+        author_email="jose.marquez.blanco@gmail.com",
+        description=DESCRIPTION,
+        long_description=LONG_DESCRIPTION,
+        long_description_content_type='text/markdown',
+        packages=find_packages(),
+        install_requires=install_requires,        
+        keywords=['Machine Learning', 'crack detections', 'computer vision', 'safe road'],
+        classifiers= [
+            "Development Status :: 3 - Alpha",
+            "Programming Language :: Python :: 3",
+            "Operating System :: OS Independent",
+            "Programming Language :: Python :: 3.7",    
+        ],
+        python_requires=">=3.7", 
+        include_package_data=True
+)
```

