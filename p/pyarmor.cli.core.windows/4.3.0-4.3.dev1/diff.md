# Comparing `tmp/pyarmor.cli.core.windows-4.3.0-cp37-none-any.whl.zip` & `tmp/pyarmor.cli.core.windows-4.3.dev1-cp39-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 819143 bytes, number of entries: 9
--rw-r--r--  2.0 unx       22 b- defN 23-Jul-29 00:46 pyarmor/cli/core/windows/__init__.py
--rwxr-xr-x  2.0 unx   754190 b- defN 23-Jul-29 00:46 pyarmor/cli/core/windows/x86/pyarmor_runtime.pyd
--rwxr-xr-x  2.0 unx   582656 b- defN 23-Jul-29 00:46 pyarmor/cli/core/windows/x86/pytransform3.pyd
--rwxr-xr-x  2.0 unx   610816 b- defN 23-Jul-29 00:46 pyarmor/cli/core/windows/x86_64/pyarmor_runtime.pyd
--rwxr-xr-x  2.0 unx   444416 b- defN 23-Jul-29 00:46 pyarmor/cli/core/windows/x86_64/pytransform3.pyd
--rw-r--r--  2.0 unx      808 b- defN 23-Jul-29 00:46 pyarmor.cli.core.windows-4.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx       93 b- defN 23-Jul-29 00:46 pyarmor.cli.core.windows-4.3.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Jul-29 00:46 pyarmor.cli.core.windows-4.3.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      883 b- defN 23-Jul-29 00:46 pyarmor.cli.core.windows-4.3.0.dist-info/RECORD
-9 files, 2393892 bytes uncompressed, 817589 bytes compressed:  65.9%
+Zip file size: 1383832 bytes, number of entries: 9
+-rw-r--r--  2.0 unx       25 b- defN 23-Jul-23 12:58 pyarmor/cli/core/windows/__init__.py
+-rwxr-xr-x  2.0 unx   762894 b- defN 23-Jul-23 12:58 pyarmor/cli/core/windows/x86/pyarmor_runtime.pyd
+-rwxr-xr-x  2.0 unx   865280 b- defN 23-Jul-23 12:58 pyarmor/cli/core/windows/x86/pytransform3.pyd
+-rwxr-xr-x  2.0 unx   617472 b- defN 23-Jul-23 12:58 pyarmor/cli/core/windows/x86_64/pyarmor_runtime.pyd
+-rwxr-xr-x  2.0 unx   725504 b- defN 23-Jul-23 12:58 pyarmor/cli/core/windows/x86_64/pytransform3.pyd
+-rw-r--r--  2.0 unx      811 b- defN 23-Jul-23 12:58 pyarmor.cli.core.windows-4.3.dev1.dist-info/METADATA
+-rw-r--r--  2.0 unx       93 b- defN 23-Jul-23 12:58 pyarmor.cli.core.windows-4.3.dev1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Jul-23 12:58 pyarmor.cli.core.windows-4.3.dev1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      895 b- defN 23-Jul-23 12:58 pyarmor.cli.core.windows-4.3.dev1.dist-info/RECORD
+9 files, 2972982 bytes uncompressed, 1382254 bytes compressed:  53.5%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: pyarmor/cli/core/windows/x86_64/pyarmor_runtime.pyd
 Comment: 
 
 Filename: pyarmor/cli/core/windows/x86_64/pytransform3.pyd
 Comment: 
 
-Filename: pyarmor.cli.core.windows-4.3.0.dist-info/METADATA
+Filename: pyarmor.cli.core.windows-4.3.dev1.dist-info/METADATA
 Comment: 
 
-Filename: pyarmor.cli.core.windows-4.3.0.dist-info/WHEEL
+Filename: pyarmor.cli.core.windows-4.3.dev1.dist-info/WHEEL
 Comment: 
 
-Filename: pyarmor.cli.core.windows-4.3.0.dist-info/top_level.txt
+Filename: pyarmor.cli.core.windows-4.3.dev1.dist-info/top_level.txt
 Comment: 
 
-Filename: pyarmor.cli.core.windows-4.3.0.dist-info/RECORD
+Filename: pyarmor.cli.core.windows-4.3.dev1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyarmor/cli/core/windows/__init__.py

```diff
@@ -1 +1 @@
-__VERSION__ = '4.3.0'
+__VERSION__ = '4.3.dev1'
```

## Comparing `pyarmor.cli.core.windows-4.3.0.dist-info/METADATA` & `pyarmor.cli.core.windows-4.3.dev1.dist-info/METADATA`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyarmor.cli.core.windows
-Version: 4.3.0
+Version: 4.3.dev1
 Summary: Provide pre-built extension modules `pytransform3` and `pyarmor_runtime` for Pyarmor
 Home-page: https://github.com/dashingsoft/pyarmor
 Author: Jondy Zhao
 Author-email: pyarmor@163.com
 License: Free To Use But Restricted
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `pyarmor.cli.core.windows-4.3.0.dist-info/RECORD` & `pyarmor.cli.core.windows-4.3.dev1.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-pyarmor/cli/core/windows/__init__.py,sha256=CDPRinTnSD2xTY7mjTAtyXcMyIiRXVKcho3q-rEYva8,22
-pyarmor/cli/core/windows/x86/pyarmor_runtime.pyd,sha256=Z56RmaRL6cgJ4pgNegSzDKA3cqzHAkV6_EdvD4s3W1E,754190
-pyarmor/cli/core/windows/x86/pytransform3.pyd,sha256=sj8DyveisdLBrkshGjzBfHVhkcUntmpIWdJIt3-PSmI,582656
-pyarmor/cli/core/windows/x86_64/pyarmor_runtime.pyd,sha256=KOMktp08fbhxwkUq-YkFlxXbpAW2ytd15cMGy6Ku3DU,610816
-pyarmor/cli/core/windows/x86_64/pytransform3.pyd,sha256=w-Xfkn50A6vF5OxHodRRp-gBpFeF4T415JUAi2XyDyM,444416
-pyarmor.cli.core.windows-4.3.0.dist-info/METADATA,sha256=2ggLU6-jIPBC8YEejS2pXnt2VbhYuCsJZ4h07xBe8Og,808
-pyarmor.cli.core.windows-4.3.0.dist-info/WHEEL,sha256=B1xNSF-3cuB7fHdJVETQupXu4HfdTmSjLassywAtmRc,93
-pyarmor.cli.core.windows-4.3.0.dist-info/top_level.txt,sha256=UE1ovZ_90YzwF_lZ3LV7o8HKLe-RgzUaUUvdH5UTUus,8
-pyarmor.cli.core.windows-4.3.0.dist-info/RECORD,,
+pyarmor/cli/core/windows/__init__.py,sha256=-ZsoB3RONIDHw9_pOlDaLpAfTbSGcr3JIbok364TpcQ,25
+pyarmor/cli/core/windows/x86/pyarmor_runtime.pyd,sha256=D6iJGQTuJqMlLng-g6MW2kRYlgpBxefzKbN9Viq6Ow8,762894
+pyarmor/cli/core/windows/x86/pytransform3.pyd,sha256=3Qv0CAs8_QTxKaKpsW1phqYLvELVR5UUxCXJAPkVlBc,865280
+pyarmor/cli/core/windows/x86_64/pyarmor_runtime.pyd,sha256=hYGqN38ZdW7Iz3He6PWS1hjkOoo9eKvwAe_a4MWesf4,617472
+pyarmor/cli/core/windows/x86_64/pytransform3.pyd,sha256=hVoBZJh1q5K5V12EmS8KE4TlIkeL-BBHLB1m99P_JoM,725504
+pyarmor.cli.core.windows-4.3.dev1.dist-info/METADATA,sha256=iJ_crMf05jETGW8PbFgX4OjEgRcLOOKtK0_UAY1liaw,811
+pyarmor.cli.core.windows-4.3.dev1.dist-info/WHEEL,sha256=QbbyyBnlPXzoGKd-349G69XkCwSd1NFnt4kuAN58gNs,93
+pyarmor.cli.core.windows-4.3.dev1.dist-info/top_level.txt,sha256=UE1ovZ_90YzwF_lZ3LV7o8HKLe-RgzUaUUvdH5UTUus,8
+pyarmor.cli.core.windows-4.3.dev1.dist-info/RECORD,,
```

