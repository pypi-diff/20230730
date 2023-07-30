# Comparing `tmp/opet-0.0.6.tar.gz` & `tmp/opet-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opet-0.0.6.tar", last modified: Sun Jul 30 20:36:46 2023, max compression
+gzip compressed data, was "opet-0.0.7.tar", last modified: Sun Jul 30 21:29:48 2023, max compression
```

## Comparing `opet-0.0.6.tar` & `opet-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 btcyz255   (501) staff       (20)        0 2023-07-30 20:36:46.291995 opet-0.0.6/
--rw-r--r--   0 btcyz255   (501) staff       (20)     1069 2023-07-30 14:59:51.000000 opet-0.0.6/LICENSE
--rw-r--r--   0 btcyz255   (501) staff       (20)     1029 2023-07-30 20:36:46.291776 opet-0.0.6/PKG-INFO
--rw-r--r--   0 btcyz255   (501) staff       (20)      555 2023-07-30 20:36:28.000000 opet-0.0.6/README.md
--rw-r--r--   0 btcyz255   (501) staff       (20)       38 2023-07-30 20:36:46.292056 opet-0.0.6/setup.cfg
--rw-r--r--   0 btcyz255   (501) staff       (20)      815 2023-07-30 20:33:35.000000 opet-0.0.6/setup.py
-drwxr-xr-x   0 btcyz255   (501) staff       (20)        0 2023-07-30 20:36:46.285596 opet-0.0.6/src/
-drwxr-xr-x   0 btcyz255   (501) staff       (20)        0 2023-07-30 20:36:46.289101 opet-0.0.6/src/opet/
--rw-r--r--   0 btcyz255   (501) staff       (20)        0 2023-07-30 20:11:51.000000 opet-0.0.6/src/opet/__init__.py
--rw-r--r--   0 btcyz255   (501) staff       (20)      866 2023-07-30 19:26:06.000000 opet-0.0.6/src/opet/api.py
--rw-r--r--   0 btcyz255   (501) staff       (20)       79 2023-07-30 14:21:02.000000 opet-0.0.6/src/opet/exceptions.py
--rw-r--r--   0 btcyz255   (501) staff       (20)      918 2023-07-30 19:29:32.000000 opet-0.0.6/src/opet/utils.py
-drwxr-xr-x   0 btcyz255   (501) staff       (20)        0 2023-07-30 20:36:46.291313 opet-0.0.6/src/opet.egg-info/
--rw-r--r--   0 btcyz255   (501) staff       (20)     1029 2023-07-30 20:36:46.000000 opet-0.0.6/src/opet.egg-info/PKG-INFO
--rw-r--r--   0 btcyz255   (501) staff       (20)      263 2023-07-30 20:36:46.000000 opet-0.0.6/src/opet.egg-info/SOURCES.txt
--rw-r--r--   0 btcyz255   (501) staff       (20)        1 2023-07-30 20:36:46.000000 opet-0.0.6/src/opet.egg-info/dependency_links.txt
--rw-r--r--   0 btcyz255   (501) staff       (20)        9 2023-07-30 20:36:46.000000 opet-0.0.6/src/opet.egg-info/requires.txt
--rw-r--r--   0 btcyz255   (501) staff       (20)        5 2023-07-30 20:36:46.000000 opet-0.0.6/src/opet.egg-info/top_level.txt
+drwxr-xr-x   0 btcyz255   (501) staff       (20)        0 2023-07-30 21:29:48.611613 opet-0.0.7/
+-rw-r--r--   0 btcyz255   (501) staff       (20)     1069 2023-07-30 14:59:51.000000 opet-0.0.7/LICENSE
+-rw-r--r--   0 btcyz255   (501) staff       (20)     1029 2023-07-30 21:29:48.611326 opet-0.0.7/PKG-INFO
+-rw-r--r--   0 btcyz255   (501) staff       (20)      555 2023-07-30 20:36:28.000000 opet-0.0.7/README.md
+drwxr-xr-x   0 btcyz255   (501) staff       (20)        0 2023-07-30 21:29:48.598946 opet-0.0.7/opet/
+-rw-r--r--   0 btcyz255   (501) staff       (20)        0 2023-07-30 20:11:51.000000 opet-0.0.7/opet/__init__.py
+-rw-r--r--   0 btcyz255   (501) staff       (20)     1448 2023-07-30 21:25:02.000000 opet-0.0.7/opet/api.py
+-rw-r--r--   0 btcyz255   (501) staff       (20)      130 2023-07-30 21:13:49.000000 opet-0.0.7/opet/exceptions.py
+-rw-r--r--   0 btcyz255   (501) staff       (20)      307 2023-07-30 21:28:21.000000 opet-0.0.7/opet/main.py
+-rw-r--r--   0 btcyz255   (501) staff       (20)     1005 2023-07-30 21:26:13.000000 opet-0.0.7/opet/utils.py
+drwxr-xr-x   0 btcyz255   (501) staff       (20)        0 2023-07-30 21:29:48.610830 opet-0.0.7/opet.egg-info/
+-rw-r--r--   0 btcyz255   (501) staff       (20)     1029 2023-07-30 21:29:48.000000 opet-0.0.7/opet.egg-info/PKG-INFO
+-rw-r--r--   0 btcyz255   (501) staff       (20)      271 2023-07-30 21:29:48.000000 opet-0.0.7/opet.egg-info/SOURCES.txt
+-rw-r--r--   0 btcyz255   (501) staff       (20)        1 2023-07-30 21:29:48.000000 opet-0.0.7/opet.egg-info/dependency_links.txt
+-rw-r--r--   0 btcyz255   (501) staff       (20)       43 2023-07-30 21:29:48.000000 opet-0.0.7/opet.egg-info/entry_points.txt
+-rw-r--r--   0 btcyz255   (501) staff       (20)        9 2023-07-30 21:29:48.000000 opet-0.0.7/opet.egg-info/requires.txt
+-rw-r--r--   0 btcyz255   (501) staff       (20)        5 2023-07-30 21:29:48.000000 opet-0.0.7/opet.egg-info/top_level.txt
+-rw-r--r--   0 btcyz255   (501) staff       (20)       38 2023-07-30 21:29:48.611675 opet-0.0.7/setup.cfg
+-rw-r--r--   0 btcyz255   (501) staff       (20)      894 2023-07-30 21:28:37.000000 opet-0.0.7/setup.py
```

### Comparing `opet-0.0.6/LICENSE` & `opet-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `opet-0.0.6/PKG-INFO` & `opet-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opet
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Python package that allows you to view fuel prices in Turkey based on cities.
 Home-page: https://github.com/sinanerdinc/opet
 Author: Sinan Erdinc
 Author-email: hello@sinanerdinc.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `opet-0.0.6/README.md` & `opet-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `opet-0.0.6/setup.py` & `opet-0.0.7/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,23 +3,27 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="opet",
     author="Sinan Erdinc",
     author_email="hello@sinanerdinc.com",
-    version="0.0.6",
+    version="0.0.7",
     install_requires=["requests"],
-    include_package_data=True,
     description="A Python package that allows you to view fuel prices in Turkey based on cities.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/sinanerdinc/opet",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    package_dir={'': 'src'},
-    packages=find_packages(where='src'),
+    entry_points={
+            'console_scripts': [
+                'opet-cli=opet.main:cli',
+            ],
+    },
+    packages=find_packages(),
+    package_dir={'opet': 'opet'},
     python_requires=">=3.0"
 )
```

### Comparing `opet-0.0.6/src/opet/api.py` & `opet-0.0.7/opet/api.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from src.opet.utils import yesterday, http_get
-
+from opet.utils import yesterday, http_get, to_json
+from opet.exceptions import ProvinceNotFoundError
 
 class OpetApiClient:
     def __init__(self):
         self.url = "https://api.opet.com.tr/api/fuelprices"
 
     def get_provinces(self):
         return http_get(f"{self.url}/provinces")
@@ -14,13 +14,26 @@
     def get_price(self, district_id: str):
         date = yesterday()
         url = f"{self.url}/prices/archive?DistrictCode={district_id}&StartDate={date}&EndDate={date}&IncludeAllProducts=true"
         r = http_get(url)
         response = list(map(lambda x: dict(name=x["productName"], amount=x["amount"]), r[0]["prices"]))
         return response
 
+    def price(self, province_id: str):
+        _provinces = self.get_provinces()
+        formatted_provinces = {str(item['code']): item['name'] for item in _provinces}
+        province_name = formatted_provinces.get(f"{province_id}", None)
+        if province_name is None:
+            raise ProvinceNotFoundError(f"Sistemde {province_id} plaka koduna ait bir il bulunamadı.")
+
+        result = dict(
+            results=dict(
+                province=province_name,
+                prices=self.get_price(self.get_districts(province_id)[0]["code"])
+            )
+        )
+        return to_json(result)
+
 
 if __name__ == '__main__':
     client = OpetApiClient()
-    print(client.get_provinces())
-    print(client.get_districts(28))
-    print(client.get_price("028002"))
+    print(client.price("28"))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `opet-0.0.6/src/opet/utils.py` & `opet-0.0.7/opet/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from datetime import datetime, timezone, timedelta
 import requests
-from src.opet.exceptions import Http200Error
+from opet.exceptions import Http200Error
+import json
 
 
 def yesterday():
     now_datetime = datetime.now(timezone.utc)
     six_hours_delta = timedelta(days=1)
     target_datetime = now_datetime - six_hours_delta
     output_datetime_str = target_datetime.strftime('%Y-%m-%dT%H:%M:%S.%fZ')
@@ -21,9 +22,13 @@
     }
     r = requests.get(url, headers=headers, verify=True)
     if r.status_code != 200:
         raise Http200Error("HttpStatusCode is not 200.")
     return r.json()
 
 
+def to_json(data):
+    return json.dumps(data, ensure_ascii=False, indent=2)
+
+
 if __name__ == '__main__':
     print(yesterday())
```

### Comparing `opet-0.0.6/src/opet.egg-info/PKG-INFO` & `opet-0.0.7/opet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opet
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Python package that allows you to view fuel prices in Turkey based on cities.
 Home-page: https://github.com/sinanerdinc/opet
 Author: Sinan Erdinc
 Author-email: hello@sinanerdinc.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

