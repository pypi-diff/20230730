# Comparing `tmp/getmyancestors-1.0.3.tar.gz` & `tmp/getmyancestors-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getmyancestors-1.0.3.tar", last modified: Sat Dec  3 21:45:46 2022, max compression
+gzip compressed data, was "getmyancestors-1.0.4.tar", last modified: Sun Jul 30 16:24:00 2023, max compression
```

## Comparing `getmyancestors-1.0.3.tar` & `getmyancestors-1.0.4.tar`

### file list

```diff
@@ -1,16 +1,28 @@
--rw-r--r--   0        0        0     2630 2021-02-23 06:49:52.637182 getmyancestors-1.0.3/README.md
--rw-r--r--   0        0        0      162 2022-12-03 21:28:26.267884 getmyancestors-1.0.3/getmyancestors/__init__.py
--rw-r--r--   0        0        0       65 2021-02-23 06:49:52.637182 getmyancestors-1.0.3/getmyancestors/__main__.py
--rw-r--r--   0        0        0        0 2022-12-03 19:33:25.558816 getmyancestors-1.0.3/getmyancestors/classes/__init__.py
--rw-r--r--   0        0        0     1824 2022-12-03 19:33:25.558816 getmyancestors-1.0.3/getmyancestors/classes/constants.py
--rw-r--r--   0        0        0    12385 2022-12-03 19:42:10.291517 getmyancestors-1.0.3/getmyancestors/classes/gedcom.py
--rw-r--r--   0        0        0    23502 2022-12-03 19:42:10.291517 getmyancestors-1.0.3/getmyancestors/classes/gui.py
--rw-r--r--   0        0        0     7028 2022-12-03 19:57:51.408868 getmyancestors-1.0.3/getmyancestors/classes/session.py
--rw-r--r--   0        0        0     7103 2022-12-03 19:42:10.295517 getmyancestors-1.0.3/getmyancestors/classes/translation.py
--rw-r--r--   0        0        0    32658 2022-12-03 19:42:10.295517 getmyancestors-1.0.3/getmyancestors/classes/tree.py
--rw-r--r--   0        0        0      198 2021-02-23 06:49:52.637182 getmyancestors-1.0.3/getmyancestors/fstogedcom.png
--rw-r--r--   0        0        0      546 2022-12-03 19:33:25.562816 getmyancestors-1.0.3/getmyancestors/fstogedcom.py
--rw-r--r--   0        0        0     8689 2022-12-03 19:42:10.295517 getmyancestors-1.0.3/getmyancestors/getmyancestors.py
--rw-r--r--   0        0        0     4376 2022-12-03 19:33:25.562816 getmyancestors-1.0.3/getmyancestors/mergemyancestors.py
--rw-r--r--   0        0        0      996 2022-12-03 21:29:53.798808 getmyancestors-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     3270 1970-01-01 00:00:00.000000 getmyancestors-1.0.3/PKG-INFO
+drwxrwxr-x   0 benoit    (1000) benoit    (1000)        0 2023-07-30 16:24:00.357203 getmyancestors-1.0.4/
+-rw-rw-r--   0 benoit    (1000) benoit    (1000)      709 2023-01-21 19:10:46.000000 getmyancestors-1.0.4/LICENSE
+-rw-rw-r--   0 benoit    (1000) benoit    (1000)     3168 2023-07-30 16:24:00.357203 getmyancestors-1.0.4/PKG-INFO
+-rw-rw-r--   0 benoit    (1000) benoit    (1000)     2630 2023-01-21 19:10:46.000000 getmyancestors-1.0.4/README.md
+drwxrwxr-x   0 benoit    (1000) benoit    (1000)        0 2023-07-30 16:24:00.353203 getmyancestors-1.0.4/getmyancestors/
+-rw-rw-r--   0 benoit    (1000) benoit    (1000)      100 2023-07-30 16:22:33.000000 getmyancestors-1.0.4/getmyancestors/__init__.py
+-rw-rw-r--   0 benoit    (1000) benoit    (1000)       65 2023-01-21 19:10:46.000000 getmyancestors-1.0.4/getmyancestors/__main__.py
+drwxrwxr-x   0 benoit    (1000) benoit    (1000)        0 2023-07-30 16:24:00.357203 getmyancestors-1.0.4/getmyancestors/classes/
+-rw-rw-r--   0 benoit    (1000) benoit    (1000)        0 2023-01-21 19:10:46.000000 getmyancestors-1.0.4/getmyancestors/classes/__init__.py
+-rw-rw-r--   0 benoit    (1000) benoit    (1000)     1824 2023-01-21 19:10:46.000000 getmyancestors-1.0.4/getmyancestors/classes/constants.py
+-rw-rw-r--   0 benoit    (1000) benoit    (1000)    12385 2023-01-21 19:10:46.000000 getmyancestors-1.0.4/getmyancestors/classes/gedcom.py
+-rw-rw-r--   0 benoit    (1000) benoit    (1000)    24133 2023-07-30 16:14:16.000000 getmyancestors-1.0.4/getmyancestors/classes/gui.py
+-rw-rw-r--   0 benoit    (1000) benoit    (1000)     7028 2023-01-21 19:10:46.000000 getmyancestors-1.0.4/getmyancestors/classes/session.py
+-rw-rw-r--   0 benoit    (1000) benoit    (1000)     7326 2023-07-30 16:14:16.000000 getmyancestors-1.0.4/getmyancestors/classes/translation.py
+-rw-rw-r--   0 benoit    (1000) benoit    (1000)    32658 2023-01-21 19:10:46.000000 getmyancestors-1.0.4/getmyancestors/classes/tree.py
+-rw-rw-r--   0 benoit    (1000) benoit    (1000)      198 2023-01-21 19:10:46.000000 getmyancestors-1.0.4/getmyancestors/fstogedcom.png
+-rw-rw-r--   0 benoit    (1000) benoit    (1000)      546 2023-01-21 19:10:46.000000 getmyancestors-1.0.4/getmyancestors/fstogedcom.py
+-rw-rw-r--   0 benoit    (1000) benoit    (1000)     8689 2023-01-21 19:10:46.000000 getmyancestors-1.0.4/getmyancestors/getmyancestors.py
+-rw-rw-r--   0 benoit    (1000) benoit    (1000)     4376 2023-01-21 19:10:46.000000 getmyancestors-1.0.4/getmyancestors/mergemyancestors.py
+drwxrwxr-x   0 benoit    (1000) benoit    (1000)        0 2023-07-30 16:24:00.353203 getmyancestors-1.0.4/getmyancestors.egg-info/
+-rw-rw-r--   0 benoit    (1000) benoit    (1000)     3168 2023-07-30 16:24:00.000000 getmyancestors-1.0.4/getmyancestors.egg-info/PKG-INFO
+-rw-rw-r--   0 benoit    (1000) benoit    (1000)      680 2023-07-30 16:24:00.000000 getmyancestors-1.0.4/getmyancestors.egg-info/SOURCES.txt
+-rw-rw-r--   0 benoit    (1000) benoit    (1000)        1 2023-07-30 16:24:00.000000 getmyancestors-1.0.4/getmyancestors.egg-info/dependency_links.txt
+-rw-rw-r--   0 benoit    (1000) benoit    (1000)      170 2023-07-30 16:24:00.000000 getmyancestors-1.0.4/getmyancestors.egg-info/entry_points.txt
+-rw-rw-r--   0 benoit    (1000) benoit    (1000)       73 2023-07-30 16:24:00.000000 getmyancestors-1.0.4/getmyancestors.egg-info/requires.txt
+-rw-rw-r--   0 benoit    (1000) benoit    (1000)       15 2023-07-30 16:24:00.000000 getmyancestors-1.0.4/getmyancestors.egg-info/top_level.txt
+-rw-rw-r--   0 benoit    (1000) benoit    (1000)     1010 2023-01-21 19:10:46.000000 getmyancestors-1.0.4/pyproject.toml
+-rw-rw-r--   0 benoit    (1000) benoit    (1000)       38 2023-07-30 16:24:00.357203 getmyancestors-1.0.4/setup.cfg
```

### Comparing `getmyancestors-1.0.3/README.md` & `getmyancestors-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `getmyancestors-1.0.3/getmyancestors/classes/constants.py` & `getmyancestors-1.0.4/getmyancestors/classes/constants.py`

 * *Files identical despite different names*

### Comparing `getmyancestors-1.0.3/getmyancestors/classes/gedcom.py` & `getmyancestors-1.0.4/getmyancestors/classes/gedcom.py`

 * *Files identical despite different names*

### Comparing `getmyancestors-1.0.3/getmyancestors/classes/gui.py` & `getmyancestors-1.0.4/getmyancestors/classes/gui.py`

 * *Files 4% similar despite different names*

```diff
@@ -244,24 +244,31 @@
     """Sign In widget"""
 
     def __init__(self, master, **kwargs):
         super().__init__(master, **kwargs)
         self.username = StringVar()
         self.username.set(cache.get("username") or "")
         self.password = StringVar()
+        self.password.set(cache.get("password") or "")
         label_username = Label(self, text=_("Username:"))
         entry_username = EntryWithMenu(self, textvariable=self.username, width=30)
         label_password = Label(self, text=_("Password:"))
         entry_password = EntryWithMenu(
             self, show="●", textvariable=self.password, width=30
         )
+
+        self.save_password = IntVar()
+        self.save_password.set(cache.get("save_password") or 0)
+        check_save_password = Checkbutton(self, text=_("Save Password"), variable=self.save_password, onvalue=1, offvalue=0)
+
         label_username.grid(row=0, column=0, pady=15, padx=(0, 5))
         entry_username.grid(row=0, column=1)
         label_password.grid(row=1, column=0, padx=(0, 5))
         entry_password.grid(row=1, column=1)
+        check_save_password.grid(row=2, column=1, pady=5)
         entry_username.focus_set()
         entry_username.bind("<Key>", self.enter)
         entry_password.bind("<Key>", self.enter)
 
     def enter(self, evt):
         """enter event"""
         if evt.keysym in {"Return", "KP_Enter"}:
@@ -489,14 +496,25 @@
         self.tree = Tree(self.fs)
         _ = self.fs._
         self.title.config(text=_("Options"))
         cache.delete("lang")
         cache.add("lang", self.fs.lang)
         cache.delete("username")
         cache.add("username", username)
+
+        cache.delete("password")
+        # cache password  only when checked
+
+        save_pass = self.sign_in.save_password.get()
+        if save_pass == 1:
+            cache.add("password", password)
+
+        cache.delete("save_password")
+        cache.add("save_password", save_pass)
+
         url = "/service/tree/tree-data/reservations/person/%s/ordinances" % self.fs.fid
         lds_account = self.fs.get_url(url, {}).get("status") == "OK"
         self.options = Options(self.form, lds_account)
         self.info("")
         self.sign_in.destroy()
         self.options.pack()
         self.master.change_lang()
```

### Comparing `getmyancestors-1.0.3/getmyancestors/classes/session.py` & `getmyancestors-1.0.4/getmyancestors/classes/session.py`

 * *Files identical despite different names*

### Comparing `getmyancestors-1.0.3/getmyancestors/classes/translation.py` & `getmyancestors-1.0.4/getmyancestors/classes/translation.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,16 +113,26 @@
     "Downloaded %s individuals, %s families, %s sources and %s notes in %s seconds with %s HTTP requests.": {
         "fr": "%s personnes, %s familles, %s sources et %s notes téléchargés en %s secondes avec %s requêtes HTTP."
     },
     "Download ": {"fr": "Téléchargement de la "},
     "Copy": {"fr": "Copier"},
     "Cut": {"fr": "Couper"},
     "Paste": {"fr": "Coller"},
-    "Username:": {"fr": "Nom d'utilisateur :"},
-    "Password:": {"fr": "Mot de passe :"},
+    "Username:": {
+            "fr": "Nom d'utilisateur :",
+            "de": "Benutzername:",
+    },
+    "Password:": {
+            "fr": "Mot de passe :",
+            "de": "Passwort:",
+    },
+    "Save Password": {
+            "fr": "Enregistrer le mot de passe",
+            "de": "Passwort speichern",
+    },
     "ID already exist": {"fr": "Cet identifiant existe déjà"},
     "Invalid FamilySearch ID: ": {"fr": "Identifiant FamilySearch invalide : "},
     "Individual not found": {"fr": "Personne non trouvée"},
     "Remove": {"fr": "Supprimer"},
     "Number of generations to ascend": {"fr": "Nombre de générations d'ancêtres"},
     "Number of generations to descend": {"fr": "Nombre de générations de descendants"},
     "Add a FamilySearch ID": {"fr": "Ajouter un identifiant FamilySearch"},
```

### Comparing `getmyancestors-1.0.3/getmyancestors/classes/tree.py` & `getmyancestors-1.0.4/getmyancestors/classes/tree.py`

 * *Files identical despite different names*

### Comparing `getmyancestors-1.0.3/getmyancestors/fstogedcom.py` & `getmyancestors-1.0.4/getmyancestors/fstogedcom.py`

 * *Files identical despite different names*

### Comparing `getmyancestors-1.0.3/getmyancestors/getmyancestors.py` & `getmyancestors-1.0.4/getmyancestors/getmyancestors.py`

 * *Files identical despite different names*

### Comparing `getmyancestors-1.0.3/getmyancestors/mergemyancestors.py` & `getmyancestors-1.0.4/getmyancestors/mergemyancestors.py`

 * *Files identical despite different names*

### Comparing `getmyancestors-1.0.3/pyproject.toml` & `getmyancestors-1.0.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 [project]
 name = "getmyancestors"
-version = "1.0.3"
 description = "Retrieve GEDCOM data from FamilySearch Tree"
-readme = "README.md"
 requires-python = ">=3.7"
 license = {text = "GNU"}
 keywords = [
   "getmyancestors",
   "familysearch",
   "fstogedcom",
   "gedcom",
@@ -19,18 +17,19 @@
 ]
 dependencies = [
     "babelfish==0.6.0",
     "diskcache==5.2.1",
     "requests==2.25.1",
     "fake-useragent==1.1.0",
 ]
+dynamic = ["version", "readme"]
 
-[build-system]
-requires = ["flit_core>=3.2,<4"]
-build-backend = "flit_core.buildapi"
+[tool.setuptools.dynamic]
+version = {attr = "getmyancestors.__version__"}
+readme = {file = ["README.md"]}
 
 [project.urls]
 HomePage = "https://github.com/Linekio/getmyancestors"
 
 [tool.setuptools.package-data]
 getmyancestors = ["fstogedcom.png"]
```

### Comparing `getmyancestors-1.0.3/PKG-INFO` & `getmyancestors-1.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 2.1
 Name: getmyancestors
-Version: 1.0.3
+Version: 1.0.4
 Summary: Retrieve GEDCOM data from FamilySearch Tree
+License: GNU
+Project-URL: HomePage, https://github.com/Linekio/getmyancestors
 Keywords: getmyancestors,familysearch,fstogedcom,gedcom
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Dist: babelfish==0.6.0
-Requires-Dist: diskcache==5.2.1
-Requires-Dist: requests==2.25.1
-Requires-Dist: fake-useragent==1.1.0
-Project-URL: HomePage, https://github.com/Linekio/getmyancestors
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+License-File: LICENSE
 
 getmyancestors
 ==============
 
 _getmyancestors_ is a python3 package that downloads family trees in GEDCOM format from FamilySearch.
 
 This program is now in production phase, but bugs might still be present. Features will be added on request. It is provided as is.
@@ -105,8 +103,7 @@
 
 Donation
 ========
 
 If this project help you, you can give me a tip :)
 
 [![paypal](https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=98X3CY93XTAYJ)
-
```

