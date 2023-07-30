# Comparing `tmp/bridgeapi-1.0.0b2.tar.gz` & `tmp/bridgeapi-1.1.0.tar.gz`

## Comparing `bridgeapi-1.0.0b2.tar` & `bridgeapi-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,52 @@
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 bridgeapi-1.0.0b2/.envrc
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 bridgeapi-1.0.0b2/.vscode/settings.json
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 bridgeapi-1.0.0b2/src/bridgeapi/__about__.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 bridgeapi-1.0.0b2/src/bridgeapi/__init__.py
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 bridgeapi-1.0.0b2/src/bridgeapi/base_client.py
--rw-r--r--   0        0        0    16307 2020-02-02 00:00:00.000000 bridgeapi-1.0.0b2/src/bridgeapi/client.py
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 bridgeapi-1.0.0b2/src/bridgeapi/exceptions.py
--rw-r--r--   0        0        0     8305 2020-02-02 00:00:00.000000 bridgeapi-1.0.0b2/src/bridgeapi/models.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 bridgeapi-1.0.0b2/tests/__init__.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 bridgeapi-1.0.0b2/tests/conftest.py
--rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 bridgeapi-1.0.0b2/tests/test_base_client.py
--rw-r--r--   0        0        0     6310 2020-02-02 00:00:00.000000 bridgeapi-1.0.0b2/tests/test_client.py
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 bridgeapi-1.0.0b2/tests/test_paginated_result.py
--rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 bridgeapi-1.0.0b2/tests/test_user_client_auth.py
--rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 bridgeapi-1.0.0b2/tests/cassettes/test_client/test_user_client[list_items].yaml
--rw-r--r--   0        0        0     3158 2020-02-02 00:00:00.000000 bridgeapi-1.0.0b2/.gitignore
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 bridgeapi-1.0.0b2/LICENSE.txt
--rw-r--r--   0        0        0     4852 2020-02-02 00:00:00.000000 bridgeapi-1.0.0b2/README.md
--rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 bridgeapi-1.0.0b2/pyproject.toml
--rw-r--r--   0        0        0     5711 2020-02-02 00:00:00.000000 bridgeapi-1.0.0b2/PKG-INFO
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 bridgeapi-1.1.0/.envrc
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 bridgeapi-1.1.0/.vscode/settings.json
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 bridgeapi-1.1.0/src/bridgeapi/__about__.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 bridgeapi-1.1.0/src/bridgeapi/__init__.py
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 bridgeapi-1.1.0/src/bridgeapi/base_client.py
+-rw-r--r--   0        0        0    16085 2020-02-02 00:00:00.000000 bridgeapi-1.1.0/src/bridgeapi/client.py
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 bridgeapi-1.1.0/src/bridgeapi/exceptions.py
+-rw-r--r--   0        0        0     8766 2020-02-02 00:00:00.000000 bridgeapi-1.1.0/src/bridgeapi/models.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 bridgeapi-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 bridgeapi-1.1.0/tests/conftest.py
+-rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 bridgeapi-1.1.0/tests/test_base_client.py
+-rw-r--r--   0        0        0     7440 2020-02-02 00:00:00.000000 bridgeapi-1.1.0/tests/test_client.py
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 bridgeapi-1.1.0/tests/test_paginated_result.py
+-rw-r--r--   0        0        0     3693 2020-02-02 00:00:00.000000 bridgeapi-1.1.0/tests/test_user_client_auth.py
+-rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 bridgeapi-1.1.0/tests/cassettes/test_client/test_app_client[get_bank].yaml
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 bridgeapi-1.1.0/tests/cassettes/test_client/test_app_client[get_category].yaml
+-rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 bridgeapi-1.1.0/tests/cassettes/test_client/test_app_client[get_user].yaml
+-rw-r--r--   0        0        0    40090 2020-02-02 00:00:00.000000 bridgeapi-1.1.0/tests/cassettes/test_client/test_app_client[list_banks].yaml
+-rw-r--r--   0        0        0     2642 2020-02-02 00:00:00.000000 bridgeapi-1.1.0/tests/cassettes/test_client/test_app_client[list_banks_limit].yaml
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 bridgeapi-1.1.0/tests/cassettes/test_client/test_app_client[list_banks_multi_capability].yaml
+-rw-r--r--   0        0        0    41162 2020-02-02 00:00:00.000000 bridgeapi-1.1.0/tests/cassettes/test_client/test_app_client[list_banks_multi_country].yaml
+-rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 bridgeapi-1.1.0/tests/cassettes/test_client/test_app_client[list_banks_one_capability].yaml
+-rw-r--r--   0        0        0    42261 2020-02-02 00:00:00.000000 bridgeapi-1.1.0/tests/cassettes/test_client/test_app_client[list_banks_one_country].yaml
+-rw-r--r--   0        0        0     6531 2020-02-02 00:00:00.000000 bridgeapi-1.1.0/tests/cassettes/test_client/test_app_client[list_categories].yaml
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 bridgeapi-1.1.0/tests/cassettes/test_client/test_app_client[list_users].yaml
+-rw-r--r--   0        0        0    52396 2020-02-02 00:00:00.000000 bridgeapi-1.1.0/tests/cassettes/test_client/test_app_client_get_bank_connectors_status.yaml
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 bridgeapi-1.1.0/tests/cassettes/test_client/test_user_client[connect_item].yaml
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 bridgeapi-1.1.0/tests/cassettes/test_client/test_user_client[edit_item].yaml
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 bridgeapi-1.1.0/tests/cassettes/test_client/test_user_client[get_account].yaml
+-rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 bridgeapi-1.1.0/tests/cassettes/test_client/test_user_client[get_email_validation].yaml
+-rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 bridgeapi-1.1.0/tests/cassettes/test_client/test_user_client[get_item].yaml
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 bridgeapi-1.1.0/tests/cassettes/test_client/test_user_client[get_item_refresh_status].yaml
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 bridgeapi-1.1.0/tests/cassettes/test_client/test_user_client[get_stock].yaml
+-rw-r--r--   0        0        0    17195 2020-02-02 00:00:00.000000 bridgeapi-1.1.0/tests/cassettes/test_client/test_user_client[list_account_transactions].yaml
+-rw-r--r--   0        0        0    17263 2020-02-02 00:00:00.000000 bridgeapi-1.1.0/tests/cassettes/test_client/test_user_client[list_account_updated_transactions].yaml
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 bridgeapi-1.1.0/tests/cassettes/test_client/test_user_client[list_accounts].yaml
+-rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 bridgeapi-1.1.0/tests/cassettes/test_client/test_user_client[list_items].yaml
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 bridgeapi-1.1.0/tests/cassettes/test_client/test_user_client[list_stocks].yaml
+-rw-r--r--   0        0        0    17147 2020-02-02 00:00:00.000000 bridgeapi-1.1.0/tests/cassettes/test_client/test_user_client[list_transactions].yaml
+-rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 bridgeapi-1.1.0/tests/cassettes/test_client/test_user_client[list_updated_stocks].yaml
+-rw-r--r--   0        0        0    19159 2020-02-02 00:00:00.000000 bridgeapi-1.1.0/tests/cassettes/test_client/test_user_client[list_updated_transactions].yaml
+-rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 bridgeapi-1.1.0/tests/cassettes/test_client/test_user_client[manage_accounts_iban].yaml
+-rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 bridgeapi-1.1.0/tests/cassettes/test_client/test_user_client[manage_sca_sync_item].yaml
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 bridgeapi-1.1.0/tests/cassettes/test_client/test_user_client[refresh_item].yaml
+-rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 bridgeapi-1.1.0/tests/cassettes/test_client/test_user_client[validate_pro_items].yaml
+-rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 bridgeapi-1.1.0/tests/cassettes/test_client/test_user_life_cycle.yaml
+-rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 bridgeapi-1.1.0/tests/cassettes/test_client/user_auth.yaml
+-rw-r--r--   0        0        0     3158 2020-02-02 00:00:00.000000 bridgeapi-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 bridgeapi-1.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     4852 2020-02-02 00:00:00.000000 bridgeapi-1.1.0/README.md
+-rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 bridgeapi-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5707 2020-02-02 00:00:00.000000 bridgeapi-1.1.0/PKG-INFO
```

### Comparing `bridgeapi-1.0.0b2/src/bridgeapi/base_client.py` & `bridgeapi-1.1.0/src/bridgeapi/base_client.py`

 * *Files identical despite different names*

### Comparing `bridgeapi-1.0.0b2/src/bridgeapi/client.py` & `bridgeapi-1.1.0/src/bridgeapi/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 """Clients for the Bridge API (https://bridgeapi.io).
 """
 
-# TODO (20230719):
-# * Handle return code of endpoints (200, 202, 204)
-# * Check presence of language header
-# * Add doc and links to Bridge API doc
-# * Sections left to implement:
+# TODO (20230719): Sections left to implement:
 #   * Payment links: app-scoped
 #   * Payment initiation: app-scoped
 #   * Bridge transfer: user-scoped, requires sales team activation
 #   * Insights: user-scoped, requires sales team activation
 #   * Account check: user-scoped
 #   * Subscriptions: user-scoped, requires sales team activation
 
@@ -62,15 +58,15 @@
         response = self._request("GET", "banks", params)
         return PaginatedResult[Bank].from_response(response, self)
 
     def get_bank(self, bank_id: int) -> Bank:
         response = self._request("GET", f"banks/{bank_id}")
         return Bank.from_response(response)
 
-    def get_bank_connectors_status(self):
+    def get_bank_connectors_status(self) -> list[dict]:
         # TODO (20230719): Deserialization models
         response = self._request("GET", "banks/insights")
         return response.json()
 
     # Users endpoints
     def list_users(
         self, after: str | None = None, limit: int | None = None
@@ -263,31 +259,23 @@
         }
         response = self._user_request("POST", "connect/items/add", json=json_data)
         return BridgeConnectUrl.from_response(response)
 
     def edit_item(
         self, item_id: int, redirect_url: str | None = None, context: str | None = None
     ) -> BridgeConnectUrl:
-        json_data = {
-            "item_id": item_id,
-            "redirect_url": redirect_url,
-            "context": context,
-        }
-        response = self._user_request("GET", "connect/items/edit", json=json_data)
+        params = {"item_id": item_id, "redirect_url": redirect_url, "context": context}
+        response = self._user_request("GET", "connect/items/edit", params=params)
         return BridgeConnectUrl.from_response(response)
 
     def manage_sca_sync_item(
         self, item_id: int, redirect_url: str | None = None, context: str | None = None
     ) -> BridgeConnectUrl:
-        json_data = {
-            "item_id": item_id,
-            "redirect_url": redirect_url,
-            "context": context,
-        }
-        response = self._user_request("GET", "connect/items/sync", json=json_data)
+        params = {"item_id": item_id, "redirect_url": redirect_url, "context": context}
+        response = self._user_request("GET", "connect/items/sync", params=params)
         return BridgeConnectUrl.from_response(response)
 
     def validate_pro_items(
         self, redirect_url: str | None = None, context: str | None = None
     ) -> BridgeConnectUrl:
         json_data = {"redirect_url": redirect_url, "context": context}
         response = self._user_request("GET", "connect/items/pro/confirmation", json=json_data)
```

### Comparing `bridgeapi-1.0.0b2/src/bridgeapi/exceptions.py` & `bridgeapi-1.1.0/src/bridgeapi/exceptions.py`

 * *Files 18% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     def __init__(self, response, status_code: int, response_data: ErrorResponseData):
         self.response = response
         self.status_code = status_code
         self.response_data = response_data
 
     @classmethod
     def from_response(cls, response: requests.Response) -> "RequestError":
-        response_data = ErrorResponseData.parse_obj(response.json())
+        response_data = ErrorResponseData.model_validate(response.json())
         return cls(response, response.status_code, response_data)
 
     def __str__(self) -> str:
         msg = (
             f"HTTP error {self.status_code} ({self.response_data.type}) upon request to URL "
             f"{self.response.url}"
         )
```

### Comparing `bridgeapi-1.0.0b2/src/bridgeapi/models.py` & `bridgeapi-1.1.0/src/bridgeapi/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # ruff: noqa: A002, A003  # Attribute names shadowing Python builtin
 import datetime as dt
+import os
 from decimal import Decimal
 from enum import Enum
-from typing import Generic, Literal, TypeVar
+from typing import Any, Generic, Literal, TypeVar
 from uuid import UUID
 
 import requests
-from pydantic import BaseModel, HttpUrl, PrivateAttr, constr
-from pydantic.generics import GenericModel
+from pydantic import BaseModel, HttpUrl, PrivateAttr, constr, model_serializer
 
 from bridgeapi.base_client import BaseClient
 from bridgeapi.exceptions import PaginationError
 
 ModelT = TypeVar("ModelT", bound="BaseResponseModel")
 
 
@@ -23,45 +23,56 @@
     container, and the property will be None in the children.
     """
 
     _response: requests.Response | None = PrivateAttr(None)
 
     @classmethod
     def from_response(cls: type[ModelT], response: requests.Response) -> ModelT:
-        value = cls.parse_obj(response.json())
+        value = cls.model_validate(response.json())
         value._response = response
         return value
 
     @property
     def response(self) -> requests.Response | None:
         return self._response
 
+    if os.environ.get("BRIDGEAPI_MODEL_SERIALIZATION_HOOK") == "1":
+
+        @model_serializer(mode="wrap")
+        def _serialize(self, default_ser) -> dict[str, Any]:
+            """Hook to turn on custom serialization. Needs redefinition of `.serialize()`.
+
+            Activation of the hook is controlled by the `BRIDGEAPI_MODEL_SERIALIZATION_HOOK`
+            environment variable. No performance impact if disabled. Used for tests.
+            """
+            return self.serialize(default_ser)
+
 
 _T = TypeVar("_T")
 
 
 class Pagination(BaseModel):
     next_uri: str | None = None
 
 
-class PaginatedResult(BaseResponseModel, GenericModel, Generic[_T]):
+class PaginatedResult(BaseResponseModel, Generic[_T]):
     """Container storing results of a paginated API call."""
 
     resources: list[_T]
     pagination: Pagination
-    generated_at: dt.datetime | None  # Only exposed by list_categories
+    generated_at: dt.datetime | None = None
 
     _client: "BaseClient" = PrivateAttr()
     _page_number: int = PrivateAttr()
 
     @classmethod
     def from_response(
         cls, response: requests.Response, client: "BaseClient", page_number: int = 0
     ) -> "PaginatedResult[_T]":
-        result = cls.parse_obj(response.json())
+        result = cls.model_validate(response.json())
         result._response = response
         result._client = client
         result._page_number = page_number
         return result
 
     def has_more(self) -> bool:
         return self.pagination.next_uri is not None
```

### Comparing `bridgeapi-1.0.0b2/tests/test_base_client.py` & `bridgeapi-1.1.0/tests/test_base_client.py`

 * *Files identical despite different names*

### Comparing `bridgeapi-1.0.0b2/tests/test_client.py` & `bridgeapi-1.1.0/tests/test_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,64 +1,65 @@
 import datetime as dt
-import json
 import os
 from collections.abc import Callable
 from dataclasses import dataclass, field
-from typing import get_type_hints
-from unittest.mock import _Call, call
+from typing import Any, get_type_hints
+from unittest.mock import _Call, call, patch
 
 import pytest
-from pydantic.json import pydantic_encoder
-from pytest_mock import MockerFixture
+import vcr
+from pydantic_core import Url
 
 from bridgeapi.base_client import BaseClient
 from bridgeapi.client import AppClient, UserClient
-from bridgeapi.models import Bank, BankCapability, BaseResponseModel, PaginatedResult, UserAuthInfo
+from bridgeapi.models import BankCapability, BaseResponseModel
 
 DEMO_BANK_ID = 574
 USER_UUID = "998945b4-c977-43e4-a854-d9680fa00fd5"
 ITEM_ID = 8170358
+ACCOUNT_ID = 37271913
 
 
 @pytest.fixture
-def app_client():
-    return AppClient(os.environ.get("BRIDGEAPI_CLIENT_ID"), os.environ.get("BRIDGEAPI_SECRET_ID"))
+def app_auth() -> dict[str, str | None]:
+    return {
+        "client_id": os.environ.get("BRIDGEAPI_CLIENT_ID"),
+        "client_secret": os.environ.get("BRIDGEAPI_SECRET_ID"),
+    }
 
 
 @pytest.fixture
-@pytest.mark.default_cassette("user_auth.yaml")
-@pytest.mark.vcr
-def user_auth():
+def app_client(app_auth: dict):
+    return AppClient(**app_auth)
+
+
+@pytest.fixture
+def user_auth(app_auth: dict):
     email = "john@doe.com"
     password = "password123"
     client = UserClient(
-        os.environ.get("BRIDGEAPI_CLIENT_ID"),
-        os.environ.get("BRIDGEAPI_SECRET_ID"),
-        email,
-        password,
+        **app_auth,
+        user_email=email,
+        user_password=password,
         auto_renew=False,
     )
-    client.renew_auth()
+    with vcr.use_cassette("tests/cassettes/test_client/user_auth.yaml"):
+        client.renew_auth()
     return {
         "user_email": email,
         "user_password": password,
         "user_uuid": client.user_uuid,
         "access_token": client.access_token,
         "expires_at": dt.datetime(3000, 1, 1, tzinfo=dt.timezone.utc),
     }
 
 
 @pytest.fixture
-def user_client(user_auth):
-    return UserClient(
-        os.environ.get("BRIDGEAPI_CLIENT_ID"),
-        os.environ.get("BRIDGEAPI_SECRET_ID"),
-        **user_auth,
-        auto_renew=False,
-    )
+def user_client(app_auth: dict, user_auth: dict):
+    return UserClient(**app_auth, **user_auth, auto_renew=False)
 
 
 @dataclass
 class CaseParameters:
     method: Callable[..., BaseResponseModel]
     call_args: _Call = field(default_factory=call)
     extra_id: str | None = None
@@ -81,93 +82,123 @@
     CaseParameters(
         AppClient.list_banks,
         call(capabilities=[BankCapability.BULK_PAYMENT, BankCapability.BULK_TRANSFER]),
         "multi_capability",
     ),
     CaseParameters(AppClient.list_banks, call(limit=2), "limit"),
     CaseParameters(AppClient.get_bank, call(bank_id=DEMO_BANK_ID)),
-    # CaseParameters(AppClient.get_bank_connectors_status),
+    # CaseParameters(AppClient.get_bank_connectors_status),  # Standalone test
     CaseParameters(AppClient.list_users),
-    # CaseParameters(AppClient.get_user, call(user_uuid=USER_UUID)),
-    # CaseParameters(AppClient.create_user),
-    # CaseParameters(AppClient.delete_user),
+    CaseParameters(AppClient.get_user, call(user_uuid=USER_UUID)),
+    # CaseParameters(AppClient.create_user),  # User life cycle test
+    # CaseParameters(AppClient.delete_user),  # User life cycle test
     # CaseParameters(AppClient.delete_all_users),
-    # CaseParameters(AppClient.authenticate_user),
-    # CaseParameters(AppClient.update_user_email),
-    # CaseParameters(AppClient.update_user_password),
+    # CaseParameters(AppClient.authenticate_user),  # Happens in user_auth fixture
+    # CaseParameters(AppClient.update_user_email),  # User life cycle test
+    # CaseParameters(AppClient.update_user_password),  # User life cycle test
     CaseParameters(AppClient.list_categories),
     CaseParameters(AppClient.get_category, call(category_id=1)),
 ]
 app_client_param_ids = [p.case_id for p in app_client_params]
 
 
 user_client_params = [
     CaseParameters(UserClient.get_email_validation),
     CaseParameters(UserClient.connect_item, call(prefill_email="john@doe.com")),
-    # CaseParameters(UserClient.edit_item, call(item_id=ITEM_ID, redirect_url="https://test.com")),
-    # CaseParameters(UserClient.manage_sca_sync_item, call(item_id=ITEM_ID)),
+    CaseParameters(UserClient.edit_item, call(item_id=ITEM_ID, redirect_url="https://test.com")),
+    CaseParameters(UserClient.manage_sca_sync_item, call(item_id=ITEM_ID)),
     CaseParameters(UserClient.validate_pro_items),
     CaseParameters(UserClient.manage_accounts_iban),
     CaseParameters(UserClient.list_items),
     CaseParameters(UserClient.get_item, call(item_id=ITEM_ID)),
     CaseParameters(UserClient.refresh_item, call(item_id=ITEM_ID)),
     CaseParameters(UserClient.get_item_refresh_status, call(item_id=ITEM_ID)),
     # CaseParameters(UserClient.delete_item, call(item_id=1)),
-    # CaseParameters(UserClient.list_accounts),
-    # CaseParameters(UserClient.get_account, call(item_id=1)),
-    # CaseParameters(UserClient.list_transactions),
-    # CaseParameters(UserClient.list_updated_transactions),
-    # CaseParameters(UserClient.list_account_transactions, call(account_id=1)),
-    # CaseParameters(UserClient.list_account_updated_transactions, call(account_id=1)),
-    # CaseParameters(UserClient.list_stocks),
-    # CaseParameters(UserClient.list_updated_stocks),
+    CaseParameters(UserClient.list_accounts),
+    CaseParameters(UserClient.get_account, call(account_id=ACCOUNT_ID)),
+    CaseParameters(UserClient.list_transactions),
+    CaseParameters(UserClient.list_updated_transactions),
+    CaseParameters(UserClient.list_account_transactions, call(account_id=ACCOUNT_ID)),
+    CaseParameters(UserClient.list_account_updated_transactions, call(account_id=ACCOUNT_ID)),
+    CaseParameters(UserClient.list_stocks),
+    CaseParameters(UserClient.list_updated_stocks),
     # CaseParameters(UserClient.get_stock, call(stock_id=1)),
 ]
 user_client_param_ids = [p.case_id for p in user_client_params]
 
 
-@pytest.mark.vcr
-def _test_app_client(app_client: AppClient):
-    result = app_client.list_banks(countries="fr")
-    assert isinstance(result, PaginatedResult[Bank])
-    assert all(isinstance(b, Bank) for b in result.resources)
-    assert result._client is app_client
-    assert result._page_number == 0
-    assert result.response.request.method == "GET"
-    assert result.response.request.path_url == "/v2/banks?countries=fr"
-    assert result.response.json() == json.loads(result.json(exclude_unset=True))
-
-
-def json_encoder(obj):
-    if isinstance(obj, dt.datetime):
-        s = obj.astimezone(dt.timezone.utc).isoformat(sep="T", timespec="milliseconds")
-        return s.split("+")[0] + "Z"
-    return pydantic_encoder(obj)
+def serialize_datetime(val: dt.datetime) -> str:
+    s = val.astimezone(dt.timezone.utc).isoformat(sep="T", timespec="milliseconds")
+    return s.split("+")[0] + "Z"
+
+
+def serialize_model(model: BaseResponseModel, default_ser: Callable) -> dict[str, Any]:
+    serialized = default_ser(model)
+    for field_name, field_value in model:
+        if isinstance(field_value, dt.datetime):
+            serialized[field_name] = serialize_datetime(field_value)
+        if isinstance(field_value, Url) and field_value.path == "/":
+            serialized[field_name] = str(field_value).replace("/?", "?")
+    return serialized
+
+
+def assert_json_eq(result: BaseResponseModel) -> None:
+    response_json = result.response.json(parse_float=str)
+    with patch.object(BaseResponseModel, "serialize", serialize_model, create=True):
+        result_json = result.model_dump(mode="json", exclude_unset=True)
+    assert response_json == result_json
 
 
 def check_client_api_method(
     client: BaseClient, method: Callable[..., BaseResponseModel], call_args: _Call
 ):
     result = method(client, *call_args.args, **call_args.kwargs)
 
     return_type = get_type_hints(method)["return"]
     if return_type is type(None):
         assert result is None
         return
 
     assert isinstance(result, return_type)
-
-    response_json = result.response.json()
-    result_json = json.loads(result.json(exclude_unset=True, encoder=json_encoder))
-    assert response_json == result_json
+    assert_json_eq(result)
 
 
 @pytest.mark.vcr
 @pytest.mark.parametrize("params", app_client_params, ids=app_client_param_ids)
 def test_app_client(app_client: AppClient, params: CaseParameters):
     check_client_api_method(app_client, params.method, params.call_args)
 
 
 @pytest.mark.vcr
 @pytest.mark.parametrize("params", user_client_params, ids=user_client_param_ids)
 def test_user_client(user_client: UserClient, params: CaseParameters):
     check_client_api_method(user_client, params.method, params.call_args)
+
+
+@pytest.mark.vcr
+def test_app_client_get_bank_connectors_status(app_client: AppClient):
+    result = app_client.get_bank_connectors_status()
+    assert isinstance(result, list)
+
+
+@pytest.mark.vcr
+def test_user_life_cycle(app_client: AppClient):
+    email = "foo@email.com"
+    email2 = "bar@email.com"
+    password = "password123"
+    password2 = "yolo"
+
+    user = app_client.create_user(email, password)
+    try:
+        assert_json_eq(user)
+        assert user.email == email
+
+        # 404 errors with update_user_email and update_user_password
+        # user = app_client.update_user_email(user.uuid, password, email2)
+        # assert_json_eq(user)
+        # assert user.email == email2
+
+        # user = app_client.update_user_password(user.uuid, password, password2)
+        # assert_json_eq(user)
+        # assert user.email == email2
+    finally:
+        assert app_client.delete_user(user.uuid, password) is None
```

### Comparing `bridgeapi-1.0.0b2/tests/test_paginated_result.py` & `bridgeapi-1.1.0/tests/test_paginated_result.py`

 * *Files identical despite different names*

### Comparing `bridgeapi-1.0.0b2/tests/test_user_client_auth.py` & `bridgeapi-1.1.0/tests/test_user_client_auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
 
 def test_renew_auth(mocker: MockerFixture, fixed_now, base_args):
     expires_at = fixed_now + dt.timedelta(hours=2)
     auth_info = UserAuthInfo(
         access_token="TOKEN",
         expires_at=expires_at,
-        user=User.construct(uuid="UUID", email="john@doe.com"),
+        user=User.model_construct(uuid="UUID", email="john@doe.com"),
     )
     m_auth = mocker.Mock(return_value=auth_info)
     mocker.patch(
         "bridgeapi.client.AppClient",
         mocker.Mock(return_value=mocker.Mock(authenticate_user=m_auth)),
     )
```

### Comparing `bridgeapi-1.0.0b2/tests/cassettes/test_client/test_user_client[list_items].yaml` & `bridgeapi-1.1.0/tests/cassettes/test_client/test_user_client[list_items].yaml`

 * *Files 13% similar despite different names*

```diff
@@ -1,70 +1,9 @@
 interactions:
 - request:
-    body: '{"email": "john@doe.com", "password": "password123"}'
-    headers:
-      Accept:
-      - '*/*'
-      Accept-Encoding:
-      - gzip, deflate
-      Bridge-Version:
-      - '2021-06-01'
-      Connection:
-      - keep-alive
-      Content-Length:
-      - '52'
-      Content-Type:
-      - application/json
-      User-Agent:
-      - python-requests/2.31.0
-    method: POST
-    uri: https://api.bridgeapi.io/v2/authenticate
-  response:
-    body:
-      string: '{"access_token":"efcb95c1a53f738330389ea32e3858c82efe1abb-ccfd8af0-af98-4c45-b954-8ce6f2354d40","expires_at":"2023-07-26T09:57:55.747Z","user":{"uuid":"998945b4-c977-43e4-a854-d9680fa00fd5","email":"john@doe.com"}}'
-    headers:
-      Cache-Control:
-      - no-cache, no-store, max-age=0, must-revalidate
-      Connection:
-      - keep-alive
-      Content-Length:
-      - '214'
-      Content-Security-Policy:
-      - default-src 'self';
-      Content-Type:
-      - application/json
-      Date:
-      - Wed, 26 Jul 2023 07:57:55 GMT
-      Expires:
-      - '0'
-      Pragma:
-      - no-cache
-      Referrer-Policy:
-      - strict-origin-when-cross-origin
-      Server:
-      - Bridge
-      Strict-Transport-Security:
-      - max-age=31536000; includeSubDomains; preload;
-      Vary:
-      - Origin
-      - Access-Control-Request-Method
-      - Access-Control-Request-Headers
-      - Origin
-      X-Robots-Tag:
-      - noindex
-      x-content-type-options:
-      - nosniff
-      x-frame-options:
-      - DENY
-      x-xss-protection:
-      - 1; mode=block
-    status:
-      code: 200
-      message: OK
-- request:
     body: null
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Bridge-Version:
@@ -88,15 +27,15 @@
       Content-Length:
       - '141'
       Content-Security-Policy:
       - default-src 'self';
       Content-Type:
       - application/json
       Date:
-      - Wed, 26 Jul 2023 07:57:55 GMT
+      - Wed, 26 Jul 2023 08:58:48 GMT
       Expires:
       - '0'
       Pragma:
       - no-cache
       Referrer-Policy:
       - strict-origin-when-cross-origin
       Server:
```

### Comparing `bridgeapi-1.0.0b2/.gitignore` & `bridgeapi-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `bridgeapi-1.0.0b2/LICENSE.txt` & `bridgeapi-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bridgeapi-1.0.0b2/README.md` & `bridgeapi-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `bridgeapi-1.0.0b2/pyproject.toml` & `bridgeapi-1.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
-dependencies = ["pydantic == 1.*", "requests"]
+dependencies = ["pydantic >= 2", "requests"]
 
 [project.urls]
 Documentation = "https://gitlab.com/alex-marty/bridgeapi"
 Issues = "https://gitlab.com/alex-marty/bridgeapi/-/issues"
 Source = "https://gitlab.com/alex-marty/bridgeapi"
 
 [tool.hatch.version]
```

### Comparing `bridgeapi-1.0.0b2/PKG-INFO` & `bridgeapi-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: bridgeapi
-Version: 1.0.0b2
+Version: 1.1.0
 Summary: Client for the Bridge open banking API aggregator
 Project-URL: Documentation, https://gitlab.com/alex-marty/bridgeapi
 Project-URL: Issues, https://gitlab.com/alex-marty/bridgeapi/-/issues
 Project-URL: Source, https://gitlab.com/alex-marty/bridgeapi
 Author-email: Alexandre Marty <contact@marty.in>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
-Requires-Dist: pydantic==1.*
+Requires-Dist: pydantic>=2
 Requires-Dist: requests
 Description-Content-Type: text/markdown
 
 # bridgeapi
 
 [![PyPI - Version](https://img.shields.io/pypi/v/bridgeapi.svg)](https://pypi.org/project/bridgeapi)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/bridgeapi.svg)](https://pypi.org/project/bridgeapi)
```

