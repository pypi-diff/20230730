# Comparing `tmp/millheater-0.8.1.tar.gz` & `tmp/millheater-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "millheater-0.8.1.tar", last modified: Wed Nov  3 05:38:07 2021, max compression
+gzip compressed data, was "millheater-0.9.0.tar", last modified: Fri Nov 19 07:47:49 2021, max compression
```

## Comparing `millheater-0.8.1.tar` & `millheater-0.9.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-03 05:38:07.993668 millheater-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1078 2021-11-03 05:37:55.000000 millheater-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      633 2021-11-03 05:38:07.993668 millheater-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1056 2021-11-03 05:37:55.000000 millheater-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-03 05:38:07.993668 millheater-0.8.1/mill/
--rw-r--r--   0 runner    (1001) docker     (121)    23911 2021-11-03 05:37:55.000000 millheater-0.8.1/mill/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-03 05:38:07.993668 millheater-0.8.1/millheater.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      633 2021-11-03 05:38:07.000000 millheater-0.8.1/millheater.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      212 2021-11-03 05:38:07.000000 millheater-0.8.1/millheater.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-03 05:38:07.000000 millheater-0.8.1/millheater.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       52 2021-11-03 05:38:07.000000 millheater-0.8.1/millheater.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2021-11-03 05:38:07.000000 millheater-0.8.1/millheater.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-03 05:38:07.993668 millheater-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      804 2021-11-03 05:37:55.000000 millheater-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-19 07:47:49.465632 millheater-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     1078 2021-11-19 07:47:36.000000 millheater-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      633 2021-11-19 07:47:49.461632 millheater-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1056 2021-11-19 07:47:36.000000 millheater-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-19 07:47:49.461632 millheater-0.9.0/mill/
+-rw-r--r--   0 runner    (1001) docker     (121)    24017 2021-11-19 07:47:36.000000 millheater-0.9.0/mill/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-19 07:47:49.461632 millheater-0.9.0/millheater.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      633 2021-11-19 07:47:49.000000 millheater-0.9.0/millheater.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      212 2021-11-19 07:47:49.000000 millheater-0.9.0/millheater.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-19 07:47:49.000000 millheater-0.9.0/millheater.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       52 2021-11-19 07:47:49.000000 millheater-0.9.0/millheater.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2021-11-19 07:47:49.000000 millheater-0.9.0/millheater.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-19 07:47:49.465632 millheater-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      804 2021-11-19 07:47:36.000000 millheater-0.9.0/setup.py
```

### Comparing `millheater-0.8.1/LICENSE` & `millheater-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `millheater-0.8.1/PKG-INFO` & `millheater-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: millheater
-Version: 0.8.1
+Version: 0.9.0
 Summary: A python3 library to communicate with Mill
 Home-page: https://github.com/Danielhiversen/pymill
 Author: Daniel Hjelseth Hoyer
 Author-email: mail@dahoiv.net
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `millheater-0.8.1/README.md` & `millheater-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `millheater-0.8.1/mill/__init__.py` & `millheater-0.9.0/mill/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
             "X-Zc-Msg-Name": "millService",
             "X-Zc-Sub-Domain": "milltype",
             "X-Zc-Seq-Id": "1",
             "X-Zc-Version": "1",
         }
         payload = {"account": self._username, "password": self._password}
         try:
-            with async_timeout.timeout(self._timeout):
+            async with async_timeout.timeout(self._timeout):
                 resp = await self.websession.post(
                     url, data=json.dumps(payload), headers=headers
                 )
         except (asyncio.TimeoutError, aiohttp.ClientError):
             if retry < 1:
                 _LOGGER.error("Error connecting to Mill", exc_info=True)
                 return False
@@ -122,15 +122,15 @@
         """Request data."""
         # pylint: disable=too-many-return-statements
 
         if self._token is None:
             _LOGGER.error("No token")
             return None
 
-        _LOGGER.debug(command, payload)
+        _LOGGER.debug("Request %s %s", command, payload)
 
         nonce = "".join(
             random.choice(string.ascii_uppercase + string.digits) for _ in range(16)
         )
         url = API_ENDPOINT_2 + command
         timestamp = int(time.time())
         signature = hashlib.sha1(
@@ -149,30 +149,30 @@
             "X-Zc-Timeout": REQUEST_TIMEOUT,
             "X-Zc-Nonce": nonce,
             "X-Zc-User-Id": str(self._user_id),
             "X-Zc-User-Signature": signature,
             "X-Zc-Content-Length": str(len(payload)),
         }
         try:
-            with async_timeout.timeout(self._timeout):
+            async with async_timeout.timeout(self._timeout):
                 resp = await self.websession.post(
                     url, data=json.dumps(payload), headers=headers
                 )
         except asyncio.TimeoutError:
             if retry < 1:
                 _LOGGER.error("Timed out sending command to Mill: %s", command)
                 return None
             return await self.request(command, payload, retry - 1)
         except aiohttp.ClientError:
             _LOGGER.error("Error sending command to Mill: %s", command, exc_info=True)
             return None
 
         result = await resp.text()
 
-        _LOGGER.debug(result)
+        _LOGGER.debug("Result %s", result)
 
         if not result or result == '{"errorCode":0}':
             return None
 
         if "access token expire" in result or "invalid signature" in result:
             if retry < 1:
                 return None
@@ -192,15 +192,15 @@
             _LOGGER.error("Failed to send request, %s", result)
             return None
         data = json.loads(result)
         return data
 
     async def request_stats(self, command, payload, retry=3):
         """Request data."""
-        _LOGGER.debug(command, payload)
+        _LOGGER.debug("Request stats %s %s", command, payload)
         url = API_ENDPOINT_STATS + command
         json_data = json.dumps(payload)
         token = str(int(time.time() * 1000)) + "_" + str(self._user_id)
         padder = padding.PKCS7(128).padder()
         data = padder.update(token.encode()) + padder.finalize()
         encryptor = self._cipher.encryptor()
         milltoken = b64encode(encryptor.update(data) + encryptor.finalize())
@@ -210,30 +210,30 @@
             "accept-language": "en-US,en;q=0.8",
             "connection": "Keep-Alive",
             "content-length": str(len(json_data)),
             "content-type": "application/json",
             "milltoken": milltoken.decode(),
         }
         try:
-            with async_timeout.timeout(self._timeout):
+            async with async_timeout.timeout(self._timeout):
                 resp = await self.websession.post(url, data=json_data, headers=headers)
         except asyncio.TimeoutError:
             if retry < 1:
                 _LOGGER.error("Timed out sending stats command to Mill: %s", command)
                 return None
             return await self.request_stats(command, payload, retry - 1)
         except aiohttp.ClientError:
             _LOGGER.error(
                 "Error sending stats command to Mill: %s", command, exc_info=True
             )
             return None
 
         result = await resp.text()
 
-        _LOGGER.debug(result)
+        _LOGGER.debug("Result %s", result)
         data = json.loads(result)
         return data
 
     async def get_home_list(self):
         """Request data."""
         resp = await self.request("selectHomeList", "{}")
         if resp is None:
@@ -414,15 +414,17 @@
         set_heater_values(_heater, heater)
         self.heaters[heater.device_id] = heater
 
     async def _update_consumption(self, heater):
         now = dt.datetime.now(dt.timezone.utc)
         if heater.last_updated and (
             now - heater.last_updated
-        ) < MIN_TIME_BETWEEN_STATS_UPDATES + dt.timedelta(seconds=random.randint(0, 60)):
+        ) < MIN_TIME_BETWEEN_STATS_UPDATES + dt.timedelta(
+            seconds=random.randint(0, 60)
+        ):
             return
 
         payload = {
             "dateType": None,
             "dateStr": now.strftime("%Y-%m-%d"),
             "timeZone": "GMT+02:00",
             "haveSensor": 1,
```

### Comparing `millheater-0.8.1/millheater.egg-info/PKG-INFO` & `millheater-0.9.0/millheater.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: millheater
-Version: 0.8.1
+Version: 0.9.0
 Summary: A python3 library to communicate with Mill
 Home-page: https://github.com/Danielhiversen/pymill
 Author: Daniel Hjelseth Hoyer
 Author-email: mail@dahoiv.net
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `millheater-0.8.1/setup.py` & `millheater-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 setup(
     name="millheater",
     packages=["mill"],
-    install_requires=["aiohttp>=3.7.4,<4", "async_timeout>=1.4.0", "cryptography"],
-    version="0.8.1",
+    install_requires=["aiohttp>=3.7.4,<4", "async_timeout>=3.0.0", "cryptography"],
+    version="0.9.0",
     description="A python3 library to communicate with Mill",
     long_description="A python3 library to communicate with Mill",
     python_requires=">=3.5.3",
     author="Daniel Hjelseth Hoyer",
     author_email="mail@dahoiv.net",
     url="https://github.com/Danielhiversen/pymill",
     license="MIT",
```

