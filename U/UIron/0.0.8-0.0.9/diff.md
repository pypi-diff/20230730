# Comparing `tmp/UIron-0.0.8.tar.gz` & `tmp/UIron-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UIron-0.0.8.tar", last modified: Sat Jul 29 04:44:34 2023, max compression
+gzip compressed data, was "UIron-0.0.9.tar", last modified: Sat Jul 29 05:40:55 2023, max compression
```

## Comparing `UIron-0.0.8.tar` & `UIron-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 04:44:34.846202 UIron-0.0.8/
--rw-rw-rw-   0        0        0     1087 2023-07-27 19:37:41.000000 UIron-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      460 2023-07-29 04:44:34.844202 UIron-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-07-27 02:09:14.000000 UIron-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-29 04:44:34.800320 UIron-0.0.8/UIron/
--rw-rw-rw-   0        0        0        0 2023-07-27 02:09:14.000000 UIron-0.0.8/UIron/__init__.py
--rw-rw-rw-   0        0        0        0 2023-07-27 02:09:14.000000 UIron-0.0.8/UIron/__main__.py
--rw-rw-rw-   0        0        0     1600 2023-07-28 05:16:34.000000 UIron-0.0.8/UIron/config.py
-drwxrwxrwx   0        0        0        0 2023-07-29 04:44:34.838204 UIron-0.0.8/UIron/data/
--rw-rw-rw-   0        0        0       10 2023-07-27 16:47:20.000000 UIron-0.0.8/UIron/data/config.json
--rw-rw-rw-   0        0        0        2 2023-07-28 05:20:04.000000 UIron-0.0.8/UIron/data/new.json
--rw-rw-rw-   0        0        0      121 2023-07-28 05:22:37.000000 UIron-0.0.8/UIron/regex.py
--rw-rw-rw-   0        0        0     9537 2023-07-29 04:44:01.000000 UIron-0.0.8/UIron/ui.py
--rw-rw-rw-   0        0        0     2234 2023-07-29 03:02:18.000000 UIron-0.0.8/UIron/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-29 04:44:34.831203 UIron-0.0.8/UIron.egg-info/
--rw-rw-rw-   0        0        0      460 2023-07-29 04:44:34.000000 UIron-0.0.8/UIron.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2023-07-29 04:44:34.000000 UIron-0.0.8/UIron.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 04:44:34.000000 UIron-0.0.8/UIron.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-29 04:44:34.000000 UIron-0.0.8/UIron.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-29 04:44:34.000000 UIron-0.0.8/UIron.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-29 04:44:34.846202 UIron-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      789 2023-07-29 04:44:33.000000 UIron-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 05:40:55.839515 UIron-0.0.9/
+-rw-rw-rw-   0        0        0     1087 2023-07-27 19:37:41.000000 UIron-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      460 2023-07-29 05:40:55.838516 UIron-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-07-27 02:09:14.000000 UIron-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-29 05:40:55.785997 UIron-0.0.9/UIron/
+-rw-rw-rw-   0        0        0        0 2023-07-27 02:09:14.000000 UIron-0.0.9/UIron/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-07-27 02:09:14.000000 UIron-0.0.9/UIron/__main__.py
+-rw-rw-rw-   0        0        0     1600 2023-07-28 05:16:34.000000 UIron-0.0.9/UIron/config.py
+drwxrwxrwx   0        0        0        0 2023-07-29 05:40:55.835515 UIron-0.0.9/UIron/data/
+-rw-rw-rw-   0        0        0       10 2023-07-27 16:47:20.000000 UIron-0.0.9/UIron/data/config.json
+-rw-rw-rw-   0        0        0        2 2023-07-28 05:20:04.000000 UIron-0.0.9/UIron/data/new.json
+-rw-rw-rw-   0        0        0      121 2023-07-28 05:22:37.000000 UIron-0.0.9/UIron/regex.py
+-rw-rw-rw-   0        0        0     9328 2023-07-29 05:40:14.000000 UIron-0.0.9/UIron/ui.py
+-rw-rw-rw-   0        0        0     2234 2023-07-29 03:02:18.000000 UIron-0.0.9/UIron/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-29 05:40:55.828519 UIron-0.0.9/UIron.egg-info/
+-rw-rw-rw-   0        0        0      460 2023-07-29 05:40:55.000000 UIron-0.0.9/UIron.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2023-07-29 05:40:55.000000 UIron-0.0.9/UIron.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 05:40:55.000000 UIron-0.0.9/UIron.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-29 05:40:55.000000 UIron-0.0.9/UIron.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-29 05:40:55.000000 UIron-0.0.9/UIron.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-29 05:40:55.839515 UIron-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      789 2023-07-29 05:40:54.000000 UIron-0.0.9/setup.py
```

### Comparing `UIron-0.0.8/LICENSE` & `UIron-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `UIron-0.0.8/UIron/config.py` & `UIron-0.0.9/UIron/config.py`

 * *Files identical despite different names*

### Comparing `UIron-0.0.8/UIron/ui.py` & `UIron-0.0.9/UIron/ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,54 +137,49 @@
 
     def get(self) -> str:
         return self.entry.get()
 
 
 class RegexEntry(ttk.Entry):
     def __init__(
-            self, master: ttk.Frame|ttk.Window, regex: str='*', width: int=20,
+            self, master: ttk.Frame|ttk.Window, regex: str='*',
             invalid_message: str='Invalid input...', show_message: bool=True, **kwargs
     ):
         super().__init__(master, **kwargs)
 
         self.regex = regex
         self.show_message = show_message
         self.invalid_message = invalid_message
 
-        self.entry = ttk.Entry(self, width=width)
-        self.entry.pack(fill='x')
         self.message = ttk.StringVar()
         self.label = ttk.Label(self, textvariable=self.message, anchor='center', bootstyle='danger')
 
-        self.entry.bind('<FocusIn>', self.check_regex)
-        self.entry.bind('<KeyRelease>', self.check_regex)
-        self.entry.bind('<FocusOut>', self.reset)
+        self.bind('<FocusIn>', self.check_regex)
+        self.bind('<KeyRelease>', self.check_regex)
+        self.bind('<FocusOut>', self.reset)
     
     def ok(self) -> bool:
         self.check_regex()
         return self._ok
 
     def reset(self, *_) -> None:
         self.label.pack_forget()
         self.message.set(value='')
-        self.entry.config(bootstyle='default')
+        self.config(bootstyle='default')
     
     def check_regex(self, *_) -> None:
         self._ok = re.match(self.regex, self.get())
         if self._ok: return self.reset()
         self.message.set(value=self.invalid_message)
-        self.entry.config(bootstyle='danger')
+        self.config(bootstyle='danger')
         if self.show_message: self.label.pack(fill='x')
-    
-    def get(self) -> str:
-        return self.entry.get()
 
     def set(self, value: str) -> None:
-        self.entry.delete(0, 'end')
-        self.entry.insert(0, value)
+        self.delete(0, 'end')
+        self.insert(0, value)
 
 
 class Image(ttk.Label):
     def __init__(self, master: ttk.Frame|ttk.Window, path: str='', **kwargs):
         super().__init__(master, **kwargs)
         if path: self.config(image=path)
```

### Comparing `UIron-0.0.8/UIron/utils.py` & `UIron-0.0.9/UIron/utils.py`

 * *Files identical despite different names*

### Comparing `UIron-0.0.8/setup.py` & `UIron-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from setuptools import setup, find_packages
-VERSION = "0.0.8"
+VERSION = "0.0.9"
 DESCRIPTION = "Package for User Interface"
 LONG_DESCRIPTION = "Package for User Interface"
 
 setup(
     name="UIron",
     version=VERSION,
     author="Armando Chaparro",
```

