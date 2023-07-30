# Comparing `tmp/isyatirimhisse-0.1.1.tar.gz` & `tmp/isyatirimhisse-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isyatirimhisse-0.1.1.tar", last modified: Thu Jul 27 13:22:29 2023, max compression
+gzip compressed data, was "isyatirimhisse-0.2.0.tar", last modified: Sun Jul 30 13:47:43 2023, max compression
```

## Comparing `isyatirimhisse-0.1.1.tar` & `isyatirimhisse-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 13:22:29.873397 isyatirimhisse-0.1.1/
--rw-rw-rw-   0        0        0     1064 2023-07-23 21:22:22.000000 isyatirimhisse-0.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0       19 2023-07-27 13:01:25.000000 isyatirimhisse-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     6230 2023-07-27 13:22:29.871401 isyatirimhisse-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     5660 2023-07-27 13:19:21.000000 isyatirimhisse-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-27 13:22:29.799600 isyatirimhisse-0.1.1/isyatirimhisse/
--rw-rw-rw-   0        0        0     3736 2023-07-27 12:57:06.000000 isyatirimhisse-0.1.1/isyatirimhisse/VeriCek.py
--rw-rw-rw-   0        0        0       29 2023-07-24 11:50:14.000000 isyatirimhisse-0.1.1/isyatirimhisse/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-27 13:22:29.861465 isyatirimhisse-0.1.1/isyatirimhisse.egg-info/
--rw-rw-rw-   0        0        0     6230 2023-07-27 13:22:29.000000 isyatirimhisse-0.1.1/isyatirimhisse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      325 2023-07-27 13:22:29.000000 isyatirimhisse-0.1.1/isyatirimhisse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 13:22:29.000000 isyatirimhisse-0.1.1/isyatirimhisse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-07-27 13:22:29.000000 isyatirimhisse-0.1.1/isyatirimhisse.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-07-27 13:22:29.000000 isyatirimhisse-0.1.1/isyatirimhisse.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-27 13:22:29.873397 isyatirimhisse-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      822 2023-07-27 13:04:08.000000 isyatirimhisse-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-27 13:22:29.869409 isyatirimhisse-0.1.1/tests/
--rw-rw-rw-   0        0        0        0 2023-07-25 09:00:45.000000 isyatirimhisse-0.1.1/tests/__init__.py
--rw-rw-rw-   0        0        0     4279 2023-07-25 13:09:24.000000 isyatirimhisse-0.1.1/tests/test_veri_cek.py
+drwxrwxrwx   0        0        0        0 2023-07-30 13:47:43.133457 isyatirimhisse-0.2.0/
+-rw-rw-rw-   0        0        0     1064 2023-07-23 21:22:22.000000 isyatirimhisse-0.2.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      173 2023-07-30 13:45:41.000000 isyatirimhisse-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    10397 2023-07-30 13:47:43.132449 isyatirimhisse-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     9827 2023-07-30 13:46:51.000000 isyatirimhisse-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-30 13:47:42.971879 isyatirimhisse-0.2.0/imgs/
+-rw-rw-rw-   0        0        0   111188 2023-07-30 13:15:39.000000 isyatirimhisse-0.2.0/imgs/gorsel_ornek_1.png
+-rw-rw-rw-   0        0        0    53435 2023-07-30 13:29:30.000000 isyatirimhisse-0.2.0/imgs/gorsel_ornek_2.png
+-rw-rw-rw-   0        0        0   433600 2023-07-30 13:17:48.000000 isyatirimhisse-0.2.0/imgs/gorsel_ornek_3.png
+drwxrwxrwx   0        0        0        0 2023-07-30 13:47:43.030729 isyatirimhisse-0.2.0/isyatirimhisse/
+-rw-rw-rw-   0        0        0     4721 2023-07-30 12:56:36.000000 isyatirimhisse-0.2.0/isyatirimhisse/VeriCek.py
+-rw-rw-rw-   0        0        0     4784 2023-07-30 13:35:14.000000 isyatirimhisse-0.2.0/isyatirimhisse/VeriGorsel.py
+-rw-rw-rw-   0        0        0       66 2023-07-28 15:01:43.000000 isyatirimhisse-0.2.0/isyatirimhisse/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-30 13:47:43.089564 isyatirimhisse-0.2.0/isyatirimhisse.egg-info/
+-rw-rw-rw-   0        0        0    10397 2023-07-30 13:47:42.000000 isyatirimhisse-0.2.0/isyatirimhisse.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      452 2023-07-30 13:47:42.000000 isyatirimhisse-0.2.0/isyatirimhisse.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 13:47:42.000000 isyatirimhisse-0.2.0/isyatirimhisse.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-07-30 13:47:42.000000 isyatirimhisse-0.2.0/isyatirimhisse.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-07-30 13:47:42.000000 isyatirimhisse-0.2.0/isyatirimhisse.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-30 13:47:43.133457 isyatirimhisse-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      880 2023-07-30 13:39:59.000000 isyatirimhisse-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 13:47:43.126465 isyatirimhisse-0.2.0/tests/
+-rw-rw-rw-   0        0        0        0 2023-07-25 09:00:45.000000 isyatirimhisse-0.2.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     5009 2023-07-30 12:17:59.000000 isyatirimhisse-0.2.0/tests/test_veri_cek.py
+-rw-rw-rw-   0        0        0     2729 2023-07-30 13:36:49.000000 isyatirimhisse-0.2.0/tests/test_veri_gorsel.py
```

### Comparing `isyatirimhisse-0.1.1/LICENSE.txt` & `isyatirimhisse-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `isyatirimhisse-0.1.1/isyatirimhisse/VeriCek.py` & `isyatirimhisse-0.2.0/isyatirimhisse/VeriCek.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 import requests
 import pandas as pd
 import numpy as np
 from datetime import datetime
+import os
 
-def veri_cek(sembol=None, baslangic_tarih=None, bitis_tarih=None, frekans='1g', gozlem='son', getiri_hesapla=True, logaritmik_getiri=True, na_kaldir=True):
+def veri_cek(sembol=None, baslangic_tarih=None, bitis_tarih=None, frekans='1g', gozlem='son', getiri_hesapla=True, logaritmik_getiri=True, na_kaldir=True, excel_kaydet=False, excel_dosya_ismi=None):
     """
     Belirtilen tarih aralığında, belirtilen hisse senedi sembolleri için veri çeker. Çıktı özelleştirilebilir.
 
     Parametreler:
         sembol (str veya list, varsayılan None): Hisse senedi sembolü veya sembollerinin listesi.
         baslangic_tarih (str, 'GG-AA-YYYY', varsayılan None): Verilerin başlangıç tarihi (örn. '01-01-2023').
         bitis_tarih (str, 'GG-AA-YYYY', varsayılan None): Verilerin bitiş tarihi (örn. '25-07-2023').
             Eğer belirtilmezse, sistem tarihini (bugünkü tarihi) otomatik olarak kullanır.
         frekans (str, varsayılan '1g'): Veri frekansı (Günlük: '1g', Haftalık: '1h', Aylık: '1a', Yıllık: '1y').
         gozlem (str, varsayılan 'son'): Haftalık, aylık ve yıllık frekanslarda istenen gözlem ('son': Son, 'ortalama': Ortalama)
         getiri_hesapla (bool, varsayılan True): Getiri hesaplanacak mı?
         logaritmik_getiri (bool, varsayılan True): Logaritmik getiri mi hesaplanacak?
         na_kaldir (bool, varsayılan True): Eksik değerler kaldırılacak mı?
+        excel_kaydet (bool, varsayılan False): pandas DataFrame Excel dosyasına kaydedilsin mi?
+        excel_dosya_ismi (str, varsayılan None): Kaydedilecek Excel dosyasının ismi (örn. 'veriler.xlsx').
+            Geçerli bir dosya adı belirtilmezse, varsayılan olarak 'veriler.xlsx' kullanılır.
 
     Dönen değer:
         pandas.DataFrame: İstenilen tarih aralığındaki hisse senedi verileri ve gerekirse getiri değerleri içeren DataFrame.
     """
 
     if not sembol or sembol is None:
         raise KeyError("Hisse senedi sembolü girilmedi. 'sembol' parametresi zorunludur.")
@@ -73,8 +77,23 @@
             df_final = df_final.apply(lambda x: x / x.shift(1) - 1)
 
     if na_kaldir:
         df_final = df_final.dropna()
 
     df_final = df_final.reset_index()
 
-    return df_final
+    if excel_kaydet:
+        if not excel_dosya_ismi or excel_dosya_ismi is None:
+            excel_bitis_tarih = datetime.now().strftime('%Y%m%d')
+            excel_dosya_ismi = f'veriler_{excel_bitis_tarih}.xlsx'
+        else:
+            dosya_ismi, dosya_uzantisi = os.path.splitext(excel_dosya_ismi)
+            if not dosya_uzantisi:
+                excel_dosya_ismi += '.xlsx'
+            i = 1
+            while os.path.exists(excel_dosya_ismi):
+                excel_dosya_ismi = f'{dosya_ismi}_{i}{dosya_uzantisi}'
+                i += 1
+
+        df_final.to_excel(excel_dosya_ismi, index=False)
+
+    return df_final
```

### Comparing `isyatirimhisse-0.1.1/setup.py` & `isyatirimhisse-0.2.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 from setuptools import setup, find_packages
 
 setup(
     name="isyatirimhisse",
-    version="0.1.1",
+    version="0.2.0",
     packages=find_packages(),
     author="Uraz Akgül",
     author_email="urazdev@gmail.com",
     description="İş Yatırım'ın web sitesinden veri çekme işlemlerini kolaylaştıran ve isteğe göre özelleştirilebilen bir kütüphane.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/urazakgul/isyatirimhisse",
     license="MIT",
     install_requires=[
         "requests",
         "pandas",
         "numpy",
+        "matplotlib",
+        "seaborn",
+        "os",
     ],
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires=">=3.8",
```

### Comparing `isyatirimhisse-0.1.1/tests/test_veri_cek.py` & `isyatirimhisse-0.2.0/tests/test_veri_cek.py`

 * *Files 22% similar despite different names*

```diff
@@ -18,99 +18,116 @@
     baslangic_tarih = '03-01-2023'
     bitis_tarih = '21-07-2023'
     frekans = '1g'
     gozlem = 'son'
     getiri_hesapla = True
     logaritmik_getiri = True
     na_kaldir = True
+    excel_kaydet = True
 
     veriler = veri_cek(
         sembol=sembol,
         baslangic_tarih=baslangic_tarih,
         bitis_tarih=bitis_tarih,
         frekans=frekans,
         gozlem=gozlem,
         getiri_hesapla=getiri_hesapla,
         logaritmik_getiri=logaritmik_getiri,
-        na_kaldir=na_kaldir
+        na_kaldir=na_kaldir,
+        excel_kaydet=excel_kaydet
     )
 
     assert isinstance(veriler, pd.DataFrame), "Veri çekme fonksiyonu DataFrame dönmeli."
     assert len(veriler) > 0, "Veri çekme fonksiyonu boş DataFrame döndü."
 
     # Test senaryosu 2: Bitiş tarihi yok
 
     sembol = 'AKBNK'
     baslangic_tarih = '03-01-2023'
     frekans = '1g'
     gozlem = 'son'
     getiri_hesapla = True
     logaritmik_getiri = True
     na_kaldir = True
+    excel_kaydet = True
+    excel_dosya_ismi = 'test_veri.xlsx'
 
     veriler = veri_cek(
         sembol=sembol,
         baslangic_tarih=baslangic_tarih,
         frekans=frekans,
         gozlem=gozlem,
         getiri_hesapla=getiri_hesapla,
         logaritmik_getiri=logaritmik_getiri,
-        na_kaldir=na_kaldir
+        na_kaldir=na_kaldir,
+        excel_kaydet=excel_kaydet,
+        excel_dosya_ismi=excel_dosya_ismi
     )
 
     assert isinstance(veriler, pd.DataFrame), "Veri çekme fonksiyonu DataFrame dönmeli."
     assert len(veriler) > 0, "Veri çekme fonksiyonu boş DataFrame döndü."
+    assert os.path.exists(excel_dosya_ismi), "Excel dosyası kaydedilmedi."
 
     # Test senaryosu 3: Birden fazla hisse, haftalık frekans, basit getiri ve NA kaldır
     sembol = ['AKBNK', 'EUPWR']
     baslangic_tarih = '03-01-2023'
     bitis_tarih = '21-07-2023'
     frekans = '1h'
     gozlem = 'son'
     getiri_hesapla = True
     logaritmik_getiri = False
     na_kaldir = True
+    excel_kaydet = True
+    excel_dosya_ismi = 'test_veri.xlsx'
 
     veriler = veri_cek(
         sembol=sembol,
         baslangic_tarih=baslangic_tarih,
         bitis_tarih=bitis_tarih,
         frekans=frekans,
         gozlem=gozlem,
         getiri_hesapla=getiri_hesapla,
         logaritmik_getiri=logaritmik_getiri,
-        na_kaldir=na_kaldir
+        na_kaldir=na_kaldir,
+        excel_kaydet=excel_kaydet,
+        excel_dosya_ismi=excel_dosya_ismi
     )
 
     assert isinstance(veriler, pd.DataFrame), "Veri çekme fonksiyonu DataFrame dönmeli."
     assert len(veriler) > 0, "Veri çekme fonksiyonu boş DataFrame döndü."
+    assert os.path.exists(excel_dosya_ismi), "Excel dosyası kaydedilmedi."
 
     # Test senaryosu 4: Birden fazla hisse, aylık frekans, kapanış fiyatı ve NA bırak
     sembol = ['AKBNK', 'EUPWR']
     baslangic_tarih = '03-01-2023'
     bitis_tarih = '21-07-2023'
     frekans = '1a'
     gozlem = 'son'
     getiri_hesapla = False
     logaritmik_getiri = True
     na_kaldir = False
+    excel_kaydet = True
+    excel_dosya_ismi = 'test_veri.xlsx'
 
     veriler = veri_cek(
         sembol=sembol,
         baslangic_tarih=baslangic_tarih,
         bitis_tarih=bitis_tarih,
         frekans=frekans,
         gozlem=gozlem,
         getiri_hesapla=getiri_hesapla,
         logaritmik_getiri=logaritmik_getiri,
-        na_kaldir=na_kaldir
+        na_kaldir=na_kaldir,
+        excel_kaydet=excel_kaydet,
+        excel_dosya_ismi=excel_dosya_ismi
     )
 
     assert isinstance(veriler, pd.DataFrame), "Veri çekme fonksiyonu DataFrame dönmeli."
     assert len(veriler) > 0, "Veri çekme fonksiyonu boş DataFrame döndü."
+    assert os.path.exists(excel_dosya_ismi), "Excel dosyası kaydedilmedi."
 
     # Test senaryosu 5: Birden fazla hisse, yıllık frekans, kapanış fiyatları, ortalama fiyatlar ve NA kaldır
     sembol = ['AKBNK', 'EUPWR']
     baslangic_tarih = '03-01-2023'
     bitis_tarih = '21-07-2023'
     frekans = '1y'
     gozlem = 'ortalama'
```

