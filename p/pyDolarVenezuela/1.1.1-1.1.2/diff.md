# Comparing `tmp/pyDolarVenezuela-1.1.1-py3-none-any.whl.zip` & `tmp/pyDolarVenezuela-1.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 6121 bytes, number of entries: 10
+Zip file size: 6244 bytes, number of entries: 10
 -rw-rw-rw-  2.0 fat       98 b- defN 23-Jul-26 05:29 pyDolarVenezuela/__init__.py
 -rw-rw-rw-  2.0 fat      389 b- defN 23-Jul-26 03:29 pyDolarVenezuela/module_bcv.py
 -rw-rw-rw-  2.0 fat      580 b- defN 23-Jul-29 04:40 pyDolarVenezuela/request.py
--rw-rw-rw-  2.0 fat     3071 b- defN 23-Jul-29 05:38 pyDolarVenezuela/scraping_monitor.py
+-rw-rw-rw-  2.0 fat     3363 b- defN 23-Jul-30 03:51 pyDolarVenezuela/scraping_monitor.py
 -rw-rw-rw-  2.0 fat       81 b- defN 23-Jul-26 04:18 pyDolarVenezuela/util.py
--rw-rw-rw-  2.0 fat     1094 b- defN 23-Jul-29 05:45 pyDolarVenezuela-1.1.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3560 b- defN 23-Jul-29 05:45 pyDolarVenezuela-1.1.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-29 05:45 pyDolarVenezuela-1.1.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 23-Jul-29 05:45 pyDolarVenezuela-1.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      855 b- defN 23-Jul-29 05:45 pyDolarVenezuela-1.1.1.dist-info/RECORD
-10 files, 9837 bytes uncompressed, 4641 bytes compressed:  52.8%
+-rw-rw-rw-  2.0 fat     1094 b- defN 23-Jul-30 04:51 pyDolarVenezuela-1.1.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3578 b- defN 23-Jul-30 04:51 pyDolarVenezuela-1.1.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-30 04:51 pyDolarVenezuela-1.1.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 23-Jul-30 04:51 pyDolarVenezuela-1.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      855 b- defN 23-Jul-30 04:51 pyDolarVenezuela-1.1.2.dist-info/RECORD
+10 files, 10147 bytes uncompressed, 4764 bytes compressed:  53.1%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: pyDolarVenezuela/scraping_monitor.py
 Comment: 
 
 Filename: pyDolarVenezuela/util.py
 Comment: 
 
-Filename: pyDolarVenezuela-1.1.1.dist-info/LICENSE
+Filename: pyDolarVenezuela-1.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: pyDolarVenezuela-1.1.1.dist-info/METADATA
+Filename: pyDolarVenezuela-1.1.2.dist-info/METADATA
 Comment: 
 
-Filename: pyDolarVenezuela-1.1.1.dist-info/WHEEL
+Filename: pyDolarVenezuela-1.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: pyDolarVenezuela-1.1.1.dist-info/top_level.txt
+Filename: pyDolarVenezuela-1.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: pyDolarVenezuela-1.1.1.dist-info/RECORD
+Filename: pyDolarVenezuela-1.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyDolarVenezuela/scraping_monitor.py

```diff
@@ -1,19 +1,24 @@
 from bs4 import BeautifulSoup
-from emoji import emojize
 
 from pyDolarVenezuela.request import get_content_page
 from pyDolarVenezuela.util import PAGINA_PRINCIPAL_EXCHANGE_MONITOR
 
 def _get_values_monitors(soup: BeautifulSoup):
     return [value for value in soup]
 
 def _get_date_value(soup: BeautifulSoup):
     return str(soup.find('p')).split("<br/>")[-1].replace("</p>", "")
 
+def _convert_specific_format(text: str) -> str:
+    acentos = {'á': 'a', 'é': 'e', 'í': 'i', 'ó': 'o', 'ú': 'u'}
+    for acento, sin_acento in acentos.items():
+        text = text.lower().replace(acento, sin_acento).replace(' ', '_')
+    return text
+
 class Monitor(object):
     """
     La clase Monitor permite consultar los precios del dólar en diversos monitores en Venezuela. \n
     El método `_load` carga los datos de los monitores a través del scraping de la página web de referencia, donde los datos son almacenados en un diccionario. \ 
     El método `get_value_monitors` permite acceder a los datos almacenados en el diccionario.
     """
     def _load(self):
@@ -30,18 +35,18 @@
         for monitor in all_monitors:
             monitor = monitor.find("div", "module-table module-table-fecha")
             change = str(monitor.find('p', 'cambio-por').text)
             data = {
                 "title": monitor.find('h6', 'nombre').text,
                 "price": str(monitor.find('p', 'precio').text).replace(',', '.'),
                 "change": ("\U00002B07" + change[1:] if change[0] == '▼' else "\U00002B06" + change[1:] if change[0] == '▲' else "" + change[1:]),
-                "last_update": monitor.find('p', 'fecha').text
+                "last_update": ' '.join(str(monitor.find('p', 'fecha').text).split(' ')[1:])
             }
-            self.all_monitors[f"{i}"] = data
-            i += 1
+            self.all_monitors[_convert_specific_format(data['title'])] = data
+            
     
     def get_value_monitors(self, monitor_code: str = None, name_property: str = None, prettify: bool = False):
         """
         El parámetro `monitor_code` indica el código del monitor del cual se desea obtener información, \
         mientras que el parámetro `prettify` permite mostrar los precios en formato de moneda con el símbolo de Bolívares. \
         Si se proporciona un nombre de propiedad válido, se devolverá el valor correspondiente para ese monitor.
         """
```

## Comparing `pyDolarVenezuela-1.1.1.dist-info/LICENSE` & `pyDolarVenezuela-1.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyDolarVenezuela-1.1.1.dist-info/METADATA` & `pyDolarVenezuela-1.1.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDolarVenezuela
-Version: 1.1.1
+Version: 1.1.2
 Summary: esta es una librería en python que te permite consultar los precios del dólar en diferentes monitores en Venezuela y el dolar oficial BCV.
 Home-page: https://github.com/fcoagz/pydolarvenezuela
 Author: Francisco Griman
 Author-email: Francisco Griman <grihardware@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/fcoagz/pydolarvenezuela
 Project-URL: Bug Tracker, https://github.com/fcoagz/pydolarvenezuela/issues
@@ -43,18 +43,18 @@
 
 monitor = pdv.Monitor()
 
 # Obtener los valores de todos los monitores
 values = monitor.get_value_monitors()
 
 # Obtener el valor del dólar en EnParaleloVzla
-get_value_enparalelovzla = monitor.get_value_monitors(monitor_code='2', name_property='price', prettify=True)
+get_value_enparalelovzla = monitor.get_value_monitors(monitor_code='enparalelovzla', name_property='price', prettify=True)
 
 # Obtener la ultima actualizacion del dólar en Binance
-get_value_binance = monitor.get_value_monitors(monitor_code='17', name_property='last_update', prettify=False)
+get_value_binance = monitor.get_value_monitors(monitor_code='binance', name_property='last_update', prettify=False)
 ```
 
 La clase `Bcv` tiene el siguiente metodo:
 
 - `Bcv().get_rates()`: Te muestra los valores de las tasas de cambio del Banco Central de Venezuela. EUR, CNY, TRY, USD.
 
 Los parametros del metodo ante mencionado son los siguientes:
```

