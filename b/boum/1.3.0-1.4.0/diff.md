# Comparing `tmp/boum-1.3.0.tar.gz` & `tmp/boum-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boum-1.3.0.tar", max compression
+gzip compressed data, was "boum-1.4.0.tar", max compression
```

## Comparing `boum-1.3.0.tar` & `boum-1.4.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1061 2023-07-29 19:38:02.878848 boum-1.3.0/LICENSE
--rw-r--r--   0        0        0     5692 2023-07-29 19:38:02.878848 boum-1.3.0/README.md
--rw-r--r--   0        0        0      121 2023-07-29 19:38:02.878848 boum-1.3.0/boum/api_client/constants.py
--rw-r--r--   0        0        0    11200 2023-07-29 19:38:02.878848 boum-1.3.0/boum/api_client/v1/client.py
--rw-r--r--   0        0        0     7853 2023-07-29 19:38:02.878848 boum-1.3.0/boum/api_client/v1/endpoint.py
--rw-r--r--   0        0        0    14182 2023-07-29 19:38:02.878848 boum-1.3.0/boum/api_client/v1/models.py
--rw-r--r--   0        0        0     9431 2023-07-29 19:38:02.878848 boum-1.3.0/boum/resources/device.py
--rw-r--r--   0        0        0      982 2023-07-29 19:38:02.878848 boum-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     6570 1970-01-01 00:00:00.000000 boum-1.3.0/setup.py
--rw-r--r--   0        0        0     6276 1970-01-01 00:00:00.000000 boum-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-07-30 10:27:42.323078 boum-1.4.0/LICENSE
+-rw-r--r--   0        0        0     5692 2023-07-30 10:27:42.323078 boum-1.4.0/README.md
+-rw-r--r--   0        0        0      121 2023-07-30 10:27:42.323078 boum-1.4.0/boum/api_client/constants.py
+-rw-r--r--   0        0        0    11200 2023-07-30 10:27:42.323078 boum-1.4.0/boum/api_client/v1/client.py
+-rw-r--r--   0        0        0     7853 2023-07-30 10:27:42.323078 boum-1.4.0/boum/api_client/v1/endpoint.py
+-rw-r--r--   0        0        0    14485 2023-07-30 10:27:42.323078 boum-1.4.0/boum/api_client/v1/models.py
+-rw-r--r--   0        0        0     9431 2023-07-30 10:27:42.323078 boum-1.4.0/boum/resources/device.py
+-rw-r--r--   0        0        0      982 2023-07-30 10:27:42.327078 boum-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     6570 1970-01-01 00:00:00.000000 boum-1.4.0/setup.py
+-rw-r--r--   0        0        0     6276 1970-01-01 00:00:00.000000 boum-1.4.0/PKG-INFO
```

### Comparing `boum-1.3.0/LICENSE` & `boum-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `boum-1.3.0/README.md` & `boum-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `boum-1.3.0/boum/api_client/v1/client.py` & `boum-1.4.0/boum/api_client/v1/client.py`

 * *Files identical despite different names*

### Comparing `boum-1.3.0/boum/api_client/v1/endpoint.py` & `boum-1.4.0/boum/api_client/v1/endpoint.py`

 * *Files identical despite different names*

### Comparing `boum-1.3.0/boum/api_client/v1/models.py` & `boum-1.4.0/boum/api_client/v1/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,14 +186,15 @@
 
 @dataclass
 class DeviceFlagsModel(Model):
     poor_us: int | None = None
     poor_wifi: int | None = None
     draws_air: int | None = None
     water_leakage: int | None = None
+    water_level: int | None = None
     low_battery: int | None = None
     slow_recharge: int | None = None
     high_water_usage: int | None = None
     low_water_usage: int | None = None
     offline_warning: int | None = None
 
     def __post_init__(self):
@@ -202,14 +203,16 @@
             raise ValueError('poor_us must be a int or None')
         if not isinstance(self.poor_wifi, int | None):
             raise ValueError('poor_wifi must be a int or None')
         if not isinstance(self.draws_air, int | None):
             raise ValueError('draws_air must be a int or None')
         if not isinstance(self.water_leakage, int | None):
             raise ValueError('water_leakage must be a int or None')
+        if not isinstance(self.water_level, int | None):
+            raise ValueError('water_level must be a int or None')
         if not isinstance(self.low_battery, int | None):
             raise ValueError('low_battery must be a int or None')
         if not isinstance(self.slow_recharge, int | None):
             raise ValueError('slow_recharge must be a int or None')
         if not isinstance(self.high_water_usage, int | None):
             raise ValueError('high_water_usage must be a int or None')
         if not isinstance(self.low_water_usage, int | None):
@@ -223,14 +226,16 @@
             payload['poorUS'] = self.poor_us
         if self.poor_wifi is not None:
             payload['poorWiFi'] = self.poor_wifi
         if self.draws_air is not None:
             payload['drawsAir'] = self.draws_air
         if self.water_leakage is not None:
             payload['waterLeakage'] = self.water_leakage
+        if self.water_level is not None:
+            payload['waterLevel'] = self.water_level
         if self.low_battery is not None:
             payload['lowBattery'] = self.low_battery
         if self.slow_recharge is not None:
             payload['slowRecharge'] = self.slow_recharge
         if self.high_water_usage is not None:
             payload['highWaterUsage'] = self.high_water_usage
         if self.low_water_usage is not None:
@@ -242,14 +247,15 @@
     @staticmethod
     def from_payload(payload: dict[str, any]) -> 'DeviceFlagsModel':
         return DeviceFlagsModel(
             poor_us=payload.get('poorUS'),
             poor_wifi=payload.get('poorWiFi'),
             draws_air=payload.get('drawsAir'),
             water_leakage=payload.get('waterLeakage'),
+            water_level=payload.get('waterLevel'),
             low_battery=payload.get('lowBattery'),
             slow_recharge=payload.get('slowRecharge'),
             high_water_usage=payload.get('highWaterUsage'),
             low_water_usage=payload.get('lowWaterUsage'),
             offline_warning=payload.get('offlineWarning')
         )
```

### Comparing `boum-1.3.0/boum/resources/device.py` & `boum-1.4.0/boum/resources/device.py`

 * *Files identical despite different names*

### Comparing `boum-1.3.0/pyproject.toml` & `boum-1.4.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "boum"
-version = "1.3.0"
+version = "1.4.0"
 description = "SDK to interact with the boum API"
 authors = ["Marc Pfander <marc.pfander@boum.garden>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/boum-garden/sdk"
 
 [tool.poetry.dependencies]
@@ -24,15 +24,15 @@
 bandit = "^1.7.4"
 coverage = "^6.5.0"
 pytest-cov = "^4.0.0"
 pytest-xdist = "^3.1.0"
 regex = "^2023.6.3"
 
 [tool.bumpver]
-current_version = "1.3.0"
+current_version = "1.4.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `boum-1.3.0/setup.py` & `boum-1.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['requests>=2.28.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'boum',
-    'version': '1.3.0',
+    'version': '1.4.0',
     'description': 'SDK to interact with the boum API',
     'long_description': "# Boum Python SDK\nStatus: ![GitHub Actions](https://github.com/boum-garden/sdk/actions/workflows/deploy_on_semver_tag.yml/badge.svg)\n\n## Overview\nThis project provides an api client to interact with the [Boum API](https://api.boum.us/swagger) and abstractions to \nsimplify interactions with the underlying resources.\n\n\n## Installation\nThe package is available on PyPI, and can be installed with pip or similar tools:\n\n```bash\n    python -m pip install boum\n    poetry add boum\n    pipenv install boum\n    ...\n```\n\n## Usage\n\n### API Client\nThe API client models the topology of the API and provides a class hierarchy that is organized in the same way as the \nendpoint paths. Email and password or a token are required to use it.\n\nThe client can either connect to the API with `client.connect()` and `client.disconnect()`methods or it can be used \nas a context manager as `with client: ...` In the former case the disconnect method should be called explicitly in the\nend.\n\n```python\n>>> from boum.api_client.v1.client import ApiClient\n>>> from boum.api_client.v1.models import DeviceModel\n>>> \n>>> client = ApiClient(email, password, base_url=base_url)\n>>> # or ApiClient(refresh_token='token', base_url=base_url)\n>>>\n>>> with client:\n...     # Get call to the devices collection\n...     device_ids = client.root.devices.get()\n...     # Get call to a specific device \n...     device_states = client.root.devices(device_id).get()\n...     # Patch call to a specific device\n...     client.root.devices(device_id).patch(DeviceModel())\n...     # Get call to a devices data\n...     data = client.root.devices(device_id).data.get()\n\n```\n\n\n### Resource Abstractions\nThe resource abstractions provide a more intuitive interface to interact with the underlying resources.\n\n```python\n>>> from datetime import time, datetime, timedelta\n>>> import pandas as pd\n>>> from boum.api_client.v1.client import ApiClient\n>>> from boum.resources.device import Device\n>>> from boum.api_client.v1.models import DeviceStateModel\n>>>\n>>> client = ApiClient(email, password, base_url=base_url)\n>>> # or ApiClient(refresh_token='token', base_url=base_url)\n>>>\n>>> with client:\n...    # Get available device ids\n...    device_ids = Device.get_device_ids(client)\n...    # Create a device instance\n...    device = Device(device_id, client)\n...    # Remove device claim\n...    # device.unclaim()\n...    # Claim a device\n...    # device.claim()\n...    # Set desired device state\n...    desired_device_State = DeviceStateModel(\n...        pump_state=True,\n...        refill_time=time(3, 32),\n...        refill_interval_days=3,\n...        max_pump_duration_minutes=5\n...    )\n...    device.set_desired_device_state(desired_device_State)\n...    # Get reported and desired device state\n...    reported, desired = device.get_device_states()\n...    # Get device telemetry data\n...    data = device.get_telemetry_data(start=datetime.now() - timedelta(days=1),\n...        end=datetime.now())\n...    # Convert telemetry data to pandas dataframe\n...    df = pd.DataFrame(data)\n\n```\n\n### Jupyter Notebook Demo\nA Jupyter notebook demo is available [here](https://github.com/boum-garden/sdk/blob/638d62836f5b8b2f169d186170c679d6a813867a/doc/boum-sdk-demo.ipynb).\n\n### Loging\nThe SDK uses the standard python logging module.\n\n## Development\n\n### Dependecy management\n[Poetry](https://python-poetry.org/) is used for depency management and publishing.\n\n### Versioning\nVersioning is done using [bumpver](https://pypi.org/project/bumpver/) \nwith [semantic versioning](https://semver.org/)\nWhen the version is updated, a new tag is created and pushed to the remote repository.\n\n\n### Testing\n\n#### Unit tests\nThese are completely self-contained and have no external dependencies.\n\nIMPORTANT: There are fixtures that model the API responses and expected calls. These mnust be kept up to date with\nthe API, otherwise the unit tests will not test the correct behavior.\n\n#### End-to-end tests\nThese test the entire flow from user facing python classes to the underlying api calls. They require an instance \n(fake or real) of the API to run against. They also require a registered user with a clamied device.\nAPI Base URL, email and password are required as environmental variables.\n\n```bash\n    BOUM_SDK_TEST_BASE_URL\n    BOUM_SDK_TEST_EMAIL\n    BOUM_SDK_TEST_PASSWORD\n    BOUM_SDK_TEST_DEVICE_ID\n    BOUM_SDK_TEST_USER_ID\n```\n\n#### Doctests\n\nPart of the end-to-end tests are document tests executed using \n[doctest](https://docs.python.org/3/library/doctest.html). \nThese tests ensure that all the examples in this README and in the docstrings are up-to-date and working.\n\n\n## CI/CD\n\n### Integration\n\nThe GitHub action workflow `.github/workflows/checks_on_push_to_branch.yml` is triggered on every push on a branch\nexcept main. It provides the following checks:\n\n- Unit and end-to-end/contract tests with pytest\n- Linting with pylint\n- Security checks with bandit\n\nThe repository settings require that all checks pass before a pull request can be merged.\n\n### Deployment\n\nThe GitHub action workflow `.github/workflows/deploy_on_push_to_main.yml` is triggered on every push to main. It runs a\ntest deployment to the test PyPI repository.\n\nThe GitHub action workflow `.github/workflows/deploy_on_release.yml` is triggered on a tag with the format `v*.*.*` and\nruns a deployment to the production PyPI. It is recommended to set these tags using the GitHub release feature. \n\n\n## Technical debt\n\n- Doctest requires a specific format to make examples in documentation executable. This makes the examples in this\n  README harder to copy and paste. There exist other packages and add-ons that could be used to make the examples easier \n  to manage.\n\n\n\n\n\n\n",
     'author': 'Marc Pfander',
     'author_email': 'marc.pfander@boum.garden',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/boum-garden/sdk',
```

### Comparing `boum-1.3.0/PKG-INFO` & `boum-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boum
-Version: 1.3.0
+Version: 1.4.0
 Summary: SDK to interact with the boum API
 Home-page: https://github.com/boum-garden/sdk
 License: MIT
 Author: Marc Pfander
 Author-email: marc.pfander@boum.garden
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

