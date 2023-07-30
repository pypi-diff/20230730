# Comparing `tmp/blizzardwarcraftapi-0.2.4.tar.gz` & `tmp/blizzardwarcraftapi-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blizzardwarcraftapi-0.2.4.tar", max compression
+gzip compressed data, was "blizzardwarcraftapi-0.2.5.tar", max compression
```

## Comparing `blizzardwarcraftapi-0.2.4.tar` & `blizzardwarcraftapi-0.2.5.tar`

### file list

```diff
@@ -1,34 +1,36 @@
--rw-r--r--   0        0        0     1003 2023-07-02 12:46:15.807100 blizzardwarcraftapi-0.2.4/BlizzardWarcraftAPI/BlizzardAuthToken.py
--rw-r--r--   0        0        0     1871 2023-07-02 12:46:15.807100 blizzardwarcraftapi-0.2.4/BlizzardWarcraftAPI/BlizzardWarcraftAPI.py
--rw-r--r--   0        0        0      139 2023-07-02 12:46:15.807100 blizzardwarcraftapi-0.2.4/BlizzardWarcraftAPI/__init__.py
--rw-r--r--   0        0        0      609 2023-07-02 12:46:15.807100 blizzardwarcraftapi-0.2.4/BlizzardWarcraftAPI/data.py
--rw-r--r--   0        0        0      292 2023-07-02 12:46:15.807100 blizzardwarcraftapi-0.2.4/BlizzardWarcraftAPI/exceptions.py
--rw-r--r--   0        0        0     1935 2023-07-02 12:46:15.807100 blizzardwarcraftapi-0.2.4/BlizzardWarcraftAPI/modules/BlizzardWarcraftAPI_base.py
--rw-r--r--   0        0        0     1201 2023-07-02 12:46:15.807100 blizzardwarcraftapi-0.2.4/BlizzardWarcraftAPI/modules/__init__.py
--rw-r--r--   0        0        0     2195 2023-07-02 12:46:15.807100 blizzardwarcraftapi-0.2.4/BlizzardWarcraftAPI/modules/gameData/AchievementAPI.py
--rw-r--r--   0        0        0     1694 2023-07-02 12:46:15.807100 blizzardwarcraftapi-0.2.4/BlizzardWarcraftAPI/modules/gameData/AuctionHouseAPI.py
--rw-r--r--   0        0        0     2056 2023-07-02 12:46:15.807100 blizzardwarcraftapi-0.2.4/BlizzardWarcraftAPI/modules/gameData/ConnectedRealmAPI.py
--rw-r--r--   0        0        0     3764 2023-07-02 12:46:15.807100 blizzardwarcraftapi-0.2.4/BlizzardWarcraftAPI/modules/gameData/CreatureAPI.py
--rw-r--r--   0        0        0     1339 2023-07-02 12:46:15.807100 blizzardwarcraftapi-0.2.4/BlizzardWarcraftAPI/modules/gameData/GuildCrestAPI.py
--rw-r--r--   0        0        0      827 2023-07-02 12:46:15.807100 blizzardwarcraftapi-0.2.4/BlizzardWarcraftAPI/modules/gameData/HeirloomAPI.py
--rw-r--r--   0        0        0     3652 2023-07-02 12:46:15.807100 blizzardwarcraftapi-0.2.4/BlizzardWarcraftAPI/modules/gameData/ItemAPI.py
--rw-r--r--   0        0        0     3420 2023-07-02 12:46:15.807100 blizzardwarcraftapi-0.2.4/BlizzardWarcraftAPI/modules/gameData/JournalAPI.py
--rw-r--r--   0        0        0        0 2023-07-02 12:46:15.807100 blizzardwarcraftapi-0.2.4/BlizzardWarcraftAPI/modules/gameData/__init__.py
--rw-r--r--   0        0        0     4997 2023-07-02 12:46:15.807100 blizzardwarcraftapi-0.2.4/BlizzardWarcraftAPI/modules/profile/AccountProfileAPI.py
--rw-r--r--   0        0        0     1271 2023-07-02 12:46:15.807100 blizzardwarcraftapi-0.2.4/BlizzardWarcraftAPI/modules/profile/CharacterAchievementsAPI.py
--rw-r--r--   0        0        0      683 2023-07-02 12:46:15.807100 blizzardwarcraftapi-0.2.4/BlizzardWarcraftAPI/modules/profile/CharacterAppearanceAPI.py
--rw-r--r--   0        0        0     2965 2023-07-02 12:46:15.807100 blizzardwarcraftapi-0.2.4/BlizzardWarcraftAPI/modules/profile/CharacterCollectionsAPI.py
--rw-r--r--   0        0        0     1766 2023-07-02 12:46:15.807100 blizzardwarcraftapi-0.2.4/BlizzardWarcraftAPI/modules/profile/CharacterEncountersAPI.py
--rw-r--r--   0        0        0      670 2023-07-02 12:46:15.807100 blizzardwarcraftapi-0.2.4/BlizzardWarcraftAPI/modules/profile/CharacterEquipmentAPI.py
--rw-r--r--   0        0        0      746 2023-07-02 12:46:15.807100 blizzardwarcraftapi-0.2.4/BlizzardWarcraftAPI/modules/profile/CharacterHunterPetsAPI.py
--rw-r--r--   0        0        0      715 2023-07-02 12:46:15.807100 blizzardwarcraftapi-0.2.4/BlizzardWarcraftAPI/modules/profile/CharacterMediaAPI.py
--rw-r--r--   0        0        0     1544 2023-07-02 12:46:15.807100 blizzardwarcraftapi-0.2.4/BlizzardWarcraftAPI/modules/profile/CharacterMythicKeystoneProfile.py
--rw-r--r--   0        0        0      680 2023-07-02 12:46:15.807100 blizzardwarcraftapi-0.2.4/BlizzardWarcraftAPI/modules/profile/CharacterProfessionsAPI.py
--rw-r--r--   0        0        0     2138 2023-07-02 12:46:15.811100 blizzardwarcraftapi-0.2.4/BlizzardWarcraftAPI/modules/profile/CharacterProfileAPI.py
--rw-r--r--   0        0        0     1312 2023-07-02 12:46:15.811100 blizzardwarcraftapi-0.2.4/BlizzardWarcraftAPI/modules/profile/CharacterPvPAPI.py
--rw-r--r--   0        0        0        0 2023-07-02 12:46:15.811100 blizzardwarcraftapi-0.2.4/BlizzardWarcraftAPI/modules/profile/__init__.py
--rw-r--r--   0        0        0      421 2023-07-02 12:46:15.811100 blizzardwarcraftapi-0.2.4/BlizzardWarcraftAPI/urls.py
--rw-r--r--   0        0        0     1066 2023-07-02 12:46:15.811100 blizzardwarcraftapi-0.2.4/LICENSE
--rw-r--r--   0        0        0     2034 2023-07-02 12:46:15.811100 blizzardwarcraftapi-0.2.4/README.md
--rw-r--r--   0        0        0      916 2023-07-02 12:46:15.811100 blizzardwarcraftapi-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     2980 1970-01-01 00:00:00.000000 blizzardwarcraftapi-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1713 2023-07-30 11:08:22.266724 blizzardwarcraftapi-0.2.5/BlizzardWarcraftAPI/BlizzardAuthToken.py
+-rw-r--r--   0        0        0     2062 2023-07-30 11:08:22.266724 blizzardwarcraftapi-0.2.5/BlizzardWarcraftAPI/BlizzardWarcraftAPI.py
+-rw-r--r--   0        0        0      139 2023-07-30 11:08:22.266724 blizzardwarcraftapi-0.2.5/BlizzardWarcraftAPI/__init__.py
+-rw-r--r--   0        0        0      609 2023-07-30 11:08:22.266724 blizzardwarcraftapi-0.2.5/BlizzardWarcraftAPI/data.py
+-rw-r--r--   0        0        0      292 2023-07-30 11:08:22.266724 blizzardwarcraftapi-0.2.5/BlizzardWarcraftAPI/exceptions.py
+-rw-r--r--   0        0        0     1933 2023-07-30 11:08:22.266724 blizzardwarcraftapi-0.2.5/BlizzardWarcraftAPI/modules/BlizzardWarcraftAPI_base.py
+-rw-r--r--   0        0        0     1237 2023-07-30 11:08:22.266724 blizzardwarcraftapi-0.2.5/BlizzardWarcraftAPI/modules/__init__.py
+-rw-r--r--   0        0        0     2195 2023-07-30 11:08:22.266724 blizzardwarcraftapi-0.2.5/BlizzardWarcraftAPI/modules/gameData/AchievementAPI.py
+-rw-r--r--   0        0        0     1694 2023-07-30 11:08:22.266724 blizzardwarcraftapi-0.2.5/BlizzardWarcraftAPI/modules/gameData/AuctionHouseAPI.py
+-rw-r--r--   0        0        0     2056 2023-07-30 11:08:22.266724 blizzardwarcraftapi-0.2.5/BlizzardWarcraftAPI/modules/gameData/ConnectedRealmAPI.py
+-rw-r--r--   0        0        0     3764 2023-07-30 11:08:22.266724 blizzardwarcraftapi-0.2.5/BlizzardWarcraftAPI/modules/gameData/CreatureAPI.py
+-rw-r--r--   0        0        0     1339 2023-07-30 11:08:22.266724 blizzardwarcraftapi-0.2.5/BlizzardWarcraftAPI/modules/gameData/GuildCrestAPI.py
+-rw-r--r--   0        0        0      827 2023-07-30 11:08:22.266724 blizzardwarcraftapi-0.2.5/BlizzardWarcraftAPI/modules/gameData/HeirloomAPI.py
+-rw-r--r--   0        0        0     3652 2023-07-30 11:08:22.266724 blizzardwarcraftapi-0.2.5/BlizzardWarcraftAPI/modules/gameData/ItemAPI.py
+-rw-r--r--   0        0        0     3420 2023-07-30 11:08:22.266724 blizzardwarcraftapi-0.2.5/BlizzardWarcraftAPI/modules/gameData/JournalAPI.py
+-rw-r--r--   0        0        0        0 2023-07-30 11:08:22.270724 blizzardwarcraftapi-0.2.5/BlizzardWarcraftAPI/modules/gameData/__init__.py
+-rw-r--r--   0        0        0     4997 2023-07-30 11:08:22.270724 blizzardwarcraftapi-0.2.5/BlizzardWarcraftAPI/modules/profile/AccountProfileAPI.py
+-rw-r--r--   0        0        0     1271 2023-07-30 11:08:22.270724 blizzardwarcraftapi-0.2.5/BlizzardWarcraftAPI/modules/profile/CharacterAchievementsAPI.py
+-rw-r--r--   0        0        0      683 2023-07-30 11:08:22.270724 blizzardwarcraftapi-0.2.5/BlizzardWarcraftAPI/modules/profile/CharacterAppearanceAPI.py
+-rw-r--r--   0        0        0     2965 2023-07-30 11:08:22.270724 blizzardwarcraftapi-0.2.5/BlizzardWarcraftAPI/modules/profile/CharacterCollectionsAPI.py
+-rw-r--r--   0        0        0     1766 2023-07-30 11:08:22.270724 blizzardwarcraftapi-0.2.5/BlizzardWarcraftAPI/modules/profile/CharacterEncountersAPI.py
+-rw-r--r--   0        0        0      670 2023-07-30 11:08:22.270724 blizzardwarcraftapi-0.2.5/BlizzardWarcraftAPI/modules/profile/CharacterEquipmentAPI.py
+-rw-r--r--   0        0        0      746 2023-07-30 11:08:22.270724 blizzardwarcraftapi-0.2.5/BlizzardWarcraftAPI/modules/profile/CharacterHunterPetsAPI.py
+-rw-r--r--   0        0        0      715 2023-07-30 11:08:22.270724 blizzardwarcraftapi-0.2.5/BlizzardWarcraftAPI/modules/profile/CharacterMediaAPI.py
+-rw-r--r--   0        0        0     1544 2023-07-30 11:08:22.270724 blizzardwarcraftapi-0.2.5/BlizzardWarcraftAPI/modules/profile/CharacterMythicKeystoneProfile.py
+-rw-r--r--   0        0        0      680 2023-07-30 11:08:22.270724 blizzardwarcraftapi-0.2.5/BlizzardWarcraftAPI/modules/profile/CharacterProfessionsAPI.py
+-rw-r--r--   0        0        0     2138 2023-07-30 11:08:22.270724 blizzardwarcraftapi-0.2.5/BlizzardWarcraftAPI/modules/profile/CharacterProfileAPI.py
+-rw-r--r--   0        0        0     1312 2023-07-30 11:08:22.270724 blizzardwarcraftapi-0.2.5/BlizzardWarcraftAPI/modules/profile/CharacterPvPAPI.py
+-rw-r--r--   0        0        0        0 2023-07-30 11:08:22.270724 blizzardwarcraftapi-0.2.5/BlizzardWarcraftAPI/modules/profile/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-30 11:08:22.270724 blizzardwarcraftapi-0.2.5/BlizzardWarcraftAPI/modules/request/__init__.py
+-rw-r--r--   0        0        0      370 2023-07-30 11:08:22.270724 blizzardwarcraftapi-0.2.5/BlizzardWarcraftAPI/modules/request/href.py
+-rw-r--r--   0        0        0      421 2023-07-30 11:08:22.270724 blizzardwarcraftapi-0.2.5/BlizzardWarcraftAPI/urls.py
+-rw-r--r--   0        0        0     1066 2023-07-30 11:08:22.270724 blizzardwarcraftapi-0.2.5/LICENSE
+-rw-r--r--   0        0        0     2034 2023-07-30 11:08:22.270724 blizzardwarcraftapi-0.2.5/README.md
+-rw-r--r--   0        0        0      916 2023-07-30 11:08:22.270724 blizzardwarcraftapi-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     2980 1970-01-01 00:00:00.000000 blizzardwarcraftapi-0.2.5/PKG-INFO
```

### Comparing `blizzardwarcraftapi-0.2.4/BlizzardWarcraftAPI/BlizzardWarcraftAPI.py` & `blizzardwarcraftapi-0.2.5/BlizzardWarcraftAPI/BlizzardWarcraftAPI.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,7 +37,13 @@
                   CharacterProfileAPI, CharacterPvPAPI):
         """
         The World of Warcraft profile APIs listed below encompass profile game data.
         https://develop.battle.net/documentation/world-of-warcraft/profile-apis
         """
         def __init__(self):
             super().__init__(BlizzardWarcraftAPI.BlizzardAuthToken, BlizzardWarcraftAPI.region, BlizzardWarcraftAPI.locale)
+
+    class Request(hrefAPI):
+        
+        def __init__(self):
+            super().__init__(BlizzardWarcraftAPI.BlizzardAuthToken, BlizzardWarcraftAPI.region, BlizzardWarcraftAPI.locale)
+
```

### Comparing `blizzardwarcraftapi-0.2.4/BlizzardWarcraftAPI/data.py` & `blizzardwarcraftapi-0.2.5/BlizzardWarcraftAPI/data.py`

 * *Files identical despite different names*

### Comparing `blizzardwarcraftapi-0.2.4/BlizzardWarcraftAPI/modules/BlizzardWarcraftAPI_base.py` & `blizzardwarcraftapi-0.2.5/BlizzardWarcraftAPI/modules/BlizzardWarcraftAPI_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import requests
 from ..data import region_data, locales_region_data
 from ..exceptions import BlizzardWarcraftApiError
 from ..urls import URL_TOKEN_VALIDATION
 
 
-class BlizzardWarcraftAPI():
+class BlizzardWarcraftAPI:
     @staticmethod
     def response(url, param):
         resp = requests.get(url, params=param)
         return resp.json()
 
     @staticmethod
     def __valid_region(region):
```

### Comparing `blizzardwarcraftapi-0.2.4/BlizzardWarcraftAPI/modules/__init__.py` & `blizzardwarcraftapi-0.2.5/BlizzardWarcraftAPI/modules/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,8 +14,10 @@
 from .profile.CharacterEquipmentAPI import CharacterEquipmentAPI
 from .profile.CharacterHunterPetsAPI import CharacterHunterPetsAPI
 from .profile.CharacterMediaAPI import CharacterMediaAPI
 from .profile.CharacterProfessionsAPI import CharacterProfessionsAPI
 from .profile.CharacterMythicKeystoneProfile import CharacterMythicKeystoneProfile
 from .profile.AccountProfileAPI import AccountProfileAPI
 from .profile.CharacterProfileAPI import CharacterProfileAPI
-from .profile.CharacterPvPAPI import CharacterPvPAPI
+from .profile.CharacterPvPAPI import CharacterPvPAPI
+
+from .request.href import hrefAPI
```

### Comparing `blizzardwarcraftapi-0.2.4/BlizzardWarcraftAPI/modules/gameData/AchievementAPI.py` & `blizzardwarcraftapi-0.2.5/BlizzardWarcraftAPI/modules/gameData/AchievementAPI.py`

 * *Files identical despite different names*

### Comparing `blizzardwarcraftapi-0.2.4/BlizzardWarcraftAPI/modules/gameData/AuctionHouseAPI.py` & `blizzardwarcraftapi-0.2.5/BlizzardWarcraftAPI/modules/gameData/AuctionHouseAPI.py`

 * *Files identical despite different names*

### Comparing `blizzardwarcraftapi-0.2.4/BlizzardWarcraftAPI/modules/gameData/ConnectedRealmAPI.py` & `blizzardwarcraftapi-0.2.5/BlizzardWarcraftAPI/modules/gameData/ConnectedRealmAPI.py`

 * *Files identical despite different names*

### Comparing `blizzardwarcraftapi-0.2.4/BlizzardWarcraftAPI/modules/gameData/CreatureAPI.py` & `blizzardwarcraftapi-0.2.5/BlizzardWarcraftAPI/modules/gameData/CreatureAPI.py`

 * *Files identical despite different names*

### Comparing `blizzardwarcraftapi-0.2.4/BlizzardWarcraftAPI/modules/gameData/GuildCrestAPI.py` & `blizzardwarcraftapi-0.2.5/BlizzardWarcraftAPI/modules/gameData/GuildCrestAPI.py`

 * *Files identical despite different names*

### Comparing `blizzardwarcraftapi-0.2.4/BlizzardWarcraftAPI/modules/gameData/HeirloomAPI.py` & `blizzardwarcraftapi-0.2.5/BlizzardWarcraftAPI/modules/gameData/HeirloomAPI.py`

 * *Files identical despite different names*

### Comparing `blizzardwarcraftapi-0.2.4/BlizzardWarcraftAPI/modules/gameData/ItemAPI.py` & `blizzardwarcraftapi-0.2.5/BlizzardWarcraftAPI/modules/gameData/ItemAPI.py`

 * *Files identical despite different names*

### Comparing `blizzardwarcraftapi-0.2.4/BlizzardWarcraftAPI/modules/gameData/JournalAPI.py` & `blizzardwarcraftapi-0.2.5/BlizzardWarcraftAPI/modules/gameData/JournalAPI.py`

 * *Files identical despite different names*

### Comparing `blizzardwarcraftapi-0.2.4/BlizzardWarcraftAPI/modules/profile/AccountProfileAPI.py` & `blizzardwarcraftapi-0.2.5/BlizzardWarcraftAPI/modules/profile/AccountProfileAPI.py`

 * *Files identical despite different names*

### Comparing `blizzardwarcraftapi-0.2.4/BlizzardWarcraftAPI/modules/profile/CharacterAchievementsAPI.py` & `blizzardwarcraftapi-0.2.5/BlizzardWarcraftAPI/modules/profile/CharacterAchievementsAPI.py`

 * *Files identical despite different names*

### Comparing `blizzardwarcraftapi-0.2.4/BlizzardWarcraftAPI/modules/profile/CharacterAppearanceAPI.py` & `blizzardwarcraftapi-0.2.5/BlizzardWarcraftAPI/modules/profile/CharacterAppearanceAPI.py`

 * *Files identical despite different names*

### Comparing `blizzardwarcraftapi-0.2.4/BlizzardWarcraftAPI/modules/profile/CharacterCollectionsAPI.py` & `blizzardwarcraftapi-0.2.5/BlizzardWarcraftAPI/modules/profile/CharacterCollectionsAPI.py`

 * *Files identical despite different names*

### Comparing `blizzardwarcraftapi-0.2.4/BlizzardWarcraftAPI/modules/profile/CharacterEncountersAPI.py` & `blizzardwarcraftapi-0.2.5/BlizzardWarcraftAPI/modules/profile/CharacterEncountersAPI.py`

 * *Files identical despite different names*

### Comparing `blizzardwarcraftapi-0.2.4/BlizzardWarcraftAPI/modules/profile/CharacterEquipmentAPI.py` & `blizzardwarcraftapi-0.2.5/BlizzardWarcraftAPI/modules/profile/CharacterEquipmentAPI.py`

 * *Files identical despite different names*

### Comparing `blizzardwarcraftapi-0.2.4/BlizzardWarcraftAPI/modules/profile/CharacterHunterPetsAPI.py` & `blizzardwarcraftapi-0.2.5/BlizzardWarcraftAPI/modules/profile/CharacterHunterPetsAPI.py`

 * *Files identical despite different names*

### Comparing `blizzardwarcraftapi-0.2.4/BlizzardWarcraftAPI/modules/profile/CharacterMediaAPI.py` & `blizzardwarcraftapi-0.2.5/BlizzardWarcraftAPI/modules/profile/CharacterMediaAPI.py`

 * *Files identical despite different names*

### Comparing `blizzardwarcraftapi-0.2.4/BlizzardWarcraftAPI/modules/profile/CharacterMythicKeystoneProfile.py` & `blizzardwarcraftapi-0.2.5/BlizzardWarcraftAPI/modules/profile/CharacterMythicKeystoneProfile.py`

 * *Files identical despite different names*

### Comparing `blizzardwarcraftapi-0.2.4/BlizzardWarcraftAPI/modules/profile/CharacterProfessionsAPI.py` & `blizzardwarcraftapi-0.2.5/BlizzardWarcraftAPI/modules/profile/CharacterProfessionsAPI.py`

 * *Files identical despite different names*

### Comparing `blizzardwarcraftapi-0.2.4/BlizzardWarcraftAPI/modules/profile/CharacterProfileAPI.py` & `blizzardwarcraftapi-0.2.5/BlizzardWarcraftAPI/modules/profile/CharacterProfileAPI.py`

 * *Files identical despite different names*

### Comparing `blizzardwarcraftapi-0.2.4/BlizzardWarcraftAPI/modules/profile/CharacterPvPAPI.py` & `blizzardwarcraftapi-0.2.5/BlizzardWarcraftAPI/modules/profile/CharacterPvPAPI.py`

 * *Files identical despite different names*

### Comparing `blizzardwarcraftapi-0.2.4/LICENSE` & `blizzardwarcraftapi-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `blizzardwarcraftapi-0.2.4/README.md` & `blizzardwarcraftapi-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `blizzardwarcraftapi-0.2.4/pyproject.toml` & `blizzardwarcraftapi-0.2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "BlizzardWarcraftAPI"
-version = "0.2.4"
+version = "0.2.5"
 authors = ["Angeloffy <angeloffy.work@gmail.com>"]
 maintainers = [
     "Angeloffy <angeloffy.work@gmail.com>",
     "Kotorkovsciy <kotorkovsciy@gmail.com>"
 ]
 description = "Warcraft API"
 readme = "README.md"
```

### Comparing `blizzardwarcraftapi-0.2.4/PKG-INFO` & `blizzardwarcraftapi-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blizzardwarcraftapi
-Version: 0.2.4
+Version: 0.2.5
 Summary: Warcraft API
 Home-page: https://github.com/Angeloffy/BlizzardWarcraftAPI/tree/main
 License: MIT
 Author: Angeloffy
 Author-email: angeloffy.work@gmail.com
 Maintainer: Angeloffy
 Maintainer-email: angeloffy.work@gmail.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: blizzardwarcraftapi Version: 0.2.4 Summary:
+Metadata-Version: 2.1 Name: blizzardwarcraftapi Version: 0.2.5 Summary:
 Warcraft API Home-page: https://github.com/Angeloffy/BlizzardWarcraftAPI/tree/
 main License: MIT Author: Angeloffy Author-email: angeloffy.work@gmail.com
 Maintainer: Angeloffy Maintainer-email: angeloffy.work@gmail.com Requires-
 Python: >=3.9,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

