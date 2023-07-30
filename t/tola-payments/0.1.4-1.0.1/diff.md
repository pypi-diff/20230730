# Comparing `tmp/tola_payments-0.1.4.tar.gz` & `tmp/tola_payments-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tola_payments-0.1.4.tar", last modified: Tue Mar 14 15:07:02 2023, max compression
+gzip compressed data, was "tola_payments-1.0.1.tar", last modified: Sun Jul 30 14:34:55 2023, max compression
```

## Comparing `tola_payments-0.1.4.tar` & `tola_payments-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-03-14 15:07:02.858554 tola_payments-0.1.4/
--rw-rw-rw-   0        0        0     1089 2023-03-07 09:09:18.000000 tola_payments-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     2083 2023-03-14 15:07:02.857344 tola_payments-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1831 2023-03-09 20:14:04.000000 tola_payments-0.1.4/README.md
--rw-rw-rw-   0        0        0       42 2023-03-14 15:07:02.858554 tola_payments-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      517 2023-03-14 14:52:37.000000 tola_payments-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-14 15:07:02.834332 tola_payments-0.1.4/tola_payments/
--rw-rw-rw-   0        0        0     2669 2023-03-14 14:44:45.000000 tola_payments-0.1.4/tola_payments/__init__.py
--rw-rw-rw-   0        0        0      261 2023-03-06 20:02:22.000000 tola_payments-0.1.4/tola_payments/testing.py
-drwxrwxrwx   0        0        0        0 2023-03-14 15:07:02.856440 tola_payments-0.1.4/tola_payments.egg-info/
--rw-rw-rw-   0        0        0     2083 2023-03-14 15:07:02.000000 tola_payments-0.1.4/tola_payments.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2023-03-14 15:07:02.000000 tola_payments-0.1.4/tola_payments.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-14 15:07:02.000000 tola_payments-0.1.4/tola_payments.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-03-14 15:07:02.000000 tola_payments-0.1.4/tola_payments.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-03-14 15:07:02.000000 tola_payments-0.1.4/tola_payments.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 14:34:55.258153 tola_payments-1.0.1/
+-rw-rw-rw-   0        0        0     1089 2023-03-07 09:09:18.000000 tola_payments-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     2236 2023-07-30 14:34:55.257145 tola_payments-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1984 2023-07-30 14:26:19.000000 tola_payments-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-30 14:34:55.258153 tola_payments-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      517 2023-07-30 14:34:25.000000 tola_payments-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 14:34:55.170842 tola_payments-1.0.1/tola_payments/
+-rw-rw-rw-   0        0        0     2481 2023-07-07 18:14:10.000000 tola_payments-1.0.1/tola_payments/__init__.py
+-rw-rw-rw-   0        0        0      261 2023-03-06 20:02:22.000000 tola_payments-1.0.1/tola_payments/testing.py
+drwxrwxrwx   0        0        0        0 2023-07-30 14:34:55.239938 tola_payments-1.0.1/tola_payments.egg-info/
+-rw-rw-rw-   0        0        0     2236 2023-07-30 14:34:53.000000 tola_payments-1.0.1/tola_payments.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2023-07-30 14:34:53.000000 tola_payments-1.0.1/tola_payments.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 14:34:53.000000 tola_payments-1.0.1/tola_payments.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-07-30 14:34:53.000000 tola_payments-1.0.1/tola_payments.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-30 14:34:53.000000 tola_payments-1.0.1/tola_payments.egg-info/top_level.txt
```

### Comparing `tola_payments-0.1.4/LICENSE` & `tola_payments-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tola_payments-0.1.4/PKG-INFO` & `tola_payments-1.0.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,58 @@
 Metadata-Version: 2.1
 Name: tola_payments
-Version: 0.1.4
+Version: 1.0.1
 Summary: A python package to easy push payment integration with Tola Payments with Mpesa, TigoPesa, and AirtelMoney Tanzania
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-Tola Payments Python Package
+
+# Tola Payments Python Package
+
 
 A python package to easy push payment integration with Tola Payments with Mpesa, TigoPesa, and AirtelMoney Tanzania. You can easily charge a customer's phone number with a specified amount, and the package will handle the necessary details to make the payment using the Tola Mobile API. No need to integrate each MNO individualy.
 
-Installation
-To install the Tola Payments package, run the following command:
+## Installation
+Use the package manager [pip](https://pip.pypa.io/en/stable/) to install Tola Payments package.
 
-pip install tola_payments
+Installation To install the Tola Payments package, run the following command:
 
-Usage
+```bash
+pip install tola_payments
+```
 
-Configuration
+## Configuration
 
-To use the package, you need to set up your Tola Mobile API credentials in a .env file. Add the following variables to your .env file:
-To use the Tola Payments package, you first need to import it into your Python code. Here's an example:
+To use the package, you need to set up your Tola Mobile API credentials in a .env file. Add the following variables to your .env file: To use the Tola Payments package, you first need to import it into your Python code. Here's an example:
 
-TOLA_USERNAME=<your Tola Mobile API username>
-TOLA_PASSWORD=<your Tola Mobile API password>
-VODA_TARGET=<your Vodacom Tola Mobile API target>
-TIGO_TARGET=<your Tigo Tola Mobile API target>
-AIRTEL_TARGET=<your Airtel Tola Mobile API target>
-TOLA_LIVE_URL = <your Tola Live Url>
 
+```env
+TOLA_USERNAME = "my_username"
+TOLA_PASSWORD = "my_password"
+VODA_TARGET = "my_voda_target"
+TIGO_TARGET = "my_tigo_target"
+AIRTEL_TARGET = "my_airtel_target"
+TOLA_LIVE_URL = "my_tola_live_url"
+```
 
 Next, create an instance of the TolaPayments class, providing your Tola Mobile API credentials:
 
+```python
 from tolapyments import TolaPayments
-
 tolapayments = TolaPayments(is_sandbox=True)
+```
+
 
 Note that the is_sandbox parameter specifies whether you're using the Tola Mobile sandbox environment or the live environment. If you're using the sandbox environment, set is_sandbox to True. Otherwise, set it to False and provide the live API URL via the TOLA_LIVE_URL environment variable.
 
 To charge a customer, call the charge_customer method on your TolaPayments instance, passing in the customer's phone number, the amount to charge, and a source reference
 
+```python
 response =tolapayments.charge_costomer(amount="1000",phone_number="+25561189850", sourcereference='4546f56543poF66')
 
 print(response.text)
+```
+
+
+## License
 
+[MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `tola_payments-0.1.4/setup.py` & `tola_payments-1.0.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setup(
     name="tola_payments",
-    version="0.1.4",
+    version="1.0.1",
     description="A python package to easy push payment integration with Tola Payments with Mpesa, TigoPesa, and AirtelMoney Tanzania",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=["phonenumbers", "tanzania_mno", "python-decouple"],
 )
```

### Comparing `tola_payments-0.1.4/tola_payments/__init__.py` & `tola_payments-1.0.1/tola_payments/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,16 +34,14 @@
             "msisdn": str(phone_number_formated),
             "type": "charge",
             "amount": amount,
             "sourcereference": sourcereference,
             "currency" :"TZS",
 
         }
-     
-        
         if mno_name == "Vodacom":
             payload["target"] = self.__voda_target
             payload["channel"] = "TANZANIA.VODACOM"
         elif mno_name == "Tigo":
             payload["target"] = self.__tigo_target
             payload["channel"] = "TANZANIA.TIGO"
         elif mno_name == "Airtel":
@@ -57,12 +55,7 @@
         headers = { "Authorization": "Basic " + base64.b64encode(f"{auth_credentials[0]}:{auth_credentials[1]}".encode('utf-8')).decode('utf-8'), "Content-Type": "application/json"}
         resp =   requests.post(self.get_url(), json=payload, headers=headers)
         try:
             return resp
         except:
             return "Number Not allowed"
 
-
-pym = TolaPayements(is_sandbox=False)
-
-response = pym.charge_costomer(phone_number="0757685690", amount="300000", sourcereference="6triuog98etu")
-print(response.text)
```

### Comparing `tola_payments-0.1.4/tola_payments.egg-info/PKG-INFO` & `tola_payments-1.0.1/tola_payments.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,45 +1,58 @@
 Metadata-Version: 2.1
 Name: tola-payments
-Version: 0.1.4
+Version: 1.0.1
 Summary: A python package to easy push payment integration with Tola Payments with Mpesa, TigoPesa, and AirtelMoney Tanzania
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-Tola Payments Python Package
+
+# Tola Payments Python Package
+
 
 A python package to easy push payment integration with Tola Payments with Mpesa, TigoPesa, and AirtelMoney Tanzania. You can easily charge a customer's phone number with a specified amount, and the package will handle the necessary details to make the payment using the Tola Mobile API. No need to integrate each MNO individualy.
 
-Installation
-To install the Tola Payments package, run the following command:
+## Installation
+Use the package manager [pip](https://pip.pypa.io/en/stable/) to install Tola Payments package.
 
-pip install tola_payments
+Installation To install the Tola Payments package, run the following command:
 
-Usage
+```bash
+pip install tola_payments
+```
 
-Configuration
+## Configuration
 
-To use the package, you need to set up your Tola Mobile API credentials in a .env file. Add the following variables to your .env file:
-To use the Tola Payments package, you first need to import it into your Python code. Here's an example:
+To use the package, you need to set up your Tola Mobile API credentials in a .env file. Add the following variables to your .env file: To use the Tola Payments package, you first need to import it into your Python code. Here's an example:
 
-TOLA_USERNAME=<your Tola Mobile API username>
-TOLA_PASSWORD=<your Tola Mobile API password>
-VODA_TARGET=<your Vodacom Tola Mobile API target>
-TIGO_TARGET=<your Tigo Tola Mobile API target>
-AIRTEL_TARGET=<your Airtel Tola Mobile API target>
-TOLA_LIVE_URL = <your Tola Live Url>
 
+```env
+TOLA_USERNAME = "my_username"
+TOLA_PASSWORD = "my_password"
+VODA_TARGET = "my_voda_target"
+TIGO_TARGET = "my_tigo_target"
+AIRTEL_TARGET = "my_airtel_target"
+TOLA_LIVE_URL = "my_tola_live_url"
+```
 
 Next, create an instance of the TolaPayments class, providing your Tola Mobile API credentials:
 
+```python
 from tolapyments import TolaPayments
-
 tolapayments = TolaPayments(is_sandbox=True)
+```
+
 
 Note that the is_sandbox parameter specifies whether you're using the Tola Mobile sandbox environment or the live environment. If you're using the sandbox environment, set is_sandbox to True. Otherwise, set it to False and provide the live API URL via the TOLA_LIVE_URL environment variable.
 
 To charge a customer, call the charge_customer method on your TolaPayments instance, passing in the customer's phone number, the amount to charge, and a source reference
 
+```python
 response =tolapayments.charge_costomer(amount="1000",phone_number="+25561189850", sourcereference='4546f56543poF66')
 
 print(response.text)
+```
+
+
+## License
 
+[MIT](https://choosealicense.com/licenses/mit/)
```

