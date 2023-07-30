# Comparing `tmp/wbBase-0.2.2.tar.gz` & `tmp/wbBase-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wbBase-0.2.2.tar", last modified: Fri Jun 30 13:31:43 2023, max compression
+gzip compressed data, was "wbBase-0.2.3.tar", last modified: Sun Jul 30 13:11:34 2023, max compression
```

## Comparing `wbBase-0.2.2.tar` & `wbBase-0.2.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:31:43.669727 wbBase-0.2.2/
--rw-rw-rw-   0 root         (0) root         (0)     1079 2023-06-30 13:31:42.000000 wbBase-0.2.2/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:31:43.663727 wbBase-0.2.2/Lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:31:43.666727 wbBase-0.2.2/Lib/wbBase/
--rw-rw-rw-   0 root         (0) root         (0)      152 2023-06-30 13:31:42.000000 wbBase-0.2.2/Lib/wbBase/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    25590 2023-06-30 13:31:42.000000 wbBase-0.2.2/Lib/wbBase/application.py
--rw-rw-rw-   0 root         (0) root         (0)     2165 2023-06-30 13:31:42.000000 wbBase-0.2.2/Lib/wbBase/applicationInfo.py
--rw-rw-rw-   0 root         (0) root         (0)    20784 2023-06-30 13:31:42.000000 wbBase-0.2.2/Lib/wbBase/applicationWindow.py
--rw-rw-rw-   0 root         (0) root         (0)   309861 2023-06-30 13:31:42.000000 wbBase-0.2.2/Lib/wbBase/artprovider.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:31:43.668727 wbBase-0.2.2/Lib/wbBase/control/
--rw-rw-rw-   0 root         (0) root         (0)     1118 2023-06-30 13:31:42.000000 wbBase-0.2.2/Lib/wbBase/control/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4414 2023-06-30 13:31:42.000000 wbBase-0.2.2/Lib/wbBase/control/externalToolConfig.py
--rw-rw-rw-   0 root         (0) root         (0)     5891 2023-06-30 13:31:42.000000 wbBase-0.2.2/Lib/wbBase/control/externalToolConfigUI.py
--rw-rw-rw-   0 root         (0) root         (0)     2666 2023-06-30 13:31:42.000000 wbBase-0.2.2/Lib/wbBase/control/filling.py
--rw-rw-rw-   0 root         (0) root         (0)     1670 2023-06-30 13:31:42.000000 wbBase-0.2.2/Lib/wbBase/control/iePanel.py
--rw-rw-rw-   0 root         (0) root         (0)     8569 2023-06-30 13:31:42.000000 wbBase-0.2.2/Lib/wbBase/control/propgrid.py
--rw-rw-rw-   0 root         (0) root         (0)    47198 2023-06-30 13:31:42.000000 wbBase-0.2.2/Lib/wbBase/control/textEditControl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:31:43.668727 wbBase-0.2.2/Lib/wbBase/dialog/
--rw-rw-rw-   0 root         (0) root         (0)       68 2023-06-30 13:31:42.000000 wbBase-0.2.2/Lib/wbBase/dialog/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2342 2023-06-30 13:31:42.000000 wbBase-0.2.2/Lib/wbBase/dialog/multiSaveModifiedDialog.py
--rw-rw-rw-   0 root         (0) root         (0)     3293 2023-06-30 13:31:42.000000 wbBase-0.2.2/Lib/wbBase/dialog/multiSaveModifiedDialogUI.py
--rw-rw-rw-   0 root         (0) root         (0)    20381 2023-06-30 13:31:42.000000 wbBase-0.2.2/Lib/wbBase/dialog/preferences.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:31:43.669727 wbBase-0.2.2/Lib/wbBase/document/
--rw-rw-rw-   0 root         (0) root         (0)    23492 2023-06-30 13:31:42.000000 wbBase-0.2.2/Lib/wbBase/document/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    36912 2023-06-30 13:31:42.000000 wbBase-0.2.2/Lib/wbBase/document/manager.py
--rw-rw-rw-   0 root         (0) root         (0)     4743 2023-06-30 13:31:42.000000 wbBase-0.2.2/Lib/wbBase/document/notebook.py
--rw-rw-rw-   0 root         (0) root         (0)     8016 2023-06-30 13:31:42.000000 wbBase-0.2.2/Lib/wbBase/document/template.py
--rw-rw-rw-   0 root         (0) root         (0)     9208 2023-06-30 13:31:42.000000 wbBase-0.2.2/Lib/wbBase/document/view.py
--rw-rw-rw-   0 root         (0) root         (0)    22086 2023-06-30 13:31:42.000000 wbBase-0.2.2/Lib/wbBase/panelManager.py
--rw-rw-rw-   0 root         (0) root         (0)     3362 2023-06-30 13:31:42.000000 wbBase-0.2.2/Lib/wbBase/pluginManager.py
--rw-rw-rw-   0 root         (0) root         (0)     2942 2023-06-30 13:31:42.000000 wbBase-0.2.2/Lib/wbBase/pluginManager_old.py
--rw-rw-rw-   0 root         (0) root         (0)     8814 2023-06-30 13:31:42.000000 wbBase-0.2.2/Lib/wbBase/scripting.py
--rw-rw-rw-   0 root         (0) root         (0)      929 2023-06-30 13:31:42.000000 wbBase-0.2.2/Lib/wbBase/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:31:43.666727 wbBase-0.2.2/Lib/wbBase.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2848 2023-06-30 13:31:43.000000 wbBase-0.2.2/Lib/wbBase.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1027 2023-06-30 13:31:43.000000 wbBase-0.2.2/Lib/wbBase.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 13:31:43.000000 wbBase-0.2.2/Lib/wbBase.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       90 2023-06-30 13:31:43.000000 wbBase-0.2.2/Lib/wbBase.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-30 13:31:43.000000 wbBase-0.2.2/Lib/wbBase.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2848 2023-06-30 13:31:43.669727 wbBase-0.2.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1444 2023-06-30 13:31:42.000000 wbBase-0.2.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2032 2023-06-30 13:31:43.670727 wbBase-0.2.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-06-30 13:31:42.000000 wbBase-0.2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 13:11:34.735358 wbBase-0.2.3/
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2023-07-30 13:11:33.000000 wbBase-0.2.3/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 13:11:34.728358 wbBase-0.2.3/Lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 13:11:34.731358 wbBase-0.2.3/Lib/wbBase/
+-rw-rw-rw-   0 root         (0) root         (0)      152 2023-07-30 13:11:33.000000 wbBase-0.2.3/Lib/wbBase/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    25620 2023-07-30 13:11:33.000000 wbBase-0.2.3/Lib/wbBase/application.py
+-rw-rw-rw-   0 root         (0) root         (0)     2377 2023-07-30 13:11:33.000000 wbBase-0.2.3/Lib/wbBase/applicationInfo.py
+-rw-rw-rw-   0 root         (0) root         (0)    20784 2023-07-30 13:11:33.000000 wbBase-0.2.3/Lib/wbBase/applicationWindow.py
+-rw-rw-rw-   0 root         (0) root         (0)   311454 2023-07-30 13:11:33.000000 wbBase-0.2.3/Lib/wbBase/artprovider.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 13:11:34.733358 wbBase-0.2.3/Lib/wbBase/control/
+-rw-rw-rw-   0 root         (0) root         (0)     1118 2023-07-30 13:11:33.000000 wbBase-0.2.3/Lib/wbBase/control/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4414 2023-07-30 13:11:33.000000 wbBase-0.2.3/Lib/wbBase/control/externalToolConfig.py
+-rw-rw-rw-   0 root         (0) root         (0)     5891 2023-07-30 13:11:33.000000 wbBase-0.2.3/Lib/wbBase/control/externalToolConfigUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     2666 2023-07-30 13:11:33.000000 wbBase-0.2.3/Lib/wbBase/control/filling.py
+-rw-rw-rw-   0 root         (0) root         (0)     1670 2023-07-30 13:11:33.000000 wbBase-0.2.3/Lib/wbBase/control/iePanel.py
+-rw-rw-rw-   0 root         (0) root         (0)     8569 2023-07-30 13:11:33.000000 wbBase-0.2.3/Lib/wbBase/control/propgrid.py
+-rw-rw-rw-   0 root         (0) root         (0)    47198 2023-07-30 13:11:33.000000 wbBase-0.2.3/Lib/wbBase/control/textEditControl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 13:11:34.734358 wbBase-0.2.3/Lib/wbBase/dialog/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-07-30 13:11:33.000000 wbBase-0.2.3/Lib/wbBase/dialog/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2342 2023-07-30 13:11:33.000000 wbBase-0.2.3/Lib/wbBase/dialog/multiSaveModifiedDialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     3293 2023-07-30 13:11:33.000000 wbBase-0.2.3/Lib/wbBase/dialog/multiSaveModifiedDialogUI.py
+-rw-rw-rw-   0 root         (0) root         (0)    20381 2023-07-30 13:11:33.000000 wbBase-0.2.3/Lib/wbBase/dialog/preferences.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 13:11:34.735358 wbBase-0.2.3/Lib/wbBase/document/
+-rw-rw-rw-   0 root         (0) root         (0)    23535 2023-07-30 13:11:33.000000 wbBase-0.2.3/Lib/wbBase/document/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    36912 2023-07-30 13:11:33.000000 wbBase-0.2.3/Lib/wbBase/document/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     4743 2023-07-30 13:11:33.000000 wbBase-0.2.3/Lib/wbBase/document/notebook.py
+-rw-rw-rw-   0 root         (0) root         (0)     8016 2023-07-30 13:11:33.000000 wbBase-0.2.3/Lib/wbBase/document/template.py
+-rw-rw-rw-   0 root         (0) root         (0)     8193 2023-07-30 13:11:33.000000 wbBase-0.2.3/Lib/wbBase/document/view.py
+-rw-rw-rw-   0 root         (0) root         (0)    22086 2023-07-30 13:11:33.000000 wbBase-0.2.3/Lib/wbBase/panelManager.py
+-rw-rw-rw-   0 root         (0) root         (0)     3362 2023-07-30 13:11:33.000000 wbBase-0.2.3/Lib/wbBase/pluginManager.py
+-rw-rw-rw-   0 root         (0) root         (0)     2942 2023-07-30 13:11:33.000000 wbBase-0.2.3/Lib/wbBase/pluginManager_old.py
+-rw-rw-rw-   0 root         (0) root         (0)     8814 2023-07-30 13:11:33.000000 wbBase-0.2.3/Lib/wbBase/scripting.py
+-rw-rw-rw-   0 root         (0) root         (0)      929 2023-07-30 13:11:33.000000 wbBase-0.2.3/Lib/wbBase/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 13:11:34.732358 wbBase-0.2.3/Lib/wbBase.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2848 2023-07-30 13:11:34.000000 wbBase-0.2.3/Lib/wbBase.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1027 2023-07-30 13:11:34.000000 wbBase-0.2.3/Lib/wbBase.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-30 13:11:34.000000 wbBase-0.2.3/Lib/wbBase.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       90 2023-07-30 13:11:34.000000 wbBase-0.2.3/Lib/wbBase.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-30 13:11:34.000000 wbBase-0.2.3/Lib/wbBase.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2848 2023-07-30 13:11:34.735358 wbBase-0.2.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1444 2023-07-30 13:11:33.000000 wbBase-0.2.3/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2032 2023-07-30 13:11:34.736358 wbBase-0.2.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-07-30 13:11:33.000000 wbBase-0.2.3/setup.py
```

### Comparing `wbBase-0.2.2/LICENSE` & `wbBase-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.2/Lib/wbBase/application.py` & `wbBase-0.2.3/Lib/wbBase/application.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     SplashScreen,
     TipProvider,
 )
 
 from .applicationInfo import ApplicationInfo
 from .applicationWindow import ApplicationWindow
 from .artprovider import Artprovider
-from .document import DOC_SILENT
+from .document import DOC_SILENT, dbg
 from .pluginManager import PluginManager
 from .scripting import execfile, execsource
 
 try:
     from git import GitCommandError, InvalidGitRepositoryError
     from git.repo import Repo
 
@@ -190,22 +190,23 @@
     config: wx.ConfigBase
     instanceChecker: wx.SingleInstanceChecker
 
     _post_init_queue: List[FunctionType] = []
 
     def __init__(
         self,
-        debug: int = 1,
+        debug: int = 0,
         iconName: str = wx.ART_EXECUTABLE_FILE,
         test: bool = False,
         info: Optional[ApplicationInfo] = None,
     ):
         """
         Constructor
         """
+        dbg._dbg = debug
         self._debug: int = debug
         self.iconName: str = iconName
         self._test = test
         self._splashScreen: Optional[AppSplashScreen] = None
         self._extChangeMode: int = self.EXT_CHANGE_TEST_ON_REQUEST
         self.allowMultipleInstances: bool = False
         self.info: ApplicationInfo = self._getAppInfo(info)
```

### Comparing `wbBase-0.2.2/Lib/wbBase/applicationInfo.py` & `wbBase-0.2.3/Lib/wbBase/applicationInfo.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,20 +5,27 @@
 from typing import Any, Dict, List
 
 import yaml
 
 
 @dataclass
 class PluginInfo:
+    """
+    Object which provides information about a Workbench plugin.
+    """
     Name: str
     Installation: str = "optional"
+    Requires: List[str] = field(default_factory=list)
 
 
 @dataclass
 class ApplicationInfo:
+    """
+    Object which provides information about a Workbench aplication.
+    """
     AppName: str = "Application"
     AppDisplayName: str = ""
     VendorName: str = "WorkBench"
     VendorDisplayName: str = ""
     Description: str = "WorkBench GUI Application"
     Copyright: str = ""
     URL: str = "https://gitlab.com/workbench2/wbbase"
@@ -67,12 +74,12 @@
 - Name: output
   Installation: required
 - Name: shell
   Installation: default
 - Name: loglist
 """
 if __name__ == "__main__":
-    appinfo = ApplicationInfo.fromString(sampleInfo)
-    print(asdict(appinfo))
+    info = ApplicationInfo.fromString(sampleInfo)
+    print(asdict(info))
     p1 = PluginInfo("test")
     p2 = PluginInfo("test")
     print(p1 == p2)
```

### Comparing `wbBase-0.2.2/Lib/wbBase/applicationWindow.py` & `wbBase-0.2.3/Lib/wbBase/applicationWindow.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.2/Lib/wbBase/artprovider.py` & `wbBase-0.2.3/Lib/wbBase/artprovider.py`

 * *Files 0% similar despite different names*

```diff
@@ -2397,14 +2397,37 @@
 [\x89C\x1963\xcf1\xec\x981\xf9h\xd1\xd6{\x02N3n\x1c\xca\xab\xb7\x98\xb7\xef\
 \x91\x8f\xfe\xf5\xdb\x7f\x1d5S\xc3\xe7\xfd\x11\rUP\xf9\xcb\xf2\xf7)\xab\x9b\
 \x9bH\xe8\xc5\x16\xb5\xcd@\'\xab\x96\xb8F\x94\xa4$\x96\xa4Z%\x17\xa5\x02)\
 \x06#\x03Cs]\x03\x13]#\xa3\x10Cs+C\x13+cKm\x03#+\x03\x03\x9b\xe0\xd3\xcfP4\
 \xe4\xe6\xa7d\xa6UB5X\xe8\x1a\x9a\x84\x18\x1aX\x19\x9bX\x19Y@4<\xe2{\xfa\x0e\
 \xa8\x81\xc1\xd3\xd5\xcfe\x9dSB\x13\x00\xea\x967\xc3' )
 
+addArtData('wxART_LOGCONFIG', 'wxART_OTHER_C', 16,
+b'x\xda\x01\xfe\x01\x01\xfe\x89PNG\r\n\x1a\n\x00\x00\x00\rIHDR\x00\x00\x00\
+\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\x00\x00\x00\tpHYs\x00\
+\x00\x0b\x13\x00\x00\x0b\x13\x01\x00\x9a\x9c\x18\x00\x00\x01\xb0IDAT8\x8d\
+\xa5SAK\x1bA\x18}[\xd2C\xef{\xe9^z/\xf4P\x16\n\x16\x84\x94\xfe\x04\x1b\x8dB\
+\xd5C\x9b\x88\x16=H{\xf7VP\xac\xa2\x89\xa4"\xec\x06\x04\xdb\xe2O(\xe4\xe4iFo\
+\x1e\xbc\xb6L\x04\x8d\xa5M69\xf9\xbd\x1efg5\n\x1e\xcc\xc00\xcc\xc7\xf7\xde\
+\xbc\xf7f\xc6#\x89AF\xce[Z\x82o\xf2\xe6>\xe0\xf3\xa0\x11\xe4|\x937O\x9e?\xbb\
+\xb3\xb1\x1c>BM\xf7\xb2\xf5\xe0\xf85^>\xfd\t\x1c\xc1x~\xa9a\x1e\x9e\x1c\xdeK\
+>\x00\xc0/5L\xaf\xd7S\x85\xb1\x11&\xdd\xae\xea$]\xd5N\xec\xfeO\xbb\xabZ\xff\
+\x12u\xfe7Q\x85\xb1\x11\x9e^tT\xb3\xd5Q\xbf[m\xf5\xeb\xac\xad\x1e\xe7WM\x0e\
+\x00\\\x8e\xa4\x07\x01\xb3B\xe9\xdd\xdb\xd0\x1d\xf4co\x1f("\\\xab\xc6\xfa\
+\xcdb\xe4\xea\xcd\xdcu5\xee>$%\xd8\xfaZ\xd7$@\x10("\\\xaf\xc6\xfa\x92\xc4\
+\xb7\xe5iM\x02C\xa3\xdb\x81U\x90BIBxE\xc4t\x8a\x00\xeb\xd5XK*\x8e\xd70\x0f\
+\xfa,8`f\x89\x10\xb1\xa4\x0b\xb3S!\x1d\x01\t\x8a\xedI\x15x\x19PH\x90@\xa5V\
+\xd7s\xe5\xc9[\x19,oDz\xfcS\xdc\x9f\x81{\x8d\xfd\x12\x81\x8d\xadX\x0b\x89Kz\
+\x16\xbc\x19i\x11b\xf7\xf3\xb4&\x05\xc3\xe3;\xc1\r\x0b\xd6\x99\x90\xf8P\x9e\
+\x0c\xb3<H\xaclF\x9a\xe2\xc8\x05\xa9\x03kA\x00\xd4\xb6\xeb\xba\xfc\xfeJ\xf2\
+\xf7\xbd}\x8c\x16\x11\xaeV"]\xf8\x98]\xdb\xcd\xd1\xf4\xfcR\xc3\x9c\xac\xbc0\
+\xce\xbb\xc0\x866?3\x15~\xa9X\x0b\xe2\xb2\xc9l\xda\xda\xab\x89\x9d`\xe0\xa7\
+\xec\r\xfa\x9d\xff\x03hl\x1dh\xf4\xc5&M\x00\x00\x00\x00IEND\xaeB`\x82\xf79\
+\xe41' )
+
 addArtData('wxART_MACRO', 'wxART_OTHER_C', 16,
 b"x\xda\xeb\x0c\xf0s\xe7\xe5\x92\xe2b``\xe0\xf5\xf4p\t\x02\xd2\x02 \xcc\xc1\
 \x0c$5t\xf9\x83\x81\x14K\xba\xa3\xaf#\x03\xc3\xc6\xbe\x9a\xdf\x81\x93\x81|\
 \x85d\x8f _\x06\x86*U\x06\x86\x86f\x06\x86\x9f\xff\x81\xf4K\x06\x86R\x03\x06\
 \x86W\t\x0c\x0cV3\x18\x18\xc4\xf3'\xc5\x1fu\x03\xaa\x8d\r\xf0\tq\xfd\xff\xff\
 \xff\xba5_\xe6\xcc~\x90\x9dv\xe8\xc6\x8d\x9f\xff\xfe\xfd\xff\xf2\xe5\x7fy\
 \xc9\xad\xf7\xef\xff\x9d8\xf6\xdc\xdfs\xfd\xae\x9dO\x9f<\xf9\xd3\xdby2.jWR\
```

### Comparing `wbBase-0.2.2/Lib/wbBase/control/__init__.py` & `wbBase-0.2.3/Lib/wbBase/control/__init__.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.2/Lib/wbBase/control/externalToolConfig.py` & `wbBase-0.2.3/Lib/wbBase/control/externalToolConfig.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.2/Lib/wbBase/control/externalToolConfigUI.py` & `wbBase-0.2.3/Lib/wbBase/control/externalToolConfigUI.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.2/Lib/wbBase/control/filling.py` & `wbBase-0.2.3/Lib/wbBase/control/filling.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.2/Lib/wbBase/control/iePanel.py` & `wbBase-0.2.3/Lib/wbBase/control/iePanel.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.2/Lib/wbBase/control/propgrid.py` & `wbBase-0.2.3/Lib/wbBase/control/propgrid.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.2/Lib/wbBase/control/textEditControl.py` & `wbBase-0.2.3/Lib/wbBase/control/textEditControl.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.2/Lib/wbBase/dialog/multiSaveModifiedDialog.py` & `wbBase-0.2.3/Lib/wbBase/dialog/multiSaveModifiedDialog.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.2/Lib/wbBase/dialog/multiSaveModifiedDialogUI.py` & `wbBase-0.2.3/Lib/wbBase/dialog/multiSaveModifiedDialogUI.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.2/Lib/wbBase/dialog/preferences.py` & `wbBase-0.2.3/Lib/wbBase/dialog/preferences.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.2/Lib/wbBase/document/__init__.py` & `wbBase-0.2.3/Lib/wbBase/document/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,17 +22,19 @@
 
 log = logging.getLogger(__name__)
 
 dbg = Logger("doc")
 if hasattr(sys, "frozen") and sys.frozen:
     dbg(enable=0)
 else:
-    # dbg(enable=wx.GetApp()._debug)
-    # print(sys.argv[0])
-    dbg(enable=int(sys.argv[0].endswith("py")))
+    app = wx.GetApp()
+    if app and hasattr(app, "_debug"):
+        dbg._dbg = app._debug
+    else:
+        dbg(enable=int(sys.argv[0].endswith("py")))
 
 
 # ----------------------------------------------------------------------
 # document globals
 # ----------------------------------------------------------------------
 
 DOC_SDI = 1
```

### Comparing `wbBase-0.2.2/Lib/wbBase/document/manager.py` & `wbBase-0.2.3/Lib/wbBase/document/manager.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.2/Lib/wbBase/document/notebook.py` & `wbBase-0.2.3/Lib/wbBase/document/notebook.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.2/Lib/wbBase/document/template.py` & `wbBase-0.2.3/Lib/wbBase/document/template.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.2/Lib/wbBase/document/view.py` & `wbBase-0.2.3/Lib/wbBase/document/view.py`

 * *Files 14% similar despite different names*

```diff
@@ -110,144 +110,124 @@
         member function, the ``View`` can create a :class:`DocChildFrame` or
         a derived class. This :class:`DocChildFrame` provides user
         interface elements to view and/or edit the contents of the wxDocument.
 
         By default, simply returns true. If the function returns false, the
         view will be deleted.
         """
-        # dbg(f'View.OnCreate(doc="{doc}", flags={flags})', indent=1)
         if self.frameType is None:
-            # dbg("View.OnCreate() -> failed: no frameType", indent=0)
             return False
         template = doc.template
         assert isinstance(template, DocumentTemplate)
         self._typeName = template.viewTypeName
         documentNotebook = self.documentNotebook
         documentNotebook.Freeze()
         self._frame = self.frameType(documentNotebook, doc, self)
         documentNotebook.AddPage(self._frame, doc.printableName, True, template.icon)
         documentNotebook.Thaw()
-        # dbg(indent=0)
         return True
 
     def OnClose(self, deleteWindow:bool=True) -> bool:
         """
         Implements closing behaviour. The default implementation calls
         :meth:`Document.Close` to close the associated document. Does not delete the
         view. The application may wish to do some cleaning up operations in
         this function, if a call to :meth:`Document::Close` succeeded. For example,
         if your application's all share the same window, you need to
         disassociate the window from the view and perhaps clear the window. If
         deleteWindow is true, delete the frame associated with the view.
         """
-        # dbg(f"View.OnClose(deleteWindow={deleteWindow})", indent=1)
         result = False
         if (
             self.document
             and len(self.document.views) == 1
             and not self.document.OnSaveModified()
         ):
-            # dbg(f"View.OnClose() returns {result}", indent=0)
             return result
         if self.document is None or self.document.RemoveView(self):
             self.Activate(False)
             if self.frame and deleteWindow:
                 index = self.pageIndex
                 # self.frame.Unlink()
                 if index is not None:
                     self.documentNotebook.DeletePage(index)
                 else:
                     self.frame.Destroy()
             self.Destroy()
             result = True
-        # dbg(f"View.OnClose() returns {result}", indent=0)
         return result
 
     def OnActivateView(self, activate, activeView, deactiveView):
         """
         Called when a view is activated by means of :meth:`View.Activate`. The
         default implementation does nothing.
         """
-        # dbg(f"View.OnActivateView({self}, activate={activate})", indent=1)
         i = self.pageIndex
         if i is not None and i != self.documentNotebook.Selection:
             self.documentNotebook.Selection = i
-        # dbg(indent=0)
 
     def OnClosingDocument(self):
         """
         Override this to clean up the view when the document is being closed.
         The default implementation does nothing.
         """
-        # dbg(f"View.OnClosingDocument()", indent=1)
         self.OnClose(deleteWindow=True)
-        # dbg(indent=0)
 
     def OnUpdate(self, sender, hint) -> bool:
         """
         Called when the view should be updated. sender is a pointer to the
         view that sent the update request, or None if no single view requested
         the update (for instance, when the document is opened). hint is as yet
         unused but may in future contain application-specific information for
         making updating more efficient.
         """
-        # dbg(f"View.OnUpdate(sender={sender}, hint={hint})", indent=1)
         if hint:
             if hint[0] == "modify":
                 # if dirty flag changed, update the view's displayed title
                 frame = self._frame
                 if frame and hasattr(frame, "OnTitleIsModified"):
                     frame.OnTitleIsModified()
-                    # dbg(f"View.OnUpdate() -> done return True", indent=0)
                     return True
-        # dbg(f"View.OnUpdate() -> done return False", indent=0)
         return False
 
 
     def OnChangeFilename(self) -> None:
         """
         Called when the filename has changed. The default implementation
         constructs a suitable title and sets the title of the view frame (if
         any).
         """
-        # dbg(f"View.OnChangeFilename()")
         frame = self._frame
         if frame:
             if self._document:
                 frame.title = self._document.printableName
 
     # -----------------------------------------------------------------------------
     # public methods
     # -----------------------------------------------------------------------------
 
     def Close(self, deleteWindow=True) -> bool:
         """
         Closes the view by calling :meth:`OnClose`. If deleteWindow is true, this
         function should delete the window associated with the view.
         """
-        # dbg("View.Close()", indent=1)
         result = self.OnClose(deleteWindow=deleteWindow)
-        # dbg(indent=0)
         return result
 
     def Activate(self, activate=True):
         """
         Call this from your view frame's OnActivate member to tell the
         framework which view is currently active. If your windowing system
         doesn't call OnActivate, you may need to call this function from
         OnMenuCommand or any place where you know the view must be active, and
         the framework will need to get the current view.
         """
-        # dbg(f"View.Activate({self}, activate={activate})", indent=1)
         if self.document and self.documentManager:
             self.OnActivateView(activate, self, self.documentManager.currentView)
             self.documentManager.ActivateView(self, activate)
-        # dbg(indent=0)
 
     def Destroy(self):
         """
         Destructor. Removes itself from the document's list of views.
         """
-        # dbg("View.Destroy", indent=1)
         if self._document:
             self._document.RemoveView(self)
-        # dbg(indent=0)
```

### Comparing `wbBase-0.2.2/Lib/wbBase/panelManager.py` & `wbBase-0.2.3/Lib/wbBase/panelManager.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.2/Lib/wbBase/pluginManager.py` & `wbBase-0.2.3/Lib/wbBase/pluginManager.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.2/Lib/wbBase/pluginManager_old.py` & `wbBase-0.2.3/Lib/wbBase/pluginManager_old.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.2/Lib/wbBase/scripting.py` & `wbBase-0.2.3/Lib/wbBase/scripting.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.2/Lib/wbBase/tools.py` & `wbBase-0.2.3/Lib/wbBase/tools.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.2/Lib/wbBase.egg-info/PKG-INFO` & `wbBase-0.2.3/Lib/wbBase.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wbBase
-Version: 0.2.2
+Version: 0.2.3
 Summary: Base package for WorkBench applications.
 Home-page: https://gitlab.com/workbench2/wbbase
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/wbbase
 Project-URL: Documentation, https://workbench2.gitlab.io/wbbase
 Project-URL: Tracker, https://gitlab.com/workbench2/wbbase/-/issues
```

### Comparing `wbBase-0.2.2/Lib/wbBase.egg-info/SOURCES.txt` & `wbBase-0.2.3/Lib/wbBase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.2/PKG-INFO` & `wbBase-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wbBase
-Version: 0.2.2
+Version: 0.2.3
 Summary: Base package for WorkBench applications.
 Home-page: https://gitlab.com/workbench2/wbbase
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/wbbase
 Project-URL: Documentation, https://workbench2.gitlab.io/wbbase
 Project-URL: Tracker, https://gitlab.com/workbench2/wbbase/-/issues
```

### Comparing `wbBase-0.2.2/README.md` & `wbBase-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.2/setup.cfg` & `wbBase-0.2.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.2.2
+current_version = 0.2.3
 commit = True
 tag = True
 tag_name = {new_version}
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)?
 serialize = 
 	{major}.{minor}.{patch}
```

