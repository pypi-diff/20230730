# Comparing `tmp/ScriptCollection-3.4.6-py3-none-any.whl.zip` & `tmp/ScriptCollection-3.4.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 62178 bytes, number of entries: 14
--rw-rw-rw-  2.0 fat    19002 b- defN 23-Jul-30 11:22 ScriptCollection/Executables.py
+Zip file size: 62146 bytes, number of entries: 14
+-rw-rw-rw-  2.0 fat    19005 b- defN 23-Jul-30 17:54 ScriptCollection/Executables.py
 -rw-rw-rw-  2.0 fat    34378 b- defN 23-Jun-27 21:57 ScriptCollection/GeneralUtilities.py
 -rw-rw-rw-  2.0 fat     1937 b- defN 22-Aug-30 21:59 ScriptCollection/ProgramRunnerBase.py
 -rw-rw-rw-  2.0 fat     6275 b- defN 23-May-26 16:46 ScriptCollection/ProgramRunnerEpew.py
 -rw-rw-rw-  2.0 fat     3023 b- defN 22-Aug-30 21:59 ScriptCollection/ProgramRunnerPopen.py
--rw-rw-rw-  2.0 fat    94554 b- defN 23-Jul-30 11:34 ScriptCollection/ScriptCollectionCore.py
+-rw-rw-rw-  2.0 fat    94509 b- defN 23-Jul-30 17:55 ScriptCollection/ScriptCollectionCore.py
 -rw-rw-rw-  2.0 fat   145487 b- defN 23-Jul-30 11:34 ScriptCollection/TasksForCommonProjectStructure.py
 -rw-rw-rw-  2.0 fat     7918 b- defN 22-Aug-30 21:59 ScriptCollection/UpdateCertificates.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Aug-29 05:45 ScriptCollection/__init__.py
--rw-rw-rw-  2.0 fat     7650 b- defN 23-Jul-30 11:34 ScriptCollection-3.4.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-30 11:34 ScriptCollection-3.4.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat     2088 b- defN 23-Jul-30 11:34 ScriptCollection-3.4.6.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       17 b- defN 23-Jul-30 11:34 ScriptCollection-3.4.6.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1290 b- defN 23-Jul-30 11:34 ScriptCollection-3.4.6.dist-info/RECORD
-14 files, 323711 bytes uncompressed, 59996 bytes compressed:  81.5%
+-rw-rw-rw-  2.0 fat     7650 b- defN 23-Jul-30 17:55 ScriptCollection-3.4.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-30 17:55 ScriptCollection-3.4.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat     2088 b- defN 23-Jul-30 17:55 ScriptCollection-3.4.7.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       17 b- defN 23-Jul-30 17:55 ScriptCollection-3.4.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1290 b- defN 23-Jul-30 17:55 ScriptCollection-3.4.7.dist-info/RECORD
+14 files, 323669 bytes uncompressed, 59964 bytes compressed:  81.5%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: ScriptCollection/UpdateCertificates.py
 Comment: 
 
 Filename: ScriptCollection/__init__.py
 Comment: 
 
-Filename: ScriptCollection-3.4.6.dist-info/METADATA
+Filename: ScriptCollection-3.4.7.dist-info/METADATA
 Comment: 
 
-Filename: ScriptCollection-3.4.6.dist-info/WHEEL
+Filename: ScriptCollection-3.4.7.dist-info/WHEEL
 Comment: 
 
-Filename: ScriptCollection-3.4.6.dist-info/entry_points.txt
+Filename: ScriptCollection-3.4.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: ScriptCollection-3.4.6.dist-info/top_level.txt
+Filename: ScriptCollection-3.4.7.dist-info/top_level.txt
 Comment: 
 
-Filename: ScriptCollection-3.4.6.dist-info/RECORD
+Filename: ScriptCollection-3.4.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ScriptCollection/Executables.py

```diff
@@ -10,15 +10,16 @@
 
 def DotNetsign() -> int:
     parser = argparse.ArgumentParser(description='Signs a dll- or exe-file with a snk-file. Requires ilasm and ildasm as available commandline-commands.')
     parser.add_argument("dllOrExefile")
     parser.add_argument("snkfile")
     parser.add_argument("verbose", action='store_true')
     args = parser.parse_args()
-    return ScriptCollectionCore().dotnet_sign(args.dllOrExefile, args.snkfile, args.verbose, {})
+    ScriptCollectionCore().dotnet_sign(args.dllOrExefile, args.snkfile, args.verbose)
+    return 0
 
 
 def FilenameObfuscator() -> int:
     parser = argparse.ArgumentParser(description=''''Obfuscates the names of all files in the given folder.
 Caution: This script can cause harm if you pass a wrong inputfolder-argument.''')
 
     parser.add_argument('--printtableheadline', type=GeneralUtilities.string_to_boolean, const=True, default=True, nargs='?',
```

## ScriptCollection/ScriptCollectionCore.py

```diff
@@ -25,15 +25,15 @@
 import PyPDF2
 from .GeneralUtilities import GeneralUtilities
 from .ProgramRunnerBase import ProgramRunnerBase
 from .ProgramRunnerPopen import ProgramRunnerPopen
 from .ProgramRunnerEpew import ProgramRunnerEpew, CustomEpewArgument
 
 
-version = "3.4.6"
+version = "3.4.7"
 __version__ = version
 
 
 class ScriptCollectionCore:
 
     # The purpose of this property is to use it when testing your code which uses scriptcollection for external program-calls.
     # Do not change this value for productive environments.
@@ -119,15 +119,15 @@
 
     @GeneralUtilities.check_arguments
     def dotnet_build(self, repository_folder: str, projectname: str, configuration: str):
         self.run_program("dotnet", f"clean -c {configuration}", repository_folder)
         self.run_program("dotnet", f"build {projectname}/{projectname}.csproj -c {configuration}", repository_folder)
 
     @GeneralUtilities.check_arguments
-    def dotnet_sign(self, dllOrExefile: str, snkfile: str, verbosity: int, current_release_information: dict[str, str]) -> None:
+    def dotnet_sign(self, dllOrExefile: str, snkfile: str, verbosity: int) -> None:
         dllOrExeFile = GeneralUtilities.resolve_relative_path_from_current_working_directory(dllOrExefile)
         snkfile = GeneralUtilities.resolve_relative_path_from_current_working_directory(snkfile)
         directory = os.path.dirname(dllOrExeFile)
         filename = os.path.basename(dllOrExeFile)
         if filename.lower().endswith(".dll"):
             filename = filename[:-4]
             extension = "dll"
```

## Comparing `ScriptCollection-3.4.6.dist-info/METADATA` & `ScriptCollection-3.4.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ScriptCollection
-Version: 3.4.6
+Version: 3.4.7
 Summary: The ScriptCollection is the place for reusable scripts.
 Home-page: https://github.com/anionDev/ScriptCollection
 Author: Marius Göcke
 Author-email: marius.goecke@gmail.com
 Project-URL: Documentation, https://aniondev.github.io/ScriptCollectionReference/index.html
 Project-URL: Changelog, https://github.com/anionDev/ScriptCollection/tree/main/Other/Resources/Changelog
 Keywords: package release build management
```

## Comparing `ScriptCollection-3.4.6.dist-info/entry_points.txt` & `ScriptCollection-3.4.7.dist-info/entry_points.txt`

 * *Files identical despite different names*

## Comparing `ScriptCollection-3.4.6.dist-info/RECORD` & `ScriptCollection-3.4.7.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-ScriptCollection/Executables.py,sha256=srooVN3-X76sJKG99BxKBV4kuF_GFNq-SuV-zTmNJGw,19002
+ScriptCollection/Executables.py,sha256=tRIsXE_ZhjnMt75YhEL-FHEHuiUC3YzGdeVibLiWvoE,19005
 ScriptCollection/GeneralUtilities.py,sha256=vZDiW5lWJRCrIZVs1bTCZ-O5slQnM5dv4GcJ-RTMowY,34378
 ScriptCollection/ProgramRunnerBase.py,sha256=2kyOuoM3oFjBfLc9Q5t5RTz7Ya2CjUxFtB1rBBDmnjU,1937
 ScriptCollection/ProgramRunnerEpew.py,sha256=nIzY4dG6W-xEpkeoTbozwNZtFSIo-bU_W6t6u1AZKtE,6275
 ScriptCollection/ProgramRunnerPopen.py,sha256=HOs1QVnXiQtwXy1_xvH79bWBdd0i-2tUyyLloQBvMto,3023
-ScriptCollection/ScriptCollectionCore.py,sha256=hOkgV6v1XGqiX9TU7_Oqe-UJlYFmFmEwxKwaIybI2JI,94554
+ScriptCollection/ScriptCollectionCore.py,sha256=3VW2HQcdg922t70dArGKLbS1bzZ2pPmJoRHnmWqe4QY,94509
 ScriptCollection/TasksForCommonProjectStructure.py,sha256=3ZXzRX7YAzLS8NurwSG0WLfnByVEbmmzx-s8zBME4vs,145487
 ScriptCollection/UpdateCertificates.py,sha256=Go-JJK-YTi7aBB1phlLxypa8GHkmFHBEPB0_TT9G-bw,7918
 ScriptCollection/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-ScriptCollection-3.4.6.dist-info/METADATA,sha256=a0a1ZlEkJK2t1C0-CV_bSxnINH0Hjw-AXuakJ6UPfSY,7650
-ScriptCollection-3.4.6.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-ScriptCollection-3.4.6.dist-info/entry_points.txt,sha256=dJKdWcH41owxlKx_khj4P7DItr9lhxWP9JU2Dq8GSsQ,2088
-ScriptCollection-3.4.6.dist-info/top_level.txt,sha256=hY2hOVH0V0Ce51WB76zKkIWTUNwMUdHo4XDkR2vYVwg,17
-ScriptCollection-3.4.6.dist-info/RECORD,,
+ScriptCollection-3.4.7.dist-info/METADATA,sha256=xdKalQHDkJxViIU3DkXJZMAP2PmiGKLh7feso3xeiv8,7650
+ScriptCollection-3.4.7.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+ScriptCollection-3.4.7.dist-info/entry_points.txt,sha256=dJKdWcH41owxlKx_khj4P7DItr9lhxWP9JU2Dq8GSsQ,2088
+ScriptCollection-3.4.7.dist-info/top_level.txt,sha256=hY2hOVH0V0Ce51WB76zKkIWTUNwMUdHo4XDkR2vYVwg,17
+ScriptCollection-3.4.7.dist-info/RECORD,,
```

