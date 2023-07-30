# Comparing `tmp/dbtc-0.5.0.tar.gz` & `tmp/dbtc-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbtc-0.5.0.tar", max compression
+gzip compressed data, was "dbtc-0.5.1.tar", max compression
```

## Comparing `dbtc-0.5.0.tar` & `dbtc-0.5.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     3872 2023-07-28 12:01:04.602736 dbtc-0.5.0/README.md
--rw-r--r--   0        0        0      124 2023-07-28 12:01:04.602736 dbtc-0.5.0/dbtc/__init__.py
--rw-r--r--   0        0        0       22 2023-07-28 12:01:04.606736 dbtc-0.5.0/dbtc/_version.py
--rw-r--r--   0        0        0    37445 2023-07-28 12:01:04.606736 dbtc-0.5.0/dbtc/cli.py
--rw-r--r--   0        0        0        0 2023-07-28 12:01:04.606736 dbtc-0.5.0/dbtc/client/__init__.py
--rw-r--r--   0        0        0    64405 2023-07-28 12:01:04.606736 dbtc-0.5.0/dbtc/client/admin.py
--rw-r--r--   0        0        0   352525 2023-07-28 12:01:04.606736 dbtc-0.5.0/dbtc/client/artifacts/metadata_schema.json
--rw-r--r--   0        0        0     2349 2023-07-28 12:01:04.606736 dbtc-0.5.0/dbtc/client/base.py
--rw-r--r--   0        0        0      258 2023-07-28 12:01:04.606736 dbtc-0.5.0/dbtc/client/main.py
--rw-r--r--   0        0        0    24548 2023-07-28 12:01:04.606736 dbtc-0.5.0/dbtc/client/metadata.py
--rw-r--r--   0        0        0    62305 2023-07-28 12:01:04.606736 dbtc-0.5.0/dbtc/client/schema.py
--rw-r--r--   0        0        0      103 2023-07-28 12:01:04.606736 dbtc-0.5.0/dbtc/console.py
--rw-r--r--   0        0        0       44 2023-07-28 12:01:04.606736 dbtc-0.5.0/dbtc/models/__init__.py
--rw-r--r--   0        0        0      524 2023-07-28 12:01:04.606736 dbtc-0.5.0/dbtc/models/webhooks.py
--rw-r--r--   0        0        0      428 2023-07-28 12:01:04.606736 dbtc-0.5.0/dbtc/utils.py
--rw-r--r--   0        0        0      905 2023-07-28 12:01:19.090560 dbtc-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     4731 1970-01-01 00:00:00.000000 dbtc-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     3827 2023-07-30 13:05:07.582308 dbtc-0.5.1/README.md
+-rw-r--r--   0        0        0      124 2023-07-30 13:05:07.582308 dbtc-0.5.1/dbtc/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-30 13:05:07.582308 dbtc-0.5.1/dbtc/_version.py
+-rw-r--r--   0        0        0    39135 2023-07-30 13:05:07.582308 dbtc-0.5.1/dbtc/cli.py
+-rw-r--r--   0        0        0        0 2023-07-30 13:05:07.582308 dbtc-0.5.1/dbtc/client/__init__.py
+-rw-r--r--   0        0        0    67683 2023-07-30 13:05:07.582308 dbtc-0.5.1/dbtc/client/admin.py
+-rw-r--r--   0        0        0   352525 2023-07-30 13:05:07.582308 dbtc-0.5.1/dbtc/client/artifacts/metadata_schema.json
+-rw-r--r--   0        0        0     2349 2023-07-30 13:05:07.582308 dbtc-0.5.1/dbtc/client/base.py
+-rw-r--r--   0        0        0      258 2023-07-30 13:05:07.582308 dbtc-0.5.1/dbtc/client/main.py
+-rw-r--r--   0        0        0    24548 2023-07-30 13:05:07.582308 dbtc-0.5.1/dbtc/client/metadata.py
+-rw-r--r--   0        0        0    62305 2023-07-30 13:05:07.586309 dbtc-0.5.1/dbtc/client/schema.py
+-rw-r--r--   0        0        0      103 2023-07-30 13:05:07.586309 dbtc-0.5.1/dbtc/console.py
+-rw-r--r--   0        0        0       44 2023-07-30 13:05:07.586309 dbtc-0.5.1/dbtc/models/__init__.py
+-rw-r--r--   0        0        0      524 2023-07-30 13:05:07.586309 dbtc-0.5.1/dbtc/models/webhooks.py
+-rw-r--r--   0        0        0      428 2023-07-30 13:05:07.586309 dbtc-0.5.1/dbtc/utils.py
+-rw-r--r--   0        0        0      905 2023-07-30 13:05:25.415146 dbtc-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     4686 1970-01-01 00:00:00.000000 dbtc-0.5.1/PKG-INFO
```

### Comparing `dbtc-0.5.0/README.md` & `dbtc-0.5.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 **Interactive Demo**: <a target="_blank" href="https://dpguthrie-dbtc-streamlit-home-yy7c0b.streamlit.app/">https://dpguthrie-dbtc-streamlit-home-yy7c0b.streamlit.app/</a>
 
 **Source Code**: <a target="_blank" href="https://github.com/dpguthrie/dbtc">https://github.com/dpguthrie/dbtc</a>
 
 **V2 Docs**: <a target="_blank" href="https://docs.getdbt.com/dbt-cloud/api-v2">https://docs.getdbt.com/dbt-cloud/api-v2</a>
 
-**V3 Docs (Unofficial)**: <a target="_blank" href="https://documenter.getpostman.com/view/14183654/UVsSNiXC">https://documenter.getpostman.com/view/14183654/UVsSNiXC</a>
+**V3 Docs**: <a target="_blank" href="https://docs.getdbt.com/dbt-cloud/api-v3">https://docs.getdbt.com/dbt-cloud/api-v3</a>
 
 ---
 
 ## Overview
 
 dbtc is an unaffiliated python interface to various dbt Cloud API endpoints.
```

#### html2text {}

```diff
@@ -1,40 +1,40 @@
                          [docs/img/dbt-standalone.png]
               An unaffiliated python interface for dbt Cloud APIs
                    [Coverage] [Package_version] [Downloads]
 --- **Documentation**: https://dbtc.dpguthrie.com **Interactive Demo**: https:/
 /dpguthrie-dbtc-streamlit-home-yy7c0b.streamlit.app/ **Source Code**: https://
 github.com/dpguthrie/dbtc **V2 Docs**: https://docs.getdbt.com/dbt-cloud/api-v2
-**V3 Docs (Unofficial)**: https://documenter.getpostman.com/view/14183654/
-UVsSNiXC --- ## Overview dbtc is an unaffiliated python interface to various
-dbt Cloud API endpoints. This library acts as a convenient interface to two
-different APIs that dbt Cloud offers: - Cloud API: This is a REST API that
-exposes endpoints that allow users to programatically create, read, update, and
-delete resources within their dbt Cloud Account. - Metadata API: This is a
-GraphQL API that exposes metadata generated from a job run within dbt Cloud. ##
-Requirements Python 3.7+ - [Requests](https://requests.readthedocs.io/en/
-master/) - The elegant and simple HTTP library for Python, built for human
-beings. - [sgqlc](https://github.com/profusion/sgqlc) - Simple GraphQL Client -
-[Typer](https://github.com/tiangolo/typer) - Library for building CLI
-applications ## Installation ```bash pip install dbtc ``` ## Basic Usage ###
-Python The interface to both APIs are located in the `dbtCloudClient` class.
-The example below shows how you use the `cloud` property on an instance of the
-`dbtCloudClient` class to to access a method, `trigger_job_from_failure`, that
-allows you to restart a job from its last point of failure. ```python from dbtc
-import dbtCloudClient # Assumes that DBT_CLOUD_SERVICE_TOKEN env var is set
-client = dbtCloudClient() account_id = 1 job_id = 1 payload = {'cause':
-'Restarting from failure'} run = client.cloud.trigger_job_from_failure
-( account_id, job_id, payload, should_poll=False, ) # This returns a dictionary
-containing two keys run['data'] run['status'] ``` Similarly, use the `metadata`
-property to retrieve information about certain resources within your project -
-the example below shows how to retrieve metadata from models related to the
-most recent run for a given `job_id`. ```python from dbtc import dbtCloudClient
-client = dbtCloudClient() job_id = 1 models = client.metadata.get_models
-(job_id) # Models nested inside a couple keys models['data']['models'] # This
-is a list models['data']['models'][0] ``` ### CLI The CLI example below will
-map to the python cloud example above: ```bash dbtc trigger-job-from-failure \
---account-id 1 \ --job-id 1 \ --payload '{"cause": "Restarting from failure"}'
-\ --no-should-poll ``` Similarly, for the metadata example above: ```bash dbtc
-get-models --job-id 1 ``` If not setting your service token as an environment
+**V3 Docs**: https://docs.getdbt.com/dbt-cloud/api-v3 --- ## Overview dbtc is
+an unaffiliated python interface to various dbt Cloud API endpoints. This
+library acts as a convenient interface to two different APIs that dbt Cloud
+offers: - Cloud API: This is a REST API that exposes endpoints that allow users
+to programatically create, read, update, and delete resources within their dbt
+Cloud Account. - Metadata API: This is a GraphQL API that exposes metadata
+generated from a job run within dbt Cloud. ## Requirements Python 3.7+ -
+[Requests](https://requests.readthedocs.io/en/master/) - The elegant and simple
+HTTP library for Python, built for human beings. - [sgqlc](https://github.com/
+profusion/sgqlc) - Simple GraphQL Client - [Typer](https://github.com/tiangolo/
+typer) - Library for building CLI applications ## Installation ```bash pip
+install dbtc ``` ## Basic Usage ### Python The interface to both APIs are
+located in the `dbtCloudClient` class. The example below shows how you use the
+`cloud` property on an instance of the `dbtCloudClient` class to to access a
+method, `trigger_job_from_failure`, that allows you to restart a job from its
+last point of failure. ```python from dbtc import dbtCloudClient # Assumes that
+DBT_CLOUD_SERVICE_TOKEN env var is set client = dbtCloudClient() account_id = 1
+job_id = 1 payload = {'cause': 'Restarting from failure'} run =
+client.cloud.trigger_job_from_failure( account_id, job_id, payload,
+should_poll=False, ) # This returns a dictionary containing two keys run
+['data'] run['status'] ``` Similarly, use the `metadata` property to retrieve
+information about certain resources within your project - the example below
+shows how to retrieve metadata from models related to the most recent run for a
+given `job_id`. ```python from dbtc import dbtCloudClient client =
+dbtCloudClient() job_id = 1 models = client.metadata.get_models(job_id) #
+Models nested inside a couple keys models['data']['models'] # This is a list
+models['data']['models'][0] ``` ### CLI The CLI example below will map to the
+python cloud example above: ```bash dbtc trigger-job-from-failure \ --account-
+id 1 \ --job-id 1 \ --payload '{"cause": "Restarting from failure"}' \ --no-
+should-poll ``` Similarly, for the metadata example above: ```bash dbtc get-
+models --job-id 1 ``` If not setting your service token as an environment
 variable, do the following: ```bash dbtc --token this_is_my_token get_models --
 job-id 1 ``` ## License This project is licensed under the terms of the MIT
 license.
```

### Comparing `dbtc-0.5.0/dbtc/cli.py` & `dbtc-0.5.1/dbtc/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -925,14 +925,66 @@
     project_id: int = PROJECT_ID,
 ):
     """List credentials for a specific account and project."""
     _dbt_cloud_request(ctx, 'list_credentials', account_id, project_id)
 
 
 @app.command()
+def list_environment_variables(
+    ctx: typer.Context,
+    account_id: int = ACCOUNT_ID,
+    project_id: int = PROJECT_ID,
+    resource_type: str = typer.Option(
+        'environment',
+        '--resource-type',
+        help='The name of the resource to retrieve',
+    ),
+    environment_id: int = typer.Option(
+        None,
+        '--environment-id',
+        help='Numeric ID of the environment to retrieve',
+    ),
+    job_id: int = typer.Option(
+        None,
+        '--job-id',
+        help='Numeric ID of the job to retrieve',
+    ),
+    user_id: int = typer.Option(None, '--user-id', '-u', help='Numeric ID of the user'),
+    name: str = typer.Option(
+        None,
+        '--name',
+        help='The name of the environment',
+    ),
+    type: str = typer.Option(
+        None,
+        '--type',
+        help='The type of environment (deployment or development)',
+    ),
+    state: str = STATE,
+    offset: int = OFFSET,
+    limit: int = LIMIT,
+):
+    _dbt_cloud_request(
+        ctx,
+        'list_environment_variables',
+        account_id,
+        project_id,
+        resource_type=resource_type,
+        environment_id=environment_id,
+        job_id=job_id,
+        user_id=user_id,
+        name=name,
+        type=type,
+        state=state,
+        offset=offset,
+        limit=limit,
+    )
+
+
+@app.command()
 def list_environments(
     ctx: typer.Context,
     account_id: int = ACCOUNT_ID,
     project_id: str = typer.Option(
         None, '--project-id', '-p', help='The project ID or IDs'
     ),
     dbt_version: str = typer.Option(
@@ -1358,14 +1410,31 @@
         project_id,
         environment_id,
         json.loads(payload),
     )
 
 
 @app.command()
+def update_environment_variables(
+    ctx: typer.Context,
+    account_id: int = ACCOUNT_ID,
+    project_id: int = PROJECT_ID,
+    payload: str = PAYLOAD,
+):
+    """Update environment variables."""
+    _dbt_cloud_request(
+        ctx,
+        'update_environment_variables',
+        account_id,
+        project_id,
+        json.loads(payload),
+    )
+
+
+@app.command()
 def update_job(
     ctx: typer.Context,
     account_id: int = ACCOUNT_ID,
     job_id: int = JOB_ID,
     payload: str = PAYLOAD,
 ):
     """Update the definition of an existing job."""
```

### Comparing `dbtc-0.5.0/dbtc/client/admin.py` & `dbtc-0.5.1/dbtc/client/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -882,23 +882,37 @@
                 'logged_at_end': logged_at_end,
                 'offset': offset,
                 'limit': limit,
             },
         )
 
     @v3
-    def list_connections(self, account_id: int, project_id: int) -> Dict:
+    def list_connections(
+        self,
+        account_id: int,
+        project_id: int,
+        *,
+        state: int = None,
+        offset: int = None,
+        limit: int = None,
+    ) -> Dict:
         """List connections for a specific account and project
 
         Args:
             account_id (int): Numeric ID of the account to retrieve
             project_id (int): Numeric ID of the project to retrieve
+            state (int, optional): 1 = active, 2 = deleted
+            offset (int, optional): The offset to apply when listing runs.
+                Use with limit to paginate results.
+            limit (int, optional): The limit to apply when listing runs.
+                Use with offset to paginate results.
         """
         return self._simple_request(
-            f'accounts/{account_id}/projects/{project_id}/connections'
+            f'accounts/{account_id}/projects/{project_id}/connections',
+            params={'state': state, 'limit': limit, 'offset': offset},
         )
 
     @v3
     def list_credentials(self, account_id: int, project_id: int) -> Dict:
         """List credentials for a specific account and project
 
         Args:
@@ -959,14 +973,68 @@
                 'offset': offset,
                 'limit': limit,
                 'order_by': order_by,
             },
         )
 
     @v3
+    def list_environment_variables(
+        self,
+        account_id: int,
+        project_id: int,
+        *,
+        resource_type: str = 'environment',
+        environment_id: int = None,
+        job_id: int = None,
+        limit: int = None,
+        offset: int = None,
+        name: str = None,
+        state: int = None,
+        type: str = None,
+        user_id: int = None,
+    ):
+        """List environment variables for a specific account and project
+
+        Args:
+            account_id (int): Numeric ID of the account to retrieve
+            project_id (int): Numeric ID of he project to retrieve
+            resource_type (str, optional): The name of the resource to retrieve. Valid
+                resources include environment, job, and user
+            environment_id (int, optional): Numeric ID of the environment to retrieve
+            job_id (int, optional): Numeric ID of the job to retrieve
+            name (str, optional): Name of the environment to retrieve
+            type (str, optional): Type of the environment variable
+            state (int, optional): 1 = active, 2 = deleted
+            offset (int, optional): The offset to apply when listing runs.
+                Use with limit to paginate results.
+            limit (int, optional): The limit to apply when listing runs.
+                Use with offset to paginate results.
+        """
+        valid_resource_types = ['environment', 'job', 'user']
+        if resource_type not in valid_resource_types:
+            raise ValueError(
+                f'{resource_type} is not a valid argument for resource_type.  Valid '
+                f'resource types include {", ".join(valid_resource_types)}.'
+            )
+
+        return self._simple_request(
+            f'accounts/{account_id}/projects/{project_id}/environment-variables/{resource_type}',  # noqa: E501
+            params={
+                'environment_id': environment_id,
+                'job_definition_id': job_id,
+                'name': name,
+                'type': type,
+                'state': state,
+                'offset': offset,
+                'limit': limit,
+                'user_id': user_id,
+            },
+        )
+
+    @v3
     def list_feature_flags(self, account_id: int) -> Dict:
         """List feature flags for a specific account
 
         Args:
             account_id (int): Numeric ID of the account to retrieve
         """
         return self._simple_request(f'accounts/{account_id}/feature-flag/')
@@ -1695,14 +1763,31 @@
         """
         return self._simple_request(
             f'accounts/{account_id}/projects/{project_id}/environments/{environment_id}/',  # noqa: E501
             method='post',
             json=payload,
         )
 
+    @v3
+    def update_environment_variables(
+        self, account_id: int, project_id: int, payload: Dict
+    ):
+        """Update an environment variable
+
+        Args:
+            account_id (int): Numeric ID of the account
+            project_id (int): Numeric ID of the project
+            payload (dict): Dictionary representing the environment to update
+        """
+        return self._simple_request(
+            f'accounts/{account_id}/projects/{project_id}/environment-variables/bulk',  # noqa: E501
+            method='post',
+            json=payload,
+        )
+
     @v2
     def update_job(self, account_id: int, job_id: int, payload: Dict) -> Dict:
         """Update a job by its ID.
 
         Args:
             account_id (int): Numeric ID of the account to retrieve
             job_id (int): Numeric ID of the job to retrieve
```

### Comparing `dbtc-0.5.0/dbtc/client/artifacts/metadata_schema.json` & `dbtc-0.5.1/dbtc/client/artifacts/metadata_schema.json`

 * *Files identical despite different names*

### Comparing `dbtc-0.5.0/dbtc/client/base.py` & `dbtc-0.5.1/dbtc/client/base.py`

 * *Files identical despite different names*

### Comparing `dbtc-0.5.0/dbtc/client/metadata.py` & `dbtc-0.5.1/dbtc/client/metadata.py`

 * *Files identical despite different names*

### Comparing `dbtc-0.5.0/dbtc/client/schema.py` & `dbtc-0.5.1/dbtc/client/schema.py`

 * *Files identical despite different names*

### Comparing `dbtc-0.5.0/dbtc/models/webhooks.py` & `dbtc-0.5.1/dbtc/models/webhooks.py`

 * *Files identical despite different names*

### Comparing `dbtc-0.5.0/pyproject.toml` & `dbtc-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dbtc"
-version = "0.5.0"
+version = "0.5.1"
 description = "An unaffiliated python wrapper for dbt Cloud APIs"
 authors = ["Doug Guthrie <douglas.p.guthrie@gmail.com>"]
 documentation = "https://dbtc.dpguthrie.com"
 keywords=["dbt", "requests", "API", "dbt Cloud"]
 license = "MIT"
 readme = "README.md"
```

### Comparing `dbtc-0.5.0/PKG-INFO` & `dbtc-0.5.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbtc
-Version: 0.5.0
+Version: 0.5.1
 Summary: An unaffiliated python wrapper for dbt Cloud APIs
 License: MIT
 Keywords: dbt,requests,API,dbt Cloud
 Author: Doug Guthrie
 Author-email: douglas.p.guthrie@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -45,15 +45,15 @@
 
 **Interactive Demo**: <a target="_blank" href="https://dpguthrie-dbtc-streamlit-home-yy7c0b.streamlit.app/">https://dpguthrie-dbtc-streamlit-home-yy7c0b.streamlit.app/</a>
 
 **Source Code**: <a target="_blank" href="https://github.com/dpguthrie/dbtc">https://github.com/dpguthrie/dbtc</a>
 
 **V2 Docs**: <a target="_blank" href="https://docs.getdbt.com/dbt-cloud/api-v2">https://docs.getdbt.com/dbt-cloud/api-v2</a>
 
-**V3 Docs (Unofficial)**: <a target="_blank" href="https://documenter.getpostman.com/view/14183654/UVsSNiXC">https://documenter.getpostman.com/view/14183654/UVsSNiXC</a>
+**V3 Docs**: <a target="_blank" href="https://docs.getdbt.com/dbt-cloud/api-v3">https://docs.getdbt.com/dbt-cloud/api-v3</a>
 
 ---
 
 ## Overview
 
 dbtc is an unaffiliated python interface to various dbt Cloud API endpoints.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbtc Version: 0.5.0 Summary: An unaffiliated python
+Metadata-Version: 2.1 Name: dbtc Version: 0.5.1 Summary: An unaffiliated python
 wrapper for dbt Cloud APIs License: MIT Keywords: dbt,requests,API,dbt Cloud
 Author: Doug Guthrie Author-email: douglas.p.guthrie@gmail.com Requires-Python:
 >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Requires-Dist: pydantic (>=1.10.5,<2.0.0) Requires-Dist:
@@ -12,41 +12,41 @@
 Type: text/markdown
                          [docs/img/dbt-standalone.png]
               An unaffiliated python interface for dbt Cloud APIs
                    [Coverage] [Package_version] [Downloads]
 --- **Documentation**: https://dbtc.dpguthrie.com **Interactive Demo**: https:/
 /dpguthrie-dbtc-streamlit-home-yy7c0b.streamlit.app/ **Source Code**: https://
 github.com/dpguthrie/dbtc **V2 Docs**: https://docs.getdbt.com/dbt-cloud/api-v2
-**V3 Docs (Unofficial)**: https://documenter.getpostman.com/view/14183654/
-UVsSNiXC --- ## Overview dbtc is an unaffiliated python interface to various
-dbt Cloud API endpoints. This library acts as a convenient interface to two
-different APIs that dbt Cloud offers: - Cloud API: This is a REST API that
-exposes endpoints that allow users to programatically create, read, update, and
-delete resources within their dbt Cloud Account. - Metadata API: This is a
-GraphQL API that exposes metadata generated from a job run within dbt Cloud. ##
-Requirements Python 3.7+ - [Requests](https://requests.readthedocs.io/en/
-master/) - The elegant and simple HTTP library for Python, built for human
-beings. - [sgqlc](https://github.com/profusion/sgqlc) - Simple GraphQL Client -
-[Typer](https://github.com/tiangolo/typer) - Library for building CLI
-applications ## Installation ```bash pip install dbtc ``` ## Basic Usage ###
-Python The interface to both APIs are located in the `dbtCloudClient` class.
-The example below shows how you use the `cloud` property on an instance of the
-`dbtCloudClient` class to to access a method, `trigger_job_from_failure`, that
-allows you to restart a job from its last point of failure. ```python from dbtc
-import dbtCloudClient # Assumes that DBT_CLOUD_SERVICE_TOKEN env var is set
-client = dbtCloudClient() account_id = 1 job_id = 1 payload = {'cause':
-'Restarting from failure'} run = client.cloud.trigger_job_from_failure
-( account_id, job_id, payload, should_poll=False, ) # This returns a dictionary
-containing two keys run['data'] run['status'] ``` Similarly, use the `metadata`
-property to retrieve information about certain resources within your project -
-the example below shows how to retrieve metadata from models related to the
-most recent run for a given `job_id`. ```python from dbtc import dbtCloudClient
-client = dbtCloudClient() job_id = 1 models = client.metadata.get_models
-(job_id) # Models nested inside a couple keys models['data']['models'] # This
-is a list models['data']['models'][0] ``` ### CLI The CLI example below will
-map to the python cloud example above: ```bash dbtc trigger-job-from-failure \
---account-id 1 \ --job-id 1 \ --payload '{"cause": "Restarting from failure"}'
-\ --no-should-poll ``` Similarly, for the metadata example above: ```bash dbtc
-get-models --job-id 1 ``` If not setting your service token as an environment
+**V3 Docs**: https://docs.getdbt.com/dbt-cloud/api-v3 --- ## Overview dbtc is
+an unaffiliated python interface to various dbt Cloud API endpoints. This
+library acts as a convenient interface to two different APIs that dbt Cloud
+offers: - Cloud API: This is a REST API that exposes endpoints that allow users
+to programatically create, read, update, and delete resources within their dbt
+Cloud Account. - Metadata API: This is a GraphQL API that exposes metadata
+generated from a job run within dbt Cloud. ## Requirements Python 3.7+ -
+[Requests](https://requests.readthedocs.io/en/master/) - The elegant and simple
+HTTP library for Python, built for human beings. - [sgqlc](https://github.com/
+profusion/sgqlc) - Simple GraphQL Client - [Typer](https://github.com/tiangolo/
+typer) - Library for building CLI applications ## Installation ```bash pip
+install dbtc ``` ## Basic Usage ### Python The interface to both APIs are
+located in the `dbtCloudClient` class. The example below shows how you use the
+`cloud` property on an instance of the `dbtCloudClient` class to to access a
+method, `trigger_job_from_failure`, that allows you to restart a job from its
+last point of failure. ```python from dbtc import dbtCloudClient # Assumes that
+DBT_CLOUD_SERVICE_TOKEN env var is set client = dbtCloudClient() account_id = 1
+job_id = 1 payload = {'cause': 'Restarting from failure'} run =
+client.cloud.trigger_job_from_failure( account_id, job_id, payload,
+should_poll=False, ) # This returns a dictionary containing two keys run
+['data'] run['status'] ``` Similarly, use the `metadata` property to retrieve
+information about certain resources within your project - the example below
+shows how to retrieve metadata from models related to the most recent run for a
+given `job_id`. ```python from dbtc import dbtCloudClient client =
+dbtCloudClient() job_id = 1 models = client.metadata.get_models(job_id) #
+Models nested inside a couple keys models['data']['models'] # This is a list
+models['data']['models'][0] ``` ### CLI The CLI example below will map to the
+python cloud example above: ```bash dbtc trigger-job-from-failure \ --account-
+id 1 \ --job-id 1 \ --payload '{"cause": "Restarting from failure"}' \ --no-
+should-poll ``` Similarly, for the metadata example above: ```bash dbtc get-
+models --job-id 1 ``` If not setting your service token as an environment
 variable, do the following: ```bash dbtc --token this_is_my_token get_models --
 job-id 1 ``` ## License This project is licensed under the terms of the MIT
 license.
```

