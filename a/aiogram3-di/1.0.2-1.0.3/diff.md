# Comparing `tmp/aiogram3_di-1.0.2.tar.gz` & `tmp/aiogram3_di-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiogram3_di-1.0.2.tar", last modified: Sat Jul 29 09:13:11 2023, max compression
+gzip compressed data, was "aiogram3_di-1.0.3.tar", last modified: Sun Jul 30 19:15:25 2023, max compression
```

## Comparing `aiogram3_di-1.0.2.tar` & `aiogram3_di-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-07-29 09:13:11.390751 aiogram3_di-1.0.2/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     1075 2023-01-01 13:29:08.000000 aiogram3_di-1.0.2/LICENSE
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     1650 2023-07-29 09:13:11.390751 aiogram3_di-1.0.2/PKG-INFO
--rw-rw-r--   0 vlad      (1000) vlad      (1000)      994 2023-07-29 09:11:26.000000 aiogram3_di-1.0.2/README.md
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-07-29 09:13:11.390751 aiogram3_di-1.0.2/aiogram3_di/
--rw-r--r--   0 vlad      (1000) vlad      (1000)      142 2023-07-28 19:36:21.000000 aiogram3_di-1.0.2/aiogram3_di/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)       22 2023-07-29 09:11:56.000000 aiogram3_di-1.0.2/aiogram3_di/_version.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)      289 2023-07-28 19:58:50.000000 aiogram3_di-1.0.2/aiogram3_di/depends.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)      628 2023-07-29 07:32:25.000000 aiogram3_di-1.0.2/aiogram3_di/middleware.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     3615 2023-07-29 07:46:05.000000 aiogram3_di-1.0.2/aiogram3_di/utils.py
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-07-29 09:13:11.390751 aiogram3_di-1.0.2/aiogram3_di.egg-info/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     1650 2023-07-29 09:13:11.000000 aiogram3_di-1.0.2/aiogram3_di.egg-info/PKG-INFO
--rw-rw-r--   0 vlad      (1000) vlad      (1000)      318 2023-07-29 09:13:11.000000 aiogram3_di-1.0.2/aiogram3_di.egg-info/SOURCES.txt
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        1 2023-07-29 09:13:11.000000 aiogram3_di-1.0.2/aiogram3_di.egg-info/dependency_links.txt
--rw-rw-r--   0 vlad      (1000) vlad      (1000)       17 2023-07-29 09:13:11.000000 aiogram3_di-1.0.2/aiogram3_di.egg-info/requires.txt
--rw-rw-r--   0 vlad      (1000) vlad      (1000)       12 2023-07-29 09:13:11.000000 aiogram3_di-1.0.2/aiogram3_di.egg-info/top_level.txt
--rw-rw-r--   0 vlad      (1000) vlad      (1000)       38 2023-07-29 09:13:11.390751 aiogram3_di-1.0.2/setup.cfg
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     1071 2023-07-29 09:13:00.000000 aiogram3_di-1.0.2/setup.py
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-07-30 19:15:25.177083 aiogram3_di-1.0.3/
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     1075 2023-01-01 13:29:08.000000 aiogram3_di-1.0.3/LICENSE
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     2050 2023-07-30 19:15:25.177083 aiogram3_di-1.0.3/PKG-INFO
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     1420 2023-07-30 18:50:20.000000 aiogram3_di-1.0.3/README.md
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-07-30 19:15:25.177083 aiogram3_di-1.0.3/aiogram3_di/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      142 2023-07-28 19:36:21.000000 aiogram3_di-1.0.3/aiogram3_di/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       22 2023-07-30 19:15:01.000000 aiogram3_di-1.0.3/aiogram3_di/_version.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      289 2023-07-28 19:58:50.000000 aiogram3_di-1.0.3/aiogram3_di/depends.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1046 2023-07-30 15:37:12.000000 aiogram3_di-1.0.3/aiogram3_di/middleware.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5568 2023-07-30 15:37:12.000000 aiogram3_di-1.0.3/aiogram3_di/utils.py
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-07-30 19:15:25.177083 aiogram3_di-1.0.3/aiogram3_di.egg-info/
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     2050 2023-07-30 19:15:25.000000 aiogram3_di-1.0.3/aiogram3_di.egg-info/PKG-INFO
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)      318 2023-07-30 19:15:25.000000 aiogram3_di-1.0.3/aiogram3_di.egg-info/SOURCES.txt
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)        1 2023-07-30 19:15:25.000000 aiogram3_di-1.0.3/aiogram3_di.egg-info/dependency_links.txt
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)       17 2023-07-30 19:15:25.000000 aiogram3_di-1.0.3/aiogram3_di.egg-info/requires.txt
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)       12 2023-07-30 19:15:25.000000 aiogram3_di-1.0.3/aiogram3_di.egg-info/top_level.txt
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)       38 2023-07-30 19:15:25.177083 aiogram3_di-1.0.3/setup.cfg
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     1044 2023-07-30 19:11:38.000000 aiogram3_di-1.0.3/setup.py
```

### Comparing `aiogram3_di-1.0.2/LICENSE` & `aiogram3_di-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aiogram3_di-1.0.2/PKG-INFO` & `aiogram3_di-1.0.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: aiogram3_di
-Version: 1.0.2
+Version: 1.0.3
 Summary: Dependency Injection implementation for aiogram 3.
 Home-page: https://github.com/Vladyslav49/aiogram3_di
 Author: Vladyslav49
 Author-email: 
 License: MIT
 Keywords: Aiogram,Telegram,Bots,DI,Dependency Injection
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ### Example of usage
 
 ```python
 import logging
@@ -50,14 +50,38 @@
     dp.run_polling(bot)
 
 
 if __name__ == '__main__':
     main()
 ```
 
+### Handler Dependencies.
+
+You can use `Depends` in the flags parameter of the handler, for example: 
+
+```python
+flags={'dependencies': [Depends(verify_user)]}
+```
+
+### Global Dependencies.
+
+You can use `Depends` in `dispatcher`, for example:
+
+```python
+dp = Dispatcher()
+dp.dependencies = [Depends(verify_user)]
+```
+
+Or in `router`, for example:
+
+```python
+router = Router()
+router.dependencies = [Depends(verify_user)]
+```
+
 ### Details
 
 It is inspired by [FastAPI](https://github.com/tiangolo/fastapi).
 
 If you define a normal def, your function will be called in a different thread.
 
 ### License
```

### Comparing `aiogram3_di-1.0.2/aiogram3_di.egg-info/PKG-INFO` & `aiogram3_di-1.0.3/aiogram3_di.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: aiogram3-di
-Version: 1.0.2
+Version: 1.0.3
 Summary: Dependency Injection implementation for aiogram 3.
 Home-page: https://github.com/Vladyslav49/aiogram3_di
 Author: Vladyslav49
 Author-email: 
 License: MIT
 Keywords: Aiogram,Telegram,Bots,DI,Dependency Injection
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ### Example of usage
 
 ```python
 import logging
@@ -50,14 +50,38 @@
     dp.run_polling(bot)
 
 
 if __name__ == '__main__':
     main()
 ```
 
+### Handler Dependencies.
+
+You can use `Depends` in the flags parameter of the handler, for example: 
+
+```python
+flags={'dependencies': [Depends(verify_user)]}
+```
+
+### Global Dependencies.
+
+You can use `Depends` in `dispatcher`, for example:
+
+```python
+dp = Dispatcher()
+dp.dependencies = [Depends(verify_user)]
+```
+
+Or in `router`, for example:
+
+```python
+router = Router()
+router.dependencies = [Depends(verify_user)]
+```
+
 ### Details
 
 It is inspired by [FastAPI](https://github.com/tiangolo/fastapi).
 
 If you define a normal def, your function will be called in a different thread.
 
 ### License
```

### Comparing `aiogram3_di-1.0.2/setup.py` & `aiogram3_di-1.0.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,22 +15,22 @@
   packages=['aiogram3_di'],
   version=version,
   license='MIT',
   description='Dependency Injection implementation for aiogram 3.',
   long_description=long_description,
   long_description_content_type='text/markdown',
   author='Vladyslav49',
+  python_requires='>=3.10',
   author_email='',
   url='https://github.com/Vladyslav49/aiogram3_di',
   keywords=['Aiogram', 'Telegram', 'Bots', 'DI', 'Dependency Injection'],
   install_requires=[
-          'aiogram>=3.0.0b7',
-      ],
+    'aiogram>=3.0.0b8',
+  ],
   classifiers=[
     'Intended Audience :: Developers',
     'Topic :: Software Development :: Libraries :: Python Modules',
     'License :: OSI Approved :: MIT License',
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
+    'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
   ],
 )
```

