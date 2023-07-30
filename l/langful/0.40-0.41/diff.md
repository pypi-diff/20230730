# Comparing `tmp/langful-0.40-py3-none-any.whl.zip` & `tmp/langful-0.41-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,10 @@
-Zip file size: 5289 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat      166 b- defN 23-Jul-06 06:25 langful/__init__.py
--rw-rw-rw-  2.0 fat     8206 b- defN 23-Jul-29 14:22 langful/lang.py
--rw-rw-rw-  2.0 fat     1066 b- defN 23-Jul-29 16:22 langful-0.40.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2984 b- defN 23-Jul-29 16:22 langful-0.40.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-29 16:22 langful-0.40.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Jul-29 16:22 langful-0.40.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      527 b- defN 23-Jul-29 16:22 langful-0.40.dist-info/RECORD
-7 files, 13049 bytes uncompressed, 4359 bytes compressed:  66.6%
+Zip file size: 5653 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat      166 b- defN 23-Jul-30 07:47 langful/__init__.py
+-rw-rw-rw-  2.0 fat      382 b- defN 23-Jul-30 12:15 langful/errors.py
+-rw-rw-rw-  2.0 fat     8308 b- defN 23-Jul-30 12:55 langful/lang.py
+-rw-rw-rw-  2.0 fat     1066 b- defN 23-Jul-30 12:57 langful-0.41.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2984 b- defN 23-Jul-30 12:57 langful-0.41.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-30 12:57 langful-0.41.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jul-30 12:57 langful-0.41.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      600 b- defN 23-Jul-30 12:57 langful-0.41.dist-info/RECORD
+8 files, 13606 bytes uncompressed, 4613 bytes compressed:  66.1%
```

## zipnote {}

```diff
@@ -1,22 +1,25 @@
 Filename: langful/__init__.py
 Comment: 
 
+Filename: langful/errors.py
+Comment: 
+
 Filename: langful/lang.py
 Comment: 
 
-Filename: langful-0.40.dist-info/LICENSE
+Filename: langful-0.41.dist-info/LICENSE
 Comment: 
 
-Filename: langful-0.40.dist-info/METADATA
+Filename: langful-0.41.dist-info/METADATA
 Comment: 
 
-Filename: langful-0.40.dist-info/WHEEL
+Filename: langful-0.41.dist-info/WHEEL
 Comment: 
 
-Filename: langful-0.40.dist-info/top_level.txt
+Filename: langful-0.41.dist-info/top_level.txt
 Comment: 
 
-Filename: langful-0.40.dist-info/RECORD
+Filename: langful-0.41.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## langful/lang.py

```diff
@@ -1,28 +1,31 @@
 """
 # lang
 """
 
+from . import errors
+
 import json
 import os
 
-__all__ = [ "to_json" , "to_lang" , "getdefaultlocale" , "lang" ]
+__all__ = [ "__version__" , "to_json" , "to_lang" , "getdefaultlocale" , "lang" ]
+__version__ = "0.41"
 
 def to_json( text : str ) -> dict[ str , str ] :
     from re import split
     ret = {}
     for line in text.split( "\n" ) :
         try :
-            ret.update( dict( [ split( "\s=\s" , line.split( "#" )[ 0 ] , 1 ) ] ) )
+            ret.update( dict( [ split( "\\s=\\s" , line.split( "#" )[ 0 ] , 1 ) ] ) )
         except ValueError :
             continue
     return ret
 
-def to_lang( text : dict ) -> str :
-    return "\n".join( [ ' = '.join( item ) for item in list( text.items() ) ] )
+def to_lang( data : dict ) -> str :
+    return "\n".join( [ ' = '.join( item ) for item in list( data.items() ) ] )
 
 def getdefaultlocale() -> str :
     """
     getdefaultlocale will deprecated so use this
     """
     from locale import getlocale
     from sys import platform
@@ -41,15 +44,15 @@
     __slots__ = [ "locale_default" , "locale_use" , "languages" , "path" , "configs" , "types" ]
 
     @property
     def locale( self ) -> str :
         for locale in [ self.locale_use , self.locale_system , self.locale_default ] :
             if locale and locale in self.locales :
                 return locale
-        raise KeyError( f"no such locale '{ self.locale_system }' or '{ self.locale_default }'" )
+        raise errors.LocaleError( f"no such locale '{ self.locale_system }' or '{ self.locale_default }'" )
 
     @property
     def locales( self ) -> list[ str ] :
         return list( self.types.keys() )
 
     @property
     def language( self ) -> dict[ str , str ] :
@@ -98,40 +101,40 @@
         self.types = {}
         self.init()
 
     def config( self , key : str , value : str ) -> None :
         if key in self.configs :
             self.configs[ key ] = value
         else :
-            raise KeyError( f"'{ key }' not in configs" )
+            raise errors.ConfigError( f"'{ key }' not in configs" )
 
     def init( self ) :
         if isinstance( self.path , str ) :
             self.init_file( self.path )
         elif isinstance( self.path , dict ) :
             self.init_dict( self.path )
 
     def init_file( self , path ) -> None :
         """
         init by a directory
         """
         loads = [ [ ".lang" , ".lang" ] , [ ".json" , ".lang" ] ][ self.configs[ "load" ] ]
         self.configs[ "file" ] = True
-        self.language = {}
+        self.languages = {}
         self.path = path
         self.types = {}
         for lang_file in os.listdir( path ) :
             name , suffix = os.path.splitext( lang_file )
             if ( suffix in loads ) and ( ( suffix == loads[ 0 ] ) or ( name not in self.locales ) ) :
                 with open( os.path.join( path , lang_file ) , "r" , encoding = "utf-8" ) as file :
                     if suffix == ".json" :
                         try :
                             data = json.load( file )
                         except json.decoder.JSONDecodeError :
-                            raise SyntaxError( "can't to load .json file" )
+                            raise errors.DecodeError( "can't to load .json file" )
                     elif suffix == ".lang" :
                         data = to_json( file.read() )
                     else :
                         continue
                 self.languages[ name ] = data
                 self.types[ name ] = suffix
 
@@ -156,15 +159,15 @@
         self.path = path
 
     def locale_get( self , locale : str = None ) -> str :
         return locale if locale else self.locale
 
     def locale_set( self , locale : str = None  ) -> None :
         if locale and locale not in self.locales :
-            raise KeyError( f"no such locale '{ locale }'" )
+            raise errors.LocaleError( f"no such locale '{ locale }'" )
         self.locale_use = locale
 
     def lang_get( self , locale : str ) -> dict[ str , str ] :
         return self.languages[ self.locale_get( locale ) ]
 
     def lang_set( self , locale : str , value : dict = {} , suffix : str = ".json" ) -> None :
         locale = self.locale_get( locale )
```

## Comparing `langful-0.40.dist-info/LICENSE` & `langful-0.41.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `langful-0.40.dist-info/METADATA` & `langful-0.41.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langful
-Version: 0.40
+Version: 0.41
 Summary: Help to localization
 Home-page: https://github.com/cueavy/langful
 Author: cueavyqwp
 Author-email: cueavyqwp@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `langful-0.40.dist-info/RECORD` & `langful-0.41.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,8 @@
 langful/__init__.py,sha256=BSJ-BT1Yr3Xz-SFnmZu7QvgV5pgg2WEqUO42oM3Py2w,166
-langful/lang.py,sha256=UwbdQF21-ec75KbuA0J1JaVWjCwUVHOAM1C4TcuVB1w,8206
-langful-0.40.dist-info/LICENSE,sha256=JrQca6fL66RGTmf-hkJU9UEX64JB0yE9gKNsOhpmZVE,1066
-langful-0.40.dist-info/METADATA,sha256=vh0jRqL75Iw4yiXHmhTq6nFUz9hpUXW1enflEESlH3I,2984
-langful-0.40.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-langful-0.40.dist-info/top_level.txt,sha256=EkKV_WnIZfE3A6EhWwDIt2uwZhMVHWXTUueKJL6K15w,8
-langful-0.40.dist-info/RECORD,,
+langful/errors.py,sha256=2Ag2tnAPSzozEIzye5U-mnyvSmvk5X8ZqB3kwLhGOIs,382
+langful/lang.py,sha256=0fEXuuM2--rtU-plANTXtEJDCQG6qnzbKdw9GVXQ77o,8308
+langful-0.41.dist-info/LICENSE,sha256=JrQca6fL66RGTmf-hkJU9UEX64JB0yE9gKNsOhpmZVE,1066
+langful-0.41.dist-info/METADATA,sha256=VrZQbsdkCLGISKnVVIPYwh_k3uW9whNuWxsAURjCmpY,2984
+langful-0.41.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+langful-0.41.dist-info/top_level.txt,sha256=EkKV_WnIZfE3A6EhWwDIt2uwZhMVHWXTUueKJL6K15w,8
+langful-0.41.dist-info/RECORD,,
```

