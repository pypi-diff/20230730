# Comparing `tmp/scrapli_replay-2023.1.30.post1.tar.gz` & `tmp/scrapli_replay-2023.7.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapli_replay-2023.1.30.post1.tar", last modified: Tue Feb 14 18:00:24 2023, max compression
+gzip compressed data, was "scrapli_replay-2023.7.30.tar", last modified: Sun Jul 30 17:18:45 2023, max compression
```

## Comparing `scrapli_replay-2023.1.30.post1.tar` & `scrapli_replay-2023.7.30.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 18:00:24.419739 scrapli_replay-2023.1.30.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-02-14 18:00:07.000000 scrapli_replay-2023.1.30.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-14 18:00:07.000000 scrapli_replay-2023.1.30.post1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-02-14 18:00:24.419739 scrapli_replay-2023.1.30.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-02-14 18:00:07.000000 scrapli_replay-2023.1.30.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-02-14 18:00:07.000000 scrapli_replay-2023.1.30.post1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-02-14 18:00:07.000000 scrapli_replay-2023.1.30.post1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-02-14 18:00:07.000000 scrapli_replay-2023.1.30.post1/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-02-14 18:00:07.000000 scrapli_replay-2023.1.30.post1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 18:00:24.419739 scrapli_replay-2023.1.30.post1/scrapli_replay/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-02-14 18:00:07.000000 scrapli_replay-2023.1.30.post1/scrapli_replay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-02-14 18:00:07.000000 scrapli_replay-2023.1.30.post1/scrapli_replay/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-02-14 18:00:07.000000 scrapli_replay-2023.1.30.post1/scrapli_replay/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 18:00:07.000000 scrapli_replay-2023.1.30.post1/scrapli_replay/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 18:00:24.419739 scrapli_replay-2023.1.30.post1/scrapli_replay/replay/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 18:00:07.000000 scrapli_replay-2023.1.30.post1/scrapli_replay/replay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-02-14 18:00:07.000000 scrapli_replay-2023.1.30.post1/scrapli_replay/replay/pytest_scrapli_replay.py
--rw-r--r--   0 runner    (1001) docker     (123)    35060 2023-02-14 18:00:07.000000 scrapli_replay-2023.1.30.post1/scrapli_replay/replay/replay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 18:00:24.419739 scrapli_replay-2023.1.30.post1/scrapli_replay/server/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-14 18:00:07.000000 scrapli_replay-2023.1.30.post1/scrapli_replay/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34966 2023-02-14 18:00:07.000000 scrapli_replay-2023.1.30.post1/scrapli_replay/server/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)    15115 2023-02-14 18:00:07.000000 scrapli_replay-2023.1.30.post1/scrapli_replay/server/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 18:00:24.419739 scrapli_replay-2023.1.30.post1/scrapli_replay.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-02-14 18:00:24.000000 scrapli_replay-2023.1.30.post1/scrapli_replay.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-02-14 18:00:24.000000 scrapli_replay-2023.1.30.post1/scrapli_replay.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-14 18:00:24.000000 scrapli_replay-2023.1.30.post1/scrapli_replay.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-02-14 18:00:24.000000 scrapli_replay-2023.1.30.post1/scrapli_replay.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-02-14 18:00:24.000000 scrapli_replay-2023.1.30.post1/scrapli_replay.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-14 18:00:24.000000 scrapli_replay-2023.1.30.post1/scrapli_replay.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-02-14 18:00:24.423739 scrapli_replay-2023.1.30.post1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:18:45.568351 scrapli_replay-2023.7.30/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-30 17:18:28.000000 scrapli_replay-2023.7.30/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-30 17:18:28.000000 scrapli_replay-2023.7.30/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-07-30 17:18:45.568351 scrapli_replay-2023.7.30/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-07-30 17:18:28.000000 scrapli_replay-2023.7.30/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-07-30 17:18:28.000000 scrapli_replay-2023.7.30/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-30 17:18:28.000000 scrapli_replay-2023.7.30/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-30 17:18:28.000000 scrapli_replay-2023.7.30/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-30 17:18:28.000000 scrapli_replay-2023.7.30/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:18:45.564351 scrapli_replay-2023.7.30/scrapli_replay/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-30 17:18:28.000000 scrapli_replay-2023.7.30/scrapli_replay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-30 17:18:28.000000 scrapli_replay-2023.7.30/scrapli_replay/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-07-30 17:18:28.000000 scrapli_replay-2023.7.30/scrapli_replay/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 17:18:28.000000 scrapli_replay-2023.7.30/scrapli_replay/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:18:45.568351 scrapli_replay-2023.7.30/scrapli_replay/replay/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 17:18:28.000000 scrapli_replay-2023.7.30/scrapli_replay/replay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-07-30 17:18:28.000000 scrapli_replay-2023.7.30/scrapli_replay/replay/pytest_scrapli_replay.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35428 2023-07-30 17:18:28.000000 scrapli_replay-2023.7.30/scrapli_replay/replay/replay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:18:45.568351 scrapli_replay-2023.7.30/scrapli_replay/server/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-30 17:18:28.000000 scrapli_replay-2023.7.30/scrapli_replay/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34982 2023-07-30 17:18:28.000000 scrapli_replay-2023.7.30/scrapli_replay/server/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15115 2023-07-30 17:18:28.000000 scrapli_replay-2023.7.30/scrapli_replay/server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:18:45.568351 scrapli_replay-2023.7.30/scrapli_replay.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-07-30 17:18:45.000000 scrapli_replay-2023.7.30/scrapli_replay.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-30 17:18:45.000000 scrapli_replay-2023.7.30/scrapli_replay.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 17:18:45.000000 scrapli_replay-2023.7.30/scrapli_replay.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-30 17:18:45.000000 scrapli_replay-2023.7.30/scrapli_replay.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-30 17:18:45.000000 scrapli_replay-2023.7.30/scrapli_replay.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-30 17:18:45.000000 scrapli_replay-2023.7.30/scrapli_replay.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-30 17:18:45.568351 scrapli_replay-2023.7.30/setup.cfg
```

### Comparing `scrapli_replay-2023.1.30.post1/LICENSE` & `scrapli_replay-2023.7.30/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapli_replay-2023.1.30.post1/PKG-INFO` & `scrapli_replay-2023.7.30/scrapli_replay.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: scrapli_replay
-Version: 2023.1.30.post1
+Name: scrapli-replay
+Version: 2023.7.30
 Summary: Tools to enable easy testing of scrapli programs
 Author-email: Carl Montanari <carl.r.montanari@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Carl Montanari
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -24,15 +24,15 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/scrapli/scrapli_replay
 Project-URL: Changelog, https://scrapli.github.io/scrapli_replay/changelog/
 Project-URL: Docs, https://scrapli.github.io/scrapli_replay/
-Keywords: ssh,telnet,netconf,automation,network,cisco,iosxr,iosxe,nxos,arista,eos,juniper,junos
+Keywords: arista,automation,cisco,eos,iosxe,iosxr,juniper,junos,netconf,network,nxos,ssh,telnet
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `scrapli_replay-2023.1.30.post1/README.md` & `scrapli_replay-2023.7.30/README.md`

 * *Files identical despite different names*

### Comparing `scrapli_replay-2023.1.30.post1/pyproject.toml` & `scrapli_replay-2023.7.30/pyproject.toml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -26,27 +26,27 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 keywords = [
-    "ssh",
-    "telnet",
-    "netconf",
+    "arista",
     "automation",
-    "network",
     "cisco",
-    "iosxr",
-    "iosxe",
-    "nxos",
-    "arista",
     "eos",
+    "iosxe",
+    "iosxr",
     "juniper",
     "junos",
+    "netconf",
+    "network",
+    "nxos",
+    "ssh",
+    "telnet",
 ]
 
 [project.urls]
 Homepage = "https://github.com/scrapli/scrapli_replay"
 Changelog = "https://scrapli.github.io/scrapli_replay/changelog/"
 Docs = "https://scrapli.github.io/scrapli_replay/"
```

### Comparing `scrapli_replay-2023.1.30.post1/scrapli_replay/exceptions.py` & `scrapli_replay-2023.7.30/scrapli_replay/exceptions.py`

 * *Files identical despite different names*

### Comparing `scrapli_replay-2023.1.30.post1/scrapli_replay/logging.py` & `scrapli_replay-2023.7.30/scrapli_replay/logging.py`

 * *Files identical despite different names*

### Comparing `scrapli_replay-2023.1.30.post1/scrapli_replay/replay/pytest_scrapli_replay.py` & `scrapli_replay-2023.7.30/scrapli_replay/replay/pytest_scrapli_replay.py`

 * *Files identical despite different names*

### Comparing `scrapli_replay-2023.1.30.post1/scrapli_replay/replay/replay.py` & `scrapli_replay-2023.7.30/scrapli_replay/replay/replay.py`

 * *Files 2% similar despite different names*

```diff
@@ -628,14 +628,16 @@
             ):
                 self.replay_mode = ReplayMode.RECORD
 
         self._block_network = block_network
         self._patched_open: Optional[mock._patch[Any]] = None  # noqa
         self.wrapped_instances: Dict[str, ScrapliReplayInstance] = {}
 
+        self._channel_close: Optional[Callable[[], None]] = None
+
     def __call__(self, wrapped_func: Callable[..., Any]) -> Callable[..., Any]:
         """
         Use ScrapliReplay as a decorator
 
         Decide if the wrapped function is sync or async and wrap that function/coroutine in context
         manager of self
 
@@ -695,14 +697,17 @@
 
             Raises:
                 N/A
 
             """
             instance_name = self.create_instance_name(scrapli_conn=cls)
 
+            cls.channel.open()
+            self._channel_close = cls.channel.close
+
             connection_profile = self.create_connection_profile(scrapli_conn=cls)
             instance_object = ScrapliReplayInstance(
                 replay_mode=self.replay_mode,
                 connection_profile=connection_profile,
                 replay_session=self.replay_session.get(instance_name, {}),
             )
             self.wrapped_instances[instance_name] = instance_object
@@ -782,14 +787,17 @@
             )
 
         self._patched_open.stop()
 
         if self.replay_mode in (ReplayMode.RECORD, ReplayMode.OVERWRITE):
             self._save()
 
+        if self._channel_close:
+            self._channel_close()
+
     async def __aenter__(self) -> None:
         """
         Enter method for context manager
 
         Args:
             N/A
 
@@ -816,14 +824,17 @@
 
             Raises:
                 N/A
 
             """
             instance_name = self.create_instance_name(scrapli_conn=cls)
 
+            cls.channel.open()
+            self._channel_close = cls.channel.close
+
             connection_profile = self.create_connection_profile(scrapli_conn=cls)
             instance_object = ScrapliReplayInstance(
                 replay_mode=self.replay_mode,
                 connection_profile=connection_profile,
                 replay_session=self.replay_session.get(instance_name, {}),
             )
             self.wrapped_instances[instance_name] = instance_object
@@ -898,14 +909,17 @@
             )
 
         self._patched_open.stop()
 
         if self.replay_mode in (ReplayMode.RECORD, ReplayMode.OVERWRITE):
             self._save()
 
+        if self._channel_close:
+            self._channel_close()
+
     def create_instance_name(self, scrapli_conn: Union[AsyncDriver, Driver]) -> str:
         """
         Create as unique as possible instance name for a given connection
 
         Since hash cant be relied on to between python executions we need to have some way to have a
         decent idea about what connection is what... using the host and port is maybe not enough as
         a user may have multiple connections to the same device in a test session. Adding in the
```

### Comparing `scrapli_replay-2023.1.30.post1/scrapli_replay/server/collector.py` & `scrapli_replay-2023.7.30/scrapli_replay/server/collector.py`

 * *Files 0% similar despite different names*

```diff
@@ -914,15 +914,15 @@
                         )
                         else "interactive"
                     )
 
         for privilege_level in self.unknown_events:
             for on_open_state in self.unknown_events[privilege_level]:
                 self.dumpable_unknown_events[privilege_level][on_open_state] = asdict(
-                    self.unknown_events[privilege_level][on_open_state]
+                    self.unknown_events[privilege_level][on_open_state]  # type: ignore
                 )
 
     def dump(self) -> None:
         """
         Primary public dump method to dump collected data out to yaml
 
         Args:
```

### Comparing `scrapli_replay-2023.1.30.post1/scrapli_replay/server/server.py` & `scrapli_replay-2023.7.30/scrapli_replay/server/server.py`

 * *Files identical despite different names*

### Comparing `scrapli_replay-2023.1.30.post1/scrapli_replay.egg-info/PKG-INFO` & `scrapli_replay-2023.7.30/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: scrapli-replay
-Version: 2023.1.30.post1
+Name: scrapli_replay
+Version: 2023.7.30
 Summary: Tools to enable easy testing of scrapli programs
 Author-email: Carl Montanari <carl.r.montanari@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Carl Montanari
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -24,15 +24,15 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/scrapli/scrapli_replay
 Project-URL: Changelog, https://scrapli.github.io/scrapli_replay/changelog/
 Project-URL: Docs, https://scrapli.github.io/scrapli_replay/
-Keywords: ssh,telnet,netconf,automation,network,cisco,iosxr,iosxe,nxos,arista,eos,juniper,junos
+Keywords: arista,automation,cisco,eos,iosxe,iosxr,juniper,junos,netconf,network,nxos,ssh,telnet
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `scrapli_replay-2023.1.30.post1/scrapli_replay.egg-info/SOURCES.txt` & `scrapli_replay-2023.7.30/scrapli_replay.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scrapli_replay-2023.1.30.post1/scrapli_replay.egg-info/requires.txt` & `scrapli_replay-2023.7.30/scrapli_replay.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 asyncssh<3.0.0,>=2.2.1
 ruamel.yaml<0.18,>=0.17
 scrapli>=2021.07.30
 
 [dev]
-black==23.1.0
+black<24.0.0,>=23.3.0
 darglint<2.0.0,>=1.8.1
 isort<6.0.0,>=5.10.1
-mypy==0.991
-nox==2022.11.21
+mypy==1.4.1
+nox==2023.4.22
 pycodestyle<3.0.0,>=2.8.0
 pydocstyle<7.0.0,>=6.1.1
 pyfakefs<6.0.0,>=5.0.0
 pylama<9.0.0,>=8.4.0
-pylint==2.16.2
+pylint==2.17.5
 pytest-asyncio<1.0.0,>=0.17.0
 pytest-cov<5.0.0,>=3.0.0
 pytest<8.0.0,>=7.0.0
 toml<1.0.0,>=0.10.2
 
 [docs]
 mdx-gh-links<1.0,>=0.2
```

