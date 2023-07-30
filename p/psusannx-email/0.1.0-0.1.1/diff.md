# Comparing `tmp/psusannx_email-0.1.0.tar.gz` & `tmp/psusannx_email-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psusannx_email-0.1.0.tar", last modified: Thu Mar 24 22:43:06 2022, max compression
+gzip compressed data, was "psusannx_email-0.1.1.tar", last modified: Sun Jul 30 21:08:38 2023, max compression
```

## Comparing `psusannx_email-0.1.0.tar` & `psusannx_email-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2022-03-24 22:43:06.326931 psusannx_email-0.1.0/
--rw-rw-rw-   0        0        0     1090 2022-03-24 22:10:42.000000 psusannx_email-0.1.0/LICENSE
--rw-rw-rw-   0        0        0       34 2022-03-24 22:10:55.000000 psusannx_email-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1690 2022-03-24 22:43:06.323592 psusannx_email-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1421 2022-03-24 22:30:55.000000 psusannx_email-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2022-03-24 22:43:06.298235 psusannx_email-0.1.0/psusannx_email/
--rw-rw-rw-   0        0        0       52 2022-03-24 22:03:52.000000 psusannx_email-0.1.0/psusannx_email/__init__.py
--rw-rw-rw-   0        0        0     1282 2022-03-24 22:26:48.000000 psusannx_email-0.1.0/psusannx_email/sendgrid_email.py
-drwxrwxrwx   0        0        0        0 2022-03-24 22:43:06.313860 psusannx_email-0.1.0/psusannx_email.egg-info/
--rw-rw-rw-   0        0        0     1690 2022-03-24 22:43:05.000000 psusannx_email-0.1.0/psusannx_email.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2022-03-24 22:43:06.000000 psusannx_email-0.1.0/psusannx_email.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-03-24 22:43:05.000000 psusannx_email-0.1.0/psusannx_email.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2022-03-24 22:43:05.000000 psusannx_email-0.1.0/psusannx_email.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2022-03-24 22:43:05.000000 psusannx_email-0.1.0/psusannx_email.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-03-24 22:43:06.327225 psusannx_email-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      705 2022-03-24 22:09:33.000000 psusannx_email-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 21:08:38.384994 psusannx_email-0.1.1/
+-rw-rw-rw-   0        0        0     1090 2022-03-24 22:10:42.000000 psusannx_email-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0       34 2022-03-24 22:10:55.000000 psusannx_email-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1734 2023-07-30 21:08:38.384994 psusannx_email-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1506 2023-07-30 20:29:02.000000 psusannx_email-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-30 21:08:38.366299 psusannx_email-0.1.1/psusannx_email/
+-rw-rw-rw-   0        0        0       52 2022-03-24 22:03:52.000000 psusannx_email-0.1.1/psusannx_email/__init__.py
+-rw-rw-rw-   0        0        0     1351 2023-07-30 20:04:57.000000 psusannx_email-0.1.1/psusannx_email/sendgrid_email.py
+drwxrwxrwx   0        0        0        0 2023-07-30 21:08:38.384994 psusannx_email-0.1.1/psusannx_email.egg-info/
+-rw-rw-rw-   0        0        0     1734 2023-07-30 21:08:38.000000 psusannx_email-0.1.1/psusannx_email.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2023-07-30 21:08:38.000000 psusannx_email-0.1.1/psusannx_email.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 21:08:38.000000 psusannx_email-0.1.1/psusannx_email.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-30 21:08:38.000000 psusannx_email-0.1.1/psusannx_email.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-30 21:08:38.000000 psusannx_email-0.1.1/psusannx_email.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-30 21:08:38.384994 psusannx_email-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      685 2023-07-30 20:37:54.000000 psusannx_email-0.1.1/setup.py
```

### Comparing `psusannx_email-0.1.0/LICENSE` & `psusannx_email-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `psusannx_email-0.1.0/PKG-INFO` & `psusannx_email-0.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: psusannx_email
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package with a function for sending emails easily using sendgrid.
 Author: Jamie O'Brien
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # psusannx_email
 
-A package that allows emails to be sent through a python function using [Sendgrid](https://www.sendgrid.com/), provided a valid [Sendgrid API Key](https://docs.sendgrid.com/ui/account-and-settings/api-keys#creating-an-api-key) is provided to the function.
+A package that allows emails to be sent through a python function using [Sendgrid](https://www.sendgrid.com/), provided a valid [Sendgrid API Key](https://docs.sendgrid.com/ui/account-and-settings/api-keys#creating-an-api-key) is passed as an argument to the function (`sendgrid_api_key`).
 
 The docs for using Sendgrid with python can be found [here](https://docs.sendgrid.com/for-developers/sending-email/quickstart-python).
 
 This package was created to be used as a subpackage in a wider project - PSUSANNX.
 
 ## Package Functions
 
@@ -26,31 +24,30 @@
 pip install psusannx-email
 ```
 
 ## Usage
 
 ```python
 # Import the function from the package
-from psusannx_email.sendgrid_email import send_email
+from psusannx_email import send_email
 
 # Get some info about the function
 help(send_email) 
 ```
 
 Now use the function to send an email.
 
 ```python
 # Send a test email from your own personal email (once you have a sendgrid api key)
 send_email(
-    subject='Test email using psusannx_email', 
-    body='This is a test email.\n\nThanks.',
-    from_email='<your-email>',
-    recipients=['<recipient-1>', '<recipient-2>']
-    )
+    subject="Test email using the psusannx_email package", 
+    body="This is a test email.\n\nThanks.",
+    from_email="<your-email>",
+    recipients=["<recipient-1>", "<recipient-2>"],
+    sendgrid_api_key="<verified-sendgrid-api-key>"
+)
 ```
 
 ## Notes
 
 - The package is quite restricted in what it can do, but it only needs to do things that are required by the parent project so there won't be much development.
-- A new feature that will be added is the abiloty to send emails where the body is html, rather than plain text.
-
-
+- A new feature that will be added is the ability to send emails where the body is html, rather than just plain text.
```

### Comparing `psusannx_email-0.1.0/README.md` & `psusannx_email-0.1.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # psusannx_email
 
-A package that allows emails to be sent through a python function using [Sendgrid](https://www.sendgrid.com/), provided a valid [Sendgrid API Key](https://docs.sendgrid.com/ui/account-and-settings/api-keys#creating-an-api-key) is provided to the function.
+A package that allows emails to be sent through a python function using [Sendgrid](https://www.sendgrid.com/), provided a valid [Sendgrid API Key](https://docs.sendgrid.com/ui/account-and-settings/api-keys#creating-an-api-key) is passed as an argument to the function (`sendgrid_api_key`).
 
 The docs for using Sendgrid with python can be found [here](https://docs.sendgrid.com/for-developers/sending-email/quickstart-python).
 
 This package was created to be used as a subpackage in a wider project - PSUSANNX.
 
 ## Package Functions
 
@@ -16,29 +16,30 @@
 pip install psusannx-email
 ```
 
 ## Usage
 
 ```python
 # Import the function from the package
-from psusannx_email.sendgrid_email import send_email
+from psusannx_email import send_email
 
 # Get some info about the function
 help(send_email) 
 ```
 
 Now use the function to send an email.
 
 ```python
 # Send a test email from your own personal email (once you have a sendgrid api key)
 send_email(
-    subject='Test email using psusannx_email', 
-    body='This is a test email.\n\nThanks.',
-    from_email='<your-email>',
-    recipients=['<recipient-1>', '<recipient-2>']
-    )
+    subject="Test email using the psusannx_email package", 
+    body="This is a test email.\n\nThanks.",
+    from_email="<your-email>",
+    recipients=["<recipient-1>", "<recipient-2>"],
+    sendgrid_api_key="<verified-sendgrid-api-key>"
+)
 ```
 
 ## Notes
 
 - The package is quite restricted in what it can do, but it only needs to do things that are required by the parent project so there won't be much development.
-- A new feature that will be added is the abiloty to send emails where the body is html, rather than plain text.
+- A new feature that will be added is the ability to send emails where the body is html, rather than just plain text.
```

### Comparing `psusannx_email-0.1.0/psusannx_email/sendgrid_email.py` & `psusannx_email-0.1.1/psusannx_email/sendgrid_email.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,41 @@
 import sendgrid
 from sendgrid.helpers.mail import Mail, Content
 
-def send_email(sendgrid_api_key, subject, body, from_email = 'psusann.01@gmail.com', recipients = ['jamie.o-brien@ucdconnect.ie']):
-
+def send_email(sendgrid_api_key: str, subject: str, body: str, from_email: str, recipients: list):
     """
-    A function to send emails using the sendgrid service
+    A function to send emails using the sendgrid service.
+    A valid sendgrid API keey needs to be passed for the function to work.
     
     Parameters
     ----------
-    subject: string
-        The subject of the email.
+    subject: The subject of the email.
         
-    body: string
-        The body of text for the email.
+    body: The body of text for the email.
 
-    from_email: string
-        The email to be used to send the email (this should be set up on the sendgrid website when setting up the sendgrid api key).
+    from_email: The email to be used to send the email 
+                (this should be set up on the sendgrid website when setting up the sendgrid api key).
 
-    recipients: list
-        A list of email addresses to send the email to.
+    recipients: A list of email addresses to send the email to.
+                Or just a string for a single recipient.
         
-    sendgrid_api_key: string
-        The verified sendgrid api key associated with the sender email.
+    sendgrid_api_key: The verified sendgrid api key associated with the sender email.
     
     Returns
     -------
     None
     """
     
     # Create the content to be sent in the email
     content = Content("text/plain", str(body))
     
     # Compile the email info as a Mail object
     mail = Mail(from_email, recipients, str(subject), content)
     
+    # Try to send the email
     try:
         sg = sendgrid.SendGridAPIClient(sendgrid_api_key)
         response = sg.client.mail.send.post(request_body=mail.get())
 
     except Exception as e:
         print("ERROR")
         print(e.message)
```

### Comparing `psusannx_email-0.1.0/psusannx_email.egg-info/PKG-INFO` & `psusannx_email-0.1.1/psusannx_email.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: psusannx-email
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package with a function for sending emails easily using sendgrid.
 Author: Jamie O'Brien
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # psusannx_email
 
-A package that allows emails to be sent through a python function using [Sendgrid](https://www.sendgrid.com/), provided a valid [Sendgrid API Key](https://docs.sendgrid.com/ui/account-and-settings/api-keys#creating-an-api-key) is provided to the function.
+A package that allows emails to be sent through a python function using [Sendgrid](https://www.sendgrid.com/), provided a valid [Sendgrid API Key](https://docs.sendgrid.com/ui/account-and-settings/api-keys#creating-an-api-key) is passed as an argument to the function (`sendgrid_api_key`).
 
 The docs for using Sendgrid with python can be found [here](https://docs.sendgrid.com/for-developers/sending-email/quickstart-python).
 
 This package was created to be used as a subpackage in a wider project - PSUSANNX.
 
 ## Package Functions
 
@@ -26,31 +24,30 @@
 pip install psusannx-email
 ```
 
 ## Usage
 
 ```python
 # Import the function from the package
-from psusannx_email.sendgrid_email import send_email
+from psusannx_email import send_email
 
 # Get some info about the function
 help(send_email) 
 ```
 
 Now use the function to send an email.
 
 ```python
 # Send a test email from your own personal email (once you have a sendgrid api key)
 send_email(
-    subject='Test email using psusannx_email', 
-    body='This is a test email.\n\nThanks.',
-    from_email='<your-email>',
-    recipients=['<recipient-1>', '<recipient-2>']
-    )
+    subject="Test email using the psusannx_email package", 
+    body="This is a test email.\n\nThanks.",
+    from_email="<your-email>",
+    recipients=["<recipient-1>", "<recipient-2>"],
+    sendgrid_api_key="<verified-sendgrid-api-key>"
+)
 ```
 
 ## Notes
 
 - The package is quite restricted in what it can do, but it only needs to do things that are required by the parent project so there won't be much development.
-- A new feature that will be added is the abiloty to send emails where the body is html, rather than plain text.
-
-
+- A new feature that will be added is the ability to send emails where the body is html, rather than just plain text.
```

### Comparing `psusannx_email-0.1.0/setup.py` & `psusannx_email-0.1.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,14 +7,12 @@
 
 # Set up the package metadata
 setup(
     name="psusannx_email",
     author="Jamie O'Brien",
     description="A package with a function for sending emails easily using sendgrid.",
     long_description=long_description,
-    long_description_content_type='text/markdown',
-    version="0.1.0",
+    long_description_content_type="text/markdown",
+    version="0.1.1",
     packages=find_packages(include=["psusannx_email", "psusannx_email.*"]),
-    install_requires=[
-        'sendgrid>=6.9.7'
-        ]
+    install_requires=["sendgrid>=6.9.7"]
 )
```

