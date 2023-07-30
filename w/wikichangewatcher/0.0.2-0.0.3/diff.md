# Comparing `tmp/wikichangewatcher-0.0.2-py3-none-any.whl.zip` & `tmp/wikichangewatcher-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,9 @@
-Zip file size: 5684 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat      486 b- defN 23-Jul-30 18:44 wikichangewatcher/__init__.py
--rw-rw-rw-  2.0 fat     8402 b- defN 23-Jul-30 18:29 wikichangewatcher/wikichangewatcher.py
--rw-rw-rw-  2.0 fat     9903 b- defN 23-Jul-30 18:44 wikichangewatcher-0.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-30 18:44 wikichangewatcher-0.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       18 b- defN 23-Jul-30 18:44 wikichangewatcher-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      518 b- defN 23-Jul-30 18:44 wikichangewatcher-0.0.2.dist-info/RECORD
-6 files, 19419 bytes uncompressed, 4736 bytes compressed:  75.6%
+Zip file size: 10196 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat      486 b- defN 23-Jul-30 21:36 wikichangewatcher/__init__.py
+-rw-rw-rw-  2.0 fat    10132 b- defN 23-Jul-30 21:33 wikichangewatcher/wikichangewatcher.py
+-rw-rw-rw-  2.0 fat    10761 b- defN 23-Jul-30 21:36 wikichangewatcher-0.0.3.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     9936 b- defN 23-Jul-30 21:36 wikichangewatcher-0.0.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-30 21:36 wikichangewatcher-0.0.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       18 b- defN 23-Jul-30 21:36 wikichangewatcher-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      618 b- defN 23-Jul-30 21:36 wikichangewatcher-0.0.3.dist-info/RECORD
+7 files, 32043 bytes uncompressed, 9090 bytes compressed:  71.6%
```

## zipnote {}

```diff
@@ -1,19 +1,22 @@
 Filename: wikichangewatcher/__init__.py
 Comment: 
 
 Filename: wikichangewatcher/wikichangewatcher.py
 Comment: 
 
-Filename: wikichangewatcher-0.0.2.dist-info/METADATA
+Filename: wikichangewatcher-0.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: wikichangewatcher-0.0.2.dist-info/WHEEL
+Filename: wikichangewatcher-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: wikichangewatcher-0.0.2.dist-info/top_level.txt
+Filename: wikichangewatcher-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: wikichangewatcher-0.0.2.dist-info/RECORD
+Filename: wikichangewatcher-0.0.3.dist-info/top_level.txt
+Comment: 
+
+Filename: wikichangewatcher-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## wikichangewatcher/__init__.py

```diff
@@ -1,7 +1,7 @@
-__version__ = "0.0.2"
+__version__ = "0.0.3"
 
 from wikichangewatcher.wikichangewatcher import FieldFilter, FilterCollection, IpV4Filter, WikiChangeWatcher, MatchType
 from wikichangewatcher.wikichangewatcher import FieldStringFilter, FieldRegexMatchFilter, FieldRegexSearchFilter
 from wikichangewatcher.wikichangewatcher import UsernameFilter, UsernameRegexMatchFilter, UsernameRegexSearchFilter
 from wikichangewatcher.wikichangewatcher import PageUrlFilter, PageUrlRegexMatchFilter, PageUrlRegexSearchFilter
```

## wikichangewatcher/wikichangewatcher.py

```diff
@@ -1,12 +1,13 @@
-import time
-import sys
 import re
 import threading
+import requests
 import json
+import ctypes
+from typing import Callable, Type, Self
 
 from sseclient import SSEClient
 
 
 WIKIMEDIA_URL = 'https://stream.wikimedia.org/v2/stream/recentchange'
 
 
@@ -17,25 +18,25 @@
 
     The json_data provided to the on_match callback is an JSON-encoded event from the WikiMedia
     "recent changes" event stream, as described here: https://www.mediawiki.org/wiki/Manual:RCFeed
     """
     def __init__(self):
         self._on_match = None
 
-    def on_match(self, on_match_handler):
+    def on_match(self, on_match_handler: Callable[[dict], None]) -> Self:
         self._on_match = on_match_handler
         return self
 
-    def _handler(self, json_data):
+    def _handler(self, json_data: dict) -> bool:
         raise NotImplementedError
 
-    def check_match(self, json_data):
+    def check_match(self, json_data: dict) -> bool:
         return self._handler(json_data)
 
-    def run_on_match(self, json_data):
+    def run_on_match(self, json_data: dict):
         if self._on_match is not None:
             self._on_match(json_data)
 
 
 class MatchType(object):
     """
     Enumerates all match types handled by a FilterCollection
@@ -48,34 +49,37 @@
     """
     A Filter object that holds multiple filters, and can run a callback if all or any one
     of the filters matches
     """
     def __init__(self, *filters):
         super(FilterCollection, self).__init__()
         self._filters = filters
-        self._on_all_match_handler = None
-        self._on_any_match_handler = None
         self._match_type = MatchType.ALL
 
-    def set_match_type(self, match_type):
+    def set_match_type(self, match_type: int) -> Self:
+        """
+        Set match type for this collection. If MatchType.ALL, then this collection will
+        match only if all contained filters match. If MatchType.ANY, then this collection will
+        match if one of the contained filters match.
+        """
         self._match_type = match_type
         return self
 
-    def _handler(self, json_data):
+    def _handler(self, json_data: dict) -> bool:
         match = False
 
         if self._match_type == MatchType.ALL:
             match = all(f.check_match(json_data) for f in self._filters)
 
         elif self._match_type == MatchType.ANY:
             match = any(f.check_match(json_data) for f in self._filters)
 
         return match
 
-def _ipv4_field_tostr(stringval):
+def _ipv4_field_tostr(stringval: str) -> int:
     intval = int(stringval)
     if not (0 <= intval <= 255):
         raise ValueError
 
     return intval
 
 
@@ -109,15 +113,15 @@
 
             if error:
                 raise ValueError(f"Invalid field '{x}' in IP address pattern '{ip_addr_pattern}'")
 
         if len(self.ip_addr_pattern) != 4:
             raise ValueError(f"Invalid number of fields ({len(self.ip_addr_pattern)}) for IP address pattern (expected 4)")
 
-    def _handler(self, json_data):
+    def _handler(self, json_data: dict) -> bool:
         if "user" not in json_data:
             return False
 
         ipaddr = json_data["user"]
 
         try:
             fields = [int(x) for x in ipaddr.split(".")]
@@ -143,133 +147,165 @@
         return True
 
 
 class FieldStringFilter(FieldFilter):
     """
     FieldFilter implementation to watch for a named field with a specific fixed string
     """
-    def __init__(self, fieldname, value):
+    def __init__(self, fieldname: str, value: str):
         super(FieldStringFilter, self).__init__()
         self.fieldname = fieldname
         self.value = value
 
-    def _handler(self, json_data):
+    def _handler(self, json_data: dict) -> bool:
         if self.fieldname not in json_data:
             return False
 
         return json_data[self.fieldname] == self.value
 
 
 class FieldRegexMatchFilter(FieldFilter):
     """
     FieldFilter implementation to watch for a named field that matches a provided regular expression
     """
-    def __init__(self, fieldname, regex):
+    def __init__(self, fieldname: str, regex: str):
         super(FieldRegexMatchFilter, self).__init__()
         self.fieldname = fieldname
         self.regex = re.compile(regex)
 
-    def _handler(self, json_data):
+    def _handler(self, json_data: dict) -> bool:
         if self.fieldname not in json_data:
             return False
 
         return bool(self.regex.match(json_data[self.fieldname]))
 
 
 class FieldRegexSearchFilter(FieldFilter):
     """
     FieldFilter implementation to watch for a named field that contains one or more instances of
     the provided regular expression
     """
-    def __init__(self, fieldname, regex):
+    def __init__(self, fieldname: str, regex: str):
         super(FieldRegexSearchFilter, self).__init__()
         self.fieldname = fieldname
         self.regex = re.compile(regex)
 
-    def _handler(self, json_data):
+    def _handler(self, json_data: dict) -> bool:
         if self.fieldname not in json_data:
             return False
 
         return bool(self.regex.search(json_data[self.fieldname]))
 
 
 class PageUrlFilter(FieldStringFilter):
     """
     FieldString Filter implementation to watch for a specific page URL
     """
-    def __init__(self, page_url):
+    def __init__(self, page_url: str):
         super(PageUrlFilter, self).__init__("title_url", page_url)
 
 
 class PageUrlRegexMatchFilter(FieldRegexMatchFilter):
     """
     FieldRegexMatchFilter implementation to watch for a "title_url" field that matches a provided regular expression
     """
-    def __init__(self, regex):
+    def __init__(self, regex: str):
         super(UsernameRegexMatchFilter, self).__init__("title_url", regex)
 
 
 class PageUrlRegexSearchFilter(FieldRegexSearchFilter):
     """
     FieldRegexSearchFilter implementation to watch for a "title_url" field that contains one or more matches of
     a provided regular expression
     """
-    def __init__(self, regex):
+    def __init__(self, regex: str):
         super(UsernameRegexSearchFilter, self).__init__("title_url", regex)
 
 
 class UsernameFilter(FieldStringFilter):
     """
     FieldStringFilter implementation to watch for a "user" field with a specific fixed string
     """
-    def __init__(self, string):
+    def __init__(self, string: str):
         super(UsernameFilter, self).__init__("user", string)
 
 
 class UsernameRegexMatchFilter(FieldRegexMatchFilter):
     """
     FieldRegexMatchFilter implementation to watch for a "user" field that matches a provided regular expression
     """
-    def __init__(self, regex):
+    def __init__(self, regex: str):
         super(UsernameRegexMatchFilter, self).__init__("user", regex)
 
 
 class UsernameRegexSearchFilter(FieldRegexSearchFilter):
     """
     FieldRegexSearchFilter implementation to watch for a "user" field that contains one or more matches of
     a provided regular expression
     """
-    def __init__(self, regex):
+    def __init__(self, regex: str):
         super(UsernameRegexSearchFilter, self).__init__("user", regex)
 
 
 class WikiChangeWatcher(object):
     """
     Consumes all events from the Wikimedia "recent changes" stream, and
     applies all provided FieldFilter instances to each received event.
     """
     def __init__(self, *filters):
         self._thread = None
         self._stop_event = threading.Event()
         self._filters = filters
+        self._session = requests.Session()
+        self._client = SSEClient(WIKIMEDIA_URL, session=self._session)
 
-    def add_filter(self, filter):
-        self._filters.append(filter)
+    def add_filter(self, fltr: Type[FieldFilter]) -> Self:
+        """
+        Add a new filter to the list of active filters
+        """
+        self._filters.append(fltr)
+        return self
 
     def run(self):
+        """
+        Start WikiWatcher running in a separate thread
+        """
+        if self._thread is not None:
+            raise RuntimeError("'run()' has already been called!")
+
         self._thread = threading.Thread(target=self._thread_task)
         self._thread.daemon = True
         self._thread.start()
 
     def stop(self):
-        self._stop_event.set()
+        """
+        Send stop event to the running WikiWatcher thread and wait for it to terminate
+        """
+        if self._thread is None:
+            return
+
+        # Use CPython API to inject a SystemExit exception into the WikiWatcher thread.
+        # Unfortunately, sseclient lib does not provide any way to terminate waiting for
+        # the next event, so this is the only way to stop the thread without having
+        # to wait for the next event.
+        exception = SystemExit
+        target_tid = self._thread.ident
+
+        ret = ctypes.pythonapi.PyThreadState_SetAsyncExc(ctypes.c_long(target_tid), ctypes.py_object(exception))
+        if ret == 0:
+            raise ValueError("Invalid thread ID")
+        elif ret > 1:
+            ctypes.pythonapi.PyThreadState_SetAsyncExc(target_tid, NULL)
+            raise SystemError("PyThreadState_SetAsyncExc failed")
+
         self._thread.join()
+        self._thread = None
 
     def _thread_task(self):
-        for event in SSEClient(WIKIMEDIA_URL):
+        for event in self._client:
             if self._stop_event.is_set():
                 return
 
             if event.event == "message":
                 try:
                     change = json.loads(event.data)
                 except ValueError:
```

## Comparing `wikichangewatcher-0.0.2.dist-info/METADATA` & `wikichangewatcher-0.0.3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: wikichangewatcher
-Version: 0.0.2
-Summary: Real-time monitoring of global Wikipedia page edits
+Version: 0.0.3
+Summary: Real-time monitoring/filtering of global Wikipedia page edits
 Home-page: http://github.com/eriknyquist/wikichangewatcher
 Author: Erik Nyquist
 Author-email: eknyquist@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
+License-File: LICENSE
 Requires-Dist: sseclient
 
 WikiChangeWatcher
 =================
 
 .. contents:: Table of Contents
```

