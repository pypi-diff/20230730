# Comparing `tmp/pmdsky_debug_py-7.0.5-py3-none-any.whl.zip` & `tmp/pmdsky_debug_py-7.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 881682 bytes, number of entries: 14
--rw-r--r--  2.0 unx     1831 b- defN 23-Jul-23 04:24 pmdsky_debug_py/__init__.py
--rw-r--r--  2.0 unx       30 b- defN 23-Jul-23 04:24 pmdsky_debug_py/_release.py
--rw-r--r--  2.0 unx   752071 b- defN 23-Jul-23 04:24 pmdsky_debug_py/eu.py
--rw-r--r--  2.0 unx   718165 b- defN 23-Jul-23 04:24 pmdsky_debug_py/eu_itcm.py
--rw-r--r--  2.0 unx   739215 b- defN 23-Jul-23 04:24 pmdsky_debug_py/jp.py
--rw-r--r--  2.0 unx   718165 b- defN 23-Jul-23 04:24 pmdsky_debug_py/jp_itcm.py
--rw-r--r--  2.0 unx   759453 b- defN 23-Jul-23 04:24 pmdsky_debug_py/na.py
--rw-r--r--  2.0 unx   718176 b- defN 23-Jul-23 04:24 pmdsky_debug_py/na_itcm.py
--rw-r--r--  2.0 unx   252390 b- defN 23-Jul-23 04:24 pmdsky_debug_py/protocol.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-23 04:24 pmdsky_debug_py/py.typed
--rw-r--r--  2.0 unx     1320 b- defN 23-Jul-23 04:24 pmdsky_debug_py-7.0.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-23 04:24 pmdsky_debug_py-7.0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Jul-23 04:24 pmdsky_debug_py-7.0.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1155 b- defN 23-Jul-23 04:24 pmdsky_debug_py-7.0.5.dist-info/RECORD
-14 files, 4662079 bytes uncompressed, 879784 bytes compressed:  81.1%
+Zip file size: 885527 bytes, number of entries: 14
+-rw-r--r--  2.0 unx     1831 b- defN 23-Jul-30 04:23 pmdsky_debug_py/__init__.py
+-rw-r--r--  2.0 unx       30 b- defN 23-Jul-30 04:23 pmdsky_debug_py/_release.py
+-rw-r--r--  2.0 unx   754662 b- defN 23-Jul-30 04:23 pmdsky_debug_py/eu.py
+-rw-r--r--  2.0 unx   720673 b- defN 23-Jul-30 04:23 pmdsky_debug_py/eu_itcm.py
+-rw-r--r--  2.0 unx   741723 b- defN 23-Jul-30 04:23 pmdsky_debug_py/jp.py
+-rw-r--r--  2.0 unx   720673 b- defN 23-Jul-30 04:23 pmdsky_debug_py/jp_itcm.py
+-rw-r--r--  2.0 unx   762044 b- defN 23-Jul-30 04:23 pmdsky_debug_py/na.py
+-rw-r--r--  2.0 unx   720684 b- defN 23-Jul-30 04:23 pmdsky_debug_py/na_itcm.py
+-rw-r--r--  2.0 unx   253000 b- defN 23-Jul-30 04:23 pmdsky_debug_py/protocol.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-30 04:23 pmdsky_debug_py/py.typed
+-rw-r--r--  2.0 unx     1320 b- defN 23-Jul-30 04:23 pmdsky_debug_py-7.0.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-30 04:23 pmdsky_debug_py-7.0.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Jul-30 04:23 pmdsky_debug_py-7.0.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1155 b- defN 23-Jul-30 04:23 pmdsky_debug_py-7.0.6.dist-info/RECORD
+14 files, 4677903 bytes uncompressed, 883629 bytes compressed:  81.1%
```

## zipnote {}

```diff
@@ -24,20 +24,20 @@
 
 Filename: pmdsky_debug_py/protocol.py
 Comment: 
 
 Filename: pmdsky_debug_py/py.typed
 Comment: 
 
-Filename: pmdsky_debug_py-7.0.5.dist-info/METADATA
+Filename: pmdsky_debug_py-7.0.6.dist-info/METADATA
 Comment: 
 
-Filename: pmdsky_debug_py-7.0.5.dist-info/WHEEL
+Filename: pmdsky_debug_py-7.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: pmdsky_debug_py-7.0.5.dist-info/top_level.txt
+Filename: pmdsky_debug_py-7.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: pmdsky_debug_py-7.0.5.dist-info/RECORD
+Filename: pmdsky_debug_py-7.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pmdsky_debug_py/_release.py

```diff
@@ -1 +1 @@
-RELEASE = "v0.7.0+66b147366a"
+RELEASE = "v0.7.0+13fdd590a2"
```

## pmdsky_debug_py/eu.py

```diff
@@ -4679,15 +4679,15 @@
         "Note: unverified, ported from Irdkwia's notes\n\nr0: id\nreturn: speed status",
     )
 
     GetMobilityType = Symbol(
         [0x52BAC],
         [0x2052BAC],
         None,
-        "Gets the mobility type for a given monster.\n\nr0: monster ID\nreturn:"
+        "Gets the mobility type for a given monster species.\n\nr0: species ID\nreturn:"
         " mobility type",
     )
 
     GetRegenSpeed = Symbol(
         [0x52BC8],
         [0x2052BC8],
         None,
@@ -10541,14 +10541,24 @@
         [0x22C0858],
         None,
         "Note: unverified, ported from Irdkwia's notes\n\nr0: move_id\nreturn:"
         " anim_ent_ptr (This might be a mistake? It seems to be an integer, not a"
         " pointer)",
     )
 
+    IsBackgroundTileset = Symbol(
+        [0x5B0C],
+        [0x22C2ECC],
+        None,
+        "Given a tileset ID, returns whether it's a background or a regular"
+        " tileset\n\nIn particular, returns r0 >= 0xAA\n\nr0: Tileset ID\nreturn: True"
+        " if the tileset ID corresponds to a background, false if it corresponds to a"
+        " regular tileset",
+    )
+
     CheckEndDungeon = Symbol(
         [0x5E24],
         [0x22C31E4],
         None,
         "Do the stuff when you lose in a dungeon.\n\nNote: unverified, ported from"
         " Irdkwia's notes\n\nr0: End condition code? Seems to control what tasks get"
         " run and what transition happens when the dungeon ends\nreturn: return code?",
@@ -16074,25 +16084,65 @@
         [0x22FFBF4],
         None,
         "Returns true if the monster has any status problem that prevents it from"
         " acting\n\nr0: Entity pointer\nreturn: True if the specified monster can't act"
         " because of a status problem, false otherwise.",
     )
 
+    GetMobilityTypeCheckSlip = Symbol(
+        [0x234D8],
+        [0x2300058],
+        None,
+        "Returns the mobility type of a monster species, accounting for"
+        " STATUS_SLIP.\n\nThe function also converts MOBILITY_LAVA and MOBILITY_WATER"
+        " to other values if required.\n\nr0: Monster species\nr1: True if the monster"
+        " can walk on water\nreturn: Mobility type",
+    )
+
+    GetMobilityTypeCheckSlipAndFloating = Symbol(
+        [0x23520],
+        [0x23000A0],
+        None,
+        "Returns the mobility type of a monster, accounting for STATUS_SLIP and the"
+        " result of a call to IsFloating.\n\nr0: Entity pointer\nr1: Monster"
+        " species\nreturn: Mobility type",
+    )
+
     IsInvalidSpawnTile = Symbol(
         [0x23570],
         [0x23000F0],
         None,
         "Checks if a monster cannot spawn on the given tile for some reason.\n\nReasons"
         " include:\n- There's another monster on the tile\n- The tile is an impassable"
         " wall\n- The monster does not have the required mobility to stand on the"
         " tile\n\nr0: monster ID\nr1: tile pointer\nreturn: true means the monster"
         " CANNOT spawn on this tile",
     )
 
+    GetMobilityTypeAfterIqSkills = Symbol(
+        [0x23774],
+        [0x23002F4],
+        None,
+        "Modifies the given mobility type to account for All-Terrain Hiker and Absolute"
+        " Mover, if the user has them.\n\nr0: Entity pointer\nr1: Mobility"
+        " type\nreturn: New mobility type, after accounting for the IQ skills mentioned"
+        " above",
+    )
+
+    CannotStandOnTile = Symbol(
+        [0x23B48],
+        [0x23006C8],
+        None,
+        "Checks if a given monster cannot stand on a given tile.\n\nReasons include:\n-"
+        " The coordinates of the tile are out of bounds\n- There's another monster on"
+        " the tile\n- The monster does not have the required mobility to stand on the"
+        " tile\n\nr0: Entity pointer\nr1: Tile pointer\nreturn: True if the monster"
+        " cannot stand on the specified tile, false if it can",
+    )
+
     CalcSpeedStage = Symbol(
         [0x23CA0],
         [0x2300820],
         None,
         "Calculates the speed stage of a monster from its speed up/down counters. The"
         " second parameter is the weight of each counter (how many stages it will"
         " add/remove), but appears to be always 1. \nTakes modifiers into account"
@@ -16263,24 +16313,24 @@
         [0x23018A4],
         None,
         "Checks if the given monster can move in the specified direction\n\nReturns"
         " false if any monster is standing on the target tile\n\nr0: Monster entity"
         " pointer\nr1: Direction to check\nreturn: bool",
     )
 
-    GetFinalMobilityType = Symbol(
+    GetDirectionalMobilityType = Symbol(
         [0x24DDC],
         [0x230195C],
         None,
         "Returns the mobility type of a monster, after accounting for things that could"
-        " affect it (like items or IQ skills)\n\nIf the specified direction is"
-        " DIR_NONE, direction checks are skipped. If it's not, MOBILITY_INTANGIBLE is"
-        " only returned if the direction is not diagonal.\n\nr0: Monster entity"
-        " pointer\nr1: Base mobility type\nr2: Direction of mobility\nreturn: Final"
-        " mobility type",
+        " affect it.\n\nList of checks: Mobile status, Mobile Scarf, All-Terrain Hiker"
+        " and Absolute Mover.\n\nIf the specified direction is DIR_NONE, direction"
+        " checks are skipped. If it's not, MOBILITY_INTANGIBLE is only returned if the"
+        " direction is not diagonal.\n\nr0: Monster entity pointer\nr1: Base mobility"
+        " type\nr2: Direction of mobility\nreturn: Final mobility type",
     )
 
     IsMonsterCornered = Symbol(
         [0x24FC4],
         [0x2301B44],
         None,
         "True if the given monster is cornered (it can't move in any direction)\n\nr0:"
@@ -18052,21 +18102,21 @@
         None,
         None,
         None,
         "Inflicts the Magnet Rise status condition on a target monster if"
         " possible.\n\nr0: user entity pointer\nr1: target entity pointer",
     )
 
-    HasConditionalGroundImmunity = Symbol(
+    IsFloating = Symbol(
         [0x3C92C],
         [0x23194AC],
         None,
-        "Checks if a monster is currently immune to Ground-type moves for reasons other"
-        " than typing and ability.\n\nThis includes checks for Gravity and Magnet"
-        " Rise.\n\nr0: entity pointer\nreturn: bool",
+        "Checks if a monster is currently floating for reasons other than its typing or"
+        " ability.\n\nIn particular, this checks for Gravity and Magnet Rise.\n\nr0:"
+        " entity pointer\nreturn: bool",
     )
 
     TryInflictSafeguardStatus = Symbol(
         None,
         None,
         None,
         "Inflicts the Safeguard status condition on a target monster if"
@@ -18598,14 +18648,23 @@
         [0x2321770],
         None,
         "Makes the target monster warp if possible.\n\nr0: user entity pointer\nr1:"
         " target entity pointer\nr2: warp type\nr3: position (if warp type is"
         " position-based)",
     )
 
+    EnsureCanStandCurrentTile = Symbol(
+        [0x44FEC],
+        [0x2321B6C],
+        None,
+        "Checks that the given monster is standing on a tile it can stand on given its"
+        " movement type, and warps it to a random location if it's not.\n\nr0: Entity"
+        " pointer",
+    )
+
     TryActivateNondamagingDefenderAbility = Symbol(
         None,
         None,
         None,
         "Applies the effects of a defender's ability on an attacker. After a move is"
         " used,\nthis function is called to see if any of the bitflags for an ability"
         " were set and\napplies the corresponding effect. (The way leech seed removes"
@@ -18979,14 +19038,22 @@
         [0x2336DA4],
         None,
         "Checks if the current fixed room on the dungeon generation info corresponds to"
         " a fixed, full-floor layout.\n\nThe first non-full-floor fixed room is 0xA5,"
         " which is for Sealed Chambers.\n\nreturn: bool",
     )
 
+    IsCurrentTilesetBackground = Symbol(
+        [0x5A254],
+        [0x2336DD4],
+        None,
+        "Calls IsBackgroundTileset with the current tileset ID\n\nreturn: True if the"
+        " current dungeon tileset is a background, false if it's a regular tileset.",
+    )
+
     TrySpawnGoldenChamber = Symbol(
         None,
         None,
         None,
         "Changes the tileset and fixed room id of the floor for the Golden Chamber if"
         " the floor should be a\nGolden Chamber.\n\nNo params.",
     )
```

## pmdsky_debug_py/eu_itcm.py

```diff
@@ -4511,15 +4511,15 @@
         "Note: unverified, ported from Irdkwia's notes\n\nr0: id\nreturn: speed status",
     )
 
     GetMobilityType = Symbol(
         None,
         None,
         None,
-        "Gets the mobility type for a given monster.\n\nr0: monster ID\nreturn:"
+        "Gets the mobility type for a given monster species.\n\nr0: species ID\nreturn:"
         " mobility type",
     )
 
     GetRegenSpeed = Symbol(
         None,
         None,
         None,
@@ -10283,14 +10283,24 @@
         None,
         None,
         "Note: unverified, ported from Irdkwia's notes\n\nr0: move_id\nreturn:"
         " anim_ent_ptr (This might be a mistake? It seems to be an integer, not a"
         " pointer)",
     )
 
+    IsBackgroundTileset = Symbol(
+        None,
+        None,
+        None,
+        "Given a tileset ID, returns whether it's a background or a regular"
+        " tileset\n\nIn particular, returns r0 >= 0xAA\n\nr0: Tileset ID\nreturn: True"
+        " if the tileset ID corresponds to a background, false if it corresponds to a"
+        " regular tileset",
+    )
+
     CheckEndDungeon = Symbol(
         None,
         None,
         None,
         "Do the stuff when you lose in a dungeon.\n\nNote: unverified, ported from"
         " Irdkwia's notes\n\nr0: End condition code? Seems to control what tasks get"
         " run and what transition happens when the dungeon ends\nreturn: return code?",
@@ -15584,25 +15594,65 @@
         None,
         None,
         "Returns true if the monster has any status problem that prevents it from"
         " acting\n\nr0: Entity pointer\nreturn: True if the specified monster can't act"
         " because of a status problem, false otherwise.",
     )
 
+    GetMobilityTypeCheckSlip = Symbol(
+        None,
+        None,
+        None,
+        "Returns the mobility type of a monster species, accounting for"
+        " STATUS_SLIP.\n\nThe function also converts MOBILITY_LAVA and MOBILITY_WATER"
+        " to other values if required.\n\nr0: Monster species\nr1: True if the monster"
+        " can walk on water\nreturn: Mobility type",
+    )
+
+    GetMobilityTypeCheckSlipAndFloating = Symbol(
+        None,
+        None,
+        None,
+        "Returns the mobility type of a monster, accounting for STATUS_SLIP and the"
+        " result of a call to IsFloating.\n\nr0: Entity pointer\nr1: Monster"
+        " species\nreturn: Mobility type",
+    )
+
     IsInvalidSpawnTile = Symbol(
         None,
         None,
         None,
         "Checks if a monster cannot spawn on the given tile for some reason.\n\nReasons"
         " include:\n- There's another monster on the tile\n- The tile is an impassable"
         " wall\n- The monster does not have the required mobility to stand on the"
         " tile\n\nr0: monster ID\nr1: tile pointer\nreturn: true means the monster"
         " CANNOT spawn on this tile",
     )
 
+    GetMobilityTypeAfterIqSkills = Symbol(
+        None,
+        None,
+        None,
+        "Modifies the given mobility type to account for All-Terrain Hiker and Absolute"
+        " Mover, if the user has them.\n\nr0: Entity pointer\nr1: Mobility"
+        " type\nreturn: New mobility type, after accounting for the IQ skills mentioned"
+        " above",
+    )
+
+    CannotStandOnTile = Symbol(
+        None,
+        None,
+        None,
+        "Checks if a given monster cannot stand on a given tile.\n\nReasons include:\n-"
+        " The coordinates of the tile are out of bounds\n- There's another monster on"
+        " the tile\n- The monster does not have the required mobility to stand on the"
+        " tile\n\nr0: Entity pointer\nr1: Tile pointer\nreturn: True if the monster"
+        " cannot stand on the specified tile, false if it can",
+    )
+
     CalcSpeedStage = Symbol(
         None,
         None,
         None,
         "Calculates the speed stage of a monster from its speed up/down counters. The"
         " second parameter is the weight of each counter (how many stages it will"
         " add/remove), but appears to be always 1. \nTakes modifiers into account"
@@ -15773,24 +15823,24 @@
         None,
         None,
         "Checks if the given monster can move in the specified direction\n\nReturns"
         " false if any monster is standing on the target tile\n\nr0: Monster entity"
         " pointer\nr1: Direction to check\nreturn: bool",
     )
 
-    GetFinalMobilityType = Symbol(
+    GetDirectionalMobilityType = Symbol(
         None,
         None,
         None,
         "Returns the mobility type of a monster, after accounting for things that could"
-        " affect it (like items or IQ skills)\n\nIf the specified direction is"
-        " DIR_NONE, direction checks are skipped. If it's not, MOBILITY_INTANGIBLE is"
-        " only returned if the direction is not diagonal.\n\nr0: Monster entity"
-        " pointer\nr1: Base mobility type\nr2: Direction of mobility\nreturn: Final"
-        " mobility type",
+        " affect it.\n\nList of checks: Mobile status, Mobile Scarf, All-Terrain Hiker"
+        " and Absolute Mover.\n\nIf the specified direction is DIR_NONE, direction"
+        " checks are skipped. If it's not, MOBILITY_INTANGIBLE is only returned if the"
+        " direction is not diagonal.\n\nr0: Monster entity pointer\nr1: Base mobility"
+        " type\nr2: Direction of mobility\nreturn: Final mobility type",
     )
 
     IsMonsterCornered = Symbol(
         None,
         None,
         None,
         "True if the given monster is cornered (it can't move in any direction)\n\nr0:"
@@ -17562,21 +17612,21 @@
         None,
         None,
         None,
         "Inflicts the Magnet Rise status condition on a target monster if"
         " possible.\n\nr0: user entity pointer\nr1: target entity pointer",
     )
 
-    HasConditionalGroundImmunity = Symbol(
+    IsFloating = Symbol(
         None,
         None,
         None,
-        "Checks if a monster is currently immune to Ground-type moves for reasons other"
-        " than typing and ability.\n\nThis includes checks for Gravity and Magnet"
-        " Rise.\n\nr0: entity pointer\nreturn: bool",
+        "Checks if a monster is currently floating for reasons other than its typing or"
+        " ability.\n\nIn particular, this checks for Gravity and Magnet Rise.\n\nr0:"
+        " entity pointer\nreturn: bool",
     )
 
     TryInflictSafeguardStatus = Symbol(
         None,
         None,
         None,
         "Inflicts the Safeguard status condition on a target monster if"
@@ -18108,14 +18158,23 @@
         None,
         None,
         "Makes the target monster warp if possible.\n\nr0: user entity pointer\nr1:"
         " target entity pointer\nr2: warp type\nr3: position (if warp type is"
         " position-based)",
     )
 
+    EnsureCanStandCurrentTile = Symbol(
+        None,
+        None,
+        None,
+        "Checks that the given monster is standing on a tile it can stand on given its"
+        " movement type, and warps it to a random location if it's not.\n\nr0: Entity"
+        " pointer",
+    )
+
     TryActivateNondamagingDefenderAbility = Symbol(
         None,
         None,
         None,
         "Applies the effects of a defender's ability on an attacker. After a move is"
         " used,\nthis function is called to see if any of the bitflags for an ability"
         " were set and\napplies the corresponding effect. (The way leech seed removes"
@@ -18483,14 +18542,22 @@
         None,
         None,
         "Checks if the current fixed room on the dungeon generation info corresponds to"
         " a fixed, full-floor layout.\n\nThe first non-full-floor fixed room is 0xA5,"
         " which is for Sealed Chambers.\n\nreturn: bool",
     )
 
+    IsCurrentTilesetBackground = Symbol(
+        None,
+        None,
+        None,
+        "Calls IsBackgroundTileset with the current tileset ID\n\nreturn: True if the"
+        " current dungeon tileset is a background, false if it's a regular tileset.",
+    )
+
     TrySpawnGoldenChamber = Symbol(
         None,
         None,
         None,
         "Changes the tileset and fixed room id of the floor for the Golden Chamber if"
         " the floor should be a\nGolden Chamber.\n\nNo params.",
     )
```

## pmdsky_debug_py/jp.py

```diff
@@ -4677,15 +4677,15 @@
         "Note: unverified, ported from Irdkwia's notes\n\nr0: id\nreturn: speed status",
     )
 
     GetMobilityType = Symbol(
         [0x52BAC],
         [0x2052BAC],
         None,
-        "Gets the mobility type for a given monster.\n\nr0: monster ID\nreturn:"
+        "Gets the mobility type for a given monster species.\n\nr0: species ID\nreturn:"
         " mobility type",
     )
 
     GetRegenSpeed = Symbol(
         [0x52BC8],
         [0x2052BC8],
         None,
@@ -10511,14 +10511,24 @@
         [0x22C16BC],
         None,
         "Note: unverified, ported from Irdkwia's notes\n\nr0: move_id\nreturn:"
         " anim_ent_ptr (This might be a mistake? It seems to be an integer, not a"
         " pointer)",
     )
 
+    IsBackgroundTileset = Symbol(
+        None,
+        None,
+        None,
+        "Given a tileset ID, returns whether it's a background or a regular"
+        " tileset\n\nIn particular, returns r0 >= 0xAA\n\nr0: Tileset ID\nreturn: True"
+        " if the tileset ID corresponds to a background, false if it corresponds to a"
+        " regular tileset",
+    )
+
     CheckEndDungeon = Symbol(
         [0x5D54],
         [0x22C3F74],
         None,
         "Do the stuff when you lose in a dungeon.\n\nNote: unverified, ported from"
         " Irdkwia's notes\n\nr0: End condition code? Seems to control what tasks get"
         " run and what transition happens when the dungeon ends\nreturn: return code?",
@@ -15831,25 +15841,65 @@
         [0x23005B8],
         None,
         "Returns true if the monster has any status problem that prevents it from"
         " acting\n\nr0: Entity pointer\nreturn: True if the specified monster can't act"
         " because of a status problem, false otherwise.",
     )
 
+    GetMobilityTypeCheckSlip = Symbol(
+        None,
+        None,
+        None,
+        "Returns the mobility type of a monster species, accounting for"
+        " STATUS_SLIP.\n\nThe function also converts MOBILITY_LAVA and MOBILITY_WATER"
+        " to other values if required.\n\nr0: Monster species\nr1: True if the monster"
+        " can walk on water\nreturn: Mobility type",
+    )
+
+    GetMobilityTypeCheckSlipAndFloating = Symbol(
+        None,
+        None,
+        None,
+        "Returns the mobility type of a monster, accounting for STATUS_SLIP and the"
+        " result of a call to IsFloating.\n\nr0: Entity pointer\nr1: Monster"
+        " species\nreturn: Mobility type",
+    )
+
     IsInvalidSpawnTile = Symbol(
         [0x231D4],
         [0x2300AB4],
         None,
         "Checks if a monster cannot spawn on the given tile for some reason.\n\nReasons"
         " include:\n- There's another monster on the tile\n- The tile is an impassable"
         " wall\n- The monster does not have the required mobility to stand on the"
         " tile\n\nr0: monster ID\nr1: tile pointer\nreturn: true means the monster"
         " CANNOT spawn on this tile",
     )
 
+    GetMobilityTypeAfterIqSkills = Symbol(
+        None,
+        None,
+        None,
+        "Modifies the given mobility type to account for All-Terrain Hiker and Absolute"
+        " Mover, if the user has them.\n\nr0: Entity pointer\nr1: Mobility"
+        " type\nreturn: New mobility type, after accounting for the IQ skills mentioned"
+        " above",
+    )
+
+    CannotStandOnTile = Symbol(
+        None,
+        None,
+        None,
+        "Checks if a given monster cannot stand on a given tile.\n\nReasons include:\n-"
+        " The coordinates of the tile are out of bounds\n- There's another monster on"
+        " the tile\n- The monster does not have the required mobility to stand on the"
+        " tile\n\nr0: Entity pointer\nr1: Tile pointer\nreturn: True if the monster"
+        " cannot stand on the specified tile, false if it can",
+    )
+
     CalcSpeedStage = Symbol(
         [0x23944],
         [0x2301224],
         None,
         "Calculates the speed stage of a monster from its speed up/down counters. The"
         " second parameter is the weight of each counter (how many stages it will"
         " add/remove), but appears to be always 1. \nTakes modifiers into account"
@@ -16020,24 +16070,24 @@
         None,
         None,
         "Checks if the given monster can move in the specified direction\n\nReturns"
         " false if any monster is standing on the target tile\n\nr0: Monster entity"
         " pointer\nr1: Direction to check\nreturn: bool",
     )
 
-    GetFinalMobilityType = Symbol(
+    GetDirectionalMobilityType = Symbol(
         None,
         None,
         None,
         "Returns the mobility type of a monster, after accounting for things that could"
-        " affect it (like items or IQ skills)\n\nIf the specified direction is"
-        " DIR_NONE, direction checks are skipped. If it's not, MOBILITY_INTANGIBLE is"
-        " only returned if the direction is not diagonal.\n\nr0: Monster entity"
-        " pointer\nr1: Base mobility type\nr2: Direction of mobility\nreturn: Final"
-        " mobility type",
+        " affect it.\n\nList of checks: Mobile status, Mobile Scarf, All-Terrain Hiker"
+        " and Absolute Mover.\n\nIf the specified direction is DIR_NONE, direction"
+        " checks are skipped. If it's not, MOBILITY_INTANGIBLE is only returned if the"
+        " direction is not diagonal.\n\nr0: Monster entity pointer\nr1: Base mobility"
+        " type\nr2: Direction of mobility\nreturn: Final mobility type",
     )
 
     IsMonsterCornered = Symbol(
         [0x24C3C],
         [0x230251C],
         None,
         "True if the given monster is cornered (it can't move in any direction)\n\nr0:"
@@ -17809,21 +17859,21 @@
         None,
         None,
         None,
         "Inflicts the Magnet Rise status condition on a target monster if"
         " possible.\n\nr0: user entity pointer\nr1: target entity pointer",
     )
 
-    HasConditionalGroundImmunity = Symbol(
+    IsFloating = Symbol(
         [0x3C63C],
         [0x2319F1C],
         None,
-        "Checks if a monster is currently immune to Ground-type moves for reasons other"
-        " than typing and ability.\n\nThis includes checks for Gravity and Magnet"
-        " Rise.\n\nr0: entity pointer\nreturn: bool",
+        "Checks if a monster is currently floating for reasons other than its typing or"
+        " ability.\n\nIn particular, this checks for Gravity and Magnet Rise.\n\nr0:"
+        " entity pointer\nreturn: bool",
     )
 
     TryInflictSafeguardStatus = Symbol(
         None,
         None,
         None,
         "Inflicts the Safeguard status condition on a target monster if"
@@ -18355,14 +18405,23 @@
         [0x23221B4],
         None,
         "Makes the target monster warp if possible.\n\nr0: user entity pointer\nr1:"
         " target entity pointer\nr2: warp type\nr3: position (if warp type is"
         " position-based)",
     )
 
+    EnsureCanStandCurrentTile = Symbol(
+        None,
+        None,
+        None,
+        "Checks that the given monster is standing on a tile it can stand on given its"
+        " movement type, and warps it to a random location if it's not.\n\nr0: Entity"
+        " pointer",
+    )
+
     TryActivateNondamagingDefenderAbility = Symbol(
         None,
         None,
         None,
         "Applies the effects of a defender's ability on an attacker. After a move is"
         " used,\nthis function is called to see if any of the bitflags for an ability"
         " were set and\napplies the corresponding effect. (The way leech seed removes"
@@ -18736,14 +18795,22 @@
         [0x23375A4],
         None,
         "Checks if the current fixed room on the dungeon generation info corresponds to"
         " a fixed, full-floor layout.\n\nThe first non-full-floor fixed room is 0xA5,"
         " which is for Sealed Chambers.\n\nreturn: bool",
     )
 
+    IsCurrentTilesetBackground = Symbol(
+        None,
+        None,
+        None,
+        "Calls IsBackgroundTileset with the current tileset ID\n\nreturn: True if the"
+        " current dungeon tileset is a background, false if it's a regular tileset.",
+    )
+
     TrySpawnGoldenChamber = Symbol(
         None,
         None,
         None,
         "Changes the tileset and fixed room id of the floor for the Golden Chamber if"
         " the floor should be a\nGolden Chamber.\n\nNo params.",
     )
```

## pmdsky_debug_py/jp_itcm.py

```diff
@@ -4511,15 +4511,15 @@
         "Note: unverified, ported from Irdkwia's notes\n\nr0: id\nreturn: speed status",
     )
 
     GetMobilityType = Symbol(
         None,
         None,
         None,
-        "Gets the mobility type for a given monster.\n\nr0: monster ID\nreturn:"
+        "Gets the mobility type for a given monster species.\n\nr0: species ID\nreturn:"
         " mobility type",
     )
 
     GetRegenSpeed = Symbol(
         None,
         None,
         None,
@@ -10283,14 +10283,24 @@
         None,
         None,
         "Note: unverified, ported from Irdkwia's notes\n\nr0: move_id\nreturn:"
         " anim_ent_ptr (This might be a mistake? It seems to be an integer, not a"
         " pointer)",
     )
 
+    IsBackgroundTileset = Symbol(
+        None,
+        None,
+        None,
+        "Given a tileset ID, returns whether it's a background or a regular"
+        " tileset\n\nIn particular, returns r0 >= 0xAA\n\nr0: Tileset ID\nreturn: True"
+        " if the tileset ID corresponds to a background, false if it corresponds to a"
+        " regular tileset",
+    )
+
     CheckEndDungeon = Symbol(
         None,
         None,
         None,
         "Do the stuff when you lose in a dungeon.\n\nNote: unverified, ported from"
         " Irdkwia's notes\n\nr0: End condition code? Seems to control what tasks get"
         " run and what transition happens when the dungeon ends\nreturn: return code?",
@@ -15584,25 +15594,65 @@
         None,
         None,
         "Returns true if the monster has any status problem that prevents it from"
         " acting\n\nr0: Entity pointer\nreturn: True if the specified monster can't act"
         " because of a status problem, false otherwise.",
     )
 
+    GetMobilityTypeCheckSlip = Symbol(
+        None,
+        None,
+        None,
+        "Returns the mobility type of a monster species, accounting for"
+        " STATUS_SLIP.\n\nThe function also converts MOBILITY_LAVA and MOBILITY_WATER"
+        " to other values if required.\n\nr0: Monster species\nr1: True if the monster"
+        " can walk on water\nreturn: Mobility type",
+    )
+
+    GetMobilityTypeCheckSlipAndFloating = Symbol(
+        None,
+        None,
+        None,
+        "Returns the mobility type of a monster, accounting for STATUS_SLIP and the"
+        " result of a call to IsFloating.\n\nr0: Entity pointer\nr1: Monster"
+        " species\nreturn: Mobility type",
+    )
+
     IsInvalidSpawnTile = Symbol(
         None,
         None,
         None,
         "Checks if a monster cannot spawn on the given tile for some reason.\n\nReasons"
         " include:\n- There's another monster on the tile\n- The tile is an impassable"
         " wall\n- The monster does not have the required mobility to stand on the"
         " tile\n\nr0: monster ID\nr1: tile pointer\nreturn: true means the monster"
         " CANNOT spawn on this tile",
     )
 
+    GetMobilityTypeAfterIqSkills = Symbol(
+        None,
+        None,
+        None,
+        "Modifies the given mobility type to account for All-Terrain Hiker and Absolute"
+        " Mover, if the user has them.\n\nr0: Entity pointer\nr1: Mobility"
+        " type\nreturn: New mobility type, after accounting for the IQ skills mentioned"
+        " above",
+    )
+
+    CannotStandOnTile = Symbol(
+        None,
+        None,
+        None,
+        "Checks if a given monster cannot stand on a given tile.\n\nReasons include:\n-"
+        " The coordinates of the tile are out of bounds\n- There's another monster on"
+        " the tile\n- The monster does not have the required mobility to stand on the"
+        " tile\n\nr0: Entity pointer\nr1: Tile pointer\nreturn: True if the monster"
+        " cannot stand on the specified tile, false if it can",
+    )
+
     CalcSpeedStage = Symbol(
         None,
         None,
         None,
         "Calculates the speed stage of a monster from its speed up/down counters. The"
         " second parameter is the weight of each counter (how many stages it will"
         " add/remove), but appears to be always 1. \nTakes modifiers into account"
@@ -15773,24 +15823,24 @@
         None,
         None,
         "Checks if the given monster can move in the specified direction\n\nReturns"
         " false if any monster is standing on the target tile\n\nr0: Monster entity"
         " pointer\nr1: Direction to check\nreturn: bool",
     )
 
-    GetFinalMobilityType = Symbol(
+    GetDirectionalMobilityType = Symbol(
         None,
         None,
         None,
         "Returns the mobility type of a monster, after accounting for things that could"
-        " affect it (like items or IQ skills)\n\nIf the specified direction is"
-        " DIR_NONE, direction checks are skipped. If it's not, MOBILITY_INTANGIBLE is"
-        " only returned if the direction is not diagonal.\n\nr0: Monster entity"
-        " pointer\nr1: Base mobility type\nr2: Direction of mobility\nreturn: Final"
-        " mobility type",
+        " affect it.\n\nList of checks: Mobile status, Mobile Scarf, All-Terrain Hiker"
+        " and Absolute Mover.\n\nIf the specified direction is DIR_NONE, direction"
+        " checks are skipped. If it's not, MOBILITY_INTANGIBLE is only returned if the"
+        " direction is not diagonal.\n\nr0: Monster entity pointer\nr1: Base mobility"
+        " type\nr2: Direction of mobility\nreturn: Final mobility type",
     )
 
     IsMonsterCornered = Symbol(
         None,
         None,
         None,
         "True if the given monster is cornered (it can't move in any direction)\n\nr0:"
@@ -17562,21 +17612,21 @@
         None,
         None,
         None,
         "Inflicts the Magnet Rise status condition on a target monster if"
         " possible.\n\nr0: user entity pointer\nr1: target entity pointer",
     )
 
-    HasConditionalGroundImmunity = Symbol(
+    IsFloating = Symbol(
         None,
         None,
         None,
-        "Checks if a monster is currently immune to Ground-type moves for reasons other"
-        " than typing and ability.\n\nThis includes checks for Gravity and Magnet"
-        " Rise.\n\nr0: entity pointer\nreturn: bool",
+        "Checks if a monster is currently floating for reasons other than its typing or"
+        " ability.\n\nIn particular, this checks for Gravity and Magnet Rise.\n\nr0:"
+        " entity pointer\nreturn: bool",
     )
 
     TryInflictSafeguardStatus = Symbol(
         None,
         None,
         None,
         "Inflicts the Safeguard status condition on a target monster if"
@@ -18108,14 +18158,23 @@
         None,
         None,
         "Makes the target monster warp if possible.\n\nr0: user entity pointer\nr1:"
         " target entity pointer\nr2: warp type\nr3: position (if warp type is"
         " position-based)",
     )
 
+    EnsureCanStandCurrentTile = Symbol(
+        None,
+        None,
+        None,
+        "Checks that the given monster is standing on a tile it can stand on given its"
+        " movement type, and warps it to a random location if it's not.\n\nr0: Entity"
+        " pointer",
+    )
+
     TryActivateNondamagingDefenderAbility = Symbol(
         None,
         None,
         None,
         "Applies the effects of a defender's ability on an attacker. After a move is"
         " used,\nthis function is called to see if any of the bitflags for an ability"
         " were set and\napplies the corresponding effect. (The way leech seed removes"
@@ -18483,14 +18542,22 @@
         None,
         None,
         "Checks if the current fixed room on the dungeon generation info corresponds to"
         " a fixed, full-floor layout.\n\nThe first non-full-floor fixed room is 0xA5,"
         " which is for Sealed Chambers.\n\nreturn: bool",
     )
 
+    IsCurrentTilesetBackground = Symbol(
+        None,
+        None,
+        None,
+        "Calls IsBackgroundTileset with the current tileset ID\n\nreturn: True if the"
+        " current dungeon tileset is a background, false if it's a regular tileset.",
+    )
+
     TrySpawnGoldenChamber = Symbol(
         None,
         None,
         None,
         "Changes the tileset and fixed room id of the floor for the Golden Chamber if"
         " the floor should be a\nGolden Chamber.\n\nNo params.",
     )
```

## pmdsky_debug_py/na.py

```diff
@@ -4679,15 +4679,15 @@
         "Note: unverified, ported from Irdkwia's notes\n\nr0: id\nreturn: speed status",
     )
 
     GetMobilityType = Symbol(
         [0x52874],
         [0x2052874],
         None,
-        "Gets the mobility type for a given monster.\n\nr0: monster ID\nreturn:"
+        "Gets the mobility type for a given monster species.\n\nr0: species ID\nreturn:"
         " mobility type",
     )
 
     GetRegenSpeed = Symbol(
         [0x52890],
         [0x2052890],
         None,
@@ -10549,14 +10549,24 @@
         [0x22BFF18],
         None,
         "Note: unverified, ported from Irdkwia's notes\n\nr0: move_id\nreturn:"
         " anim_ent_ptr (This might be a mistake? It seems to be an integer, not a"
         " pointer)",
     )
 
+    IsBackgroundTileset = Symbol(
+        [0x5AF4],
+        [0x22C2574],
+        None,
+        "Given a tileset ID, returns whether it's a background or a regular"
+        " tileset\n\nIn particular, returns r0 >= 0xAA\n\nr0: Tileset ID\nreturn: True"
+        " if the tileset ID corresponds to a background, false if it corresponds to a"
+        " regular tileset",
+    )
+
     CheckEndDungeon = Symbol(
         [0x5E0C],
         [0x22C288C],
         None,
         "Do the stuff when you lose in a dungeon.\n\nNote: unverified, ported from"
         " Irdkwia's notes\n\nr0: End condition code? Seems to control what tasks get"
         " run and what transition happens when the dungeon ends\nreturn: return code?",
@@ -16158,25 +16168,65 @@
         [0x22FF1C8],
         None,
         "Returns true if the monster has any status problem that prevents it from"
         " acting\n\nr0: Entity pointer\nreturn: True if the specified monster can't act"
         " because of a status problem, false otherwise.",
     )
 
+    GetMobilityTypeCheckSlip = Symbol(
+        [0x233EC],
+        [0x22FF62C],
+        None,
+        "Returns the mobility type of a monster species, accounting for"
+        " STATUS_SLIP.\n\nThe function also converts MOBILITY_LAVA and MOBILITY_WATER"
+        " to other values if required.\n\nr0: Monster species\nr1: True if the monster"
+        " can walk on water\nreturn: Mobility type",
+    )
+
+    GetMobilityTypeCheckSlipAndFloating = Symbol(
+        [0x23434],
+        [0x22FF674],
+        None,
+        "Returns the mobility type of a monster, accounting for STATUS_SLIP and the"
+        " result of a call to IsFloating.\n\nr0: Entity pointer\nr1: Monster"
+        " species\nreturn: Mobility type",
+    )
+
     IsInvalidSpawnTile = Symbol(
         [0x23484],
         [0x22FF6C4],
         None,
         "Checks if a monster cannot spawn on the given tile for some reason.\n\nReasons"
         " include:\n- There's another monster on the tile\n- The tile is an impassable"
         " wall\n- The monster does not have the required mobility to stand on the"
         " tile\n\nr0: monster ID\nr1: tile pointer\nreturn: true means the monster"
         " CANNOT spawn on this tile",
     )
 
+    GetMobilityTypeAfterIqSkills = Symbol(
+        [0x23688],
+        [0x22FF8C8],
+        None,
+        "Modifies the given mobility type to account for All-Terrain Hiker and Absolute"
+        " Mover, if the user has them.\n\nr0: Entity pointer\nr1: Mobility"
+        " type\nreturn: New mobility type, after accounting for the IQ skills mentioned"
+        " above",
+    )
+
+    CannotStandOnTile = Symbol(
+        [0x23524],
+        [0x22FF764],
+        None,
+        "Checks if a given monster cannot stand on a given tile.\n\nReasons include:\n-"
+        " The coordinates of the tile are out of bounds\n- There's another monster on"
+        " the tile\n- The monster does not have the required mobility to stand on the"
+        " tile\n\nr0: Entity pointer\nr1: Tile pointer\nreturn: True if the monster"
+        " cannot stand on the specified tile, false if it can",
+    )
+
     CalcSpeedStage = Symbol(
         [0x23BB4],
         [0x22FFDF4],
         None,
         "Calculates the speed stage of a monster from its speed up/down counters. The"
         " second parameter is the weight of each counter (how many stages it will"
         " add/remove), but appears to be always 1. \nTakes modifiers into account"
@@ -16347,24 +16397,24 @@
         [0x230105C],
         None,
         "Checks if the given monster can move in the specified direction\n\nReturns"
         " false if any monster is standing on the target tile\n\nr0: Monster entity"
         " pointer\nr1: Direction to check\nreturn: bool",
     )
 
-    GetFinalMobilityType = Symbol(
+    GetDirectionalMobilityType = Symbol(
         [0x24CF0],
         [0x2300F30],
         None,
         "Returns the mobility type of a monster, after accounting for things that could"
-        " affect it (like items or IQ skills)\n\nIf the specified direction is"
-        " DIR_NONE, direction checks are skipped. If it's not, MOBILITY_INTANGIBLE is"
-        " only returned if the direction is not diagonal.\n\nr0: Monster entity"
-        " pointer\nr1: Base mobility type\nr2: Direction of mobility\nreturn: Final"
-        " mobility type",
+        " affect it.\n\nList of checks: Mobile status, Mobile Scarf, All-Terrain Hiker"
+        " and Absolute Mover.\n\nIf the specified direction is DIR_NONE, direction"
+        " checks are skipped. If it's not, MOBILITY_INTANGIBLE is only returned if the"
+        " direction is not diagonal.\n\nr0: Monster entity pointer\nr1: Base mobility"
+        " type\nr2: Direction of mobility\nreturn: Final mobility type",
     )
 
     IsMonsterCornered = Symbol(
         [0x24ED8],
         [0x2301118],
         None,
         "True if the given monster is cornered (it can't move in any direction)\n\nr0:"
@@ -18136,21 +18186,21 @@
         [0x3C744],
         [0x2318984],
         None,
         "Inflicts the Magnet Rise status condition on a target monster if"
         " possible.\n\nr0: user entity pointer\nr1: target entity pointer",
     )
 
-    HasConditionalGroundImmunity = Symbol(
+    IsFloating = Symbol(
         [0x3C80C],
         [0x2318A4C],
         None,
-        "Checks if a monster is currently immune to Ground-type moves for reasons other"
-        " than typing and ability.\n\nThis includes checks for Gravity and Magnet"
-        " Rise.\n\nr0: entity pointer\nreturn: bool",
+        "Checks if a monster is currently floating for reasons other than its typing or"
+        " ability.\n\nIn particular, this checks for Gravity and Magnet Rise.\n\nr0:"
+        " entity pointer\nreturn: bool",
     )
 
     TryInflictSafeguardStatus = Symbol(
         [0x3CC30],
         [0x2318E70],
         None,
         "Inflicts the Safeguard status condition on a target monster if"
@@ -18682,14 +18732,23 @@
         [0x2320D08],
         None,
         "Makes the target monster warp if possible.\n\nr0: user entity pointer\nr1:"
         " target entity pointer\nr2: warp type\nr3: position (if warp type is"
         " position-based)",
     )
 
+    EnsureCanStandCurrentTile = Symbol(
+        [0x44EC4],
+        [0x2321104],
+        None,
+        "Checks that the given monster is standing on a tile it can stand on given its"
+        " movement type, and warps it to a random location if it's not.\n\nr0: Entity"
+        " pointer",
+    )
+
     TryActivateNondamagingDefenderAbility = Symbol(
         [0x45838],
         [0x2321A78],
         None,
         "Applies the effects of a defender's ability on an attacker. After a move is"
         " used,\nthis function is called to see if any of the bitflags for an ability"
         " were set and\napplies the corresponding effect. (The way leech seed removes"
@@ -19063,14 +19122,22 @@
         [0x23361D4],
         None,
         "Checks if the current fixed room on the dungeon generation info corresponds to"
         " a fixed, full-floor layout.\n\nThe first non-full-floor fixed room is 0xA5,"
         " which is for Sealed Chambers.\n\nreturn: bool",
     )
 
+    IsCurrentTilesetBackground = Symbol(
+        [0x59FC4],
+        [0x2336204],
+        None,
+        "Calls IsBackgroundTileset with the current tileset ID\n\nreturn: True if the"
+        " current dungeon tileset is a background, false if it's a regular tileset.",
+    )
+
     TrySpawnGoldenChamber = Symbol(
         [0x59FE4],
         [0x2336224],
         None,
         "Changes the tileset and fixed room id of the floor for the Golden Chamber if"
         " the floor should be a\nGolden Chamber.\n\nNo params.",
     )
```

## pmdsky_debug_py/na_itcm.py

```diff
@@ -4511,15 +4511,15 @@
         "Note: unverified, ported from Irdkwia's notes\n\nr0: id\nreturn: speed status",
     )
 
     GetMobilityType = Symbol(
         None,
         None,
         None,
-        "Gets the mobility type for a given monster.\n\nr0: monster ID\nreturn:"
+        "Gets the mobility type for a given monster species.\n\nr0: species ID\nreturn:"
         " mobility type",
     )
 
     GetRegenSpeed = Symbol(
         None,
         None,
         None,
@@ -10283,14 +10283,24 @@
         None,
         None,
         "Note: unverified, ported from Irdkwia's notes\n\nr0: move_id\nreturn:"
         " anim_ent_ptr (This might be a mistake? It seems to be an integer, not a"
         " pointer)",
     )
 
+    IsBackgroundTileset = Symbol(
+        None,
+        None,
+        None,
+        "Given a tileset ID, returns whether it's a background or a regular"
+        " tileset\n\nIn particular, returns r0 >= 0xAA\n\nr0: Tileset ID\nreturn: True"
+        " if the tileset ID corresponds to a background, false if it corresponds to a"
+        " regular tileset",
+    )
+
     CheckEndDungeon = Symbol(
         None,
         None,
         None,
         "Do the stuff when you lose in a dungeon.\n\nNote: unverified, ported from"
         " Irdkwia's notes\n\nr0: End condition code? Seems to control what tasks get"
         " run and what transition happens when the dungeon ends\nreturn: return code?",
@@ -15584,25 +15594,65 @@
         None,
         None,
         "Returns true if the monster has any status problem that prevents it from"
         " acting\n\nr0: Entity pointer\nreturn: True if the specified monster can't act"
         " because of a status problem, false otherwise.",
     )
 
+    GetMobilityTypeCheckSlip = Symbol(
+        None,
+        None,
+        None,
+        "Returns the mobility type of a monster species, accounting for"
+        " STATUS_SLIP.\n\nThe function also converts MOBILITY_LAVA and MOBILITY_WATER"
+        " to other values if required.\n\nr0: Monster species\nr1: True if the monster"
+        " can walk on water\nreturn: Mobility type",
+    )
+
+    GetMobilityTypeCheckSlipAndFloating = Symbol(
+        None,
+        None,
+        None,
+        "Returns the mobility type of a monster, accounting for STATUS_SLIP and the"
+        " result of a call to IsFloating.\n\nr0: Entity pointer\nr1: Monster"
+        " species\nreturn: Mobility type",
+    )
+
     IsInvalidSpawnTile = Symbol(
         None,
         None,
         None,
         "Checks if a monster cannot spawn on the given tile for some reason.\n\nReasons"
         " include:\n- There's another monster on the tile\n- The tile is an impassable"
         " wall\n- The monster does not have the required mobility to stand on the"
         " tile\n\nr0: monster ID\nr1: tile pointer\nreturn: true means the monster"
         " CANNOT spawn on this tile",
     )
 
+    GetMobilityTypeAfterIqSkills = Symbol(
+        None,
+        None,
+        None,
+        "Modifies the given mobility type to account for All-Terrain Hiker and Absolute"
+        " Mover, if the user has them.\n\nr0: Entity pointer\nr1: Mobility"
+        " type\nreturn: New mobility type, after accounting for the IQ skills mentioned"
+        " above",
+    )
+
+    CannotStandOnTile = Symbol(
+        None,
+        None,
+        None,
+        "Checks if a given monster cannot stand on a given tile.\n\nReasons include:\n-"
+        " The coordinates of the tile are out of bounds\n- There's another monster on"
+        " the tile\n- The monster does not have the required mobility to stand on the"
+        " tile\n\nr0: Entity pointer\nr1: Tile pointer\nreturn: True if the monster"
+        " cannot stand on the specified tile, false if it can",
+    )
+
     CalcSpeedStage = Symbol(
         None,
         None,
         None,
         "Calculates the speed stage of a monster from its speed up/down counters. The"
         " second parameter is the weight of each counter (how many stages it will"
         " add/remove), but appears to be always 1. \nTakes modifiers into account"
@@ -15773,24 +15823,24 @@
         None,
         None,
         "Checks if the given monster can move in the specified direction\n\nReturns"
         " false if any monster is standing on the target tile\n\nr0: Monster entity"
         " pointer\nr1: Direction to check\nreturn: bool",
     )
 
-    GetFinalMobilityType = Symbol(
+    GetDirectionalMobilityType = Symbol(
         None,
         None,
         None,
         "Returns the mobility type of a monster, after accounting for things that could"
-        " affect it (like items or IQ skills)\n\nIf the specified direction is"
-        " DIR_NONE, direction checks are skipped. If it's not, MOBILITY_INTANGIBLE is"
-        " only returned if the direction is not diagonal.\n\nr0: Monster entity"
-        " pointer\nr1: Base mobility type\nr2: Direction of mobility\nreturn: Final"
-        " mobility type",
+        " affect it.\n\nList of checks: Mobile status, Mobile Scarf, All-Terrain Hiker"
+        " and Absolute Mover.\n\nIf the specified direction is DIR_NONE, direction"
+        " checks are skipped. If it's not, MOBILITY_INTANGIBLE is only returned if the"
+        " direction is not diagonal.\n\nr0: Monster entity pointer\nr1: Base mobility"
+        " type\nr2: Direction of mobility\nreturn: Final mobility type",
     )
 
     IsMonsterCornered = Symbol(
         None,
         None,
         None,
         "True if the given monster is cornered (it can't move in any direction)\n\nr0:"
@@ -17562,21 +17612,21 @@
         None,
         None,
         None,
         "Inflicts the Magnet Rise status condition on a target monster if"
         " possible.\n\nr0: user entity pointer\nr1: target entity pointer",
     )
 
-    HasConditionalGroundImmunity = Symbol(
+    IsFloating = Symbol(
         None,
         None,
         None,
-        "Checks if a monster is currently immune to Ground-type moves for reasons other"
-        " than typing and ability.\n\nThis includes checks for Gravity and Magnet"
-        " Rise.\n\nr0: entity pointer\nreturn: bool",
+        "Checks if a monster is currently floating for reasons other than its typing or"
+        " ability.\n\nIn particular, this checks for Gravity and Magnet Rise.\n\nr0:"
+        " entity pointer\nreturn: bool",
     )
 
     TryInflictSafeguardStatus = Symbol(
         None,
         None,
         None,
         "Inflicts the Safeguard status condition on a target monster if"
@@ -18108,14 +18158,23 @@
         None,
         None,
         "Makes the target monster warp if possible.\n\nr0: user entity pointer\nr1:"
         " target entity pointer\nr2: warp type\nr3: position (if warp type is"
         " position-based)",
     )
 
+    EnsureCanStandCurrentTile = Symbol(
+        None,
+        None,
+        None,
+        "Checks that the given monster is standing on a tile it can stand on given its"
+        " movement type, and warps it to a random location if it's not.\n\nr0: Entity"
+        " pointer",
+    )
+
     TryActivateNondamagingDefenderAbility = Symbol(
         None,
         None,
         None,
         "Applies the effects of a defender's ability on an attacker. After a move is"
         " used,\nthis function is called to see if any of the bitflags for an ability"
         " were set and\napplies the corresponding effect. (The way leech seed removes"
@@ -18483,14 +18542,22 @@
         None,
         None,
         "Checks if the current fixed room on the dungeon generation info corresponds to"
         " a fixed, full-floor layout.\n\nThe first non-full-floor fixed room is 0xA5,"
         " which is for Sealed Chambers.\n\nreturn: bool",
     )
 
+    IsCurrentTilesetBackground = Symbol(
+        None,
+        None,
+        None,
+        "Calls IsBackgroundTileset with the current tileset ID\n\nreturn: True if the"
+        " current dungeon tileset is a background, false if it's a regular tileset.",
+    )
+
     TrySpawnGoldenChamber = Symbol(
         None,
         None,
         None,
         "Changes the tileset and fixed room id of the floor for the Golden Chamber if"
         " the floor should be a\nGolden Chamber.\n\nNo params.",
     )
```

## pmdsky_debug_py/protocol.py

```diff
@@ -6624,14 +6624,19 @@
     ]
 
     GetMoveAnimationSpeed: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    IsBackgroundTileset: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     CheckEndDungeon: Symbol[
         Optional[List[int]],
         None,
     ]
 
 
 class Overlay10DataProtocol(Protocol):
@@ -10725,19 +10730,39 @@
     ]
 
     HasStatusThatPreventsActing: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    GetMobilityTypeCheckSlip: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    GetMobilityTypeCheckSlipAndFloating: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     IsInvalidSpawnTile: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    GetMobilityTypeAfterIqSkills: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    CannotStandOnTile: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     CalcSpeedStage: Symbol[
         Optional[List[int]],
         None,
     ]
 
     CalcSpeedStageWrapper: Symbol[
         Optional[List[int]],
@@ -10825,15 +10850,15 @@
     ]
 
     CanMonsterMoveInDirection: Symbol[
         Optional[List[int]],
         None,
     ]
 
-    GetFinalMobilityType: Symbol[
+    GetDirectionalMobilityType: Symbol[
         Optional[List[int]],
         None,
     ]
 
     IsMonsterCornered: Symbol[
         Optional[List[int]],
         None,
@@ -11750,15 +11775,15 @@
     ]
 
     TryInflictMagnetRiseStatus: Symbol[
         Optional[List[int]],
         None,
     ]
 
-    HasConditionalGroundImmunity: Symbol[
+    IsFloating: Symbol[
         Optional[List[int]],
         None,
     ]
 
     TryInflictSafeguardStatus: Symbol[
         Optional[List[int]],
         None,
@@ -12050,14 +12075,19 @@
     ]
 
     TryWarp: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    EnsureCanStandCurrentTile: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     TryActivateNondamagingDefenderAbility: Symbol[
         Optional[List[int]],
         None,
     ]
 
     TryActivateNondamagingDefenderExclusiveItem: Symbol[
         Optional[List[int]],
@@ -12240,14 +12270,19 @@
     ]
 
     IsFullFloorFixedRoom: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    IsCurrentTilesetBackground: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     TrySpawnGoldenChamber: Symbol[
         Optional[List[int]],
         None,
     ]
 
     CountItemsOnFloorForAcuteSniffer: Symbol[
         Optional[List[int]],
```

## Comparing `pmdsky_debug_py-7.0.5.dist-info/METADATA` & `pmdsky_debug_py-7.0.6.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmdsky-debug-py
-Version: 7.0.5
+Version: 7.0.6
 Summary: pmdsky-debug symbols for Python.
 Author-email: Marco 'Capypara' Köpcke <hello@capypara.de>
 License: MIT
 Project-URL: repository, https://github.com/SkyTemple/pmdsky-debug-py
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
```

