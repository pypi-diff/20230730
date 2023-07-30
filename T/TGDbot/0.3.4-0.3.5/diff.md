# Comparing `tmp/TGDbot-0.3.4-py3-none-any.whl.zip` & `tmp/TGDbot-0.3.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 19056 bytes, number of entries: 9
--rwxrwxrwx  2.0 unx    44851 b- defN 23-Apr-14 19:51 TGDbot/__init__.py
+Zip file size: 19012 bytes, number of entries: 9
+-rwxrwxrwx  2.0 unx    44799 b- defN 23-Jul-30 14:35 TGDbot/__init__.py
 -rwxrwxrwx  2.0 unx    44441 b- defN 23-Apr-12 06:25 schbot/__init__.py
--rwxrwxrwx  2.0 unx       10 b- defN 23-Apr-14 20:19 TGDbot-0.3.4.dist-info/DESCRIPTION.rst
--rwxrwxrwx  2.0 unx       47 b- defN 23-Apr-14 20:19 TGDbot-0.3.4.dist-info/dependency_links.txt
--rwxrwxrwx  2.0 unx      619 b- defN 23-Apr-14 20:19 TGDbot-0.3.4.dist-info/metadata.json
--rwxrwxrwx  2.0 unx        7 b- defN 23-Apr-14 20:19 TGDbot-0.3.4.dist-info/top_level.txt
--rwxrwxrwx  2.0 unx       92 b- defN 23-Apr-14 20:19 TGDbot-0.3.4.dist-info/WHEEL
--rwxrwxrwx  2.0 unx      531 b- defN 23-Apr-14 20:19 TGDbot-0.3.4.dist-info/METADATA
--rwxrwxrwx  2.0 unx      736 b- defN 23-Apr-14 20:19 TGDbot-0.3.4.dist-info/RECORD
-9 files, 91334 bytes uncompressed, 17796 bytes compressed:  80.5%
+-rwxrwxrwx  2.0 unx       10 b- defN 23-Jul-30 14:35 TGDbot-0.3.5.dist-info/DESCRIPTION.rst
+-rwxrwxrwx  2.0 unx       47 b- defN 23-Jul-30 14:35 TGDbot-0.3.5.dist-info/dependency_links.txt
+-rwxrwxrwx  2.0 unx      619 b- defN 23-Jul-30 14:35 TGDbot-0.3.5.dist-info/metadata.json
+-rwxrwxrwx  2.0 unx        7 b- defN 23-Jul-30 14:35 TGDbot-0.3.5.dist-info/top_level.txt
+-rwxrwxrwx  2.0 unx       92 b- defN 23-Jul-30 14:35 TGDbot-0.3.5.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx      531 b- defN 23-Jul-30 14:35 TGDbot-0.3.5.dist-info/METADATA
+-rwxrwxrwx  2.0 unx      736 b- defN 23-Jul-30 14:35 TGDbot-0.3.5.dist-info/RECORD
+9 files, 91282 bytes uncompressed, 17752 bytes compressed:  80.6%
```

## zipnote {}

```diff
@@ -1,28 +1,28 @@
 Filename: TGDbot/__init__.py
 Comment: 
 
 Filename: schbot/__init__.py
 Comment: 
 
-Filename: TGDbot-0.3.4.dist-info/DESCRIPTION.rst
+Filename: TGDbot-0.3.5.dist-info/DESCRIPTION.rst
 Comment: 
 
-Filename: TGDbot-0.3.4.dist-info/dependency_links.txt
+Filename: TGDbot-0.3.5.dist-info/dependency_links.txt
 Comment: 
 
-Filename: TGDbot-0.3.4.dist-info/metadata.json
+Filename: TGDbot-0.3.5.dist-info/metadata.json
 Comment: 
 
-Filename: TGDbot-0.3.4.dist-info/top_level.txt
+Filename: TGDbot-0.3.5.dist-info/top_level.txt
 Comment: 
 
-Filename: TGDbot-0.3.4.dist-info/WHEEL
+Filename: TGDbot-0.3.5.dist-info/WHEEL
 Comment: 
 
-Filename: TGDbot-0.3.4.dist-info/METADATA
+Filename: TGDbot-0.3.5.dist-info/METADATA
 Comment: 
 
-Filename: TGDbot-0.3.4.dist-info/RECORD
+Filename: TGDbot-0.3.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## TGDbot/__init__.py

```diff
@@ -178,15 +178,15 @@
         self.default_level = 68
         self.default_bp_tier = 68
         self.invitecc = ''
         self.invite_message = "JOIN ME \n USE CODE OIM"
 
         self.sanic_app = sanic_app
         self.server = server
-        self.welcome_message =  " Use Code OIM in the Item Shop (#EpicPartner)\n Create own your bot : https://schbots.com \n free battle pass code here : 8455-3482-1956 \n"
+        self.welcome_message =  " Use Code OIM in the Item Shop (#EpicPartner)\n join my discord : discord.gg/lobbybot\n"
 
     async def set_and_update_party_prop(self, schema_key: str, new_value: Any) -> None:
         prop = {schema_key: self.party.me.meta.set_prop(schema_key, new_value)}
 
         await self.party.patch(updated=prop)
 
     async def add_list(self) -> None:
```

## Comparing `TGDbot-0.3.4.dist-info/metadata.json` & `TGDbot-0.3.5.dist-info/metadata.json`

 * *Files 25% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9444444444444444%*

 * *Differences: {"'version'": "'0.3.5'"}*

```diff
@@ -34,9 +34,9 @@
                 "crayons",
                 "fortnitepy (==3.6.7)",
                 "sanic (==21.6.2)"
             ]
         }
     ],
     "summary": "Lobby bot.",
-    "version": "0.3.4"
+    "version": "0.3.5"
 }
```

## Comparing `TGDbot-0.3.4.dist-info/METADATA` & `TGDbot-0.3.5.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.0
 Name: TGDbot
-Version: 0.3.4
+Version: 0.3.5
 Summary: Lobby bot.
 Home-page: https://www.youtube.com/
 Author: Aeroz
 Author-email: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `TGDbot-0.3.4.dist-info/RECORD` & `TGDbot-0.3.5.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-TGDbot/__init__.py,sha256=iyhFNn2uRl01EwK7I6M-lpyVH37TXYBJ8NeeL45Pjkg,44851
-TGDbot-0.3.4.dist-info/DESCRIPTION.rst,sha256=OCTuuN6LcWulhHS3d5rfjdsQtW22n7HENFRh6jC6ego,10
-TGDbot-0.3.4.dist-info/METADATA,sha256=0KIlH80PjhEGraRQ9s03j-o9c7mDnE9A9i7FyK_pAK0,531
-TGDbot-0.3.4.dist-info/RECORD,,
-TGDbot-0.3.4.dist-info/WHEEL,sha256=8Lm45v9gcYRm70DrgFGVe4WsUtUMi1_0Tso1hqPGMjA,92
-TGDbot-0.3.4.dist-info/dependency_links.txt,sha256=qghdsulj9f7KujhhUbgS6dtbeW8ot_ySInuAyvtQmzg,47
-TGDbot-0.3.4.dist-info/metadata.json,sha256=oP52vsyY91AMpZTbV_c4bicyOriBvgQzczGoO-hCrc4,619
-TGDbot-0.3.4.dist-info/top_level.txt,sha256=NM8_-Mr8DPlOkU_x-Chrck1522cPPh-rqp6YvASDJdM,7
+TGDbot/__init__.py,sha256=fJFvTsnnE_Rbza13GpSc51_nGXjKu3vpEZYp33pWU6M,44799
+TGDbot-0.3.5.dist-info/DESCRIPTION.rst,sha256=OCTuuN6LcWulhHS3d5rfjdsQtW22n7HENFRh6jC6ego,10
+TGDbot-0.3.5.dist-info/METADATA,sha256=lyWDbNROjehno4wGcl1l3tgeVCP608uvJqDM3ffh_xI,531
+TGDbot-0.3.5.dist-info/RECORD,,
+TGDbot-0.3.5.dist-info/WHEEL,sha256=8Lm45v9gcYRm70DrgFGVe4WsUtUMi1_0Tso1hqPGMjA,92
+TGDbot-0.3.5.dist-info/dependency_links.txt,sha256=qghdsulj9f7KujhhUbgS6dtbeW8ot_ySInuAyvtQmzg,47
+TGDbot-0.3.5.dist-info/metadata.json,sha256=4F9UUvHfUFzvsFRTlgW2_YBXBne5ogJ8QwgzfSmOcsE,619
+TGDbot-0.3.5.dist-info/top_level.txt,sha256=NM8_-Mr8DPlOkU_x-Chrck1522cPPh-rqp6YvASDJdM,7
 schbot/__init__.py,sha256=ApMuqWSZv7bmzEwuuc7vtYnI_WrlIYfzYRHYaA9vhEo,44441
```

