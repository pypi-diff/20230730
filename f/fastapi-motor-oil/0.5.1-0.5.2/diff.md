# Comparing `tmp/fastapi_motor_oil-0.5.1.tar.gz` & `tmp/fastapi_motor_oil-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_motor_oil-0.5.1.tar", max compression
+gzip compressed data, was "fastapi_motor_oil-0.5.2.tar", max compression
```

## Comparing `fastapi_motor_oil-0.5.1.tar` & `fastapi_motor_oil-0.5.2.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0     1067 2023-02-22 21:38:05.147034 fastapi_motor_oil-0.5.1/LICENSE
--rw-r--r--   0        0        0     9954 2023-04-01 14:14:36.921182 fastapi_motor_oil-0.5.1/README.md
--rw-r--r--   0        0        0     1631 2023-06-04 12:59:37.309187 fastapi_motor_oil-0.5.1/fastapi_motor_oil/__init__.py
--rw-r--r--   0        0        0     3145 2023-06-04 12:09:52.899211 fastapi_motor_oil-0.5.1/fastapi_motor_oil/bound_method_wrapper.py
--rw-r--r--   0        0        0     2641 2023-06-04 12:09:20.394794 fastapi_motor_oil-0.5.1/fastapi_motor_oil/delete_rule.py
--rw-r--r--   0        0        0     2768 2023-06-04 12:12:44.073079 fastapi_motor_oil-0.5.1/fastapi_motor_oil/model.py
--rw-r--r--   0        0        0        0 2023-02-24 18:46:38.693945 fastapi_motor_oil-0.5.1/fastapi_motor_oil/py.typed
--rw-r--r--   0        0        0    26224 2023-06-04 12:34:04.571192 fastapi_motor_oil-0.5.1/fastapi_motor_oil/service.py
--rw-r--r--   0        0        0     5225 2023-06-04 12:18:18.159592 fastapi_motor_oil-0.5.1/fastapi_motor_oil/typing.py
--rw-r--r--   0        0        0     1636 2023-06-04 12:13:45.573637 fastapi_motor_oil-0.5.1/fastapi_motor_oil/validator.py
--rw-r--r--   0        0        0     2702 2023-06-04 12:41:38.300297 fastapi_motor_oil-0.5.1/pyproject.toml
--rw-r--r--   0        0        0    11047 1970-01-01 00:00:00.000000 fastapi_motor_oil-0.5.1/setup.py
--rw-r--r--   0        0        0    10516 1970-01-01 00:00:00.000000 fastapi_motor_oil-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-02-22 21:38:05.147034 fastapi_motor_oil-0.5.2/LICENSE
+-rw-r--r--   0        0        0    10178 2023-07-30 09:40:41.458126 fastapi_motor_oil-0.5.2/README.md
+-rw-r--r--   0        0        0     1847 2023-07-30 09:47:56.451525 fastapi_motor_oil-0.5.2/fastapi_motor_oil/__init__.py
+-rw-r--r--   0        0        0     3145 2023-06-04 12:09:52.899211 fastapi_motor_oil-0.5.2/fastapi_motor_oil/bound_method_wrapper.py
+-rw-r--r--   0        0        0     2641 2023-06-04 12:09:20.394794 fastapi_motor_oil-0.5.2/fastapi_motor_oil/delete_rule.py
+-rw-r--r--   0        0        0     2768 2023-06-04 12:12:44.073079 fastapi_motor_oil-0.5.2/fastapi_motor_oil/model.py
+-rw-r--r--   0        0        0        0 2023-02-24 18:46:38.693945 fastapi_motor_oil-0.5.2/fastapi_motor_oil/py.typed
+-rw-r--r--   0        0        0    26224 2023-06-04 12:34:04.571192 fastapi_motor_oil-0.5.2/fastapi_motor_oil/service.py
+-rw-r--r--   0        0        0     5225 2023-06-04 12:18:18.159592 fastapi_motor_oil-0.5.2/fastapi_motor_oil/typing.py
+-rw-r--r--   0        0        0     1636 2023-06-04 12:13:45.573637 fastapi_motor_oil-0.5.2/fastapi_motor_oil/validator.py
+-rw-r--r--   0        0        0     2702 2023-07-30 09:48:22.723609 fastapi_motor_oil-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0    10740 1970-01-01 00:00:00.000000 fastapi_motor_oil-0.5.2/PKG-INFO
```

### Comparing `fastapi_motor_oil-0.5.1/LICENSE` & `fastapi_motor_oil-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_motor_oil-0.5.1/README.md` & `fastapi_motor_oil-0.5.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # FastAPI-motor-oil
 
+**This project is deprecated and replaced by [motorhead](volfpeter.github.io/motorhead), adding Pydantic v2 support along with a couple of smaller improvements. Please create an issue if you need help with the migration.**
+
 `FastAPI-motor-oil` is a collection of async utilities for working with MongoDB and conveniently creating performant APIs with async web frameworks such a [FastAPI](https://fastapi.tiangolo.com/).
 
 Key features:
 
 - Database **model** design with `Pydantic`.
 - Relationship support and validation using async **validators and delete rules** with a declarative, decorator-based syntax.
 - Declarative **index** specification.
```

### Comparing `fastapi_motor_oil-0.5.1/fastapi_motor_oil/__init__.py` & `fastapi_motor_oil-0.5.2/fastapi_motor_oil/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from warnings import warn
+
 from .bound_method_wrapper import BoundMethodWrapper as BoundMethodWrapper
 from .delete_rule import DeleteConfig as DeleteConfig
 from .delete_rule import DeleteError as DeleteError
 from .delete_rule import delete_rule as delete_rule
 from .model import AgnosticClient as AgnosticClient
 from .model import AgnosticDatabase as AgnosticDatabase
 from .model import ClientProvider as ClientProvider
@@ -25,7 +27,13 @@
 from .typing import MongoQuery as MongoQuery
 from .typing import UpdateManyOptions as UpdateManyOptions
 from .typing import UpdateObject as UpdateObject
 from .typing import UpdateOneOptions as UpdateOneOptions
 from .validator import ValidationError as ValidationError
 from .validator import Validator as Validator
 from .validator import validator as validator
+
+warn(
+    "FastAPI-motor-oil is deprecated and replaced by motorhead with support for Pydantic v2. See https://volfpeter.github.io/motorhead/",
+    DeprecationWarning,
+    stacklevel=2,
+)
```

### Comparing `fastapi_motor_oil-0.5.1/fastapi_motor_oil/bound_method_wrapper.py` & `fastapi_motor_oil-0.5.2/fastapi_motor_oil/bound_method_wrapper.py`

 * *Files identical despite different names*

### Comparing `fastapi_motor_oil-0.5.1/fastapi_motor_oil/delete_rule.py` & `fastapi_motor_oil-0.5.2/fastapi_motor_oil/delete_rule.py`

 * *Files identical despite different names*

### Comparing `fastapi_motor_oil-0.5.1/fastapi_motor_oil/model.py` & `fastapi_motor_oil-0.5.2/fastapi_motor_oil/model.py`

 * *Files identical despite different names*

### Comparing `fastapi_motor_oil-0.5.1/fastapi_motor_oil/service.py` & `fastapi_motor_oil-0.5.2/fastapi_motor_oil/service.py`

 * *Files identical despite different names*

### Comparing `fastapi_motor_oil-0.5.1/fastapi_motor_oil/typing.py` & `fastapi_motor_oil-0.5.2/fastapi_motor_oil/typing.py`

 * *Files identical despite different names*

### Comparing `fastapi_motor_oil-0.5.1/fastapi_motor_oil/validator.py` & `fastapi_motor_oil-0.5.2/fastapi_motor_oil/validator.py`

 * *Files identical despite different names*

### Comparing `fastapi_motor_oil-0.5.1/pyproject.toml` & `fastapi_motor_oil-0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 [project.urls]
 Homepage = "https://github.com/volfpeter/fastapi-motor-oil"
 Documentation = "https://volfpeter.github.io/fastapi-motor-oil"
 
 [tool.poetry]
 name = "fastapi-motor-oil"
-version = "0.5.1"
+version = "0.5.2"
 description = "Collection of async utilities for working with MongoDB and conveniently creating performant APIs with async web frameworks such a FastAPI."
 authors = ["Peter Volf <do.volfp@gmail.com>"]
 readme = "README.md"
 packages = [{include = "fastapi_motor_oil"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `fastapi_motor_oil-0.5.1/setup.py` & `fastapi_motor_oil-0.5.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,341 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: fastapi-motor-oil
+Version: 0.5.2
+Summary: Collection of async utilities for working with MongoDB and conveniently creating performant APIs with async web frameworks such a FastAPI.
+Author: Peter Volf
+Author-email: do.volfp@gmail.com
+Requires-Python: >=3.10,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: motor (>=3.1.1,<4.0.0)
+Requires-Dist: pydantic (>=1.10.5,<2.0.0)
+Description-Content-Type: text/markdown
 
-packages = \
-['fastapi_motor_oil']
+# FastAPI-motor-oil
 
-package_data = \
-{'': ['*']}
+**This project is deprecated and replaced by [motorhead](volfpeter.github.io/motorhead), adding Pydantic v2 support along with a couple of smaller improvements. Please create an issue if you need help with the migration.**
 
-install_requires = \
-['motor>=3.1.1,<4.0.0', 'pydantic>=1.10.5,<2.0.0']
-
-setup_kwargs = {
-    'name': 'fastapi-motor-oil',
-    'version': '0.5.1',
-    'description': 'Collection of async utilities for working with MongoDB and conveniently creating performant APIs with async web frameworks such a FastAPI.',
-    'long_description': '# FastAPI-motor-oil\n\n`FastAPI-motor-oil` is a collection of async utilities for working with MongoDB and conveniently creating performant APIs with async web frameworks such a [FastAPI](https://fastapi.tiangolo.com/).\n\nKey features:\n\n- Database **model** design with `Pydantic`.\n- Relationship support and validation using async **validators and delete rules** with a declarative, decorator-based syntax.\n- Declarative **index** specification.\n- Typed **utilities** for convenient model and API creation.\n- Ready to use, customizable **async service layer** with **transaction support** that integrates all the above to keep your API and business logic clean, flexible, and easy to understand.\n\nBy providing a convenient, declarative middle layer between MongoDB and your API, `FastAPI-motor-oil` is halfway between an object document mapper (based on `Pydantic`) and a database driver (by wrapping the official, async `motor` driver).\n\nSee the [full documentation here](https://volfpeter.github.io/fastapi-motor-oil/).\n\n## Installation\n\nThe library is available on PyPI and can be installed with:\n\n```console\n$ pip install fastapi-motor-oil\n```\n\n## Example\n\nPrerequisites:\n\n- MongoDB (e.g. the Community Edition) installed and running locally;\n- `fastapi` with all its dependencies (`pip install fastapi[all]`);\n- This library (`pip install fastapi-motor-oil`).\n\nIn this example we will create:\n\n- a simple `TreeNode` document model with a `name` and an optional reference to a `parent` node and some delete rules;\n- the services that are necessary to create, read, update, and delete documents;\n- a `fastapi` `APIRouter` factory that can be included in `fastapi` applications;\n- and the `fastapi` application itself.\n\nThe project layout under your root directory will be as follows:\n\n- `/tree_app`\n  - `__init__.py`\n  - `api.py`\n  - `main.py`\n  - `model.py`\n  - `service.py`\n\nModel definitions (in `model.py`):\n\n```python\nfrom fastapi_motor_oil import DocumentModel, StrObjectId, UTCDatetime\nfrom pydantic import BaseModel\n\nclass TreeNode(DocumentModel):\n    """\n    Tree node document model.\n    """\n\n    name: str\n    parent: StrObjectId | None\n    created_at: UTCDatetime\n\nclass TreeNodeCreate(BaseModel):\n    """\n    Tree node creation model.\n    """\n\n    name: str\n    parent: StrObjectId | None\n\nclass TreeNodeUpdate(BaseModel):\n    """\n    Tree node update model.\n    """\n\n    name: str | None\n    parent: StrObjectId | None\n\n```\n\nService implementation (in `service.py`):\n\n```python\nfrom typing import Any\nfrom collections.abc import Sequence\nfrom datetime import datetime, timezone\n\nfrom bson import ObjectId\nfrom fastapi_motor_oil import (\n    CollectionOptions,\n    MongoQuery,\n    MongoService,\n    delete_rule,\n    validator,\n)\nfrom motor.core import AgnosticClientSession\n\nfrom .model import TreeNodeCreate, TreeNodeUpdate\n\nclass TreeNodeService(MongoService[TreeNodeCreate, TreeNodeUpdate]):\n    """\n    Tree node database services.\n    """\n\n    __slots__ = ()\n\n    collection_name: str = "tree_nodes"\n\n    collection_options: CollectionOptions | None = None\n\n    @delete_rule("pre")  # Delete rule that remove the subtrees of deleted nodes.\n    async def dr_delete_subtree(\n        self, session: AgnosticClientSession, ids: Sequence[ObjectId]\n    ) -> None:\n        child_ids = await self.find_ids({"parent": {"$in": ids}}, session=session)\n        if len(child_ids) > 0:\n            # Recursion\n            await self.delete_many(\n                {"_id": {"$in": child_ids}}, options={"session": session}\n            )\n\n    @delete_rule("deny")  # Delete rule that prevents the removal of root nodes.\n    async def dr_deny_if_root(\n        self, session: AgnosticClientSession, ids: Sequence[ObjectId]\n    ) -> None:\n        root_cnt = await self.count_documents(\n            {"$and": [{"_id": {"$in": ids}}, {"parent": None}]},\n            options={"session": session},\n        )\n        if root_cnt > 0:\n            raise ValueError("Can not delete root nodes.")\n\n    @validator("insert-update")\n    async def v_parent_valid(\n        self, query: MongoQuery | None, data: TreeNodeCreate | TreeNodeUpdate\n    ) -> None:\n        if data.parent is None:  # No parent node is always fine\n            return\n\n        if not await self.exists(data.parent):  # Parent must exist.\n            raise ValueError("Parent does not exist.")\n\n        if isinstance(data, TreeNodeCreate):  # No more checks during creation.\n            return\n\n        matched_ids = (\n            (await self.find_ids(query)) if isinstance(data, TreeNodeUpdate) else []\n        )\n        if data.parent in matched_ids:  # Self reference is forbidden.\n            raise ValueError("Self-reference.")\n\n    async def _convert_for_insert(self, data: TreeNodeCreate) -> dict[str, Any]:\n        return {\n            **(await super()._convert_for_insert(data)),\n            "created_at": datetime.now(timezone.utc),\n        }\n```\n\nRouting implementation (in `api.py`):\n\n```python\nfrom typing import Any\n\nfrom fastapi import APIRouter, Depends, HTTPException, status\nfrom fastapi_motor_oil import (\n    AgnosticDatabase,\n    DatabaseProvider,\n    DeleteError,\n    DeleteResultModel,\n    StrObjectId,\n)\n\nfrom .model import TreeNode, TreeNodeCreate, TreeNodeUpdate\nfrom .service import TreeNodeService\n\ndef make_api(\n    *,\n    get_database: DatabaseProvider,\n    prefix: str = "/tree-node",\n) -> APIRouter:\n    """\n    Tree node `APIRouter` factory.\n\n    Arguments:\n        get_database: FastAPI dependency that returns the `AgnosticDatabase`\n                      database instance for the API.\n        prefix: The prefix for the created `APIRouter`.\n\n    Returns:\n        The created `APIRouter` instance.\n    """\n    api = APIRouter(prefix=prefix)\n\n    @api.get("/", response_model=list[TreeNode])\n    async def get_all(\n        database: AgnosticDatabase = Depends(get_database),\n    ) -> list[dict[str, Any]]:\n        svc = TreeNodeService(database)\n        return [d async for d in svc.find()]\n\n    @api.post("/", response_model=TreeNode)\n    async def create(\n        data: TreeNodeCreate,\n        database: AgnosticDatabase = Depends(get_database),\n    ) -> dict[str, Any]:\n        svc = TreeNodeService(database)\n\n        try:\n            result = await svc.insert_one(data)\n        except Exception:\n            raise HTTPException(\n                status_code=status.HTTP_400_BAD_REQUEST, detail="Creation failed."\n            )\n\n        if (created := await svc.get_by_id(result.inserted_id)) is not None:\n            return created\n\n        raise HTTPException(status.HTTP_409_CONFLICT)\n\n    @api.get("/{id}", response_model=TreeNode)\n    async def get_by_id(\n        id: StrObjectId,\n        database: AgnosticDatabase = Depends(get_database),\n    ) -> dict[str, Any]:\n        svc = TreeNodeService(database)\n        if (result := await svc.get_by_id(id)) is not None:\n            return result\n\n        raise HTTPException(status_code=status.HTTP_404_NOT_FOUND, detail=str(id))\n\n    @api.put("/{id}", response_model=TreeNode)\n    async def update_by_id(\n        id: StrObjectId,\n        data: TreeNodeUpdate,\n        database: AgnosticDatabase = Depends(get_database),\n    ) -> dict[str, Any]:\n        svc = TreeNodeService(database)\n\n        try:\n            result = await svc.update_by_id(id, data)\n        except Exception:\n            raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST, detail=str(id))\n\n        if result.matched_count == 0:\n            raise HTTPException(status.HTTP_404_NOT_FOUND, detail=str(id))\n\n        if (updated := await svc.get_by_id(id)) is not None:\n            return updated\n\n        raise HTTPException(status.HTTP_404_NOT_FOUND, detail=str(id))\n\n    @api.delete("/{id}", response_model=DeleteResultModel)\n    async def delete_by_id(\n        id: StrObjectId,\n        database: AgnosticDatabase = Depends(get_database),\n    ) -> DeleteResultModel:\n        svc = TreeNodeService(database)\n        try:\n            result = await svc.delete_by_id(id)\n        except DeleteError:\n            raise HTTPException(status.HTTP_400_BAD_REQUEST, detail=str(id))\n        if result.deleted_count == 0:\n            raise HTTPException(status.HTTP_404_NOT_FOUND, detail=str(id))\n\n        return DeleteResultModel(delete_count=result.deleted_count)\n\n    return api\n```\n\nApplication (in `main.py`):\n\n```python\nfrom functools import lru_cache\n\nfrom fastapi import FastAPI\nfrom motor.motor_asyncio import AsyncIOMotorClient, AsyncIOMotorDatabase\n\n@lru_cache(maxsize=1)\ndef get_database() -> AsyncIOMotorDatabase:\n    """Database provider dependency for the created API."""\n    mongo_connection_string = "mongodb://127.0.0.1:27017"\n    database_name = "tree-db"\n    client = AsyncIOMotorClient(mongo_connection_string)\n    return client[database_name]\n\ndef register_routes(app: FastAPI) -> None:\n    """Registers all routes of the application."""\n    from .api import make_api as make_tree_node_api\n\n    api_prefix = "/api/v1"\n\n    app.include_router(\n        make_tree_node_api(get_database=get_database),\n        prefix=api_prefix,\n    )\n\ndef create_app() -> FastAPI:\n    app = FastAPI()\n\n    register_routes(app)\n\n    return app\n```\n\nWith everything in place, you can serve the application by executing `uvicorn tree_app.main:create_app --reload --factory` in your root directory. Go to [http://127.0.0.1:8000/docs](http://127.0.0.1:8000/docs) in the browser to see and try the created REST API.\n\n## Requirements\n\nThe project depends on `motor` (the official asyncio MongoDB driver, which is built on top of `pymongo` and `bson`) and `pydantic`.\n\n`fastapi` is not an actual dependency, but the code was written with `fastapi` applications with a REST API in mind.\n\n## Development\n\nUse `black` for code formatting and `mypy` for static code analysis.\n\n## Contributing\n\nContributions are welcome.\n\n## License - MIT\n\nThe library is open-sourced under the conditions of the [MIT license](https://choosealicense.com/licenses/mit/).\n',
-    'author': 'Peter Volf',
-    'author_email': 'do.volfp@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.10,<4.0',
-}
+`FastAPI-motor-oil` is a collection of async utilities for working with MongoDB and conveniently creating performant APIs with async web frameworks such a [FastAPI](https://fastapi.tiangolo.com/).
 
+Key features:
+
+- Database **model** design with `Pydantic`.
+- Relationship support and validation using async **validators and delete rules** with a declarative, decorator-based syntax.
+- Declarative **index** specification.
+- Typed **utilities** for convenient model and API creation.
+- Ready to use, customizable **async service layer** with **transaction support** that integrates all the above to keep your API and business logic clean, flexible, and easy to understand.
+
+By providing a convenient, declarative middle layer between MongoDB and your API, `FastAPI-motor-oil` is halfway between an object document mapper (based on `Pydantic`) and a database driver (by wrapping the official, async `motor` driver).
+
+See the [full documentation here](https://volfpeter.github.io/fastapi-motor-oil/).
+
+## Installation
+
+The library is available on PyPI and can be installed with:
+
+```console
+$ pip install fastapi-motor-oil
+```
+
+## Example
+
+Prerequisites:
+
+- MongoDB (e.g. the Community Edition) installed and running locally;
+- `fastapi` with all its dependencies (`pip install fastapi[all]`);
+- This library (`pip install fastapi-motor-oil`).
+
+In this example we will create:
+
+- a simple `TreeNode` document model with a `name` and an optional reference to a `parent` node and some delete rules;
+- the services that are necessary to create, read, update, and delete documents;
+- a `fastapi` `APIRouter` factory that can be included in `fastapi` applications;
+- and the `fastapi` application itself.
+
+The project layout under your root directory will be as follows:
+
+- `/tree_app`
+  - `__init__.py`
+  - `api.py`
+  - `main.py`
+  - `model.py`
+  - `service.py`
+
+Model definitions (in `model.py`):
+
+```python
+from fastapi_motor_oil import DocumentModel, StrObjectId, UTCDatetime
+from pydantic import BaseModel
+
+class TreeNode(DocumentModel):
+    """
+    Tree node document model.
+    """
+
+    name: str
+    parent: StrObjectId | None
+    created_at: UTCDatetime
+
+class TreeNodeCreate(BaseModel):
+    """
+    Tree node creation model.
+    """
+
+    name: str
+    parent: StrObjectId | None
+
+class TreeNodeUpdate(BaseModel):
+    """
+    Tree node update model.
+    """
+
+    name: str | None
+    parent: StrObjectId | None
+
+```
+
+Service implementation (in `service.py`):
+
+```python
+from typing import Any
+from collections.abc import Sequence
+from datetime import datetime, timezone
+
+from bson import ObjectId
+from fastapi_motor_oil import (
+    CollectionOptions,
+    MongoQuery,
+    MongoService,
+    delete_rule,
+    validator,
+)
+from motor.core import AgnosticClientSession
+
+from .model import TreeNodeCreate, TreeNodeUpdate
+
+class TreeNodeService(MongoService[TreeNodeCreate, TreeNodeUpdate]):
+    """
+    Tree node database services.
+    """
+
+    __slots__ = ()
+
+    collection_name: str = "tree_nodes"
+
+    collection_options: CollectionOptions | None = None
+
+    @delete_rule("pre")  # Delete rule that remove the subtrees of deleted nodes.
+    async def dr_delete_subtree(
+        self, session: AgnosticClientSession, ids: Sequence[ObjectId]
+    ) -> None:
+        child_ids = await self.find_ids({"parent": {"$in": ids}}, session=session)
+        if len(child_ids) > 0:
+            # Recursion
+            await self.delete_many(
+                {"_id": {"$in": child_ids}}, options={"session": session}
+            )
+
+    @delete_rule("deny")  # Delete rule that prevents the removal of root nodes.
+    async def dr_deny_if_root(
+        self, session: AgnosticClientSession, ids: Sequence[ObjectId]
+    ) -> None:
+        root_cnt = await self.count_documents(
+            {"$and": [{"_id": {"$in": ids}}, {"parent": None}]},
+            options={"session": session},
+        )
+        if root_cnt > 0:
+            raise ValueError("Can not delete root nodes.")
+
+    @validator("insert-update")
+    async def v_parent_valid(
+        self, query: MongoQuery | None, data: TreeNodeCreate | TreeNodeUpdate
+    ) -> None:
+        if data.parent is None:  # No parent node is always fine
+            return
+
+        if not await self.exists(data.parent):  # Parent must exist.
+            raise ValueError("Parent does not exist.")
+
+        if isinstance(data, TreeNodeCreate):  # No more checks during creation.
+            return
+
+        matched_ids = (
+            (await self.find_ids(query)) if isinstance(data, TreeNodeUpdate) else []
+        )
+        if data.parent in matched_ids:  # Self reference is forbidden.
+            raise ValueError("Self-reference.")
+
+    async def _convert_for_insert(self, data: TreeNodeCreate) -> dict[str, Any]:
+        return {
+            **(await super()._convert_for_insert(data)),
+            "created_at": datetime.now(timezone.utc),
+        }
+```
+
+Routing implementation (in `api.py`):
+
+```python
+from typing import Any
+
+from fastapi import APIRouter, Depends, HTTPException, status
+from fastapi_motor_oil import (
+    AgnosticDatabase,
+    DatabaseProvider,
+    DeleteError,
+    DeleteResultModel,
+    StrObjectId,
+)
+
+from .model import TreeNode, TreeNodeCreate, TreeNodeUpdate
+from .service import TreeNodeService
+
+def make_api(
+    *,
+    get_database: DatabaseProvider,
+    prefix: str = "/tree-node",
+) -> APIRouter:
+    """
+    Tree node `APIRouter` factory.
+
+    Arguments:
+        get_database: FastAPI dependency that returns the `AgnosticDatabase`
+                      database instance for the API.
+        prefix: The prefix for the created `APIRouter`.
+
+    Returns:
+        The created `APIRouter` instance.
+    """
+    api = APIRouter(prefix=prefix)
+
+    @api.get("/", response_model=list[TreeNode])
+    async def get_all(
+        database: AgnosticDatabase = Depends(get_database),
+    ) -> list[dict[str, Any]]:
+        svc = TreeNodeService(database)
+        return [d async for d in svc.find()]
+
+    @api.post("/", response_model=TreeNode)
+    async def create(
+        data: TreeNodeCreate,
+        database: AgnosticDatabase = Depends(get_database),
+    ) -> dict[str, Any]:
+        svc = TreeNodeService(database)
+
+        try:
+            result = await svc.insert_one(data)
+        except Exception:
+            raise HTTPException(
+                status_code=status.HTTP_400_BAD_REQUEST, detail="Creation failed."
+            )
+
+        if (created := await svc.get_by_id(result.inserted_id)) is not None:
+            return created
+
+        raise HTTPException(status.HTTP_409_CONFLICT)
+
+    @api.get("/{id}", response_model=TreeNode)
+    async def get_by_id(
+        id: StrObjectId,
+        database: AgnosticDatabase = Depends(get_database),
+    ) -> dict[str, Any]:
+        svc = TreeNodeService(database)
+        if (result := await svc.get_by_id(id)) is not None:
+            return result
+
+        raise HTTPException(status_code=status.HTTP_404_NOT_FOUND, detail=str(id))
+
+    @api.put("/{id}", response_model=TreeNode)
+    async def update_by_id(
+        id: StrObjectId,
+        data: TreeNodeUpdate,
+        database: AgnosticDatabase = Depends(get_database),
+    ) -> dict[str, Any]:
+        svc = TreeNodeService(database)
+
+        try:
+            result = await svc.update_by_id(id, data)
+        except Exception:
+            raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST, detail=str(id))
+
+        if result.matched_count == 0:
+            raise HTTPException(status.HTTP_404_NOT_FOUND, detail=str(id))
+
+        if (updated := await svc.get_by_id(id)) is not None:
+            return updated
+
+        raise HTTPException(status.HTTP_404_NOT_FOUND, detail=str(id))
+
+    @api.delete("/{id}", response_model=DeleteResultModel)
+    async def delete_by_id(
+        id: StrObjectId,
+        database: AgnosticDatabase = Depends(get_database),
+    ) -> DeleteResultModel:
+        svc = TreeNodeService(database)
+        try:
+            result = await svc.delete_by_id(id)
+        except DeleteError:
+            raise HTTPException(status.HTTP_400_BAD_REQUEST, detail=str(id))
+        if result.deleted_count == 0:
+            raise HTTPException(status.HTTP_404_NOT_FOUND, detail=str(id))
+
+        return DeleteResultModel(delete_count=result.deleted_count)
+
+    return api
+```
+
+Application (in `main.py`):
+
+```python
+from functools import lru_cache
+
+from fastapi import FastAPI
+from motor.motor_asyncio import AsyncIOMotorClient, AsyncIOMotorDatabase
+
+@lru_cache(maxsize=1)
+def get_database() -> AsyncIOMotorDatabase:
+    """Database provider dependency for the created API."""
+    mongo_connection_string = "mongodb://127.0.0.1:27017"
+    database_name = "tree-db"
+    client = AsyncIOMotorClient(mongo_connection_string)
+    return client[database_name]
+
+def register_routes(app: FastAPI) -> None:
+    """Registers all routes of the application."""
+    from .api import make_api as make_tree_node_api
+
+    api_prefix = "/api/v1"
+
+    app.include_router(
+        make_tree_node_api(get_database=get_database),
+        prefix=api_prefix,
+    )
+
+def create_app() -> FastAPI:
+    app = FastAPI()
+
+    register_routes(app)
+
+    return app
+```
+
+With everything in place, you can serve the application by executing `uvicorn tree_app.main:create_app --reload --factory` in your root directory. Go to [http://127.0.0.1:8000/docs](http://127.0.0.1:8000/docs) in the browser to see and try the created REST API.
+
+## Requirements
+
+The project depends on `motor` (the official asyncio MongoDB driver, which is built on top of `pymongo` and `bson`) and `pydantic`.
+
+`fastapi` is not an actual dependency, but the code was written with `fastapi` applications with a REST API in mind.
+
+## Development
+
+Use `black` for code formatting and `mypy` for static code analysis.
+
+## Contributing
+
+Contributions are welcome.
+
+## License - MIT
+
+The library is open-sourced under the conditions of the [MIT license](https://choosealicense.com/licenses/mit/).
 
-setup(**setup_kwargs)
```

