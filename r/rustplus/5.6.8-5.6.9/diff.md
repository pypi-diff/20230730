# Comparing `tmp/rustplus-5.6.8.tar.gz` & `tmp/rustplus-5.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rustplus-5.6.8.tar", last modified: Wed Jul  5 19:24:14 2023, max compression
+gzip compressed data, was "rustplus-5.6.9.tar", last modified: Sun Jul 30 09:53:43 2023, max compression
```

## Comparing `rustplus-5.6.8.tar` & `rustplus-5.6.9.tar`

### file list

```diff
@@ -1,120 +1,120 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 19:24:14.875584 rustplus-5.6.8/
--rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-07-05 19:24:06.000000 rustplus-5.6.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-07-05 19:24:06.000000 rustplus-5.6.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     2355 2023-07-05 19:24:14.875584 rustplus-5.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2005 2023-07-05 19:24:06.000000 rustplus-5.6.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 19:24:14.867584 rustplus-5.6.8/rustplus/
--rw-r--r--   0 runner    (1001) docker     (122)      775 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 19:24:14.867584 rustplus-5.6.8/rustplus/api/
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    20445 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/base_rust_api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 19:24:14.871584 rustplus-5.6.8/rustplus/api/icons/
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    23598 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/airfield.png
--rw-r--r--   0 runner    (1001) docker     (122)    13944 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/arctic_base.png
--rw-r--r--   0 runner    (1001) docker     (122)     3475 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/bandit.png
--rw-r--r--   0 runner    (1001) docker     (122)    35348 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/barn.png
--rw-r--r--   0 runner    (1001) docker     (122)     2553 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/cargo.png
--rw-r--r--   0 runner    (1001) docker     (122)     2058 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/chinook.png
--rw-r--r--   0 runner    (1001) docker     (122)     4228 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/chinook_blades.png
--rw-r--r--   0 runner    (1001) docker     (122)    23420 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/crate.png
--rw-r--r--   0 runner    (1001) docker     (122)    12339 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/desert_base.png
--rw-r--r--   0 runner    (1001) docker     (122)    34156 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/dome.png
--rw-r--r--   0 runner    (1001) docker     (122)    34662 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/excavator.png
--rw-r--r--   0 runner    (1001) docker     (122)     4934 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/explosion.png
--rw-r--r--   0 runner    (1001) docker     (122)    24176 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/fishing.png
--rw-r--r--   0 runner    (1001) docker     (122)     2882 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/harbour.png
--rw-r--r--   0 runner    (1001) docker     (122)    12195 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/icon.png
--rw-r--r--   0 runner    (1001) docker     (122)    41087 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/junkyard.png
--rw-r--r--   0 runner    (1001) docker     (122)     9091 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/large_oil_rig.png
--rw-r--r--   0 runner    (1001) docker     (122)    23696 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/launchsite.png
--rw-r--r--   0 runner    (1001) docker     (122)    27391 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/lighthouse.png
--rw-r--r--   0 runner    (1001) docker     (122)    23532 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/military_tunnels.png
--rw-r--r--   0 runner    (1001) docker     (122)    27923 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/mining_outpost.png
--rw-r--r--   0 runner    (1001) docker     (122)    30573 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/outpost.png
--rw-r--r--   0 runner    (1001) docker     (122)     2384 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/oxums.png
--rw-r--r--   0 runner    (1001) docker     (122)     2742 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/patrol.png
--rw-r--r--   0 runner    (1001) docker     (122)    23513 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/power_plant.png
--rw-r--r--   0 runner    (1001) docker     (122)    36433 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/quarry.png
--rw-r--r--   0 runner    (1001) docker     (122)    28365 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/satellite.png
--rw-r--r--   0 runner    (1001) docker     (122)    17804 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/sewer.png
--rw-r--r--   0 runner    (1001) docker     (122)     8114 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/small_oil_rig.png
--rw-r--r--   0 runner    (1001) docker     (122)    30710 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/stable.png
--rw-r--r--   0 runner    (1001) docker     (122)    28458 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/supermarket.png
--rw-r--r--   0 runner    (1001) docker     (122)     2049 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/swamp.png
--rw-r--r--   0 runner    (1001) docker     (122)     5300 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/train.png
--rw-r--r--   0 runner    (1001) docker     (122)    20587 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/train_yard.png
--rw-r--r--   0 runner    (1001) docker     (122)     3066 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/underwater_lab.png
--rw-r--r--   0 runner    (1001) docker     (122)     5705 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/vending_machine.png
--rw-r--r--   0 runner    (1001) docker     (122)    23907 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/water_treatment.png
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 19:24:14.871584 rustplus-5.6.8/rustplus/api/remote/
--rw-r--r--   0 runner    (1001) docker     (122)      341 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/remote/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 19:24:14.871584 rustplus-5.6.8/rustplus/api/remote/camera/
--rw-r--r--   0 runner    (1001) docker     (122)      147 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/remote/camera/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   118649 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/remote/camera/camera_constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     5588 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/remote/camera/camera_manager.py
--rw-r--r--   0 runner    (1001) docker     (122)    24457 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/remote/camera/camera_parser.py
--rw-r--r--   0 runner    (1001) docker     (122)     3354 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/remote/camera/structures.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 19:24:14.871584 rustplus-5.6.8/rustplus/api/remote/events/
--rw-r--r--   0 runner    (1001) docker     (122)      223 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/remote/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1617 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/remote/events/event_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)      751 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/remote/events/event_loop_manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     3325 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/remote/events/events.py
--rw-r--r--   0 runner    (1001) docker     (122)     2312 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/remote/events/handler_list.py
--rw-r--r--   0 runner    (1001) docker     (122)     3101 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/remote/events/map_event_listener.py
--rw-r--r--   0 runner    (1001) docker     (122)      862 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/remote/events/registered_listener.py
--rw-r--r--   0 runner    (1001) docker     (122)      542 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/remote/expo_bundle_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)      664 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/remote/fcm_listener.py
--rw-r--r--   0 runner    (1001) docker     (122)      799 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/remote/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (122)     4210 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/remote/ratelimiter.py
--rw-r--r--   0 runner    (1001) docker     (122)     8169 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/remote/rust_remote_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 19:24:14.875584 rustplus-5.6.8/rustplus/api/remote/rustplus_proto/
--rw-r--r--   0 runner    (1001) docker     (122)       24 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/remote/rustplus_proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    16144 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/remote/rustplus_proto/rustplus.py
--rw-r--r--   0 runner    (1001) docker     (122)    12828 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/remote/rustws.py
--rw-r--r--   0 runner    (1001) docker     (122)      892 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/remote/server_checker.py
--rw-r--r--   0 runner    (1001) docker     (122)    13358 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/rust_api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 19:24:14.875584 rustplus-5.6.8/rustplus/api/structures/
--rw-r--r--   0 runner    (1001) docker     (122)      390 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      894 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/structures/rust_chat_message.py
--rw-r--r--   0 runner    (1001) docker     (122)      852 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/structures/rust_contents.py
--rw-r--r--   0 runner    (1001) docker     (122)     2048 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/structures/rust_entity_info.py
--rw-r--r--   0 runner    (1001) docker     (122)     2004 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/structures/rust_info.py
--rw-r--r--   0 runner    (1001) docker     (122)      824 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/structures/rust_item.py
--rw-r--r--   0 runner    (1001) docker     (122)     1813 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/structures/rust_map.py
--rw-r--r--   0 runner    (1001) docker     (122)     4805 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/structures/rust_marker.py
--rw-r--r--   0 runner    (1001) docker     (122)     3008 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/structures/rust_team_info.py
--rw-r--r--   0 runner    (1001) docker     (122)     1110 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/structures/rust_time.py
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/structures/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 19:24:14.875584 rustplus-5.6.8/rustplus/commands/
--rw-r--r--   0 runner    (1001) docker     (122)      130 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      542 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/commands/command.py
--rw-r--r--   0 runner    (1001) docker     (122)      522 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/commands/command_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     2441 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/commands/command_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)      444 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/commands/command_options.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 19:24:14.875584 rustplus-5.6.8/rustplus/conversation/
--rw-r--r--   0 runner    (1001) docker     (122)      145 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/conversation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1885 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/conversation/conversation.py
--rw-r--r--   0 runner    (1001) docker     (122)     1550 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/conversation/conversation_factory.py
--rw-r--r--   0 runner    (1001) docker     (122)      289 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/conversation/conversation_prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 19:24:14.875584 rustplus-5.6.8/rustplus/exceptions/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1158 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 19:24:14.875584 rustplus-5.6.8/rustplus/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      181 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      924 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/utils/deprecated.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 19:24:14.875584 rustplus-5.6.8/rustplus/utils/fonts/
--rw-r--r--   0 runner    (1001) docker     (122)    74752 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/utils/fonts/PermanentMarker.ttf
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/utils/fonts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    27771 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/utils/grab_items.py
--rw-r--r--   0 runner    (1001) docker     (122)     6950 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/utils/rust_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      752 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/utils/server_id.py
--rw-r--r--   0 runner    (1001) docker     (122)      770 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/utils/yielding_event.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 19:24:14.867584 rustplus-5.6.8/rustplus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2355 2023-07-05 19:24:14.000000 rustplus-5.6.8/rustplus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3536 2023-07-05 19:24:14.000000 rustplus-5.6.8/rustplus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-05 19:24:14.000000 rustplus-5.6.8/rustplus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      105 2023-07-05 19:24:14.000000 rustplus-5.6.8/rustplus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-07-05 19:24:14.000000 rustplus-5.6.8/rustplus.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-07-05 19:24:14.875584 rustplus-5.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-07-05 19:24:06.000000 rustplus-5.6.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 09:53:43.467074 rustplus-5.6.9/
+-rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-07-30 09:53:30.000000 rustplus-5.6.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-07-30 09:53:30.000000 rustplus-5.6.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2058 2023-07-30 09:53:43.467074 rustplus-5.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1708 2023-07-30 09:53:30.000000 rustplus-5.6.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 09:53:43.447074 rustplus-5.6.9/rustplus/
+-rw-r--r--   0 runner    (1001) docker     (122)      775 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 09:53:43.451074 rustplus-5.6.9/rustplus/api/
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20445 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/base_rust_api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 09:53:43.463074 rustplus-5.6.9/rustplus/api/icons/
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/icons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23598 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/icons/airfield.png
+-rw-r--r--   0 runner    (1001) docker     (122)    13944 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/icons/arctic_base.png
+-rw-r--r--   0 runner    (1001) docker     (122)     3475 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/icons/bandit.png
+-rw-r--r--   0 runner    (1001) docker     (122)    35348 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/icons/barn.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2553 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/icons/cargo.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2058 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/icons/chinook.png
+-rw-r--r--   0 runner    (1001) docker     (122)     4228 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/icons/chinook_blades.png
+-rw-r--r--   0 runner    (1001) docker     (122)    23420 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/icons/crate.png
+-rw-r--r--   0 runner    (1001) docker     (122)    12339 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/icons/desert_base.png
+-rw-r--r--   0 runner    (1001) docker     (122)    34156 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/icons/dome.png
+-rw-r--r--   0 runner    (1001) docker     (122)    34662 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/icons/excavator.png
+-rw-r--r--   0 runner    (1001) docker     (122)     4934 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/icons/explosion.png
+-rw-r--r--   0 runner    (1001) docker     (122)    24176 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/icons/fishing.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2882 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/icons/harbour.png
+-rw-r--r--   0 runner    (1001) docker     (122)    12195 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/icons/icon.png
+-rw-r--r--   0 runner    (1001) docker     (122)    41087 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/icons/junkyard.png
+-rw-r--r--   0 runner    (1001) docker     (122)     9091 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/icons/large_oil_rig.png
+-rw-r--r--   0 runner    (1001) docker     (122)    23696 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/icons/launchsite.png
+-rw-r--r--   0 runner    (1001) docker     (122)    27391 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/icons/lighthouse.png
+-rw-r--r--   0 runner    (1001) docker     (122)    23532 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/icons/military_tunnels.png
+-rw-r--r--   0 runner    (1001) docker     (122)    27923 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/icons/mining_outpost.png
+-rw-r--r--   0 runner    (1001) docker     (122)    30573 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/icons/outpost.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2384 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/icons/oxums.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2742 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/icons/patrol.png
+-rw-r--r--   0 runner    (1001) docker     (122)    23513 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/icons/power_plant.png
+-rw-r--r--   0 runner    (1001) docker     (122)    36433 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/icons/quarry.png
+-rw-r--r--   0 runner    (1001) docker     (122)    28365 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/icons/satellite.png
+-rw-r--r--   0 runner    (1001) docker     (122)    17804 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/icons/sewer.png
+-rw-r--r--   0 runner    (1001) docker     (122)     8114 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/icons/small_oil_rig.png
+-rw-r--r--   0 runner    (1001) docker     (122)    30710 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/icons/stable.png
+-rw-r--r--   0 runner    (1001) docker     (122)    28458 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/icons/supermarket.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2049 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/icons/swamp.png
+-rw-r--r--   0 runner    (1001) docker     (122)     5300 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/icons/train.png
+-rw-r--r--   0 runner    (1001) docker     (122)    20587 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/icons/train_yard.png
+-rw-r--r--   0 runner    (1001) docker     (122)     3066 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/icons/underwater_lab.png
+-rw-r--r--   0 runner    (1001) docker     (122)     5705 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/icons/vending_machine.png
+-rw-r--r--   0 runner    (1001) docker     (122)    23907 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/icons/water_treatment.png
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 09:53:43.463074 rustplus-5.6.9/rustplus/api/remote/
+-rw-r--r--   0 runner    (1001) docker     (122)      341 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/remote/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 09:53:43.463074 rustplus-5.6.9/rustplus/api/remote/camera/
+-rw-r--r--   0 runner    (1001) docker     (122)      147 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/remote/camera/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   118649 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/remote/camera/camera_constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5588 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/remote/camera/camera_manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24457 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/remote/camera/camera_parser.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3354 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/remote/camera/structures.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 09:53:43.463074 rustplus-5.6.9/rustplus/api/remote/events/
+-rw-r--r--   0 runner    (1001) docker     (122)      223 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/remote/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1617 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/remote/events/event_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)      751 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/remote/events/event_loop_manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3325 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/remote/events/events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2312 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/remote/events/handler_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3101 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/remote/events/map_event_listener.py
+-rw-r--r--   0 runner    (1001) docker     (122)      862 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/remote/events/registered_listener.py
+-rw-r--r--   0 runner    (1001) docker     (122)      664 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/remote/fcm_listener.py
+-rw-r--r--   0 runner    (1001) docker     (122)      799 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/remote/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4210 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/remote/ratelimiter.py
+-rw-r--r--   0 runner    (1001) docker     (122)      542 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/remote/rplus_version_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8171 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/remote/rust_remote_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 09:53:43.463074 rustplus-5.6.9/rustplus/api/remote/rustplus_proto/
+-rw-r--r--   0 runner    (1001) docker     (122)       24 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/remote/rustplus_proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16144 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/remote/rustplus_proto/rustplus.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12828 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/remote/rustws.py
+-rw-r--r--   0 runner    (1001) docker     (122)      892 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/remote/server_checker.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13352 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/rust_api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 09:53:43.463074 rustplus-5.6.9/rustplus/api/structures/
+-rw-r--r--   0 runner    (1001) docker     (122)      390 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      894 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/structures/rust_chat_message.py
+-rw-r--r--   0 runner    (1001) docker     (122)      852 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/structures/rust_contents.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2048 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/structures/rust_entity_info.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2004 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/structures/rust_info.py
+-rw-r--r--   0 runner    (1001) docker     (122)      824 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/structures/rust_item.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1813 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/structures/rust_map.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4805 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/structures/rust_marker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3008 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/structures/rust_team_info.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1110 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/structures/rust_time.py
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/api/structures/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 09:53:43.463074 rustplus-5.6.9/rustplus/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)      130 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      542 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/commands/command.py
+-rw-r--r--   0 runner    (1001) docker     (122)      522 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/commands/command_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2441 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/commands/command_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)      444 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/commands/command_options.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 09:53:43.467074 rustplus-5.6.9/rustplus/conversation/
+-rw-r--r--   0 runner    (1001) docker     (122)      145 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/conversation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1885 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/conversation/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1550 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/conversation/conversation_factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)      289 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/conversation/conversation_prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 09:53:43.467074 rustplus-5.6.9/rustplus/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1158 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 09:53:43.467074 rustplus-5.6.9/rustplus/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      181 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      924 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/utils/deprecated.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 09:53:43.467074 rustplus-5.6.9/rustplus/utils/fonts/
+-rw-r--r--   0 runner    (1001) docker     (122)    74752 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/utils/fonts/PermanentMarker.ttf
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/utils/fonts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27771 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/utils/grab_items.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6950 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/utils/rust_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      752 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/utils/server_id.py
+-rw-r--r--   0 runner    (1001) docker     (122)      770 2023-07-30 09:53:30.000000 rustplus-5.6.9/rustplus/utils/yielding_event.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 09:53:43.447074 rustplus-5.6.9/rustplus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2058 2023-07-30 09:53:43.000000 rustplus-5.6.9/rustplus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3538 2023-07-30 09:53:43.000000 rustplus-5.6.9/rustplus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-30 09:53:43.000000 rustplus-5.6.9/rustplus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      105 2023-07-30 09:53:43.000000 rustplus-5.6.9/rustplus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-07-30 09:53:43.000000 rustplus-5.6.9/rustplus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-07-30 09:53:43.467074 rustplus-5.6.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-07-30 09:53:30.000000 rustplus-5.6.9/setup.py
```

### Comparing `rustplus-5.6.8/LICENSE` & `rustplus-5.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/PKG-INFO` & `rustplus-5.6.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rustplus
-Version: 5.6.8
+Version: 5.6.9
 Summary: A python wrapper for the Rust Plus API
 Home-page: https://github.com/olijeffers0n/rustplus
 Author: olijeffers0n
 License: MIT
 Project-URL: Issue tracker, https://github.com/olijeffers0n/rustplus/issues
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
@@ -22,42 +22,38 @@
     <div>
         <a href = "https://ko-fi.com/O5O3ALGLJ">
             <img src= "https://ko-fi.com/img/githubbutton_sm.svg" width="190">
         </a>
     </div>
 </div>
 
-A lot of code and ideas have come from the JavaScript version of a wrapper, so I will credit it now:
-[RustPlus.js](https://github.com/liamcottle/rustplus.js)
-I have used his Protocol Buffer file for generating the necessary requests so chuck some support their way
-
-
 ## Installation:
 Install the package with:
 ```
 pip install rustplus
 ```
-It should also install all the dependencies, but if not you will have to install them yourself
 
 ## What can you do?
 - Get the Map
 - Get Team Info
 - Get Team Chat
 - Get Server Info
 - Send Team Messages
 - Getting the time
 - Using Smart Devices
 - Camera Handling
 
 # For information on all the above methods, see the [Wiki](https://rplus.ollieee.xyz)
 
 ### Support:
-If you need help, or you think that there is an issue feel free to open an issue. If you think you have made some improvements, open a PR! 
+If you need help, or you think that there is a problem feel free to open an issue. If you think you have made some improvements, open a PR! 
+
+Feel free to chuck some support to Liam at [RustPlus.js](https://github.com/liamcottle/rustplus.js) as he was the first to really crack this API
 
-I have tried to explain this a well as possible, but if you should need further clarification, join me on my discord server:
+You can also join me on my discord server:
 <div align="center">
     <a href = "https://discord.gg/nQqJe8qvP8">
         <img src="https://discordapp.com/api/guilds/872406750639321088/widget.png?style=banner2" alt="Discord">
     </a>
 </div>
 
 GitHub ⭐'s are always welcome :)
```

### Comparing `rustplus-5.6.8/README.md` & `rustplus-5.6.9/rustplus.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: rustplus
+Version: 5.6.9
+Summary: A python wrapper for the Rust Plus API
+Home-page: https://github.com/olijeffers0n/rustplus
+Author: olijeffers0n
+License: MIT
+Project-URL: Issue tracker, https://github.com/olijeffers0n/rustplus/issues
+Requires-Python: >=3.8.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ![Rust+.py](https://raw.githubusercontent.com/olijeffers0n/rustplus/master/icon.png)
 <div align = "center">
 	<img src = "https://static.pepy.tech/personalized-badge/rustplus?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads">
 	<img src = "https://img.shields.io/pypi/v/rustplus?label=PYPI%20Version">
 	<img src = "https://img.shields.io/pypi/l/rustplus">
 	<img src = "https://img.shields.io/github/stars/olijeffers0n/rustplus?label=GitHub%20Stars">
 	<a href = "https://discord.gg/nQqJe8qvP8">
@@ -10,42 +22,38 @@
     <div>
         <a href = "https://ko-fi.com/O5O3ALGLJ">
             <img src= "https://ko-fi.com/img/githubbutton_sm.svg" width="190">
         </a>
     </div>
 </div>
 
-A lot of code and ideas have come from the JavaScript version of a wrapper, so I will credit it now:
-[RustPlus.js](https://github.com/liamcottle/rustplus.js)
-I have used his Protocol Buffer file for generating the necessary requests so chuck some support their way
-
-
 ## Installation:
 Install the package with:
 ```
 pip install rustplus
 ```
-It should also install all the dependencies, but if not you will have to install them yourself
 
 ## What can you do?
 - Get the Map
 - Get Team Info
 - Get Team Chat
 - Get Server Info
 - Send Team Messages
 - Getting the time
 - Using Smart Devices
 - Camera Handling
 
 # For information on all the above methods, see the [Wiki](https://rplus.ollieee.xyz)
 
 ### Support:
-If you need help, or you think that there is an issue feel free to open an issue. If you think you have made some improvements, open a PR! 
+If you need help, or you think that there is a problem feel free to open an issue. If you think you have made some improvements, open a PR! 
+
+Feel free to chuck some support to Liam at [RustPlus.js](https://github.com/liamcottle/rustplus.js) as he was the first to really crack this API
 
-I have tried to explain this a well as possible, but if you should need further clarification, join me on my discord server:
+You can also join me on my discord server:
 <div align="center">
     <a href = "https://discord.gg/nQqJe8qvP8">
         <img src="https://discordapp.com/api/guilds/872406750639321088/widget.png?style=banner2" alt="Discord">
     </a>
 </div>
 
 GitHub ⭐'s are always welcome :)
```

### Comparing `rustplus-5.6.8/rustplus/__init__.py` & `rustplus-5.6.9/rustplus/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,9 +18,9 @@
 from .commands import CommandOptions, Command
 from .exceptions import *
 from .conversation import ConversationFactory, Conversation, ConversationPrompt
 from .utils import *
 
 __name__ = "rustplus"
 __author__ = "olijeffers0n"
-__version__ = "5.6.8"
+__version__ = "5.6.9"
 __support__ = "Discord: https://discord.gg/nQqJe8qvP8"
```

### Comparing `rustplus-5.6.8/rustplus/api/base_rust_api.py` & `rustplus-5.6.9/rustplus/api/base_rust_api.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/api/icons/airfield.png` & `rustplus-5.6.9/rustplus/api/icons/airfield.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/api/icons/arctic_base.png` & `rustplus-5.6.9/rustplus/api/icons/arctic_base.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/api/icons/bandit.png` & `rustplus-5.6.9/rustplus/api/icons/bandit.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/api/icons/barn.png` & `rustplus-5.6.9/rustplus/api/icons/barn.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/api/icons/cargo.png` & `rustplus-5.6.9/rustplus/api/icons/cargo.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/api/icons/chinook.png` & `rustplus-5.6.9/rustplus/api/icons/chinook.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/api/icons/chinook_blades.png` & `rustplus-5.6.9/rustplus/api/icons/chinook_blades.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/api/icons/crate.png` & `rustplus-5.6.9/rustplus/api/icons/crate.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/api/icons/desert_base.png` & `rustplus-5.6.9/rustplus/api/icons/desert_base.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/api/icons/dome.png` & `rustplus-5.6.9/rustplus/api/icons/dome.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/api/icons/excavator.png` & `rustplus-5.6.9/rustplus/api/icons/excavator.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/api/icons/explosion.png` & `rustplus-5.6.9/rustplus/api/icons/explosion.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/api/icons/fishing.png` & `rustplus-5.6.9/rustplus/api/icons/fishing.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/api/icons/harbour.png` & `rustplus-5.6.9/rustplus/api/icons/harbour.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/api/icons/icon.png` & `rustplus-5.6.9/rustplus/api/icons/icon.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/api/icons/junkyard.png` & `rustplus-5.6.9/rustplus/api/icons/junkyard.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/api/icons/large_oil_rig.png` & `rustplus-5.6.9/rustplus/api/icons/large_oil_rig.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/api/icons/launchsite.png` & `rustplus-5.6.9/rustplus/api/icons/launchsite.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/api/icons/lighthouse.png` & `rustplus-5.6.9/rustplus/api/icons/lighthouse.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/api/icons/military_tunnels.png` & `rustplus-5.6.9/rustplus/api/icons/military_tunnels.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/api/icons/mining_outpost.png` & `rustplus-5.6.9/rustplus/api/icons/mining_outpost.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/api/icons/outpost.png` & `rustplus-5.6.9/rustplus/api/icons/outpost.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/api/icons/oxums.png` & `rustplus-5.6.9/rustplus/api/icons/oxums.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/api/icons/patrol.png` & `rustplus-5.6.9/rustplus/api/icons/patrol.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/api/icons/power_plant.png` & `rustplus-5.6.9/rustplus/api/icons/power_plant.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/api/icons/quarry.png` & `rustplus-5.6.9/rustplus/api/icons/quarry.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/api/icons/satellite.png` & `rustplus-5.6.9/rustplus/api/icons/satellite.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/api/icons/sewer.png` & `rustplus-5.6.9/rustplus/api/icons/sewer.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/api/icons/small_oil_rig.png` & `rustplus-5.6.9/rustplus/api/icons/small_oil_rig.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/api/icons/stable.png` & `rustplus-5.6.9/rustplus/api/icons/stable.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/api/icons/supermarket.png` & `rustplus-5.6.9/rustplus/api/icons/supermarket.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/api/icons/swamp.png` & `rustplus-5.6.9/rustplus/api/icons/swamp.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/api/icons/train.png` & `rustplus-5.6.9/rustplus/api/icons/train.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/api/icons/train_yard.png` & `rustplus-5.6.9/rustplus/api/icons/train_yard.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/api/icons/underwater_lab.png` & `rustplus-5.6.9/rustplus/api/icons/underwater_lab.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/api/icons/vending_machine.png` & `rustplus-5.6.9/rustplus/api/icons/vending_machine.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/api/icons/water_treatment.png` & `rustplus-5.6.9/rustplus/api/icons/water_treatment.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/api/remote/camera/camera_constants.py` & `rustplus-5.6.9/rustplus/api/remote/camera/camera_constants.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/api/remote/camera/camera_manager.py` & `rustplus-5.6.9/rustplus/api/remote/camera/camera_manager.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/api/remote/camera/camera_parser.py` & `rustplus-5.6.9/rustplus/api/remote/camera/camera_parser.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/api/remote/camera/structures.py` & `rustplus-5.6.9/rustplus/api/remote/camera/structures.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/api/remote/events/event_handler.py` & `rustplus-5.6.9/rustplus/api/remote/events/event_handler.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/api/remote/events/event_loop_manager.py` & `rustplus-5.6.9/rustplus/api/remote/events/event_loop_manager.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/api/remote/events/events.py` & `rustplus-5.6.9/rustplus/api/remote/events/events.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/api/remote/events/handler_list.py` & `rustplus-5.6.9/rustplus/api/remote/events/handler_list.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/api/remote/events/map_event_listener.py` & `rustplus-5.6.9/rustplus/api/remote/events/map_event_listener.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/api/remote/events/registered_listener.py` & `rustplus-5.6.9/rustplus/api/remote/events/registered_listener.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/api/remote/expo_bundle_handler.py` & `rustplus-5.6.9/rustplus/api/remote/rplus_version_handler.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/api/remote/fcm_listener.py` & `rustplus-5.6.9/rustplus/api/remote/fcm_listener.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/api/remote/heartbeat.py` & `rustplus-5.6.9/rustplus/api/remote/heartbeat.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/api/remote/ratelimiter.py` & `rustplus-5.6.9/rustplus/api/remote/ratelimiter.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/api/remote/rust_remote_interface.py` & `rustplus-5.6.9/rustplus/api/remote/rust_remote_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import betterproto
 
 from .camera.camera_manager import CameraManager
 from .events import EventLoopManager, EntityEvent, RegisteredListener
 from .rustplus_proto import AppRequest, AppMessage, AppEmpty, AppCameraSubscribe
 from .rustws import RustWebsocket, CONNECTED, PENDING_CONNECTION
 from .ratelimiter import RateLimiter
-from .expo_bundle_handler import MagicValueGrabber
+from .rplus_version_handler import MagicValueGrabber
 from ...utils import ServerID, YieldingEvent
 from ...conversation import ConversationFactory
 from ...commands import CommandHandler
 from ...exceptions import (
     ClientNotConnectedError,
     RequestError,
     SmartDeviceRegistrationError,
```

### Comparing `rustplus-5.6.8/rustplus/api/remote/rustplus_proto/rustplus.py` & `rustplus-5.6.9/rustplus/api/remote/rustplus_proto/rustplus.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/api/remote/rustws.py` & `rustplus-5.6.9/rustplus/api/remote/rustws.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/api/remote/server_checker.py` & `rustplus-5.6.9/rustplus/api/remote/server_checker.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/api/rust_api.py` & `rustplus-5.6.9/rustplus/api/rust_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,24 +196,24 @@
             image = Image.open(BytesIO(game_map.jpg_image))
         except Exception:
             raise ImageError("Invalid bytes for the image")
 
         if not self.use_test_server:
             image = image.crop((500, 500, game_map.height - 500, game_map.width - 500))
 
-        game_map = image.resize((map_size, map_size), Image.ANTIALIAS).convert("RGBA")
+        game_map = image.resize((map_size, map_size), Image.LANCZOS).convert("RGBA")
 
         if add_grid:
             grid = (
                 Image.open(
                     requests.get(
                         f"https://files.rustmaps.com/grids/{map_size}.png", stream=True
                     ).raw
                 )
-                .resize((map_size, map_size), Image.ANTIALIAS)
+                .resize((map_size, map_size), Image.LANCZOS)
                 .convert("RGBA")
             )
 
             game_map.paste(grid, (0, 0), grid)
 
         if add_icons or add_events or add_vending_machines:
             map_markers = (
@@ -273,15 +273,15 @@
                 if add_vending_machines and marker.type == 3:
                     game_map.paste(
                         vending_machine,
                         (int(marker.x) - 50, map_size - int(marker.y) - 50),
                         vending_machine,
                     )
 
-        return game_map.resize((2000, 2000), Image.ANTIALIAS)
+        return game_map.resize((2000, 2000), Image.LANCZOS)
 
     async def get_entity_info(self, eid: int = None) -> RustEntityInfo:
         await self._handle_ratelimit()
 
         if eid is None:
             raise ValueError("EID cannot be None")
```

### Comparing `rustplus-5.6.8/rustplus/api/structures/rust_chat_message.py` & `rustplus-5.6.9/rustplus/api/structures/rust_chat_message.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/api/structures/rust_contents.py` & `rustplus-5.6.9/rustplus/api/structures/rust_contents.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/api/structures/rust_entity_info.py` & `rustplus-5.6.9/rustplus/api/structures/rust_entity_info.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/api/structures/rust_info.py` & `rustplus-5.6.9/rustplus/api/structures/rust_info.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/api/structures/rust_item.py` & `rustplus-5.6.9/rustplus/api/structures/rust_item.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/api/structures/rust_map.py` & `rustplus-5.6.9/rustplus/api/structures/rust_map.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/api/structures/rust_marker.py` & `rustplus-5.6.9/rustplus/api/structures/rust_marker.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/api/structures/rust_team_info.py` & `rustplus-5.6.9/rustplus/api/structures/rust_team_info.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/api/structures/rust_time.py` & `rustplus-5.6.9/rustplus/api/structures/rust_time.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/commands/command.py` & `rustplus-5.6.9/rustplus/commands/command.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/commands/command_data.py` & `rustplus-5.6.9/rustplus/commands/command_data.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/commands/command_handler.py` & `rustplus-5.6.9/rustplus/commands/command_handler.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/conversation/conversation.py` & `rustplus-5.6.9/rustplus/conversation/conversation.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/conversation/conversation_factory.py` & `rustplus-5.6.9/rustplus/conversation/conversation_factory.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/exceptions/exceptions.py` & `rustplus-5.6.9/rustplus/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/utils/deprecated.py` & `rustplus-5.6.9/rustplus/utils/deprecated.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/utils/fonts/PermanentMarker.ttf` & `rustplus-5.6.9/rustplus/utils/fonts/PermanentMarker.ttf`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/utils/grab_items.py` & `rustplus-5.6.9/rustplus/utils/grab_items.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/utils/rust_utils.py` & `rustplus-5.6.9/rustplus/utils/rust_utils.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/utils/server_id.py` & `rustplus-5.6.9/rustplus/utils/server_id.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus/utils/yielding_event.py` & `rustplus-5.6.9/rustplus/utils/yielding_event.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.8/rustplus.egg-info/SOURCES.txt` & `rustplus-5.6.9/rustplus.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -47,18 +47,18 @@
 rustplus/api/icons/swamp.png
 rustplus/api/icons/train.png
 rustplus/api/icons/train_yard.png
 rustplus/api/icons/underwater_lab.png
 rustplus/api/icons/vending_machine.png
 rustplus/api/icons/water_treatment.png
 rustplus/api/remote/__init__.py
-rustplus/api/remote/expo_bundle_handler.py
 rustplus/api/remote/fcm_listener.py
 rustplus/api/remote/heartbeat.py
 rustplus/api/remote/ratelimiter.py
+rustplus/api/remote/rplus_version_handler.py
 rustplus/api/remote/rust_remote_interface.py
 rustplus/api/remote/rustws.py
 rustplus/api/remote/server_checker.py
 rustplus/api/remote/camera/__init__.py
 rustplus/api/remote/camera/camera_constants.py
 rustplus/api/remote/camera/camera_manager.py
 rustplus/api/remote/camera/camera_parser.py
```

### Comparing `rustplus-5.6.8/setup.py` & `rustplus-5.6.9/setup.py`

 * *Files identical despite different names*

