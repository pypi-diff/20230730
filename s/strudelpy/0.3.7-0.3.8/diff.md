# Comparing `tmp/strudelpy-0.3.7.tar.gz` & `tmp/strudelpy-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strudelpy-0.3.7.tar", last modified: Tue Jul 25 00:36:53 2023, max compression
+gzip compressed data, was "strudelpy-0.3.8.tar", last modified: Sun Jul 30 01:32:27 2023, max compression
```

## Comparing `strudelpy-0.3.7.tar` & `strudelpy-0.3.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 harel     (1000) harel     (1000)        0 2023-07-25 00:36:53.199488 strudelpy-0.3.7/
--rw-rw-r--   0 harel     (1000) harel     (1000)     1077 2023-07-24 23:27:58.000000 strudelpy-0.3.7/LICENSE.txt
--rw-rw-r--   0 harel     (1000) harel     (1000)      854 2023-07-25 00:36:53.199488 strudelpy-0.3.7/PKG-INFO
--rw-rw-r--   0 harel     (1000) harel     (1000)     3155 2023-07-25 00:34:08.000000 strudelpy-0.3.7/README.md
--rw-rw-r--   0 harel     (1000) harel     (1000)       79 2023-07-25 00:36:53.199488 strudelpy-0.3.7/setup.cfg
--rw-rw-r--   0 harel     (1000) harel     (1000)     1094 2023-07-25 00:33:57.000000 strudelpy-0.3.7/setup.py
-drwxrwxr-x   0 harel     (1000) harel     (1000)        0 2023-07-25 00:36:53.195488 strudelpy-0.3.7/strudelpy/
--rw-rw-r--   0 harel     (1000) harel     (1000)    12923 2023-07-25 00:33:18.000000 strudelpy-0.3.7/strudelpy/__init__.py
-drwxrwxr-x   0 harel     (1000) harel     (1000)        0 2023-07-25 00:36:53.199488 strudelpy-0.3.7/strudelpy/tests/
--rw-rw-r--   0 harel     (1000) harel     (1000)        0 2023-07-24 23:27:58.000000 strudelpy-0.3.7/strudelpy/tests/__init__.py
--rw-rw-r--   0 harel     (1000) harel     (1000)     9572 2023-07-24 23:27:58.000000 strudelpy-0.3.7/strudelpy/tests/tests.py
-drwxrwxr-x   0 harel     (1000) harel     (1000)        0 2023-07-25 00:36:53.199488 strudelpy-0.3.7/strudelpy.egg-info/
--rw-rw-r--   0 harel     (1000) harel     (1000)      854 2023-07-25 00:36:53.000000 strudelpy-0.3.7/strudelpy.egg-info/PKG-INFO
--rw-rw-r--   0 harel     (1000) harel     (1000)      279 2023-07-25 00:36:53.000000 strudelpy-0.3.7/strudelpy.egg-info/SOURCES.txt
--rw-rw-r--   0 harel     (1000) harel     (1000)        1 2023-07-25 00:36:53.000000 strudelpy-0.3.7/strudelpy.egg-info/dependency_links.txt
--rw-rw-r--   0 harel     (1000) harel     (1000)        4 2023-07-25 00:36:53.000000 strudelpy-0.3.7/strudelpy.egg-info/requires.txt
--rw-rw-r--   0 harel     (1000) harel     (1000)       10 2023-07-25 00:36:53.000000 strudelpy-0.3.7/strudelpy.egg-info/top_level.txt
+drwxrwxr-x   0 harel     (1000) harel     (1000)        0 2023-07-30 01:32:27.103336 strudelpy-0.3.8/
+-rw-rw-r--   0 harel     (1000) harel     (1000)     1077 2023-07-24 23:27:58.000000 strudelpy-0.3.8/LICENSE.txt
+-rw-rw-r--   0 harel     (1000) harel     (1000)      854 2023-07-30 01:32:27.103336 strudelpy-0.3.8/PKG-INFO
+-rw-rw-r--   0 harel     (1000) harel     (1000)     3336 2023-07-30 01:23:31.000000 strudelpy-0.3.8/README.md
+-rw-rw-r--   0 harel     (1000) harel     (1000)       79 2023-07-30 01:32:27.103336 strudelpy-0.3.8/setup.cfg
+-rw-rw-r--   0 harel     (1000) harel     (1000)     1094 2023-07-28 14:27:30.000000 strudelpy-0.3.8/setup.py
+drwxrwxr-x   0 harel     (1000) harel     (1000)        0 2023-07-30 01:32:27.103336 strudelpy-0.3.8/strudelpy/
+-rw-rw-r--   0 harel     (1000) harel     (1000)    13268 2023-07-30 01:18:38.000000 strudelpy-0.3.8/strudelpy/__init__.py
+drwxrwxr-x   0 harel     (1000) harel     (1000)        0 2023-07-30 01:32:27.103336 strudelpy-0.3.8/strudelpy/tests/
+-rw-rw-r--   0 harel     (1000) harel     (1000)        0 2023-07-24 23:27:58.000000 strudelpy-0.3.8/strudelpy/tests/__init__.py
+-rw-rw-r--   0 harel     (1000) harel     (1000)     9572 2023-07-24 23:27:58.000000 strudelpy-0.3.8/strudelpy/tests/tests.py
+drwxrwxr-x   0 harel     (1000) harel     (1000)        0 2023-07-30 01:32:27.103336 strudelpy-0.3.8/strudelpy.egg-info/
+-rw-rw-r--   0 harel     (1000) harel     (1000)      854 2023-07-30 01:32:27.000000 strudelpy-0.3.8/strudelpy.egg-info/PKG-INFO
+-rw-rw-r--   0 harel     (1000) harel     (1000)      279 2023-07-30 01:32:27.000000 strudelpy-0.3.8/strudelpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 harel     (1000) harel     (1000)        1 2023-07-30 01:32:27.000000 strudelpy-0.3.8/strudelpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 harel     (1000) harel     (1000)        4 2023-07-30 01:32:27.000000 strudelpy-0.3.8/strudelpy.egg-info/requires.txt
+-rw-rw-r--   0 harel     (1000) harel     (1000)       10 2023-07-30 01:32:27.000000 strudelpy-0.3.8/strudelpy.egg-info/top_level.txt
```

### Comparing `strudelpy-0.3.7/LICENSE.txt` & `strudelpy-0.3.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `strudelpy-0.3.7/PKG-INFO` & `strudelpy-0.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strudelpy
-Version: 0.3.7
+Version: 0.3.8
 Summary: Easy as Pie Emails in Python
 Home-page: https://github.com/harel/strudelpy
 Author: Harel Malka
 Author-email: harel@harelmalka.com
 License: MIT
 Download-URL: https://github.com/harel/strudelpy/archive/0.3.tar.gz
 Keywords: email,smtp
```

### Comparing `strudelpy-0.3.7/README.md` & `strudelpy-0.3.8/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-## StrudelPy v0.3.7
+## StrudelPy v0.3.8
 ### A tastier way to send emails with Python
 
 ### Features
 * Attachments, multiple recipients, cc, bcc - the standard stuff
 * Embedded Images
 * Plays well with Unicode
 * Easy OOP approach
@@ -18,19 +18,23 @@
 ### TL;DR
 
 ```
 from strudelpy import SMTP, Email
 
 smtpclient = SMTP('smtp.example.com', 456, 'myuser', 'muchsecret', ssl=True)
 with smtpclient as smtp:
-    smtp.send(Email(sender='me@example.com,
-                     recipients=['him@example.com', 'her@example.com'],
-                     subject='The Subject Matters',
-                     text='Plain text body',
-                     html='HTML body'))
+    smtp.send(
+        Email(
+            sender='me@example.com,
+            recipients=['him@example.com', 'her@example.com'],
+            subject='The Subject Matters',
+            text='Plain text body',
+            html='HTML body'
+        )
+    )
 ```
 
 ### The 'Can Read' Version
 
 Strudelpy consists mainly of two objects: `SMTP` to manage connections to SMTP
 servers, and Email to encapsulate an email message.
 
@@ -73,17 +77,20 @@
 ```
 <img src="cid:filename.jpg">
 ```
 
 Look at the tests/tests.py file for examples.
 
 
-#### TLS Version
-(v0.3.5): to configure the TLS protocol version, set an env variable `EMAIL_TLS_VERSION`
-with either `PROTOCOL_TLSv1`, `PROTOCOL_TLSv1_1` or `PROTOCOL_TLSv1_2`. The default is `PROTOCOL_TLSv1_2`
+#### TLS
+(v0.3.8): It's possible to pass a specific TLS version (ssl.PROTOCOL_TLS*) to the SMTP 
+init, as well as function to work on the context if required (like setting min/max TLS versions, cert location etc.). By default the default context is generated. 
+
+`tls_version`: e.g. ssl.PROTOCOL_TLSv1_2
+`tls_context_handler`: Any function that receives SSLContext instance as first argument. 
 
 #### Tests
 
 This test suite relies on the existence of a SMTP server, real or fake to connect to.
 By default it will attempt to connect to a 'fake' one that can be run using:
 
 `sudo python -m smtpd -n -c DebuggingServer localhost:25`
```

### Comparing `strudelpy-0.3.7/setup.py` & `strudelpy-0.3.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='strudelpy',
-    version='0.3.7',
+    version='0.3.8',
     description='Easy as Pie Emails in Python',
     long_description='StrudelPy is an easy to use library to manage sending emails in a OO way.'
                      'The library is comprised of a SMTP object to manage connections to SMTP'
                      'servers and an Email object to handle the messages themselves.'
                      'Supports Python 2 and 3.',
     author='Harel Malka',
     author_email='harel@harelmalka.com',
```

### Comparing `strudelpy-0.3.7/strudelpy/__init__.py` & `strudelpy-0.3.8/strudelpy/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,24 +25,25 @@
 from email.mime.multipart import MIMEMultipart
 from email.header import Header
 from email.utils import formatdate, formataddr, make_msgid
 from email.encoders import encode_base64
 from email.charset import Charset
 
 __author__ = 'Harel Malka'
-__version__ = '0.3.7'
+__version__ = '0.3.8'
 
 # initialise the mimetypes module
 mimetypes.init()
 
 try:
-    PROTOCOL_TLS = getattr(ssl, os.environ.get('EMAIL_TLS_VERSION', 'PROTOCOL_TLSv1_2'))
+    PROTOCOL_TLS = getattr(ssl, os.environ.get('EMAIL_TLS_VERSION', 'PROTOCOL_TLS'))
 except AttributeError:
     PROTOCOL_TLS = getattr(ssl, 'PROTOCOL_TLS')
 
+
 class InvalidConfiguration(Exception):
     pass
 
 
 class SMTP(object):
     """
     A wrapper around SMTP accounts.
@@ -51,22 +52,26 @@
     use as a transport).
     However, a better usage pattern is via the `with` keyword:
 
     with smtp_instance as smtp:
         Email(...).send()
 
     """
-    def __init__(self, host, port, username=None, password=None, ssl=False, tls=False,
-                 timeout=None, debug_level=None):
+    def __init__(
+        self, host, port, username=None, password=None, ssl=False, tls=False,
+        timeout=None, debug_level=None, tls_version=None, tls_context_handler=None
+    ):
         self.host = host
         self.port = port
         self.username = username
         self.password = password
         self.ssl = ssl
         self.tls = tls
+        self.tls_version = tls_version
+        self.tls_context_handler = tls_context_handler
         self.timeout = timeout
         self.debug_level = debug_level
         self.client = None
 
     def __enter__(self):
         self.login()
         return self
@@ -85,18 +90,22 @@
         if self.timeout:
             connection_args['timeout'] = self.timeout
         if self.ssl:
             client = smtplib.SMTP_SSL(**connection_args)
         else:
             client = smtplib.SMTP(**connection_args)
         if self.tls:
-            context = ssl.SSLContext(PROTOCOL_TLS)
-            client.ehlo()
+            if self.tls_version:
+                context = ssl.SSLContext(self.tls_version)
+                if self.tls_context_handler:
+                    self.tls_context_handler(context)
+            else:
+                context = ssl.create_default_context()
             client.starttls(context=context)
-            client.ehlo()
+            client.ehlo_or_helo_if_needed()
         if self.debug_level:
             client.set_debuglevel(self.debug_level)
         return client
 
     def login(self):
         """
         Connect to the server using hte login (with credentials) or connect (without).
```

### Comparing `strudelpy-0.3.7/strudelpy/tests/tests.py` & `strudelpy-0.3.8/strudelpy/tests/tests.py`

 * *Files identical despite different names*

### Comparing `strudelpy-0.3.7/strudelpy.egg-info/PKG-INFO` & `strudelpy-0.3.8/strudelpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strudelpy
-Version: 0.3.7
+Version: 0.3.8
 Summary: Easy as Pie Emails in Python
 Home-page: https://github.com/harel/strudelpy
 Author: Harel Malka
 Author-email: harel@harelmalka.com
 License: MIT
 Download-URL: https://github.com/harel/strudelpy/archive/0.3.tar.gz
 Keywords: email,smtp
```

