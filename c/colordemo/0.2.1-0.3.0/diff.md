# Comparing `tmp/colordemo-0.2.1.tar.gz` & `tmp/colordemo-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colordemo-0.2.1.tar", last modified: Tue Jul 25 05:00:48 2023, max compression
+gzip compressed data, was "colordemo-0.3.0.tar", last modified: Sat Jul 29 23:30:29 2023, max compression
```

## Comparing `colordemo-0.2.1.tar` & `colordemo-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35147 2023-07-06 06:17:57.182174 colordemo-0.2.1/COPYING
--rw-r--r--   0        0        0     6358 2023-07-25 02:06:14.521093 colordemo-0.2.1/README.md
--rw-r--r--   0        0        0     1014 2023-07-23 04:19:34.075191 colordemo-0.2.1/colordemo/__init__.py
--rwxr-xr-x   0        0        0     5344 2023-07-23 04:19:34.075191 colordemo-0.2.1/colordemo/__main__.py
--rw-r--r--   0        0        0    13792 2023-07-23 04:24:27.225184 colordemo-0.2.1/colordemo/color_display.py
--rw-r--r--   0        0        0      820 2023-07-23 04:19:34.075191 colordemo-0.2.1/colordemo/colors.py
--rw-r--r--   0        0        0    14220 2023-07-25 02:09:12.741089 colordemo-0.2.1/colordemo/terminal_query.py
--rw-r--r--   0        0        0      839 2023-07-25 05:00:48.777500 colordemo-0.2.1/pyproject.toml
--rw-r--r--   0        0        0    47543 1970-01-01 00:00:00.000000 colordemo-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    35147 2023-07-06 06:17:57.182174 colordemo-0.3.0/COPYING
+-rw-r--r--   0        0        0     6358 2023-07-25 02:06:14.521093 colordemo-0.3.0/README.md
+-rw-r--r--   0        0        0     1014 2023-07-23 04:19:34.075191 colordemo-0.3.0/colordemo/__init__.py
+-rwxr-xr-x   0        0        0     5344 2023-07-23 04:19:34.075191 colordemo-0.3.0/colordemo/__main__.py
+-rw-r--r--   0        0        0    13792 2023-07-23 04:24:27.225184 colordemo-0.3.0/colordemo/color_display.py
+-rw-r--r--   0        0        0      820 2023-07-23 04:19:34.075191 colordemo-0.3.0/colordemo/colors.py
+-rw-r--r--   0        0        0    13770 2023-07-29 23:18:26.399751 colordemo-0.3.0/colordemo/terminal_query.py
+-rw-r--r--   0        0        0      839 2023-07-29 23:30:29.673066 colordemo-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    47543 1970-01-01 00:00:00.000000 colordemo-0.3.0/PKG-INFO
```

### Comparing `colordemo-0.2.1/COPYING` & `colordemo-0.3.0/COPYING`

 * *Files identical despite different names*

### Comparing `colordemo-0.2.1/README.md` & `colordemo-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `colordemo-0.2.1/colordemo/__init__.py` & `colordemo-0.3.0/colordemo/__init__.py`

 * *Files identical despite different names*

### Comparing `colordemo-0.2.1/colordemo/__main__.py` & `colordemo-0.3.0/colordemo/__main__.py`

 * *Files identical despite different names*

### Comparing `colordemo-0.2.1/colordemo/color_display.py` & `colordemo-0.3.0/colordemo/color_display.py`

 * *Files identical despite different names*

### Comparing `colordemo-0.2.1/colordemo/colors.py` & `colordemo-0.3.0/colordemo/colors.py`

 * *Files identical despite different names*

### Comparing `colordemo-0.2.1/colordemo/terminal_query.py` & `colordemo-0.3.0/colordemo/terminal_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -298,17 +298,17 @@
     str_guard = "(.*)\033\\[{ndec};{ndec}R".format(**vars())
     re_guard = re.compile(str_guard)
 
     # This is what we expect the terminal's response to a query for a
     # color to look like.  If we didn't care about urxvt, we could get
     # away with a simpler implementation here, since xterm and vte seem
     # to give pretty consistent and systematic responses.
-    str_rgb = ("\033\\]({ndec};)+rgba?:(({nhex})/)?" +
-               "({nhex})/({nhex})/({nhex})").format(**vars())
-
+    str_rgb = ("\033\\]({ndec};)+rgba?:" +
+               "({nhex})/({nhex})/({nhex})(/({nhex}))?"
+              ).format(**vars())
     re_rgb = re.compile(str_rgb)
 
     def rgb_query(self, q, timeout=-1):
         r"""
         Query a color-valued terminal parameter.
 
         See
@@ -356,31 +356,18 @@
 
         # (possibly overkill, since all terminals that reply seem to
         # give 4-digit RGB components, in which case `nd' is 4 and `u'
         # is 0xffff)
         nd = len(m.group(4))
         u = (1 << (nd << 2)) - 1
 
-        # An "rgba"-type reply (for urxvt) is apparently actually
-        #
-        #    rgba:{alpha}/{alpha * red}/{alpha * green}/{alpha * blue}
-        #
-        # We opt to extract the actual RGB values by eliminating alpha.
-        # (In other words, the alpha value is discarded completely in
-        # the reported color value.)
-
-        alpha = float(int(m.group(3), 16))/u if m.group(3) else 1.0
-
-        if alpha > 0:
-            (r, g, b) = (int(m.group(i), 16)/(alpha*u)
-                         for i in [4, 5, 6])
-
-            return RGBAColor(r, g, b, alpha)
-        else:
-            return RGBAColor(0.0, 0.0, 0.0, 0.0)
+        alpha = float(int(m.group(6), 16))/u if m.group(6) else 1.0
+        (r, g, b) = (int(m.group(i), 16)/u for i in [2, 3, 4])
+
+        return RGBAColor(r, g, b, alpha)
 
     # If a terminal sees an escape sequence it doesn't like, it will
     # simply ignore it. Also, it's hard to predict how long a terminal
     # will take to respond to a query it does like. However, some
     # escape sequences, like "\033[6n", will produce a predictable
     # response on *most* (but not all) terminals, and this fact can be
     # used to test for the absence of a response to a particular query
```

### Comparing `colordemo-0.2.1/pyproject.toml` & `colordemo-0.3.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "colordemo"
-version = "0.2.1"
+version = "0.3.0"
 description = "RGB queries on xterm-like terminals"
 authors = [
     { name = "Darsh Ranjan", email = "dranjan@berkeley.edu" },
 ]
 readme = "README.md"
 requires-python = ">=3.0"
 dependencies = []
```

### Comparing `colordemo-0.2.1/PKG-INFO` & `colordemo-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colordemo
-Version: 0.2.1
+Version: 0.3.0
 Summary: RGB queries on xterm-like terminals
 Author-Email: Darsh Ranjan <dranjan@berkeley.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

