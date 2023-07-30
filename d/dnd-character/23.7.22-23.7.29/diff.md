# Comparing `tmp/dnd_character-23.7.22.tar.gz` & `tmp/dnd_character-23.7.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dnd_character-23.7.22.tar", last modified: Sat Jul 22 21:49:02 2023, max compression
+gzip compressed data, was "dnd_character-23.7.29.tar", last modified: Sun Jul 30 01:48:19 2023, max compression
```

## Comparing `dnd_character-23.7.22.tar` & `dnd_character-23.7.29.tar`

### file list

```diff
@@ -1,1246 +1,1246 @@
-drwxrwxr-x   0 b         (1000) b         (1000)        0 2023-07-22 21:49:02.483644 dnd_character-23.7.22/
--rw-rw-r--   0 b         (1000) b         (1000)    14199 2022-09-20 01:54:47.000000 dnd_character-23.7.22/LICENSE
--rw-rw-r--   0 b         (1000) b         (1000)       52 2022-09-20 01:54:47.000000 dnd_character-23.7.22/MANIFEST.in
--rw-rw-r--   0 b         (1000) b         (1000)     5480 2023-07-22 21:49:02.479644 dnd_character-23.7.22/PKG-INFO
--rw-rw-r--   0 b         (1000) b         (1000)     4833 2023-07-22 21:12:36.000000 dnd_character-23.7.22/README.md
-drwxrwxr-x   0 b         (1000) b         (1000)        0 2023-07-22 21:49:02.311644 dnd_character-23.7.22/dnd_character/
--rw-rw-r--   0 b         (1000) b         (1000)     2430 2023-07-22 21:36:09.000000 dnd_character-23.7.22/dnd_character/SRD.py
--rw-rw-r--   0 b         (1000) b         (1000)      594 2023-07-22 21:35:20.000000 dnd_character-23.7.22/dnd_character/__init__.py
--rw-rw-r--   0 b         (1000) b         (1000)     1735 2023-07-12 17:26:36.000000 dnd_character-23.7.22/dnd_character/__main__.py
--rw-rw-r--   0 b         (1000) b         (1000)    23814 2023-07-22 20:47:06.000000 dnd_character-23.7.22/dnd_character/character.py
--rw-rw-r--   0 b         (1000) b         (1000)     1049 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/classes.py
--rw-rw-r--   0 b         (1000) b         (1000)     1190 2023-07-22 20:13:10.000000 dnd_character-23.7.22/dnd_character/dice.py
--rw-rw-r--   0 b         (1000) b         (1000)      158 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/equipment.py
--rw-rw-r--   0 b         (1000) b         (1000)     3002 2023-07-12 16:46:59.000000 dnd_character-23.7.22/dnd_character/experience.py
-drwxrwxr-x   0 b         (1000) b         (1000)        0 2023-07-22 21:49:02.479644 dnd_character-23.7.22/dnd_character/json_cache/
--rw-rw-r--   0 b         (1000) b         (1000)     6468 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/OGLv1.0a.txt
--rw-rw-r--   0 b         (1000) b         (1000)       95 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/README.md
--rw-rw-r--   0 b         (1000) b         (1000)      784 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_.json
--rw-rw-r--   0 b         (1000) b         (1000)      860 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_classes.json
--rw-rw-r--   0 b         (1000) b         (1000)     4057 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_classes_barbarian.json
--rw-rw-r--   0 b         (1000) b         (1000)     8578 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_classes_barbarian_levels.json
--rw-rw-r--   0 b         (1000) b         (1000)    13694 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_classes_bard.json
--rw-rw-r--   0 b         (1000) b         (1000)    15727 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_classes_bard_levels.json
--rw-rw-r--   0 b         (1000) b         (1000)     7660 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_classes_cleric.json
--rw-rw-r--   0 b         (1000) b         (1000)    14080 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_classes_cleric_levels.json
--rw-rw-r--   0 b         (1000) b         (1000)     7654 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_classes_druid.json
--rw-rw-r--   0 b         (1000) b         (1000)    13282 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_classes_druid_levels.json
--rw-rw-r--   0 b         (1000) b         (1000)     6103 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_classes_fighter.json
--rw-rw-r--   0 b         (1000) b         (1000)     8172 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_classes_fighter_levels.json
--rw-rw-r--   0 b         (1000) b         (1000)     7806 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_classes_monk.json
--rw-rw-r--   0 b         (1000) b         (1000)     9190 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_classes_monk_levels.json
--rw-rw-r--   0 b         (1000) b         (1000)     7193 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_classes_paladin.json
--rw-rw-r--   0 b         (1000) b         (1000)    10285 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_classes_paladin_levels.json
--rw-rw-r--   0 b         (1000) b         (1000)     8002 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_classes_ranger.json
--rw-rw-r--   0 b         (1000) b         (1000)    11393 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_classes_ranger_levels.json
--rw-rw-r--   0 b         (1000) b         (1000)     7246 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_classes_rogue.json
--rw-rw-r--   0 b         (1000) b         (1000)     7636 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_classes_rogue_levels.json
--rw-rw-r--   0 b         (1000) b         (1000)     6488 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_classes_sorcerer.json
--rw-rw-r--   0 b         (1000) b         (1000)    18613 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_classes_sorcerer_levels.json
--rw-rw-r--   0 b         (1000) b         (1000)     7003 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_classes_warlock.json
--rw-rw-r--   0 b         (1000) b         (1000)    15137 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_classes_warlock_levels.json
--rw-rw-r--   0 b         (1000) b         (1000)     6717 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_classes_wizard.json
--rw-rw-r--   0 b         (1000) b         (1000)    11937 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_classes_wizard_levels.json
--rw-rw-r--   0 b         (1000) b         (1000)      441 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment-categories_arcane-foci.json
--rw-rw-r--   0 b         (1000) b         (1000)      454 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment-categories_druidic-foci.json
--rw-rw-r--   0 b         (1000) b         (1000)      335 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment-categories_holy-symbols.json
--rw-rw-r--   0 b         (1000) b         (1000)     1484 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment-categories_martial-melee-weapons.json
--rw-rw-r--   0 b         (1000) b         (1000)     1865 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment-categories_martial-weapons.json
--rw-rw-r--   0 b         (1000) b         (1000)      829 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment-categories_musical-instruments.json
--rw-rw-r--   0 b         (1000) b         (1000)      883 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment-categories_simple-melee-weapons.json
--rw-rw-r--   0 b         (1000) b         (1000)     1171 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment-categories_simple-weapons.json
--rw-rw-r--   0 b         (1000) b         (1000)    20241 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment.json
--rw-rw-r--   0 b         (1000) b         (1000)      436 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_abacus.json
--rw-rw-r--   0 b         (1000) b         (1000)      756 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_acid-vial.json
--rw-rw-r--   0 b         (1000) b         (1000)      921 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_alchemists-fire-flask.json
--rw-rw-r--   0 b         (1000) b         (1000)      744 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_alchemists-supplies.json
--rw-rw-r--   0 b         (1000) b         (1000)      501 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_alms-box.json
--rw-rw-r--   0 b         (1000) b         (1000)      934 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_amulet.json
--rw-rw-r--   0 b         (1000) b         (1000)      418 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_animal-feed-1-day.json
--rw-rw-r--   0 b         (1000) b         (1000)      614 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_antitoxin-vial.json
--rw-rw-r--   0 b         (1000) b         (1000)      440 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_arrow.json
--rw-rw-r--   0 b         (1000) b         (1000)      442 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_backpack.json
--rw-rw-r--   0 b         (1000) b         (1000)      706 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_bagpipes.json
--rw-rw-r--   0 b         (1000) b         (1000)      812 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_ball-bearings-bag-of-1000.json
--rw-rw-r--   0 b         (1000) b         (1000)      670 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_barding-breastplate.json
--rw-rw-r--   0 b         (1000) b         (1000)      667 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_barding-chain-mail.json
--rw-rw-r--   0 b         (1000) b         (1000)      669 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_barding-chain-shirt.json
--rw-rw-r--   0 b         (1000) b         (1000)      667 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_barding-half-plate.json
--rw-rw-r--   0 b         (1000) b         (1000)      647 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_barding-hide.json
--rw-rw-r--   0 b         (1000) b         (1000)      656 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_barding-leather.json
--rw-rw-r--   0 b         (1000) b         (1000)      653 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_barding-padded.json
--rw-rw-r--   0 b         (1000) b         (1000)      653 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_barding-plate.json
--rw-rw-r--   0 b         (1000) b         (1000)      662 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_barding-ring-mail.json
--rw-rw-r--   0 b         (1000) b         (1000)      666 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_barding-scale-mail.json
--rw-rw-r--   0 b         (1000) b         (1000)      655 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_barding-splint.json
--rw-rw-r--   0 b         (1000) b         (1000)      681 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_barding-studded-leather.json
--rw-rw-r--   0 b         (1000) b         (1000)      437 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_barrel.json
--rw-rw-r--   0 b         (1000) b         (1000)      436 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_basket.json
--rw-rw-r--   0 b         (1000) b         (1000)      766 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_battleaxe.json
--rw-rw-r--   0 b         (1000) b         (1000)      439 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_bedroll.json
--rw-rw-r--   0 b         (1000) b         (1000)      430 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_bell.json
--rw-rw-r--   0 b         (1000) b         (1000)      406 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_bit-and-bridle.json
--rw-rw-r--   0 b         (1000) b         (1000)      439 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_blanket.json
--rw-rw-r--   0 b         (1000) b         (1000)      642 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_block-and-tackle.json
--rw-rw-r--   0 b         (1000) b         (1000)      523 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_block-of-incense.json
--rw-rw-r--   0 b         (1000) b         (1000)      467 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_blowgun-needle.json
--rw-rw-r--   0 b         (1000) b         (1000)      718 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_blowgun.json
--rw-rw-r--   0 b         (1000) b         (1000)      723 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_book.json
--rw-rw-r--   0 b         (1000) b         (1000)      455 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_bottle-glass.json
--rw-rw-r--   0 b         (1000) b         (1000)      442 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_breastplate.json
--rw-rw-r--   0 b         (1000) b         (1000)      735 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_brewers-supplies.json
--rw-rw-r--   0 b         (1000) b         (1000)      436 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_bucket.json
--rw-rw-r--   0 b         (1000) b         (1000)     2000 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_burglars-pack.json
--rw-rw-r--   0 b         (1000) b         (1000)      753 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_calligraphers-supplies.json
--rw-rw-r--   0 b         (1000) b         (1000)      878 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_caltrops.json
--rw-rw-r--   0 b         (1000) b         (1000)      428 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_camel.json
--rw-rw-r--   0 b         (1000) b         (1000)      536 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_candle.json
--rw-rw-r--   0 b         (1000) b         (1000)      734 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_carpenters-tools.json
--rw-rw-r--   0 b         (1000) b         (1000)      392 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_carriage.json
--rw-rw-r--   0 b         (1000) b         (1000)      379 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_cart.json
--rw-rw-r--   0 b         (1000) b         (1000)      744 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_cartographers-tools.json
--rw-rw-r--   0 b         (1000) b         (1000)      529 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_case-crossbow-bolt.json
--rw-rw-r--   0 b         (1000) b         (1000)      588 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_case-map-or-scroll.json
--rw-rw-r--   0 b         (1000) b         (1000)      483 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_censer.json
--rw-rw-r--   0 b         (1000) b         (1000)      544 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_chain-10-feet.json
--rw-rw-r--   0 b         (1000) b         (1000)      422 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_chain-mail.json
--rw-rw-r--   0 b         (1000) b         (1000)      441 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_chain-shirt.json
--rw-rw-r--   0 b         (1000) b         (1000)      459 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_chalk-1-piece.json
--rw-rw-r--   0 b         (1000) b         (1000)      389 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_chariot.json
--rw-rw-r--   0 b         (1000) b         (1000)      434 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_chest.json
--rw-rw-r--   0 b         (1000) b         (1000)      746 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_climbers-kit.json
--rw-rw-r--   0 b         (1000) b         (1000)      461 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_clothes-common.json
--rw-rw-r--   0 b         (1000) b         (1000)      464 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_clothes-costume.json
--rw-rw-r--   0 b         (1000) b         (1000)      456 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_clothes-fine.json
--rw-rw-r--   0 b         (1000) b         (1000)      471 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_clothes-travelers.json
--rw-rw-r--   0 b         (1000) b         (1000)      677 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_club.json
--rw-rw-r--   0 b         (1000) b         (1000)      728 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_cobblers-tools.json
--rw-rw-r--   0 b         (1000) b         (1000)      733 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_component-pouch.json
--rw-rw-r--   0 b         (1000) b         (1000)      728 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_cooks-utensils.json
--rw-rw-r--   0 b         (1000) b         (1000)      466 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_crossbow-bolt.json
--rw-rw-r--   0 b         (1000) b         (1000)      815 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_crossbow-hand.json
--rw-rw-r--   0 b         (1000) b         (1000)      912 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_crossbow-heavy.json
--rw-rw-r--   0 b         (1000) b         (1000)      831 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_crossbow-light.json
--rw-rw-r--   0 b         (1000) b         (1000)      537 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_crowbar.json
--rw-rw-r--   0 b         (1000) b         (1000)      702 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_crystal.json
--rw-rw-r--   0 b         (1000) b         (1000)      878 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_dagger.json
--rw-rw-r--   0 b         (1000) b         (1000)      741 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_dart.json
--rw-rw-r--   0 b         (1000) b         (1000)      723 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_dice-set.json
--rw-rw-r--   0 b         (1000) b         (1000)     1666 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_diplomats-pack.json
--rw-rw-r--   0 b         (1000) b         (1000)      666 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_disguise-kit.json
--rw-rw-r--   0 b         (1000) b         (1000)      430 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_donkey.json
--rw-rw-r--   0 b         (1000) b         (1000)      693 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_drum.json
--rw-rw-r--   0 b         (1000) b         (1000)      707 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_dulcimer.json
--rw-rw-r--   0 b         (1000) b         (1000)     1412 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_dungeoneers-pack.json
--rw-rw-r--   0 b         (1000) b         (1000)      440 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_elephant.json
--rw-rw-r--   0 b         (1000) b         (1000)      934 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_emblem.json
--rw-rw-r--   0 b         (1000) b         (1000)     1221 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_entertainers-pack.json
--rw-rw-r--   0 b         (1000) b         (1000)     1318 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_explorers-pack.json
--rw-rw-r--   0 b         (1000) b         (1000)      585 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_fishing-tackle.json
--rw-rw-r--   0 b         (1000) b         (1000)      536 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_flail.json
--rw-rw-r--   0 b         (1000) b         (1000)      466 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_flask-or-tankard.json
--rw-rw-r--   0 b         (1000) b         (1000)      696 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_flute.json
--rw-rw-r--   0 b         (1000) b         (1000)      766 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_forgery-kit.json
--rw-rw-r--   0 b         (1000) b         (1000)      400 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_galley.json
--rw-rw-r--   0 b         (1000) b         (1000)      772 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_glaive.json
--rw-rw-r--   0 b         (1000) b         (1000)      741 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_glassblowers-tools.json
--rw-rw-r--   0 b         (1000) b         (1000)      460 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_grappling-hook.json
--rw-rw-r--   0 b         (1000) b         (1000)      702 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_greataxe.json
--rw-rw-r--   0 b         (1000) b         (1000)      635 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_greatclub.json
--rw-rw-r--   0 b         (1000) b         (1000)      707 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_greatsword.json
--rw-rw-r--   0 b         (1000) b         (1000)      775 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_halberd.json
--rw-rw-r--   0 b         (1000) b         (1000)      456 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_half-plate-armor.json
--rw-rw-r--   0 b         (1000) b         (1000)      459 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_hammer-sledge.json
--rw-rw-r--   0 b         (1000) b         (1000)      436 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_hammer.json
--rw-rw-r--   0 b         (1000) b         (1000)      799 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_handaxe.json
--rw-rw-r--   0 b         (1000) b         (1000)      664 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_healers-kit.json
--rw-rw-r--   0 b         (1000) b         (1000)      793 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_herbalism-kit.json
--rw-rw-r--   0 b         (1000) b         (1000)      438 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_hide-armor.json
--rw-rw-r--   0 b         (1000) b         (1000)     1007 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_holy-water-flask.json
--rw-rw-r--   0 b         (1000) b         (1000)      693 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_horn.json
--rw-rw-r--   0 b         (1000) b         (1000)      447 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_horse-draft.json
--rw-rw-r--   0 b         (1000) b         (1000)      450 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_horse-riding.json
--rw-rw-r--   0 b         (1000) b         (1000)      446 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_hourglass.json
--rw-rw-r--   0 b         (1000) b         (1000)     1176 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_hunting-trap.json
--rw-rw-r--   0 b         (1000) b         (1000)      475 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_ink-1-ounce-bottle.json
--rw-rw-r--   0 b         (1000) b         (1000)      439 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_ink-pen.json
--rw-rw-r--   0 b         (1000) b         (1000)      724 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_javelin.json
--rw-rw-r--   0 b         (1000) b         (1000)      729 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_jewelers-tools.json
--rw-rw-r--   0 b         (1000) b         (1000)      460 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_jug-or-pitcher.json
--rw-rw-r--   0 b         (1000) b         (1000)      763 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_keelboat.json
--rw-rw-r--   0 b         (1000) b         (1000)      463 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_ladder-10-foot.json
--rw-rw-r--   0 b         (1000) b         (1000)      577 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_lamp.json
--rw-rw-r--   0 b         (1000) b         (1000)      836 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_lance.json
--rw-rw-r--   0 b         (1000) b         (1000)      625 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_lantern-bullseye.json
--rw-rw-r--   0 b         (1000) b         (1000)      708 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_lantern-hooded.json
--rw-rw-r--   0 b         (1000) b         (1000)      430 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_leather-armor.json
--rw-rw-r--   0 b         (1000) b         (1000)      746 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_leatherworkers-tools.json
--rw-rw-r--   0 b         (1000) b         (1000)      823 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_light-hammer.json
--rw-rw-r--   0 b         (1000) b         (1000)      531 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_little-bag-of-sand.json
--rw-rw-r--   0 b         (1000) b         (1000)      654 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_lock.json
--rw-rw-r--   0 b         (1000) b         (1000)      806 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_longbow.json
--rw-rw-r--   0 b         (1000) b         (1000)      406 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_longship.json
--rw-rw-r--   0 b         (1000) b         (1000)      766 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_longsword.json
--rw-rw-r--   0 b         (1000) b         (1000)      694 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_lute.json
--rw-rw-r--   0 b         (1000) b         (1000)      694 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_lyre.json
--rw-rw-r--   0 b         (1000) b         (1000)      601 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_mace.json
--rw-rw-r--   0 b         (1000) b         (1000)      872 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_magnifying-glass.json
--rw-rw-r--   0 b         (1000) b         (1000)      829 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_manacles.json
--rw-rw-r--   0 b         (1000) b         (1000)      723 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_masons-tools.json
--rw-rw-r--   0 b         (1000) b         (1000)      434 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_mastiff.json
--rw-rw-r--   0 b         (1000) b         (1000)      699 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_maul.json
--rw-rw-r--   0 b         (1000) b         (1000)      573 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_mess-kit.json
--rw-rw-r--   0 b         (1000) b         (1000)      457 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_mirror-steel.json
--rw-rw-r--   0 b         (1000) b         (1000)      545 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_morningstar.json
--rw-rw-r--   0 b         (1000) b         (1000)      424 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_mule.json
--rw-rw-r--   0 b         (1000) b         (1000)      624 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_navigators-tools.json
--rw-rw-r--   0 b         (1000) b         (1000)     1190 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_net.json
--rw-rw-r--   0 b         (1000) b         (1000)     1227 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_oil-flask.json
--rw-rw-r--   0 b         (1000) b         (1000)      690 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_orb.json
--rw-rw-r--   0 b         (1000) b         (1000)      424 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_padded-armor.json
--rw-rw-r--   0 b         (1000) b         (1000)      738 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_painters-supplies.json
--rw-rw-r--   0 b         (1000) b         (1000)      709 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_pan-flute.json
--rw-rw-r--   0 b         (1000) b         (1000)      465 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_paper-one-sheet.json
--rw-rw-r--   0 b         (1000) b         (1000)      477 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_parchment-one-sheet.json
--rw-rw-r--   0 b         (1000) b         (1000)      456 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_perfume-vial.json
--rw-rw-r--   0 b         (1000) b         (1000)      454 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_pick-miners.json
--rw-rw-r--   0 b         (1000) b         (1000)      766 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_pike.json
--rw-rw-r--   0 b         (1000) b         (1000)      436 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_piton.json
--rw-rw-r--   0 b         (1000) b         (1000)      427 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_plate-armor.json
--rw-rw-r--   0 b         (1000) b         (1000)      747 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_playing-card-set.json
--rw-rw-r--   0 b         (1000) b         (1000)      817 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_poison-basic-vial.json
--rw-rw-r--   0 b         (1000) b         (1000)      658 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_poisoners-kit.json
--rw-rw-r--   0 b         (1000) b         (1000)      456 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_pole-10-foot.json
--rw-rw-r--   0 b         (1000) b         (1000)      425 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_pony.json
--rw-rw-r--   0 b         (1000) b         (1000)      444 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_pot-iron.json
--rw-rw-r--   0 b         (1000) b         (1000)      726 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_potters-tools.json
--rw-rw-r--   0 b         (1000) b         (1000)      654 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_pouch.json
--rw-rw-r--   0 b         (1000) b         (1000)     1503 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_priests-pack.json
--rw-rw-r--   0 b         (1000) b         (1000)      862 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_quarterstaff.json
--rw-rw-r--   0 b         (1000) b         (1000)      472 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_quiver.json
--rw-rw-r--   0 b         (1000) b         (1000)      645 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_ram-portable.json
--rw-rw-r--   0 b         (1000) b         (1000)      610 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_rapier.json
--rw-rw-r--   0 b         (1000) b         (1000)      569 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_rations-1-day.json
--rw-rw-r--   0 b         (1000) b         (1000)      943 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_reliquary.json
--rw-rw-r--   0 b         (1000) b         (1000)      418 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_ring-mail.json
--rw-rw-r--   0 b         (1000) b         (1000)      433 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_robes.json
--rw-rw-r--   0 b         (1000) b         (1000)      690 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_rod.json
--rw-rw-r--   0 b         (1000) b         (1000)      579 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_rope-hempen-50-feet.json
--rw-rw-r--   0 b         (1000) b         (1000)      573 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_rope-silk-50-feet.json
--rw-rw-r--   0 b         (1000) b         (1000)      760 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_rowboat.json
--rw-rw-r--   0 b         (1000) b         (1000)      432 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_sack.json
--rw-rw-r--   0 b         (1000) b         (1000)      476 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_saddle-exotic.json
--rw-rw-r--   0 b         (1000) b         (1000)      570 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_saddle-military.json
--rw-rw-r--   0 b         (1000) b         (1000)      399 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_saddle-pack.json
--rw-rw-r--   0 b         (1000) b         (1000)      406 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_saddle-riding.json
--rw-rw-r--   0 b         (1000) b         (1000)      394 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_saddlebags.json
--rw-rw-r--   0 b         (1000) b         (1000)      418 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_sailing-ship.json
--rw-rw-r--   0 b         (1000) b         (1000)      437 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_scale-mail.json
--rw-rw-r--   0 b         (1000) b         (1000)      694 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_scale-merchants.json
--rw-rw-r--   0 b         (1000) b         (1000)     1256 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_scholars-pack.json
--rw-rw-r--   0 b         (1000) b         (1000)      692 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_scimitar.json
--rw-rw-r--   0 b         (1000) b         (1000)      451 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_sealing-wax.json
--rw-rw-r--   0 b         (1000) b         (1000)      696 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_shawm.json
--rw-rw-r--   0 b         (1000) b         (1000)      409 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_shield.json
--rw-rw-r--   0 b         (1000) b         (1000)      730 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_shortbow.json
--rw-rw-r--   0 b         (1000) b         (1000)      771 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_shortsword.json
--rw-rw-r--   0 b         (1000) b         (1000)      436 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_shovel.json
--rw-rw-r--   0 b         (1000) b         (1000)      674 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_sickle.json
--rw-rw-r--   0 b         (1000) b         (1000)      460 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_signal-whistle.json
--rw-rw-r--   0 b         (1000) b         (1000)      451 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_signet-ring.json
--rw-rw-r--   0 b         (1000) b         (1000)      379 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_sled.json
--rw-rw-r--   0 b         (1000) b         (1000)      463 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_sling-bullet.json
--rw-rw-r--   0 b         (1000) b         (1000)      638 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_sling.json
--rw-rw-r--   0 b         (1000) b         (1000)      504 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_small-knife.json
--rw-rw-r--   0 b         (1000) b         (1000)      723 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_smiths-tools.json
--rw-rw-r--   0 b         (1000) b         (1000)      430 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_soap.json
--rw-rw-r--   0 b         (1000) b         (1000)      945 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_spear.json
--rw-rw-r--   0 b         (1000) b         (1000)      565 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_spellbook.json
--rw-rw-r--   0 b         (1000) b         (1000)      449 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_spike-iron.json
--rw-rw-r--   0 b         (1000) b         (1000)      429 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_splint-armor.json
--rw-rw-r--   0 b         (1000) b         (1000)      764 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_sprig-of-mistletoe.json
--rw-rw-r--   0 b         (1000) b         (1000)      515 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_spyglass.json
--rw-rw-r--   0 b         (1000) b         (1000)      408 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_stabling-1-day.json
--rw-rw-r--   0 b         (1000) b         (1000)      695 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_staff.json
--rw-rw-r--   0 b         (1000) b         (1000)      528 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_string-10-feet.json
--rw-rw-r--   0 b         (1000) b         (1000)      454 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_studded-leather-armor.json
--rw-rw-r--   0 b         (1000) b         (1000)      523 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_tent-two-person.json
--rw-rw-r--   0 b         (1000) b         (1000)      625 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_thieves-tools.json
--rw-rw-r--   0 b         (1000) b         (1000)      699 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_tinderbox.json
--rw-rw-r--   0 b         (1000) b         (1000)      727 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_tinkers-tools.json
--rw-rw-r--   0 b         (1000) b         (1000)      625 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_torch.json
--rw-rw-r--   0 b         (1000) b         (1000)      725 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_totem.json
--rw-rw-r--   0 b         (1000) b         (1000)      880 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_trident.json
--rw-rw-r--   0 b         (1000) b         (1000)      502 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_vestments.json
--rw-rw-r--   0 b         (1000) b         (1000)      430 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_vial.json
--rw-rw-r--   0 b         (1000) b         (1000)      694 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_viol.json
--rw-rw-r--   0 b         (1000) b         (1000)      382 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_wagon.json
--rw-rw-r--   0 b         (1000) b         (1000)      693 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_wand.json
--rw-rw-r--   0 b         (1000) b         (1000)      535 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_war-pick.json
--rw-rw-r--   0 b         (1000) b         (1000)      784 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_warhammer.json
--rw-rw-r--   0 b         (1000) b         (1000)      438 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_warhorse.json
--rw-rw-r--   0 b         (1000) b         (1000)      405 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_warship.json
--rw-rw-r--   0 b         (1000) b         (1000)      445 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_waterskin.json
--rw-rw-r--   0 b         (1000) b         (1000)      725 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_weavers-tools.json
--rw-rw-r--   0 b         (1000) b         (1000)      445 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_whetstone.json
--rw-rw-r--   0 b         (1000) b         (1000)      679 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_whip.json
--rw-rw-r--   0 b         (1000) b         (1000)      737 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_woodcarvers-tools.json
--rw-rw-r--   0 b         (1000) b         (1000)      746 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_wooden-staff.json
--rw-rw-r--   0 b         (1000) b         (1000)      735 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_equipment_yew-wand.json
--rw-rw-r--   0 b         (1000) b         (1000)      614 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_action-surge-1-use.json
--rw-rw-r--   0 b         (1000) b         (1000)      618 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_action-surge-2-uses.json
--rw-rw-r--   0 b         (1000) b         (1000)      729 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_arcane-recovery.json
--rw-rw-r--   0 b         (1000) b         (1000)      448 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_arcane-tradition.json
--rw-rw-r--   0 b         (1000) b         (1000)      530 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_archdruid.json
--rw-rw-r--   0 b         (1000) b         (1000)      289 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_aura-improvements.json
--rw-rw-r--   0 b         (1000) b         (1000)      404 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_aura-of-courage.json
--rw-rw-r--   0 b         (1000) b         (1000)      553 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_aura-of-protection.json
--rw-rw-r--   0 b         (1000) b         (1000)      546 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_barbarian-ability-score-improvement-1.json
--rw-rw-r--   0 b         (1000) b         (1000)      546 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_barbarian-ability-score-improvement-2.json
--rw-rw-r--   0 b         (1000) b         (1000)      547 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_barbarian-ability-score-improvement-3.json
--rw-rw-r--   0 b         (1000) b         (1000)      547 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_barbarian-ability-score-improvement-4.json
--rw-rw-r--   0 b         (1000) b         (1000)      547 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_barbarian-ability-score-improvement-5.json
--rw-rw-r--   0 b         (1000) b         (1000)      352 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_barbarian-extra-attack.json
--rw-rw-r--   0 b         (1000) b         (1000)      424 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_barbarian-unarmored-defense.json
--rw-rw-r--   0 b         (1000) b         (1000)      521 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_bard-ability-score-improvement-1.json
--rw-rw-r--   0 b         (1000) b         (1000)      521 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_bard-ability-score-improvement-2.json
--rw-rw-r--   0 b         (1000) b         (1000)      522 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_bard-ability-score-improvement-3.json
--rw-rw-r--   0 b         (1000) b         (1000)      522 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_bard-ability-score-improvement-4.json
--rw-rw-r--   0 b         (1000) b         (1000)      522 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_bard-ability-score-improvement-5.json
--rw-rw-r--   0 b         (1000) b         (1000)      398 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_bard-college.json
--rw-rw-r--   0 b         (1000) b         (1000)     3182 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_bard-expertise-1.json
--rw-rw-r--   0 b         (1000) b         (1000)     3183 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_bard-expertise-2.json
--rw-rw-r--   0 b         (1000) b         (1000)     1240 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_bardic-inspiration-d10.json
--rw-rw-r--   0 b         (1000) b         (1000)     1240 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_bardic-inspiration-d12.json
--rw-rw-r--   0 b         (1000) b         (1000)     1236 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_bardic-inspiration-d6.json
--rw-rw-r--   0 b         (1000) b         (1000)     1236 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_bardic-inspiration-d8.json
--rw-rw-r--   0 b         (1000) b         (1000)      457 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_beast-spells.json
--rw-rw-r--   0 b         (1000) b         (1000)      340 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_blindsense.json
--rw-rw-r--   0 b         (1000) b         (1000)      485 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_brutal-critical-1-die.json
--rw-rw-r--   0 b         (1000) b         (1000)      489 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_brutal-critical-2-dice.json
--rw-rw-r--   0 b         (1000) b         (1000)      489 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_brutal-critical-3-dice.json
--rw-rw-r--   0 b         (1000) b         (1000)     1080 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_channel-divinity-1-rest.json
--rw-rw-r--   0 b         (1000) b         (1000)      464 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_channel-divinity-2-rest.json
--rw-rw-r--   0 b         (1000) b         (1000)      465 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_channel-divinity-3-rest.json
--rw-rw-r--   0 b         (1000) b         (1000)      889 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_channel-divinity-turn-undead.json
--rw-rw-r--   0 b         (1000) b         (1000)      663 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_channel-divinity.json
--rw-rw-r--   0 b         (1000) b         (1000)      497 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_cleansing-touch.json
--rw-rw-r--   0 b         (1000) b         (1000)      531 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_cleric-ability-score-improvement-1.json
--rw-rw-r--   0 b         (1000) b         (1000)      531 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_cleric-ability-score-improvement-2.json
--rw-rw-r--   0 b         (1000) b         (1000)      532 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_cleric-ability-score-improvement-3.json
--rw-rw-r--   0 b         (1000) b         (1000)      532 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_cleric-ability-score-improvement-4.json
--rw-rw-r--   0 b         (1000) b         (1000)      532 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_cleric-ability-score-improvement-5.json
--rw-rw-r--   0 b         (1000) b         (1000)      714 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_countercharm.json
--rw-rw-r--   0 b         (1000) b         (1000)      438 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_cunning-action.json
--rw-rw-r--   0 b         (1000) b         (1000)      537 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_danger-sense.json
--rw-rw-r--   0 b         (1000) b         (1000)      976 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_deflect-missiles.json
--rw-rw-r--   0 b         (1000) b         (1000)      457 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_destroy-undead-cr-1-2-or-below.json
--rw-rw-r--   0 b         (1000) b         (1000)      451 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_destroy-undead-cr-1-or-below.json
--rw-rw-r--   0 b         (1000) b         (1000)      452 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_destroy-undead-cr-2-or-below.json
--rw-rw-r--   0 b         (1000) b         (1000)      452 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_destroy-undead-cr-3-or-below.json
--rw-rw-r--   0 b         (1000) b         (1000)      452 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_destroy-undead-cr-4-or-below.json
--rw-rw-r--   0 b         (1000) b         (1000)      420 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_diamond-soul.json
--rw-rw-r--   0 b         (1000) b         (1000)      725 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_divine-domain.json
--rw-rw-r--   0 b         (1000) b         (1000)      296 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_divine-health.json
--rw-rw-r--   0 b         (1000) b         (1000)      352 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_divine-intervention-improvement.json
--rw-rw-r--   0 b         (1000) b         (1000)      892 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_divine-intervention.json
--rw-rw-r--   0 b         (1000) b         (1000)      948 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_divine-sense.json
--rw-rw-r--   0 b         (1000) b         (1000)      579 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_divine-smite.json
--rw-rw-r--   0 b         (1000) b         (1000)      598 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_domain-spells-1.json
--rw-rw-r--   0 b         (1000) b         (1000)      598 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_domain-spells-2.json
--rw-rw-r--   0 b         (1000) b         (1000)      598 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_domain-spells-3.json
--rw-rw-r--   0 b         (1000) b         (1000)      598 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_domain-spells-4.json
--rw-rw-r--   0 b         (1000) b         (1000)      598 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_domain-spells-5.json
--rw-rw-r--   0 b         (1000) b         (1000)      526 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_druid-ability-score-improvement-1.json
--rw-rw-r--   0 b         (1000) b         (1000)      526 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_druid-ability-score-improvement-2.json
--rw-rw-r--   0 b         (1000) b         (1000)      527 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_druid-ability-score-improvement-3.json
--rw-rw-r--   0 b         (1000) b         (1000)      527 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_druid-ability-score-improvement-4.json
--rw-rw-r--   0 b         (1000) b         (1000)      527 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_druid-ability-score-improvement-5.json
--rw-rw-r--   0 b         (1000) b         (1000)      386 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_druid-circle.json
--rw-rw-r--   0 b         (1000) b         (1000)      368 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_druid-timeless-body.json
--rw-rw-r--   0 b         (1000) b         (1000)      500 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_druidic.json
--rw-rw-r--   0 b         (1000) b         (1000)     6107 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_eldritch-invocations.json
--rw-rw-r--   0 b         (1000) b         (1000)      582 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_eldritch-master.json
--rw-rw-r--   0 b         (1000) b         (1000)      365 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_elusive.json
--rw-rw-r--   0 b         (1000) b         (1000)      556 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_empty-body.json
--rw-rw-r--   0 b         (1000) b         (1000)      464 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_extra-attack-1.json
--rw-rw-r--   0 b         (1000) b         (1000)      469 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_extra-attack-2.json
--rw-rw-r--   0 b         (1000) b         (1000)      469 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_extra-attack-3.json
--rw-rw-r--   0 b         (1000) b         (1000)      315 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_fast-movement.json
--rw-rw-r--   0 b         (1000) b         (1000)     1129 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_favored-enemy-1-type.json
--rw-rw-r--   0 b         (1000) b         (1000)     1132 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_favored-enemy-2-types.json
--rw-rw-r--   0 b         (1000) b         (1000)     1139 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_favored-enemy-3-enemies.json
--rw-rw-r--   0 b         (1000) b         (1000)      517 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_feral-instinct.json
--rw-rw-r--   0 b         (1000) b         (1000)      601 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_feral-senses.json
--rw-rw-r--   0 b         (1000) b         (1000)      547 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_fighter-ability-score-improvement-1.json
--rw-rw-r--   0 b         (1000) b         (1000)      547 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_fighter-ability-score-improvement-2.json
--rw-rw-r--   0 b         (1000) b         (1000)      547 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_fighter-ability-score-improvement-3.json
--rw-rw-r--   0 b         (1000) b         (1000)      548 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_fighter-ability-score-improvement-4.json
--rw-rw-r--   0 b         (1000) b         (1000)      548 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_fighter-ability-score-improvement-5.json
--rw-rw-r--   0 b         (1000) b         (1000)      548 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_fighter-ability-score-improvement-6.json
--rw-rw-r--   0 b         (1000) b         (1000)      548 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_fighter-ability-score-improvement-7.json
--rw-rw-r--   0 b         (1000) b         (1000)     1707 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_fighter-fighting-style.json
--rw-rw-r--   0 b         (1000) b         (1000)      421 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_flexible-casting-converting-spell-slot.json
--rw-rw-r--   0 b         (1000) b         (1000)      619 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_flexible-casting-creating-spell-slots.json
--rw-rw-r--   0 b         (1000) b         (1000)      344 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_flurry-of-blows.json
--rw-rw-r--   0 b         (1000) b         (1000)      538 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_foe-slayer.json
--rw-rw-r--   0 b         (1000) b         (1000)      358 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_font-of-inspiration.json
--rw-rw-r--   0 b         (1000) b         (1000)      695 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_font-of-magic.json
--rw-rw-r--   0 b         (1000) b         (1000)      843 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_hide-in-plain-sight.json
--rw-rw-r--   0 b         (1000) b         (1000)      571 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_improved-divine-smite.json
--rw-rw-r--   0 b         (1000) b         (1000)      539 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_indomitable-1-use.json
--rw-rw-r--   0 b         (1000) b         (1000)      543 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_indomitable-2-uses.json
--rw-rw-r--   0 b         (1000) b         (1000)      543 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_indomitable-3-uses.json
--rw-rw-r--   0 b         (1000) b         (1000)      375 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_indomitable-might.json
--rw-rw-r--   0 b         (1000) b         (1000)      383 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_jack-of-all-trades.json
--rw-rw-r--   0 b         (1000) b         (1000)      377 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_ki-empowered-strikes.json
--rw-rw-r--   0 b         (1000) b         (1000)     1112 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_ki.json
--rw-rw-r--   0 b         (1000) b         (1000)      937 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_lay-on-hands.json
--rw-rw-r--   0 b         (1000) b         (1000)      673 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_magical-secrets-1.json
--rw-rw-r--   0 b         (1000) b         (1000)      673 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_magical-secrets-2.json
--rw-rw-r--   0 b         (1000) b         (1000)      673 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_magical-secrets-3.json
--rw-rw-r--   0 b         (1000) b         (1000)      453 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_martial-archetype.json
--rw-rw-r--   0 b         (1000) b         (1000)     1544 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_martial-arts.json
--rw-rw-r--   0 b         (1000) b         (1000)     1947 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_metamagic-1.json
--rw-rw-r--   0 b         (1000) b         (1000)     1948 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_metamagic-2.json
--rw-rw-r--   0 b         (1000) b         (1000)     1948 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_metamagic-3.json
--rw-rw-r--   0 b         (1000) b         (1000)      415 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_monastic-tradition.json
--rw-rw-r--   0 b         (1000) b         (1000)      521 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_monk-ability-score-improvement-1.json
--rw-rw-r--   0 b         (1000) b         (1000)      521 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_monk-ability-score-improvement-2.json
--rw-rw-r--   0 b         (1000) b         (1000)      522 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_monk-ability-score-improvement-3.json
--rw-rw-r--   0 b         (1000) b         (1000)      522 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_monk-ability-score-improvement-4.json
--rw-rw-r--   0 b         (1000) b         (1000)      522 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_monk-ability-score-improvement-5.json
--rw-rw-r--   0 b         (1000) b         (1000)      563 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_monk-evasion.json
--rw-rw-r--   0 b         (1000) b         (1000)      327 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_monk-extra-attack.json
--rw-rw-r--   0 b         (1000) b         (1000)      424 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_monk-timeless-body.json
--rw-rw-r--   0 b         (1000) b         (1000)      379 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_monk-unarmored-defense.json
--rw-rw-r--   0 b         (1000) b         (1000)      810 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_mystic-arcanum-6th-level.json
--rw-rw-r--   0 b         (1000) b         (1000)      810 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_mystic-arcanum-7th-level.json
--rw-rw-r--   0 b         (1000) b         (1000)      810 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_mystic-arcanum-8th-level.json
--rw-rw-r--   0 b         (1000) b         (1000)      810 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_mystic-arcanum-9th-level.json
--rw-rw-r--   0 b         (1000) b         (1000)     1360 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_natural-explorer-1-terrain-type.json
--rw-rw-r--   0 b         (1000) b         (1000)     1363 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_natural-explorer-2-terrain-types.json
--rw-rw-r--   0 b         (1000) b         (1000)     1364 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_natural-explorer-3-terrain-types.json
--rw-rw-r--   0 b         (1000) b         (1000)      607 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_oath-spells.json
--rw-rw-r--   0 b         (1000) b         (1000)      421 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_otherworldly-patron.json
--rw-rw-r--   0 b         (1000) b         (1000)      922 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_pact-boon.json
--rw-rw-r--   0 b         (1000) b         (1000)      360 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_pact-magic.json
--rw-rw-r--   0 b         (1000) b         (1000)      536 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_paladin-ability-score-improvement-1.json
--rw-rw-r--   0 b         (1000) b         (1000)      536 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_paladin-ability-score-improvement-2.json
--rw-rw-r--   0 b         (1000) b         (1000)      537 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_paladin-ability-score-improvement-3.json
--rw-rw-r--   0 b         (1000) b         (1000)      537 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_paladin-ability-score-improvement-4.json
--rw-rw-r--   0 b         (1000) b         (1000)      537 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_paladin-ability-score-improvement-5.json
--rw-rw-r--   0 b         (1000) b         (1000)      342 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_paladin-extra-attack.json
--rw-rw-r--   0 b         (1000) b         (1000)     1264 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_paladin-fighting-style.json
--rw-rw-r--   0 b         (1000) b         (1000)      295 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_patient-defense.json
--rw-rw-r--   0 b         (1000) b         (1000)      306 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_perfect-self.json
--rw-rw-r--   0 b         (1000) b         (1000)      353 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_persistent-rage.json
--rw-rw-r--   0 b         (1000) b         (1000)      373 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_primal-champion.json
--rw-rw-r--   0 b         (1000) b         (1000)      489 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_primal-path.json
--rw-rw-r--   0 b         (1000) b         (1000)      696 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_primeval-awareness.json
--rw-rw-r--   0 b         (1000) b         (1000)      309 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_purity-of-body.json
--rw-rw-r--   0 b         (1000) b         (1000)     1204 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_rage.json
--rw-rw-r--   0 b         (1000) b         (1000)      531 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_ranger-ability-score-improvement-1.json
--rw-rw-r--   0 b         (1000) b         (1000)      531 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_ranger-ability-score-improvement-2.json
--rw-rw-r--   0 b         (1000) b         (1000)      532 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_ranger-ability-score-improvement-3.json
--rw-rw-r--   0 b         (1000) b         (1000)      532 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_ranger-ability-score-improvement-4.json
--rw-rw-r--   0 b         (1000) b         (1000)      532 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_ranger-ability-score-improvement-5.json
--rw-rw-r--   0 b         (1000) b         (1000)      393 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_ranger-archetype.json
--rw-rw-r--   0 b         (1000) b         (1000)      337 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_ranger-extra-attack.json
--rw-rw-r--   0 b         (1000) b         (1000)     1311 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_ranger-fighting-style.json
--rw-rw-r--   0 b         (1000) b         (1000)      651 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_ranger-lands-stride.json
--rw-rw-r--   0 b         (1000) b         (1000)      570 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_reckless-attack.json
--rw-rw-r--   0 b         (1000) b         (1000)      612 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_relentless-rage.json
--rw-rw-r--   0 b         (1000) b         (1000)      425 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_reliable-talent.json
--rw-rw-r--   0 b         (1000) b         (1000)      532 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_rogue-ability-score-improvement-1.json
--rw-rw-r--   0 b         (1000) b         (1000)      532 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_rogue-ability-score-improvement-2.json
--rw-rw-r--   0 b         (1000) b         (1000)      533 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_rogue-ability-score-improvement-3.json
--rw-rw-r--   0 b         (1000) b         (1000)      533 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_rogue-ability-score-improvement-4.json
--rw-rw-r--   0 b         (1000) b         (1000)      533 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_rogue-ability-score-improvement-5.json
--rw-rw-r--   0 b         (1000) b         (1000)      533 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_rogue-ability-score-improvement-6.json
--rw-rw-r--   0 b         (1000) b         (1000)      556 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_rogue-evasion.json
--rw-rw-r--   0 b         (1000) b         (1000)     6307 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_rogue-expertise-1.json
--rw-rw-r--   0 b         (1000) b         (1000)     3434 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_rogue-expertise-2.json
--rw-rw-r--   0 b         (1000) b         (1000)      502 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_roguish-archetype.json
--rw-rw-r--   0 b         (1000) b         (1000)      604 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_sacred-oath.json
--rw-rw-r--   0 b         (1000) b         (1000)      488 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_second-wind.json
--rw-rw-r--   0 b         (1000) b         (1000)      762 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_signature-spell.json
--rw-rw-r--   0 b         (1000) b         (1000)      315 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_slippery-mind.json
--rw-rw-r--   0 b         (1000) b         (1000)      347 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_slow-fall.json
--rw-rw-r--   0 b         (1000) b         (1000)      793 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_sneak-attack.json
--rw-rw-r--   0 b         (1000) b         (1000)      692 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_song-of-rest-d10.json
--rw-rw-r--   0 b         (1000) b         (1000)      692 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_song-of-rest-d12.json
--rw-rw-r--   0 b         (1000) b         (1000)      688 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_song-of-rest-d6.json
--rw-rw-r--   0 b         (1000) b         (1000)      688 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_song-of-rest-d8.json
--rw-rw-r--   0 b         (1000) b         (1000)      541 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_sorcerer-ability-score-improvement-1.json
--rw-rw-r--   0 b         (1000) b         (1000)      541 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_sorcerer-ability-score-improvement-2.json
--rw-rw-r--   0 b         (1000) b         (1000)      542 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_sorcerer-ability-score-improvement-3.json
--rw-rw-r--   0 b         (1000) b         (1000)      542 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_sorcerer-ability-score-improvement-4.json
--rw-rw-r--   0 b         (1000) b         (1000)      542 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_sorcerer-ability-score-improvement-5.json
--rw-rw-r--   0 b         (1000) b         (1000)      447 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_sorcerous-origin.json
--rw-rw-r--   0 b         (1000) b         (1000)      330 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_sorcerous-restoration.json
--rw-rw-r--   0 b         (1000) b         (1000)      728 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_spell-mastery.json
--rw-rw-r--   0 b         (1000) b         (1000)      464 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_spellcasting-bard.json
--rw-rw-r--   0 b         (1000) b         (1000)      340 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_spellcasting-cleric.json
--rw-rw-r--   0 b         (1000) b         (1000)      378 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_spellcasting-druid.json
--rw-rw-r--   0 b         (1000) b         (1000)      406 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_spellcasting-paladin.json
--rw-rw-r--   0 b         (1000) b         (1000)      406 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_spellcasting-ranger.json
--rw-rw-r--   0 b         (1000) b         (1000)      481 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_spellcasting-sorcerer.json
--rw-rw-r--   0 b         (1000) b         (1000)      402 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_spellcasting-wizard.json
--rw-rw-r--   0 b         (1000) b         (1000)      358 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_step-of-the-wind.json
--rw-rw-r--   0 b         (1000) b         (1000)      345 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_stillness-of-mind.json
--rw-rw-r--   0 b         (1000) b         (1000)      540 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_stroke-of-luck.json
--rw-rw-r--   0 b         (1000) b         (1000)      512 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_stunning-strike.json
--rw-rw-r--   0 b         (1000) b         (1000)      334 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_superior-inspiration.json
--rw-rw-r--   0 b         (1000) b         (1000)      846 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_thieves-cant.json
--rw-rw-r--   0 b         (1000) b         (1000)      440 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_tongue-of-the-sun-and-moon.json
--rw-rw-r--   0 b         (1000) b         (1000)      556 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_unarmored-movement-1.json
--rw-rw-r--   0 b         (1000) b         (1000)      556 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_unarmored-movement-2.json
--rw-rw-r--   0 b         (1000) b         (1000)      360 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_uncanny-dodge.json
--rw-rw-r--   0 b         (1000) b         (1000)      361 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_vanish.json
--rw-rw-r--   0 b         (1000) b         (1000)      536 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_warlock-ability-score-improvement-1.json
--rw-rw-r--   0 b         (1000) b         (1000)      536 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_warlock-ability-score-improvement-2.json
--rw-rw-r--   0 b         (1000) b         (1000)      537 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_warlock-ability-score-improvement-3.json
--rw-rw-r--   0 b         (1000) b         (1000)      537 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_warlock-ability-score-improvement-4.json
--rw-rw-r--   0 b         (1000) b         (1000)      537 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_warlock-ability-score-improvement-5.json
--rw-rw-r--   0 b         (1000) b         (1000)     3304 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_wild-shape-cr-1-2-or-below-no-flying-speed.json
--rw-rw-r--   0 b         (1000) b         (1000)     3328 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_wild-shape-cr-1-4-or-below-no-flying-or-swim-speed.json
--rw-rw-r--   0 b         (1000) b         (1000)     3249 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_wild-shape-cr-1-or-below.json
--rw-rw-r--   0 b         (1000) b         (1000)      531 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_wizard-ability-score-improvement-1.json
--rw-rw-r--   0 b         (1000) b         (1000)      531 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_wizard-ability-score-improvement-2.json
--rw-rw-r--   0 b         (1000) b         (1000)      532 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_wizard-ability-score-improvement-3.json
--rw-rw-r--   0 b         (1000) b         (1000)      532 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_wizard-ability-score-improvement-4.json
--rw-rw-r--   0 b         (1000) b         (1000)      532 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_features_wizard-ability-score-improvement-5.json
--rw-rw-r--   0 b         (1000) b         (1000)    28083 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters.json
--rw-rw-r--   0 b         (1000) b         (1000)     5182 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_aboleth.json
--rw-rw-r--   0 b         (1000) b         (1000)     2451 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_acolyte.json
--rw-rw-r--   0 b         (1000) b         (1000)     5211 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_adult-black-dragon.json
--rw-rw-r--   0 b         (1000) b         (1000)     5138 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_adult-blue-dragon.json
--rw-rw-r--   0 b         (1000) b         (1000)     5890 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_adult-brass-dragon.json
--rw-rw-r--   0 b         (1000) b         (1000)     5817 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_adult-bronze-dragon.json
--rw-rw-r--   0 b         (1000) b         (1000)     6007 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_adult-copper-dragon.json
--rw-rw-r--   0 b         (1000) b         (1000)     6028 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_adult-gold-dragon.json
--rw-rw-r--   0 b         (1000) b         (1000)     5636 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_adult-green-dragon.json
--rw-rw-r--   0 b         (1000) b         (1000)     5058 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_adult-red-dragon.json
--rw-rw-r--   0 b         (1000) b         (1000)     5875 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_adult-silver-dragon.json
--rw-rw-r--   0 b         (1000) b         (1000)     5302 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_adult-white-dragon.json
--rw-rw-r--   0 b         (1000) b         (1000)     2911 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_air-elemental.json
--rw-rw-r--   0 b         (1000) b         (1000)     5230 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_ancient-black-dragon.json
--rw-rw-r--   0 b         (1000) b         (1000)     5158 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_ancient-blue-dragon.json
--rw-rw-r--   0 b         (1000) b         (1000)     6589 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_ancient-brass-dragon.json
--rw-rw-r--   0 b         (1000) b         (1000)     6518 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_ancient-bronze-dragon.json
--rw-rw-r--   0 b         (1000) b         (1000)     6707 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_ancient-copper-dragon.json
--rw-rw-r--   0 b         (1000) b         (1000)     6734 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_ancient-gold-dragon.json
--rw-rw-r--   0 b         (1000) b         (1000)     5655 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_ancient-green-dragon.json
--rw-rw-r--   0 b         (1000) b         (1000)     5090 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_ancient-red-dragon.json
--rw-rw-r--   0 b         (1000) b         (1000)     6582 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_ancient-silver-dragon.json
--rw-rw-r--   0 b         (1000) b         (1000)     5319 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_ancient-white-dragon.json
--rw-rw-r--   0 b         (1000) b         (1000)     6803 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_androsphinx.json
--rw-rw-r--   0 b         (1000) b         (1000)     2304 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_animated-armor.json
--rw-rw-r--   0 b         (1000) b         (1000)     2143 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_ankheg.json
--rw-rw-r--   0 b         (1000) b         (1000)     1740 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_ape.json
--rw-rw-r--   0 b         (1000) b         (1000)     5732 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_archmage.json
--rw-rw-r--   0 b         (1000) b         (1000)     4238 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_assassin.json
--rw-rw-r--   0 b         (1000) b         (1000)     1296 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_awakened-shrub.json
--rw-rw-r--   0 b         (1000) b         (1000)     1328 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_awakened-tree.json
--rw-rw-r--   0 b         (1000) b         (1000)     1188 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_axe-beak.json
--rw-rw-r--   0 b         (1000) b         (1000)     2190 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_azer.json
--rw-rw-r--   0 b         (1000) b         (1000)     1155 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_baboon.json
--rw-rw-r--   0 b         (1000) b         (1000)     1081 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_badger.json
--rw-rw-r--   0 b         (1000) b         (1000)     4252 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_balor.json
--rw-rw-r--   0 b         (1000) b         (1000)     3658 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_bandit-captain.json
--rw-rw-r--   0 b         (1000) b         (1000)     1875 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_bandit.json
--rw-rw-r--   0 b         (1000) b         (1000)     3933 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_barbed-devil.json
--rw-rw-r--   0 b         (1000) b         (1000)     2207 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_basilisk.json
--rw-rw-r--   0 b         (1000) b         (1000)     1148 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_bat.json
--rw-rw-r--   0 b         (1000) b         (1000)     3279 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_bearded-devil.json
--rw-rw-r--   0 b         (1000) b         (1000)     3784 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_behir.json
--rw-rw-r--   0 b         (1000) b         (1000)     1341 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_berserker.json
--rw-rw-r--   0 b         (1000) b         (1000)     1630 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_black-bear.json
--rw-rw-r--   0 b         (1000) b         (1000)     2744 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_black-dragon-wyrmling.json
--rw-rw-r--   0 b         (1000) b         (1000)     3172 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_black-pudding.json
--rw-rw-r--   0 b         (1000) b         (1000)     1842 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_blink-dog.json
--rw-rw-r--   0 b         (1000) b         (1000)     1657 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_blood-hawk.json
--rw-rw-r--   0 b         (1000) b         (1000)     2675 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_blue-dragon-wyrmling.json
--rw-rw-r--   0 b         (1000) b         (1000)     1582 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_boar.json
--rw-rw-r--   0 b         (1000) b         (1000)     3021 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_bone-devil.json
--rw-rw-r--   0 b         (1000) b         (1000)     3157 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_brass-dragon-wyrmling.json
--rw-rw-r--   0 b         (1000) b         (1000)     3220 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_bronze-dragon-wyrmling.json
--rw-rw-r--   0 b         (1000) b         (1000)     1766 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_brown-bear.json
--rw-rw-r--   0 b         (1000) b         (1000)     2136 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_bugbear.json
--rw-rw-r--   0 b         (1000) b         (1000)     1995 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_bulette.json
--rw-rw-r--   0 b         (1000) b         (1000)      943 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_camel.json
--rw-rw-r--   0 b         (1000) b         (1000)     1294 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_cat.json
--rw-rw-r--   0 b         (1000) b         (1000)     2873 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_centaur.json
--rw-rw-r--   0 b         (1000) b         (1000)     3504 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_chain-devil.json
--rw-rw-r--   0 b         (1000) b         (1000)     3576 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_chimera.json
--rw-rw-r--   0 b         (1000) b         (1000)     2695 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_chuul.json
--rw-rw-r--   0 b         (1000) b         (1000)     3368 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_clay-golem.json
--rw-rw-r--   0 b         (1000) b         (1000)     4159 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_cloaker.json
--rw-rw-r--   0 b         (1000) b         (1000)     3867 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_cloud-giant.json
--rw-rw-r--   0 b         (1000) b         (1000)     1321 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_cockatrice.json
--rw-rw-r--   0 b         (1000) b         (1000)     1121 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_commoner.json
--rw-rw-r--   0 b         (1000) b         (1000)     1468 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_constrictor-snake.json
--rw-rw-r--   0 b         (1000) b         (1000)     3405 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_copper-dragon-wyrmling.json
--rw-rw-r--   0 b         (1000) b         (1000)     5448 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_couatl.json
--rw-rw-r--   0 b         (1000) b         (1000)     1162 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_crab.json
--rw-rw-r--   0 b         (1000) b         (1000)     1380 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_crocodile.json
--rw-rw-r--   0 b         (1000) b         (1000)     3245 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_cult-fanatic.json
--rw-rw-r--   0 b         (1000) b         (1000)     1801 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_cultist.json
--rw-rw-r--   0 b         (1000) b         (1000)     2652 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_darkmantle.json
--rw-rw-r--   0 b         (1000) b         (1000)     2303 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_death-dog.json
--rw-rw-r--   0 b         (1000) b         (1000)     3318 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_deep-gnome-svirfneblin.json
--rw-rw-r--   0 b         (1000) b         (1000)      924 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_deer.json
--rw-rw-r--   0 b         (1000) b         (1000)     4196 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_deva.json
--rw-rw-r--   0 b         (1000) b         (1000)     1643 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_dire-wolf.json
--rw-rw-r--   0 b         (1000) b         (1000)     5483 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_djinni.json
--rw-rw-r--   0 b         (1000) b         (1000)     2826 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_doppelganger.json
--rw-rw-r--   0 b         (1000) b         (1000)      972 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_draft-horse.json
--rw-rw-r--   0 b         (1000) b         (1000)     3673 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_dragon-turtle.json
--rw-rw-r--   0 b         (1000) b         (1000)     2407 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_dretch.json
--rw-rw-r--   0 b         (1000) b         (1000)     4770 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_drider.json
--rw-rw-r--   0 b         (1000) b         (1000)     3066 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_drow.json
--rw-rw-r--   0 b         (1000) b         (1000)     3695 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_druid.json
--rw-rw-r--   0 b         (1000) b         (1000)     4354 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_dryad.json
--rw-rw-r--   0 b         (1000) b         (1000)     2854 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_duergar.json
--rw-rw-r--   0 b         (1000) b         (1000)     2758 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_dust-mephit.json
--rw-rw-r--   0 b         (1000) b         (1000)     1199 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_eagle.json
--rw-rw-r--   0 b         (1000) b         (1000)     2060 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_earth-elemental.json
--rw-rw-r--   0 b         (1000) b         (1000)     4245 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_efreeti.json
--rw-rw-r--   0 b         (1000) b         (1000)     1593 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_elephant.json
--rw-rw-r--   0 b         (1000) b         (1000)     1535 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_elk.json
--rw-rw-r--   0 b         (1000) b         (1000)     4267 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_erinyes.json
--rw-rw-r--   0 b         (1000) b         (1000)     3216 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_ettercap.json
--rw-rw-r--   0 b         (1000) b         (1000)     1991 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_ettin.json
--rw-rw-r--   0 b         (1000) b         (1000)     3030 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_fire-elemental.json
--rw-rw-r--   0 b         (1000) b         (1000)     2242 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_fire-giant.json
--rw-rw-r--   0 b         (1000) b         (1000)     3315 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_flesh-golem.json
--rw-rw-r--   0 b         (1000) b         (1000)     1481 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_flying-snake.json
--rw-rw-r--   0 b         (1000) b         (1000)     2155 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_flying-sword.json
--rw-rw-r--   0 b         (1000) b         (1000)     1346 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_frog.json
--rw-rw-r--   0 b         (1000) b         (1000)     2165 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_frost-giant.json
--rw-rw-r--   0 b         (1000) b         (1000)     2018 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_gargoyle.json
--rw-rw-r--   0 b         (1000) b         (1000)     3508 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_gelatinous-cube.json
--rw-rw-r--   0 b         (1000) b         (1000)     2314 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_ghast.json
--rw-rw-r--   0 b         (1000) b         (1000)     4590 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_ghost.json
--rw-rw-r--   0 b         (1000) b         (1000)     1756 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_ghoul.json
--rw-rw-r--   0 b         (1000) b         (1000)     1726 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_giant-ape.json
--rw-rw-r--   0 b         (1000) b         (1000)     1661 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_giant-badger.json
--rw-rw-r--   0 b         (1000) b         (1000)     1188 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_giant-bat.json
--rw-rw-r--   0 b         (1000) b         (1000)     1471 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_giant-boar.json
--rw-rw-r--   0 b         (1000) b         (1000)     1297 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_giant-centipede.json
--rw-rw-r--   0 b         (1000) b         (1000)     1619 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_giant-constrictor-snake.json
--rw-rw-r--   0 b         (1000) b         (1000)     1312 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_giant-crab.json
--rw-rw-r--   0 b         (1000) b         (1000)     2032 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_giant-crocodile.json
--rw-rw-r--   0 b         (1000) b         (1000)     2063 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_giant-eagle.json
--rw-rw-r--   0 b         (1000) b         (1000)     2093 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_giant-elk.json
--rw-rw-r--   0 b         (1000) b         (1000)     1465 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_giant-fire-beetle.json
--rw-rw-r--   0 b         (1000) b         (1000)     2183 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_giant-frog.json
--rw-rw-r--   0 b         (1000) b         (1000)     1407 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_giant-goat.json
--rw-rw-r--   0 b         (1000) b         (1000)     1291 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_giant-hyena.json
--rw-rw-r--   0 b         (1000) b         (1000)     1207 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_giant-lizard.json
--rw-rw-r--   0 b         (1000) b         (1000)     2138 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_giant-octopus.json
--rw-rw-r--   0 b         (1000) b         (1000)     1559 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_giant-owl.json
--rw-rw-r--   0 b         (1000) b         (1000)     1315 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_giant-poisonous-snake.json
--rw-rw-r--   0 b         (1000) b         (1000)     1659 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_giant-rat-diseased.json
--rw-rw-r--   0 b         (1000) b         (1000)     1274 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_giant-rat.json
--rw-rw-r--   0 b         (1000) b         (1000)     1829 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_giant-scorpion.json
--rw-rw-r--   0 b         (1000) b         (1000)     1533 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_giant-sea-horse.json
--rw-rw-r--   0 b         (1000) b         (1000)     1509 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_giant-shark.json
--rw-rw-r--   0 b         (1000) b         (1000)     2679 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_giant-spider.json
--rw-rw-r--   0 b         (1000) b         (1000)     2073 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_giant-toad.json
--rw-rw-r--   0 b         (1000) b         (1000)     2291 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_giant-vulture.json
--rw-rw-r--   0 b         (1000) b         (1000)     1330 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_giant-wasp.json
--rw-rw-r--   0 b         (1000) b         (1000)     1372 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_giant-weasel.json
--rw-rw-r--   0 b         (1000) b         (1000)     2195 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_giant-wolf-spider.json
--rw-rw-r--   0 b         (1000) b         (1000)     3214 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_gibbering-mouther.json
--rw-rw-r--   0 b         (1000) b         (1000)     4287 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_glabrezu.json
--rw-rw-r--   0 b         (1000) b         (1000)     4348 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_gladiator.json
--rw-rw-r--   0 b         (1000) b         (1000)     2362 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_gnoll.json
--rw-rw-r--   0 b         (1000) b         (1000)     1382 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_goat.json
--rw-rw-r--   0 b         (1000) b         (1000)     1774 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_goblin.json
--rw-rw-r--   0 b         (1000) b         (1000)     3294 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_gold-dragon-wyrmling.json
--rw-rw-r--   0 b         (1000) b         (1000)     2514 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_gorgon.json
--rw-rw-r--   0 b         (1000) b         (1000)     2635 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_gray-ooze.json
--rw-rw-r--   0 b         (1000) b         (1000)     2771 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_green-dragon-wyrmling.json
--rw-rw-r--   0 b         (1000) b         (1000)     3580 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_green-hag.json
--rw-rw-r--   0 b         (1000) b         (1000)     1791 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_grick.json
--rw-rw-r--   0 b         (1000) b         (1000)     1785 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_griffon.json
--rw-rw-r--   0 b         (1000) b         (1000)     2072 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_grimlock.json
--rw-rw-r--   0 b         (1000) b         (1000)     1860 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_guard.json
--rw-rw-r--   0 b         (1000) b         (1000)     4418 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_guardian-naga.json
--rw-rw-r--   0 b         (1000) b         (1000)     4618 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_gynosphinx.json
--rw-rw-r--   0 b         (1000) b         (1000)     3040 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_half-red-dragon-veteran.json
--rw-rw-r--   0 b         (1000) b         (1000)     2591 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_harpy.json
--rw-rw-r--   0 b         (1000) b         (1000)     1172 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_hawk.json
--rw-rw-r--   0 b         (1000) b         (1000)     2192 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_hell-hound.json
--rw-rw-r--   0 b         (1000) b         (1000)     2689 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_hezrou.json
--rw-rw-r--   0 b         (1000) b         (1000)     1605 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_hill-giant.json
--rw-rw-r--   0 b         (1000) b         (1000)     1777 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_hippogriff.json
--rw-rw-r--   0 b         (1000) b         (1000)     2086 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_hobgoblin.json
--rw-rw-r--   0 b         (1000) b         (1000)     1632 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_homunculus.json
--rw-rw-r--   0 b         (1000) b         (1000)     4160 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_horned-devil.json
--rw-rw-r--   0 b         (1000) b         (1000)     1591 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_hunter-shark.json
--rw-rw-r--   0 b         (1000) b         (1000)     2222 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_hydra.json
--rw-rw-r--   0 b         (1000) b         (1000)     1262 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_hyena.json
--rw-rw-r--   0 b         (1000) b         (1000)     4586 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_ice-devil.json
--rw-rw-r--   0 b         (1000) b         (1000)     3181 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_ice-mephit.json
--rw-rw-r--   0 b         (1000) b         (1000)     2722 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_imp.json
--rw-rw-r--   0 b         (1000) b         (1000)     2561 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_invisible-stalker.json
--rw-rw-r--   0 b         (1000) b         (1000)     3626 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_iron-golem.json
--rw-rw-r--   0 b         (1000) b         (1000)     1402 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_jackal.json
--rw-rw-r--   0 b         (1000) b         (1000)     1404 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_killer-whale.json
--rw-rw-r--   0 b         (1000) b         (1000)     2961 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_knight.json
--rw-rw-r--   0 b         (1000) b         (1000)     1683 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_kobold.json
--rw-rw-r--   0 b         (1000) b         (1000)     6598 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_kraken.json
--rw-rw-r--   0 b         (1000) b         (1000)     4022 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_lamia.json
--rw-rw-r--   0 b         (1000) b         (1000)     1646 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_lemure.json
--rw-rw-r--   0 b         (1000) b         (1000)     7447 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_lich.json
--rw-rw-r--   0 b         (1000) b         (1000)     2330 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_lion.json
--rw-rw-r--   0 b         (1000) b         (1000)      960 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_lizard.json
--rw-rw-r--   0 b         (1000) b         (1000)     4033 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_lizardfolk.json
--rw-rw-r--   0 b         (1000) b         (1000)     3800 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_mage.json
--rw-rw-r--   0 b         (1000) b         (1000)     3042 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_magma-mephit.json
--rw-rw-r--   0 b         (1000) b         (1000)     2024 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_magmin.json
--rw-rw-r--   0 b         (1000) b         (1000)     1791 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_mammoth.json
--rw-rw-r--   0 b         (1000) b         (1000)     2326 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_manticore.json
--rw-rw-r--   0 b         (1000) b         (1000)     3257 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_marilith.json
--rw-rw-r--   0 b         (1000) b         (1000)     1530 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_mastiff.json
--rw-rw-r--   0 b         (1000) b         (1000)     4285 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_medusa.json
--rw-rw-r--   0 b         (1000) b         (1000)     1612 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_merfolk.json
--rw-rw-r--   0 b         (1000) b         (1000)     2722 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_merrow.json
--rw-rw-r--   0 b         (1000) b         (1000)     2528 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_mimic.json
--rw-rw-r--   0 b         (1000) b         (1000)     1842 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_minotaur-skeleton.json
--rw-rw-r--   0 b         (1000) b         (1000)     2077 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_minotaur.json
--rw-rw-r--   0 b         (1000) b         (1000)     1234 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_mule.json
--rw-rw-r--   0 b         (1000) b         (1000)     7673 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_mummy-lord.json
--rw-rw-r--   0 b         (1000) b         (1000)     3119 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_mummy.json
--rw-rw-r--   0 b         (1000) b         (1000)     3471 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_nalfeshnee.json
--rw-rw-r--   0 b         (1000) b         (1000)     5078 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_night-hag.json
--rw-rw-r--   0 b         (1000) b         (1000)     1632 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_nightmare.json
--rw-rw-r--   0 b         (1000) b         (1000)     2051 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_noble.json
--rw-rw-r--   0 b         (1000) b         (1000)     2257 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_ochre-jelly.json
--rw-rw-r--   0 b         (1000) b         (1000)     2071 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_octopus.json
--rw-rw-r--   0 b         (1000) b         (1000)     1529 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_ogre-zombie.json
--rw-rw-r--   0 b         (1000) b         (1000)     1408 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_ogre.json
--rw-rw-r--   0 b         (1000) b         (1000)     4881 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_oni.json
--rw-rw-r--   0 b         (1000) b         (1000)     1682 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_orc.json
--rw-rw-r--   0 b         (1000) b         (1000)     3229 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_otyugh.json
--rw-rw-r--   0 b         (1000) b         (1000)     1454 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_owl.json
--rw-rw-r--   0 b         (1000) b         (1000)     1796 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_owlbear.json
--rw-rw-r--   0 b         (1000) b         (1000)     2062 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_panther.json
--rw-rw-r--   0 b         (1000) b         (1000)     1589 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_pegasus.json
--rw-rw-r--   0 b         (1000) b         (1000)     2155 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_phase-spider.json
--rw-rw-r--   0 b         (1000) b         (1000)     4979 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_pit-fiend.json
--rw-rw-r--   0 b         (1000) b         (1000)     4633 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_planetar.json
--rw-rw-r--   0 b         (1000) b         (1000)     1335 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_plesiosaurus.json
--rw-rw-r--   0 b         (1000) b         (1000)     1143 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_poisonous-snake.json
--rw-rw-r--   0 b         (1000) b         (1000)     1763 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_polar-bear.json
--rw-rw-r--   0 b         (1000) b         (1000)      951 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_pony.json
--rw-rw-r--   0 b         (1000) b         (1000)     3726 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_priest.json
--rw-rw-r--   0 b         (1000) b         (1000)     2365 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_pseudodragon.json
--rw-rw-r--   0 b         (1000) b         (1000)     2905 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_purple-worm.json
--rw-rw-r--   0 b         (1000) b         (1000)     2872 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_quasit.json
--rw-rw-r--   0 b         (1000) b         (1000)     1415 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_quipper.json
--rw-rw-r--   0 b         (1000) b         (1000)     4385 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_rakshasa.json
--rw-rw-r--   0 b         (1000) b         (1000)     1040 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_rat.json
--rw-rw-r--   0 b         (1000) b         (1000)     1324 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_raven.json
--rw-rw-r--   0 b         (1000) b         (1000)     2592 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_red-dragon-wyrmling.json
--rw-rw-r--   0 b         (1000) b         (1000)     1586 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_reef-shark.json
--rw-rw-r--   0 b         (1000) b         (1000)     2478 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_remorhaz.json
--rw-rw-r--   0 b         (1000) b         (1000)     1271 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_rhinoceros.json
--rw-rw-r--   0 b         (1000) b         (1000)      975 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_riding-horse.json
--rw-rw-r--   0 b         (1000) b         (1000)     2451 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_roc.json
--rw-rw-r--   0 b         (1000) b         (1000)     2775 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_roper.json
--rw-rw-r--   0 b         (1000) b         (1000)     2292 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_rug-of-smothering.json
--rw-rw-r--   0 b         (1000) b         (1000)     2163 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_rust-monster.json
--rw-rw-r--   0 b         (1000) b         (1000)     2079 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_saber-toothed-tiger.json
--rw-rw-r--   0 b         (1000) b         (1000)     3287 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_sahuagin.json
--rw-rw-r--   0 b         (1000) b         (1000)     2978 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_salamander.json
--rw-rw-r--   0 b         (1000) b         (1000)     2191 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_satyr.json
--rw-rw-r--   0 b         (1000) b         (1000)     1114 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_scorpion.json
--rw-rw-r--   0 b         (1000) b         (1000)     2673 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_scout.json
--rw-rw-r--   0 b         (1000) b         (1000)     2933 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_sea-hag.json
--rw-rw-r--   0 b         (1000) b         (1000)      738 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_sea-horse.json
--rw-rw-r--   0 b         (1000) b         (1000)     2581 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_shadow.json
--rw-rw-r--   0 b         (1000) b         (1000)     2442 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_shambling-mound.json
--rw-rw-r--   0 b         (1000) b         (1000)     3043 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_shield-guardian.json
--rw-rw-r--   0 b         (1000) b         (1000)     1344 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_shrieker.json
--rw-rw-r--   0 b         (1000) b         (1000)     3156 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_silver-dragon-wyrmling.json
--rw-rw-r--   0 b         (1000) b         (1000)     1541 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_skeleton.json
--rw-rw-r--   0 b         (1000) b         (1000)     6690 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_solar.json
--rw-rw-r--   0 b         (1000) b         (1000)     2545 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_specter.json
--rw-rw-r--   0 b         (1000) b         (1000)     1583 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_spider.json
--rw-rw-r--   0 b         (1000) b         (1000)     3819 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_spirit-naga.json
--rw-rw-r--   0 b         (1000) b         (1000)     2585 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_sprite.json
--rw-rw-r--   0 b         (1000) b         (1000)     2994 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_spy.json
--rw-rw-r--   0 b         (1000) b         (1000)     2702 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_steam-mephit.json
--rw-rw-r--   0 b         (1000) b         (1000)     1410 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_stirge.json
--rw-rw-r--   0 b         (1000) b         (1000)     2617 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_stone-giant.json
--rw-rw-r--   0 b         (1000) b         (1000)     2867 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_stone-golem.json
--rw-rw-r--   0 b         (1000) b         (1000)     4592 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_storm-giant.json
--rw-rw-r--   0 b         (1000) b         (1000)     3982 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_succubus-incubus.json
--rw-rw-r--   0 b         (1000) b         (1000)     2199 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_swarm-of-bats.json
--rw-rw-r--   0 b         (1000) b         (1000)     2033 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_swarm-of-beetles.json
--rw-rw-r--   0 b         (1000) b         (1000)     2194 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_swarm-of-centipedes.json
--rw-rw-r--   0 b         (1000) b         (1000)     2014 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_swarm-of-insects.json
--rw-rw-r--   0 b         (1000) b         (1000)     2184 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_swarm-of-poisonous-snakes.json
--rw-rw-r--   0 b         (1000) b         (1000)     2235 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_swarm-of-quippers.json
--rw-rw-r--   0 b         (1000) b         (1000)     2090 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_swarm-of-rats.json
--rw-rw-r--   0 b         (1000) b         (1000)     1982 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_swarm-of-ravens.json
--rw-rw-r--   0 b         (1000) b         (1000)     2334 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_swarm-of-spiders.json
--rw-rw-r--   0 b         (1000) b         (1000)     2005 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_swarm-of-wasps.json
--rw-rw-r--   0 b         (1000) b         (1000)     6911 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_tarrasque.json
--rw-rw-r--   0 b         (1000) b         (1000)     2056 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_thug.json
--rw-rw-r--   0 b         (1000) b         (1000)     2059 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_tiger.json
--rw-rw-r--   0 b         (1000) b         (1000)     2349 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_treant.json
--rw-rw-r--   0 b         (1000) b         (1000)     1979 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_tribal-warrior.json
--rw-rw-r--   0 b         (1000) b         (1000)     1609 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_triceratops.json
--rw-rw-r--   0 b         (1000) b         (1000)     2050 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_troll.json
--rw-rw-r--   0 b         (1000) b         (1000)     1920 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_tyrannosaurus-rex.json
--rw-rw-r--   0 b         (1000) b         (1000)     4630 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_unicorn.json
--rw-rw-r--   0 b         (1000) b         (1000)     7313 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_vampire-bat.json
--rw-rw-r--   0 b         (1000) b         (1000)     4923 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_vampire-mist.json
--rw-rw-r--   0 b         (1000) b         (1000)     4116 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_vampire-spawn.json
--rw-rw-r--   0 b         (1000) b         (1000)     8320 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_vampire-vampire.json
--rw-rw-r--   0 b         (1000) b         (1000)     2884 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_veteran.json
--rw-rw-r--   0 b         (1000) b         (1000)     1567 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_violet-fungus.json
--rw-rw-r--   0 b         (1000) b         (1000)     3457 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_vrock.json
--rw-rw-r--   0 b         (1000) b         (1000)     1418 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_vulture.json
--rw-rw-r--   0 b         (1000) b         (1000)     1225 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_warhorse-skeleton.json
--rw-rw-r--   0 b         (1000) b         (1000)     1350 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_warhorse.json
--rw-rw-r--   0 b         (1000) b         (1000)     3436 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_water-elemental.json
--rw-rw-r--   0 b         (1000) b         (1000)     1356 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_weasel.json
--rw-rw-r--   0 b         (1000) b         (1000)     2631 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_werebear-bear.json
--rw-rw-r--   0 b         (1000) b         (1000)     2212 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_werebear-human.json
--rw-rw-r--   0 b         (1000) b         (1000)     3360 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_werebear-hybrid.json
--rw-rw-r--   0 b         (1000) b         (1000)     2442 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_wereboar-boar.json
--rw-rw-r--   0 b         (1000) b         (1000)     2245 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_wereboar-human.json
--rw-rw-r--   0 b         (1000) b         (1000)     3298 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_wereboar-hybrid.json
--rw-rw-r--   0 b         (1000) b         (1000)     2956 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_wererat-human.json
--rw-rw-r--   0 b         (1000) b         (1000)     3780 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_wererat-hybrid.json
--rw-rw-r--   0 b         (1000) b         (1000)     2140 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_wererat-rat.json
--rw-rw-r--   0 b         (1000) b         (1000)     2893 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_weretiger-human.json
--rw-rw-r--   0 b         (1000) b         (1000)     4121 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_weretiger-hybrid.json
--rw-rw-r--   0 b         (1000) b         (1000)     2932 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_weretiger-tiger.json
--rw-rw-r--   0 b         (1000) b         (1000)     2585 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_werewolf-human.json
--rw-rw-r--   0 b         (1000) b         (1000)     2636 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_werewolf-hybrid.json
--rw-rw-r--   0 b         (1000) b         (1000)     2025 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_werewolf-wolf.json
--rw-rw-r--   0 b         (1000) b         (1000)     2632 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_white-dragon-wyrmling.json
--rw-rw-r--   0 b         (1000) b         (1000)     4020 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_wight.json
--rw-rw-r--   0 b         (1000) b         (1000)     2976 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_will-o-wisp.json
--rw-rw-r--   0 b         (1000) b         (1000)     2852 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_winter-wolf.json
--rw-rw-r--   0 b         (1000) b         (1000)     1669 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_wolf.json
--rw-rw-r--   0 b         (1000) b         (1000)     1800 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_worg.json
--rw-rw-r--   0 b         (1000) b         (1000)     2895 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_wraith.json
--rw-rw-r--   0 b         (1000) b         (1000)     2800 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_wyvern.json
--rw-rw-r--   0 b         (1000) b         (1000)     2379 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_xorn.json
--rw-rw-r--   0 b         (1000) b         (1000)     3300 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_young-black-dragon.json
--rw-rw-r--   0 b         (1000) b         (1000)     3231 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_young-blue-dragon.json
--rw-rw-r--   0 b         (1000) b         (1000)     3852 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_young-brass-dragon.json
--rw-rw-r--   0 b         (1000) b         (1000)     3905 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_young-bronze-dragon.json
--rw-rw-r--   0 b         (1000) b         (1000)     4095 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_young-copper-dragon.json
--rw-rw-r--   0 b         (1000) b         (1000)     4119 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_young-gold-dragon.json
--rw-rw-r--   0 b         (1000) b         (1000)     3463 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_young-green-dragon.json
--rw-rw-r--   0 b         (1000) b         (1000)     3153 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_young-red-dragon.json
--rw-rw-r--   0 b         (1000) b         (1000)     3968 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_young-silver-dragon.json
--rw-rw-r--   0 b         (1000) b         (1000)     3392 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_young-white-dragon.json
--rw-rw-r--   0 b         (1000) b         (1000)     1564 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_monsters_zombie.json
--rw-rw-r--   0 b         (1000) b         (1000)      361 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_proficiencies_all-armor.json
--rw-rw-r--   0 b         (1000) b         (1000)      259 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_proficiencies_clubs.json
--rw-rw-r--   0 b         (1000) b         (1000)      399 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_proficiencies_crossbows-light.json
--rw-rw-r--   0 b         (1000) b         (1000)      415 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_proficiencies_daggers.json
--rw-rw-r--   0 b         (1000) b         (1000)      403 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_proficiencies_darts.json
--rw-rw-r--   0 b         (1000) b         (1000)      377 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_proficiencies_hand-crossbows.json
--rw-rw-r--   0 b         (1000) b         (1000)      308 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_proficiencies_herbalism-kit.json
--rw-rw-r--   0 b         (1000) b         (1000)      277 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_proficiencies_javelins.json
--rw-rw-r--   0 b         (1000) b         (1000)      724 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_proficiencies_light-armor.json
--rw-rw-r--   0 b         (1000) b         (1000)      426 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_proficiencies_longswords.json
--rw-rw-r--   0 b         (1000) b         (1000)      259 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_proficiencies_maces.json
--rw-rw-r--   0 b         (1000) b         (1000)      558 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_proficiencies_martial-weapons.json
--rw-rw-r--   0 b         (1000) b         (1000)      529 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_proficiencies_medium-armor.json
--rw-rw-r--   0 b         (1000) b         (1000)      451 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_proficiencies_quarterstaffs.json
--rw-rw-r--   0 b         (1000) b         (1000)      334 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_proficiencies_rapiers.json
--rw-rw-r--   0 b         (1000) b         (1000)      586 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_proficiencies_saving-throw-cha.json
--rw-rw-r--   0 b         (1000) b         (1000)      460 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_proficiencies_saving-throw-con.json
--rw-rw-r--   0 b         (1000) b         (1000)      496 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_proficiencies_saving-throw-dex.json
--rw-rw-r--   0 b         (1000) b         (1000)      436 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_proficiencies_saving-throw-int.json
--rw-rw-r--   0 b         (1000) b         (1000)      517 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_proficiencies_saving-throw-str.json
--rw-rw-r--   0 b         (1000) b         (1000)      583 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_proficiencies_saving-throw-wis.json
--rw-rw-r--   0 b         (1000) b         (1000)      283 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_proficiencies_scimitars.json
--rw-rw-r--   0 b         (1000) b         (1000)      629 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_proficiencies_shields.json
--rw-rw-r--   0 b         (1000) b         (1000)      495 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_proficiencies_shortswords.json
--rw-rw-r--   0 b         (1000) b         (1000)      271 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_proficiencies_sickles.json
--rw-rw-r--   0 b         (1000) b         (1000)      885 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_proficiencies_simple-weapons.json
--rw-rw-r--   0 b         (1000) b         (1000)      409 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_proficiencies_slings.json
--rw-rw-r--   0 b         (1000) b         (1000)      265 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_proficiencies_spears.json
--rw-rw-r--   0 b         (1000) b         (1000)      310 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_proficiencies_thieves-tools.json
--rw-rw-r--   0 b         (1000) b         (1000)     8668 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_ability-checks.json
--rw-rw-r--   0 b         (1000) b         (1000)      898 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_ability-scores-and-modifiers.json
--rw-rw-r--   0 b         (1000) b         (1000)     5185 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_actions-in-combat.json
--rw-rw-r--   0 b         (1000) b         (1000)     2459 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_activating-an-item.json
--rw-rw-r--   0 b         (1000) b         (1000)     1844 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_advantage-and-disadvantage.json
--rw-rw-r--   0 b         (1000) b         (1000)     2341 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_attunement.json
--rw-rw-r--   0 b         (1000) b         (1000)     6080 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_between-adventures.json
--rw-rw-r--   0 b         (1000) b         (1000)    13605 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_casting-a-spell.json
--rw-rw-r--   0 b         (1000) b         (1000)     1449 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_cover.json
--rw-rw-r--   0 b         (1000) b         (1000)    10998 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_damage-and-healing.json
--rw-rw-r--   0 b         (1000) b         (1000)     5315 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_diseases.json
--rw-rw-r--   0 b         (1000) b         (1000)    12813 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_fantasy-historical-pantheons.json
--rw-rw-r--   0 b         (1000) b         (1000)     9411 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_madness.json
--rw-rw-r--   0 b         (1000) b         (1000)     8932 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_making-an-attack.json
--rw-rw-r--   0 b         (1000) b         (1000)     2341 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_mounted-combat.json
--rw-rw-r--   0 b         (1000) b         (1000)     6909 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_movement-and-position.json
--rw-rw-r--   0 b         (1000) b         (1000)     6367 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_movement.json
--rw-rw-r--   0 b         (1000) b         (1000)     4127 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_objects.json
--rw-rw-r--   0 b         (1000) b         (1000)     6612 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_poisons.json
--rw-rw-r--   0 b         (1000) b         (1000)     1676 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_proficiency-bonus.json
--rw-rw-r--   0 b         (1000) b         (1000)     2112 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_resting.json
--rw-rw-r--   0 b         (1000) b         (1000)     1451 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_saving-throws.json
--rw-rw-r--   0 b         (1000) b         (1000)     7309 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_sentient-magic-items.json
--rw-rw-r--   0 b         (1000) b         (1000)      575 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_standard-exchange-rates.json
--rw-rw-r--   0 b         (1000) b         (1000)     6567 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_the-environment.json
--rw-rw-r--   0 b         (1000) b         (1000)     6297 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_the-order-of-combat.json
--rw-rw-r--   0 b         (1000) b         (1000)     9702 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_the-planes-of-existence.json
--rw-rw-r--   0 b         (1000) b         (1000)     1118 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_time.json
--rw-rw-r--   0 b         (1000) b         (1000)    17744 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_traps.json
--rw-rw-r--   0 b         (1000) b         (1000)      989 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_underwater-combat.json
--rw-rw-r--   0 b         (1000) b         (1000)    16317 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_using-each-ability.json
--rw-rw-r--   0 b         (1000) b         (1000)     2000 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_wearing-and-wielding-items.json
--rw-rw-r--   0 b         (1000) b         (1000)     5515 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_what-is-a-spell.json
--rw-rw-r--   0 b         (1000) b         (1000)      517 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_rules.json
--rw-rw-r--   0 b         (1000) b         (1000)      796 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_rules_adventuring.json
--rw-rw-r--   0 b         (1000) b         (1000)      379 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_rules_appendix.json
--rw-rw-r--   0 b         (1000) b         (1000)      941 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_rules_combat.json
--rw-rw-r--   0 b         (1000) b         (1000)     2455 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_rules_equipment.json
--rw-rw-r--   0 b         (1000) b         (1000)      659 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_rules_spellcasting.json
--rw-rw-r--   0 b         (1000) b         (1000)     2551 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_rules_using-ability-scores.json
--rw-rw-r--   0 b         (1000) b         (1000)    27593 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells.json
--rw-rw-r--   0 b         (1000) b         (1000)     1431 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_acid-arrow.json
--rw-rw-r--   0 b         (1000) b         (1000)     1216 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_acid-splash.json
--rw-rw-r--   0 b         (1000) b         (1000)     1073 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_aid.json
--rw-rw-r--   0 b         (1000) b         (1000)     1299 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_alarm.json
--rw-rw-r--   0 b         (1000) b         (1000)     2084 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_alter-self.json
--rw-rw-r--   0 b         (1000) b         (1000)     1197 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_animal-friendship.json
--rw-rw-r--   0 b         (1000) b         (1000)     1818 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_animal-messenger.json
--rw-rw-r--   0 b         (1000) b         (1000)     1746 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_animal-shapes.json
--rw-rw-r--   0 b         (1000) b         (1000)     2287 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_animate-dead.json
--rw-rw-r--   0 b         (1000) b         (1000)     3180 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_animate-objects.json
--rw-rw-r--   0 b         (1000) b         (1000)     1003 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_antilife-shell.json
--rw-rw-r--   0 b         (1000) b         (1000)     3331 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_antimagic-field.json
--rw-rw-r--   0 b         (1000) b         (1000)     3063 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_antipathy-sympathy.json
--rw-rw-r--   0 b         (1000) b         (1000)     1152 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_arcane-eye.json
--rw-rw-r--   0 b         (1000) b         (1000)     2968 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_arcane-hand.json
--rw-rw-r--   0 b         (1000) b         (1000)     1216 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_arcane-lock.json
--rw-rw-r--   0 b         (1000) b         (1000)     1244 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_arcane-sword.json
--rw-rw-r--   0 b         (1000) b         (1000)     1853 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_arcanists-magic-aura.json
--rw-rw-r--   0 b         (1000) b         (1000)     2992 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_astral-projection.json
--rw-rw-r--   0 b         (1000) b         (1000)     1474 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_augury.json
--rw-rw-r--   0 b         (1000) b         (1000)     1461 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_awaken.json
--rw-rw-r--   0 b         (1000) b         (1000)     1165 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_bane.json
--rw-rw-r--   0 b         (1000) b         (1000)     1887 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_banishment.json
--rw-rw-r--   0 b         (1000) b         (1000)      898 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_barkskin.json
--rw-rw-r--   0 b         (1000) b         (1000)      932 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_beacon-of-hope.json
--rw-rw-r--   0 b         (1000) b         (1000)     2173 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_bestow-curse.json
--rw-rw-r--   0 b         (1000) b         (1000)     1754 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_black-tentacles.json
--rw-rw-r--   0 b         (1000) b         (1000)     1440 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_blade-barrier.json
--rw-rw-r--   0 b         (1000) b         (1000)     1069 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_bless.json
--rw-rw-r--   0 b         (1000) b         (1000)     1785 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_blight.json
--rw-rw-r--   0 b         (1000) b         (1000)     1381 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_blindness-deafness.json
--rw-rw-r--   0 b         (1000) b         (1000)     1612 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_blink.json
--rw-rw-r--   0 b         (1000) b         (1000)      922 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_blur.json
--rw-rw-r--   0 b         (1000) b         (1000)     1166 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_branding-smite.json
--rw-rw-r--   0 b         (1000) b         (1000)     1577 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_burning-hands.json
--rw-rw-r--   0 b         (1000) b         (1000)     2005 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_call-lightning.json
--rw-rw-r--   0 b         (1000) b         (1000)     1591 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_calm-emotions.json
--rw-rw-r--   0 b         (1000) b         (1000)     1545 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_chain-lightning.json
--rw-rw-r--   0 b         (1000) b         (1000)     1545 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_charm-person.json
--rw-rw-r--   0 b         (1000) b         (1000)     1440 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_chill-touch.json
--rw-rw-r--   0 b         (1000) b         (1000)     1433 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_circle-of-death.json
--rw-rw-r--   0 b         (1000) b         (1000)     1550 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_clairvoyance.json
--rw-rw-r--   0 b         (1000) b         (1000)     1615 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_clone.json
--rw-rw-r--   0 b         (1000) b         (1000)     1975 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_cloudkill.json
--rw-rw-r--   0 b         (1000) b         (1000)     1533 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_color-spray.json
--rw-rw-r--   0 b         (1000) b         (1000)     2077 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_command.json
--rw-rw-r--   0 b         (1000) b         (1000)     1486 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_commune-with-nature.json
--rw-rw-r--   0 b         (1000) b         (1000)     1327 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_commune.json
--rw-rw-r--   0 b         (1000) b         (1000)     1199 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_comprehend-languages.json
--rw-rw-r--   0 b         (1000) b         (1000)     1338 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_compulsion.json
--rw-rw-r--   0 b         (1000) b         (1000)     1490 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_cone-of-cold.json
--rw-rw-r--   0 b         (1000) b         (1000)     2119 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_confusion.json
--rw-rw-r--   0 b         (1000) b         (1000)     1689 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_conjure-animals.json
--rw-rw-r--   0 b         (1000) b         (1000)     1222 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_conjure-celestial.json
--rw-rw-r--   0 b         (1000) b         (1000)     2026 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_conjure-elemental.json
--rw-rw-r--   0 b         (1000) b         (1000)     1683 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_conjure-fey.json
--rw-rw-r--   0 b         (1000) b         (1000)     1642 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_conjure-minor-elementals.json
--rw-rw-r--   0 b         (1000) b         (1000)     1698 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_conjure-woodland-beings.json
--rw-rw-r--   0 b         (1000) b         (1000)     1680 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_contact-other-plane.json
--rw-rw-r--   0 b         (1000) b         (1000)     2588 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_contagion.json
--rw-rw-r--   0 b         (1000) b         (1000)     1596 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_contingency.json
--rw-rw-r--   0 b         (1000) b         (1000)      929 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_continual-flame.json
--rw-rw-r--   0 b         (1000) b         (1000)     3934 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_control-water.json
--rw-rw-r--   0 b         (1000) b         (1000)     2060 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_control-weather.json
--rw-rw-r--   0 b         (1000) b         (1000)     1161 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_counterspell.json
--rw-rw-r--   0 b         (1000) b         (1000)     1048 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_create-food-and-water.json
--rw-rw-r--   0 b         (1000) b         (1000)     1354 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_create-or-destroy-water.json
--rw-rw-r--   0 b         (1000) b         (1000)     2380 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_create-undead.json
--rw-rw-r--   0 b         (1000) b         (1000)     1609 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_creation.json
--rw-rw-r--   0 b         (1000) b         (1000)     1330 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_cure-wounds.json
--rw-rw-r--   0 b         (1000) b         (1000)     1290 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_dancing-lights.json
--rw-rw-r--   0 b         (1000) b         (1000)     1521 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_darkness.json
--rw-rw-r--   0 b         (1000) b         (1000)      950 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_darkvision.json
--rw-rw-r--   0 b         (1000) b         (1000)     1477 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_daylight.json
--rw-rw-r--   0 b         (1000) b         (1000)     1016 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_death-ward.json
--rw-rw-r--   0 b         (1000) b         (1000)     2241 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_delayed-blast-fireball.json
--rw-rw-r--   0 b         (1000) b         (1000)     1323 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_demiplane.json
--rw-rw-r--   0 b         (1000) b         (1000)     1118 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_detect-evil-and-good.json
--rw-rw-r--   0 b         (1000) b         (1000)     1409 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_detect-magic.json
--rw-rw-r--   0 b         (1000) b         (1000)     1223 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_detect-poison-and-disease.json
--rw-rw-r--   0 b         (1000) b         (1000)     2653 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_detect-thoughts.json
--rw-rw-r--   0 b         (1000) b         (1000)     1613 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_dimension-door.json
--rw-rw-r--   0 b         (1000) b         (1000)     1665 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_disguise-self.json
--rw-rw-r--   0 b         (1000) b         (1000)     1941 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_disintegrate.json
--rw-rw-r--   0 b         (1000) b         (1000)     1874 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_dispel-evil-and-good.json
--rw-rw-r--   0 b         (1000) b         (1000)     1540 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_dispel-magic.json
--rw-rw-r--   0 b         (1000) b         (1000)     1326 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_divination.json
--rw-rw-r--   0 b         (1000) b         (1000)      811 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_divine-favor.json
--rw-rw-r--   0 b         (1000) b         (1000)     1455 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_divine-word.json
--rw-rw-r--   0 b         (1000) b         (1000)     2032 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_dominate-beast.json
--rw-rw-r--   0 b         (1000) b         (1000)     2249 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_dominate-monster.json
--rw-rw-r--   0 b         (1000) b         (1000)     2430 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_dominate-person.json
--rw-rw-r--   0 b         (1000) b         (1000)     2862 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_dream.json
--rw-rw-r--   0 b         (1000) b         (1000)     1192 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_druidcraft.json
--rw-rw-r--   0 b         (1000) b         (1000)     2830 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_earthquake.json
--rw-rw-r--   0 b         (1000) b         (1000)     1166 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_eldritch-blast.json
--rw-rw-r--   0 b         (1000) b         (1000)     1721 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_enhance-ability.json
--rw-rw-r--   0 b         (1000) b         (1000)     2272 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_enlarge-reduce.json
--rw-rw-r--   0 b         (1000) b         (1000)     1213 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_entangle.json
--rw-rw-r--   0 b         (1000) b         (1000)     1266 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_enthrall.json
--rw-rw-r--   0 b         (1000) b         (1000)     2356 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_etherealness.json
--rw-rw-r--   0 b         (1000) b         (1000)      896 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_expeditious-retreat.json
--rw-rw-r--   0 b         (1000) b         (1000)     2680 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_eyebite.json
--rw-rw-r--   0 b         (1000) b         (1000)     1442 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_fabricate.json
--rw-rw-r--   0 b         (1000) b         (1000)     1147 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_faerie-fire.json
--rw-rw-r--   0 b         (1000) b         (1000)     1522 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_faithful-hound.json
--rw-rw-r--   0 b         (1000) b         (1000)     1093 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_false-life.json
--rw-rw-r--   0 b         (1000) b         (1000)     1595 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_fear.json
--rw-rw-r--   0 b         (1000) b         (1000)     1001 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_feather-fall.json
--rw-rw-r--   0 b         (1000) b         (1000)     1809 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_feeblemind.json
--rw-rw-r--   0 b         (1000) b         (1000)     2542 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_find-familiar.json
--rw-rw-r--   0 b         (1000) b         (1000)     1962 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_find-steed.json
--rw-rw-r--   0 b         (1000) b         (1000)     1440 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_find-the-path.json
--rw-rw-r--   0 b         (1000) b         (1000)     1325 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_find-traps.json
--rw-rw-r--   0 b         (1000) b         (1000)     1320 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_finger-of-death.json
--rw-rw-r--   0 b         (1000) b         (1000)     1089 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_fire-bolt.json
--rw-rw-r--   0 b         (1000) b         (1000)     1351 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_fire-shield.json
--rw-rw-r--   0 b         (1000) b         (1000)     1476 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_fire-storm.json
--rw-rw-r--   0 b         (1000) b         (1000)     1669 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_fireball.json
--rw-rw-r--   0 b         (1000) b         (1000)     1315 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_flame-blade.json
--rw-rw-r--   0 b         (1000) b         (1000)     1521 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_flame-strike.json
--rw-rw-r--   0 b         (1000) b         (1000)     1841 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_flaming-sphere.json
--rw-rw-r--   0 b         (1000) b         (1000)     1789 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_flesh-to-stone.json
--rw-rw-r--   0 b         (1000) b         (1000)     1494 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_floating-disk.json
--rw-rw-r--   0 b         (1000) b         (1000)     1032 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_fly.json
--rw-rw-r--   0 b         (1000) b         (1000)     1189 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_fog-cloud.json
--rw-rw-r--   0 b         (1000) b         (1000)     1844 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_forbiddance.json
--rw-rw-r--   0 b         (1000) b         (1000)     1933 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_forcecage.json
--rw-rw-r--   0 b         (1000) b         (1000)     1086 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_foresight.json
--rw-rw-r--   0 b         (1000) b         (1000)     1374 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_freedom-of-movement.json
--rw-rw-r--   0 b         (1000) b         (1000)     2193 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_freezing-sphere.json
--rw-rw-r--   0 b         (1000) b         (1000)     1772 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_gaseous-form.json
--rw-rw-r--   0 b         (1000) b         (1000)     1830 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_gate.json
--rw-rw-r--   0 b         (1000) b         (1000)     1845 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_geas.json
--rw-rw-r--   0 b         (1000) b         (1000)     1054 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_gentle-repose.json
--rw-rw-r--   0 b         (1000) b         (1000)     1258 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_giant-insect.json
--rw-rw-r--   0 b         (1000) b         (1000)      752 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_glibness.json
--rw-rw-r--   0 b         (1000) b         (1000)     1340 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_globe-of-invulnerability.json
--rw-rw-r--   0 b         (1000) b         (1000)     3823 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_glyph-of-warding.json
--rw-rw-r--   0 b         (1000) b         (1000)      930 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_goodberry.json
--rw-rw-r--   0 b         (1000) b         (1000)     1093 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_grease.json
--rw-rw-r--   0 b         (1000) b         (1000)      853 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_greater-invisibility.json
--rw-rw-r--   0 b         (1000) b         (1000)     1125 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_greater-restoration.json
--rw-rw-r--   0 b         (1000) b         (1000)     1429 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_guardian-of-faith.json
--rw-rw-r--   0 b         (1000) b         (1000)     3195 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_guards-and-wards.json
--rw-rw-r--   0 b         (1000) b         (1000)      816 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_guidance.json
--rw-rw-r--   0 b         (1000) b         (1000)     1254 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_guiding-bolt.json
--rw-rw-r--   0 b         (1000) b         (1000)     1615 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_gust-of-wind.json
--rw-rw-r--   0 b         (1000) b         (1000)     3273 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_hallow.json
--rw-rw-r--   0 b         (1000) b         (1000)     1757 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_hallucinatory-terrain.json
--rw-rw-r--   0 b         (1000) b         (1000)     1227 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_harm.json
--rw-rw-r--   0 b         (1000) b         (1000)     1198 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_haste.json
--rw-rw-r--   0 b         (1000) b         (1000)      988 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_heal.json
--rw-rw-r--   0 b         (1000) b         (1000)     1152 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_healing-word.json
--rw-rw-r--   0 b         (1000) b         (1000)     1809 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_heat-metal.json
--rw-rw-r--   0 b         (1000) b         (1000)      959 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_hellish-rebuke.json
--rw-rw-r--   0 b         (1000) b         (1000)     1233 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_heroes-feast.json
--rw-rw-r--   0 b         (1000) b         (1000)      904 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_heroism.json
--rw-rw-r--   0 b         (1000) b         (1000)     1362 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_hideous-laughter.json
--rw-rw-r--   0 b         (1000) b         (1000)     1356 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_hold-monster.json
--rw-rw-r--   0 b         (1000) b         (1000)     1576 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_hold-person.json
--rw-rw-r--   0 b         (1000) b         (1000)     1232 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_holy-aura.json
--rw-rw-r--   0 b         (1000) b         (1000)     1227 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_hunters-mark.json
--rw-rw-r--   0 b         (1000) b         (1000)     1550 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_hypnotic-pattern.json
--rw-rw-r--   0 b         (1000) b         (1000)     1688 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_ice-storm.json
--rw-rw-r--   0 b         (1000) b         (1000)     1168 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_identify.json
--rw-rw-r--   0 b         (1000) b         (1000)     1493 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_illusory-script.json
--rw-rw-r--   0 b         (1000) b         (1000)     3954 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_imprisonment.json
--rw-rw-r--   0 b         (1000) b         (1000)     1580 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_incendiary-cloud.json
--rw-rw-r--   0 b         (1000) b         (1000)     1052 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_inflict-wounds.json
--rw-rw-r--   0 b         (1000) b         (1000)     1814 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_insect-plague.json
--rw-rw-r--   0 b         (1000) b         (1000)     1369 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_instant-summons.json
--rw-rw-r--   0 b         (1000) b         (1000)     1210 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_invisibility.json
--rw-rw-r--   0 b         (1000) b         (1000)     1140 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_irresistible-dance.json
--rw-rw-r--   0 b         (1000) b         (1000)      852 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_jump.json
--rw-rw-r--   0 b         (1000) b         (1000)     1313 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_knock.json
--rw-rw-r--   0 b         (1000) b         (1000)     1612 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_legend-lore.json
--rw-rw-r--   0 b         (1000) b         (1000)     1112 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_lesser-restoration.json
--rw-rw-r--   0 b         (1000) b         (1000)     1542 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_levitate.json
--rw-rw-r--   0 b         (1000) b         (1000)     1359 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_light.json
--rw-rw-r--   0 b         (1000) b         (1000)     1623 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_lightning-bolt.json
--rw-rw-r--   0 b         (1000) b         (1000)      977 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_locate-animals-or-plants.json
--rw-rw-r--   0 b         (1000) b         (1000)     1655 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_locate-creature.json
--rw-rw-r--   0 b         (1000) b         (1000)     1537 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_locate-object.json
--rw-rw-r--   0 b         (1000) b         (1000)      989 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_longstrider.json
--rw-rw-r--   0 b         (1000) b         (1000)      901 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_mage-armor.json
--rw-rw-r--   0 b         (1000) b         (1000)     1321 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_mage-hand.json
--rw-rw-r--   0 b         (1000) b         (1000)     2262 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_magic-circle.json
--rw-rw-r--   0 b         (1000) b         (1000)     3172 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_magic-jar.json
--rw-rw-r--   0 b         (1000) b         (1000)     1273 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_magic-missile.json
--rw-rw-r--   0 b         (1000) b         (1000)     1952 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_magic-mouth.json
--rw-rw-r--   0 b         (1000) b         (1000)      928 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_magic-weapon.json
--rw-rw-r--   0 b         (1000) b         (1000)     2286 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_magnificent-mansion.json
--rw-rw-r--   0 b         (1000) b         (1000)     2350 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_major-image.json
--rw-rw-r--   0 b         (1000) b         (1000)     1259 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_mass-cure-wounds.json
--rw-rw-r--   0 b         (1000) b         (1000)      853 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_mass-heal.json
--rw-rw-r--   0 b         (1000) b         (1000)     1048 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_mass-healing-word.json
--rw-rw-r--   0 b         (1000) b         (1000)     2342 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_mass-suggestion.json
--rw-rw-r--   0 b         (1000) b         (1000)      947 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_maze.json
--rw-rw-r--   0 b         (1000) b         (1000)     1739 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_meld-into-stone.json
--rw-rw-r--   0 b         (1000) b         (1000)     1200 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_mending.json
--rw-rw-r--   0 b         (1000) b         (1000)     1232 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_message.json
--rw-rw-r--   0 b         (1000) b         (1000)     1385 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_meteor-swarm.json
--rw-rw-r--   0 b         (1000) b         (1000)      857 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_mind-blank.json
--rw-rw-r--   0 b         (1000) b         (1000)     1850 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_minor-illusion.json
--rw-rw-r--   0 b         (1000) b         (1000)     1782 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_mirage-arcane.json
--rw-rw-r--   0 b         (1000) b         (1000)     1822 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_mirror-image.json
--rw-rw-r--   0 b         (1000) b         (1000)     1144 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_mislead.json
--rw-rw-r--   0 b         (1000) b         (1000)      846 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_misty-step.json
--rw-rw-r--   0 b         (1000) b         (1000)     2692 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_modify-memory.json
--rw-rw-r--   0 b         (1000) b         (1000)     1899 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_moonbeam.json
--rw-rw-r--   0 b         (1000) b         (1000)     1939 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_move-earth.json
--rw-rw-r--   0 b         (1000) b         (1000)     1042 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_nondetection.json
--rw-rw-r--   0 b         (1000) b         (1000)     1122 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_pass-without-trace.json
--rw-rw-r--   0 b         (1000) b         (1000)     1097 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_passwall.json
--rw-rw-r--   0 b         (1000) b         (1000)     1309 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_phantasmal-killer.json
--rw-rw-r--   0 b         (1000) b         (1000)     1243 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_phantom-steed.json
--rw-rw-r--   0 b         (1000) b         (1000)     2712 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_planar-ally.json
--rw-rw-r--   0 b         (1000) b         (1000)     2312 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_planar-binding.json
--rw-rw-r--   0 b         (1000) b         (1000)     2446 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_plane-shift.json
--rw-rw-r--   0 b         (1000) b         (1000)     1463 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_plant-growth.json
--rw-rw-r--   0 b         (1000) b         (1000)     1229 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_poison-spray.json
--rw-rw-r--   0 b         (1000) b         (1000)     2151 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_polymorph.json
--rw-rw-r--   0 b         (1000) b         (1000)      886 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_power-word-kill.json
--rw-rw-r--   0 b         (1000) b         (1000)     1043 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_power-word-stun.json
--rw-rw-r--   0 b         (1000) b         (1000)     1029 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_prayer-of-healing.json
--rw-rw-r--   0 b         (1000) b         (1000)     1669 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_prestidigitation.json
--rw-rw-r--   0 b         (1000) b         (1000)     2651 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_prismatic-spray.json
--rw-rw-r--   0 b         (1000) b         (1000)     4369 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_prismatic-wall.json
--rw-rw-r--   0 b         (1000) b         (1000)     1823 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_private-sanctum.json
--rw-rw-r--   0 b         (1000) b         (1000)     1393 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_produce-flame.json
--rw-rw-r--   0 b         (1000) b         (1000)     2110 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_programmed-illusion.json
--rw-rw-r--   0 b         (1000) b         (1000)     1811 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_project-image.json
--rw-rw-r--   0 b         (1000) b         (1000)     1045 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_protection-from-energy.json
--rw-rw-r--   0 b         (1000) b         (1000)     1473 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_protection-from-evil-and-good.json
--rw-rw-r--   0 b         (1000) b         (1000)     1087 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_protection-from-poison.json
--rw-rw-r--   0 b         (1000) b         (1000)      868 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_purify-food-and-drink.json
--rw-rw-r--   0 b         (1000) b         (1000)     1758 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_raise-dead.json
--rw-rw-r--   0 b         (1000) b         (1000)     1136 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_ray-of-enfeeblement.json
--rw-rw-r--   0 b         (1000) b         (1000)     1146 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_ray-of-frost.json
--rw-rw-r--   0 b         (1000) b         (1000)     1143 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_regenerate.json
--rw-rw-r--   0 b         (1000) b         (1000)     1727 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_reincarnate.json
--rw-rw-r--   0 b         (1000) b         (1000)      959 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_remove-curse.json
--rw-rw-r--   0 b         (1000) b         (1000)     1657 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_resilient-sphere.json
--rw-rw-r--   0 b         (1000) b         (1000)      859 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_resistance.json
--rw-rw-r--   0 b         (1000) b         (1000)     1646 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_resurrection.json
--rw-rw-r--   0 b         (1000) b         (1000)     1708 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_reverse-gravity.json
--rw-rw-r--   0 b         (1000) b         (1000)      948 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_revivify.json
--rw-rw-r--   0 b         (1000) b         (1000)     1390 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_rope-trick.json
--rw-rw-r--   0 b         (1000) b         (1000)     1151 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_sacred-flame.json
--rw-rw-r--   0 b         (1000) b         (1000)     1132 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_sanctuary.json
--rw-rw-r--   0 b         (1000) b         (1000)     1143 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_scorching-ray.json
--rw-rw-r--   0 b         (1000) b         (1000)     2393 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_scrying.json
--rw-rw-r--   0 b         (1000) b         (1000)     1548 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_secret-chest.json
--rw-rw-r--   0 b         (1000) b         (1000)      939 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_see-invisibility.json
--rw-rw-r--   0 b         (1000) b         (1000)     1909 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_seeming.json
--rw-rw-r--   0 b         (1000) b         (1000)     1241 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_sending.json
--rw-rw-r--   0 b         (1000) b         (1000)     1313 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_sequester.json
--rw-rw-r--   0 b         (1000) b         (1000)     3021 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_shapechange.json
--rw-rw-r--   0 b         (1000) b         (1000)     1805 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_shatter.json
--rw-rw-r--   0 b         (1000) b         (1000)      828 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_shield-of-faith.json
--rw-rw-r--   0 b         (1000) b         (1000)      794 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_shield.json
--rw-rw-r--   0 b         (1000) b         (1000)     1001 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_shillelagh.json
--rw-rw-r--   0 b         (1000) b         (1000)     1261 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_shocking-grasp.json
--rw-rw-r--   0 b         (1000) b         (1000)     1102 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_silence.json
--rw-rw-r--   0 b         (1000) b         (1000)     1714 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_silent-image.json
--rw-rw-r--   0 b         (1000) b         (1000)     1949 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_simulacrum.json
--rw-rw-r--   0 b         (1000) b         (1000)     1764 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_sleep.json
--rw-rw-r--   0 b         (1000) b         (1000)     1491 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_sleet-storm.json
--rw-rw-r--   0 b         (1000) b         (1000)     1832 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_slow.json
--rw-rw-r--   0 b         (1000) b         (1000)      607 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_spare-the-dying.json
--rw-rw-r--   0 b         (1000) b         (1000)     1100 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_speak-with-animals.json
--rw-rw-r--   0 b         (1000) b         (1000)     1472 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_speak-with-dead.json
--rw-rw-r--   0 b         (1000) b         (1000)     1837 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_speak-with-plants.json
--rw-rw-r--   0 b         (1000) b         (1000)     1051 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_spider-climb.json
--rw-rw-r--   0 b         (1000) b         (1000)     1340 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_spike-growth.json
--rw-rw-r--   0 b         (1000) b         (1000)     1416 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_spirit-guardians.json
--rw-rw-r--   0 b         (1000) b         (1000)     1712 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_spiritual-weapon.json
--rw-rw-r--   0 b         (1000) b         (1000)     1815 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_stinking-cloud.json
--rw-rw-r--   0 b         (1000) b         (1000)     1272 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_stone-shape.json
--rw-rw-r--   0 b         (1000) b         (1000)      987 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_stoneskin.json
--rw-rw-r--   0 b         (1000) b         (1000)     2476 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_storm-of-vengeance.json
--rw-rw-r--   0 b         (1000) b         (1000)     2060 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_suggestion.json
--rw-rw-r--   0 b         (1000) b         (1000)     1712 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_sunbeam.json
--rw-rw-r--   0 b         (1000) b         (1000)     1632 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_sunburst.json
--rw-rw-r--   0 b         (1000) b         (1000)     4345 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_symbol.json
--rw-rw-r--   0 b         (1000) b         (1000)     2353 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_telekinesis.json
--rw-rw-r--   0 b         (1000) b         (1000)     1021 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_telepathic-bond.json
--rw-rw-r--   0 b         (1000) b         (1000)     4184 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_teleport.json
--rw-rw-r--   0 b         (1000) b         (1000)     2024 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_teleportation-circle.json
--rw-rw-r--   0 b         (1000) b         (1000)     1342 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_thaumaturgy.json
--rw-rw-r--   0 b         (1000) b         (1000)     1775 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_thunderwave.json
--rw-rw-r--   0 b         (1000) b         (1000)     1051 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_time-stop.json
--rw-rw-r--   0 b         (1000) b         (1000)     1509 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_tiny-hut.json
--rw-rw-r--   0 b         (1000) b         (1000)     1065 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_tongues.json
--rw-rw-r--   0 b         (1000) b         (1000)      846 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_transport-via-plants.json
--rw-rw-r--   0 b         (1000) b         (1000)     1337 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_tree-stride.json
--rw-rw-r--   0 b         (1000) b         (1000)     3331 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_true-polymorph.json
--rw-rw-r--   0 b         (1000) b         (1000)     1271 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_true-resurrection.json
--rw-rw-r--   0 b         (1000) b         (1000)     1126 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_true-seeing.json
--rw-rw-r--   0 b         (1000) b         (1000)      986 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_true-strike.json
--rw-rw-r--   0 b         (1000) b         (1000)     1628 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_unseen-servant.json
--rw-rw-r--   0 b         (1000) b         (1000)     1349 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_vampiric-touch.json
--rw-rw-r--   0 b         (1000) b         (1000)     1199 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_vicious-mockery.json
--rw-rw-r--   0 b         (1000) b         (1000)     1962 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_wall-of-fire.json
--rw-rw-r--   0 b         (1000) b         (1000)     1464 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_wall-of-force.json
--rw-rw-r--   0 b         (1000) b         (1000)     2182 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_wall-of-ice.json
--rw-rw-r--   0 b         (1000) b         (1000)     2363 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_wall-of-stone.json
--rw-rw-r--   0 b         (1000) b         (1000)     1931 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_wall-of-thorns.json
--rw-rw-r--   0 b         (1000) b         (1000)     1206 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_warding-bond.json
--rw-rw-r--   0 b         (1000) b         (1000)     1080 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_water-breathing.json
--rw-rw-r--   0 b         (1000) b         (1000)     1295 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_water-walk.json
--rw-rw-r--   0 b         (1000) b         (1000)     1762 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_web.json
--rw-rw-r--   0 b         (1000) b         (1000)     1205 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_weird.json
--rw-rw-r--   0 b         (1000) b         (1000)     1287 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_wind-walk.json
--rw-rw-r--   0 b         (1000) b         (1000)     1906 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_wind-wall.json
--rw-rw-r--   0 b         (1000) b         (1000)     3433 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_wish.json
--rw-rw-r--   0 b         (1000) b         (1000)     1139 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_word-of-recall.json
--rw-rw-r--   0 b         (1000) b         (1000)     1472 2023-06-29 01:34:15.000000 dnd_character-23.7.22/dnd_character/json_cache/api_spells_zone-of-truth.json
--rw-rw-r--   0 b         (1000) b         (1000)      156 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/monsters.py
--rw-rw-r--   0 b         (1000) b         (1000)      721 2022-09-20 01:54:47.000000 dnd_character-23.7.22/dnd_character/spellcasting.py
-drwxrwxr-x   0 b         (1000) b         (1000)        0 2023-07-22 21:49:02.311644 dnd_character-23.7.22/dnd_character.egg-info/
--rw-rw-r--   0 b         (1000) b         (1000)     5480 2023-07-22 21:49:02.000000 dnd_character-23.7.22/dnd_character.egg-info/PKG-INFO
--rw-rw-r--   0 b         (1000) b         (1000)    70285 2023-07-22 21:49:02.000000 dnd_character-23.7.22/dnd_character.egg-info/SOURCES.txt
--rw-rw-r--   0 b         (1000) b         (1000)        1 2023-07-22 21:49:02.000000 dnd_character-23.7.22/dnd_character.egg-info/dependency_links.txt
--rw-rw-r--   0 b         (1000) b         (1000)       14 2023-07-22 21:49:02.000000 dnd_character-23.7.22/dnd_character.egg-info/top_level.txt
--rw-rw-r--   0 b         (1000) b         (1000)       38 2023-07-22 21:49:02.483644 dnd_character-23.7.22/setup.cfg
--rw-rw-r--   0 b         (1000) b         (1000)     1238 2022-09-20 01:54:47.000000 dnd_character-23.7.22/setup.py
+drwxrwxr-x   0 b         (1000) b         (1000)        0 2023-07-30 01:48:19.832039 dnd_character-23.7.29/
+-rw-rw-r--   0 b         (1000) b         (1000)    14199 2022-09-20 01:54:47.000000 dnd_character-23.7.29/LICENSE
+-rw-rw-r--   0 b         (1000) b         (1000)       52 2022-09-20 01:54:47.000000 dnd_character-23.7.29/MANIFEST.in
+-rw-rw-r--   0 b         (1000) b         (1000)     7121 2023-07-30 01:48:19.832039 dnd_character-23.7.29/PKG-INFO
+-rw-rw-r--   0 b         (1000) b         (1000)     6473 2023-07-30 01:23:48.000000 dnd_character-23.7.29/README.md
+drwxrwxr-x   0 b         (1000) b         (1000)        0 2023-07-30 01:48:19.704028 dnd_character-23.7.29/dnd_character/
+-rw-rw-r--   0 b         (1000) b         (1000)     3312 2023-07-29 01:51:03.000000 dnd_character-23.7.29/dnd_character/SRD.py
+-rw-rw-r--   0 b         (1000) b         (1000)      564 2023-07-30 00:46:51.000000 dnd_character-23.7.29/dnd_character/__init__.py
+-rw-rw-r--   0 b         (1000) b         (1000)     1743 2023-07-23 14:32:03.000000 dnd_character-23.7.29/dnd_character/__main__.py
+-rw-rw-r--   0 b         (1000) b         (1000)    31956 2023-07-30 01:08:35.000000 dnd_character-23.7.29/dnd_character/character.py
+-rw-rw-r--   0 b         (1000) b         (1000)     1828 2023-07-29 02:30:02.000000 dnd_character-23.7.29/dnd_character/classes.py
+-rw-rw-r--   0 b         (1000) b         (1000)     1204 2023-07-23 13:35:40.000000 dnd_character-23.7.29/dnd_character/dice.py
+-rw-rw-r--   0 b         (1000) b         (1000)     1768 2023-07-29 21:20:41.000000 dnd_character-23.7.29/dnd_character/equipment.py
+-rw-rw-r--   0 b         (1000) b         (1000)     3300 2023-07-30 00:54:27.000000 dnd_character-23.7.29/dnd_character/experience.py
+drwxrwxr-x   0 b         (1000) b         (1000)        0 2023-07-30 01:48:19.832039 dnd_character-23.7.29/dnd_character/json_cache/
+-rw-rw-r--   0 b         (1000) b         (1000)     6468 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/OGLv1.0a.txt
+-rw-rw-r--   0 b         (1000) b         (1000)       95 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/README.md
+-rw-rw-r--   0 b         (1000) b         (1000)      784 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_.json
+-rw-rw-r--   0 b         (1000) b         (1000)      860 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_classes.json
+-rw-rw-r--   0 b         (1000) b         (1000)     4057 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_classes_barbarian.json
+-rw-rw-r--   0 b         (1000) b         (1000)     8578 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_classes_barbarian_levels.json
+-rw-rw-r--   0 b         (1000) b         (1000)    13694 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_classes_bard.json
+-rw-rw-r--   0 b         (1000) b         (1000)    15727 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_classes_bard_levels.json
+-rw-rw-r--   0 b         (1000) b         (1000)     7660 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_classes_cleric.json
+-rw-rw-r--   0 b         (1000) b         (1000)    14080 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_classes_cleric_levels.json
+-rw-rw-r--   0 b         (1000) b         (1000)     7654 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_classes_druid.json
+-rw-rw-r--   0 b         (1000) b         (1000)    13282 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_classes_druid_levels.json
+-rw-rw-r--   0 b         (1000) b         (1000)     6103 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_classes_fighter.json
+-rw-rw-r--   0 b         (1000) b         (1000)     8172 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_classes_fighter_levels.json
+-rw-rw-r--   0 b         (1000) b         (1000)     7806 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_classes_monk.json
+-rw-rw-r--   0 b         (1000) b         (1000)     9190 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_classes_monk_levels.json
+-rw-rw-r--   0 b         (1000) b         (1000)     7193 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_classes_paladin.json
+-rw-rw-r--   0 b         (1000) b         (1000)    10285 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_classes_paladin_levels.json
+-rw-rw-r--   0 b         (1000) b         (1000)     8002 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_classes_ranger.json
+-rw-rw-r--   0 b         (1000) b         (1000)    11393 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_classes_ranger_levels.json
+-rw-rw-r--   0 b         (1000) b         (1000)     7246 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_classes_rogue.json
+-rw-rw-r--   0 b         (1000) b         (1000)     7636 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_classes_rogue_levels.json
+-rw-rw-r--   0 b         (1000) b         (1000)     6488 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_classes_sorcerer.json
+-rw-rw-r--   0 b         (1000) b         (1000)    18613 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_classes_sorcerer_levels.json
+-rw-rw-r--   0 b         (1000) b         (1000)     7003 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_classes_warlock.json
+-rw-rw-r--   0 b         (1000) b         (1000)    15137 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_classes_warlock_levels.json
+-rw-rw-r--   0 b         (1000) b         (1000)     6717 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_classes_wizard.json
+-rw-rw-r--   0 b         (1000) b         (1000)    11937 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_classes_wizard_levels.json
+-rw-rw-r--   0 b         (1000) b         (1000)      441 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment-categories_arcane-foci.json
+-rw-rw-r--   0 b         (1000) b         (1000)      454 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment-categories_druidic-foci.json
+-rw-rw-r--   0 b         (1000) b         (1000)      335 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment-categories_holy-symbols.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1484 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment-categories_martial-melee-weapons.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1865 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment-categories_martial-weapons.json
+-rw-rw-r--   0 b         (1000) b         (1000)      829 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment-categories_musical-instruments.json
+-rw-rw-r--   0 b         (1000) b         (1000)      883 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment-categories_simple-melee-weapons.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1171 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment-categories_simple-weapons.json
+-rw-rw-r--   0 b         (1000) b         (1000)    20241 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment.json
+-rw-rw-r--   0 b         (1000) b         (1000)      436 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_abacus.json
+-rw-rw-r--   0 b         (1000) b         (1000)      756 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_acid-vial.json
+-rw-rw-r--   0 b         (1000) b         (1000)      921 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_alchemists-fire-flask.json
+-rw-rw-r--   0 b         (1000) b         (1000)      744 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_alchemists-supplies.json
+-rw-rw-r--   0 b         (1000) b         (1000)      501 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_alms-box.json
+-rw-rw-r--   0 b         (1000) b         (1000)      934 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_amulet.json
+-rw-rw-r--   0 b         (1000) b         (1000)      418 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_animal-feed-1-day.json
+-rw-rw-r--   0 b         (1000) b         (1000)      614 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_antitoxin-vial.json
+-rw-rw-r--   0 b         (1000) b         (1000)      440 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_arrow.json
+-rw-rw-r--   0 b         (1000) b         (1000)      442 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_backpack.json
+-rw-rw-r--   0 b         (1000) b         (1000)      706 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_bagpipes.json
+-rw-rw-r--   0 b         (1000) b         (1000)      812 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_ball-bearings-bag-of-1000.json
+-rw-rw-r--   0 b         (1000) b         (1000)      670 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_barding-breastplate.json
+-rw-rw-r--   0 b         (1000) b         (1000)      667 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_barding-chain-mail.json
+-rw-rw-r--   0 b         (1000) b         (1000)      669 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_barding-chain-shirt.json
+-rw-rw-r--   0 b         (1000) b         (1000)      667 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_barding-half-plate.json
+-rw-rw-r--   0 b         (1000) b         (1000)      647 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_barding-hide.json
+-rw-rw-r--   0 b         (1000) b         (1000)      656 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_barding-leather.json
+-rw-rw-r--   0 b         (1000) b         (1000)      653 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_barding-padded.json
+-rw-rw-r--   0 b         (1000) b         (1000)      653 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_barding-plate.json
+-rw-rw-r--   0 b         (1000) b         (1000)      662 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_barding-ring-mail.json
+-rw-rw-r--   0 b         (1000) b         (1000)      666 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_barding-scale-mail.json
+-rw-rw-r--   0 b         (1000) b         (1000)      655 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_barding-splint.json
+-rw-rw-r--   0 b         (1000) b         (1000)      681 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_barding-studded-leather.json
+-rw-rw-r--   0 b         (1000) b         (1000)      437 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_barrel.json
+-rw-rw-r--   0 b         (1000) b         (1000)      436 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_basket.json
+-rw-rw-r--   0 b         (1000) b         (1000)      766 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_battleaxe.json
+-rw-rw-r--   0 b         (1000) b         (1000)      439 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_bedroll.json
+-rw-rw-r--   0 b         (1000) b         (1000)      430 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_bell.json
+-rw-rw-r--   0 b         (1000) b         (1000)      406 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_bit-and-bridle.json
+-rw-rw-r--   0 b         (1000) b         (1000)      439 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_blanket.json
+-rw-rw-r--   0 b         (1000) b         (1000)      642 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_block-and-tackle.json
+-rw-rw-r--   0 b         (1000) b         (1000)      523 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_block-of-incense.json
+-rw-rw-r--   0 b         (1000) b         (1000)      467 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_blowgun-needle.json
+-rw-rw-r--   0 b         (1000) b         (1000)      718 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_blowgun.json
+-rw-rw-r--   0 b         (1000) b         (1000)      723 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_book.json
+-rw-rw-r--   0 b         (1000) b         (1000)      455 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_bottle-glass.json
+-rw-rw-r--   0 b         (1000) b         (1000)      442 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_breastplate.json
+-rw-rw-r--   0 b         (1000) b         (1000)      735 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_brewers-supplies.json
+-rw-rw-r--   0 b         (1000) b         (1000)      436 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_bucket.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2000 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_burglars-pack.json
+-rw-rw-r--   0 b         (1000) b         (1000)      753 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_calligraphers-supplies.json
+-rw-rw-r--   0 b         (1000) b         (1000)      878 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_caltrops.json
+-rw-rw-r--   0 b         (1000) b         (1000)      428 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_camel.json
+-rw-rw-r--   0 b         (1000) b         (1000)      536 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_candle.json
+-rw-rw-r--   0 b         (1000) b         (1000)      734 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_carpenters-tools.json
+-rw-rw-r--   0 b         (1000) b         (1000)      392 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_carriage.json
+-rw-rw-r--   0 b         (1000) b         (1000)      379 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_cart.json
+-rw-rw-r--   0 b         (1000) b         (1000)      744 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_cartographers-tools.json
+-rw-rw-r--   0 b         (1000) b         (1000)      529 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_case-crossbow-bolt.json
+-rw-rw-r--   0 b         (1000) b         (1000)      588 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_case-map-or-scroll.json
+-rw-rw-r--   0 b         (1000) b         (1000)      483 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_censer.json
+-rw-rw-r--   0 b         (1000) b         (1000)      544 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_chain-10-feet.json
+-rw-rw-r--   0 b         (1000) b         (1000)      422 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_chain-mail.json
+-rw-rw-r--   0 b         (1000) b         (1000)      441 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_chain-shirt.json
+-rw-rw-r--   0 b         (1000) b         (1000)      459 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_chalk-1-piece.json
+-rw-rw-r--   0 b         (1000) b         (1000)      389 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_chariot.json
+-rw-rw-r--   0 b         (1000) b         (1000)      434 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_chest.json
+-rw-rw-r--   0 b         (1000) b         (1000)      746 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_climbers-kit.json
+-rw-rw-r--   0 b         (1000) b         (1000)      461 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_clothes-common.json
+-rw-rw-r--   0 b         (1000) b         (1000)      464 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_clothes-costume.json
+-rw-rw-r--   0 b         (1000) b         (1000)      456 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_clothes-fine.json
+-rw-rw-r--   0 b         (1000) b         (1000)      471 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_clothes-travelers.json
+-rw-rw-r--   0 b         (1000) b         (1000)      677 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_club.json
+-rw-rw-r--   0 b         (1000) b         (1000)      728 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_cobblers-tools.json
+-rw-rw-r--   0 b         (1000) b         (1000)      733 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_component-pouch.json
+-rw-rw-r--   0 b         (1000) b         (1000)      728 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_cooks-utensils.json
+-rw-rw-r--   0 b         (1000) b         (1000)      466 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_crossbow-bolt.json
+-rw-rw-r--   0 b         (1000) b         (1000)      815 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_crossbow-hand.json
+-rw-rw-r--   0 b         (1000) b         (1000)      912 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_crossbow-heavy.json
+-rw-rw-r--   0 b         (1000) b         (1000)      831 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_crossbow-light.json
+-rw-rw-r--   0 b         (1000) b         (1000)      537 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_crowbar.json
+-rw-rw-r--   0 b         (1000) b         (1000)      702 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_crystal.json
+-rw-rw-r--   0 b         (1000) b         (1000)      878 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_dagger.json
+-rw-rw-r--   0 b         (1000) b         (1000)      741 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_dart.json
+-rw-rw-r--   0 b         (1000) b         (1000)      723 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_dice-set.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1666 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_diplomats-pack.json
+-rw-rw-r--   0 b         (1000) b         (1000)      666 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_disguise-kit.json
+-rw-rw-r--   0 b         (1000) b         (1000)      430 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_donkey.json
+-rw-rw-r--   0 b         (1000) b         (1000)      693 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_drum.json
+-rw-rw-r--   0 b         (1000) b         (1000)      707 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_dulcimer.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1412 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_dungeoneers-pack.json
+-rw-rw-r--   0 b         (1000) b         (1000)      440 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_elephant.json
+-rw-rw-r--   0 b         (1000) b         (1000)      934 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_emblem.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1221 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_entertainers-pack.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1318 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_explorers-pack.json
+-rw-rw-r--   0 b         (1000) b         (1000)      585 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_fishing-tackle.json
+-rw-rw-r--   0 b         (1000) b         (1000)      536 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_flail.json
+-rw-rw-r--   0 b         (1000) b         (1000)      466 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_flask-or-tankard.json
+-rw-rw-r--   0 b         (1000) b         (1000)      696 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_flute.json
+-rw-rw-r--   0 b         (1000) b         (1000)      766 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_forgery-kit.json
+-rw-rw-r--   0 b         (1000) b         (1000)      400 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_galley.json
+-rw-rw-r--   0 b         (1000) b         (1000)      772 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_glaive.json
+-rw-rw-r--   0 b         (1000) b         (1000)      741 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_glassblowers-tools.json
+-rw-rw-r--   0 b         (1000) b         (1000)      460 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_grappling-hook.json
+-rw-rw-r--   0 b         (1000) b         (1000)      702 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_greataxe.json
+-rw-rw-r--   0 b         (1000) b         (1000)      635 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_greatclub.json
+-rw-rw-r--   0 b         (1000) b         (1000)      707 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_greatsword.json
+-rw-rw-r--   0 b         (1000) b         (1000)      775 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_halberd.json
+-rw-rw-r--   0 b         (1000) b         (1000)      456 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_half-plate-armor.json
+-rw-rw-r--   0 b         (1000) b         (1000)      459 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_hammer-sledge.json
+-rw-rw-r--   0 b         (1000) b         (1000)      436 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_hammer.json
+-rw-rw-r--   0 b         (1000) b         (1000)      799 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_handaxe.json
+-rw-rw-r--   0 b         (1000) b         (1000)      664 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_healers-kit.json
+-rw-rw-r--   0 b         (1000) b         (1000)      793 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_herbalism-kit.json
+-rw-rw-r--   0 b         (1000) b         (1000)      438 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_hide-armor.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1007 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_holy-water-flask.json
+-rw-rw-r--   0 b         (1000) b         (1000)      693 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_horn.json
+-rw-rw-r--   0 b         (1000) b         (1000)      447 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_horse-draft.json
+-rw-rw-r--   0 b         (1000) b         (1000)      450 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_horse-riding.json
+-rw-rw-r--   0 b         (1000) b         (1000)      446 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_hourglass.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1176 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_hunting-trap.json
+-rw-rw-r--   0 b         (1000) b         (1000)      475 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_ink-1-ounce-bottle.json
+-rw-rw-r--   0 b         (1000) b         (1000)      439 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_ink-pen.json
+-rw-rw-r--   0 b         (1000) b         (1000)      724 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_javelin.json
+-rw-rw-r--   0 b         (1000) b         (1000)      729 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_jewelers-tools.json
+-rw-rw-r--   0 b         (1000) b         (1000)      460 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_jug-or-pitcher.json
+-rw-rw-r--   0 b         (1000) b         (1000)      763 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_keelboat.json
+-rw-rw-r--   0 b         (1000) b         (1000)      463 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_ladder-10-foot.json
+-rw-rw-r--   0 b         (1000) b         (1000)      577 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_lamp.json
+-rw-rw-r--   0 b         (1000) b         (1000)      836 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_lance.json
+-rw-rw-r--   0 b         (1000) b         (1000)      625 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_lantern-bullseye.json
+-rw-rw-r--   0 b         (1000) b         (1000)      708 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_lantern-hooded.json
+-rw-rw-r--   0 b         (1000) b         (1000)      430 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_leather-armor.json
+-rw-rw-r--   0 b         (1000) b         (1000)      746 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_leatherworkers-tools.json
+-rw-rw-r--   0 b         (1000) b         (1000)      823 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_light-hammer.json
+-rw-rw-r--   0 b         (1000) b         (1000)      531 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_little-bag-of-sand.json
+-rw-rw-r--   0 b         (1000) b         (1000)      654 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_lock.json
+-rw-rw-r--   0 b         (1000) b         (1000)      806 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_longbow.json
+-rw-rw-r--   0 b         (1000) b         (1000)      406 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_longship.json
+-rw-rw-r--   0 b         (1000) b         (1000)      766 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_longsword.json
+-rw-rw-r--   0 b         (1000) b         (1000)      694 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_lute.json
+-rw-rw-r--   0 b         (1000) b         (1000)      694 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_lyre.json
+-rw-rw-r--   0 b         (1000) b         (1000)      601 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_mace.json
+-rw-rw-r--   0 b         (1000) b         (1000)      872 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_magnifying-glass.json
+-rw-rw-r--   0 b         (1000) b         (1000)      829 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_manacles.json
+-rw-rw-r--   0 b         (1000) b         (1000)      723 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_masons-tools.json
+-rw-rw-r--   0 b         (1000) b         (1000)      434 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_mastiff.json
+-rw-rw-r--   0 b         (1000) b         (1000)      699 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_maul.json
+-rw-rw-r--   0 b         (1000) b         (1000)      573 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_mess-kit.json
+-rw-rw-r--   0 b         (1000) b         (1000)      457 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_mirror-steel.json
+-rw-rw-r--   0 b         (1000) b         (1000)      545 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_morningstar.json
+-rw-rw-r--   0 b         (1000) b         (1000)      424 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_mule.json
+-rw-rw-r--   0 b         (1000) b         (1000)      624 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_navigators-tools.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1190 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_net.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1227 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_oil-flask.json
+-rw-rw-r--   0 b         (1000) b         (1000)      690 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_orb.json
+-rw-rw-r--   0 b         (1000) b         (1000)      424 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_padded-armor.json
+-rw-rw-r--   0 b         (1000) b         (1000)      738 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_painters-supplies.json
+-rw-rw-r--   0 b         (1000) b         (1000)      709 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_pan-flute.json
+-rw-rw-r--   0 b         (1000) b         (1000)      465 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_paper-one-sheet.json
+-rw-rw-r--   0 b         (1000) b         (1000)      477 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_parchment-one-sheet.json
+-rw-rw-r--   0 b         (1000) b         (1000)      456 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_perfume-vial.json
+-rw-rw-r--   0 b         (1000) b         (1000)      454 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_pick-miners.json
+-rw-rw-r--   0 b         (1000) b         (1000)      766 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_pike.json
+-rw-rw-r--   0 b         (1000) b         (1000)      436 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_piton.json
+-rw-rw-r--   0 b         (1000) b         (1000)      427 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_plate-armor.json
+-rw-rw-r--   0 b         (1000) b         (1000)      747 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_playing-card-set.json
+-rw-rw-r--   0 b         (1000) b         (1000)      817 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_poison-basic-vial.json
+-rw-rw-r--   0 b         (1000) b         (1000)      658 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_poisoners-kit.json
+-rw-rw-r--   0 b         (1000) b         (1000)      456 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_pole-10-foot.json
+-rw-rw-r--   0 b         (1000) b         (1000)      425 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_pony.json
+-rw-rw-r--   0 b         (1000) b         (1000)      444 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_pot-iron.json
+-rw-rw-r--   0 b         (1000) b         (1000)      726 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_potters-tools.json
+-rw-rw-r--   0 b         (1000) b         (1000)      654 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_pouch.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1503 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_priests-pack.json
+-rw-rw-r--   0 b         (1000) b         (1000)      862 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_quarterstaff.json
+-rw-rw-r--   0 b         (1000) b         (1000)      472 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_quiver.json
+-rw-rw-r--   0 b         (1000) b         (1000)      645 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_ram-portable.json
+-rw-rw-r--   0 b         (1000) b         (1000)      610 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_rapier.json
+-rw-rw-r--   0 b         (1000) b         (1000)      569 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_rations-1-day.json
+-rw-rw-r--   0 b         (1000) b         (1000)      943 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_reliquary.json
+-rw-rw-r--   0 b         (1000) b         (1000)      418 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_ring-mail.json
+-rw-rw-r--   0 b         (1000) b         (1000)      433 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_robes.json
+-rw-rw-r--   0 b         (1000) b         (1000)      690 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_rod.json
+-rw-rw-r--   0 b         (1000) b         (1000)      579 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_rope-hempen-50-feet.json
+-rw-rw-r--   0 b         (1000) b         (1000)      573 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_rope-silk-50-feet.json
+-rw-rw-r--   0 b         (1000) b         (1000)      760 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_rowboat.json
+-rw-rw-r--   0 b         (1000) b         (1000)      432 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_sack.json
+-rw-rw-r--   0 b         (1000) b         (1000)      476 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_saddle-exotic.json
+-rw-rw-r--   0 b         (1000) b         (1000)      570 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_saddle-military.json
+-rw-rw-r--   0 b         (1000) b         (1000)      399 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_saddle-pack.json
+-rw-rw-r--   0 b         (1000) b         (1000)      406 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_saddle-riding.json
+-rw-rw-r--   0 b         (1000) b         (1000)      394 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_saddlebags.json
+-rw-rw-r--   0 b         (1000) b         (1000)      418 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_sailing-ship.json
+-rw-rw-r--   0 b         (1000) b         (1000)      437 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_scale-mail.json
+-rw-rw-r--   0 b         (1000) b         (1000)      694 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_scale-merchants.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1256 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_scholars-pack.json
+-rw-rw-r--   0 b         (1000) b         (1000)      692 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_scimitar.json
+-rw-rw-r--   0 b         (1000) b         (1000)      451 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_sealing-wax.json
+-rw-rw-r--   0 b         (1000) b         (1000)      696 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_shawm.json
+-rw-rw-r--   0 b         (1000) b         (1000)      409 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_shield.json
+-rw-rw-r--   0 b         (1000) b         (1000)      730 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_shortbow.json
+-rw-rw-r--   0 b         (1000) b         (1000)      771 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_shortsword.json
+-rw-rw-r--   0 b         (1000) b         (1000)      436 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_shovel.json
+-rw-rw-r--   0 b         (1000) b         (1000)      674 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_sickle.json
+-rw-rw-r--   0 b         (1000) b         (1000)      460 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_signal-whistle.json
+-rw-rw-r--   0 b         (1000) b         (1000)      451 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_signet-ring.json
+-rw-rw-r--   0 b         (1000) b         (1000)      379 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_sled.json
+-rw-rw-r--   0 b         (1000) b         (1000)      463 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_sling-bullet.json
+-rw-rw-r--   0 b         (1000) b         (1000)      638 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_sling.json
+-rw-rw-r--   0 b         (1000) b         (1000)      504 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_small-knife.json
+-rw-rw-r--   0 b         (1000) b         (1000)      723 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_smiths-tools.json
+-rw-rw-r--   0 b         (1000) b         (1000)      430 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_soap.json
+-rw-rw-r--   0 b         (1000) b         (1000)      945 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_spear.json
+-rw-rw-r--   0 b         (1000) b         (1000)      565 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_spellbook.json
+-rw-rw-r--   0 b         (1000) b         (1000)      449 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_spike-iron.json
+-rw-rw-r--   0 b         (1000) b         (1000)      429 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_splint-armor.json
+-rw-rw-r--   0 b         (1000) b         (1000)      764 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_sprig-of-mistletoe.json
+-rw-rw-r--   0 b         (1000) b         (1000)      515 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_spyglass.json
+-rw-rw-r--   0 b         (1000) b         (1000)      408 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_stabling-1-day.json
+-rw-rw-r--   0 b         (1000) b         (1000)      695 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_staff.json
+-rw-rw-r--   0 b         (1000) b         (1000)      528 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_string-10-feet.json
+-rw-rw-r--   0 b         (1000) b         (1000)      454 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_studded-leather-armor.json
+-rw-rw-r--   0 b         (1000) b         (1000)      523 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_tent-two-person.json
+-rw-rw-r--   0 b         (1000) b         (1000)      625 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_thieves-tools.json
+-rw-rw-r--   0 b         (1000) b         (1000)      699 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_tinderbox.json
+-rw-rw-r--   0 b         (1000) b         (1000)      727 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_tinkers-tools.json
+-rw-rw-r--   0 b         (1000) b         (1000)      625 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_torch.json
+-rw-rw-r--   0 b         (1000) b         (1000)      725 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_totem.json
+-rw-rw-r--   0 b         (1000) b         (1000)      880 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_trident.json
+-rw-rw-r--   0 b         (1000) b         (1000)      502 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_vestments.json
+-rw-rw-r--   0 b         (1000) b         (1000)      430 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_vial.json
+-rw-rw-r--   0 b         (1000) b         (1000)      694 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_viol.json
+-rw-rw-r--   0 b         (1000) b         (1000)      382 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_wagon.json
+-rw-rw-r--   0 b         (1000) b         (1000)      693 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_wand.json
+-rw-rw-r--   0 b         (1000) b         (1000)      535 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_war-pick.json
+-rw-rw-r--   0 b         (1000) b         (1000)      784 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_warhammer.json
+-rw-rw-r--   0 b         (1000) b         (1000)      438 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_warhorse.json
+-rw-rw-r--   0 b         (1000) b         (1000)      405 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_warship.json
+-rw-rw-r--   0 b         (1000) b         (1000)      445 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_waterskin.json
+-rw-rw-r--   0 b         (1000) b         (1000)      725 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_weavers-tools.json
+-rw-rw-r--   0 b         (1000) b         (1000)      445 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_whetstone.json
+-rw-rw-r--   0 b         (1000) b         (1000)      679 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_whip.json
+-rw-rw-r--   0 b         (1000) b         (1000)      737 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_woodcarvers-tools.json
+-rw-rw-r--   0 b         (1000) b         (1000)      746 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_wooden-staff.json
+-rw-rw-r--   0 b         (1000) b         (1000)      735 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_equipment_yew-wand.json
+-rw-rw-r--   0 b         (1000) b         (1000)      614 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_action-surge-1-use.json
+-rw-rw-r--   0 b         (1000) b         (1000)      618 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_action-surge-2-uses.json
+-rw-rw-r--   0 b         (1000) b         (1000)      729 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_arcane-recovery.json
+-rw-rw-r--   0 b         (1000) b         (1000)      448 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_arcane-tradition.json
+-rw-rw-r--   0 b         (1000) b         (1000)      530 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_archdruid.json
+-rw-rw-r--   0 b         (1000) b         (1000)      289 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_aura-improvements.json
+-rw-rw-r--   0 b         (1000) b         (1000)      404 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_aura-of-courage.json
+-rw-rw-r--   0 b         (1000) b         (1000)      553 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_aura-of-protection.json
+-rw-rw-r--   0 b         (1000) b         (1000)      546 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_barbarian-ability-score-improvement-1.json
+-rw-rw-r--   0 b         (1000) b         (1000)      546 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_barbarian-ability-score-improvement-2.json
+-rw-rw-r--   0 b         (1000) b         (1000)      547 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_barbarian-ability-score-improvement-3.json
+-rw-rw-r--   0 b         (1000) b         (1000)      547 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_barbarian-ability-score-improvement-4.json
+-rw-rw-r--   0 b         (1000) b         (1000)      547 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_barbarian-ability-score-improvement-5.json
+-rw-rw-r--   0 b         (1000) b         (1000)      352 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_barbarian-extra-attack.json
+-rw-rw-r--   0 b         (1000) b         (1000)      424 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_barbarian-unarmored-defense.json
+-rw-rw-r--   0 b         (1000) b         (1000)      521 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_bard-ability-score-improvement-1.json
+-rw-rw-r--   0 b         (1000) b         (1000)      521 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_bard-ability-score-improvement-2.json
+-rw-rw-r--   0 b         (1000) b         (1000)      522 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_bard-ability-score-improvement-3.json
+-rw-rw-r--   0 b         (1000) b         (1000)      522 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_bard-ability-score-improvement-4.json
+-rw-rw-r--   0 b         (1000) b         (1000)      522 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_bard-ability-score-improvement-5.json
+-rw-rw-r--   0 b         (1000) b         (1000)      398 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_bard-college.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3182 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_bard-expertise-1.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3183 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_bard-expertise-2.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1240 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_bardic-inspiration-d10.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1240 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_bardic-inspiration-d12.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1236 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_bardic-inspiration-d6.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1236 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_bardic-inspiration-d8.json
+-rw-rw-r--   0 b         (1000) b         (1000)      457 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_beast-spells.json
+-rw-rw-r--   0 b         (1000) b         (1000)      340 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_blindsense.json
+-rw-rw-r--   0 b         (1000) b         (1000)      485 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_brutal-critical-1-die.json
+-rw-rw-r--   0 b         (1000) b         (1000)      489 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_brutal-critical-2-dice.json
+-rw-rw-r--   0 b         (1000) b         (1000)      489 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_brutal-critical-3-dice.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1080 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_channel-divinity-1-rest.json
+-rw-rw-r--   0 b         (1000) b         (1000)      464 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_channel-divinity-2-rest.json
+-rw-rw-r--   0 b         (1000) b         (1000)      465 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_channel-divinity-3-rest.json
+-rw-rw-r--   0 b         (1000) b         (1000)      889 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_channel-divinity-turn-undead.json
+-rw-rw-r--   0 b         (1000) b         (1000)      663 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_channel-divinity.json
+-rw-rw-r--   0 b         (1000) b         (1000)      497 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_cleansing-touch.json
+-rw-rw-r--   0 b         (1000) b         (1000)      531 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_cleric-ability-score-improvement-1.json
+-rw-rw-r--   0 b         (1000) b         (1000)      531 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_cleric-ability-score-improvement-2.json
+-rw-rw-r--   0 b         (1000) b         (1000)      532 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_cleric-ability-score-improvement-3.json
+-rw-rw-r--   0 b         (1000) b         (1000)      532 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_cleric-ability-score-improvement-4.json
+-rw-rw-r--   0 b         (1000) b         (1000)      532 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_cleric-ability-score-improvement-5.json
+-rw-rw-r--   0 b         (1000) b         (1000)      714 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_countercharm.json
+-rw-rw-r--   0 b         (1000) b         (1000)      438 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_cunning-action.json
+-rw-rw-r--   0 b         (1000) b         (1000)      537 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_danger-sense.json
+-rw-rw-r--   0 b         (1000) b         (1000)      976 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_deflect-missiles.json
+-rw-rw-r--   0 b         (1000) b         (1000)      457 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_destroy-undead-cr-1-2-or-below.json
+-rw-rw-r--   0 b         (1000) b         (1000)      451 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_destroy-undead-cr-1-or-below.json
+-rw-rw-r--   0 b         (1000) b         (1000)      452 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_destroy-undead-cr-2-or-below.json
+-rw-rw-r--   0 b         (1000) b         (1000)      452 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_destroy-undead-cr-3-or-below.json
+-rw-rw-r--   0 b         (1000) b         (1000)      452 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_destroy-undead-cr-4-or-below.json
+-rw-rw-r--   0 b         (1000) b         (1000)      420 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_diamond-soul.json
+-rw-rw-r--   0 b         (1000) b         (1000)      725 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_divine-domain.json
+-rw-rw-r--   0 b         (1000) b         (1000)      296 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_divine-health.json
+-rw-rw-r--   0 b         (1000) b         (1000)      352 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_divine-intervention-improvement.json
+-rw-rw-r--   0 b         (1000) b         (1000)      892 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_divine-intervention.json
+-rw-rw-r--   0 b         (1000) b         (1000)      948 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_divine-sense.json
+-rw-rw-r--   0 b         (1000) b         (1000)      579 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_divine-smite.json
+-rw-rw-r--   0 b         (1000) b         (1000)      598 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_domain-spells-1.json
+-rw-rw-r--   0 b         (1000) b         (1000)      598 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_domain-spells-2.json
+-rw-rw-r--   0 b         (1000) b         (1000)      598 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_domain-spells-3.json
+-rw-rw-r--   0 b         (1000) b         (1000)      598 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_domain-spells-4.json
+-rw-rw-r--   0 b         (1000) b         (1000)      598 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_domain-spells-5.json
+-rw-rw-r--   0 b         (1000) b         (1000)      526 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_druid-ability-score-improvement-1.json
+-rw-rw-r--   0 b         (1000) b         (1000)      526 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_druid-ability-score-improvement-2.json
+-rw-rw-r--   0 b         (1000) b         (1000)      527 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_druid-ability-score-improvement-3.json
+-rw-rw-r--   0 b         (1000) b         (1000)      527 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_druid-ability-score-improvement-4.json
+-rw-rw-r--   0 b         (1000) b         (1000)      527 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_druid-ability-score-improvement-5.json
+-rw-rw-r--   0 b         (1000) b         (1000)      386 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_druid-circle.json
+-rw-rw-r--   0 b         (1000) b         (1000)      368 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_druid-timeless-body.json
+-rw-rw-r--   0 b         (1000) b         (1000)      500 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_druidic.json
+-rw-rw-r--   0 b         (1000) b         (1000)     6107 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_eldritch-invocations.json
+-rw-rw-r--   0 b         (1000) b         (1000)      582 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_eldritch-master.json
+-rw-rw-r--   0 b         (1000) b         (1000)      365 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_elusive.json
+-rw-rw-r--   0 b         (1000) b         (1000)      556 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_empty-body.json
+-rw-rw-r--   0 b         (1000) b         (1000)      464 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_extra-attack-1.json
+-rw-rw-r--   0 b         (1000) b         (1000)      469 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_extra-attack-2.json
+-rw-rw-r--   0 b         (1000) b         (1000)      469 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_extra-attack-3.json
+-rw-rw-r--   0 b         (1000) b         (1000)      315 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_fast-movement.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1129 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_favored-enemy-1-type.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1132 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_favored-enemy-2-types.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1139 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_favored-enemy-3-enemies.json
+-rw-rw-r--   0 b         (1000) b         (1000)      517 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_feral-instinct.json
+-rw-rw-r--   0 b         (1000) b         (1000)      601 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_feral-senses.json
+-rw-rw-r--   0 b         (1000) b         (1000)      547 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_fighter-ability-score-improvement-1.json
+-rw-rw-r--   0 b         (1000) b         (1000)      547 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_fighter-ability-score-improvement-2.json
+-rw-rw-r--   0 b         (1000) b         (1000)      547 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_fighter-ability-score-improvement-3.json
+-rw-rw-r--   0 b         (1000) b         (1000)      548 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_fighter-ability-score-improvement-4.json
+-rw-rw-r--   0 b         (1000) b         (1000)      548 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_fighter-ability-score-improvement-5.json
+-rw-rw-r--   0 b         (1000) b         (1000)      548 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_fighter-ability-score-improvement-6.json
+-rw-rw-r--   0 b         (1000) b         (1000)      548 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_fighter-ability-score-improvement-7.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1707 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_fighter-fighting-style.json
+-rw-rw-r--   0 b         (1000) b         (1000)      421 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_flexible-casting-converting-spell-slot.json
+-rw-rw-r--   0 b         (1000) b         (1000)      619 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_flexible-casting-creating-spell-slots.json
+-rw-rw-r--   0 b         (1000) b         (1000)      344 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_flurry-of-blows.json
+-rw-rw-r--   0 b         (1000) b         (1000)      538 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_foe-slayer.json
+-rw-rw-r--   0 b         (1000) b         (1000)      358 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_font-of-inspiration.json
+-rw-rw-r--   0 b         (1000) b         (1000)      695 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_font-of-magic.json
+-rw-rw-r--   0 b         (1000) b         (1000)      843 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_hide-in-plain-sight.json
+-rw-rw-r--   0 b         (1000) b         (1000)      571 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_improved-divine-smite.json
+-rw-rw-r--   0 b         (1000) b         (1000)      539 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_indomitable-1-use.json
+-rw-rw-r--   0 b         (1000) b         (1000)      543 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_indomitable-2-uses.json
+-rw-rw-r--   0 b         (1000) b         (1000)      543 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_indomitable-3-uses.json
+-rw-rw-r--   0 b         (1000) b         (1000)      375 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_indomitable-might.json
+-rw-rw-r--   0 b         (1000) b         (1000)      383 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_jack-of-all-trades.json
+-rw-rw-r--   0 b         (1000) b         (1000)      377 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_ki-empowered-strikes.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1112 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_ki.json
+-rw-rw-r--   0 b         (1000) b         (1000)      937 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_lay-on-hands.json
+-rw-rw-r--   0 b         (1000) b         (1000)      673 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_magical-secrets-1.json
+-rw-rw-r--   0 b         (1000) b         (1000)      673 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_magical-secrets-2.json
+-rw-rw-r--   0 b         (1000) b         (1000)      673 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_magical-secrets-3.json
+-rw-rw-r--   0 b         (1000) b         (1000)      453 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_martial-archetype.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1544 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_martial-arts.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1947 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_metamagic-1.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1948 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_metamagic-2.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1948 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_metamagic-3.json
+-rw-rw-r--   0 b         (1000) b         (1000)      415 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_monastic-tradition.json
+-rw-rw-r--   0 b         (1000) b         (1000)      521 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_monk-ability-score-improvement-1.json
+-rw-rw-r--   0 b         (1000) b         (1000)      521 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_monk-ability-score-improvement-2.json
+-rw-rw-r--   0 b         (1000) b         (1000)      522 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_monk-ability-score-improvement-3.json
+-rw-rw-r--   0 b         (1000) b         (1000)      522 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_monk-ability-score-improvement-4.json
+-rw-rw-r--   0 b         (1000) b         (1000)      522 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_monk-ability-score-improvement-5.json
+-rw-rw-r--   0 b         (1000) b         (1000)      563 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_monk-evasion.json
+-rw-rw-r--   0 b         (1000) b         (1000)      327 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_monk-extra-attack.json
+-rw-rw-r--   0 b         (1000) b         (1000)      424 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_monk-timeless-body.json
+-rw-rw-r--   0 b         (1000) b         (1000)      379 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_monk-unarmored-defense.json
+-rw-rw-r--   0 b         (1000) b         (1000)      810 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_mystic-arcanum-6th-level.json
+-rw-rw-r--   0 b         (1000) b         (1000)      810 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_mystic-arcanum-7th-level.json
+-rw-rw-r--   0 b         (1000) b         (1000)      810 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_mystic-arcanum-8th-level.json
+-rw-rw-r--   0 b         (1000) b         (1000)      810 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_mystic-arcanum-9th-level.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1360 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_natural-explorer-1-terrain-type.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1363 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_natural-explorer-2-terrain-types.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1364 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_natural-explorer-3-terrain-types.json
+-rw-rw-r--   0 b         (1000) b         (1000)      607 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_oath-spells.json
+-rw-rw-r--   0 b         (1000) b         (1000)      421 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_otherworldly-patron.json
+-rw-rw-r--   0 b         (1000) b         (1000)      922 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_pact-boon.json
+-rw-rw-r--   0 b         (1000) b         (1000)      360 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_pact-magic.json
+-rw-rw-r--   0 b         (1000) b         (1000)      536 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_paladin-ability-score-improvement-1.json
+-rw-rw-r--   0 b         (1000) b         (1000)      536 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_paladin-ability-score-improvement-2.json
+-rw-rw-r--   0 b         (1000) b         (1000)      537 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_paladin-ability-score-improvement-3.json
+-rw-rw-r--   0 b         (1000) b         (1000)      537 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_paladin-ability-score-improvement-4.json
+-rw-rw-r--   0 b         (1000) b         (1000)      537 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_paladin-ability-score-improvement-5.json
+-rw-rw-r--   0 b         (1000) b         (1000)      342 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_paladin-extra-attack.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1264 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_paladin-fighting-style.json
+-rw-rw-r--   0 b         (1000) b         (1000)      295 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_patient-defense.json
+-rw-rw-r--   0 b         (1000) b         (1000)      306 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_perfect-self.json
+-rw-rw-r--   0 b         (1000) b         (1000)      353 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_persistent-rage.json
+-rw-rw-r--   0 b         (1000) b         (1000)      373 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_primal-champion.json
+-rw-rw-r--   0 b         (1000) b         (1000)      489 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_primal-path.json
+-rw-rw-r--   0 b         (1000) b         (1000)      696 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_primeval-awareness.json
+-rw-rw-r--   0 b         (1000) b         (1000)      309 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_purity-of-body.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1204 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_rage.json
+-rw-rw-r--   0 b         (1000) b         (1000)      531 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_ranger-ability-score-improvement-1.json
+-rw-rw-r--   0 b         (1000) b         (1000)      531 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_ranger-ability-score-improvement-2.json
+-rw-rw-r--   0 b         (1000) b         (1000)      532 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_ranger-ability-score-improvement-3.json
+-rw-rw-r--   0 b         (1000) b         (1000)      532 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_ranger-ability-score-improvement-4.json
+-rw-rw-r--   0 b         (1000) b         (1000)      532 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_ranger-ability-score-improvement-5.json
+-rw-rw-r--   0 b         (1000) b         (1000)      393 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_ranger-archetype.json
+-rw-rw-r--   0 b         (1000) b         (1000)      337 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_ranger-extra-attack.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1311 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_ranger-fighting-style.json
+-rw-rw-r--   0 b         (1000) b         (1000)      651 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_ranger-lands-stride.json
+-rw-rw-r--   0 b         (1000) b         (1000)      570 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_reckless-attack.json
+-rw-rw-r--   0 b         (1000) b         (1000)      612 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_relentless-rage.json
+-rw-rw-r--   0 b         (1000) b         (1000)      425 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_reliable-talent.json
+-rw-rw-r--   0 b         (1000) b         (1000)      532 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_rogue-ability-score-improvement-1.json
+-rw-rw-r--   0 b         (1000) b         (1000)      532 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_rogue-ability-score-improvement-2.json
+-rw-rw-r--   0 b         (1000) b         (1000)      533 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_rogue-ability-score-improvement-3.json
+-rw-rw-r--   0 b         (1000) b         (1000)      533 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_rogue-ability-score-improvement-4.json
+-rw-rw-r--   0 b         (1000) b         (1000)      533 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_rogue-ability-score-improvement-5.json
+-rw-rw-r--   0 b         (1000) b         (1000)      533 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_rogue-ability-score-improvement-6.json
+-rw-rw-r--   0 b         (1000) b         (1000)      556 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_rogue-evasion.json
+-rw-rw-r--   0 b         (1000) b         (1000)     6307 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_rogue-expertise-1.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3434 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_rogue-expertise-2.json
+-rw-rw-r--   0 b         (1000) b         (1000)      502 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_roguish-archetype.json
+-rw-rw-r--   0 b         (1000) b         (1000)      604 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_sacred-oath.json
+-rw-rw-r--   0 b         (1000) b         (1000)      488 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_second-wind.json
+-rw-rw-r--   0 b         (1000) b         (1000)      762 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_signature-spell.json
+-rw-rw-r--   0 b         (1000) b         (1000)      315 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_slippery-mind.json
+-rw-rw-r--   0 b         (1000) b         (1000)      347 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_slow-fall.json
+-rw-rw-r--   0 b         (1000) b         (1000)      793 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_sneak-attack.json
+-rw-rw-r--   0 b         (1000) b         (1000)      692 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_song-of-rest-d10.json
+-rw-rw-r--   0 b         (1000) b         (1000)      692 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_song-of-rest-d12.json
+-rw-rw-r--   0 b         (1000) b         (1000)      688 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_song-of-rest-d6.json
+-rw-rw-r--   0 b         (1000) b         (1000)      688 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_song-of-rest-d8.json
+-rw-rw-r--   0 b         (1000) b         (1000)      541 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_sorcerer-ability-score-improvement-1.json
+-rw-rw-r--   0 b         (1000) b         (1000)      541 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_sorcerer-ability-score-improvement-2.json
+-rw-rw-r--   0 b         (1000) b         (1000)      542 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_sorcerer-ability-score-improvement-3.json
+-rw-rw-r--   0 b         (1000) b         (1000)      542 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_sorcerer-ability-score-improvement-4.json
+-rw-rw-r--   0 b         (1000) b         (1000)      542 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_sorcerer-ability-score-improvement-5.json
+-rw-rw-r--   0 b         (1000) b         (1000)      447 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_sorcerous-origin.json
+-rw-rw-r--   0 b         (1000) b         (1000)      330 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_sorcerous-restoration.json
+-rw-rw-r--   0 b         (1000) b         (1000)      728 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_spell-mastery.json
+-rw-rw-r--   0 b         (1000) b         (1000)      464 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_spellcasting-bard.json
+-rw-rw-r--   0 b         (1000) b         (1000)      340 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_spellcasting-cleric.json
+-rw-rw-r--   0 b         (1000) b         (1000)      378 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_spellcasting-druid.json
+-rw-rw-r--   0 b         (1000) b         (1000)      406 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_spellcasting-paladin.json
+-rw-rw-r--   0 b         (1000) b         (1000)      406 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_spellcasting-ranger.json
+-rw-rw-r--   0 b         (1000) b         (1000)      481 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_spellcasting-sorcerer.json
+-rw-rw-r--   0 b         (1000) b         (1000)      402 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_spellcasting-wizard.json
+-rw-rw-r--   0 b         (1000) b         (1000)      358 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_step-of-the-wind.json
+-rw-rw-r--   0 b         (1000) b         (1000)      345 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_stillness-of-mind.json
+-rw-rw-r--   0 b         (1000) b         (1000)      540 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_stroke-of-luck.json
+-rw-rw-r--   0 b         (1000) b         (1000)      512 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_stunning-strike.json
+-rw-rw-r--   0 b         (1000) b         (1000)      334 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_superior-inspiration.json
+-rw-rw-r--   0 b         (1000) b         (1000)      846 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_thieves-cant.json
+-rw-rw-r--   0 b         (1000) b         (1000)      440 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_tongue-of-the-sun-and-moon.json
+-rw-rw-r--   0 b         (1000) b         (1000)      556 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_unarmored-movement-1.json
+-rw-rw-r--   0 b         (1000) b         (1000)      556 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_unarmored-movement-2.json
+-rw-rw-r--   0 b         (1000) b         (1000)      360 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_uncanny-dodge.json
+-rw-rw-r--   0 b         (1000) b         (1000)      361 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_vanish.json
+-rw-rw-r--   0 b         (1000) b         (1000)      536 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_warlock-ability-score-improvement-1.json
+-rw-rw-r--   0 b         (1000) b         (1000)      536 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_warlock-ability-score-improvement-2.json
+-rw-rw-r--   0 b         (1000) b         (1000)      537 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_warlock-ability-score-improvement-3.json
+-rw-rw-r--   0 b         (1000) b         (1000)      537 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_warlock-ability-score-improvement-4.json
+-rw-rw-r--   0 b         (1000) b         (1000)      537 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_warlock-ability-score-improvement-5.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3304 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_wild-shape-cr-1-2-or-below-no-flying-speed.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3328 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_wild-shape-cr-1-4-or-below-no-flying-or-swim-speed.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3249 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_wild-shape-cr-1-or-below.json
+-rw-rw-r--   0 b         (1000) b         (1000)      531 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_wizard-ability-score-improvement-1.json
+-rw-rw-r--   0 b         (1000) b         (1000)      531 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_wizard-ability-score-improvement-2.json
+-rw-rw-r--   0 b         (1000) b         (1000)      532 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_wizard-ability-score-improvement-3.json
+-rw-rw-r--   0 b         (1000) b         (1000)      532 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_wizard-ability-score-improvement-4.json
+-rw-rw-r--   0 b         (1000) b         (1000)      532 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_features_wizard-ability-score-improvement-5.json
+-rw-rw-r--   0 b         (1000) b         (1000)    28083 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters.json
+-rw-rw-r--   0 b         (1000) b         (1000)     5182 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_aboleth.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2451 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_acolyte.json
+-rw-rw-r--   0 b         (1000) b         (1000)     5211 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_adult-black-dragon.json
+-rw-rw-r--   0 b         (1000) b         (1000)     5138 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_adult-blue-dragon.json
+-rw-rw-r--   0 b         (1000) b         (1000)     5890 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_adult-brass-dragon.json
+-rw-rw-r--   0 b         (1000) b         (1000)     5817 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_adult-bronze-dragon.json
+-rw-rw-r--   0 b         (1000) b         (1000)     6007 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_adult-copper-dragon.json
+-rw-rw-r--   0 b         (1000) b         (1000)     6028 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_adult-gold-dragon.json
+-rw-rw-r--   0 b         (1000) b         (1000)     5636 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_adult-green-dragon.json
+-rw-rw-r--   0 b         (1000) b         (1000)     5058 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_adult-red-dragon.json
+-rw-rw-r--   0 b         (1000) b         (1000)     5875 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_adult-silver-dragon.json
+-rw-rw-r--   0 b         (1000) b         (1000)     5302 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_adult-white-dragon.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2911 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_air-elemental.json
+-rw-rw-r--   0 b         (1000) b         (1000)     5230 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_ancient-black-dragon.json
+-rw-rw-r--   0 b         (1000) b         (1000)     5158 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_ancient-blue-dragon.json
+-rw-rw-r--   0 b         (1000) b         (1000)     6589 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_ancient-brass-dragon.json
+-rw-rw-r--   0 b         (1000) b         (1000)     6518 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_ancient-bronze-dragon.json
+-rw-rw-r--   0 b         (1000) b         (1000)     6707 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_ancient-copper-dragon.json
+-rw-rw-r--   0 b         (1000) b         (1000)     6734 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_ancient-gold-dragon.json
+-rw-rw-r--   0 b         (1000) b         (1000)     5655 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_ancient-green-dragon.json
+-rw-rw-r--   0 b         (1000) b         (1000)     5090 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_ancient-red-dragon.json
+-rw-rw-r--   0 b         (1000) b         (1000)     6582 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_ancient-silver-dragon.json
+-rw-rw-r--   0 b         (1000) b         (1000)     5319 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_ancient-white-dragon.json
+-rw-rw-r--   0 b         (1000) b         (1000)     6803 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_androsphinx.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2304 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_animated-armor.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2143 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_ankheg.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1740 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_ape.json
+-rw-rw-r--   0 b         (1000) b         (1000)     5732 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_archmage.json
+-rw-rw-r--   0 b         (1000) b         (1000)     4238 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_assassin.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1296 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_awakened-shrub.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1328 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_awakened-tree.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1188 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_axe-beak.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2190 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_azer.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1155 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_baboon.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1081 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_badger.json
+-rw-rw-r--   0 b         (1000) b         (1000)     4252 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_balor.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3658 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_bandit-captain.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1875 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_bandit.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3933 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_barbed-devil.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2207 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_basilisk.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1148 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_bat.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3279 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_bearded-devil.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3784 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_behir.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1341 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_berserker.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1630 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_black-bear.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2744 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_black-dragon-wyrmling.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3172 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_black-pudding.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1842 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_blink-dog.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1657 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_blood-hawk.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2675 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_blue-dragon-wyrmling.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1582 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_boar.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3021 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_bone-devil.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3157 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_brass-dragon-wyrmling.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3220 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_bronze-dragon-wyrmling.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1766 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_brown-bear.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2136 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_bugbear.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1995 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_bulette.json
+-rw-rw-r--   0 b         (1000) b         (1000)      943 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_camel.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1294 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_cat.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2873 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_centaur.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3504 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_chain-devil.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3576 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_chimera.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2695 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_chuul.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3368 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_clay-golem.json
+-rw-rw-r--   0 b         (1000) b         (1000)     4159 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_cloaker.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3867 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_cloud-giant.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1321 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_cockatrice.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1121 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_commoner.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1468 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_constrictor-snake.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3405 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_copper-dragon-wyrmling.json
+-rw-rw-r--   0 b         (1000) b         (1000)     5448 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_couatl.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1162 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_crab.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1380 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_crocodile.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3245 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_cult-fanatic.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1801 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_cultist.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2652 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_darkmantle.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2303 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_death-dog.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3318 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_deep-gnome-svirfneblin.json
+-rw-rw-r--   0 b         (1000) b         (1000)      924 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_deer.json
+-rw-rw-r--   0 b         (1000) b         (1000)     4196 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_deva.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1643 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_dire-wolf.json
+-rw-rw-r--   0 b         (1000) b         (1000)     5483 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_djinni.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2826 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_doppelganger.json
+-rw-rw-r--   0 b         (1000) b         (1000)      972 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_draft-horse.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3673 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_dragon-turtle.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2407 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_dretch.json
+-rw-rw-r--   0 b         (1000) b         (1000)     4770 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_drider.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3066 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_drow.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3695 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_druid.json
+-rw-rw-r--   0 b         (1000) b         (1000)     4354 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_dryad.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2854 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_duergar.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2758 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_dust-mephit.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1199 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_eagle.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2060 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_earth-elemental.json
+-rw-rw-r--   0 b         (1000) b         (1000)     4245 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_efreeti.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1593 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_elephant.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1535 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_elk.json
+-rw-rw-r--   0 b         (1000) b         (1000)     4267 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_erinyes.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3216 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_ettercap.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1991 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_ettin.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3030 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_fire-elemental.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2242 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_fire-giant.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3315 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_flesh-golem.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1481 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_flying-snake.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2155 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_flying-sword.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1346 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_frog.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2165 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_frost-giant.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2018 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_gargoyle.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3508 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_gelatinous-cube.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2314 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_ghast.json
+-rw-rw-r--   0 b         (1000) b         (1000)     4590 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_ghost.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1756 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_ghoul.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1726 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_giant-ape.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1661 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_giant-badger.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1188 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_giant-bat.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1471 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_giant-boar.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1297 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_giant-centipede.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1619 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_giant-constrictor-snake.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1312 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_giant-crab.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2032 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_giant-crocodile.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2063 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_giant-eagle.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2093 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_giant-elk.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1465 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_giant-fire-beetle.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2183 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_giant-frog.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1407 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_giant-goat.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1291 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_giant-hyena.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1207 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_giant-lizard.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2138 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_giant-octopus.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1559 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_giant-owl.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1315 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_giant-poisonous-snake.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1659 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_giant-rat-diseased.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1274 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_giant-rat.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1829 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_giant-scorpion.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1533 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_giant-sea-horse.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1509 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_giant-shark.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2679 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_giant-spider.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2073 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_giant-toad.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2291 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_giant-vulture.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1330 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_giant-wasp.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1372 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_giant-weasel.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2195 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_giant-wolf-spider.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3214 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_gibbering-mouther.json
+-rw-rw-r--   0 b         (1000) b         (1000)     4287 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_glabrezu.json
+-rw-rw-r--   0 b         (1000) b         (1000)     4348 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_gladiator.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2362 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_gnoll.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1382 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_goat.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1774 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_goblin.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3294 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_gold-dragon-wyrmling.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2514 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_gorgon.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2635 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_gray-ooze.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2771 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_green-dragon-wyrmling.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3580 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_green-hag.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1791 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_grick.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1785 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_griffon.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2072 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_grimlock.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1860 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_guard.json
+-rw-rw-r--   0 b         (1000) b         (1000)     4418 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_guardian-naga.json
+-rw-rw-r--   0 b         (1000) b         (1000)     4618 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_gynosphinx.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3040 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_half-red-dragon-veteran.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2591 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_harpy.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1172 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_hawk.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2192 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_hell-hound.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2689 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_hezrou.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1605 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_hill-giant.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1777 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_hippogriff.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2086 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_hobgoblin.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1632 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_homunculus.json
+-rw-rw-r--   0 b         (1000) b         (1000)     4160 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_horned-devil.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1591 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_hunter-shark.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2222 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_hydra.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1262 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_hyena.json
+-rw-rw-r--   0 b         (1000) b         (1000)     4586 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_ice-devil.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3181 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_ice-mephit.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2722 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_imp.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2561 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_invisible-stalker.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3626 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_iron-golem.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1402 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_jackal.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1404 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_killer-whale.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2961 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_knight.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1683 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_kobold.json
+-rw-rw-r--   0 b         (1000) b         (1000)     6598 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_kraken.json
+-rw-rw-r--   0 b         (1000) b         (1000)     4022 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_lamia.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1646 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_lemure.json
+-rw-rw-r--   0 b         (1000) b         (1000)     7447 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_lich.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2330 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_lion.json
+-rw-rw-r--   0 b         (1000) b         (1000)      960 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_lizard.json
+-rw-rw-r--   0 b         (1000) b         (1000)     4033 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_lizardfolk.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3800 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_mage.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3042 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_magma-mephit.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2024 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_magmin.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1791 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_mammoth.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2326 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_manticore.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3257 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_marilith.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1530 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_mastiff.json
+-rw-rw-r--   0 b         (1000) b         (1000)     4285 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_medusa.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1612 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_merfolk.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2722 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_merrow.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2528 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_mimic.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1842 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_minotaur-skeleton.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2077 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_minotaur.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1234 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_mule.json
+-rw-rw-r--   0 b         (1000) b         (1000)     7673 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_mummy-lord.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3119 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_mummy.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3471 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_nalfeshnee.json
+-rw-rw-r--   0 b         (1000) b         (1000)     5078 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_night-hag.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1632 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_nightmare.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2051 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_noble.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2257 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_ochre-jelly.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2071 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_octopus.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1529 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_ogre-zombie.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1408 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_ogre.json
+-rw-rw-r--   0 b         (1000) b         (1000)     4881 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_oni.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1682 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_orc.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3229 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_otyugh.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1454 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_owl.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1796 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_owlbear.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2062 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_panther.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1589 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_pegasus.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2155 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_phase-spider.json
+-rw-rw-r--   0 b         (1000) b         (1000)     4979 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_pit-fiend.json
+-rw-rw-r--   0 b         (1000) b         (1000)     4633 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_planetar.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1335 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_plesiosaurus.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1143 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_poisonous-snake.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1763 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_polar-bear.json
+-rw-rw-r--   0 b         (1000) b         (1000)      951 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_pony.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3726 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_priest.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2365 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_pseudodragon.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2905 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_purple-worm.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2872 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_quasit.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1415 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_quipper.json
+-rw-rw-r--   0 b         (1000) b         (1000)     4385 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_rakshasa.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1040 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_rat.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1324 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_raven.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2592 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_red-dragon-wyrmling.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1586 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_reef-shark.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2478 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_remorhaz.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1271 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_rhinoceros.json
+-rw-rw-r--   0 b         (1000) b         (1000)      975 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_riding-horse.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2451 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_roc.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2775 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_roper.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2292 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_rug-of-smothering.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2163 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_rust-monster.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2079 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_saber-toothed-tiger.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3287 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_sahuagin.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2978 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_salamander.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2191 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_satyr.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1114 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_scorpion.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2673 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_scout.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2933 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_sea-hag.json
+-rw-rw-r--   0 b         (1000) b         (1000)      738 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_sea-horse.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2581 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_shadow.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2442 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_shambling-mound.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3043 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_shield-guardian.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1344 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_shrieker.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3156 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_silver-dragon-wyrmling.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1541 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_skeleton.json
+-rw-rw-r--   0 b         (1000) b         (1000)     6690 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_solar.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2545 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_specter.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1583 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_spider.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3819 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_spirit-naga.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2585 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_sprite.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2994 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_spy.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2702 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_steam-mephit.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1410 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_stirge.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2617 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_stone-giant.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2867 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_stone-golem.json
+-rw-rw-r--   0 b         (1000) b         (1000)     4592 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_storm-giant.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3982 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_succubus-incubus.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2199 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_swarm-of-bats.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2033 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_swarm-of-beetles.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2194 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_swarm-of-centipedes.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2014 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_swarm-of-insects.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2184 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_swarm-of-poisonous-snakes.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2235 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_swarm-of-quippers.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2090 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_swarm-of-rats.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1982 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_swarm-of-ravens.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2334 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_swarm-of-spiders.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2005 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_swarm-of-wasps.json
+-rw-rw-r--   0 b         (1000) b         (1000)     6911 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_tarrasque.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2056 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_thug.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2059 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_tiger.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2349 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_treant.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1979 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_tribal-warrior.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1609 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_triceratops.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2050 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_troll.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1920 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_tyrannosaurus-rex.json
+-rw-rw-r--   0 b         (1000) b         (1000)     4630 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_unicorn.json
+-rw-rw-r--   0 b         (1000) b         (1000)     7313 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_vampire-bat.json
+-rw-rw-r--   0 b         (1000) b         (1000)     4923 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_vampire-mist.json
+-rw-rw-r--   0 b         (1000) b         (1000)     4116 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_vampire-spawn.json
+-rw-rw-r--   0 b         (1000) b         (1000)     8320 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_vampire-vampire.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2884 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_veteran.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1567 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_violet-fungus.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3457 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_vrock.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1418 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_vulture.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1225 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_warhorse-skeleton.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1350 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_warhorse.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3436 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_water-elemental.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1356 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_weasel.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2631 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_werebear-bear.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2212 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_werebear-human.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3360 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_werebear-hybrid.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2442 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_wereboar-boar.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2245 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_wereboar-human.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3298 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_wereboar-hybrid.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2956 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_wererat-human.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3780 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_wererat-hybrid.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2140 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_wererat-rat.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2893 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_weretiger-human.json
+-rw-rw-r--   0 b         (1000) b         (1000)     4121 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_weretiger-hybrid.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2932 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_weretiger-tiger.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2585 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_werewolf-human.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2636 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_werewolf-hybrid.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2025 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_werewolf-wolf.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2632 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_white-dragon-wyrmling.json
+-rw-rw-r--   0 b         (1000) b         (1000)     4020 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_wight.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2976 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_will-o-wisp.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2852 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_winter-wolf.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1669 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_wolf.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1800 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_worg.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2895 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_wraith.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2800 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_wyvern.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2379 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_xorn.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3300 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_young-black-dragon.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3231 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_young-blue-dragon.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3852 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_young-brass-dragon.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3905 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_young-bronze-dragon.json
+-rw-rw-r--   0 b         (1000) b         (1000)     4095 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_young-copper-dragon.json
+-rw-rw-r--   0 b         (1000) b         (1000)     4119 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_young-gold-dragon.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3463 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_young-green-dragon.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3153 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_young-red-dragon.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3968 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_young-silver-dragon.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3392 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_young-white-dragon.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1564 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_monsters_zombie.json
+-rw-rw-r--   0 b         (1000) b         (1000)      361 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_proficiencies_all-armor.json
+-rw-rw-r--   0 b         (1000) b         (1000)      259 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_proficiencies_clubs.json
+-rw-rw-r--   0 b         (1000) b         (1000)      399 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_proficiencies_crossbows-light.json
+-rw-rw-r--   0 b         (1000) b         (1000)      415 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_proficiencies_daggers.json
+-rw-rw-r--   0 b         (1000) b         (1000)      403 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_proficiencies_darts.json
+-rw-rw-r--   0 b         (1000) b         (1000)      377 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_proficiencies_hand-crossbows.json
+-rw-rw-r--   0 b         (1000) b         (1000)      308 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_proficiencies_herbalism-kit.json
+-rw-rw-r--   0 b         (1000) b         (1000)      277 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_proficiencies_javelins.json
+-rw-rw-r--   0 b         (1000) b         (1000)      724 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_proficiencies_light-armor.json
+-rw-rw-r--   0 b         (1000) b         (1000)      426 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_proficiencies_longswords.json
+-rw-rw-r--   0 b         (1000) b         (1000)      259 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_proficiencies_maces.json
+-rw-rw-r--   0 b         (1000) b         (1000)      558 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_proficiencies_martial-weapons.json
+-rw-rw-r--   0 b         (1000) b         (1000)      529 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_proficiencies_medium-armor.json
+-rw-rw-r--   0 b         (1000) b         (1000)      451 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_proficiencies_quarterstaffs.json
+-rw-rw-r--   0 b         (1000) b         (1000)      334 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_proficiencies_rapiers.json
+-rw-rw-r--   0 b         (1000) b         (1000)      586 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_proficiencies_saving-throw-cha.json
+-rw-rw-r--   0 b         (1000) b         (1000)      460 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_proficiencies_saving-throw-con.json
+-rw-rw-r--   0 b         (1000) b         (1000)      496 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_proficiencies_saving-throw-dex.json
+-rw-rw-r--   0 b         (1000) b         (1000)      436 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_proficiencies_saving-throw-int.json
+-rw-rw-r--   0 b         (1000) b         (1000)      517 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_proficiencies_saving-throw-str.json
+-rw-rw-r--   0 b         (1000) b         (1000)      583 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_proficiencies_saving-throw-wis.json
+-rw-rw-r--   0 b         (1000) b         (1000)      283 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_proficiencies_scimitars.json
+-rw-rw-r--   0 b         (1000) b         (1000)      629 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_proficiencies_shields.json
+-rw-rw-r--   0 b         (1000) b         (1000)      495 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_proficiencies_shortswords.json
+-rw-rw-r--   0 b         (1000) b         (1000)      271 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_proficiencies_sickles.json
+-rw-rw-r--   0 b         (1000) b         (1000)      885 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_proficiencies_simple-weapons.json
+-rw-rw-r--   0 b         (1000) b         (1000)      409 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_proficiencies_slings.json
+-rw-rw-r--   0 b         (1000) b         (1000)      265 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_proficiencies_spears.json
+-rw-rw-r--   0 b         (1000) b         (1000)      310 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_proficiencies_thieves-tools.json
+-rw-rw-r--   0 b         (1000) b         (1000)     8668 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_ability-checks.json
+-rw-rw-r--   0 b         (1000) b         (1000)      898 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_ability-scores-and-modifiers.json
+-rw-rw-r--   0 b         (1000) b         (1000)     5185 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_actions-in-combat.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2459 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_activating-an-item.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1844 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_advantage-and-disadvantage.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2341 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_attunement.json
+-rw-rw-r--   0 b         (1000) b         (1000)     6080 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_between-adventures.json
+-rw-rw-r--   0 b         (1000) b         (1000)    13605 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_casting-a-spell.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1449 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_cover.json
+-rw-rw-r--   0 b         (1000) b         (1000)    10998 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_damage-and-healing.json
+-rw-rw-r--   0 b         (1000) b         (1000)     5315 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_diseases.json
+-rw-rw-r--   0 b         (1000) b         (1000)    12813 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_fantasy-historical-pantheons.json
+-rw-rw-r--   0 b         (1000) b         (1000)     9411 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_madness.json
+-rw-rw-r--   0 b         (1000) b         (1000)     8932 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_making-an-attack.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2341 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_mounted-combat.json
+-rw-rw-r--   0 b         (1000) b         (1000)     6909 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_movement-and-position.json
+-rw-rw-r--   0 b         (1000) b         (1000)     6367 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_movement.json
+-rw-rw-r--   0 b         (1000) b         (1000)     4127 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_objects.json
+-rw-rw-r--   0 b         (1000) b         (1000)     6612 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_poisons.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1676 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_proficiency-bonus.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2112 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_resting.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1451 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_saving-throws.json
+-rw-rw-r--   0 b         (1000) b         (1000)     7309 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_sentient-magic-items.json
+-rw-rw-r--   0 b         (1000) b         (1000)      575 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_standard-exchange-rates.json
+-rw-rw-r--   0 b         (1000) b         (1000)     6567 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_the-environment.json
+-rw-rw-r--   0 b         (1000) b         (1000)     6297 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_the-order-of-combat.json
+-rw-rw-r--   0 b         (1000) b         (1000)     9702 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_the-planes-of-existence.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1118 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_time.json
+-rw-rw-r--   0 b         (1000) b         (1000)    17744 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_traps.json
+-rw-rw-r--   0 b         (1000) b         (1000)      989 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_underwater-combat.json
+-rw-rw-r--   0 b         (1000) b         (1000)    16317 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_using-each-ability.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2000 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_wearing-and-wielding-items.json
+-rw-rw-r--   0 b         (1000) b         (1000)     5515 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_what-is-a-spell.json
+-rw-rw-r--   0 b         (1000) b         (1000)      517 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_rules.json
+-rw-rw-r--   0 b         (1000) b         (1000)      796 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_rules_adventuring.json
+-rw-rw-r--   0 b         (1000) b         (1000)      379 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_rules_appendix.json
+-rw-rw-r--   0 b         (1000) b         (1000)      941 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_rules_combat.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2455 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_rules_equipment.json
+-rw-rw-r--   0 b         (1000) b         (1000)      659 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_rules_spellcasting.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2551 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_rules_using-ability-scores.json
+-rw-rw-r--   0 b         (1000) b         (1000)    27593 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1431 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_acid-arrow.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1216 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_acid-splash.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1073 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_aid.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1299 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_alarm.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2084 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_alter-self.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1197 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_animal-friendship.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1818 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_animal-messenger.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1746 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_animal-shapes.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2287 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_animate-dead.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3180 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_animate-objects.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1003 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_antilife-shell.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3331 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_antimagic-field.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3063 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_antipathy-sympathy.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1152 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_arcane-eye.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2968 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_arcane-hand.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1216 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_arcane-lock.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1244 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_arcane-sword.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1853 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_arcanists-magic-aura.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2992 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_astral-projection.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1474 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_augury.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1461 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_awaken.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1165 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_bane.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1887 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_banishment.json
+-rw-rw-r--   0 b         (1000) b         (1000)      898 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_barkskin.json
+-rw-rw-r--   0 b         (1000) b         (1000)      932 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_beacon-of-hope.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2173 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_bestow-curse.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1754 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_black-tentacles.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1440 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_blade-barrier.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1069 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_bless.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1785 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_blight.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1381 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_blindness-deafness.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1612 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_blink.json
+-rw-rw-r--   0 b         (1000) b         (1000)      922 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_blur.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1166 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_branding-smite.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1577 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_burning-hands.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2005 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_call-lightning.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1591 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_calm-emotions.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1545 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_chain-lightning.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1545 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_charm-person.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1440 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_chill-touch.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1433 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_circle-of-death.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1550 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_clairvoyance.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1615 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_clone.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1975 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_cloudkill.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1533 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_color-spray.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2077 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_command.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1486 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_commune-with-nature.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1327 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_commune.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1199 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_comprehend-languages.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1338 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_compulsion.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1490 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_cone-of-cold.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2119 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_confusion.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1689 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_conjure-animals.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1222 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_conjure-celestial.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2026 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_conjure-elemental.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1683 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_conjure-fey.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1642 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_conjure-minor-elementals.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1698 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_conjure-woodland-beings.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1680 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_contact-other-plane.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2588 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_contagion.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1596 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_contingency.json
+-rw-rw-r--   0 b         (1000) b         (1000)      929 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_continual-flame.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3934 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_control-water.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2060 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_control-weather.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1161 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_counterspell.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1048 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_create-food-and-water.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1354 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_create-or-destroy-water.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2380 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_create-undead.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1609 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_creation.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1330 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_cure-wounds.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1290 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_dancing-lights.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1521 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_darkness.json
+-rw-rw-r--   0 b         (1000) b         (1000)      950 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_darkvision.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1477 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_daylight.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1016 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_death-ward.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2241 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_delayed-blast-fireball.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1323 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_demiplane.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1118 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_detect-evil-and-good.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1409 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_detect-magic.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1223 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_detect-poison-and-disease.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2653 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_detect-thoughts.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1613 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_dimension-door.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1665 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_disguise-self.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1941 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_disintegrate.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1874 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_dispel-evil-and-good.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1540 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_dispel-magic.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1326 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_divination.json
+-rw-rw-r--   0 b         (1000) b         (1000)      811 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_divine-favor.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1455 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_divine-word.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2032 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_dominate-beast.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2249 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_dominate-monster.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2430 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_dominate-person.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2862 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_dream.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1192 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_druidcraft.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2830 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_earthquake.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1166 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_eldritch-blast.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1721 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_enhance-ability.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2272 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_enlarge-reduce.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1213 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_entangle.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1266 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_enthrall.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2356 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_etherealness.json
+-rw-rw-r--   0 b         (1000) b         (1000)      896 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_expeditious-retreat.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2680 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_eyebite.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1442 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_fabricate.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1147 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_faerie-fire.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1522 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_faithful-hound.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1093 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_false-life.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1595 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_fear.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1001 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_feather-fall.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1809 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_feeblemind.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2542 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_find-familiar.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1962 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_find-steed.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1440 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_find-the-path.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1325 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_find-traps.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1320 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_finger-of-death.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1089 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_fire-bolt.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1351 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_fire-shield.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1476 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_fire-storm.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1669 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_fireball.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1315 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_flame-blade.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1521 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_flame-strike.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1841 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_flaming-sphere.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1789 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_flesh-to-stone.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1494 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_floating-disk.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1032 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_fly.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1189 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_fog-cloud.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1844 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_forbiddance.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1933 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_forcecage.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1086 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_foresight.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1374 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_freedom-of-movement.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2193 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_freezing-sphere.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1772 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_gaseous-form.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1830 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_gate.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1845 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_geas.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1054 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_gentle-repose.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1258 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_giant-insect.json
+-rw-rw-r--   0 b         (1000) b         (1000)      752 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_glibness.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1340 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_globe-of-invulnerability.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3823 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_glyph-of-warding.json
+-rw-rw-r--   0 b         (1000) b         (1000)      930 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_goodberry.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1093 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_grease.json
+-rw-rw-r--   0 b         (1000) b         (1000)      853 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_greater-invisibility.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1125 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_greater-restoration.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1429 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_guardian-of-faith.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3195 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_guards-and-wards.json
+-rw-rw-r--   0 b         (1000) b         (1000)      816 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_guidance.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1254 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_guiding-bolt.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1615 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_gust-of-wind.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3273 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_hallow.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1757 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_hallucinatory-terrain.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1227 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_harm.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1198 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_haste.json
+-rw-rw-r--   0 b         (1000) b         (1000)      988 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_heal.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1152 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_healing-word.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1809 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_heat-metal.json
+-rw-rw-r--   0 b         (1000) b         (1000)      959 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_hellish-rebuke.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1233 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_heroes-feast.json
+-rw-rw-r--   0 b         (1000) b         (1000)      904 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_heroism.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1362 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_hideous-laughter.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1356 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_hold-monster.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1576 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_hold-person.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1232 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_holy-aura.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1227 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_hunters-mark.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1550 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_hypnotic-pattern.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1688 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_ice-storm.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1168 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_identify.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1493 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_illusory-script.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3954 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_imprisonment.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1580 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_incendiary-cloud.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1052 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_inflict-wounds.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1814 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_insect-plague.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1369 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_instant-summons.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1210 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_invisibility.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1140 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_irresistible-dance.json
+-rw-rw-r--   0 b         (1000) b         (1000)      852 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_jump.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1313 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_knock.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1612 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_legend-lore.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1112 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_lesser-restoration.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1542 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_levitate.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1359 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_light.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1623 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_lightning-bolt.json
+-rw-rw-r--   0 b         (1000) b         (1000)      977 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_locate-animals-or-plants.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1655 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_locate-creature.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1537 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_locate-object.json
+-rw-rw-r--   0 b         (1000) b         (1000)      989 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_longstrider.json
+-rw-rw-r--   0 b         (1000) b         (1000)      901 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_mage-armor.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1321 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_mage-hand.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2262 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_magic-circle.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3172 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_magic-jar.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1273 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_magic-missile.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1952 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_magic-mouth.json
+-rw-rw-r--   0 b         (1000) b         (1000)      928 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_magic-weapon.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2286 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_magnificent-mansion.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2350 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_major-image.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1259 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_mass-cure-wounds.json
+-rw-rw-r--   0 b         (1000) b         (1000)      853 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_mass-heal.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1048 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_mass-healing-word.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2342 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_mass-suggestion.json
+-rw-rw-r--   0 b         (1000) b         (1000)      947 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_maze.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1739 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_meld-into-stone.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1200 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_mending.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1232 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_message.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1385 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_meteor-swarm.json
+-rw-rw-r--   0 b         (1000) b         (1000)      857 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_mind-blank.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1850 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_minor-illusion.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1782 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_mirage-arcane.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1822 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_mirror-image.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1144 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_mislead.json
+-rw-rw-r--   0 b         (1000) b         (1000)      846 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_misty-step.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2692 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_modify-memory.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1899 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_moonbeam.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1939 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_move-earth.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1042 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_nondetection.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1122 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_pass-without-trace.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1097 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_passwall.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1309 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_phantasmal-killer.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1243 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_phantom-steed.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2712 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_planar-ally.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2312 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_planar-binding.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2446 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_plane-shift.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1463 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_plant-growth.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1229 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_poison-spray.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2151 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_polymorph.json
+-rw-rw-r--   0 b         (1000) b         (1000)      886 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_power-word-kill.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1043 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_power-word-stun.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1029 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_prayer-of-healing.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1669 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_prestidigitation.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2651 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_prismatic-spray.json
+-rw-rw-r--   0 b         (1000) b         (1000)     4369 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_prismatic-wall.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1823 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_private-sanctum.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1393 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_produce-flame.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2110 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_programmed-illusion.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1811 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_project-image.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1045 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_protection-from-energy.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1473 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_protection-from-evil-and-good.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1087 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_protection-from-poison.json
+-rw-rw-r--   0 b         (1000) b         (1000)      868 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_purify-food-and-drink.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1758 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_raise-dead.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1136 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_ray-of-enfeeblement.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1146 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_ray-of-frost.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1143 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_regenerate.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1727 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_reincarnate.json
+-rw-rw-r--   0 b         (1000) b         (1000)      959 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_remove-curse.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1657 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_resilient-sphere.json
+-rw-rw-r--   0 b         (1000) b         (1000)      859 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_resistance.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1646 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_resurrection.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1708 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_reverse-gravity.json
+-rw-rw-r--   0 b         (1000) b         (1000)      948 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_revivify.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1390 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_rope-trick.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1151 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_sacred-flame.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1132 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_sanctuary.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1143 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_scorching-ray.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2393 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_scrying.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1548 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_secret-chest.json
+-rw-rw-r--   0 b         (1000) b         (1000)      939 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_see-invisibility.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1909 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_seeming.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1241 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_sending.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1313 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_sequester.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3021 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_shapechange.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1805 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_shatter.json
+-rw-rw-r--   0 b         (1000) b         (1000)      828 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_shield-of-faith.json
+-rw-rw-r--   0 b         (1000) b         (1000)      794 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_shield.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1001 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_shillelagh.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1261 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_shocking-grasp.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1102 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_silence.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1714 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_silent-image.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1949 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_simulacrum.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1764 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_sleep.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1491 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_sleet-storm.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1832 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_slow.json
+-rw-rw-r--   0 b         (1000) b         (1000)      607 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_spare-the-dying.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1100 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_speak-with-animals.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1472 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_speak-with-dead.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1837 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_speak-with-plants.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1051 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_spider-climb.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1340 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_spike-growth.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1416 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_spirit-guardians.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1712 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_spiritual-weapon.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1815 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_stinking-cloud.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1272 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_stone-shape.json
+-rw-rw-r--   0 b         (1000) b         (1000)      987 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_stoneskin.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2476 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_storm-of-vengeance.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2060 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_suggestion.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1712 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_sunbeam.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1632 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_sunburst.json
+-rw-rw-r--   0 b         (1000) b         (1000)     4345 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_symbol.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2353 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_telekinesis.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1021 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_telepathic-bond.json
+-rw-rw-r--   0 b         (1000) b         (1000)     4184 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_teleport.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2024 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_teleportation-circle.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1342 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_thaumaturgy.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1775 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_thunderwave.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1051 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_time-stop.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1509 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_tiny-hut.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1065 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_tongues.json
+-rw-rw-r--   0 b         (1000) b         (1000)      846 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_transport-via-plants.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1337 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_tree-stride.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3331 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_true-polymorph.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1271 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_true-resurrection.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1126 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_true-seeing.json
+-rw-rw-r--   0 b         (1000) b         (1000)      986 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_true-strike.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1628 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_unseen-servant.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1349 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_vampiric-touch.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1199 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_vicious-mockery.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1962 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_wall-of-fire.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1464 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_wall-of-force.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2182 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_wall-of-ice.json
+-rw-rw-r--   0 b         (1000) b         (1000)     2363 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_wall-of-stone.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1931 2022-09-20 01:54:47.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_wall-of-thorns.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1206 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_warding-bond.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1080 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_water-breathing.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1295 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_water-walk.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1762 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_web.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1205 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_weird.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1287 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_wind-walk.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1906 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_wind-wall.json
+-rw-rw-r--   0 b         (1000) b         (1000)     3433 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_wish.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1139 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_word-of-recall.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1472 2023-06-29 01:34:15.000000 dnd_character-23.7.29/dnd_character/json_cache/api_spells_zone-of-truth.json
+-rw-rw-r--   0 b         (1000) b         (1000)     1505 2023-07-29 21:20:33.000000 dnd_character-23.7.29/dnd_character/monsters.py
+-rw-rw-r--   0 b         (1000) b         (1000)     1710 2023-07-29 21:20:09.000000 dnd_character-23.7.29/dnd_character/spellcasting.py
+drwxrwxr-x   0 b         (1000) b         (1000)        0 2023-07-30 01:48:19.704028 dnd_character-23.7.29/dnd_character.egg-info/
+-rw-rw-r--   0 b         (1000) b         (1000)     7121 2023-07-30 01:48:19.000000 dnd_character-23.7.29/dnd_character.egg-info/PKG-INFO
+-rw-rw-r--   0 b         (1000) b         (1000)    70285 2023-07-30 01:48:19.000000 dnd_character-23.7.29/dnd_character.egg-info/SOURCES.txt
+-rw-rw-r--   0 b         (1000) b         (1000)        1 2023-07-30 01:48:19.000000 dnd_character-23.7.29/dnd_character.egg-info/dependency_links.txt
+-rw-rw-r--   0 b         (1000) b         (1000)       14 2023-07-30 01:48:19.000000 dnd_character-23.7.29/dnd_character.egg-info/top_level.txt
+-rw-rw-r--   0 b         (1000) b         (1000)       38 2023-07-30 01:48:19.832039 dnd_character-23.7.29/setup.cfg
+-rw-rw-r--   0 b         (1000) b         (1000)     1239 2023-07-29 02:30:02.000000 dnd_character-23.7.29/setup.py
```

### Comparing `dnd_character-23.7.22/LICENSE` & `dnd_character-23.7.29/LICENSE`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/PKG-INFO` & `dnd_character-23.7.29/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,133 +1,172 @@
 Metadata-Version: 2.1
 Name: dnd_character
-Version: 23.7.22
+Version: 23.7.29
 Summary: make Dungeons & Dragons characters as serializable objects
 Home-page: https://github.com/tassaron/dnd-character
 Author: Brianna Rainey
 License: EPL-2.0
 Keywords: dnd trpg tabletop rpg
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Games/Entertainment
 Classifier: Topic :: Games/Entertainment :: Role-Playing
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Eclipse Public License 2.0 (EPL-2.0)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # dnd-character
+
 A Python library to make 5e Dungeons & Dragons characters for use in another app. Characters are serializable into Python dicts so they can be saved and loaded however you wish.
 
 SRD rules are fetched from the [5e SRD API](https://github.com/5e-bits/5e-srd-api) the first time they're requested, then the JSON is cached locally for faster retrieval in the future. I've included the `json_cache` containing the SRD inside the repo in case this API changes, but when the API does change I will update this library. So please pin your version if you want to avoid any breaking changes.
 
 You can use this library as a CLI tool to generate character sheets from the terminal; see `python -m dnd_character --help` for details.
 
-
 ## Installation and Use
+
 1. Install from PyPI using `pip install dnd-character`
 1. See `example.py` for example code on how to use the library.
 1. Generate random character sheet text file with `python -m dnd_character --random > mycharactername.txt`
 
-
 ## Licenses
-The software is EPL-2.0 and the text for this license is in `LICENSE` as is standard for software. Originally forked from [PyDnD](https://github.com/Coffee-fueled-deadlines/PyDnD). The contents of `dnd_character/json_cache` are retrieved from [5e-srd-api](https://github.com/5e-bits/5e-srd-api), and are covered by the Open Game License. See `dnd_character/json_cache/OGLv1.0a.txt` for details.
 
+The software is EPL-2.0 and the text for this license is in `LICENSE` as is standard for software. Originally forked from [PyDnD](https://github.com/Coffee-fueled-deadlines/PyDnD). The contents of `dnd_character/json_cache` are retrieved from [5e-srd-api](https://github.com/5e-bits/5e-srd-api), and are covered by the Open Game License. See `dnd_character/json_cache/OGLv1.0a.txt` for details.
 
 ## Example Code
 
 ### Creating Characters and Monsters
-The `classes` module has functions for creating all 12 classes from the System Reference Document. The `monsters` module has a dictionary of monsters, which are dictionaries themselves.
-```
+
+The `classes` module has functions for creating all 12 classes from the System Reference Document. The `monsters` module has a factory function for creating monsters.
+
+```python
 from dnd_character.classes import Bard
-from dnd_character.monsters import SRD_monsters
+from dnd_character.monsters import Monster
 from random import randint
 
 brianna = Bard(
     name="Brianna",
     level=10,
     )
-zombie = SRD_monsters["zombie"]
-attack_bonus = zombie["actions"][0]["attack_bonus"]
+zombie = Monster("zombie")
+attack_bonus = zombie.actions[0]["attack_bonus"]
 # Zombie rolls a d20 to attack a Bard
 if randint(1, 20) + attack_bonus >= brianna.armor_class:
-    print(f"{brianna.name} was hit by {zombie['name']}!")
+    print(f"{brianna.name} was hit by {zombie.name}!")
 else:
     print(f"{brianna.name} bravely dodged the attack")
 ```
 
 ### Leveling and Experience
+
 The library should help leveling up characters automatically if you manage the Character's `experience` attribute. It's simpler to avoid modifying the level directly.
-```
-import dnd_character
+
+```python
+from dnd_character import Character
 thor = Character(name="Thor")
 assert thor.level == 1
 thor.experience += 1000
 assert thor.level == 3
 assert thor.experience.to_next_level == 1700
 thor.experience += thor.experience.to_next_level
 assert thor.level == 4
 ```
 
 ### Starting Equipment
+
 Characters initialized with a class will have the starting equipment of that class, and an attribute called `player_options` which lists the optional starting equipment.
-```
+
+```python
 from dnd_character.classes import Paladin
+from dnd_character.equipment import Item
 from pprint import pprint
 sturm = Paladin(dexterity=10)
 pprint(sturm.inventory)
 print(sturm.armor_class)
 # Remove Chain Mail
-sturm.removeItem(sturm.inventory[0])
+sturm.remove_item(sturm.inventory[0])
 print(sturm.armor_class)
 # New Item
-from dnd_character.equipment import SRD_equipment
-dragonlance = SRD_equipment['lance']
-dragonlance["name"] = "Dragonlance®"
-sturm.giveItem(dragonlance)
+dragonlance = Item('lance')
+dragonlance.name = "Dragonlance®"
+sturm.give_item(dragonlance)
 # View optional starting equipment
 pprint(sturm.player_options)
 ```
 
-
 ### Using Spells
-Support for spells is not super great at the moment. Characters have dictionaries like `spells_known` and `cantrips_known` in which you're expected to store dictionaries from `SRD_spells`... but there's no useful help from the library here. Yet!
-```
-from dnd_character.spellcasting import SRD_spells, spells_for_class_level
-from pprint import pprint
+
+Spells are represented by _SPELL objects from `dnd_character.spellcasting`. The best way to find spells is using the `spells_for_class_level` function.
+
+```python
+from dnd_character.spellcasting import spells_for_class_level
 cantrips = spells_for_class_level('wizard', 0)
-print(f"Cantrips available to a Wizard: {', '.join(cantrips)}")
+print(f"Cantrips available to a Wizard:")
 for spell in cantrips:
-    print(f"{SRD_spells[spell]['name']}:")
-    pprint(SRD_spells[spell])
-    break
+    print(spell)
 ```
 
+Characters have lists to store _SPELL objects:
+
+- `spells_prepared`
+- `spells_known`
+- `cantrips_known`
+
+Characters have a `spell_slots` dictionary which shows the **total** spell slots. Depletion and rest mechanics are planned for a future version.
+
+```python
+from dnd_character import Wizard
+from dnd_character.spellcasting import SPELLS
+# Create wizard and teach Identify, a level 1 spell
+my_wizard = Wizard(name="Gormwinkle")
+my_wizard.spells_prepared.append(SPELLS["identify"])
+# Get total spell slots
+spell_slots_level_1 = my_wizard.spell_slots["spell_slots_level_1"]
+print(f"{my_wizard.name} has {spell_slots_level_1} spell slots of 1st level")
+# Cast until wizard runs out of spell slots
+while spell_slots_level_1 > 0:
+    print(f"Casting {SPELLS['identify'].name}!")
+    spell_slots_level_1 -= 1
+```
+
+There is currently no way to manage wizard spellbooks or class-specific features such as the Wizard's arcane recovery or the Sorcerer's metamagic.
 
 ## Character Object
+
 Normal initialization arguments for a Character object:
-```
+
+```text
 name         (str)
 age          (str)
 gender       (str)
-alignment    (str): character's two letter alignment
-description  (str): physical description of player character
-biography    (str): backstory of player character	
 level        (int): starting level
-wealth       (int): starting wealth	
-strength     (int)
-dexterity    (int)
-constitution (int)
-wisdom       (int)
-intelligence (int)
-charisma     (int)
-hp           (int):
-classs      (dict): JSON returned from the 5e API -- dnd_character.SRD.SRD_classes["bard"]
+hp           (int)
+alignment    (str): character's two letter alignment (LE, CG, TN, etc.)
+description  (str): physical description of player character
+background   (str): one-word backstory (e.g., knight, chef, acolyte)
+wealth       (int): if None, roll 4d10 for starting gp (gold pieces)
+strength     (int): if None, roll 4d6 and drop the lowest
+dexterity    (int): if None, roll 4d6 and drop the lowest
+constitution (int): if None, roll 4d6 and drop the lowest
+wisdom       (int): if None, roll 4d6 and drop the lowest
+intelligence (int): if None, roll 4d6 and drop the lowest
+charisma     (int): if None, roll 4d6 and drop the lowest
+classs    (_CLASS): a D&D class object (e.g., CLASSES['bard'])
 ```
+
 In addition, the Character object can receive attributes that are normally set automatically, such as the UUID. This is for re-loading the objects from serialized data (via `Character(**characterData)`) and probably aren't arguments you would write manually into your code.
 
+## Serializing objects
+
+All objects in this library can be turned into Python dicts, which can then be turned back into objects. This means characters (along with their items and spells), and monsters as well.
+
+- `dict(object)` creates a serializable dict that could be reloaded from text (e.g., suitable for conversion to and from JSON)
+- `repr(object)` prints a string that would re-construct the Python object if pasted into a REPL
+- `str(object)` is not for serialization. It creates a "user-friendly" string
 
 ## Contributing
-Please feel free to open a Pull Request on GitHub! I would be happy to help merge any contributions no matter your skill level.
+
+I greatly appreciate feedback about desired features and information about how you're using this library. Please feel free to open an issue or pull request on GitHub! I would be happy to help merge any contributions no matter your skill level.
```

### Comparing `dnd_character-23.7.22/README.md` & `dnd_character-23.7.29/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,113 +1,152 @@
 # dnd-character
+
 A Python library to make 5e Dungeons & Dragons characters for use in another app. Characters are serializable into Python dicts so they can be saved and loaded however you wish.
 
 SRD rules are fetched from the [5e SRD API](https://github.com/5e-bits/5e-srd-api) the first time they're requested, then the JSON is cached locally for faster retrieval in the future. I've included the `json_cache` containing the SRD inside the repo in case this API changes, but when the API does change I will update this library. So please pin your version if you want to avoid any breaking changes.
 
 You can use this library as a CLI tool to generate character sheets from the terminal; see `python -m dnd_character --help` for details.
 
-
 ## Installation and Use
+
 1. Install from PyPI using `pip install dnd-character`
 1. See `example.py` for example code on how to use the library.
 1. Generate random character sheet text file with `python -m dnd_character --random > mycharactername.txt`
 
-
 ## Licenses
-The software is EPL-2.0 and the text for this license is in `LICENSE` as is standard for software. Originally forked from [PyDnD](https://github.com/Coffee-fueled-deadlines/PyDnD). The contents of `dnd_character/json_cache` are retrieved from [5e-srd-api](https://github.com/5e-bits/5e-srd-api), and are covered by the Open Game License. See `dnd_character/json_cache/OGLv1.0a.txt` for details.
 
+The software is EPL-2.0 and the text for this license is in `LICENSE` as is standard for software. Originally forked from [PyDnD](https://github.com/Coffee-fueled-deadlines/PyDnD). The contents of `dnd_character/json_cache` are retrieved from [5e-srd-api](https://github.com/5e-bits/5e-srd-api), and are covered by the Open Game License. See `dnd_character/json_cache/OGLv1.0a.txt` for details.
 
 ## Example Code
 
 ### Creating Characters and Monsters
-The `classes` module has functions for creating all 12 classes from the System Reference Document. The `monsters` module has a dictionary of monsters, which are dictionaries themselves.
-```
+
+The `classes` module has functions for creating all 12 classes from the System Reference Document. The `monsters` module has a factory function for creating monsters.
+
+```python
 from dnd_character.classes import Bard
-from dnd_character.monsters import SRD_monsters
+from dnd_character.monsters import Monster
 from random import randint
 
 brianna = Bard(
     name="Brianna",
     level=10,
     )
-zombie = SRD_monsters["zombie"]
-attack_bonus = zombie["actions"][0]["attack_bonus"]
+zombie = Monster("zombie")
+attack_bonus = zombie.actions[0]["attack_bonus"]
 # Zombie rolls a d20 to attack a Bard
 if randint(1, 20) + attack_bonus >= brianna.armor_class:
-    print(f"{brianna.name} was hit by {zombie['name']}!")
+    print(f"{brianna.name} was hit by {zombie.name}!")
 else:
     print(f"{brianna.name} bravely dodged the attack")
 ```
 
 ### Leveling and Experience
+
 The library should help leveling up characters automatically if you manage the Character's `experience` attribute. It's simpler to avoid modifying the level directly.
-```
-import dnd_character
+
+```python
+from dnd_character import Character
 thor = Character(name="Thor")
 assert thor.level == 1
 thor.experience += 1000
 assert thor.level == 3
 assert thor.experience.to_next_level == 1700
 thor.experience += thor.experience.to_next_level
 assert thor.level == 4
 ```
 
 ### Starting Equipment
+
 Characters initialized with a class will have the starting equipment of that class, and an attribute called `player_options` which lists the optional starting equipment.
-```
+
+```python
 from dnd_character.classes import Paladin
+from dnd_character.equipment import Item
 from pprint import pprint
 sturm = Paladin(dexterity=10)
 pprint(sturm.inventory)
 print(sturm.armor_class)
 # Remove Chain Mail
-sturm.removeItem(sturm.inventory[0])
+sturm.remove_item(sturm.inventory[0])
 print(sturm.armor_class)
 # New Item
-from dnd_character.equipment import SRD_equipment
-dragonlance = SRD_equipment['lance']
-dragonlance["name"] = "Dragonlance®"
-sturm.giveItem(dragonlance)
+dragonlance = Item('lance')
+dragonlance.name = "Dragonlance®"
+sturm.give_item(dragonlance)
 # View optional starting equipment
 pprint(sturm.player_options)
 ```
 
-
 ### Using Spells
-Support for spells is not super great at the moment. Characters have dictionaries like `spells_known` and `cantrips_known` in which you're expected to store dictionaries from `SRD_spells`... but there's no useful help from the library here. Yet!
-```
-from dnd_character.spellcasting import SRD_spells, spells_for_class_level
-from pprint import pprint
+
+Spells are represented by _SPELL objects from `dnd_character.spellcasting`. The best way to find spells is using the `spells_for_class_level` function.
+
+```python
+from dnd_character.spellcasting import spells_for_class_level
 cantrips = spells_for_class_level('wizard', 0)
-print(f"Cantrips available to a Wizard: {', '.join(cantrips)}")
+print(f"Cantrips available to a Wizard:")
 for spell in cantrips:
-    print(f"{SRD_spells[spell]['name']}:")
-    pprint(SRD_spells[spell])
-    break
+    print(spell)
 ```
 
+Characters have lists to store _SPELL objects:
+
+- `spells_prepared`
+- `spells_known`
+- `cantrips_known`
+
+Characters have a `spell_slots` dictionary which shows the **total** spell slots. Depletion and rest mechanics are planned for a future version.
+
+```python
+from dnd_character import Wizard
+from dnd_character.spellcasting import SPELLS
+# Create wizard and teach Identify, a level 1 spell
+my_wizard = Wizard(name="Gormwinkle")
+my_wizard.spells_prepared.append(SPELLS["identify"])
+# Get total spell slots
+spell_slots_level_1 = my_wizard.spell_slots["spell_slots_level_1"]
+print(f"{my_wizard.name} has {spell_slots_level_1} spell slots of 1st level")
+# Cast until wizard runs out of spell slots
+while spell_slots_level_1 > 0:
+    print(f"Casting {SPELLS['identify'].name}!")
+    spell_slots_level_1 -= 1
+```
+
+There is currently no way to manage wizard spellbooks or class-specific features such as the Wizard's arcane recovery or the Sorcerer's metamagic.
 
 ## Character Object
+
 Normal initialization arguments for a Character object:
-```
+
+```text
 name         (str)
 age          (str)
 gender       (str)
-alignment    (str): character's two letter alignment
-description  (str): physical description of player character
-biography    (str): backstory of player character	
 level        (int): starting level
-wealth       (int): starting wealth	
-strength     (int)
-dexterity    (int)
-constitution (int)
-wisdom       (int)
-intelligence (int)
-charisma     (int)
-hp           (int):
-classs      (dict): JSON returned from the 5e API -- dnd_character.SRD.SRD_classes["bard"]
+hp           (int)
+alignment    (str): character's two letter alignment (LE, CG, TN, etc.)
+description  (str): physical description of player character
+background   (str): one-word backstory (e.g., knight, chef, acolyte)
+wealth       (int): if None, roll 4d10 for starting gp (gold pieces)
+strength     (int): if None, roll 4d6 and drop the lowest
+dexterity    (int): if None, roll 4d6 and drop the lowest
+constitution (int): if None, roll 4d6 and drop the lowest
+wisdom       (int): if None, roll 4d6 and drop the lowest
+intelligence (int): if None, roll 4d6 and drop the lowest
+charisma     (int): if None, roll 4d6 and drop the lowest
+classs    (_CLASS): a D&D class object (e.g., CLASSES['bard'])
 ```
+
 In addition, the Character object can receive attributes that are normally set automatically, such as the UUID. This is for re-loading the objects from serialized data (via `Character(**characterData)`) and probably aren't arguments you would write manually into your code.
 
+## Serializing objects
+
+All objects in this library can be turned into Python dicts, which can then be turned back into objects. This means characters (along with their items and spells), and monsters as well.
+
+- `dict(object)` creates a serializable dict that could be reloaded from text (e.g., suitable for conversion to and from JSON)
+- `repr(object)` prints a string that would re-construct the Python object if pasted into a REPL
+- `str(object)` is not for serialization. It creates a "user-friendly" string
 
 ## Contributing
-Please feel free to open a Pull Request on GitHub! I would be happy to help merge any contributions no matter your skill level.
+
+I greatly appreciate feedback about desired features and information about how you're using this library. Please feel free to open an issue or pull request on GitHub! I would be happy to help merge any contributions no matter your skill level.
```

### Comparing `dnd_character-23.7.22/dnd_character/__init__.py` & `dnd_character-23.7.29/dnd_character/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,12 +3,12 @@
 into external applications. The character data is serializable so it
 can be stored as json or a Python dict.
 """
 from .character import Character  # noqa: F401, F405 (ignore unused import)
 from .classes import *  # noqa: F401, F403 (ignore star import)
 
 __author__ = "Brianna Rainey"
-__copyright__ = "Copyright 2019-2023 Brianna Rainey & Markis Cook"
-__credits__ = ["Brianna Rainey (Current Programmer)", "Markis Cook (Original Creator)"]
+__copyright__ = "Copyright 2023 Brianna Rainey"
+__credits__ = ["Brianna Rainey", "Gergő", "Markis Cook", "Tim Van Rillaer"]
 __license__ = "EPL-2.0"
-__version__ = "23.07.22"
+__version__ = "23.07.29"
 __maintainer__ = "Brianna Rainey"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dnd_character-23.7.22/dnd_character/__main__.py` & `dnd_character-23.7.29/dnd_character/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pprint import pprint
 from dnd_character.character import Character
 from dnd_character.classes import CLASSES
 
 CLASS_NAMES = list(CLASSES.keys())
 
 
-def main():
+def main() -> None:
     parser = argparse.ArgumentParser(
         prog="dnd-character",
         description="generate D&D 5e character sheet from terminal",
     )
     actions = parser.add_mutually_exclusive_group()
     actions.add_argument(
         "-r",
```

### Comparing `dnd_character-23.7.22/dnd_character/character.py` & `dnd_character-23.7.29/dnd_character/character.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,109 +1,120 @@
-from typing import Optional, Union
+from typing import Optional, Union, Iterator, TYPE_CHECKING
 from uuid import uuid4, UUID
-import math
 import logging
 
+if TYPE_CHECKING:
+    from .classes import _CLASS
+    from .spellcasting import _SPELL
+
 from .SRD import SRD, SRD_class_levels
+from .equipment import _Item, Item
 from .experience import Experience, experience_at_level, level_at_experience
 from .dice import sum_rolls
 
 
 LOG = logging.getLogger(__package__)
 
+coin_value = {"pp": 10, "gp": 1, "ep": 0.5, "sp": 0.1, "cp": 0.01}
+
+
+class InvalidParameterError(Exception):
+    pass
+
 
 class Character:
     """
     Character Object deals with all aspects of the player character including
     name, age, gender, description, biography, level, wealth, and all
     player ability scores.  All can be omitted to create a blank, level 1
     player.
     """
 
     def __init__(
         self,
         *,  # This * forces the caller to use keyword arguments
-        uid: UUID = None,
-        name: str = None,
-        age: str = None,
-        gender: str = None,
-        species: str = None,
-        speed: int = None,
-        alignment: str = None,
-        description: str = None,
-        background: str = None,
-        personality: str = None,
-        ideals: str = None,
-        bonds: str = None,
-        flaws: str = None,
-        classs: dict = None,
-        class_name: str = None,
-        class_index: str = None,
-        class_levels: list = None,
-        level: Union[int, None] = None,
+        uid: Optional[Union[UUID, str]] = None,
+        classs: Optional["_CLASS"] = None,
+        class_name: Optional[str] = None,
+        class_index: Optional[str] = None,
+        name: Optional[str] = None,
+        age: Optional[str] = None,
+        gender: Optional[str] = None,
+        species: Optional[str] = None,
+        speed: Optional[int] = None,
+        alignment: Optional[str] = None,
+        description: Optional[str] = None,
+        background: Optional[str] = None,
+        personality: Optional[str] = None,
+        ideals: Optional[str] = None,
+        bonds: Optional[str] = None,
+        flaws: Optional[str] = None,
+        level: Optional[int] = None,
         experience: Union[int, None, Experience] = None,
-        wealth: int = 0,
-        strength: int = None,
-        dexterity: int = None,
-        constitution: int = None,
-        wisdom: int = None,
-        intelligence: int = None,
-        charisma: int = None,
-        max_hp: int = None,
-        current_hp: int = None,
-        temp_hp: int = None,
+        wealth: Optional[Union[int, float]] = None,
+        wealth_detailed: Optional[dict] = None,
+        strength: Optional[int] = None,
+        dexterity: Optional[int] = None,
+        constitution: Optional[int] = None,
+        wisdom: Optional[int] = None,
+        intelligence: Optional[int] = None,
+        charisma: Optional[int] = None,
+        max_hp: Optional[int] = None,
+        current_hp: Optional[int] = None,
+        temp_hp: Optional[int] = None,
         hd: int = 8,
-        max_hd: int = None,
-        current_hd: int = None,
-        proficiencies: dict = None,
-        saving_throws: list = None,
-        cantrips_known: dict = None,
-        spells_known: dict = None,
-        spells_prepared: list = None,
-        spell_slots: dict = None,
-        skills_strength: dict = None,
-        skills_dexterity: dict = None,
-        skills_wisdom: dict = None,
-        skills_intelligence: dict = None,
-        skills_charisma: dict = None,
-        inventory: list = None,
+        max_hd: Optional[int] = None,
+        current_hd: Optional[int] = None,
+        proficiencies: Optional[dict] = None,
+        saving_throws: Optional[list] = None,
+        cantrips_known: Optional[list["_SPELL"]] = None,
+        spells_known: Optional[list["_SPELL"]] = None,
+        spells_prepared: Optional[list["_SPELL"]] = None,
+        spell_slots: Optional[dict[str, int]] = None,
+        skills_strength: Optional[dict] = None,
+        skills_dexterity: Optional[dict] = None,
+        skills_wisdom: Optional[dict] = None,
+        skills_intelligence: Optional[dict] = None,
+        skills_charisma: Optional[dict] = None,
+        inventory: Optional[list[dict]] = None,
         prof_bonus: int = 0,
         ability_score_bonus: int = 0,
-        class_features: dict = None,
-        class_spellcasting: dict = None,
-        class_features_enabled: list = None,
-        spellcasting_stat: str = None,
-        player_options: dict = None,
-        armor_class: int = None,
+        class_features: Optional[dict] = None,
+        class_features_enabled: Optional[list] = None,
+        spellcasting_stat: Optional[str] = None,
+        player_options: Optional[dict] = None,
+        armor_class: Optional[int] = None,
         death_saves: int = 0,
         death_fails: int = 0,
         exhaustion: int = 0,
         dead: bool = False,
-        conditions: dict = None,
+        conditions: Optional[dict] = None,
     ):
         """
         Typical Arguments:
                 name         (str)
                 age          (str)
                 gender       (str)
                 alignment    (str): two letter alignment (LE, TN, CN, LG, etc.)
                 description  (str): physical description of character
-                biography    (str): backstory of character
+                background   (str): one-word backstory of character (e.g. knight, chef)
                 level        (int): character's starting level
                 wealth       (int): character's starting wealth
                 strength     (int): character's starting strength
                 dexterity    (int):  character's starting dexterity
                 constitution (int):  character's starting constitution
                 wisdom       (int):  character's starting wisdom
                 intelligence (int):  character's starting intelligence
                 charisma     (int):  character's starting charisma
         """
 
         # Decorative attrs that don't affect program logic
-        self.uid = UUID(uid) if uid is not None else uuid4()
+        self.uid: UUID = (
+            uuid4() if uid is None else uid if isinstance(uid, UUID) else UUID(uid)
+        )
         self.name = name
         self.age = age
         self.gender = gender
         self.description = description
         self.background = background
         self.personality = personality
         self.ideals = ideals
@@ -129,72 +140,76 @@
         )
         self.prof_bonus = prof_bonus
         self.ability_score_bonus = ability_score_bonus
         self.class_features = class_features if class_features is not None else {}
         self.class_features_enabled = (
             class_features_enabled if class_features_enabled is not None else []
         )
-        self.class_spellcasting = (
-            class_spellcasting if class_spellcasting is not None else {}
-        )
 
         # Ability Scores
-        self.strength = self.setInitialAbilityScore(strength)
-        self._dexterity = self.setInitialAbilityScore(dexterity)
-        self.constitution = self.setInitialAbilityScore(constitution)
-        self.wisdom = self.setInitialAbilityScore(wisdom)
-        self.intelligence = self.setInitialAbilityScore(intelligence)
-        self.charisma = self.setInitialAbilityScore(charisma)
+        self.strength = self.set_initial_ability_score(strength)
+        self._dexterity = self.set_initial_ability_score(dexterity)
+        self.constitution = self.set_initial_ability_score(constitution)
+        self.wisdom = self.set_initial_ability_score(wisdom)
+        self.intelligence = self.set_initial_ability_score(intelligence)
+        self.charisma = self.set_initial_ability_score(charisma)
 
         # Hit Dice and Hit Points: self.hd == 8 is a d8, 10 is a d10, etc
         self.hd = 8 if hd is None else hd
         self.max_hd = 1 if max_hd is None else max_hd
         self.current_hd = 1 if current_hd is None else current_hd
         self.max_hp = (
-            Character.maximum_hp(
+            Character.get_maximum_hp(
                 self.hd, 1 if level is None else int(level), self.constitution
             )
             if max_hp is None
             else max_hp
         )
         self._current_hp = current_hp if current_hp is not None else int(self.max_hp)
         self.temp_hp = 0 if temp_hp is None else int(temp_hp)
 
+        # Spells, Skills, Proficiencies
+        self.proficiencies = proficiencies if proficiencies is not None else {}
+        self.saving_throws = saving_throws if saving_throws is not None else []
+        self.spellcasting_stat = spellcasting_stat
+        self._cantrips_known: list["_SPELL"] = (
+            cantrips_known if cantrips_known is not None else []
+        )
+        self._spells_known: list["_SPELL"] = (
+            spells_known if spells_known is not None else []
+        )
+        self._spells_prepared: list["_SPELL"] = (
+            spells_prepared if spells_prepared is not None else []
+        )
+        self.set_spell_slots(spell_slots)
+
         # Experience points
         self._level = 1
         # self.level could be altered by Experience object below
         if experience is None:
             experience = 0
         self._experience = Experience(character=self, experience=int(experience))
 
         # Levels
         # self.level could be altered by Experience object above
         if level is not None:
             if self._experience.experience == 0:
                 # if only level is specified, set the experience to the amount for that level
-                self._experience.experience = experience_at_level(level)
+                self._experience._experience = experience_at_level(level)
+                self._experience.update_level()
                 # Experience alters self.level so it is now the correct value
             else:
                 # if level is specified AND experience is not zero:
                 # the Experience object normally handles the self.level attr
                 # but if a user changes their level manually, it should override this anyway
                 LOG.info(
                     f"Custom level for {str(self.name)}: {str(level)} instead of {str(self.level)}"
                 )
                 self._level = level
 
-        # Spells, Skills, Proficiencies
-        self.proficiencies = proficiencies if proficiencies is not None else {}
-        self.saving_throws = saving_throws if saving_throws is not None else []
-        self.cantrips_known = cantrips_known
-        self.spells_known = spells_known
-        self.spells_prepared = spells_prepared
-        self.spell_slots = spell_slots
-        self.spellcasting_stat = spellcasting_stat
-
         if skills_charisma is None:
             self.skills_charisma = {
                 "deception": False,
                 "intimidation": False,
                 "performance": False,
                 "persuasion": False,
             }
@@ -232,40 +247,57 @@
             self.skills_strength = {
                 "athletics": False,
             }
         else:
             self.skills_strength = skills_strength
 
         # Inventory & Wealth
-        self.wealth = wealth
-        self.inventory = []
+        final_wealth = None
+        if wealth_detailed is None:
+            final_wealth = float(sum_rolls(d10=4)) if wealth is None else wealth
+            self.wealth_detailed = self.infer_wealth(final_wealth)
+        else:
+            self.wealth_detailed = wealth_detailed
+            final_wealth = sum(
+                [coin_value[u] * v for u, v in self.wealth_detailed.items()]
+            )
+
+        # if both wealth parameters provided
+        if wealth is not None and float(wealth) != final_wealth:
+            raise InvalidParameterError(
+                "Both 'wealth' and 'wealth_detailed' parameters are provided, but 'wealth' seems incorrect."
+            )
+        self.wealth = final_wealth
+
+        # Inventory. Deserialize items and give them one by one
+        self._inventory: list[_Item] = []
         if inventory is not None:
             for item in inventory:
-                self.giveItem(item)
+                self.give_item(_Item(**item))
 
         # Final steps of initialization -- the classs.setter does lots of work here
         # setting the self.classs attr applies "class features" appropriate to character's level
         self.classs = classs
 
         # base armor class is 10 + DEX; will be affected by inventory
         if armor_class is not None:
             self.armor_class = armor_class
         elif not hasattr(self, "armor_class"):
-            self.armor_class = self.baseArmorClass
+            self.armor_class = self.base_armor_class
         self._dead = dead
         self._death_saves = death_saves
         self._death_fails = death_fails
-        self.exhaustion = int(exhaustion)
+        self.exhaustion = exhaustion
 
         if self.level == level_at_experience(self._experience._experience):
             self.level = self._level
             if current_hp is None:
                 # Set character's HP to the maximum for their level,
                 # only if the level isn't custom! (if it matches experience points according to SRD)
-                self.current_hp = Character.maximum_hp(
+                self.current_hp = Character.get_maximum_hp(
                     self.hd, self.level, self.constitution
                 )
 
         # Conditions
         all_conditions = [
             "blinded",
             "charmed",
@@ -279,381 +311,534 @@
             "poisoned",
             "prone",
             "restrained",
             "stunned",
             "unconscious",
         ]
         if conditions is None:
-            conditions = {}
-        for condition in all_conditions:
-            if condition not in conditions:
-                conditions[condition] = False
+            self.conditions = {k: False for k in all_conditions}
+        else:
+            self.conditions = {
+                k: conditions[k] if k in conditions.keys() else False
+                for k in all_conditions
+            }
 
-    def __str__(self):
+    def __str__(self) -> str:
         return (
             f"Name: {self.name}\n"
             f"Background:\n{self.background}\n\n"
             f"Age: {self.age}\n"
             f"Gender: {self.gender}\n"
             f"Description: {self.description}\n"
             f"Class: {self.class_name}\n"
             f"Level: {str(self.level)}\n"
             f"Current Experience: {str(self.experience)}\n"
             f"EXP to next Level: {str(self.experience.to_next_level)}\n\n"
             f"Proficiencies:\n{', '.join([value['name'] for value in self.proficiencies.values()])}\n\n"
-            f"Inventory:\n{', '.join([item['name'] for item in self.inventory])}\n\n"
+            f"Inventory:\n{', '.join([item.name for item in self.inventory])}\n\n"
             f"Class Features:\n{', '.join([item['name'] for item in self.class_features.values()])}\n\n"
         )
 
-    def keys(self):
-        keys = [key for key in self.__dict__ if not key.startswith("_")]
-        keys.extend(
-            [
-                "experience",
-                "death_saves",
-                "death_fails",
-                "dexterity",
-                "dead",
-                "current_hp",
-            ]
-        )
-        return keys
+    def __iter__(self) -> Iterator[tuple[str, Union[dict, list, int, str, bool, None]]]:
+        """
+        Enables `dict(self)` to return a dictionary representation of this object.
+        Iterate over this object to get (key, value) pairs.
 
-    def values(self):
-        vals = [
-            value if key != "uid" else str(value)
-            for key, value in self.__dict__.items()
-            if not key.startswith("_")
-        ]
-        vals.extend(
-            [
-                self._experience._experience,
-                self._death_saves,
-                self._death_fails,
-                self._dexterity,
-                self._dead,
-                self._current_hp,
+        Attrs starting with _ are skipped, as we assume they are non-serializable.
+        Such attrs must be added manually to the functions in this method.
+        """
+
+        def keys() -> list[str]:
+            keys = [key for key in self.__dict__ if not key.startswith("_")]
+            keys.extend(
+                [
+                    "experience",
+                    "death_saves",
+                    "death_fails",
+                    "dexterity",
+                    "dead",
+                    "current_hp",
+                    "inventory",
+                    "cantrips_known",
+                    "spells_known",
+                    "spells_prepared",
+                ]
+            )
+            return keys
+
+        def values() -> list[Union[dict, list, int, str, bool, None]]:
+            vals = [
+                value if key != "uid" else str(value)
+                for key, value in self.__dict__.items()
+                if not key.startswith("_")
             ]
-        )
-        return vals
+            vals.extend(
+                [
+                    self._experience._experience,
+                    self._death_saves,
+                    self._death_fails,
+                    self._dexterity,
+                    self._dead,
+                    self._current_hp,
+                    [dict(item) for item in self._inventory],
+                    [dict(spell) for spell in self._cantrips_known],
+                    [dict(spell) for spell in self._spells_known],
+                    [dict(spell) for spell in self._spells_prepared],
+                ]
+            )
+            return vals
+
+        return zip(keys(), values())
+
+    def __repr__(self) -> str:
+        """Returns a string that could be copy-pasted to create a new instance of this object"""
+        quote = lambda value: "'" if type(value) is str else ""
+        kwargs = [f"{key}={quote(value)}{value}{quote(value)}" for key, value in self]
+        return f"{type(self).__name__}({', '.join(kwargs)})"
+
+    def __eq__(self, other) -> bool:
+        """
+        Check if `other` is an identical character to `self`
+        Or if `other` is a dict that would construct an identical character
+        """
+        if type(other) is dict:
+            other = Character(**other)
+        if not isinstance(other, type(self)):
+            return False
+        for pair1, pair2 in zip(self, other):
+            if pair1 != pair2:
+                return False
+        return True
+
+    @property
+    def cantrips_known(self) -> list["_SPELL"]:
+        return self._cantrips_known
 
-    def __getitem__(self, key):
-        return dict(zip(self.keys(), self.values()))[key]
+    @cantrips_known.setter
+    def cantrips_known(self, new_val) -> None:
+        self._cantrips_known = new_val
 
     @property
-    def dead(self):
+    def spells_known(self) -> list["_SPELL"]:
+        return self._spells_known
+
+    @spells_known.setter
+    def spells_known(self, new_val) -> None:
+        self._spells_known = new_val
+
+    @property
+    def spells_prepared(self) -> list["_SPELL"]:
+        return self._spells_prepared
+
+    @spells_prepared.setter
+    def spells_prepared(self, new_val) -> None:
+        self._spells_prepared = new_val
+
+    @property
+    def inventory(self) -> list[_Item]:
+        return self._inventory
+
+    @property
+    def dead(self) -> bool:
         return self._dead
 
     @dead.setter
-    def dead(self, new_value: bool):
+    def dead(self, new_value: bool) -> None:
         self._dead = new_value
         self._death_saves = 0
         self._death_fails = 0
 
     @property
-    def death_saves(self):
+    def death_saves(self) -> int:
         return self._death_saves
 
     @death_saves.setter
-    def death_saves(self, new_value: int):
+    def death_saves(self, new_value: int) -> None:
         if not 4 > new_value > -1:
             raise ValueError("Death saving throws must be in range 0-3")
         elif new_value == 3:
             self._death_saves = 0
             self._death_fails = 0
             self._dead = False
         else:
             self._death_saves = new_value
 
     @property
-    def death_fails(self):
+    def death_fails(self) -> int:
         return self._death_fails
 
     @death_fails.setter
-    def death_fails(self, new_value: int):
+    def death_fails(self, new_value: int) -> None:
         if not 4 > new_value > -1:
             raise ValueError("Death saving throws must be in range 0-3")
         elif new_value == 3:
             self._death_saves = 0
             self._death_fails = 0
             self._dead = True
         else:
             self._death_fails = new_value
 
     @property
-    def current_hp(self):
+    def current_hp(self) -> int:
         return self._current_hp
 
     @current_hp.setter
-    def current_hp(self, new_value: int):
+    def current_hp(self, new_value: int) -> None:
         if new_value < 0:
             new_value = 0
         elif new_value > self.max_hp:
             new_value = int(self.max_hp)
         self._current_hp = new_value
 
     @property
-    def dexterity(self):
+    def dexterity(self) -> int:
         return self._dexterity
 
     @dexterity.setter
-    def dexterity(self, new_value):
+    def dexterity(self, new_value: int) -> None:
         self._dexterity = new_value
-        self.armor_class = self.baseArmorClass
+        self.armor_class = self.base_armor_class
         for item in self.inventory:
-            self.applyArmorClass(item)
+            self.apply_armor_class(item)
 
     @property
-    def experience(self):
+    def experience(self) -> Experience:
         return self._experience.experience
 
     @experience.setter
-    def experience(self, new_val):
+    def experience(self, new_val: int) -> None:
         if new_val is None:
             pass
         elif type(new_val) is Experience:
             self._experience = new_val
         else:
-            self._experience.experience = new_val
+            self._experience._experience = new_val
+            self._experience.update_level()
 
     @property
-    def classs(self):
+    def classs(self) -> Optional["_CLASS"]:
         return self.__class
 
     @classs.setter
-    def classs(self, new_class):
-        self.__class = new_class
+    def classs(self, new_class: Optional["_CLASS"]) -> None:
+        """
+        Triggered when the character's class is changed
+        """
+        if isinstance(new_class, dict):
+            # backwards compatibility
+            from .classes import CLASSES
+
+            LOG.warning("Implicitly converting classs dict to dataclass.")
+            new_class = CLASSES[new_class["index"]]
 
+        self.__class = new_class
         if new_class is None:
             return
 
-        self.class_name = new_class["name"]
-        self.class_index = new_class["index"]
-        self.hd = new_class["hit_die"]
-        self._class_levels = SRD_class_levels[self.class_index]
-        if "spellcasting" in new_class:
-            self.spellcasting_stat = new_class["spellcasting"]["spellcasting_ability"][
-                "index"
-            ]
-        else:
-            self.spellcasting_stat = None
-        self.applyClassLevel()
-
-        # create dict such as { "all-armor": {"name": "All armor", "type": "Armor"} }
-        for proficiency in new_class["proficiencies"]:
-            data = SRD(proficiency["url"])
-            self.proficiencies[proficiency["index"]] = {
-                "name": data["name"],
-                "type": data["type"],
-            }
+        def set_class() -> None:
+            """
+            Set miscellaneous class-related properties such as:
+            class name, hit dice, level progression data, proficiencies, saving throws,
+            spellcasting, and class features
+            """
+            self.class_name = new_class.name
+            self.class_index = new_class.index
+            self.hd = new_class.hit_die
+            self._class_levels = SRD_class_levels[self.class_index]
+            if new_class.spellcasting:
+                self.spellcasting_stat = new_class.spellcasting["spellcasting_ability"][
+                    "index"
+                ]
+            else:
+                self.spellcasting_stat = None
+            self.apply_class_level()
 
-        self.saving_throws = [
-            saving_throw["name"] for saving_throw in new_class["saving_throws"]
-        ]
+            # create dict such as { "all-armor": {"name": "All armor", "type": "Armor"} }
+            for proficiency in new_class.proficiencies:
+                data = SRD(proficiency["url"])
+                self.proficiencies[proficiency["index"]] = {
+                    "name": data["name"],
+                    "type": data["type"],
+                }
 
-        starting_equipment = new_class["starting_equipment"]
-        for item in starting_equipment:
-            for i in range(item["quantity"]):
-                self.giveItem(SRD(item["equipment"]["url"]))
-
-        self.player_options["starting_equipment"] = []
-
-        def add_to_starting_options(choice: str):
-            self.player_options["starting_equipment"].append(choice)
-
-        def fetch_choices_string(option):
-            choices = SRD(option["equipment_category"]["url"])["equipment"]
-            choices_names = [c["name"] for c in choices]
-            return "{} (choice from {})".format(
-                option["equipment_category"]["name"], ", ".join(choices_names)
-            )
+            self.saving_throws = [
+                saving_throw["name"] for saving_throw in new_class.saving_throws
+            ]
 
-        for item_option in new_class["starting_equipment_options"]:
-            options = []
-            opts = item_option["from"]
-            if "options" not in opts.keys():
-                choices = fetch_choices_string(opts)
-                add_to_starting_options(choices)
+        def set_starting_equipment() -> None:
+            """
+            Sets `player_options["starting_equipment"]` to a list of strings
+            """
+            for starting_equipment in new_class.starting_equipment:
+                new_item = Item(starting_equipment["equipment"]["index"])
+                new_item.quantity = starting_equipment["quantity"]
+                self.give_item(new_item)
+
+            self.player_options["starting_equipment"] = []
+
+            def add_to_starting_options(choice: str) -> None:
+                self.player_options["starting_equipment"].append(choice)
+
+            def fetch_choices_string(option: dict[str, dict[str, str]]) -> str:
+                choices = SRD(option["equipment_category"]["url"])["equipment"]
+                choices_names = [c["name"] for c in choices]
+                return "{} (choice from {})".format(
+                    option["equipment_category"]["name"], ", ".join(choices_names)
+                )
 
-            else:
-                for opt in opts["options"]:
-                    opt_type = opt["option_type"]
-                    if opt_type == "counted_reference":
-                        options.append(
-                            "{} x {}".format(opt["count"], opt["of"]["name"])
-                        )
-                    elif opt_type == "choice":
-                        how_many = opt["choice"]["choose"]
-                        choices = fetch_choices_string(opt["choice"]["from"])
-                        options.append("{} x {}".format(how_many, choices))
-                    elif opt_type == "multiple":
-                        try:
-                            combo = [
-                                str(c["count"]) + " " + c["of"]["name"]
-                                for c in opt["items"]
-                            ]
-                            add_to_starting_options("{}".format(", ".join(combo)))
-                        except KeyError:
-                            # shield or martial weapon
-                            martial_weapons = fetch_choices_string(
-                                opt["items"][0]["choice"]["from"]
+            for item_option in new_class.starting_equipment_options:
+                options = []
+                opts = item_option["from"]
+                if "options" not in opts.keys():
+                    choices = fetch_choices_string(opts)
+                    add_to_starting_options(choices)
+
+                else:
+                    for opt in opts["options"]:
+                        opt_type = opt["option_type"]
+                        if opt_type == "counted_reference":
+                            options.append(
+                                "{} x {}".format(opt["count"], opt["of"]["name"])
                             )
-                            shield = opt["items"][1]["of"]["name"]
-                            add_to_starting_options(
-                                "choose 1 from {} or a {}".format(
-                                    martial_weapons, shield
+                        elif opt_type == "choice":
+                            how_many = opt["choice"]["choose"]
+                            choices = fetch_choices_string(opt["choice"]["from"])
+                            options.append("{} x {}".format(how_many, choices))
+                        elif opt_type == "multiple":
+                            try:
+                                combo = [
+                                    str(c["count"]) + " " + c["of"]["name"]
+                                    for c in opt["items"]
+                                ]
+                                add_to_starting_options("{}".format(", ".join(combo)))
+                            except KeyError:
+                                # shield or martial weapon
+                                martial_weapons = fetch_choices_string(
+                                    opt["items"][0]["choice"]["from"]
                                 )
-                            )
-                            continue
+                                shield = opt["items"][1]["of"]["name"]
+                                add_to_starting_options(
+                                    "choose 1 from {} or a {}".format(
+                                        martial_weapons, shield
+                                    )
+                                )
+                                continue
 
-                add_to_starting_options("choose from {}".format(", ".join(options)))
+                    add_to_starting_options("choose from {}".format(", ".join(options)))
 
-    def applyClassLevel(self):
+        set_class()
+        set_starting_equipment()
+
+    def apply_class_level(self) -> None:
+        """
+        Applies changes based on the character's class and level
+        e.g., adds new class features, spell slots
+        Called by `level.setter` and `classs.setter`
+        """
         if self.level > 20:
             return
         for data in self._class_levels:
             if data["level"] > self.level:
                 break
             self.ability_score_bonus = data.get(
                 "ability_score_bonuses", self.ability_score_bonus
             )
             self.prof_bonus = data.get("prof_bonus", self.prof_bonus)
             for feat in data["features"]:
                 self.class_features[feat["index"]] = SRD(feat["url"])
             while len(self.class_features_enabled) < len(self.class_features):
                 self.class_features_enabled.append(True)
-            self.class_spellcasting = data.get("spellcasting", self.class_spellcasting)
+
+            # Fetch new spell slots
+            spell_slots = data.get("spellcasting", self.spell_slots)
+            self.set_spell_slots(spell_slots)
+
+    def set_spell_slots(self, new_spell_slots: dict[str, int]) -> dict[str, int]:
+        default_spell_slots = {
+            "cantrips_known": 0,
+            "spells_known": 0,
+            "spell_slots_level_1": 0,
+            "spell_slots_level_2": 0,
+            "spell_slots_level_3": 0,
+            "spell_slots_level_4": 0,
+            "spell_slots_level_5": 0,
+            "spell_slots_level_6": 0,
+            "spell_slots_level_7": 0,
+            "spell_slots_level_8": 0,
+            "spell_slots_level_9": 0,
+        }
+        self.spell_slots = new_spell_slots if new_spell_slots is not None else {}
+        for key in default_spell_slots:
+            if key not in self.spell_slots:
+                self.spell_slots[key] = default_spell_slots[key]
 
     @property
-    def level(self):
+    def level(self) -> int:
         return self._level
 
     @level.setter
-    def level(self, new_level):
+    def level(self, new_level: int) -> None:
         self._level = new_level
         if self.current_hp == self.max_hp:
-            self.current_hp = Character.maximum_hp(
+            self.current_hp = Character.get_maximum_hp(
                 self.hd, new_level, self.constitution
             )
-        self.max_hp = Character.maximum_hp(self.hd, new_level, self.constitution)
+        self.max_hp = Character.get_maximum_hp(self.hd, new_level, self.constitution)
         if self.current_hd == self.max_hd:
             self.current_hd = new_level
         self.max_hd = new_level
         if self.current_hd > self.max_hd:
             self.current_hd = self.max_hd
-        self.applyClassLevel()
+        self.apply_class_level()
 
-    def removeShields(self):
-        """Removes all shields from self.inventory. Used by self.giveItem when equipping shield"""
-        for i, item in enumerate(self.inventory):
+    def remove_shields(self) -> None:
+        """Removes all shields from self._inventory. Used by self.give_item when equipping shield"""
+        for i, item in enumerate(self._inventory):
             if (
-                item["equipment_category"]["index"] == "armor"
-                and item["armor_category"] == "Shield"
+                item.equipment_category["index"] == "armor"
+                and item.armor_category == "Shield"
             ):
-                self.inventory.pop(i)
+                self._inventory.pop(i)
 
-    def removeArmor(self):
-        """Removes all armor from self.inventory. Used by self.giveItem when equipping armor"""
-        for i, item in enumerate(self.inventory):
+    def remove_armor(self) -> None:
+        """Removes all armor from self._inventory. Used by self.give_item when equipping armor"""
+        for i, item in enumerate(self._inventory):
             if (
-                item["equipment_category"]["index"] == "armor"
-                and item["armor_category"] != "Shield"
+                item.equipment_category["index"] == "armor"
+                and item.armor_category != "Shield"
             ):
-                self.inventory.pop(i)
+                self._inventory.pop(i)
 
-    def applyArmorClass(self, item: dict):
-        if item["equipment_category"]["index"] == "armor":
-            if item["armor_category"] == "Shield":
-                self.removeShields()
+    def apply_armor_class(self, item: _Item) -> None:
+        if item.equipment_category["index"] == "armor":
+            if item.armor_category == "Shield":
+                self.remove_shields()
                 try:
-                    self.armor_class += item["armor_class"]["base"]
+                    self.armor_class += item.armor_class["base"]
                 except AttributeError:
                     # shield during __init__ without armor
                     self.armor_class = (
                         10
-                        + item["armor_class"]["base"]
-                        + Character.getModifier(self.dexterity)
+                        + item.armor_class["base"]
+                        + Character.get_ability_modifier(self.dexterity)
                     )
             else:
-                self.removeArmor()
-                self.armor_class = item["armor_class"]["base"] + (
+                self.remove_armor()
+                self.armor_class = item.armor_class["base"] + (
                     0
-                    if not item["armor_class"]["dex_bonus"]
-                    else Character.getModifier(self.dexterity)
+                    if not item.armor_class["dex_bonus"]
+                    else Character.get_ability_modifier(self.dexterity)
                 )
 
     @property
-    def baseArmorClass(self):
-        return 10 + Character.getModifier(self.dexterity)
+    def base_armor_class(self) -> int:
+        return 10 + Character.get_ability_modifier(self.dexterity)
 
-    def giveItem(self, item: dict):
+    def give_item(self, item: _Item) -> None:
         """
-        Adds an item to the Character's inventory list, as a dictionary.
+        Adds an item to the Character's inventory list.
         If the item is armor or a shield, the armor_class attribute will be set
         and any other armor/shields in the inventory will be removed.
         """
-        self.applyArmorClass(item)
-
+        self.apply_armor_class(item)
         self.inventory.append(item)
 
-    def removeItem(self, item):
-        if item["equipment_category"]["index"] == "armor":
-            if item["armor_category"] == "Shield":
-                self.armor_class -= item["armor_class"]["base"]
+    def remove_item(self, item: _Item) -> None:
+        if item.equipment_category["index"] == "armor":
+            if item.armor_category == "Shield":
+                self.armor_class -= item.armor_class["base"]
             else:
                 extra_ac_bonus = 0
                 shield = [
                     item
-                    for item in self.inventory
-                    if item["equipment_category"]["index"] == "armor"
-                    and item["armor_category"] == "Shield"
+                    for item in self._inventory
+                    if item.equipment_category["index"] == "armor"
+                    and item.armor_category == "Shield"
                 ]
                 if shield:
-                    extra_ac_bonus = shield[0]["armor_class"]["base"]
+                    extra_ac_bonus = shield[0].armor_class["base"]
                 self.armor_class = (
-                    10 + extra_ac_bonus + Character.getModifier(self.dexterity)
+                    10 + extra_ac_bonus + Character.get_ability_modifier(self.dexterity)
                 )
 
-        self.inventory.remove(item)
+        self._inventory.remove(item)
 
-    def giveWealth(self, amount) -> None:
-        """
-        Give wealth to character
-        """
-        self.wealth += amount
+    def change_wealth(
+        self,
+        pp: int = 0,
+        gp: int = 0,
+        ep: int = 0,
+        sp: int = 0,
+        cp: int = 0,
+        conversion: bool = False,
+    ) -> None:
+        change = locals()
+        change.pop("self", None)
+        change.pop("conversion", None)
+
+        total_change = sum([coin_value[u] * v for u, v in change.items()])
+        new_wealth = round(self.wealth + total_change, 2)
+        if new_wealth < 0:
+            raise ValueError("Character has not enough wealth to cover the change!")
+
+        if conversion:
+            self.wealth_detailed = self.infer_wealth(new_wealth)
+        else:
+            for unit, value in change.items():
+                new_value = self.wealth_detailed[unit] + value
+                if new_value < 0:
+                    raise ValueError(
+                        f"Character has not enough {unit}! Current balance: {self.wealth_detailed[unit]}"
+                    )
+                self.wealth_detailed[unit] = new_value
 
-    def removeWealth(self, amount: int) -> bool:
-        """
-        Remove wealth from character if possible. Returns bool to indicate success or failure.
-        If wealth < amount then wealth remains unchanged, otherwise this character loses wealth
-        """
-        if amount > self.wealth:
-            return False
-        else:
-            self.wealth -= amount
-            return True
+        self.wealth = new_wealth
 
     @staticmethod
-    def setInitialAbilityScore(stat: Optional[int]) -> int:
+    def infer_wealth(wealth: Union[int, float]) -> dict[str, int]:
+        """Estimates a reasonable coin distribution from gold denominated total wealth."""
+        # Convert to platinum for smaller weight/volume
+        if wealth > 100:
+            pp = int((wealth - 100) / 10)
+            gp = wealth - 10 * pp
+        else:
+            pp = 0
+            gp = wealth
+
+        # Convert fractional part to silver and copper (no electrum!)
+        gp_str = "{:.2f}".format(gp)  # two decimal rounded gp to two decimal string
+        gp_str_decimal = gp_str.split(".")[1]
+        sp = int(gp_str_decimal[0])
+        cp = int(gp_str_decimal[1])
+        gp = int(gp)
+
+        return {"pp": pp, "gp": gp, "ep": 0, "sp": sp, "cp": cp}
+
+    @staticmethod
+    def set_initial_ability_score(stat: Optional[int]) -> int:
         """
         Set ability score to an int. If the argument is None, then this method
         instead rolls for the initial starting ability score.
         """
         if stat is None:
             return sum_rolls(d6=4, drop_lowest=True)  # roll 4d6, drop lowest
         else:
             return int(stat)
 
     @staticmethod
-    def getModifier(number: int) -> int:
+    def get_ability_modifier(number: int) -> int:
         """
         This method returns the modifier for the given stat (INT, CON, etc.)
         The formula for this is (STAT - 10 / 2) so e.g. 14 results in 2
         """
-        return math.floor((number - 10) / 2)
+        return (number - 10) // 2
 
-    @classmethod
-    def maximum_hp(cls, hd: int, level: int, constitution: int) -> int:
+    @staticmethod
+    def get_maximum_hp(hd: int, level: int, constitution: int) -> int:
         """
         Calculate maximum hitpoints using hit dice (HD), level and constitution modifier
         """
-        return hd + ((int(hd / 2) + 1) * (level - 1)) + cls.getModifier(constitution)
+        return (
+            hd
+            + ((int(hd / 2) + 1) * (level - 1))
+            + Character.get_ability_modifier(constitution)
+        )
```

### Comparing `dnd_character-23.7.22/dnd_character/dice.py` & `dnd_character-23.7.29/dnd_character/dice.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     d20: int = 0,
     d12: int = 0,
     d10: int = 0,
     d8: int = 0,
     d6: int = 0,
     d4: int = 0,
     drop_lowest: bool = False,
-):
+) -> int:
     """Expected use: attack calculation, initial ability score, etc."""
     rolls = [random.randint(1, 100) for _ in range(d100)]
     rolls += [random.randint(1, 20) for _ in range(d20)]
     rolls += [random.randint(1, 12) for _ in range(d12)]
     rolls += [random.randint(1, 10) for _ in range(d10)]
     rolls += [random.randint(1, 8) for _ in range(d8)]
     rolls += [random.randint(1, 6) for _ in range(d6)]
@@ -25,15 +25,15 @@
         rolls = sorted(rolls)[1:]
 
     return sum(rolls)
 
 
 def roll_with_advantage_disadvantage(
     dice: int = 20, advantage: bool = False, disadvantage: bool = False
-):
+) -> int:
     """Expected use: D20 (ability checks, saving throws, attack rolls)"""
     if advantage == disadvantage:
         result = random.randint(1, dice)
     else:
         rolls = [random.randint(1, dice) for _ in range(2)]
         result = max(rolls) if advantage else min(rolls)
     return result
```

### Comparing `dnd_character-23.7.22/dnd_character/experience.py` & `dnd_character-23.7.29/dnd_character/experience.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 An integer-like property of the Character object that handles everything related to experience:
 experience points, leveling up and down, etc.
 """
 from functools import lru_cache
+from typing import TYPE_CHECKING
 import logging
-import typing
 
 
-if typing.TYPE_CHECKING:
+if TYPE_CHECKING:
     # allows type annotations to work without a circular import
     # https://peps.python.org/pep-0563/
     from .character import Character as Character
 
 
 LOG = logging.getLogger(__package__)
 
@@ -20,41 +20,46 @@
     def __init__(self, character: "Character", experience: int):
         # this typically occurs while `character` is partially initialized (during __init__)
         self.character = character
         self._experience = experience
         self.character.level = level_at_experience(experience)
 
     @property
-    def experience(self):
+    def experience(self) -> "Experience":
         return self
 
-    def __eq__(self, other):
-        return self._experience == other
-
     @experience.setter
-    def experience(self, new_val):
+    def experience(self, new_val: int) -> None:
         self._experience = new_val
+        self.update_level()
+
+    def update_level(self) -> None:
         self.character.level = level_at_experience(self._experience)
 
-    def __add__(self, new_val):
+    def __eq__(self, other: object) -> bool:
+        if isinstance(object, type(self)):
+            return self._experience == other._experience
+        return self._experience == other
+
+    def __add__(self, new_val: int) -> int:
         val = self._experience + int(new_val)
         return val if val >= 0 else 0
 
-    def __sub__(self, new_val):
+    def __sub__(self, new_val: int) -> int:
         val = self._experience - new_val
         return val if val >= 0 else 0
 
-    def __str__(self):
+    def __str__(self) -> str:
         return str(self._experience)
 
-    def __int__(self):
+    def __int__(self) -> int:
         return self._experience
 
     @property
-    def to_next_level(self):
+    def to_next_level(self) -> int:
         """
         Returns experience remaining until next level is reached
         """
         if self.character.level != level_at_experience(self._experience):
             LOG.warning(
                 f"{str(self.character.name)} has a custom level: {str(self.character.level)}"
                 f" which means to_next_level returned 0"
@@ -62,37 +67,37 @@
             return 0
         try:
             return level_progression[self.character.level + 1] - self._experience
         except IndexError:
             return 0
 
     @property
-    def to_last_level(self):
+    def to_last_level(self) -> int:
         """
         Returns experience remaining (to subtract) until previous level is reached
         """
         if self.character.level != level_at_experience(self._experience):
             LOG.warning(
                 f"{str(self.character.name)} has a custom level: {str(self.character.level)}"
                 f" which means to_last_level returned 0"
             )
             return 0
         return self._experience - level_progression[self.character.level]
 
 
 @lru_cache(maxsize=None)
-def level_at_experience(num):
+def level_at_experience(num: int) -> int:
     for level, threshold in enumerate(level_progression):
         if num >= threshold:
             continue
         return level - 1
     return 20
 
 
-def experience_at_level(num):
+def experience_at_level(num: int) -> int:
     return level_progression[num]
 
 
 level_progression = [
     0,
     0,
     300,
```

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/OGLv1.0a.txt` & `dnd_character-23.7.29/dnd_character/json_cache/OGLv1.0a.txt`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_classes.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_classes.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_classes_barbarian.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_classes_barbarian.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_classes_barbarian_levels.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_classes_barbarian_levels.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_classes_bard.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_classes_bard.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_classes_bard_levels.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_classes_bard_levels.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_classes_cleric.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_classes_cleric.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_classes_cleric_levels.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_classes_cleric_levels.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_classes_druid.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_classes_druid.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_classes_druid_levels.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_classes_druid_levels.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_classes_fighter.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_classes_fighter.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_classes_fighter_levels.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_classes_fighter_levels.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_classes_monk.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_classes_monk.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_classes_monk_levels.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_classes_monk_levels.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_classes_paladin.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_classes_paladin.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_classes_paladin_levels.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_classes_paladin_levels.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_classes_ranger.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_classes_ranger.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_classes_ranger_levels.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_classes_ranger_levels.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_classes_rogue.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_classes_rogue.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_classes_rogue_levels.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_classes_rogue_levels.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_classes_sorcerer.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_classes_sorcerer.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_classes_sorcerer_levels.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_classes_sorcerer_levels.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_classes_warlock.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_classes_warlock.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_classes_warlock_levels.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_classes_warlock_levels.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_classes_wizard.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_classes_wizard.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_classes_wizard_levels.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_classes_wizard_levels.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment-categories_martial-melee-weapons.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment-categories_martial-melee-weapons.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment-categories_martial-weapons.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment-categories_martial-weapons.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment-categories_musical-instruments.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment-categories_musical-instruments.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment-categories_simple-melee-weapons.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment-categories_simple-melee-weapons.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment-categories_simple-weapons.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment-categories_simple-weapons.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_acid-vial.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_acid-vial.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_alchemists-fire-flask.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_alchemists-fire-flask.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_alchemists-supplies.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_alchemists-supplies.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_amulet.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_amulet.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_antitoxin-vial.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_antitoxin-vial.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_bagpipes.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_bagpipes.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_ball-bearings-bag-of-1000.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_ball-bearings-bag-of-1000.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_barding-breastplate.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_barding-breastplate.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_barding-chain-mail.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_barding-chain-mail.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_barding-chain-shirt.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_barding-chain-shirt.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_barding-half-plate.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_barding-half-plate.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_barding-hide.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_barding-hide.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_barding-leather.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_barding-leather.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_barding-padded.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_barding-padded.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_barding-plate.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_barding-plate.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_barding-ring-mail.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_barding-ring-mail.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_barding-scale-mail.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_barding-scale-mail.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_barding-splint.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_barding-splint.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_barding-studded-leather.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_barding-studded-leather.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_battleaxe.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_battleaxe.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_block-and-tackle.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_block-and-tackle.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_block-of-incense.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_block-of-incense.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_blowgun.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_blowgun.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_book.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_book.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_brewers-supplies.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_brewers-supplies.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_burglars-pack.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_burglars-pack.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_calligraphers-supplies.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_calligraphers-supplies.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_caltrops.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_caltrops.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_candle.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_candle.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_carpenters-tools.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_carpenters-tools.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_cartographers-tools.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_cartographers-tools.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_case-crossbow-bolt.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_case-crossbow-bolt.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_case-map-or-scroll.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_case-map-or-scroll.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_chain-10-feet.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_chain-10-feet.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_climbers-kit.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_climbers-kit.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_club.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_club.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_cobblers-tools.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_cobblers-tools.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_component-pouch.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_component-pouch.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_cooks-utensils.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_cooks-utensils.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_crossbow-hand.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_crossbow-hand.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_crossbow-heavy.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_crossbow-heavy.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_crossbow-light.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_crossbow-light.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_crowbar.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_crowbar.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_crystal.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_crystal.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_dagger.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_dagger.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_dart.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_dart.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_dice-set.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_dice-set.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_diplomats-pack.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_diplomats-pack.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_disguise-kit.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_disguise-kit.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_drum.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_drum.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_dulcimer.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_dulcimer.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_dungeoneers-pack.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_dungeoneers-pack.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_emblem.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_emblem.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_entertainers-pack.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_entertainers-pack.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_explorers-pack.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_explorers-pack.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_fishing-tackle.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_fishing-tackle.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_flail.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_flail.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_flute.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_flute.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_forgery-kit.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_forgery-kit.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_glaive.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_glaive.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_glassblowers-tools.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_glassblowers-tools.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_greataxe.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_greataxe.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_greatclub.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_greatclub.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_greatsword.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_greatsword.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_halberd.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_halberd.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_handaxe.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_handaxe.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_healers-kit.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_healers-kit.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_herbalism-kit.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_herbalism-kit.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_holy-water-flask.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_holy-water-flask.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_horn.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_horn.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_hunting-trap.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_hunting-trap.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_javelin.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_javelin.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_jewelers-tools.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_jewelers-tools.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_keelboat.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_keelboat.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_lamp.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_lamp.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_lance.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_lance.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_lantern-bullseye.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_lantern-bullseye.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_lantern-hooded.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_lantern-hooded.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_leatherworkers-tools.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_leatherworkers-tools.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_light-hammer.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_light-hammer.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_little-bag-of-sand.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_little-bag-of-sand.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_lock.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_lock.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_longbow.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_longbow.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_longsword.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_longsword.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_lute.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_lute.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_lyre.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_lyre.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_mace.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_mace.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_magnifying-glass.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_magnifying-glass.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_manacles.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_manacles.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_masons-tools.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_masons-tools.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_maul.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_maul.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_mess-kit.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_mess-kit.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_morningstar.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_morningstar.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_navigators-tools.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_navigators-tools.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_net.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_net.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_oil-flask.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_oil-flask.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_orb.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_orb.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_painters-supplies.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_painters-supplies.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_pan-flute.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_pan-flute.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_pike.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_pike.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_playing-card-set.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_playing-card-set.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_poison-basic-vial.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_poison-basic-vial.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_poisoners-kit.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_poisoners-kit.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_potters-tools.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_potters-tools.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_pouch.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_pouch.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_priests-pack.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_priests-pack.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_quarterstaff.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_quarterstaff.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_ram-portable.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_ram-portable.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_rapier.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_rapier.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_rations-1-day.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_rations-1-day.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_reliquary.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_reliquary.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_rod.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_rod.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_rope-hempen-50-feet.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_rope-hempen-50-feet.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_rope-silk-50-feet.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_rope-silk-50-feet.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_rowboat.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_rowboat.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_saddle-military.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_saddle-military.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_scale-merchants.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_scale-merchants.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_scholars-pack.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_scholars-pack.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_scimitar.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_scimitar.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_shawm.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_shawm.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_shortbow.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_shortbow.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_shortsword.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_shortsword.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_sickle.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_sickle.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_sling.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_sling.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_smiths-tools.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_smiths-tools.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_spear.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_spear.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_spellbook.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_spellbook.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_sprig-of-mistletoe.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_sprig-of-mistletoe.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_spyglass.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_spyglass.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_staff.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_staff.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_string-10-feet.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_string-10-feet.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_tent-two-person.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_tent-two-person.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_thieves-tools.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_thieves-tools.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_tinderbox.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_tinderbox.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_tinkers-tools.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_tinkers-tools.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_torch.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_torch.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_totem.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_totem.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_trident.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_trident.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_viol.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_viol.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_wand.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_wand.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_war-pick.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_war-pick.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_warhammer.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_warhammer.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_weavers-tools.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_weavers-tools.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_whip.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_whip.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_woodcarvers-tools.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_woodcarvers-tools.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_wooden-staff.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_wooden-staff.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_equipment_yew-wand.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_equipment_yew-wand.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_action-surge-1-use.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_action-surge-1-use.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_action-surge-2-uses.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_action-surge-2-uses.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_arcane-recovery.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_arcane-recovery.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_archdruid.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_archdruid.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_aura-of-protection.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_aura-of-protection.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_barbarian-ability-score-improvement-1.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_barbarian-ability-score-improvement-1.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_barbarian-ability-score-improvement-2.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_barbarian-ability-score-improvement-2.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_barbarian-ability-score-improvement-3.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_barbarian-ability-score-improvement-3.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_barbarian-ability-score-improvement-4.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_barbarian-ability-score-improvement-4.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_barbarian-ability-score-improvement-5.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_barbarian-ability-score-improvement-5.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_bard-ability-score-improvement-1.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_bard-ability-score-improvement-1.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_bard-ability-score-improvement-2.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_bard-ability-score-improvement-2.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_bard-ability-score-improvement-3.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_bard-ability-score-improvement-3.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_bard-ability-score-improvement-4.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_bard-ability-score-improvement-4.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_bard-ability-score-improvement-5.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_bard-ability-score-improvement-5.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_bard-expertise-1.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_bard-expertise-1.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_bard-expertise-2.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_bard-expertise-2.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_bardic-inspiration-d10.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_bardic-inspiration-d10.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_bardic-inspiration-d12.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_bardic-inspiration-d12.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_bardic-inspiration-d6.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_bardic-inspiration-d6.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_bardic-inspiration-d8.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_bardic-inspiration-d8.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_channel-divinity-1-rest.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_channel-divinity-1-rest.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_channel-divinity-turn-undead.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_channel-divinity-turn-undead.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_channel-divinity.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_channel-divinity.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_cleric-ability-score-improvement-1.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_cleric-ability-score-improvement-1.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_cleric-ability-score-improvement-2.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_cleric-ability-score-improvement-2.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_cleric-ability-score-improvement-3.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_cleric-ability-score-improvement-3.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_cleric-ability-score-improvement-4.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_cleric-ability-score-improvement-4.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_cleric-ability-score-improvement-5.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_cleric-ability-score-improvement-5.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_countercharm.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_countercharm.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_danger-sense.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_danger-sense.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_deflect-missiles.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_deflect-missiles.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_divine-domain.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_divine-domain.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_divine-intervention.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_divine-intervention.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_divine-sense.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_divine-sense.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_divine-smite.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_divine-smite.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_domain-spells-1.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_domain-spells-1.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_domain-spells-2.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_domain-spells-2.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_domain-spells-3.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_domain-spells-3.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_domain-spells-4.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_domain-spells-4.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_domain-spells-5.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_domain-spells-5.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_druid-ability-score-improvement-1.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_druid-ability-score-improvement-1.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_druid-ability-score-improvement-2.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_druid-ability-score-improvement-2.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_druid-ability-score-improvement-3.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_druid-ability-score-improvement-3.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_druid-ability-score-improvement-4.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_druid-ability-score-improvement-4.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_druid-ability-score-improvement-5.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_druid-ability-score-improvement-5.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_eldritch-invocations.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_eldritch-invocations.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_eldritch-master.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_eldritch-master.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_empty-body.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_empty-body.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_favored-enemy-1-type.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_favored-enemy-1-type.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_favored-enemy-2-types.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_favored-enemy-2-types.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_favored-enemy-3-enemies.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_favored-enemy-3-enemies.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_feral-instinct.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_feral-instinct.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_feral-senses.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_feral-senses.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_fighter-ability-score-improvement-1.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_fighter-ability-score-improvement-1.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_fighter-ability-score-improvement-2.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_fighter-ability-score-improvement-2.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_fighter-ability-score-improvement-3.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_fighter-ability-score-improvement-3.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_fighter-ability-score-improvement-4.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_fighter-ability-score-improvement-4.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_fighter-ability-score-improvement-5.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_fighter-ability-score-improvement-5.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_fighter-ability-score-improvement-6.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_fighter-ability-score-improvement-6.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_fighter-ability-score-improvement-7.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_fighter-ability-score-improvement-7.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_fighter-fighting-style.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_fighter-fighting-style.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_flexible-casting-creating-spell-slots.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_flexible-casting-creating-spell-slots.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_foe-slayer.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_foe-slayer.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_font-of-magic.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_font-of-magic.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_hide-in-plain-sight.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_hide-in-plain-sight.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_improved-divine-smite.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_improved-divine-smite.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_indomitable-1-use.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_indomitable-1-use.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_indomitable-2-uses.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_indomitable-2-uses.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_indomitable-3-uses.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_indomitable-3-uses.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_ki.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_ki.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_lay-on-hands.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_lay-on-hands.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_magical-secrets-1.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_magical-secrets-1.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_magical-secrets-2.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_magical-secrets-2.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_magical-secrets-3.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_magical-secrets-3.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_martial-arts.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_martial-arts.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_metamagic-1.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_metamagic-1.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_metamagic-2.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_metamagic-2.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_metamagic-3.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_metamagic-3.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_monk-ability-score-improvement-1.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_monk-ability-score-improvement-1.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_monk-ability-score-improvement-2.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_monk-ability-score-improvement-2.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_monk-ability-score-improvement-3.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_monk-ability-score-improvement-3.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_monk-ability-score-improvement-4.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_monk-ability-score-improvement-4.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_monk-ability-score-improvement-5.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_monk-ability-score-improvement-5.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_monk-evasion.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_monk-evasion.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_mystic-arcanum-6th-level.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_mystic-arcanum-6th-level.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_mystic-arcanum-7th-level.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_mystic-arcanum-7th-level.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_mystic-arcanum-8th-level.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_mystic-arcanum-8th-level.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_mystic-arcanum-9th-level.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_mystic-arcanum-9th-level.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_natural-explorer-1-terrain-type.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_natural-explorer-1-terrain-type.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_natural-explorer-2-terrain-types.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_natural-explorer-2-terrain-types.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_natural-explorer-3-terrain-types.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_natural-explorer-3-terrain-types.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_oath-spells.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_oath-spells.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_pact-boon.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_pact-boon.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_paladin-ability-score-improvement-1.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_paladin-ability-score-improvement-1.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_paladin-ability-score-improvement-2.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_paladin-ability-score-improvement-2.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_paladin-ability-score-improvement-3.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_paladin-ability-score-improvement-3.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_paladin-ability-score-improvement-4.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_paladin-ability-score-improvement-4.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_paladin-ability-score-improvement-5.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_paladin-ability-score-improvement-5.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_paladin-fighting-style.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_paladin-fighting-style.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_primeval-awareness.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_primeval-awareness.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_rage.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_rage.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_ranger-ability-score-improvement-1.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_ranger-ability-score-improvement-1.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_ranger-ability-score-improvement-2.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_ranger-ability-score-improvement-2.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_ranger-ability-score-improvement-3.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_ranger-ability-score-improvement-3.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_ranger-ability-score-improvement-4.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_ranger-ability-score-improvement-4.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_ranger-ability-score-improvement-5.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_ranger-ability-score-improvement-5.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_ranger-fighting-style.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_ranger-fighting-style.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_ranger-lands-stride.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_ranger-lands-stride.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_reckless-attack.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_reckless-attack.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_relentless-rage.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_relentless-rage.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_rogue-ability-score-improvement-1.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_rogue-ability-score-improvement-1.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_rogue-ability-score-improvement-2.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_rogue-ability-score-improvement-2.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_rogue-ability-score-improvement-3.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_rogue-ability-score-improvement-3.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_rogue-ability-score-improvement-4.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_rogue-ability-score-improvement-4.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_rogue-ability-score-improvement-5.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_rogue-ability-score-improvement-5.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_rogue-ability-score-improvement-6.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_rogue-ability-score-improvement-6.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_rogue-evasion.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_rogue-evasion.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_rogue-expertise-1.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_rogue-expertise-1.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_rogue-expertise-2.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_rogue-expertise-2.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_sacred-oath.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_sacred-oath.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_signature-spell.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_signature-spell.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_sneak-attack.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_sneak-attack.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_song-of-rest-d10.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_song-of-rest-d10.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_song-of-rest-d12.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_song-of-rest-d12.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_song-of-rest-d6.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_song-of-rest-d6.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_song-of-rest-d8.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_song-of-rest-d8.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_sorcerer-ability-score-improvement-1.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_sorcerer-ability-score-improvement-1.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_sorcerer-ability-score-improvement-2.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_sorcerer-ability-score-improvement-2.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_sorcerer-ability-score-improvement-3.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_sorcerer-ability-score-improvement-3.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_sorcerer-ability-score-improvement-4.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_sorcerer-ability-score-improvement-4.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_sorcerer-ability-score-improvement-5.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_sorcerer-ability-score-improvement-5.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_spell-mastery.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_spell-mastery.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_stroke-of-luck.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_stroke-of-luck.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_stunning-strike.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_stunning-strike.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_thieves-cant.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_thieves-cant.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_unarmored-movement-1.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_unarmored-movement-1.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_unarmored-movement-2.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_unarmored-movement-2.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_warlock-ability-score-improvement-1.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_warlock-ability-score-improvement-1.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_warlock-ability-score-improvement-2.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_warlock-ability-score-improvement-2.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_warlock-ability-score-improvement-3.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_warlock-ability-score-improvement-3.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_warlock-ability-score-improvement-4.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_warlock-ability-score-improvement-4.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_warlock-ability-score-improvement-5.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_warlock-ability-score-improvement-5.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_wild-shape-cr-1-2-or-below-no-flying-speed.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_wild-shape-cr-1-2-or-below-no-flying-speed.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_wild-shape-cr-1-4-or-below-no-flying-or-swim-speed.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_wild-shape-cr-1-4-or-below-no-flying-or-swim-speed.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_wild-shape-cr-1-or-below.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_wild-shape-cr-1-or-below.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_wizard-ability-score-improvement-1.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_wizard-ability-score-improvement-1.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_wizard-ability-score-improvement-2.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_wizard-ability-score-improvement-2.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_wizard-ability-score-improvement-3.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_wizard-ability-score-improvement-3.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_wizard-ability-score-improvement-4.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_wizard-ability-score-improvement-4.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_features_wizard-ability-score-improvement-5.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_features_wizard-ability-score-improvement-5.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_aboleth.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_aboleth.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_acolyte.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_acolyte.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_adult-black-dragon.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_adult-black-dragon.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_adult-blue-dragon.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_adult-blue-dragon.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_adult-brass-dragon.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_adult-brass-dragon.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_adult-bronze-dragon.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_adult-bronze-dragon.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_adult-copper-dragon.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_adult-copper-dragon.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_adult-gold-dragon.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_adult-gold-dragon.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_adult-green-dragon.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_adult-green-dragon.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_adult-red-dragon.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_adult-red-dragon.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_adult-silver-dragon.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_adult-silver-dragon.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_adult-white-dragon.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_adult-white-dragon.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_air-elemental.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_air-elemental.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_ancient-black-dragon.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_ancient-black-dragon.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_ancient-blue-dragon.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_ancient-blue-dragon.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_ancient-brass-dragon.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_ancient-brass-dragon.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_ancient-bronze-dragon.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_ancient-bronze-dragon.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_ancient-copper-dragon.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_ancient-copper-dragon.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_ancient-gold-dragon.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_ancient-gold-dragon.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_ancient-green-dragon.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_ancient-green-dragon.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_ancient-red-dragon.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_ancient-red-dragon.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_ancient-silver-dragon.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_ancient-silver-dragon.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_ancient-white-dragon.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_ancient-white-dragon.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_androsphinx.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_androsphinx.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_animated-armor.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_animated-armor.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_ankheg.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_ankheg.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_ape.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_ape.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_archmage.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_archmage.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_assassin.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_assassin.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_awakened-shrub.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_awakened-shrub.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_awakened-tree.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_awakened-tree.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_axe-beak.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_axe-beak.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_azer.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_azer.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_baboon.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_baboon.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_badger.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_badger.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_balor.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_balor.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_bandit-captain.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_bandit-captain.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_bandit.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_bandit.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_barbed-devil.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_barbed-devil.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_basilisk.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_basilisk.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_bat.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_bat.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_bearded-devil.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_bearded-devil.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_behir.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_behir.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_berserker.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_berserker.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_black-bear.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_black-bear.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_black-dragon-wyrmling.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_black-dragon-wyrmling.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_black-pudding.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_black-pudding.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_blink-dog.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_blink-dog.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_blood-hawk.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_blood-hawk.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_blue-dragon-wyrmling.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_blue-dragon-wyrmling.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_boar.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_boar.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_bone-devil.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_bone-devil.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_brass-dragon-wyrmling.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_brass-dragon-wyrmling.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_bronze-dragon-wyrmling.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_bronze-dragon-wyrmling.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_brown-bear.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_brown-bear.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_bugbear.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_bugbear.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_bulette.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_bulette.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_camel.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_camel.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_cat.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_cat.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_centaur.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_centaur.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_chain-devil.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_chain-devil.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_chimera.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_chimera.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_chuul.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_chuul.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_clay-golem.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_clay-golem.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_cloaker.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_cloaker.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_cloud-giant.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_cloud-giant.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_cockatrice.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_cockatrice.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_commoner.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_commoner.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_constrictor-snake.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_constrictor-snake.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_copper-dragon-wyrmling.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_copper-dragon-wyrmling.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_couatl.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_couatl.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_crab.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_crab.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_crocodile.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_crocodile.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_cult-fanatic.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_cult-fanatic.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_cultist.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_cultist.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_darkmantle.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_darkmantle.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_death-dog.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_death-dog.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_deep-gnome-svirfneblin.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_deep-gnome-svirfneblin.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_deer.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_deer.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_deva.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_deva.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_dire-wolf.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_dire-wolf.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_djinni.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_djinni.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_doppelganger.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_doppelganger.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_draft-horse.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_draft-horse.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_dragon-turtle.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_dragon-turtle.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_dretch.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_dretch.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_drider.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_drider.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_drow.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_drow.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_druid.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_druid.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_dryad.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_dryad.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_duergar.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_duergar.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_dust-mephit.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_dust-mephit.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_eagle.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_eagle.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_earth-elemental.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_earth-elemental.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_efreeti.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_efreeti.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_elephant.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_elephant.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_elk.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_elk.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_erinyes.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_erinyes.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_ettercap.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_ettercap.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_ettin.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_ettin.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_fire-elemental.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_fire-elemental.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_fire-giant.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_fire-giant.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_flesh-golem.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_flesh-golem.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_flying-snake.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_flying-snake.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_flying-sword.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_flying-sword.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_frog.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_frog.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_frost-giant.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_frost-giant.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_gargoyle.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_gargoyle.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_gelatinous-cube.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_gelatinous-cube.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_ghast.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_ghast.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_ghost.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_ghost.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_ghoul.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_ghoul.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_giant-ape.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_giant-ape.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_giant-badger.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_giant-badger.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_giant-bat.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_giant-bat.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_giant-boar.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_giant-boar.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_giant-centipede.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_giant-centipede.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_giant-constrictor-snake.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_giant-constrictor-snake.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_giant-crab.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_giant-crab.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_giant-crocodile.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_giant-crocodile.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_giant-eagle.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_giant-eagle.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_giant-elk.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_giant-elk.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_giant-fire-beetle.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_giant-fire-beetle.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_giant-frog.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_giant-frog.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_giant-goat.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_giant-goat.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_giant-hyena.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_giant-hyena.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_giant-lizard.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_giant-lizard.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_giant-octopus.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_giant-octopus.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_giant-owl.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_giant-owl.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_giant-poisonous-snake.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_giant-poisonous-snake.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_giant-rat-diseased.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_giant-rat-diseased.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_giant-rat.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_giant-rat.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_giant-scorpion.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_giant-scorpion.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_giant-sea-horse.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_giant-sea-horse.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_giant-shark.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_giant-shark.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_giant-spider.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_giant-spider.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_giant-toad.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_giant-toad.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_giant-vulture.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_giant-vulture.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_giant-wasp.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_giant-wasp.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_giant-weasel.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_giant-weasel.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_giant-wolf-spider.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_giant-wolf-spider.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_gibbering-mouther.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_gibbering-mouther.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_glabrezu.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_glabrezu.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_gladiator.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_gladiator.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_gnoll.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_gnoll.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_goat.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_goat.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_goblin.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_goblin.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_gold-dragon-wyrmling.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_gold-dragon-wyrmling.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_gorgon.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_gorgon.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_gray-ooze.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_gray-ooze.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_green-dragon-wyrmling.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_green-dragon-wyrmling.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_green-hag.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_green-hag.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_grick.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_grick.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_griffon.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_griffon.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_grimlock.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_grimlock.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_guard.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_guard.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_guardian-naga.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_guardian-naga.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_gynosphinx.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_gynosphinx.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_half-red-dragon-veteran.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_half-red-dragon-veteran.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_harpy.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_harpy.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_hawk.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_hawk.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_hell-hound.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_hell-hound.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_hezrou.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_hezrou.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_hill-giant.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_hill-giant.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_hippogriff.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_hippogriff.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_hobgoblin.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_hobgoblin.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_homunculus.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_homunculus.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_horned-devil.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_horned-devil.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_hunter-shark.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_hunter-shark.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_hydra.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_hydra.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_hyena.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_hyena.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_ice-devil.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_ice-devil.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_ice-mephit.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_ice-mephit.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_imp.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_imp.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_invisible-stalker.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_invisible-stalker.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_iron-golem.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_iron-golem.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_jackal.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_jackal.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_killer-whale.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_killer-whale.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_knight.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_knight.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_kobold.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_kobold.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_kraken.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_kraken.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_lamia.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_lamia.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_lemure.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_lemure.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_lich.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_lich.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_lion.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_lion.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_lizard.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_lizard.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_lizardfolk.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_lizardfolk.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_mage.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_mage.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_magma-mephit.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_magma-mephit.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_magmin.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_magmin.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_mammoth.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_mammoth.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_manticore.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_manticore.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_marilith.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_marilith.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_mastiff.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_mastiff.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_medusa.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_medusa.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_merfolk.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_merfolk.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_merrow.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_merrow.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_mimic.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_mimic.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_minotaur-skeleton.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_minotaur-skeleton.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_minotaur.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_minotaur.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_mule.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_mule.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_mummy-lord.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_mummy-lord.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_mummy.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_mummy.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_nalfeshnee.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_nalfeshnee.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_night-hag.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_night-hag.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_nightmare.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_nightmare.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_noble.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_noble.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_ochre-jelly.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_ochre-jelly.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_octopus.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_octopus.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_ogre-zombie.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_ogre-zombie.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_ogre.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_ogre.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_oni.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_oni.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_orc.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_orc.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_otyugh.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_otyugh.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_owl.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_owl.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_owlbear.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_owlbear.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_panther.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_panther.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_pegasus.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_pegasus.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_phase-spider.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_phase-spider.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_pit-fiend.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_pit-fiend.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_planetar.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_planetar.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_plesiosaurus.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_plesiosaurus.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_poisonous-snake.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_poisonous-snake.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_polar-bear.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_polar-bear.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_pony.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_pony.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_priest.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_priest.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_pseudodragon.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_pseudodragon.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_purple-worm.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_purple-worm.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_quasit.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_quasit.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_quipper.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_quipper.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_rakshasa.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_rakshasa.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_rat.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_rat.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_raven.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_raven.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_red-dragon-wyrmling.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_red-dragon-wyrmling.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_reef-shark.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_reef-shark.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_remorhaz.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_remorhaz.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_rhinoceros.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_rhinoceros.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_riding-horse.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_riding-horse.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_roc.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_roc.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_roper.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_roper.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_rug-of-smothering.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_rug-of-smothering.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_rust-monster.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_rust-monster.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_saber-toothed-tiger.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_saber-toothed-tiger.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_sahuagin.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_sahuagin.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_salamander.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_salamander.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_satyr.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_satyr.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_scorpion.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_scorpion.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_scout.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_scout.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_sea-hag.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_sea-hag.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_sea-horse.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_sea-horse.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_shadow.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_shadow.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_shambling-mound.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_shambling-mound.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_shield-guardian.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_shield-guardian.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_shrieker.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_shrieker.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_silver-dragon-wyrmling.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_silver-dragon-wyrmling.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_skeleton.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_skeleton.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_solar.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_solar.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_specter.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_specter.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_spider.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_spider.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_spirit-naga.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_spirit-naga.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_sprite.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_sprite.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_spy.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_spy.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_steam-mephit.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_steam-mephit.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_stirge.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_stirge.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_stone-giant.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_stone-giant.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_stone-golem.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_stone-golem.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_storm-giant.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_storm-giant.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_succubus-incubus.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_succubus-incubus.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_swarm-of-bats.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_swarm-of-bats.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_swarm-of-beetles.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_swarm-of-beetles.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_swarm-of-centipedes.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_swarm-of-centipedes.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_swarm-of-insects.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_swarm-of-insects.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_swarm-of-poisonous-snakes.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_swarm-of-poisonous-snakes.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_swarm-of-quippers.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_swarm-of-quippers.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_swarm-of-rats.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_swarm-of-rats.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_swarm-of-ravens.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_swarm-of-ravens.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_swarm-of-spiders.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_swarm-of-spiders.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_swarm-of-wasps.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_swarm-of-wasps.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_tarrasque.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_tarrasque.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_thug.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_thug.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_tiger.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_tiger.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_treant.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_treant.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_tribal-warrior.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_tribal-warrior.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_triceratops.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_triceratops.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_troll.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_troll.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_tyrannosaurus-rex.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_tyrannosaurus-rex.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_unicorn.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_unicorn.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_vampire-bat.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_vampire-bat.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_vampire-mist.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_vampire-mist.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_vampire-spawn.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_vampire-spawn.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_vampire-vampire.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_vampire-vampire.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_veteran.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_veteran.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_violet-fungus.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_violet-fungus.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_vrock.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_vrock.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_vulture.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_vulture.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_warhorse-skeleton.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_warhorse-skeleton.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_warhorse.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_warhorse.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_water-elemental.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_water-elemental.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_weasel.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_weasel.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_werebear-bear.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_werebear-bear.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_werebear-human.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_werebear-human.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_werebear-hybrid.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_werebear-hybrid.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_wereboar-boar.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_wereboar-boar.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_wereboar-human.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_wereboar-human.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_wereboar-hybrid.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_wereboar-hybrid.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_wererat-human.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_wererat-human.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_wererat-hybrid.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_wererat-hybrid.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_wererat-rat.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_wererat-rat.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_weretiger-human.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_weretiger-human.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_weretiger-hybrid.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_weretiger-hybrid.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_weretiger-tiger.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_weretiger-tiger.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_werewolf-human.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_werewolf-human.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_werewolf-hybrid.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_werewolf-hybrid.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_werewolf-wolf.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_werewolf-wolf.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_white-dragon-wyrmling.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_white-dragon-wyrmling.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_wight.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_wight.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_will-o-wisp.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_will-o-wisp.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_winter-wolf.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_winter-wolf.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_wolf.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_wolf.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_worg.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_worg.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_wraith.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_wraith.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_wyvern.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_wyvern.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_xorn.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_xorn.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_young-black-dragon.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_young-black-dragon.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_young-blue-dragon.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_young-blue-dragon.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_young-brass-dragon.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_young-brass-dragon.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_young-bronze-dragon.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_young-bronze-dragon.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_young-copper-dragon.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_young-copper-dragon.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_young-gold-dragon.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_young-gold-dragon.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_young-green-dragon.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_young-green-dragon.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_young-red-dragon.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_young-red-dragon.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_young-silver-dragon.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_young-silver-dragon.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_young-white-dragon.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_young-white-dragon.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_monsters_zombie.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_monsters_zombie.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_proficiencies_light-armor.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_proficiencies_light-armor.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_proficiencies_martial-weapons.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_proficiencies_martial-weapons.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_proficiencies_medium-armor.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_proficiencies_medium-armor.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_proficiencies_saving-throw-cha.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_proficiencies_saving-throw-cha.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_proficiencies_saving-throw-str.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_proficiencies_saving-throw-str.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_proficiencies_saving-throw-wis.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_proficiencies_saving-throw-wis.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_proficiencies_shields.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_proficiencies_shields.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_proficiencies_simple-weapons.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_proficiencies_simple-weapons.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_ability-checks.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_ability-checks.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_ability-scores-and-modifiers.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_ability-scores-and-modifiers.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_actions-in-combat.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_actions-in-combat.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_activating-an-item.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_activating-an-item.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_advantage-and-disadvantage.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_advantage-and-disadvantage.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_attunement.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_attunement.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_between-adventures.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_between-adventures.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_casting-a-spell.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_casting-a-spell.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_cover.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_cover.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_damage-and-healing.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_damage-and-healing.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_diseases.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_diseases.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_fantasy-historical-pantheons.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_fantasy-historical-pantheons.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_madness.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_madness.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_making-an-attack.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_making-an-attack.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_mounted-combat.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_mounted-combat.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_movement-and-position.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_movement-and-position.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_movement.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_movement.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_objects.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_objects.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_poisons.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_poisons.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_proficiency-bonus.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_proficiency-bonus.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_resting.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_resting.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_saving-throws.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_saving-throws.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_sentient-magic-items.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_sentient-magic-items.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_standard-exchange-rates.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_standard-exchange-rates.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_the-environment.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_the-environment.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_the-order-of-combat.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_the-order-of-combat.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_the-planes-of-existence.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_the-planes-of-existence.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_time.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_time.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_traps.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_traps.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_underwater-combat.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_underwater-combat.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_using-each-ability.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_using-each-ability.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_wearing-and-wielding-items.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_wearing-and-wielding-items.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_rule-sections_what-is-a-spell.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_rule-sections_what-is-a-spell.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_rules.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_rules.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_rules_adventuring.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_rules_adventuring.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_rules_combat.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_rules_combat.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_rules_equipment.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_rules_equipment.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_rules_spellcasting.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_rules_spellcasting.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_rules_using-ability-scores.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_rules_using-ability-scores.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_acid-arrow.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_acid-arrow.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_acid-splash.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_acid-splash.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_aid.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_aid.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_alarm.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_alarm.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_alter-self.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_alter-self.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_animal-friendship.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_animal-friendship.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_animal-messenger.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_animal-messenger.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_animal-shapes.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_animal-shapes.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_animate-dead.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_animate-dead.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_animate-objects.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_animate-objects.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_antilife-shell.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_antilife-shell.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_antimagic-field.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_antimagic-field.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_antipathy-sympathy.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_antipathy-sympathy.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_arcane-eye.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_arcane-eye.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_arcane-hand.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_arcane-hand.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_arcane-lock.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_arcane-lock.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_arcane-sword.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_arcane-sword.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_arcanists-magic-aura.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_arcanists-magic-aura.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_astral-projection.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_astral-projection.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_augury.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_augury.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_awaken.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_awaken.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_bane.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_bane.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_banishment.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_banishment.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_barkskin.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_barkskin.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_beacon-of-hope.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_beacon-of-hope.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_bestow-curse.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_bestow-curse.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_black-tentacles.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_black-tentacles.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_blade-barrier.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_blade-barrier.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_bless.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_bless.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_blight.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_blight.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_blindness-deafness.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_blindness-deafness.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_blink.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_blink.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_blur.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_blur.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_branding-smite.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_branding-smite.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_burning-hands.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_burning-hands.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_call-lightning.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_call-lightning.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_calm-emotions.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_calm-emotions.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_chain-lightning.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_chain-lightning.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_charm-person.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_charm-person.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_chill-touch.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_chill-touch.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_circle-of-death.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_circle-of-death.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_clairvoyance.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_clairvoyance.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_clone.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_clone.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_cloudkill.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_cloudkill.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_color-spray.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_color-spray.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_command.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_command.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_commune-with-nature.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_commune-with-nature.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_commune.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_commune.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_comprehend-languages.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_comprehend-languages.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_compulsion.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_compulsion.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_cone-of-cold.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_cone-of-cold.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_confusion.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_confusion.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_conjure-animals.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_conjure-animals.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_conjure-celestial.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_conjure-celestial.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_conjure-elemental.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_conjure-elemental.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_conjure-fey.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_conjure-fey.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_conjure-minor-elementals.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_conjure-minor-elementals.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_conjure-woodland-beings.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_conjure-woodland-beings.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_contact-other-plane.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_contact-other-plane.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_contagion.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_contagion.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_contingency.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_contingency.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_continual-flame.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_continual-flame.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_control-water.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_control-water.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_control-weather.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_control-weather.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_counterspell.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_counterspell.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_create-food-and-water.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_create-food-and-water.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_create-or-destroy-water.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_create-or-destroy-water.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_create-undead.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_create-undead.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_creation.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_creation.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_cure-wounds.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_cure-wounds.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_dancing-lights.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_dancing-lights.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_darkness.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_darkness.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_darkvision.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_darkvision.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_daylight.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_daylight.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_death-ward.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_death-ward.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_delayed-blast-fireball.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_delayed-blast-fireball.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_demiplane.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_demiplane.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_detect-evil-and-good.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_detect-evil-and-good.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_detect-magic.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_detect-magic.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_detect-poison-and-disease.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_detect-poison-and-disease.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_detect-thoughts.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_detect-thoughts.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_dimension-door.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_dimension-door.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_disguise-self.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_disguise-self.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_disintegrate.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_disintegrate.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_dispel-evil-and-good.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_dispel-evil-and-good.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_dispel-magic.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_dispel-magic.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_divination.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_divination.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_divine-favor.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_divine-favor.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_divine-word.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_divine-word.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_dominate-beast.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_dominate-beast.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_dominate-monster.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_dominate-monster.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_dominate-person.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_dominate-person.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_dream.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_dream.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_druidcraft.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_druidcraft.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_earthquake.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_earthquake.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_eldritch-blast.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_eldritch-blast.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_enhance-ability.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_enhance-ability.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_enlarge-reduce.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_enlarge-reduce.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_entangle.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_entangle.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_enthrall.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_enthrall.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_etherealness.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_etherealness.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_expeditious-retreat.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_expeditious-retreat.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_eyebite.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_eyebite.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_fabricate.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_fabricate.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_faerie-fire.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_faerie-fire.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_faithful-hound.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_faithful-hound.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_false-life.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_false-life.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_fear.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_fear.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_feather-fall.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_feather-fall.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_feeblemind.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_feeblemind.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_find-familiar.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_find-familiar.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_find-steed.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_find-steed.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_find-the-path.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_find-the-path.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_find-traps.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_find-traps.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_finger-of-death.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_finger-of-death.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_fire-bolt.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_fire-bolt.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_fire-shield.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_fire-shield.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_fire-storm.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_fire-storm.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_fireball.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_fireball.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_flame-blade.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_flame-blade.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_flame-strike.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_flame-strike.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_flaming-sphere.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_flaming-sphere.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_flesh-to-stone.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_flesh-to-stone.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_floating-disk.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_floating-disk.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_fly.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_fly.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_fog-cloud.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_fog-cloud.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_forbiddance.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_forbiddance.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_forcecage.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_forcecage.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_foresight.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_foresight.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_freedom-of-movement.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_freedom-of-movement.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_freezing-sphere.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_freezing-sphere.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_gaseous-form.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_gaseous-form.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_gate.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_gate.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_geas.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_geas.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_gentle-repose.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_gentle-repose.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_giant-insect.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_giant-insect.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_glibness.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_glibness.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_globe-of-invulnerability.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_globe-of-invulnerability.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_glyph-of-warding.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_glyph-of-warding.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_goodberry.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_goodberry.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_grease.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_grease.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_greater-invisibility.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_greater-invisibility.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_greater-restoration.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_greater-restoration.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_guardian-of-faith.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_guardian-of-faith.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_guards-and-wards.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_guards-and-wards.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_guidance.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_guidance.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_guiding-bolt.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_guiding-bolt.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_gust-of-wind.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_gust-of-wind.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_hallow.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_hallow.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_hallucinatory-terrain.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_hallucinatory-terrain.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_harm.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_harm.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_haste.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_haste.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_heal.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_heal.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_healing-word.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_healing-word.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_heat-metal.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_heat-metal.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_hellish-rebuke.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_hellish-rebuke.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_heroes-feast.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_heroes-feast.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_heroism.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_heroism.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_hideous-laughter.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_hideous-laughter.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_hold-monster.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_hold-monster.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_hold-person.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_hold-person.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_holy-aura.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_holy-aura.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_hunters-mark.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_hunters-mark.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_hypnotic-pattern.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_hypnotic-pattern.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_ice-storm.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_ice-storm.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_identify.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_identify.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_illusory-script.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_illusory-script.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_imprisonment.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_imprisonment.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_incendiary-cloud.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_incendiary-cloud.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_inflict-wounds.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_inflict-wounds.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_insect-plague.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_insect-plague.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_instant-summons.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_instant-summons.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_invisibility.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_invisibility.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_irresistible-dance.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_irresistible-dance.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_jump.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_jump.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_knock.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_knock.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_legend-lore.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_legend-lore.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_lesser-restoration.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_lesser-restoration.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_levitate.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_levitate.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_light.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_light.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_lightning-bolt.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_lightning-bolt.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_locate-animals-or-plants.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_locate-animals-or-plants.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_locate-creature.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_locate-creature.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_locate-object.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_locate-object.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_longstrider.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_longstrider.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_mage-armor.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_mage-armor.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_mage-hand.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_mage-hand.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_magic-circle.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_magic-circle.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_magic-jar.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_magic-jar.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_magic-missile.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_magic-missile.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_magic-mouth.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_magic-mouth.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_magic-weapon.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_magic-weapon.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_magnificent-mansion.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_magnificent-mansion.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_major-image.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_major-image.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_mass-cure-wounds.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_mass-cure-wounds.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_mass-heal.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_mass-heal.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_mass-healing-word.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_mass-healing-word.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_mass-suggestion.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_mass-suggestion.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_maze.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_maze.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_meld-into-stone.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_meld-into-stone.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_mending.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_mending.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_message.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_message.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_meteor-swarm.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_meteor-swarm.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_mind-blank.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_mind-blank.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_minor-illusion.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_minor-illusion.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_mirage-arcane.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_mirage-arcane.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_mirror-image.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_mirror-image.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_mislead.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_mislead.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_misty-step.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_misty-step.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_modify-memory.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_modify-memory.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_moonbeam.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_moonbeam.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_move-earth.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_move-earth.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_nondetection.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_nondetection.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_pass-without-trace.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_pass-without-trace.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_passwall.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_passwall.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_phantasmal-killer.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_phantasmal-killer.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_phantom-steed.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_phantom-steed.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_planar-ally.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_planar-ally.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_planar-binding.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_planar-binding.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_plane-shift.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_plane-shift.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_plant-growth.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_plant-growth.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_poison-spray.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_poison-spray.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_polymorph.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_polymorph.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_power-word-kill.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_power-word-kill.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_power-word-stun.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_power-word-stun.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_prayer-of-healing.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_prayer-of-healing.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_prestidigitation.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_prestidigitation.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_prismatic-spray.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_prismatic-spray.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_prismatic-wall.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_prismatic-wall.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_private-sanctum.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_private-sanctum.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_produce-flame.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_produce-flame.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_programmed-illusion.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_programmed-illusion.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_project-image.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_project-image.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_protection-from-energy.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_protection-from-energy.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_protection-from-evil-and-good.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_protection-from-evil-and-good.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_protection-from-poison.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_protection-from-poison.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_purify-food-and-drink.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_purify-food-and-drink.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_raise-dead.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_raise-dead.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_ray-of-enfeeblement.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_ray-of-enfeeblement.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_ray-of-frost.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_ray-of-frost.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_regenerate.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_regenerate.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_reincarnate.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_reincarnate.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_remove-curse.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_remove-curse.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_resilient-sphere.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_resilient-sphere.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_resistance.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_resistance.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_resurrection.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_resurrection.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_reverse-gravity.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_reverse-gravity.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_revivify.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_revivify.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_rope-trick.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_rope-trick.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_sacred-flame.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_sacred-flame.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_sanctuary.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_sanctuary.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_scorching-ray.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_scorching-ray.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_scrying.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_scrying.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_secret-chest.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_secret-chest.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_see-invisibility.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_see-invisibility.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_seeming.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_seeming.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_sending.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_sending.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_sequester.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_sequester.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_shapechange.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_shapechange.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_shatter.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_shatter.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_shield-of-faith.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_shield-of-faith.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_shield.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_shield.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_shillelagh.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_shillelagh.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_shocking-grasp.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_shocking-grasp.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_silence.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_silence.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_silent-image.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_silent-image.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_simulacrum.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_simulacrum.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_sleep.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_sleep.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_sleet-storm.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_sleet-storm.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_slow.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_slow.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_spare-the-dying.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_spare-the-dying.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_speak-with-animals.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_speak-with-animals.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_speak-with-dead.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_speak-with-dead.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_speak-with-plants.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_speak-with-plants.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_spider-climb.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_spider-climb.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_spike-growth.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_spike-growth.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_spirit-guardians.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_spirit-guardians.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_spiritual-weapon.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_spiritual-weapon.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_stinking-cloud.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_stinking-cloud.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_stone-shape.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_stone-shape.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_stoneskin.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_stoneskin.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_storm-of-vengeance.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_storm-of-vengeance.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_suggestion.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_suggestion.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_sunbeam.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_sunbeam.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_sunburst.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_sunburst.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_symbol.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_symbol.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_telekinesis.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_telekinesis.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_telepathic-bond.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_telepathic-bond.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_teleport.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_teleport.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_teleportation-circle.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_teleportation-circle.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_thaumaturgy.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_thaumaturgy.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_thunderwave.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_thunderwave.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_time-stop.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_time-stop.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_tiny-hut.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_tiny-hut.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_tongues.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_tongues.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_transport-via-plants.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_transport-via-plants.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_tree-stride.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_tree-stride.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_true-polymorph.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_true-polymorph.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_true-resurrection.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_true-resurrection.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_true-seeing.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_true-seeing.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_true-strike.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_true-strike.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_unseen-servant.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_unseen-servant.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_vampiric-touch.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_vampiric-touch.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_vicious-mockery.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_vicious-mockery.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_wall-of-fire.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_wall-of-fire.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_wall-of-force.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_wall-of-force.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_wall-of-ice.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_wall-of-ice.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_wall-of-stone.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_wall-of-stone.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_wall-of-thorns.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_wall-of-thorns.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_warding-bond.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_warding-bond.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_water-breathing.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_water-breathing.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_water-walk.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_water-walk.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_web.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_web.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_weird.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_weird.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_wind-walk.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_wind-walk.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_wind-wall.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_wind-wall.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_wish.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_wish.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_word-of-recall.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_word-of-recall.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character/json_cache/api_spells_zone-of-truth.json` & `dnd_character-23.7.29/dnd_character/json_cache/api_spells_zone-of-truth.json`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/dnd_character.egg-info/PKG-INFO` & `dnd_character-23.7.29/dnd_character.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,133 +1,172 @@
 Metadata-Version: 2.1
 Name: dnd-character
-Version: 23.7.22
+Version: 23.7.29
 Summary: make Dungeons & Dragons characters as serializable objects
 Home-page: https://github.com/tassaron/dnd-character
 Author: Brianna Rainey
 License: EPL-2.0
 Keywords: dnd trpg tabletop rpg
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Games/Entertainment
 Classifier: Topic :: Games/Entertainment :: Role-Playing
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Eclipse Public License 2.0 (EPL-2.0)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # dnd-character
+
 A Python library to make 5e Dungeons & Dragons characters for use in another app. Characters are serializable into Python dicts so they can be saved and loaded however you wish.
 
 SRD rules are fetched from the [5e SRD API](https://github.com/5e-bits/5e-srd-api) the first time they're requested, then the JSON is cached locally for faster retrieval in the future. I've included the `json_cache` containing the SRD inside the repo in case this API changes, but when the API does change I will update this library. So please pin your version if you want to avoid any breaking changes.
 
 You can use this library as a CLI tool to generate character sheets from the terminal; see `python -m dnd_character --help` for details.
 
-
 ## Installation and Use
+
 1. Install from PyPI using `pip install dnd-character`
 1. See `example.py` for example code on how to use the library.
 1. Generate random character sheet text file with `python -m dnd_character --random > mycharactername.txt`
 
-
 ## Licenses
-The software is EPL-2.0 and the text for this license is in `LICENSE` as is standard for software. Originally forked from [PyDnD](https://github.com/Coffee-fueled-deadlines/PyDnD). The contents of `dnd_character/json_cache` are retrieved from [5e-srd-api](https://github.com/5e-bits/5e-srd-api), and are covered by the Open Game License. See `dnd_character/json_cache/OGLv1.0a.txt` for details.
 
+The software is EPL-2.0 and the text for this license is in `LICENSE` as is standard for software. Originally forked from [PyDnD](https://github.com/Coffee-fueled-deadlines/PyDnD). The contents of `dnd_character/json_cache` are retrieved from [5e-srd-api](https://github.com/5e-bits/5e-srd-api), and are covered by the Open Game License. See `dnd_character/json_cache/OGLv1.0a.txt` for details.
 
 ## Example Code
 
 ### Creating Characters and Monsters
-The `classes` module has functions for creating all 12 classes from the System Reference Document. The `monsters` module has a dictionary of monsters, which are dictionaries themselves.
-```
+
+The `classes` module has functions for creating all 12 classes from the System Reference Document. The `monsters` module has a factory function for creating monsters.
+
+```python
 from dnd_character.classes import Bard
-from dnd_character.monsters import SRD_monsters
+from dnd_character.monsters import Monster
 from random import randint
 
 brianna = Bard(
     name="Brianna",
     level=10,
     )
-zombie = SRD_monsters["zombie"]
-attack_bonus = zombie["actions"][0]["attack_bonus"]
+zombie = Monster("zombie")
+attack_bonus = zombie.actions[0]["attack_bonus"]
 # Zombie rolls a d20 to attack a Bard
 if randint(1, 20) + attack_bonus >= brianna.armor_class:
-    print(f"{brianna.name} was hit by {zombie['name']}!")
+    print(f"{brianna.name} was hit by {zombie.name}!")
 else:
     print(f"{brianna.name} bravely dodged the attack")
 ```
 
 ### Leveling and Experience
+
 The library should help leveling up characters automatically if you manage the Character's `experience` attribute. It's simpler to avoid modifying the level directly.
-```
-import dnd_character
+
+```python
+from dnd_character import Character
 thor = Character(name="Thor")
 assert thor.level == 1
 thor.experience += 1000
 assert thor.level == 3
 assert thor.experience.to_next_level == 1700
 thor.experience += thor.experience.to_next_level
 assert thor.level == 4
 ```
 
 ### Starting Equipment
+
 Characters initialized with a class will have the starting equipment of that class, and an attribute called `player_options` which lists the optional starting equipment.
-```
+
+```python
 from dnd_character.classes import Paladin
+from dnd_character.equipment import Item
 from pprint import pprint
 sturm = Paladin(dexterity=10)
 pprint(sturm.inventory)
 print(sturm.armor_class)
 # Remove Chain Mail
-sturm.removeItem(sturm.inventory[0])
+sturm.remove_item(sturm.inventory[0])
 print(sturm.armor_class)
 # New Item
-from dnd_character.equipment import SRD_equipment
-dragonlance = SRD_equipment['lance']
-dragonlance["name"] = "Dragonlance®"
-sturm.giveItem(dragonlance)
+dragonlance = Item('lance')
+dragonlance.name = "Dragonlance®"
+sturm.give_item(dragonlance)
 # View optional starting equipment
 pprint(sturm.player_options)
 ```
 
-
 ### Using Spells
-Support for spells is not super great at the moment. Characters have dictionaries like `spells_known` and `cantrips_known` in which you're expected to store dictionaries from `SRD_spells`... but there's no useful help from the library here. Yet!
-```
-from dnd_character.spellcasting import SRD_spells, spells_for_class_level
-from pprint import pprint
+
+Spells are represented by _SPELL objects from `dnd_character.spellcasting`. The best way to find spells is using the `spells_for_class_level` function.
+
+```python
+from dnd_character.spellcasting import spells_for_class_level
 cantrips = spells_for_class_level('wizard', 0)
-print(f"Cantrips available to a Wizard: {', '.join(cantrips)}")
+print(f"Cantrips available to a Wizard:")
 for spell in cantrips:
-    print(f"{SRD_spells[spell]['name']}:")
-    pprint(SRD_spells[spell])
-    break
+    print(spell)
 ```
 
+Characters have lists to store _SPELL objects:
+
+- `spells_prepared`
+- `spells_known`
+- `cantrips_known`
+
+Characters have a `spell_slots` dictionary which shows the **total** spell slots. Depletion and rest mechanics are planned for a future version.
+
+```python
+from dnd_character import Wizard
+from dnd_character.spellcasting import SPELLS
+# Create wizard and teach Identify, a level 1 spell
+my_wizard = Wizard(name="Gormwinkle")
+my_wizard.spells_prepared.append(SPELLS["identify"])
+# Get total spell slots
+spell_slots_level_1 = my_wizard.spell_slots["spell_slots_level_1"]
+print(f"{my_wizard.name} has {spell_slots_level_1} spell slots of 1st level")
+# Cast until wizard runs out of spell slots
+while spell_slots_level_1 > 0:
+    print(f"Casting {SPELLS['identify'].name}!")
+    spell_slots_level_1 -= 1
+```
+
+There is currently no way to manage wizard spellbooks or class-specific features such as the Wizard's arcane recovery or the Sorcerer's metamagic.
 
 ## Character Object
+
 Normal initialization arguments for a Character object:
-```
+
+```text
 name         (str)
 age          (str)
 gender       (str)
-alignment    (str): character's two letter alignment
-description  (str): physical description of player character
-biography    (str): backstory of player character	
 level        (int): starting level
-wealth       (int): starting wealth	
-strength     (int)
-dexterity    (int)
-constitution (int)
-wisdom       (int)
-intelligence (int)
-charisma     (int)
-hp           (int):
-classs      (dict): JSON returned from the 5e API -- dnd_character.SRD.SRD_classes["bard"]
+hp           (int)
+alignment    (str): character's two letter alignment (LE, CG, TN, etc.)
+description  (str): physical description of player character
+background   (str): one-word backstory (e.g., knight, chef, acolyte)
+wealth       (int): if None, roll 4d10 for starting gp (gold pieces)
+strength     (int): if None, roll 4d6 and drop the lowest
+dexterity    (int): if None, roll 4d6 and drop the lowest
+constitution (int): if None, roll 4d6 and drop the lowest
+wisdom       (int): if None, roll 4d6 and drop the lowest
+intelligence (int): if None, roll 4d6 and drop the lowest
+charisma     (int): if None, roll 4d6 and drop the lowest
+classs    (_CLASS): a D&D class object (e.g., CLASSES['bard'])
 ```
+
 In addition, the Character object can receive attributes that are normally set automatically, such as the UUID. This is for re-loading the objects from serialized data (via `Character(**characterData)`) and probably aren't arguments you would write manually into your code.
 
+## Serializing objects
+
+All objects in this library can be turned into Python dicts, which can then be turned back into objects. This means characters (along with their items and spells), and monsters as well.
+
+- `dict(object)` creates a serializable dict that could be reloaded from text (e.g., suitable for conversion to and from JSON)
+- `repr(object)` prints a string that would re-construct the Python object if pasted into a REPL
+- `str(object)` is not for serialization. It creates a "user-friendly" string
 
 ## Contributing
-Please feel free to open a Pull Request on GitHub! I would be happy to help merge any contributions no matter your skill level.
+
+I greatly appreciate feedback about desired features and information about how you're using this library. Please feel free to open an issue or pull request on GitHub! I would be happy to help merge any contributions no matter your skill level.
```

### Comparing `dnd_character-23.7.22/dnd_character.egg-info/SOURCES.txt` & `dnd_character-23.7.29/dnd_character.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dnd_character-23.7.22/setup.py` & `dnd_character-23.7.29/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,13 +24,13 @@
     long_description_content_type="text/markdown",
     keywords="dnd trpg tabletop rpg",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Topic :: Games/Entertainment",
         "Topic :: Games/Entertainment :: Role-Playing",
-        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: Eclipse Public License 2.0 (EPL-2.0)",
     ],
     # requests is needed in development to update the json_cache
     # install_requires=["requests"],
 )
```

