# Comparing `tmp/tuidbtv-0.1.9.tar.gz` & `tmp/tuidbtv-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuidbtv-0.1.9.tar", max compression
+gzip compressed data, was "tuidbtv-0.2.0.tar", max compression
```

## Comparing `tuidbtv-0.1.9.tar` & `tuidbtv-0.2.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1084 2023-07-03 17:12:50.721482 tuidbtv-0.1.9/LICENSE
--rw-r--r--   0        0        0      917 2023-07-15 19:46:44.454160 tuidbtv-0.1.9/pyproject.toml
--rw-r--r--   0        0        0      586 2023-07-03 17:12:50.723479 tuidbtv-0.1.9/README.md
--rw-r--r--   0        0        0        0 2023-07-03 17:12:50.728476 tuidbtv-0.1.9/tuidbtv/__init__.py
--rw-r--r--   0        0        0     5299 2023-07-15 19:52:15.173681 tuidbtv-0.1.9/tuidbtv/__main__.py
--rw-r--r--   0        0        0        0 2023-07-03 17:12:50.732474 tuidbtv-0.1.9/tuidbtv/config/__init__.py
--rw-r--r--   0        0        0     2366 2023-07-03 17:12:50.731466 tuidbtv-0.1.9/tuidbtv/config/ConfigParser.py
--rw-r--r--   0        0        0        0 2023-07-03 17:12:50.742470 tuidbtv-0.1.9/tuidbtv/controllers/__init__.py
--rw-r--r--   0        0        0      811 2023-07-03 17:12:50.733489 tuidbtv-0.1.9/tuidbtv/controllers/ControllerFactory.py
--rw-r--r--   0        0        0      497 2023-07-15 19:44:48.564736 tuidbtv-0.1.9/tuidbtv/controllers/DBController.py
--rw-r--r--   0        0        0     2568 2023-07-15 19:44:48.566111 tuidbtv-0.1.9/tuidbtv/controllers/MySQLController.py
--rw-r--r--   0        0        0     3450 2023-07-15 19:44:48.567113 tuidbtv-0.1.9/tuidbtv/controllers/PostgresController.py
--rw-r--r--   0        0        0     1551 2023-07-15 19:44:48.568108 tuidbtv-0.1.9/tuidbtv/controllers/SQLLiteController.py
--rw-r--r--   0        0        0     2808 2023-07-03 17:12:50.744473 tuidbtv-0.1.9/tuidbtv/default.css
--rw-r--r--   0        0        0      299 2023-07-15 19:52:15.177577 tuidbtv-0.1.9/tuidbtv/enums_and_variables/__init__.py
--rw-r--r--   0        0        0      416 2023-07-15 19:44:48.569112 tuidbtv-0.1.9/tuidbtv/signals/__init__.py
--rw-r--r--   0        0        0        0 2023-07-03 17:12:50.747479 tuidbtv-0.1.9/tuidbtv/suggesters/__init__.py
--rw-r--r--   0        0        0      838 2023-07-03 17:12:50.746488 tuidbtv-0.1.9/tuidbtv/suggesters/SuggesterDict.py
--rw-r--r--   0        0        0        0 2023-07-03 17:12:50.757487 tuidbtv-0.1.9/tuidbtv/widgets/__init__.py
--rw-r--r--   0        0        0        0 2023-07-03 17:12:50.760465 tuidbtv-0.1.9/tuidbtv/widgets/forms/__init__.py
--rw-r--r--   0        0        0     1704 2023-07-03 17:12:50.759464 tuidbtv-0.1.9/tuidbtv/widgets/forms/ConnectionForms.py
--rw-r--r--   0        0        0     3382 2023-07-03 17:12:50.748488 tuidbtv-0.1.9/tuidbtv/widgets/NewConnection.py
--rw-r--r--   0        0        0      612 2023-07-03 17:12:50.750478 tuidbtv-0.1.9/tuidbtv/widgets/PopUpScreen.py
--rw-r--r--   0        0        0     1860 2023-07-15 19:44:48.569112 tuidbtv-0.1.9/tuidbtv/widgets/PreviewData.py
--rw-r--r--   0        0        0      668 2023-07-03 17:12:50.751469 tuidbtv-0.1.9/tuidbtv/widgets/QuitScreen.py
--rw-r--r--   0        0        0     5781 2023-07-07 21:46:01.271982 tuidbtv-0.1.9/tuidbtv/widgets/SelectConnection.py
--rw-r--r--   0        0        0     1902 2023-07-07 20:07:13.437708 tuidbtv-0.1.9/tuidbtv/widgets/SQLEditor.py
--rw-r--r--   0        0        0     1276 1970-01-01 00:00:00.000000 tuidbtv-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-07-03 17:12:50.721482 tuidbtv-0.2.0/LICENSE
+-rw-r--r--   0        0        0      917 2023-07-30 14:16:04.401989 tuidbtv-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      586 2023-07-03 17:12:50.723479 tuidbtv-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-03 17:12:50.728476 tuidbtv-0.2.0/tuidbtv/__init__.py
+-rw-r--r--   0        0        0     6129 2023-07-30 14:14:09.667894 tuidbtv-0.2.0/tuidbtv/__main__.py
+-rw-r--r--   0        0        0        0 2023-07-03 17:12:50.732474 tuidbtv-0.2.0/tuidbtv/config/__init__.py
+-rw-r--r--   0        0        0     2366 2023-07-03 17:12:50.731466 tuidbtv-0.2.0/tuidbtv/config/ConfigParser.py
+-rw-r--r--   0        0        0        0 2023-07-03 17:12:50.742470 tuidbtv-0.2.0/tuidbtv/controllers/__init__.py
+-rw-r--r--   0        0        0      811 2023-07-03 17:12:50.733489 tuidbtv-0.2.0/tuidbtv/controllers/ControllerFactory.py
+-rw-r--r--   0        0        0      497 2023-07-15 19:44:48.564736 tuidbtv-0.2.0/tuidbtv/controllers/DBController.py
+-rw-r--r--   0        0        0     2568 2023-07-15 19:44:48.566111 tuidbtv-0.2.0/tuidbtv/controllers/MySQLController.py
+-rw-r--r--   0        0        0     3450 2023-07-15 19:44:48.567113 tuidbtv-0.2.0/tuidbtv/controllers/PostgresController.py
+-rw-r--r--   0        0        0     1551 2023-07-15 19:44:48.568108 tuidbtv-0.2.0/tuidbtv/controllers/SQLLiteController.py
+-rw-r--r--   0        0        0     2808 2023-07-23 21:39:11.017145 tuidbtv-0.2.0/tuidbtv/default.css
+-rw-r--r--   0        0        0      299 2023-07-15 19:52:15.177577 tuidbtv-0.2.0/tuidbtv/enums_and_variables/__init__.py
+-rw-r--r--   0        0        0      416 2023-07-15 19:44:48.569112 tuidbtv-0.2.0/tuidbtv/signals/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 17:12:50.747479 tuidbtv-0.2.0/tuidbtv/suggesters/__init__.py
+-rw-r--r--   0        0        0      838 2023-07-03 17:12:50.746488 tuidbtv-0.2.0/tuidbtv/suggesters/SuggesterDict.py
+-rw-r--r--   0        0        0        0 2023-07-03 17:12:50.757487 tuidbtv-0.2.0/tuidbtv/widgets/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 17:12:50.760465 tuidbtv-0.2.0/tuidbtv/widgets/forms/__init__.py
+-rw-r--r--   0        0        0     1704 2023-07-03 17:12:50.759464 tuidbtv-0.2.0/tuidbtv/widgets/forms/ConnectionForms.py
+-rw-r--r--   0        0        0     3382 2023-07-03 17:12:50.748488 tuidbtv-0.2.0/tuidbtv/widgets/NewConnection.py
+-rw-r--r--   0        0        0      612 2023-07-03 17:12:50.750478 tuidbtv-0.2.0/tuidbtv/widgets/PopUpScreen.py
+-rw-r--r--   0        0        0     1860 2023-07-15 19:44:48.569112 tuidbtv-0.2.0/tuidbtv/widgets/PreviewData.py
+-rw-r--r--   0        0        0      668 2023-07-03 17:12:50.751469 tuidbtv-0.2.0/tuidbtv/widgets/QuitScreen.py
+-rw-r--r--   0        0        0     6185 2023-07-30 13:23:54.977819 tuidbtv-0.2.0/tuidbtv/widgets/SelectConnection.py
+-rw-r--r--   0        0        0     1902 2023-07-07 20:07:13.437708 tuidbtv-0.2.0/tuidbtv/widgets/SQLEditor.py
+-rw-r--r--   0        0        0     1276 1970-01-01 00:00:00.000000 tuidbtv-0.2.0/PKG-INFO
```

### Comparing `tuidbtv-0.1.9/LICENSE` & `tuidbtv-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.9/pyproject.toml` & `tuidbtv-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tuidbtv"
-version = "0.1.9"
+version = "0.2.0"
 description = "console database client"
 authors = ["lakdemon"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/lakdemon/TUIDBTV"
 classifiers = [
     "Environment :: Console",
```

### Comparing `tuidbtv-0.1.9/README.md` & `tuidbtv-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.9/tuidbtv/__main__.py` & `tuidbtv-0.2.0/tuidbtv/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,30 +40,31 @@
         self.tabs_count = 0
         self.suggestions = []
         self.dbController = None
 
     def compose(self) -> ComposeResult:
         yield Header(name="tuidbtv 0.1.9")
         with Horizontal():
-            yield Tree("schemas")
+            yield Tree(" ")
             with TabbedContent():
                 with TabPane("preview", id="preview_tab"):
                     yield PreviewData()
                 with TabPane("editor", id="editor_tab"):
                     yield SQLEditor()
                 with TabPane(" + ", id="add_new_tab_pane"):
                     yield Markdown()
         yield Footer()
 
     def openConnectionSelectScreen(self, _firstRun=False):
-        def select_connection(db_controller):
-            self.dbController = db_controller
+        def select_connection(result: SelectConnection.SelectConnectionResult):
+            self.dbController = result.get_controller()
             tree = self.query_one(Tree)
             tree.clear()
             tree.root.expand()
+            tree.root.label = result.get_conn_name()
             self.suggestions = []
             for schemaName in self.dbController.getSchemaNames():
                 schema = tree.root.add(schemaName[0])
                 self.suggestions.append(schemaName[0])
                 for tableName in self.dbController.getTableNamesBySchema(schemaName[0]):
                     schema.add_leaf(tableName[0])
                     self.suggestions.append(tableName[0])
@@ -75,23 +76,37 @@
         self.push_screen(SelectConnection(firstRun=_firstRun), select_connection)
 
     def on_mount(self) -> None:
         header = self.query_one(HeaderTitle)
         header.text = f"tuidbtv {APP_VERSION}"
         self.openConnectionSelectScreen(_firstRun=True)
 
-
     def action_toggle_dark(self) -> None:
         self.dark = not self.dark
 
     @on(Tree.NodeSelected)
-    def refresh_preview_data(self, event: Tree.NodeSelected):
-        preview = self.query(PreviewData).first()
+    async def refresh_preview_data(self, event: Tree.NodeSelected):
+        if not event.node.allow_expand:
+            await self.refresh_preview_tab_name(f"{event.node.label}")
+        preview = self.query_one(PreviewData)
         preview.refresh_table_data(event)
 
+    async def refresh_preview_tab_name(self, new_name: str):
+        preview_tab: TabPane = self.query("#preview_tab")\
+            .filter("TabPane")\
+            .first(expect_type=TabPane)
+        editor_tab: TabPane = self.query("#editor_tab")\
+            .filter("TabPane")\
+            .first(expect_type=TabPane)
+        new_preview_tab = TabPane(new_name, PreviewData(), id="preview_tab")
+        tab_pane = self.query_one(TabbedContent)
+        await tab_pane.remove_pane(preview_tab.id)
+        await tab_pane.add_pane(new_preview_tab, before=editor_tab)
+        tab_pane.active = new_preview_tab.id
+
     @on(PreviewNeed)
     def update_preview_data(self, event: PreviewNeed):
         preview = self.query_one(PreviewData)
         data = self.dbController.getTablePreview(event.schema,
                                                  event.table,
                                                  event.column,
                                                  event.desc)
```

### Comparing `tuidbtv-0.1.9/tuidbtv/config/ConfigParser.py` & `tuidbtv-0.2.0/tuidbtv/config/ConfigParser.py`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.9/tuidbtv/controllers/ControllerFactory.py` & `tuidbtv-0.2.0/tuidbtv/controllers/ControllerFactory.py`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.9/tuidbtv/controllers/MySQLController.py` & `tuidbtv-0.2.0/tuidbtv/controllers/MySQLController.py`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.9/tuidbtv/controllers/PostgresController.py` & `tuidbtv-0.2.0/tuidbtv/controllers/PostgresController.py`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.9/tuidbtv/controllers/SQLLiteController.py` & `tuidbtv-0.2.0/tuidbtv/controllers/SQLLiteController.py`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.9/tuidbtv/default.css` & `tuidbtv-0.2.0/tuidbtv/default.css`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.9/tuidbtv/suggesters/SuggesterDict.py` & `tuidbtv-0.2.0/tuidbtv/suggesters/SuggesterDict.py`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.9/tuidbtv/widgets/forms/ConnectionForms.py` & `tuidbtv-0.2.0/tuidbtv/widgets/forms/ConnectionForms.py`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.9/tuidbtv/widgets/NewConnection.py` & `tuidbtv-0.2.0/tuidbtv/widgets/NewConnection.py`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.9/tuidbtv/widgets/PopUpScreen.py` & `tuidbtv-0.2.0/tuidbtv/widgets/PopUpScreen.py`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.9/tuidbtv/widgets/PreviewData.py` & `tuidbtv-0.2.0/tuidbtv/widgets/PreviewData.py`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.9/tuidbtv/widgets/QuitScreen.py` & `tuidbtv-0.2.0/tuidbtv/widgets/QuitScreen.py`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.9/tuidbtv/widgets/SelectConnection.py` & `tuidbtv-0.2.0/tuidbtv/widgets/SelectConnection.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,14 +32,25 @@
         )
 
     def on_mount(self):
         optionList: OptionList = self.queryConnectionsList()
         for connection in ConfigParser.readConnectionList():
             optionList.add_option(connection["connectionName"])
 
+    class SelectConnectionResult:
+        def __init__(self, db_controller, connection_name):
+            self.controller = db_controller
+            self.connection_name = connection_name
+
+        def get_controller(self):
+            return self.controller
+
+        def get_conn_name(self):
+            return self.connection_name
+
     def on_button_pressed(self, event):
         def addNewConnection(connectionName):
             optionList: OptionList = self.queryConnectionsList()
             optionList.add_option(connectionName)
 
         match event.button.id:
             case "new_connection_button":
@@ -55,15 +66,15 @@
             case "connect_button":
                 selectedConnection: OptionList = self.queryConnectionsList()
                 selectedOption = selectedConnection.get_option_at_index(self.highlighted_index).prompt.__str__()
                 for connection in ConfigParser.readConnectionList():
                     if connection['connectionName'] == selectedOption:
                         try:
                             controller = ControllerFactory.getController(connection)
-                            self.dismiss(controller)
+                            self.dismiss(self.SelectConnectionResult(controller, connection['connectionName']))
                         except:
                             self.app.push_screen(PopUpScreen("Some errors happened while trying to connect :c"))
             case "cancel_select_connection_button":
                 if self.firstRun:
                     self.app.exit()
                 else:
                     self.app.pop_screen()
```

### Comparing `tuidbtv-0.1.9/tuidbtv/widgets/SQLEditor.py` & `tuidbtv-0.2.0/tuidbtv/widgets/SQLEditor.py`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.9/PKG-INFO` & `tuidbtv-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuidbtv
-Version: 0.1.9
+Version: 0.2.0
 Summary: console database client
 Home-page: https://github.com/lakdemon/TUIDBTV
 License: MIT
 Author: lakdemon
 Requires-Python: >=3.10,<4.0
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
```

