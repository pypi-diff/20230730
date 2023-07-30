# Comparing `tmp/wikichangewatcher-0.0.1-py3-none-any.whl.zip` & `tmp/wikichangewatcher-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 4923 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat      358 b- defN 23-Jul-24 05:45 wikichangewatcher/__init__.py
--rw-rw-rw-  2.0 fat     6540 b- defN 23-Jul-24 04:46 wikichangewatcher/wikichangewatcher.py
--rw-rw-rw-  2.0 fat     6520 b- defN 23-Jul-24 05:58 wikichangewatcher-0.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-24 05:58 wikichangewatcher-0.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       18 b- defN 23-Jul-24 05:58 wikichangewatcher-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      518 b- defN 23-Jul-24 05:58 wikichangewatcher-0.0.1.dist-info/RECORD
-6 files, 14046 bytes uncompressed, 3975 bytes compressed:  71.7%
+Zip file size: 5684 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat      486 b- defN 23-Jul-30 18:44 wikichangewatcher/__init__.py
+-rw-rw-rw-  2.0 fat     8402 b- defN 23-Jul-30 18:29 wikichangewatcher/wikichangewatcher.py
+-rw-rw-rw-  2.0 fat     9903 b- defN 23-Jul-30 18:44 wikichangewatcher-0.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-30 18:44 wikichangewatcher-0.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       18 b- defN 23-Jul-30 18:44 wikichangewatcher-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      518 b- defN 23-Jul-30 18:44 wikichangewatcher-0.0.2.dist-info/RECORD
+6 files, 19419 bytes uncompressed, 4736 bytes compressed:  75.6%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: wikichangewatcher/__init__.py
 Comment: 
 
 Filename: wikichangewatcher/wikichangewatcher.py
 Comment: 
 
-Filename: wikichangewatcher-0.0.1.dist-info/METADATA
+Filename: wikichangewatcher-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: wikichangewatcher-0.0.1.dist-info/WHEEL
+Filename: wikichangewatcher-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: wikichangewatcher-0.0.1.dist-info/top_level.txt
+Filename: wikichangewatcher-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: wikichangewatcher-0.0.1.dist-info/RECORD
+Filename: wikichangewatcher-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## wikichangewatcher/__init__.py

```diff
@@ -1,6 +1,7 @@
-__version__ = "0.0.1"
+__version__ = "0.0.2"
 
-from wikichangewatcher.wikichangewatcher import FieldWatcher, IpV4Watcher, WikiChangeWatcher
-from wikichangewatcher.wikichangewatcher import FieldStringWatcher, FieldRegexMatchWatcher, FieldRegexSearchWatcher
-from wikichangewatcher.wikichangewatcher import UsernameStringWatcher, UsernameRegexMatchWatcher, UsernameRegexSearchWatcher
+from wikichangewatcher.wikichangewatcher import FieldFilter, FilterCollection, IpV4Filter, WikiChangeWatcher, MatchType
+from wikichangewatcher.wikichangewatcher import FieldStringFilter, FieldRegexMatchFilter, FieldRegexSearchFilter
+from wikichangewatcher.wikichangewatcher import UsernameFilter, UsernameRegexMatchFilter, UsernameRegexSearchFilter
+from wikichangewatcher.wikichangewatcher import PageUrlFilter, PageUrlRegexMatchFilter, PageUrlRegexSearchFilter
```

## wikichangewatcher/wikichangewatcher.py

```diff
@@ -6,48 +6,90 @@
 
 from sseclient import SSEClient
 
 
 WIKIMEDIA_URL = 'https://stream.wikimedia.org/v2/stream/recentchange'
 
 
-class FieldWatcher(object):
+class FieldFilter(object):
     """
-    Generic/abstract  class for checking whether a specific field of the "recent changes"
+    Generic/abstract class for checking whether a specific field of the "recent changes"
     JSON event data matches some expected format/values.
 
     The json_data provided to the on_match callback is an JSON-encoded event from the WikiMedia
     "recent changes" event stream, as described here: https://www.mediawiki.org/wiki/Manual:RCFeed
     """
-    def __init__(self, on_match):
-        self._on_match = on_match
+    def __init__(self):
+        self._on_match = None
+
+    def on_match(self, on_match_handler):
+        self._on_match = on_match_handler
+        return self
 
     def _handler(self, json_data):
         raise NotImplementedError
 
     def check_match(self, json_data):
-        if self._handler(json_data):
+        return self._handler(json_data)
+
+    def run_on_match(self, json_data):
+        if self._on_match is not None:
             self._on_match(json_data)
 
 
+class MatchType(object):
+    """
+    Enumerates all match types handled by a FilterCollection
+    """
+    ALL = 0
+    ANY = 1
+
+
+class FilterCollection(FieldFilter):
+    """
+    A Filter object that holds multiple filters, and can run a callback if all or any one
+    of the filters matches
+    """
+    def __init__(self, *filters):
+        super(FilterCollection, self).__init__()
+        self._filters = filters
+        self._on_all_match_handler = None
+        self._on_any_match_handler = None
+        self._match_type = MatchType.ALL
+
+    def set_match_type(self, match_type):
+        self._match_type = match_type
+        return self
+
+    def _handler(self, json_data):
+        match = False
+
+        if self._match_type == MatchType.ALL:
+            match = all(f.check_match(json_data) for f in self._filters)
+
+        elif self._match_type == MatchType.ANY:
+            match = any(f.check_match(json_data) for f in self._filters)
+
+        return match
+
 def _ipv4_field_tostr(stringval):
     intval = int(stringval)
     if not (0 <= intval <= 255):
         raise ValueError
 
     return intval
 
 
-class IpV4Watcher(FieldWatcher):
+class IpV4Filter(FieldFilter):
     """
     FieldWatcher implementation to watch for "user" fields that contain IPv4 addresses
     in the specified ranges
     """
-    def __init__(self, on_match, ip_addr_pattern="*.*.*.*"):
-        super(IpV4Watcher, self).__init__(on_match)
+    def __init__(self, ip_addr_pattern="*.*.*.*"):
+        super(IpV4Filter, self).__init__()
         self.ip_addr_pattern = []
 
         for x in ip_addr_pattern.split("."):
             error = False
 
             if x == "*":
                 self.ip_addr_pattern.append(None)
@@ -97,100 +139,125 @@
 
             elif self.ip_addr_pattern[i] != fields[i]:
                 return False
 
         return True
 
 
-class FieldStringWatcher(FieldWatcher):
+class FieldStringFilter(FieldFilter):
     """
-    FieldWatcher implementation to watch for a named field with a specific fixed string
+    FieldFilter implementation to watch for a named field with a specific fixed string
     """
-    def __init__(self, on_match, fieldname, value):
-        super(FieldStringWatcher, self).__init__(on_match)
+    def __init__(self, fieldname, value):
+        super(FieldStringFilter, self).__init__()
         self.fieldname = fieldname
-        self.value
+        self.value = value
 
     def _handler(self, json_data):
         if self.fieldname not in json_data:
             return False
 
         return json_data[self.fieldname] == self.value
 
 
-class FieldRegexMatchWatcher(FieldWatcher):
+class FieldRegexMatchFilter(FieldFilter):
     """
-    FieldWatcher implementation to watch for a named field that matches a provided regular expression
+    FieldFilter implementation to watch for a named field that matches a provided regular expression
     """
-    def __init__(self, on_match, fieldname, regex):
-        super(FieldRegexMatchWatcher, self).__init__(on_match)
+    def __init__(self, fieldname, regex):
+        super(FieldRegexMatchFilter, self).__init__()
         self.fieldname = fieldname
         self.regex = re.compile(regex)
 
     def _handler(self, json_data):
         if self.fieldname not in json_data:
             return False
 
         return bool(self.regex.match(json_data[self.fieldname]))
 
 
-class FieldRegexSearchWatcher(FieldWatcher):
+class FieldRegexSearchFilter(FieldFilter):
     """
-    FieldWatcher implementation to watch for a named field that contains one or more instances of
+    FieldFilter implementation to watch for a named field that contains one or more instances of
     the provided regular expression
     """
-    def __init__(self, on_match, fieldname, regex):
-        super(FieldRegexSearchWatcher, self).__init__(on_match)
+    def __init__(self, fieldname, regex):
+        super(FieldRegexSearchFilter, self).__init__()
         self.fieldname = fieldname
         self.regex = re.compile(regex)
 
     def _handler(self, json_data):
         if self.fieldname not in json_data:
             return False
 
         return bool(self.regex.search(json_data[self.fieldname]))
 
 
-class UsernameStringWatcher(FieldStringWatcher):
+class PageUrlFilter(FieldStringFilter):
+    """
+    FieldString Filter implementation to watch for a specific page URL
+    """
+    def __init__(self, page_url):
+        super(PageUrlFilter, self).__init__("title_url", page_url)
+
+
+class PageUrlRegexMatchFilter(FieldRegexMatchFilter):
+    """
+    FieldRegexMatchFilter implementation to watch for a "title_url" field that matches a provided regular expression
+    """
+    def __init__(self, regex):
+        super(UsernameRegexMatchFilter, self).__init__("title_url", regex)
+
+
+class PageUrlRegexSearchFilter(FieldRegexSearchFilter):
+    """
+    FieldRegexSearchFilter implementation to watch for a "title_url" field that contains one or more matches of
+    a provided regular expression
+    """
+    def __init__(self, regex):
+        super(UsernameRegexSearchFilter, self).__init__("title_url", regex)
+
+
+class UsernameFilter(FieldStringFilter):
     """
-    FieldStringWatcher implementation to watch for a "user" field with a specific fixed string
+    FieldStringFilter implementation to watch for a "user" field with a specific fixed string
     """
-    def __init__(self, on_match, string):
-        super(UsernameStringWatcher, self).__init__(on_match, "user", string)
+    def __init__(self, string):
+        super(UsernameFilter, self).__init__("user", string)
 
 
-class UsernameRegexMatchWatcher(FieldRegexMatchWatcher):
+class UsernameRegexMatchFilter(FieldRegexMatchFilter):
     """
-    FieldRegexMatchWatcher implementation to watch for a "user" field that matches a provided regular expression
+    FieldRegexMatchFilter implementation to watch for a "user" field that matches a provided regular expression
     """
-    def __init__(self, on_match, regex):
-        super(UsernameRegexMatchWatcher, self).__init__(on_match, "user", regex)
+    def __init__(self, regex):
+        super(UsernameRegexMatchFilter, self).__init__("user", regex)
 
 
-class UsernameRegexSearchWatcher(FieldRegexSearchWatcher):
+class UsernameRegexSearchFilter(FieldRegexSearchFilter):
     """
-    FieldRegexSearchWatcher implementation to watch for a "user" field that contains one or more matches of
+    FieldRegexSearchFilter implementation to watch for a "user" field that contains one or more matches of
     a provided regular expression
     """
-    def __init__(self, on_match, regex):
-        super(UsernameRegexSearchWatcher, self).__init__(on_match, "user", regex)
+    def __init__(self, regex):
+        super(UsernameRegexSearchFilter, self).__init__("user", regex)
 
 
 class WikiChangeWatcher(object):
     """
     Consumes all events from the Wikimedia "recent changes" stream, and
-    applies all provided FieldWatcher instances to each received event.
+    applies all provided FieldFilter instances to each received event.
     """
-    def __init__(self, watchers=[]):
+    def __init__(self, *filters):
         self._thread = None
         self._stop_event = threading.Event()
-        self._watchers = watchers
+        self._filters = filters
 
-    def add_watcher(self, watcher):
-        self._watchers.append(watcher)
+    def add_filter(self, filter):
+        self._filters.append(filter)
 
     def run(self):
         self._thread = threading.Thread(target=self._thread_task)
         self._thread.daemon = True
         self._thread.start()
 
     def stop(self):
@@ -204,9 +271,10 @@
 
             if event.event == "message":
                 try:
                     change = json.loads(event.data)
                 except ValueError:
                     continue
 
-                for w in self._watchers:
-                    w.check_match(change)
+                for f in self._filters:
+                    if f.check_match(change):
+                        f.run_on_match(change)
```

## Comparing `wikichangewatcher-0.0.1.dist-info/METADATA` & `wikichangewatcher-0.0.2.dist-info/METADATA`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wikichangewatcher
-Version: 0.0.1
+Version: 0.0.2
 Summary: Real-time monitoring of global Wikipedia page edits
 Home-page: http://github.com/eriknyquist/wikichangewatcher
 Author: Erik Nyquist
 Author-email: eknyquist@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -35,14 +35,23 @@
 
 ``WikiChangeWatcher`` is just a thin wrapper around an SSE client, pointed at the URL for
 the SSE stream for wikipedia edits, with some filtering features that allow you to watch for page edit
 events with specific attributes (e.g. `"anonymous" <https://en.wikipedia.org/wiki/Wikipedia:IP_edits_are_not_anonymous>`_
 edits with IP addresses in specific ranges, or edits made by a wikipedia user whose username matches
 a specific regular expression).
 
+Install
+=======
+
+Install using ``pip``.
+
+::
+
+    pip install wikichangewatcher
+
 Examples
 ========
 
 Some example scripts illustrating how to use ``WikiChangeWatcher`` are presented in
 the following sections.
 
 Monitoring "anonymous" page edits made from specific IP address ranges
@@ -52,69 +61,66 @@
 
 .. code:: python
 
     # Example script showing how to use WikiChangeWatcher to watch for "anonymous" edits to any
     # wikipedia page from specific IP address ranges
 
     import time
-    from wikichangewatcher import WikiChangeWatcher, IpV4Watcher
+    from wikichangewatcher import WikiChangeWatcher, IpV4Filter
 
     # Callback function to run whenever an event matching our IPv4 address pattern is seen
-    def on_match(json_data):
+    def match_handler(json_data):
         """
         json_data is a JSON-encoded event from the WikiMedia "recent changes" event stream,
         as described here: https://www.mediawiki.org/wiki/Manual:RCFeed
         """
         print("{user} edited {title_url}".format(**json_data))
 
-
-    # Watch for anonymous edits from some known IP addresses within the UK houses of parliament
-    # (taken from https://gist.github.com/Jonty/aabb42ab31d970dfb447, probably old/invalid by now)
-    wc = WikiChangeWatcher([IpV4Watcher(on_match, "192.60.38.225-230"),
-                            IpV4Watcher(on_match, "194.60.38.200-205"),
-                            IpV4Watcher(on_match, "194.60.38.215-219")])
+    # Watch for anonymous edits from some specific IP address ranges
+    wc = WikiChangeWatcher(IpV4Filter("192.60.38.225-230").on_match(match_handler),
+                           IpV4Filter("194.60.38.200-205").on_match(match_handler),
+                           IpV4Filter("194.60.38.215-219").on_match(match_handler))
 
     # You can also use the wildcard '*' character within IP addresses; the following line
     # sets up a watcher that triggers on any IP address (all anonymous edits)
-    # wc = WikiChangeWatcher([IpV4Watcher(on_match, "*.*.*.*")])
+    #wc = WikiChangeWatcher(IpV4Filter("*.*.*.*").on_match(match_handler))
 
     wc.run()
 
     # Watch for page edits forever until KeyboardInterrupt
     try:
         while True:
             time.sleep(0.1)
     except KeyboardInterrupt:
         wc.stop()
 
-
 Monitoring page edits made by usernames that match a regular expression
 -----------------------------------------------------------------------
 
 The following example code watches for edits made by signed-in users with usernames
 that contain one or more strings matching a regular expression.
 
 .. code:: python
 
     # Example script showing how to use WikiChangeWatcher to watch for NON-"anonymous" edits to any
-    # wikipedia page, by usernames that contain a string matching a regular expression
+    # wikipedia page, by usernames that contain a string matching a provided regular expression
 
     import time
-    from wikichangewatcher import WikiChangeWatcher, UsernameRegexSearchWatcher
+    from wikichangewatcher import WikiChangeWatcher, UsernameRegexSearchFilter
 
     # Callback function to run whenever an edit by a user with a username containing our regex is seen
-    def on_match(json_data):
+    def match_handler(json_data):
         """
         json_data is a JSON-encoded event from the WikiMedia "recent changes" event stream,
         as described here: https://www.mediawiki.org/wiki/Manual:RCFeed
         """
         print("{user} edited {title_url}".format(**json_data))
 
     # Watch for edits made by users with "bot" in their username
-    wc = WikiChangeWatcher([UsernameRegexSearchWatcher(on_match, r"[Bb]ot|BOT")])
+    wc = WikiChangeWatcher(UsernameRegexSearchFilter(r"[Bb]ot|BOT").on_match(match_handler))
 
     wc.run()
 
     # Watch for page edits forever until KeyboardInterrupt
     try:
         while True:
             time.sleep(0.1)
@@ -131,30 +137,119 @@
 .. code:: python
 
     # Example script showing how to use WikiChangeWatcher to filter page edit events
     # by a regular expression match in an arbitrary named field from the JSON event
     # provided by the SSE stream of wikipedia page edits
 
     import time
-    from wikichangewatcher import WikiChangeWatcher, FieldRegexSearchWatcher
+    from wikichangewatcher import WikiChangeWatcher, FieldRegexSearchFilter
 
     # Callback function to run whenever an edit is made to a page that has a regex match in the page URL
-    def on_match(json_data):
+    def match_handler(json_data):
         """
         json_data is a JSON-encoded event from the WikiMedia "recent changes" event stream,
         as described here: https://www.mediawiki.org/wiki/Manual:RCFeed
         """
         print("{user} edited {title_url}".format(**json_data))
 
     # Watch for edits made to any page that has the word "publish" in the page URL
     # ("title_url" field in the JSON object)
-    wc = WikiChangeWatcher([FieldRegexSearchWatcher(on_match, "title_url", r"[Pp]ublish")])
+    wc = WikiChangeWatcher(FieldRegexSearchFilter("title_url", r"[Pp]ublish").on_match(match_handler))
+
+    wc.run()
+
+    # Watch for page edits forever until KeyboardInterrupt
+    try:
+        while True:
+            time.sleep(0.1)
+    except KeyboardInterrupt:
+        wc.stop()
+
+
+Combining multiple filter classes with the ``FilterCollection`` class
+---------------------------------------------------------------------
+
+The following example watches for anonymous page edits to a specific page URL.
+
+.. code:: python
+
+    # Example script showing how to use WikiChangeWatcher to watch for "anonymous" edits to
+    # a specific wikipedia page
+
+    import time
+    from wikichangewatcher import WikiChangeWatcher, FilterCollection, IpV4Filter, PageUrlFilter
+
+    # Callback function to run whenever an event matching our filters is seen
+    def match_handler(json_data):
+        """
+        json_data is a JSON-encoded event from the WikiMedia "recent changes" event stream,
+        as described here: https://www.mediawiki.org/wiki/Manual:RCFeed
+        """
+        print("{user} edited {title_url}".format(**json_data))
+
+    # Default match type is is MatchType.ALL
+    filters = FilterCollection(
+        # Filter for any edits to a specific wikipedia page URL
+        PageUrlFilter("https://es.wikipedia.org/wiki/Reclus_(La_Rioja)"),
+
+        # Filter for any IP address (any anonymous edit)
+        IpV4Filter("*.*.*.*"),
+    ).on_match(match_handler)
+
+
+    wc = WikiChangeWatcher(filters)
 
     wc.run()
 
     # Watch for page edits forever until KeyboardInterrupt
     try:
         while True:
             time.sleep(0.1)
     except KeyboardInterrupt:
         wc.stop()
 
+Combining/nesting multiple ``FilterCollection`` classes
+-------------------------------------------------------
+
+The following example watches for page edits to several specific page URLs made by
+user with the word "bot" in their username.
+
+.. code:: python
+
+    # Example script showing how to use WikiChangeWatcher to watch for edit to specific
+    # wikipedia page URLs by users with the word "bot" in their name
+
+    import time
+    from wikichangewatcher import WikiChangeWatcher, FilterCollection, UsernameRegexSearchFilter, PageUrlFilter, MatchType
+
+    # Callback function to run whenever an event matching our filters is seen
+    def match_handler(json_data):
+        """
+        json_data is a JSON-encoded event from the WikiMedia "recent changes" event stream,
+        as described here: https://www.mediawiki.org/wiki/Manual:RCFeed
+        """
+        print("{user} edited {title_url}".format(**json_data))
+
+    # Make a filter collection that matches any one of several wikipedia pages
+    page_urls = FilterCollection(
+        # Filters for any edits to multiple specific wikipedia page URLs
+        PageUrlFilter("https://en.wikipedia.org/wiki/Python_(programming_language)"),
+        PageUrlFilter("https://en.wikipedia.org/wiki/CPython"),
+        PageUrlFilter("https://en.wikipedia.org/wiki/Server-sent_events"),
+    ).set_match_type(MatchType.ANY)
+
+    # Make a filter collection that matches one of the page URLs, *and* a specific username regex
+    main_filter = FilterCollection(
+        page_urls,
+        UsernameRegexSearchFilter(r"[Bb][Oo][Tt]")
+    ).set_match_type(MatchType.ALL).on_match(match_handler)
+
+    wc = WikiChangeWatcher(main_filter)
+
+    wc.run()
+
+    # Watch for page edits forever until KeyboardInterrupt
+    try:
+        while True:
+            time.sleep(0.1)
+    except KeyboardInterrupt:
+        wc.stop()
```

