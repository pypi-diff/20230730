# Comparing `tmp/Scrapset-4.3.5.tar.gz` & `tmp/Scrapset-5.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Scrapset-4.3.5.tar", last modified: Thu Jul 13 18:27:52 2023, max compression
+gzip compressed data, was "Scrapset-5.3.1.tar", last modified: Sun Jul 30 10:17:21 2023, max compression
```

## Comparing `Scrapset-4.3.5.tar` & `Scrapset-5.3.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 18:27:52.862599 Scrapset-4.3.5/
--rw-rw-rw-   0        0        0     4648 2023-07-13 18:27:52.862599 Scrapset-4.3.5/PKG-INFO
--rw-rw-rw-   0        0        0     4417 2023-07-12 16:15:55.000000 Scrapset-4.3.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-13 18:27:52.855623 Scrapset-4.3.5/Scrapset/
--rw-rw-rw-   0        0        0    10284 2023-07-13 18:25:37.000000 Scrapset-4.3.5/Scrapset/Scrapset.py
--rw-rw-rw-   0        0        0       61 2023-07-13 16:57:26.000000 Scrapset-4.3.5/Scrapset/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 18:27:52.861395 Scrapset-4.3.5/Scrapset.egg-info/
--rw-rw-rw-   0        0        0     4648 2023-07-13 18:27:52.000000 Scrapset-4.3.5/Scrapset.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2023-07-13 18:27:52.000000 Scrapset-4.3.5/Scrapset.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 18:27:52.000000 Scrapset-4.3.5/Scrapset.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-13 18:27:52.000000 Scrapset-4.3.5/Scrapset.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2023-07-13 18:27:52.000000 Scrapset-4.3.5/Scrapset.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-13 18:27:52.000000 Scrapset-4.3.5/Scrapset.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      632 2023-06-05 15:50:58.000000 Scrapset-4.3.5/licence.txt
--rw-rw-rw-   0        0        0      158 2023-07-13 18:27:52.862599 Scrapset-4.3.5/setup.cfg
--rw-rw-rw-   0        0        0      499 2023-07-13 18:27:05.000000 Scrapset-4.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 10:17:21.644474 Scrapset-5.3.1/
+-rw-rw-rw-   0        0        0     4648 2023-07-30 10:17:21.652452 Scrapset-5.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4417 2023-07-30 04:41:08.000000 Scrapset-5.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-30 10:17:21.620477 Scrapset-5.3.1/Scrapset/
+-rw-rw-rw-   0        0        0    11789 2023-07-30 10:13:44.000000 Scrapset-5.3.1/Scrapset/Scrapset.py
+-rw-rw-rw-   0        0        0       67 2023-07-30 10:14:01.000000 Scrapset-5.3.1/Scrapset/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-30 10:17:21.644474 Scrapset-5.3.1/Scrapset.egg-info/
+-rw-rw-rw-   0        0        0     4648 2023-07-30 10:17:21.000000 Scrapset-5.3.1/Scrapset.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2023-07-30 10:17:21.000000 Scrapset-5.3.1/Scrapset.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 10:17:21.000000 Scrapset-5.3.1/Scrapset.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-30 10:17:21.000000 Scrapset-5.3.1/Scrapset.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2023-07-30 10:17:21.000000 Scrapset-5.3.1/Scrapset.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-30 10:17:21.000000 Scrapset-5.3.1/Scrapset.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      632 2023-07-30 04:41:08.000000 Scrapset-5.3.1/licence.txt
+-rw-rw-rw-   0        0        0      158 2023-07-30 10:17:21.652452 Scrapset-5.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      499 2023-07-30 10:16:56.000000 Scrapset-5.3.1/setup.py
```

### Comparing `Scrapset-4.3.5/PKG-INFO` & `Scrapset-5.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Scrapset
-Version: 4.3.5
+Version: 5.3.1
 Summary: DataScraper: Effortless Dataset Extraction
 Author: Ibrahim
 Author-email: string2025@gmail.com
 Description-Content-Type: text/markdown
 License-File: licence.txt
 
 # Dataset Scraper (Scrapset)
```

### Comparing `Scrapset-4.3.5/README.md` & `Scrapset-5.3.1/README.md`

 * *Files identical despite different names*

### Comparing `Scrapset-4.3.5/Scrapset/Scrapset.py` & `Scrapset-5.3.1/Scrapset/Scrapset.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from selenium import webdriver
 from selenium.webdriver.common.by import By
+from selenium.webdriver.support.ui import WebDriverWait
+from selenium.webdriver.support import expected_conditions as EC
 import time
 import logging
 
 
 class KaggleDataSet:
     def web_driver_chrome(self):
         options = webdriver.ChromeOptions()
@@ -179,15 +181,14 @@
         return driver 
     def ai_jobs_net(self,url):
             try:
             
                 driver = self.web_driver_chrome()
                 self.url=url
                 time.sleep(1)
-                c=0
                 corpus=list()
                 driver.get(url)
                 while True:
                     cards=driver.find_elements(By.XPATH,'.//*[@id="job-list"]/li')
                     
                     try:
                         load_more_elements=driver.find_element(By.XPATH,'.//*[@id="load-more-jobs"]/a/h5')
@@ -199,8 +200,47 @@
                         time.sleep(1)
                     except:
                         break
                     
                 driver.quit()
                 return corpus  
             except:
-                 logging.error("Invalid url")
+                 logging.error("Invalid url")
+class imdb:
+    def web_driver_chrome(self):
+        options = webdriver.ChromeOptions()
+        options.add_argument("--verbose")
+        options.add_argument('--no-sandbox')
+        options.add_argument('--headless')
+        options.add_argument('--disable-gpu')
+        options.add_argument("--window-size=1920,1200")
+        options.add_argument('--disable-dev-shm-usage')
+        driver = webdriver.Chrome(options=options)
+        return driver
+    def comments(self,url):
+        try:
+            driver = webdriver.Chrome()
+            self.url=url
+
+            driver.get(url)
+
+            time.sleep(1)
+            corpus=[]
+            while True:
+                try:
+                    cards=driver.find_elements(By.XPATH,'//*[@id="main"]/section/div[2]/div[2]/div')
+                    for card in cards:
+                        corpus.append(card.text+'<>?')
+                    
+                    load_more_element = WebDriverWait(driver, 10).until(
+                        EC.element_to_be_clickable((By.XPATH, '//*[@id="load-more-trigger"]'))
+                    )
+                    load_more_element.click()
+
+                    time.sleep(1)  # Adjust this delay as needed
+
+                except:
+                     break
+            driver.quit()
+            return corpus  
+        except:
+                logging.error("Invalid url")
```

### Comparing `Scrapset-4.3.5/Scrapset.egg-info/PKG-INFO` & `Scrapset-5.3.1/Scrapset.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Scrapset
-Version: 4.3.5
+Version: 5.3.1
 Summary: DataScraper: Effortless Dataset Extraction
 Author: Ibrahim
 Author-email: string2025@gmail.com
 Description-Content-Type: text/markdown
 License-File: licence.txt
 
 # Dataset Scraper (Scrapset)
```

### Comparing `Scrapset-4.3.5/licence.txt` & `Scrapset-5.3.1/licence.txt`

 * *Files identical despite different names*

