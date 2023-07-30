# Comparing `tmp/smartrent.py-0.4.2.tar.gz` & `tmp/smartrent.py-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartrent.py-0.4.2.tar", max compression
+gzip compressed data, was "smartrent.py-0.4.3.tar", max compression
```

## Comparing `smartrent.py-0.4.2.tar` & `smartrent.py-0.4.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1071 2021-08-02 01:26:04.116665 smartrent.py-0.4.2/LICENSE.md
--rw-r--r--   0        0        0     5995 2023-07-20 04:26:47.992335 smartrent.py-0.4.2/README.md
--rw-r--r--   0        0        0      622 2023-07-20 02:30:41.380636 smartrent.py-0.4.2/pyproject.toml
--rw-r--r--   0        0        0      397 2022-09-24 23:36:24.499151 smartrent.py-0.4.2/smartrent/__init__.py
--rw-r--r--   0        0        0     4849 2023-07-20 04:26:47.994917 smartrent.py-0.4.2/smartrent/api.py
--rw-r--r--   0        0        0     4665 2023-04-02 19:13:33.849963 smartrent.py-0.4.2/smartrent/device.py
--rw-r--r--   0        0        0     1904 2023-07-20 02:30:02.433231 smartrent.py-0.4.2/smartrent/lock.py
--rw-r--r--   0        0        0     1187 2022-06-03 03:39:09.127111 smartrent.py-0.4.2/smartrent/sensor.py
--rw-r--r--   0        0        0     2976 2023-07-20 02:30:08.401732 smartrent.py-0.4.2/smartrent/switch.py
--rw-r--r--   0        0        0     5262 2023-07-20 02:28:03.084560 smartrent.py-0.4.2/smartrent/thermostat.py
--rw-r--r--   0        0        0    18181 2023-02-25 15:36:34.396014 smartrent.py-0.4.2/smartrent/utils.py
--rw-r--r--   0        0        0     6881 2023-07-20 04:26:48.683006 smartrent.py-0.4.2/setup.py
--rw-r--r--   0        0        0     6830 2023-07-20 04:26:48.683529 smartrent.py-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2021-08-02 01:26:04.116665 smartrent.py-0.4.3/LICENSE.md
+-rw-r--r--   0        0        0     5995 2023-07-30 20:49:48.694582 smartrent.py-0.4.3/README.md
+-rw-r--r--   0        0        0      622 2023-07-30 20:44:26.268017 smartrent.py-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0      397 2022-09-24 23:36:24.499151 smartrent.py-0.4.3/smartrent/__init__.py
+-rw-r--r--   0        0        0     4849 2023-07-30 20:49:48.696383 smartrent.py-0.4.3/smartrent/api.py
+-rw-r--r--   0        0        0     4665 2023-04-02 19:13:33.849963 smartrent.py-0.4.3/smartrent/device.py
+-rw-r--r--   0        0        0     1904 2023-07-20 02:30:02.433231 smartrent.py-0.4.3/smartrent/lock.py
+-rw-r--r--   0        0        0     1187 2022-06-03 03:39:09.127111 smartrent.py-0.4.3/smartrent/sensor.py
+-rw-r--r--   0        0        0     2976 2023-07-20 02:30:08.401732 smartrent.py-0.4.3/smartrent/switch.py
+-rw-r--r--   0        0        0     5228 2023-07-30 20:42:39.135199 smartrent.py-0.4.3/smartrent/thermostat.py
+-rw-r--r--   0        0        0    18181 2023-02-25 15:36:34.396014 smartrent.py-0.4.3/smartrent/utils.py
+-rw-r--r--   0        0        0     6881 2023-07-30 20:49:49.280356 smartrent.py-0.4.3/setup.py
+-rw-r--r--   0        0        0     6830 2023-07-30 20:49:49.280885 smartrent.py-0.4.3/PKG-INFO
```

### Comparing `smartrent.py-0.4.2/LICENSE.md` & `smartrent.py-0.4.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `smartrent.py-0.4.2/README.md` & `smartrent.py-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `smartrent.py-0.4.2/pyproject.toml` & `smartrent.py-0.4.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "smartrent.py"
-version = "0.4.2"
+version = "0.4.3"
 description = "Unofficial Python API for SmartRent devices"
 readme = "README.md"
 license = "MIT"
 authors = ["Zachery Thomas <zacherythomas12@gmail.com>"]
 repository = "https://github.com/zacherythomas/smartrent.py"
 documentation = "https://smartrentpy.readthedocs.io"
 packages = [
```

### Comparing `smartrent.py-0.4.2/smartrent/api.py` & `smartrent.py-0.4.3/smartrent/api.py`

 * *Files identical despite different names*

### Comparing `smartrent.py-0.4.2/smartrent/device.py` & `smartrent.py-0.4.3/smartrent/device.py`

 * *Files identical despite different names*

### Comparing `smartrent.py-0.4.2/smartrent/lock.py` & `smartrent.py-0.4.3/smartrent/lock.py`

 * *Files identical despite different names*

### Comparing `smartrent.py-0.4.2/smartrent/sensor.py` & `smartrent.py-0.4.3/smartrent/sensor.py`

 * *Files identical despite different names*

### Comparing `smartrent.py-0.4.2/smartrent/switch.py` & `smartrent.py-0.4.3/smartrent/switch.py`

 * *Files identical despite different names*

### Comparing `smartrent.py-0.4.2/smartrent/thermostat.py` & `smartrent.py-0.4.3/smartrent/thermostat.py`

 * *Files 3% similar despite different names*

```diff
@@ -146,31 +146,30 @@
     def _update_parser(self, event: dict) -> None:
         """
         Called when ``Client._async_update_state`` returns info
 
         ``event`` dict passed in from ``Client._async_update_state``
         """
         _LOGGER.info("Updating Thermostat")
-        last_read_state_str = str(event.get("last_read_state"))
-        last_read_state_int = int(float(last_read_state_str))
+        last_read_state = str(event.get("last_read_state"))
 
         if event.get("name") == "current_humidity":
             self._current_humidity = (
-                last_read_state_int
-                if last_read_state_int > 0
+                int(float(last_read_state))
+                if int(float(last_read_state)) > 0
                 else self._current_humidity
             )
 
         elif event.get("name") == "current_temp":
-            self._current_temp = last_read_state_int
+            self._current_temp = int(float(last_read_state))
 
         elif event.get("name") == "heating_setpoint":
-            self._heating_setpoint = last_read_state_int
+            self._heating_setpoint = int(float(last_read_state))
 
         elif event.get("name") == "cooling_setpoint":
-            self._cooling_setpoint = last_read_state_int
+            self._cooling_setpoint = int(float(last_read_state))
 
         elif event.get("name") == "mode":
-            self._mode = last_read_state_str
+            self._mode = last_read_state
 
         elif event.get("name") == "fan_mode":
-            self._fan_mode = last_read_state_str
+            self._fan_mode = last_read_state
```

### Comparing `smartrent.py-0.4.2/smartrent/utils.py` & `smartrent.py-0.4.3/smartrent/utils.py`

 * *Files identical despite different names*

### Comparing `smartrent.py-0.4.2/setup.py` & `smartrent.py-0.4.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['aiohttp>=3.8.4,<4.0.0', 'websockets>=11.0.1,<12.0.0']
 
 setup_kwargs = {
     'name': 'smartrent.py',
-    'version': '0.4.2',
+    'version': '0.4.3',
     'description': 'Unofficial Python API for SmartRent devices',
     'long_description': "# SmartRent API\n\n[![PyPI version][pypi-version-badge]](https://pypi.org/project/smartrent-py/)\n[![Supported Python versions][supported-versions-badge]](https://pypi.org/project/smartrent-py/)\n[![PyPI downloads monthly][m-downloads-badge]](https://pypistats.org/packages/smartrent-py)\n[![GitHub License][license-badge]](LICENSE.txt)\n[![Documentation Status][docs-badge]](https://smartrentpy.readthedocs.io/en/latest/?badge=latest)\n[![Code style: black][black-badge]](https://github.com/psf/black)\n\n`smartrent.py` is a simple library for SmartRent devices\n\nUses websockets for communication and supports async functions\n\nFeel free to ⭐️ this repo to get notified about the latest features!\n\n[📚 Read the docs! 📚](https://smartrentpy.readthedocs.io)\n## Supported Devices\nThis client supports:\n* 🔐 Door Locks\n* 🌡 Thermostats\n* 💧 Leak Sensors\n* 💡 Binary Switches\n* 🎚 Multilevel (Dimmer) Switches\n\n\n## Usage\n\n### Installation\n\n```bash\npip install smartrent.py\n```\n\n### Getting an API Object\nIn order to get an api object to interact with, you must login with the `async_login` function. This starts and handles a web session with SmartRent.\n\n```python\nimport asyncio\n\nfrom smartrent import async_login\n\nasync def main():\n    api = await async_login('<EMAIL>', '<PASSWORD>')\n\nasyncio.run(main())\n```\n\n### Getting Devices\nYou can get lists of your devices from the api with the `get_locks`, `get_thermostats`, `get_switches` and `get_leak_sensors` functions. You can then interact with the devices with their getter and setter functions.\n\n```python\nimport asyncio\n\nfrom smartrent import async_login\n\nasync def main():\n    api = await async_login('<EMAIL>', '<PASSWORD>')\n\n    lock = api.get_locks()[0]\n    locked = lock.get_locked()\n\n    if not locked:\n        await lock.async_set_locked(True)\n\nasyncio.run(main())\n```\n\n### Automatic Updating\nIf you need to get live updates to your device object from SmartRent, you can do that by calling `start_updater`. You can stop getting updates by calling `stop_updater`.\n\nYou can also set a callback function via `set_update_callback` that will be called when an update is triggered.\n\nFor example, if you want to set your thermostat to `Dad Mode` you can trigger an event every time the `cooling_setpoint` is changed and just change it back to your own desired value.\n```python\nimport asyncio\n\nfrom smartrent import async_login\n\nasync def main():\n    api = await async_login('<EMAIL>', '<PASSWORD>')\n\n    thermo = api.get_thermostats()[0]\n    thermo.start_updater()\n\n    CONSTANT_COOL = 80\n\n    async def on_evt():\n        if CONSTANT_COOL != thermo.get_cooling_setpoint():\n            await thermo.async_set_cooling_setpoint(CONSTANT_COOL)\n\n    thermo.set_update_callback(on_evt)\n\n    while True:\n        await asyncio.sleep(60)\n\nasyncio.run(main())\n```\n\n## Development\n### Setting up dev enviornment\n\n```\npip install -r requirements_test.txt\n```\n\n### Running the code formatter\n[Black](https://github.com/psf/black) is used for quick and easy code formatting\n\n```\nblack smartrent\n```\n\n## Special thanks\nMuch inspiration was taken from these projects:\n\n[AMcPherran/SmartRent-MQTT-Bridge](https://github.com/AMcPherran/SmartRent-MQTT-Bridge)\n\n[natanweinberger/smartrent-python](https://github.com/natanweinberger/smartrent-python)\n\n[Burry/homebridge-smartrent](https://github.com/Burry/homebridge-smartrent)\n## Versioning\n\nWe use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/your/project/tags).\n\n# Adding Unsupported Devices!\n\nThis library is built in a way that it is easy to add any smartrent device. If you find that one of the devices you own is not supported, we should be able to add it to this libray.\n\nTwo things are needed to get the info to add a new device:\n* We have to get some device info from smartrents api\n* We need to get info about how the device reacts when it enters different states\n\nBoth of these can be done in one script.\n\nYou have to run `python3 ./tools/device_helper.py`\n\nIt will print out some output and a table with `Device ID`s and `Device Names`. The device you wish to add should be listed in that table.\n```\nDevice ID:      Device Name:\n==============================\n2211234         Thermostat\n2212345         Front Door - Lock\n2212347         Washer - Leak Sensor\n```\n\nThe program will then ask for a `Device ID` that you wish to track. Enter in the `Device ID` you want to gather information from.\n\n```\nPut in the Device ID you wish to track: 2211234\nJoining topic for 2211234...\n{'response': {}, 'status': 'ok'}\n```\n\nYou can now change the state of your device either physically in your apartment/house or through the SmartRent app. For example, this is a thermostat's cooling point being turned up, and then the thermostat sending an update about the current humidity\n```\nThermostatSetpoint  cooling_setpoint    77\nMultiLvlSensor      current_humidity    53\n```\n\nOnce you get a good amount of info, open up an issue describing that you wish to add support for a new device and paste all of the output from `device_helper.py`. Feel free to hide your `Device ID`s if you wish.\n\n\n[pypi-version-badge]: https://img.shields.io/pypi/v/smartrent-py.svg?logo=pypi&logoColor=FFE873&style=for-the-badge\n[supported-versions-badge]: https://img.shields.io/pypi/pyversions/smartrent-py.svg?logo=python&logoColor=FFE873&style=for-the-badge\n[downloads-badge]: https://static.pepy.tech/personalized-badge/smartrent-py?period=total&units=international_system&left_color=grey&right_color=orange&left_text=total%20downloads&style=for-the-badge\n[m-downloads-badge]: https://img.shields.io/pypi/dm/smartrent-py.svg?style=for-the-badge\n[license-badge]: https://img.shields.io/github/license/ZacheryThomas/smartrent.py.svg?style=for-the-badge\n[docs-badge]: https://readthedocs.org/projects/smartrentpy/badge/?version=latest&style=for-the-badge\n[black-badge]: https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge\n",
     'author': 'Zachery Thomas',
     'author_email': 'zacherythomas12@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/zacherythomas/smartrent.py',
```

### Comparing `smartrent.py-0.4.2/PKG-INFO` & `smartrent.py-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartrent.py
-Version: 0.4.2
+Version: 0.4.3
 Summary: Unofficial Python API for SmartRent devices
 Home-page: https://github.com/zacherythomas/smartrent.py
 License: MIT
 Author: Zachery Thomas
 Author-email: zacherythomas12@gmail.com
 Requires-Python: >=3.6.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

