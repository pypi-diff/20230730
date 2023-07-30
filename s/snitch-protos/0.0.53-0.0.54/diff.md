# Comparing `tmp/snitch-protos-0.0.53.tar.gz` & `tmp/snitch-protos-0.0.54.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snitch-protos-0.0.53.tar", last modified: Fri Jul 28 22:08:45 2023, max compression
+gzip compressed data, was "snitch-protos-0.0.54.tar", last modified: Sun Jul 30 18:55:41 2023, max compression
```

## Comparing `snitch-protos-0.0.53.tar` & `snitch-protos-0.0.54.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:08:45.403022 snitch-protos-0.0.53/
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-28 22:08:45.403022 snitch-protos-0.0.53/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-28 22:08:12.000000 snitch-protos-0.0.53/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 22:08:45.403022 snitch-protos-0.0.53/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-28 22:08:44.000000 snitch-protos-0.0.53/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:08:45.399022 snitch-protos-0.0.53/snitch_protos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 22:08:12.000000 snitch-protos-0.0.53/snitch_protos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:08:45.403022 snitch-protos-0.0.53/snitch_protos/protos/
--rw-r--r--   0 runner    (1001) docker     (123)    33159 2023-07-28 22:08:12.000000 snitch-protos-0.0.53/snitch_protos/protos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:08:45.403022 snitch-protos-0.0.53/snitch_protos/protos/steps/
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-07-28 22:08:12.000000 snitch-protos-0.0.53/snitch_protos/protos/steps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:08:45.403022 snitch-protos-0.0.53/snitch_protos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-28 22:08:45.000000 snitch-protos-0.0.53/snitch_protos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-28 22:08:45.000000 snitch-protos-0.0.53/snitch_protos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 22:08:45.000000 snitch-protos-0.0.53/snitch_protos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-28 22:08:45.000000 snitch-protos-0.0.53/snitch_protos.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:55:41.122539 snitch-protos-0.0.54/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-30 18:55:41.118538 snitch-protos-0.0.54/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-30 18:55:08.000000 snitch-protos-0.0.54/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 18:55:41.122539 snitch-protos-0.0.54/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-30 18:55:40.000000 snitch-protos-0.0.54/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:55:41.118538 snitch-protos-0.0.54/snitch_protos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 18:55:08.000000 snitch-protos-0.0.54/snitch_protos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:55:41.118538 snitch-protos-0.0.54/snitch_protos/protos/
+-rw-r--r--   0 runner    (1001) docker     (123)    34958 2023-07-30 18:55:08.000000 snitch-protos-0.0.54/snitch_protos/protos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:55:41.118538 snitch-protos-0.0.54/snitch_protos/protos/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-07-30 18:55:08.000000 snitch-protos-0.0.54/snitch_protos/protos/steps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:55:41.118538 snitch-protos-0.0.54/snitch_protos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-30 18:55:41.000000 snitch-protos-0.0.54/snitch_protos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-30 18:55:41.000000 snitch-protos-0.0.54/snitch_protos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 18:55:41.000000 snitch-protos-0.0.54/snitch_protos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-30 18:55:41.000000 snitch-protos-0.0.54/snitch_protos.egg-info/top_level.txt
```

### Comparing `snitch-protos-0.0.53/PKG-INFO` & `snitch-protos-0.0.54/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snitch-protos
-Version: 0.0.53
+Version: 0.0.54
 Summary: Protobuf python package for Streamdal.com Snitch
 Home-page: https://github.com/streamdal/snitch-protos
 Author: Streamdal.com
 Author-email: engineering@streamdal.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
```

### Comparing `snitch-protos-0.0.53/setup.py` & `snitch-protos-0.0.54/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='snitch-protos',
-    version='0.0.53',
+    version='0.0.54',
     description='Protobuf python package for Streamdal.com Snitch',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/streamdal/snitch-protos',
     author='Streamdal.com',
     author_email='engineering@streamdal.com',
     license='MIT',
```

### Comparing `snitch-protos-0.0.53/snitch_protos/protos/__init__.py` & `snitch-protos-0.0.54/snitch_protos/protos/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -317,22 +317,31 @@
 
 @dataclass(eq=False, repr=False)
 class KeepAliveCommand(betterproto.Message):
     pass
 
 
 @dataclass(eq=False, repr=False)
+class NewAudienceRequest(betterproto.Message):
+    session_id: str = betterproto.string_field(1)
+    """The session that is performing this call"""
+
+    audience: "Audience" = betterproto.message_field(2)
+    """Newly created audience."""
+
+
+@dataclass(eq=False, repr=False)
 class HeartbeatRequest(betterproto.Message):
     """
     Each consumer and producer should send periodic heartbeats to the server to
     let the server know that they are still active.
     """
 
-    audience: "Audience" = betterproto.message_field(1)
-    last_activity_unix_timestamp_utc: int = betterproto.int64_field(2)
+    session_id: str = betterproto.string_field(1)
+    """Session ID for this instance of the SDK."""
 
 
 @dataclass(eq=False, repr=False)
 class NotifyRequest(betterproto.Message):
     pipeline_id: str = betterproto.string_field(1)
     step_name: str = betterproto.string_field(2)
     audience: "Audience" = betterproto.message_field(3)
@@ -352,30 +361,39 @@
 class MetricsRequest(betterproto.Message):
     metrics: List["Metrics"] = betterproto.message_field(1)
 
 
 @dataclass(eq=False, repr=False)
 class RegisterRequest(betterproto.Message):
     service_name: str = betterproto.string_field(1)
-    dry_run: bool = betterproto.bool_field(2)
+    """REQUIRED -- Name of the service that is registering."""
+
+    session_id: str = betterproto.string_field(2)
     """
-    If set, we know that any pipelines or steps executed in this SDK will NOT
-    modify the input/output data. As in, the SDK will log what it _would_ do
-    and always return the original data set.
+    REQUIRED -- Unique ID for this SDK instance. This should be generated every
+    time the SDK is instantiated (oe. every time a NEW registration is
+    performed).
     """
 
     client_info: "ClientInfo" = betterproto.message_field(3)
-    """Info about the client (lib name, lang, os, arch, etc.)"""
+    """REQUIRED -- Info about the client (lib name, lang, os, arch, etc.)"""
 
     audiences: List["Audience"] = betterproto.message_field(4)
     """
     OPTIONAL -- if these are defined, these will show up in the UI even if
     there is no active .Process() call from the SDK.
     """
 
+    dry_run: bool = betterproto.bool_field(5)
+    """
+    OPTIONAL -- If set, we know that any pipelines or steps executed in this
+    SDK will NOT modify the input/output data. As in, the SDK will log what it
+    _would_ do and always return the original data set.
+    """
+
 
 @dataclass(eq=False, repr=False)
 class DeregisterRequest(betterproto.Message):
     """
     Same as RegisterRequest - used for broadcasting a deregistration event
     """
 
@@ -653,14 +671,31 @@
             Command,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         ):
             yield response
 
+    async def new_audience(
+        self,
+        new_audience_request: "NewAudienceRequest",
+        *,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None
+    ) -> "StandardResponse":
+        return await self._unary_unary(
+            "/protos.Internal/NewAudience",
+            new_audience_request,
+            StandardResponse,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        )
+
     async def heartbeat(
         self,
         heartbeat_request: "HeartbeatRequest",
         *,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None
@@ -915,14 +950,19 @@
 class InternalBase(ServiceBase):
     async def register(
         self, register_request: "RegisterRequest"
     ) -> AsyncIterator["Command"]:
         raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
         yield Command()
 
+    async def new_audience(
+        self, new_audience_request: "NewAudienceRequest"
+    ) -> "StandardResponse":
+        raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
+
     async def heartbeat(
         self, heartbeat_request: "HeartbeatRequest"
     ) -> "StandardResponse":
         raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
 
     async def notify(self, notify_request: "NotifyRequest") -> "StandardResponse":
         raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
@@ -936,14 +976,21 @@
         request = await stream.recv_message()
         await self._call_rpc_handler_server_stream(
             self.register,
             stream,
             request,
         )
 
+    async def __rpc_new_audience(
+        self, stream: "grpclib.server.Stream[NewAudienceRequest, StandardResponse]"
+    ) -> None:
+        request = await stream.recv_message()
+        response = await self.new_audience(request)
+        await stream.send_message(response)
+
     async def __rpc_heartbeat(
         self, stream: "grpclib.server.Stream[HeartbeatRequest, StandardResponse]"
     ) -> None:
         request = await stream.recv_message()
         response = await self.heartbeat(request)
         await stream.send_message(response)
 
@@ -965,14 +1012,20 @@
         return {
             "/protos.Internal/Register": grpclib.const.Handler(
                 self.__rpc_register,
                 grpclib.const.Cardinality.UNARY_STREAM,
                 RegisterRequest,
                 Command,
             ),
+            "/protos.Internal/NewAudience": grpclib.const.Handler(
+                self.__rpc_new_audience,
+                grpclib.const.Cardinality.UNARY_UNARY,
+                NewAudienceRequest,
+                StandardResponse,
+            ),
             "/protos.Internal/Heartbeat": grpclib.const.Handler(
                 self.__rpc_heartbeat,
                 grpclib.const.Cardinality.UNARY_UNARY,
                 HeartbeatRequest,
                 StandardResponse,
             ),
             "/protos.Internal/Notify": grpclib.const.Handler(
```

### Comparing `snitch-protos-0.0.53/snitch_protos/protos/steps/__init__.py` & `snitch-protos-0.0.54/snitch_protos/protos/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `snitch-protos-0.0.53/snitch_protos.egg-info/PKG-INFO` & `snitch-protos-0.0.54/snitch_protos.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snitch-protos
-Version: 0.0.53
+Version: 0.0.54
 Summary: Protobuf python package for Streamdal.com Snitch
 Home-page: https://github.com/streamdal/snitch-protos
 Author: Streamdal.com
 Author-email: engineering@streamdal.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
```

