# Comparing `tmp/rustplus-5.5.8.tar.gz` & `tmp/rustplus-5.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rustplus-5.5.8.tar", last modified: Wed Mar 15 22:08:54 2023, max compression
+gzip compressed data, was "rustplus-5.6.0.tar", last modified: Mon May  8 11:11:37 2023, max compression
```

## Comparing `rustplus-5.5.8.tar` & `rustplus-5.6.0.tar`

### file list

```diff
@@ -1,116 +1,120 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 22:08:54.011145 rustplus-5.5.8/
--rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-03-15 22:08:43.000000 rustplus-5.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-03-15 22:08:43.000000 rustplus-5.5.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     2355 2023-03-15 22:08:54.011145 rustplus-5.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2005 2023-03-15 22:08:43.000000 rustplus-5.5.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 22:08:54.003145 rustplus-5.5.8/rustplus/
--rw-r--r--   0 runner    (1001) docker     (122)      775 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 22:08:54.003145 rustplus-5.5.8/rustplus/api/
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    19720 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/base_rust_api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 22:08:54.007145 rustplus-5.5.8/rustplus/api/icons/
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    23598 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/airfield.png
--rw-r--r--   0 runner    (1001) docker     (122)    13944 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/arctic_base.png
--rw-r--r--   0 runner    (1001) docker     (122)     3475 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/bandit.png
--rw-r--r--   0 runner    (1001) docker     (122)    35348 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/barn.png
--rw-r--r--   0 runner    (1001) docker     (122)     2553 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/cargo.png
--rw-r--r--   0 runner    (1001) docker     (122)     2058 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/chinook.png
--rw-r--r--   0 runner    (1001) docker     (122)     4228 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/chinook_blades.png
--rw-r--r--   0 runner    (1001) docker     (122)    23420 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/crate.png
--rw-r--r--   0 runner    (1001) docker     (122)    12339 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/desert_base.png
--rw-r--r--   0 runner    (1001) docker     (122)    34156 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/dome.png
--rw-r--r--   0 runner    (1001) docker     (122)    34662 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/excavator.png
--rw-r--r--   0 runner    (1001) docker     (122)     4934 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/explosion.png
--rw-r--r--   0 runner    (1001) docker     (122)    24176 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/fishing.png
--rw-r--r--   0 runner    (1001) docker     (122)     2882 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/harbour.png
--rw-r--r--   0 runner    (1001) docker     (122)    12195 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/icon.png
--rw-r--r--   0 runner    (1001) docker     (122)    41087 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/junkyard.png
--rw-r--r--   0 runner    (1001) docker     (122)     9091 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/large_oil_rig.png
--rw-r--r--   0 runner    (1001) docker     (122)    23696 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/launchsite.png
--rw-r--r--   0 runner    (1001) docker     (122)    27391 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/lighthouse.png
--rw-r--r--   0 runner    (1001) docker     (122)    23532 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/military_tunnels.png
--rw-r--r--   0 runner    (1001) docker     (122)    27923 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/mining_outpost.png
--rw-r--r--   0 runner    (1001) docker     (122)    30573 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/outpost.png
--rw-r--r--   0 runner    (1001) docker     (122)     2384 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/oxums.png
--rw-r--r--   0 runner    (1001) docker     (122)     2742 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/patrol.png
--rw-r--r--   0 runner    (1001) docker     (122)    23513 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/power_plant.png
--rw-r--r--   0 runner    (1001) docker     (122)    36433 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/quarry.png
--rw-r--r--   0 runner    (1001) docker     (122)    28365 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/satellite.png
--rw-r--r--   0 runner    (1001) docker     (122)    17804 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/sewer.png
--rw-r--r--   0 runner    (1001) docker     (122)     8114 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/small_oil_rig.png
--rw-r--r--   0 runner    (1001) docker     (122)    30710 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/stable.png
--rw-r--r--   0 runner    (1001) docker     (122)    28458 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/supermarket.png
--rw-r--r--   0 runner    (1001) docker     (122)     2049 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/swamp.png
--rw-r--r--   0 runner    (1001) docker     (122)     5300 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/train.png
--rw-r--r--   0 runner    (1001) docker     (122)    20587 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/train_yard.png
--rw-r--r--   0 runner    (1001) docker     (122)     3066 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/underwater_lab.png
--rw-r--r--   0 runner    (1001) docker     (122)     5705 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/vending_machine.png
--rw-r--r--   0 runner    (1001) docker     (122)    23907 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/water_treatment.png
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 22:08:54.007145 rustplus-5.5.8/rustplus/api/remote/
--rw-r--r--   0 runner    (1001) docker     (122)      341 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/remote/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 22:08:54.007145 rustplus-5.5.8/rustplus/api/remote/camera/
--rw-r--r--   0 runner    (1001) docker     (122)      147 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/remote/camera/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   118649 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/remote/camera/camera_constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     3629 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/remote/camera/camera_manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     6029 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/remote/camera/camera_parser.py
--rw-r--r--   0 runner    (1001) docker     (122)     2479 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/remote/camera/structures.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 22:08:54.007145 rustplus-5.5.8/rustplus/api/remote/events/
--rw-r--r--   0 runner    (1001) docker     (122)      183 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/remote/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2141 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/remote/events/event_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)      684 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/remote/events/event_loop_manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     3195 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/remote/events/events.py
--rw-r--r--   0 runner    (1001) docker     (122)     2286 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/remote/events/handler_list.py
--rw-r--r--   0 runner    (1001) docker     (122)     3105 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/remote/events/map_event_listener.py
--rw-r--r--   0 runner    (1001) docker     (122)      738 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/remote/events/registered_listener.py
--rw-r--r--   0 runner    (1001) docker     (122)     1841 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/remote/expo_bundle_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)      665 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/remote/fcm_listener.py
--rw-r--r--   0 runner    (1001) docker     (122)      806 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/remote/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (122)     4123 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/remote/ratelimiter.py
--rw-r--r--   0 runner    (1001) docker     (122)     8293 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/remote/rust_remote_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 22:08:54.007145 rustplus-5.5.8/rustplus/api/remote/rustplus_proto/
--rw-r--r--   0 runner    (1001) docker     (122)     3946 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/remote/rustplus_proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    18568 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/remote/rustplus_proto/rustplus_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)    11412 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/remote/rustws.py
--rw-r--r--   0 runner    (1001) docker     (122)      781 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/remote/server_checker.py
--rw-r--r--   0 runner    (1001) docker     (122)    13311 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/rust_api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 22:08:54.007145 rustplus-5.5.8/rustplus/api/structures/
--rw-r--r--   0 runner    (1001) docker     (122)      390 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      824 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/structures/rust_chat_message.py
--rw-r--r--   0 runner    (1001) docker     (122)      852 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/structures/rust_contents.py
--rw-r--r--   0 runner    (1001) docker     (122)     1948 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/structures/rust_entity_info.py
--rw-r--r--   0 runner    (1001) docker     (122)     1943 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/structures/rust_info.py
--rw-r--r--   0 runner    (1001) docker     (122)      780 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/structures/rust_item.py
--rw-r--r--   0 runner    (1001) docker     (122)     1759 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/structures/rust_map.py
--rw-r--r--   0 runner    (1001) docker     (122)     4676 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/structures/rust_marker.py
--rw-r--r--   0 runner    (1001) docker     (122)     2864 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/structures/rust_team_info.py
--rw-r--r--   0 runner    (1001) docker     (122)     1110 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/structures/rust_time.py
--rw-r--r--   0 runner    (1001) docker     (122)       93 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/structures/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 22:08:54.007145 rustplus-5.5.8/rustplus/commands/
--rw-r--r--   0 runner    (1001) docker     (122)      130 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      542 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/commands/command.py
--rw-r--r--   0 runner    (1001) docker     (122)      522 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/commands/command_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     2963 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/commands/command_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)      445 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/commands/command_options.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 22:08:54.011145 rustplus-5.5.8/rustplus/conversation/
--rw-r--r--   0 runner    (1001) docker     (122)      145 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/conversation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1882 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/conversation/conversation.py
--rw-r--r--   0 runner    (1001) docker     (122)     1551 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/conversation/conversation_factory.py
--rw-r--r--   0 runner    (1001) docker     (122)      289 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/conversation/conversation_prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 22:08:54.011145 rustplus-5.5.8/rustplus/exceptions/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1158 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 22:08:54.011145 rustplus-5.5.8/rustplus/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      139 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      925 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/utils/deprecated.py
--rw-r--r--   0 runner    (1001) docker     (122)    26442 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/utils/grab_items.py
--rw-r--r--   0 runner    (1001) docker     (122)     5322 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/utils/rust_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      752 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/utils/server_id.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 22:08:54.003145 rustplus-5.5.8/rustplus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2355 2023-03-15 22:08:53.000000 rustplus-5.5.8/rustplus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3433 2023-03-15 22:08:53.000000 rustplus-5.5.8/rustplus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-15 22:08:53.000000 rustplus-5.5.8/rustplus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       95 2023-03-15 22:08:53.000000 rustplus-5.5.8/rustplus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-03-15 22:08:53.000000 rustplus-5.5.8/rustplus.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-03-15 22:08:54.011145 rustplus-5.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1081 2023-03-15 22:08:43.000000 rustplus-5.5.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 11:11:37.582576 rustplus-5.6.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-05-08 11:11:28.000000 rustplus-5.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-05-08 11:11:28.000000 rustplus-5.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2355 2023-05-08 11:11:37.582576 rustplus-5.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2005 2023-05-08 11:11:28.000000 rustplus-5.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 11:11:37.574576 rustplus-5.6.0/rustplus/
+-rw-r--r--   0 runner    (1001) docker     (122)      775 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 11:11:37.574576 rustplus-5.6.0/rustplus/api/
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19850 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/base_rust_api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 11:11:37.578576 rustplus-5.6.0/rustplus/api/icons/
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/icons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23598 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/icons/airfield.png
+-rw-r--r--   0 runner    (1001) docker     (122)    13944 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/icons/arctic_base.png
+-rw-r--r--   0 runner    (1001) docker     (122)     3475 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/icons/bandit.png
+-rw-r--r--   0 runner    (1001) docker     (122)    35348 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/icons/barn.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2553 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/icons/cargo.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2058 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/icons/chinook.png
+-rw-r--r--   0 runner    (1001) docker     (122)     4228 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/icons/chinook_blades.png
+-rw-r--r--   0 runner    (1001) docker     (122)    23420 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/icons/crate.png
+-rw-r--r--   0 runner    (1001) docker     (122)    12339 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/icons/desert_base.png
+-rw-r--r--   0 runner    (1001) docker     (122)    34156 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/icons/dome.png
+-rw-r--r--   0 runner    (1001) docker     (122)    34662 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/icons/excavator.png
+-rw-r--r--   0 runner    (1001) docker     (122)     4934 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/icons/explosion.png
+-rw-r--r--   0 runner    (1001) docker     (122)    24176 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/icons/fishing.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2882 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/icons/harbour.png
+-rw-r--r--   0 runner    (1001) docker     (122)    12195 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/icons/icon.png
+-rw-r--r--   0 runner    (1001) docker     (122)    41087 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/icons/junkyard.png
+-rw-r--r--   0 runner    (1001) docker     (122)     9091 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/icons/large_oil_rig.png
+-rw-r--r--   0 runner    (1001) docker     (122)    23696 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/icons/launchsite.png
+-rw-r--r--   0 runner    (1001) docker     (122)    27391 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/icons/lighthouse.png
+-rw-r--r--   0 runner    (1001) docker     (122)    23532 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/icons/military_tunnels.png
+-rw-r--r--   0 runner    (1001) docker     (122)    27923 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/icons/mining_outpost.png
+-rw-r--r--   0 runner    (1001) docker     (122)    30573 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/icons/outpost.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2384 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/icons/oxums.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2742 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/icons/patrol.png
+-rw-r--r--   0 runner    (1001) docker     (122)    23513 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/icons/power_plant.png
+-rw-r--r--   0 runner    (1001) docker     (122)    36433 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/icons/quarry.png
+-rw-r--r--   0 runner    (1001) docker     (122)    28365 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/icons/satellite.png
+-rw-r--r--   0 runner    (1001) docker     (122)    17804 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/icons/sewer.png
+-rw-r--r--   0 runner    (1001) docker     (122)     8114 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/icons/small_oil_rig.png
+-rw-r--r--   0 runner    (1001) docker     (122)    30710 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/icons/stable.png
+-rw-r--r--   0 runner    (1001) docker     (122)    28458 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/icons/supermarket.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2049 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/icons/swamp.png
+-rw-r--r--   0 runner    (1001) docker     (122)     5300 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/icons/train.png
+-rw-r--r--   0 runner    (1001) docker     (122)    20587 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/icons/train_yard.png
+-rw-r--r--   0 runner    (1001) docker     (122)     3066 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/icons/underwater_lab.png
+-rw-r--r--   0 runner    (1001) docker     (122)     5705 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/icons/vending_machine.png
+-rw-r--r--   0 runner    (1001) docker     (122)    23907 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/icons/water_treatment.png
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 11:11:37.578576 rustplus-5.6.0/rustplus/api/remote/
+-rw-r--r--   0 runner    (1001) docker     (122)      341 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/remote/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 11:11:37.578576 rustplus-5.6.0/rustplus/api/remote/camera/
+-rw-r--r--   0 runner    (1001) docker     (122)      147 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/remote/camera/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   118649 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/remote/camera/camera_constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5711 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/remote/camera/camera_manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24243 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/remote/camera/camera_parser.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3354 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/remote/camera/structures.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 11:11:37.582576 rustplus-5.6.0/rustplus/api/remote/events/
+-rw-r--r--   0 runner    (1001) docker     (122)      223 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/remote/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1660 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/remote/events/event_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)      751 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/remote/events/event_loop_manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3325 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/remote/events/events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2285 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/remote/events/handler_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3101 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/remote/events/map_event_listener.py
+-rw-r--r--   0 runner    (1001) docker     (122)      776 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/remote/events/registered_listener.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1840 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/remote/expo_bundle_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)      664 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/remote/fcm_listener.py
+-rw-r--r--   0 runner    (1001) docker     (122)      799 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/remote/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4114 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/remote/ratelimiter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8086 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/remote/rust_remote_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 11:11:37.582576 rustplus-5.6.0/rustplus/api/remote/rustplus_proto/
+-rw-r--r--   0 runner    (1001) docker     (122)       24 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/remote/rustplus_proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16092 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/remote/rustplus_proto/rustplus.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11295 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/remote/rustws.py
+-rw-r--r--   0 runner    (1001) docker     (122)      892 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/remote/server_checker.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13801 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/rust_api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 11:11:37.582576 rustplus-5.6.0/rustplus/api/structures/
+-rw-r--r--   0 runner    (1001) docker     (122)      390 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      894 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/structures/rust_chat_message.py
+-rw-r--r--   0 runner    (1001) docker     (122)      852 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/structures/rust_contents.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2048 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/structures/rust_entity_info.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2004 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/structures/rust_info.py
+-rw-r--r--   0 runner    (1001) docker     (122)      824 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/structures/rust_item.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1813 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/structures/rust_map.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4805 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/structures/rust_marker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3008 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/structures/rust_team_info.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1110 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/structures/rust_time.py
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/api/structures/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 11:11:37.582576 rustplus-5.6.0/rustplus/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)      130 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      542 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/commands/command.py
+-rw-r--r--   0 runner    (1001) docker     (122)      522 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/commands/command_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2435 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/commands/command_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)      444 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/commands/command_options.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 11:11:37.582576 rustplus-5.6.0/rustplus/conversation/
+-rw-r--r--   0 runner    (1001) docker     (122)      145 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/conversation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1885 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/conversation/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1550 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/conversation/conversation_factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)      289 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/conversation/conversation_prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 11:11:37.582576 rustplus-5.6.0/rustplus/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1158 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 11:11:37.582576 rustplus-5.6.0/rustplus/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      181 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      924 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/utils/deprecated.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 11:11:37.582576 rustplus-5.6.0/rustplus/utils/fonts/
+-rw-r--r--   0 runner    (1001) docker     (122)    74752 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/utils/fonts/PermanentMarker.ttf
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/utils/fonts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26480 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/utils/grab_items.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5388 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/utils/rust_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      752 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/utils/server_id.py
+-rw-r--r--   0 runner    (1001) docker     (122)      770 2023-05-08 11:11:28.000000 rustplus-5.6.0/rustplus/utils/yielding_event.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 11:11:37.574576 rustplus-5.6.0/rustplus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2355 2023-05-08 11:11:37.000000 rustplus-5.6.0/rustplus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3536 2023-05-08 11:11:37.000000 rustplus-5.6.0/rustplus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-08 11:11:37.000000 rustplus-5.6.0/rustplus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       96 2023-05-08 11:11:37.000000 rustplus-5.6.0/rustplus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-08 11:11:37.000000 rustplus-5.6.0/rustplus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-05-08 11:11:37.586577 rustplus-5.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-05-08 11:11:28.000000 rustplus-5.6.0/setup.py
```

### Comparing `rustplus-5.5.8/LICENSE` & `rustplus-5.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.8/PKG-INFO` & `rustplus-5.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rustplus
-Version: 5.5.8
+Version: 5.6.0
 Summary: A python wrapper for the Rust Plus API
 Home-page: https://github.com/olijeffers0n/rustplus
 Author: olijeffers0n
 License: MIT
 Project-URL: Issue tracker, https://github.com/olijeffers0n/rustplus/issues
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
```

### Comparing `rustplus-5.5.8/README.md` & `rustplus-5.6.0/README.md`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.8/rustplus/__init__.py` & `rustplus-5.6.0/rustplus/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,9 +18,9 @@
 from .commands import CommandOptions, Command
 from .exceptions import *
 from .conversation import ConversationFactory, Conversation, ConversationPrompt
 from .utils import *
 
 __name__ = "rustplus"
 __author__ = "olijeffers0n"
-__version__ = "5.5.8"
+__version__ = "5.6.0"
 __support__ = "Discord: https://discord.gg/nQqJe8qvP8"
```

### Comparing `rustplus-5.5.8/rustplus/api/base_rust_api.py` & `rustplus-5.6.0/rustplus/api/base_rust_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,14 @@
         ratelimit_refill: int = 3,
         heartbeat: HeartBeat = None,
         use_proxy: bool = False,
         use_test_server: bool = False,
         event_loop: asyncio.AbstractEventLoop = None,
         rate_limiter: RateLimiter = None,
     ) -> None:
-
         if ip is None:
             raise ValueError("Ip cannot be None")
         if steam_id is None:
             raise ValueError("SteamID cannot be None")
         if player_token is None:
             raise ValueError("PlayerToken cannot be None")
 
@@ -76,38 +75,37 @@
         """
         Handles the ratelimit for a specific request. Will sleep if tokens are not currently available and is set to wait
         :param amount: The amount to consume
         :raises RateLimitError - If the tokens are not available and is not set to wait
         :return: None
         """
         while True:
-
-            if self.remote.ratelimiter.can_consume(self.server_id, amount):
-                self.remote.ratelimiter.consume(self.server_id, amount)
+            if await self.remote.ratelimiter.can_consume(self.server_id, amount):
+                await self.remote.ratelimiter.consume(self.server_id, amount)
                 break
 
             if self.raise_ratelimit_exception:
                 raise RateLimitError("Out of tokens")
 
             await asyncio.sleep(
-                self.remote.ratelimiter.get_estimated_delay_time(self.server_id, amount)
+                await self.remote.ratelimiter.get_estimated_delay_time(self.server_id, amount)
             )
 
         self.heartbeat.reset_rhythm()
 
     def _generate_protobuf(self) -> AppRequest:
         """
         Generates the default protobuf for a request
 
         :return: AppRequest - The default request object
         """
         app_request = AppRequest()
         app_request.seq = self.seq
-        app_request.playerId = self.server_id.player_id
-        app_request.playerToken = self.server_id.player_token
+        app_request.player_id = self.server_id.player_id
+        app_request.player_token = self.server_id.player_token
 
         self.seq += 1
 
         return app_request
 
     async def connect(
         self, retries: int = float("inf"), delay: int = 20, on_failure=None
@@ -147,15 +145,15 @@
 
     async def close_connection(self) -> None:
         """
         Disconnects from the Rust Server
 
         :return: None
         """
-        self.remote.close()
+        await self.remote.close()
 
     async def disconnect(self) -> None:
         """
         Disconnects from the Rust Server
 
         :return: None
         """
@@ -166,17 +164,18 @@
         Sends a request to the server to wake up broadcast responses
 
         :return: None
         """
         await self._handle_ratelimit()
 
         app_request = self._generate_protobuf()
-        app_request.getTime.CopyFrom(AppEmpty())
+        app_request.get_time = AppEmpty()
+        app_request.get_time._serialized_on_wire = True
 
-        self.remote.ignored_responses.append(app_request.seq)
+        await self.remote.add_ignored_response(app_request.seq)
 
         await self.remote.send_message(app_request)
 
     async def switch_server(
         self,
         ip: str = None,
         port: str = None,
@@ -233,15 +232,16 @@
 
         self.raise_ratelimit_exception = raise_ratelimit_exception
 
         self.remote.pending_entity_subscriptions = []
         self.remote.server_id = ServerID(ip, port, steam_id, player_token)
 
         # reset ratelimiter
-        self.remote.ratelimiter.remove(self.server_id)
+        self.remote.use_proxy = use_proxy
+        await self.remote.ratelimiter.remove(self.server_id)
         self.remote.ratelimiter.add_socket(
             self.server_id,
             self.ratelimit_limit,
             self.ratelimit_limit,
             1,
             self.ratelimit_refill,
         )
@@ -279,15 +279,14 @@
                 aliases,
                 alias_func,
             )
             self.remote.command_handler.register_command(cmd_data)
             return RegisteredListener(coro.__name__, cmd_data.coro)
 
         def wrap_func(coro):
-
             if self.command_options is None:
                 raise CommandsNotEnabledError("Not enabled")
 
             if isinstance(coro, RegisteredListener):
                 coro = coro.get_coro()
 
             cmd_data = CommandData(
@@ -336,15 +335,14 @@
 
         :param eid: The entity id of the entity
         :return: RegisteredListener - The listener object
         :raises SmartDeviceRegistrationError
         """
 
         def wrap_func(coro) -> RegisteredListener:
-
             if isinstance(coro, RegisteredListener):
                 coro = coro.get_coro()
 
             self.remote.handle_subscribing_entity(eid, coro)
 
             return RegisteredListener(eid, coro)
 
@@ -583,18 +581,18 @@
     ) -> RustContents:
         """
         Gets the Information about TC Upkeep and Contents.
         Do not use this for any other storage monitor than a TC
         """
         raise NotImplementedError("Not Implemented")
 
-    async def get_camera_manager(self, id: str) -> CameraManager:
+    async def get_camera_manager(self, cam_id: str) -> CameraManager:
         """
         Gets a camera manager for a given camera ID
 
         NOTE: This will override the current camera manager if one exists for the given ID so you cannot have multiple
 
-        :param id: The ID of the camera
+        :param cam_id: The ID of the camera
         :return CameraManager: The camera manager
-        :raises RequestError: If the camera is not found or you cannot access it. See reason for more info
+        :raises RequestError: If the camera is not found, or you cannot access it. See reason for more info
         """
         raise NotImplementedError("Not Implemented")
```

### Comparing `rustplus-5.5.8/rustplus/api/icons/airfield.png` & `rustplus-5.6.0/rustplus/api/icons/airfield.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.8/rustplus/api/icons/arctic_base.png` & `rustplus-5.6.0/rustplus/api/icons/arctic_base.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.8/rustplus/api/icons/bandit.png` & `rustplus-5.6.0/rustplus/api/icons/bandit.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.8/rustplus/api/icons/barn.png` & `rustplus-5.6.0/rustplus/api/icons/barn.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.8/rustplus/api/icons/cargo.png` & `rustplus-5.6.0/rustplus/api/icons/cargo.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.8/rustplus/api/icons/chinook.png` & `rustplus-5.6.0/rustplus/api/icons/chinook.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.8/rustplus/api/icons/chinook_blades.png` & `rustplus-5.6.0/rustplus/api/icons/chinook_blades.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.8/rustplus/api/icons/crate.png` & `rustplus-5.6.0/rustplus/api/icons/crate.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.8/rustplus/api/icons/desert_base.png` & `rustplus-5.6.0/rustplus/api/icons/desert_base.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.8/rustplus/api/icons/dome.png` & `rustplus-5.6.0/rustplus/api/icons/dome.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.8/rustplus/api/icons/excavator.png` & `rustplus-5.6.0/rustplus/api/icons/excavator.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.8/rustplus/api/icons/explosion.png` & `rustplus-5.6.0/rustplus/api/icons/explosion.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.8/rustplus/api/icons/fishing.png` & `rustplus-5.6.0/rustplus/api/icons/fishing.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.8/rustplus/api/icons/harbour.png` & `rustplus-5.6.0/rustplus/api/icons/harbour.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.8/rustplus/api/icons/icon.png` & `rustplus-5.6.0/rustplus/api/icons/icon.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.8/rustplus/api/icons/junkyard.png` & `rustplus-5.6.0/rustplus/api/icons/junkyard.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.8/rustplus/api/icons/large_oil_rig.png` & `rustplus-5.6.0/rustplus/api/icons/large_oil_rig.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.8/rustplus/api/icons/launchsite.png` & `rustplus-5.6.0/rustplus/api/icons/launchsite.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.8/rustplus/api/icons/lighthouse.png` & `rustplus-5.6.0/rustplus/api/icons/lighthouse.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.8/rustplus/api/icons/military_tunnels.png` & `rustplus-5.6.0/rustplus/api/icons/military_tunnels.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.8/rustplus/api/icons/mining_outpost.png` & `rustplus-5.6.0/rustplus/api/icons/mining_outpost.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.8/rustplus/api/icons/outpost.png` & `rustplus-5.6.0/rustplus/api/icons/outpost.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.8/rustplus/api/icons/oxums.png` & `rustplus-5.6.0/rustplus/api/icons/oxums.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.8/rustplus/api/icons/patrol.png` & `rustplus-5.6.0/rustplus/api/icons/patrol.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.8/rustplus/api/icons/power_plant.png` & `rustplus-5.6.0/rustplus/api/icons/power_plant.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.8/rustplus/api/icons/quarry.png` & `rustplus-5.6.0/rustplus/api/icons/quarry.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.8/rustplus/api/icons/satellite.png` & `rustplus-5.6.0/rustplus/api/icons/satellite.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.8/rustplus/api/icons/sewer.png` & `rustplus-5.6.0/rustplus/api/icons/sewer.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.8/rustplus/api/icons/small_oil_rig.png` & `rustplus-5.6.0/rustplus/api/icons/small_oil_rig.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.8/rustplus/api/icons/stable.png` & `rustplus-5.6.0/rustplus/api/icons/stable.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.8/rustplus/api/icons/supermarket.png` & `rustplus-5.6.0/rustplus/api/icons/supermarket.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.8/rustplus/api/icons/swamp.png` & `rustplus-5.6.0/rustplus/api/icons/swamp.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.8/rustplus/api/icons/train.png` & `rustplus-5.6.0/rustplus/api/icons/train.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.8/rustplus/api/icons/train_yard.png` & `rustplus-5.6.0/rustplus/api/icons/train_yard.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.8/rustplus/api/icons/underwater_lab.png` & `rustplus-5.6.0/rustplus/api/icons/underwater_lab.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.8/rustplus/api/icons/vending_machine.png` & `rustplus-5.6.0/rustplus/api/icons/vending_machine.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.8/rustplus/api/icons/water_treatment.png` & `rustplus-5.6.0/rustplus/api/icons/water_treatment.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.8/rustplus/api/remote/camera/camera_constants.py` & `rustplus-5.6.0/rustplus/api/remote/camera/camera_constants.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.8/rustplus/api/remote/camera/structures.py` & `rustplus-5.6.0/rustplus/api/remote/camera/structures.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,73 @@
 from typing import Any
 
+from ..rustplus_proto import AppCameraInfo, AppCameraRaysEntity, AppCameraRays
+
 
 class CameraInfo:
-    def __init__(self, camera_info_message) -> None:
-        self.width = camera_info_message.width
-        self.height = camera_info_message.height
-        self.near_plane = camera_info_message.nearPlane
-        self.far_plane = camera_info_message.farPlane
-        self.control_flags = camera_info_message.controlFlags
+    def __init__(self, camera_info_message: AppCameraInfo) -> None:
+        self.width: int = camera_info_message.width
+        self.height: int = camera_info_message.height
+        self.near_plane: float = camera_info_message.near_plane
+        self.far_plane: float = camera_info_message.far_plane
+        self.control_flags: int = camera_info_message.control_flags
 
     def is_move_option_permissible(self, value: int) -> bool:
         return self.control_flags & value == value
 
     def __str__(self) -> str:
         return (
             f"CameraInfo(width={self.width}, height={self.height}, near_plane={self.near_plane}, "
             f"far_plane={self.far_plane}, control_flags={self.control_flags})"
         )
 
 
 class Entity:
-    def __init__(self, entity_data) -> None:
-        self.entity_id = entity_data.entityId
-        self.type = entity_data.type
-        self.position = entity_data.position
-        self.rotation = entity_data.rotation
-        self.size = entity_data.size
+    def __init__(self, entity_data: AppCameraRaysEntity) -> None:
+        self.entity_id: int = entity_data.entity_id
+        self.type: int = entity_data.type
+        self.position: Vector3 = Vector3(entity_data.position)
+        self.rotation: Vector3 = Vector3(entity_data.rotation)
+        self.size: Vector3 = Vector3(entity_data.size)
         self.name: str = entity_data.name
 
     def __str__(self) -> str:
         return (
             f"Entity(entity_id={self.entity_id}, type={self.type}, position={self.position}, "
             f"rotation={self.rotation}, size={self.size}, name={self.name})"
         )
 
+    def __repr__(self):
+        return self.__str__()
+
+
+class Vector3:
+    def __init__(self, vector3=None, x=None, y=None, z=None) -> None:
+        self.x: float = vector3.x if x is None else x
+        self.y: float = vector3.y if y is None else y
+        self.z: float = vector3.z if z is None else z
+
+    def __eq__(self, other):
+        if not isinstance(other, Vector3):
+            return False
+
+        return self.x == other.x and self.y == other.y and self.z == other.z
+
+    def __hash__(self):
+        return hash((self.x, self.y, self.z))
+
+    def __str__(self) -> str:
+        return f"Vector3(x={self.x}, y={self.y}, z={self.z})"
+
 
 class RayPacket:
-    def __init__(self, ray_packet) -> None:
-        self.vertical_fov = ray_packet.verticalFov
-        self.sample_offset = ray_packet.sampleOffset
-        self.ray_data = ray_packet.rayData
+    def __init__(self, ray_packet: AppCameraRays) -> None:
+        self.vertical_fov = ray_packet.vertical_fov
+        self.sample_offset = ray_packet.sample_offset
+        self.ray_data = ray_packet.ray_data
         self.distance = ray_packet.distance
         self.entities = [Entity(data) for data in ray_packet.entities]
 
     def __str__(self) -> str:
         return (
             f"RayPacket(vertical_fov={self.vertical_fov}, sample_offset={self.sample_offset}, "
             f"ray_data={self.ray_data}, distance={self.distance}, entities={self.entities})"
```

### Comparing `rustplus-5.5.8/rustplus/api/remote/events/events.py` & `rustplus-5.6.0/rustplus/api/remote/events/events.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from typing import List
 
+from ..rustplus_proto import AppMessage, AppEntityPayloadItem
 from ...structures import RustChatMessage
 from ...structures.rust_team_info import RustTeamInfo
 from ...structures.rust_marker import RustMarker
 from .handler_list import HandlerList, EntityHandlerList
 
 
 class Item:
-    def __init__(self, app_message) -> None:
-        self._item_id: int = app_message.itemId
+    def __init__(self, app_message: AppEntityPayloadItem) -> None:
+        self._item_id: int = app_message.item_id
         self._quantity: int = app_message.quantity
-        self._item_is_blueprint: bool = app_message.itemIsBlueprint
+        self._item_is_blueprint: bool = app_message.item_is_blueprint
 
     @property
     def item_id(self) -> int:
         return self._item_id
 
     @property
     def quantity(self) -> int:
@@ -22,60 +23,57 @@
 
     @property
     def item_is_blueprint(self) -> bool:
         return self._item_is_blueprint
 
 
 class TeamEvent:
-
     handlers = HandlerList()
 
-    def __init__(self, app_message) -> None:
-        self._player_id: int = app_message.broadcast.teamChanged.playerId
-        self._team_info = RustTeamInfo(app_message.broadcast.teamChanged.teamInfo)
+    def __init__(self, app_message: AppMessage) -> None:
+        self._player_id: int = app_message.broadcast.team_changed.player_id
+        self._team_info = RustTeamInfo(app_message.broadcast.team_changed.team_info)
 
     @property
     def player_id(self) -> int:
         return self._player_id
 
     @property
     def team_info(self) -> RustTeamInfo:
         return self._team_info
 
 
 class ChatEvent:
-
     handlers = HandlerList()
 
-    def __init__(self, app_message) -> None:
-        self._message = RustChatMessage(app_message.broadcast.newTeamMessage.message)
+    def __init__(self, app_message: AppMessage) -> None:
+        self._message = RustChatMessage(app_message.broadcast.team_message.message)
 
     @property
     def message(self) -> RustChatMessage:
         return self._message
 
 
 class EntityEvent:
-
     handlers = EntityHandlerList()
 
-    def __init__(self, app_message, entity_type) -> None:
+    def __init__(self, app_message: AppMessage, entity_type) -> None:
         self._type = int(entity_type)
-        self._entity_id: int = app_message.broadcast.entityChanged.entityId
-        self._value: bool = app_message.broadcast.entityChanged.payload.value
-        self._capacity: int = app_message.broadcast.entityChanged.payload.capacity
+        self._entity_id: int = app_message.broadcast.entity_changed.entity_id
+        self._value: bool = app_message.broadcast.entity_changed.payload.value
+        self._capacity: int = app_message.broadcast.entity_changed.payload.capacity
         self._has_protection: bool = (
-            app_message.broadcast.entityChanged.payload.hasProtection
+            app_message.broadcast.entity_changed.payload.has_protection
         )
         self._protection_expiry: int = (
-            app_message.broadcast.entityChanged.payload.protectionExpiry
+            app_message.broadcast.entity_changed.payload.protection_expiry
         )
 
         self._items: List[Item] = [
-            Item(item) for item in app_message.broadcast.entityChanged.payload.items
+            Item(item) for item in app_message.broadcast.entity_changed.payload.items
         ]
 
     @property
     def type(self) -> int:
         return self._type
 
     @property
@@ -114,15 +112,14 @@
 
     @property
     def is_new(self) -> bool:
         return self._is_new
 
 
 class ProtobufEvent:
-
     handlers = HandlerList()
 
     def __init__(self, byte_data) -> None:
         self._byte_data = byte_data
 
     @property
     def byte_data(self) -> bytes:
```

### Comparing `rustplus-5.5.8/rustplus/api/remote/events/handler_list.py` & `rustplus-5.6.0/rustplus/api/remote/events/handler_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,14 @@
         ] = defaultdict(dict)
 
     def unregister(self, listener: RegisteredListener, server_id: ServerID) -> None:
         if listener.listener_id in self._handlers.get(server_id):
             self._handlers.get(server_id).get(listener.listener_id).remove(listener)
 
     def register(self, listener: RegisteredListener, server_id: ServerID) -> None:
-
         if server_id not in self._handlers:
             self._handlers[server_id] = defaultdict(set)
 
         if listener.listener_id not in self._handlers.get(server_id):
             self._handlers.get(server_id)[listener.listener_id] = set()
 
         self._handlers.get(server_id).get(listener.listener_id).add(listener)
```

### Comparing `rustplus-5.5.8/rustplus/api/remote/events/map_event_listener.py` & `rustplus-5.6.0/rustplus/api/remote/events/map_event_listener.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,26 +32,22 @@
             target=self._run, daemon=True, name="MapEventListener"
         )
         self.thread.start()
         self.gc = IDGarbageCollector(self.persistent_ids)
         self.gc.start()
 
     def _run(self) -> None:
-
         while True:
-
             try:
-
                 future = asyncio.run_coroutine_threadsafe(
                     self.api.get_markers(),
                     EventLoopManager.get_loop(self.api.server_id),
                 )
                 new_highest_id = 0
                 for marker in future.result():
-
                     new = False
 
                     if marker.id in self.persistent_ids:
                         self.call_event(marker, new)
                         continue
 
                     if marker.id > self.highest_id:
```

### Comparing `rustplus-5.5.8/rustplus/api/remote/events/registered_listener.py` & `rustplus-5.6.0/rustplus/api/remote/events/registered_listener.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,22 @@
+from typing import Union
+
+
 class RegisteredListener:
-    def __init__(self, listener_id: str, data) -> None:
+    def __init__(self, listener_id: Union[str, int], data) -> None:
         self.listener_id = str(listener_id)
         self.data = data
 
     def get_coro(self):
         if isinstance(self.data, tuple):
             return self.data[0]
         return self.data
 
     def __eq__(self, other) -> bool:
         if isinstance(other, RegisteredListener):
-
             coro = self.data
             if isinstance(self.data, tuple):
                 coro = self.data[0]
 
             return self.listener_id == other.listener_id and coro == coro
         return False
```

### Comparing `rustplus-5.5.8/rustplus/api/remote/expo_bundle_handler.py` & `rustplus-5.6.0/rustplus/api/remote/expo_bundle_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import json
 from datetime import datetime
 
 
 class MagicValueGrabber:
     @staticmethod
     def get_magic_value() -> int:
-
         try:
             data = requests.get(
                 "https://exp.host/@facepunch/RustCompanion",
                 headers={
                     "Exponent-SDK-Version": "40.0.0",  # These are the two lines that determine the version of data that
                     "Exponent-Version": "0.0.29",  # you receive as far as I can tell from my limited debugging. As of
                     # now (8th April 2022), this is the latest
```

### Comparing `rustplus-5.5.8/rustplus/api/remote/fcm_listener.py` & `rustplus-5.6.0/rustplus/api/remote/fcm_listener.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,12 +11,11 @@
     def on_notification(self, obj, notification, data_message) -> None:
         pass
 
     def start(self, daemon=False) -> None:
         self.thread = Thread(target=self.__fcm_listen, daemon=daemon).start()
 
     def __fcm_listen(self) -> None:
-
         if self.data is None:
             raise ValueError("Data is None")
 
         self._push_listener.listen(callback=self.on_notification)
```

### Comparing `rustplus-5.5.8/rustplus/api/remote/heartbeat.py` & `rustplus-5.6.0/rustplus/api/remote/heartbeat.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,32 @@
 import asyncio
 import time
 
 
 class HeartBeat:
     def __init__(self, rust_api) -> None:
-
         self.rust_api = rust_api
         self.next_run = time.time()
         self.running = False
 
     async def start_beat(self) -> None:
-
         if self.running:
             return
 
         self.running = True
 
         asyncio.create_task(self._heart_beat())
 
     async def _heart_beat(self) -> None:
-
         while True:
-
             if time.time() >= self.next_run:
-
                 await self.beat()
 
             else:
                 await asyncio.sleep(1)
 
     async def beat(self) -> None:
-
         if self.rust_api.remote.ws is not None and self.rust_api.remote.is_open():
             await self.rust_api.send_wakeup_request()
 
     def reset_rhythm(self) -> None:
-
         self.next_run = time.time() + 240
```

### Comparing `rustplus-5.5.8/rustplus/api/remote/ratelimiter.py` & `rustplus-5.6.0/rustplus/api/remote/ratelimiter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import math
 import time
-import threading
+import asyncio
 from typing import Dict
 
 from ...exceptions.exceptions import RateLimitError
 from ...utils import ServerID
 
 
 class TokenBucket:
@@ -33,29 +33,28 @@
         time_delta = time_now - self.last_update
         self.last_update = time_now
 
         self.current = min([self.current + time_delta * self.refresh_amount, self.max])
 
 
 class RateLimiter:
-
     SERVER_LIMIT = 50
     SERVER_REFRESH_AMOUNT = 15
 
     @classmethod
     def default(cls) -> "RateLimiter":
         """
         Returns a default rate limiter with 3 tokens per second
         """
         return cls()
 
     def __init__(self) -> None:
         self.socket_buckets: Dict[ServerID, TokenBucket] = {}
         self.server_buckets: Dict[str, TokenBucket] = {}
-        self.lock = threading.Lock()
+        self.lock = asyncio.Lock()
 
     def add_socket(
         self,
         server_id: ServerID,
         current: float,
         maximum: float,
         refresh_rate: float,
@@ -65,70 +64,66 @@
             current, maximum, refresh_rate, refresh_amount
         )
         if server_id.get_server_string() not in self.server_buckets:
             self.server_buckets[server_id.get_server_string()] = TokenBucket(
                 self.SERVER_LIMIT, self.SERVER_LIMIT, 1, self.SERVER_REFRESH_AMOUNT
             )
 
-    def can_consume(self, server_id: ServerID, amount: int = 1) -> bool:
+    async def can_consume(self, server_id: ServerID, amount: int = 1) -> bool:
         """
         Returns whether the user can consume the amount of tokens provided
         """
-        self.lock.acquire(blocking=True)
-        can_consume = True
+        async with self.lock:
+            can_consume = True
 
-        for bucket in [
-            self.socket_buckets.get(server_id),
-            self.server_buckets.get(server_id.get_server_string()),
-        ]:
-            bucket.refresh()
-            if not bucket.can_consume(amount):
-                can_consume = False
+            for bucket in [
+                self.socket_buckets.get(server_id),
+                self.server_buckets.get(server_id.get_server_string()),
+            ]:
+                bucket.refresh()
+                if not bucket.can_consume(amount):
+                    can_consume = False
 
-        self.lock.release()
         return can_consume
 
-    def consume(self, server_id: ServerID, amount: int = 1) -> None:
+    async def consume(self, server_id: ServerID, amount: int = 1) -> None:
         """
         Consumes an amount of tokens from the bucket. You should first check to see whether it is possible with can_consume
         """
-        self.lock.acquire(blocking=True)
-        for bucket in [
-            self.socket_buckets.get(server_id),
-            self.server_buckets.get(server_id.get_server_string()),
-        ]:
-            bucket.refresh()
-            if not bucket.can_consume(amount):
-                self.lock.release()
-                raise RateLimitError("Not Enough Tokens")
-            bucket.consume(amount)
-        self.lock.release()
+        async with self.lock:
+            for bucket in [
+                self.socket_buckets.get(server_id),
+                self.server_buckets.get(server_id.get_server_string()),
+            ]:
+                bucket.refresh()
+                if not bucket.can_consume(amount):
+                    self.lock.release()
+                    raise RateLimitError("Not Enough Tokens")
+                bucket.consume(amount)
 
-    def get_estimated_delay_time(self, server_id: ServerID, target_cost: int) -> float:
+    async def get_estimated_delay_time(self, server_id: ServerID, target_cost: int) -> float:
         """
         Returns how long until the amount of tokens needed will be available
         """
-        self.lock.acquire(blocking=True)
-        delay = 0
-        for bucket in [
-            self.socket_buckets.get(server_id),
-            self.server_buckets.get(server_id.get_server_string()),
-        ]:
-            val = (
-                math.ceil(
-                    (((target_cost - bucket.current) / bucket.refresh_per_second) + 0.1)
-                    * 100
+        async with self.lock:
+            delay = 0
+            for bucket in [
+                self.socket_buckets.get(server_id),
+                self.server_buckets.get(server_id.get_server_string()),
+            ]:
+                val = (
+                    math.ceil(
+                        (((target_cost - bucket.current) / bucket.refresh_per_second) + 0.1)
+                        * 100
+                    )
+                    / 100
                 )
-                / 100
-            )
-            if val > delay:
-                delay = val
-        self.lock.release()
+                if val > delay:
+                    delay = val
         return delay
 
-    def remove(self, server_id: ServerID) -> None:
+    async def remove(self, server_id: ServerID) -> None:
         """
         Removes the limiter
         """
-        self.lock.acquire(blocking=True)
-        del self.socket_buckets[server_id]
-        self.lock.release()
+        async with self.lock:
+            del self.socket_buckets[server_id]
```

### Comparing `rustplus-5.5.8/rustplus/api/remote/rust_remote_interface.py` & `rustplus-5.6.0/rustplus/api/remote/rust_remote_interface.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,45 +1,40 @@
 import asyncio
 import logging
-
 from asyncio import Future
-from typing import Dict
+from typing import Union, Dict
 
 from .camera.camera_manager import CameraManager
 from .events import EventLoopManager, EntityEvent, RegisteredListener
-from .events.event_handler import EventHandler
 from .rustplus_proto import AppRequest, AppMessage, AppEmpty, AppCameraSubscribe
 from .rustws import RustWebsocket, CONNECTED, PENDING_CONNECTION
 from .ratelimiter import RateLimiter
 from .expo_bundle_handler import MagicValueGrabber
-from ...utils import ServerID
+from ...utils import ServerID, YieldingEvent
 from ...conversation import ConversationFactory
 from ...commands import CommandHandler
 from ...exceptions import (
     ClientNotConnectedError,
-    ResponseNotReceivedError,
     RequestError,
     SmartDeviceRegistrationError,
 )
 
 
 class RustRemote:
     def __init__(
         self,
         server_id: ServerID,
         command_options,
         ratelimit_limit,
         ratelimit_refill,
-        websocket_length=600,
         use_proxy: bool = False,
         api=None,
         use_test_server: bool = False,
         rate_limiter: RateLimiter = None,
     ) -> None:
-
         self.server_id = server_id
         self.api = api
         self.command_options = command_options
         self.ratelimit_limit = ratelimit_limit
         self.ratelimit_refill = ratelimit_refill
         self.use_proxy = use_proxy
         if isinstance(rate_limiter, RateLimiter):
@@ -47,170 +42,150 @@
         else:
             self.ratelimiter = RateLimiter.default()
 
         self.ratelimiter.add_socket(
             self.server_id, ratelimit_limit, ratelimit_limit, 1, ratelimit_refill
         )
         self.ws = None
-        self.websocket_length = websocket_length
-        self.responses = {}
-        self.ignored_responses = []
-        self.pending_for_response = {}
-        self.sent_requests = []
-        self.command_handler = None
+        self.logger = logging.getLogger("rustplus.py")
+
+        self.ignored_responses = set()
+        self.pending_response_events: Dict[int, YieldingEvent] = {}
 
+        self.command_handler = None
         if command_options is None:
             self.use_commands = False
         else:
             self.use_commands = True
             self.command_handler = CommandHandler(self.command_options, api)
 
-        self.event_handler = EventHandler()
-
         self.magic_value = MagicValueGrabber.get_magic_value()
         self.conversation_factory = ConversationFactory(api)
         self.use_test_server = use_test_server
         self.pending_entity_subscriptions = []
-        self.camera_manager: CameraManager = None
+        self.camera_manager: Union[CameraManager, None] = None
 
     async def connect(self, retries, delay, on_failure=None) -> None:
-
         self.ws = RustWebsocket(
             server_id=self.server_id,
             remote=self,
             use_proxy=self.use_proxy,
             magic_value=self.magic_value,
             use_test_server=self.use_test_server,
             on_failure=on_failure,
             delay=delay,
         )
         await self.ws.connect(retries=retries)
 
         for entity_id, coroutine in self.pending_entity_subscriptions:
             self.handle_subscribing_entity(entity_id, coroutine)
 
-    def close(self) -> None:
-
+    async def close(self) -> None:
         if self.ws is not None:
-            self.ws.close()
+            await self.ws.close()
             del self.ws
             self.ws = None
 
     def is_pending(self) -> bool:
         if self.ws is not None:
             return self.ws.connection_status == PENDING_CONNECTION
         return False
 
     def is_open(self) -> bool:
         if self.ws is not None:
             return self.ws.connection_status == CONNECTED
         return False
 
     async def send_message(self, request: AppRequest) -> None:
-
         if self.ws is None:
             raise ClientNotConnectedError("No Current Websocket Connection")
 
+        self.pending_response_events[request.seq] = YieldingEvent()
         await self.ws.send_message(request)
 
     async def get_response(
         self, seq: int, app_request: AppRequest, error_check: bool = True
     ) -> AppMessage:
         """
         Returns a given response from the server.
         """
 
-        attempts = 0
-
-        while seq in self.pending_for_response and seq not in self.responses:
-
-            if seq in self.sent_requests:
-
-                if attempts <= 40:
-
-                    attempts += 1
-                    await asyncio.sleep(0.1)
+        attempts = 1
 
-                else:
+        while True:
+            event = self.pending_response_events.get(seq)
+            if event is None:
+                raise Exception("Event Doesn't exist")
+
+            response: AppMessage = await event.event_wait_for(4)
+            if response is not None:
+                break
 
-                    await self.send_message(app_request)
-                    await asyncio.sleep(0.1)
-                    attempts = 0
-
-            if attempts <= 10:
-                await asyncio.sleep(0.1)
-                attempts += 1
+            await self.send_message(app_request)
 
-            else:
-                await self.send_message(app_request)
-                await asyncio.sleep(1)
-                attempts = 0
+            if attempts % 150 == 0:
+                self.logger.info(
+                    f"[RustPlus.py] Been waiting 10 minutes for a response for seq {seq}"
+                )
 
-        if seq not in self.responses:
-            raise ResponseNotReceivedError("Not Received")
+            attempts += 1
 
-        response = self.responses.pop(seq)
+        self.pending_response_events.pop(seq)
 
         if response.response.error.error == "rate_limit":
             logging.getLogger("rustplus.py").warning(
                 "[Rustplus.py] RateLimit Exception Occurred. Retrying after bucket is full"
             )
 
             # Fully Refill the bucket
+            bucket = self.ratelimiter.socket_buckets.get(self.server_id)
+            bucket.current = 0
 
-            self.ratelimiter.socket_buckets.get(self.server_id).current = 0
-
-            while (
-                self.ratelimiter.socket_buckets.get(self.server_id).current
-                < self.ratelimiter.socket_buckets.get(self.server_id).max
-            ):
+            while bucket.current < bucket.max:
                 await asyncio.sleep(1)
-                self.ratelimiter.socket_buckets.get(self.server_id).refresh()
+                bucket.refresh()
 
             # Reattempt the sending with a full bucket
             cost = self.ws.get_proto_cost(app_request)
 
             while True:
-
-                if self.ratelimiter.can_consume(self.server_id, cost):
-                    self.ratelimiter.consume(self.server_id, cost)
+                if await self.ratelimiter.can_consume(self.server_id, cost):
+                    await self.ratelimiter.consume(self.server_id, cost)
                     break
 
                 await asyncio.sleep(
-                    self.ratelimiter.get_estimated_delay_time(self.server_id, cost)
+                    await self.ratelimiter.get_estimated_delay_time(self.server_id, cost)
                 )
 
             await self.send_message(app_request)
             response = await self.get_response(seq, app_request)
 
         elif self.ws.error_present(response.response.error.error) and error_check:
             raise RequestError(response.response.error.error)
 
         return response
 
     def handle_subscribing_entity(self, entity_id: int, coroutine) -> None:
-
         if not self.is_open():
             self.pending_entity_subscriptions.append((entity_id, coroutine))
             return
 
-        async def get_entity_info(self: RustRemote, eid):
-
-            await self.api._handle_ratelimit()
+        async def get_entity_info(remote: RustRemote, eid):
+            await remote.api._handle_ratelimit()
 
-            app_request = self.api._generate_protobuf()
+            app_request: AppRequest = remote.api._generate_protobuf()
             app_request.entityId = eid
-            app_request.getEntityInfo.CopyFrom(AppEmpty())
+            app_request.get_entity_info = AppEmpty()
+            app_request.get_entity_info._serialized_on_wire = True
 
-            await self.send_message(app_request)
+            await remote.send_message(app_request)
 
-            return await self.get_response(app_request.seq, app_request, False)
+            return await remote.get_response(app_request.seq, app_request, False)
 
         def entity_event_callback(future_inner: Future) -> None:
-
             entity_info = future_inner.result()
 
             if entity_info.response.HasField("error"):
                 raise SmartDeviceRegistrationError(
                     f"Entity: '{entity_id}' has not been found"
                 )
 
@@ -226,32 +201,34 @@
         )
         future.add_done_callback(entity_event_callback)
 
     async def subscribe_to_camera(
         self, entity_id: int, ignore_response: bool = False
     ) -> AppRequest:
         await self.api._handle_ratelimit()
-        app_request = self.api._generate_protobuf()
+        app_request: AppRequest = self.api._generate_protobuf()
         subscribe = AppCameraSubscribe()
-        subscribe.cameraId = entity_id
-        app_request.cameraSubscribe.CopyFrom(subscribe)
+        subscribe.camera_id = entity_id
+        app_request.camera_subscribe = subscribe
 
         await self.send_message(app_request)
 
         if ignore_response:
-            self.ignored_responses.append(app_request.seq)
+            await self.add_ignored_response(app_request.seq)
 
         return app_request
 
     async def create_camera_manager(self, cam_id) -> CameraManager:
-
         if self.camera_manager is not None:
             if self.camera_manager._cam_id == cam_id:
                 return self.camera_manager
 
         app_request = await self.subscribe_to_camera(cam_id)
         app_message = await self.get_response(app_request.seq, app_request)
 
         self.camera_manager = CameraManager(
-            self.api, cam_id, app_message.response.cameraSubscribeInfo
+            self.api, cam_id, app_message.response.camera_subscribe_info
         )
         return self.camera_manager
+
+    async def add_ignored_response(self, seq) -> None:
+        self.ignored_responses.add(seq)
```

### Comparing `rustplus-5.5.8/rustplus/api/remote/rustws.py` & `rustplus-5.6.0/rustplus/api/remote/rustws.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,94 +1,90 @@
 import asyncio
 import base64
 import logging
 import time
 from datetime import datetime
-from threading import Thread
-from typing import Optional
-import websocket
+from typing import Optional, Union
+import betterproto
+from asyncio import Task
+from websockets.client import connect
+from websockets.legacy.client import WebSocketClientProtocol
 
 from .camera.structures import RayPacket
-from .events import EventLoopManager
 from .rustplus_proto import AppMessage, AppRequest
+from .events import EventHandler
 from ..structures import RustChatMessage
 from ...exceptions import ClientNotConnectedError
 from ...conversation import Conversation
-from ...utils import ServerID
+from ...utils import ServerID, YieldingEvent
 
 CONNECTED = 1
 PENDING_CONNECTION = 2
 CLOSING = 4
 CLOSED = 3
 
 
-class RustWebsocket(websocket.WebSocket):
+class RustWebsocket:
     def __init__(
         self,
         server_id: ServerID,
         remote,
         use_proxy,
         magic_value,
         use_test_server,
         on_failure,
         delay,
     ):
-
+        self.connection: Union[WebSocketClientProtocol, None] = None
+        self.task: Union[Task, None] = None
         self.server_id = server_id
-        self.thread: Thread = None
         self.connection_status = CLOSED
         self.use_proxy = use_proxy
         self.remote = remote
         self.logger = logging.getLogger("rustplus.py")
         self.connected_time = time.time()
         self.magic_value = magic_value
         self.use_test_server = use_test_server
         self.outgoing_conversation_messages = []
         self.on_failure = on_failure
         self.delay = delay
 
-        super().__init__()
-
     async def connect(
         self, retries=float("inf"), ignore_open_value: bool = False
     ) -> None:
-
         if (
             not self.connection_status == CONNECTED or ignore_open_value
         ) and not self.remote.is_pending():
-
             attempts = 0
 
             while True:
-
                 if attempts >= retries:
                     raise ConnectionAbortedError("Reached Retry Limit")
 
                 self.connection_status = PENDING_CONNECTION
 
                 try:
                     address = (
                         (
                             f"wss://{self.server_id.ip}"
                             if self.server_id.port is None
-                            else f"wss://{self.server_id.ip}:{self.server_id.port}"
+                            else f"ws://{self.server_id.ip}:{self.server_id.port}"
                         )
                         if self.use_test_server
                         else (
                             f"wss://companion-rust.facepunch.com/game/{self.server_id.ip}/{self.server_id.port}"
                             if self.use_proxy
                             else f"ws://{self.server_id.ip}:{self.server_id.port}"
                         )
                     )
                     address += f"?v={str(self.magic_value)}"
-                    super().connect(address)
+                    self.connection = await connect(address, close_timeout=0)
                     self.connected_time = time.time()
                     break
                 except Exception as exception:
-
                     print_error = True
 
                     if not isinstance(exception, KeyboardInterrupt):
                         # Run the failure callback
                         try:
                             if self.on_failure is not None:
                                 if asyncio.iscoroutinefunction(self.on_failure):
@@ -104,166 +100,155 @@
 
                     if print_error:
                         self.logger.warning(
                             f"{datetime.now().strftime('%d/%m/%Y %H:%M:%S')} "
                             f"[RustPlus.py] Cannot Connect to server. Retrying in {str(self.delay)} second/s"
                         )
                     attempts += 1
-                    time.sleep(self.delay)
+                    await asyncio.sleep(self.delay)
 
             self.connection_status = CONNECTED
 
         if not ignore_open_value:
-            self.thread = Thread(
-                target=self.run, name="[RustPlus.py] WebsocketThread", daemon=True
+            self.task = asyncio.create_task(
+                self.run(), name="[RustPlus.py] Websocket Polling Task"
             )
-            self.thread.start()
-
-    def close(self) -> None:
 
+    async def close(self) -> None:
         self.connection_status = CLOSING
-        self.shutdown()
-        # super().close()
+        await self.connection.close()
+        self.connection = None
+        self.task.cancel()
+        self.task = None
         self.connection_status = CLOSED
 
     async def send_message(self, message: AppRequest) -> None:
         """
         Send the Protobuf to the server
         """
 
         if self.connection_status == CLOSED:
             raise ClientNotConnectedError("Not Connected")
 
         try:
             if self.use_test_server:
-                self.send(base64.b64encode(message.SerializeToString()))
+                await self.connection.send(
+                    base64.b64encode(bytes(message)).decode("utf-8")
+                )
             else:
-                self.send_binary(message.SerializeToString())
-            self.remote.pending_for_response[message.seq] = message
+                await self.connection.send(bytes(message))
         except Exception:
+            self.logger.exception("An exception occurred whilst sending a message")
+
             while self.remote.is_pending():
                 await asyncio.sleep(0.5)
-            return await self.remote.send_message(message)
-
-    def run(self) -> None:
+            return await self.send_message(message)
 
+    async def run(self) -> None:
         while self.connection_status == CONNECTED:
             try:
-                data = self.recv()
+                data = await self.connection.recv()
 
-                self.remote.event_handler.run_proto_event(data, self.server_id)
+                await EventHandler.run_proto_event(data, self.server_id)
 
                 app_message = AppMessage()
-                if self.use_test_server:
-                    app_message.ParseFromString(base64.b64decode(data))
-                else:
-                    app_message.ParseFromString(data)
+                app_message.parse(
+                    base64.b64decode(data) if self.use_test_server else data
+                )
 
             except Exception:
                 if self.connection_status == CONNECTED:
                     self.logger.warning(
                         f"{datetime.now().strftime('%d/%m/%Y %H:%M:%S')} [RustPlus.py] Connection interrupted, Retrying"
                     )
-                    asyncio.run_coroutine_threadsafe(
-                        self.connect(ignore_open_value=True),
-                        EventLoopManager.get_loop(self.server_id),
-                    ).result()
+                    await self.connect(ignore_open_value=True)
+
                     continue
                 return
 
             try:
-                del self.remote.pending_for_response[app_message.response.seq]
-            except KeyError:
-                pass
-
-            try:
-                self.handle_message(app_message)
-            except Exception as e:
-                self.logger.error(e)
-
-    def handle_message(self, app_message: AppMessage) -> None:
+                await self.handle_message(app_message)
+            except Exception:
+                self.logger.exception("An Error occurred whilst handling the event")
 
+    async def handle_message(self, app_message: AppMessage) -> None:
         if app_message.response.seq in self.remote.ignored_responses:
             self.remote.ignored_responses.remove(app_message.response.seq)
             return
 
         prefix = self.get_prefix(
-            str(app_message.broadcast.newTeamMessage.message.message)
+            str(app_message.broadcast.team_message.message.message)
         )
 
         if prefix is not None:
             # This means it is a command
 
-            message = RustChatMessage(app_message.broadcast.newTeamMessage.message)
-
-            self.remote.command_handler.run_command(message, prefix)
+            message = RustChatMessage(app_message.broadcast.team_message.message)
+            await self.remote.command_handler.run_command(message, prefix)
 
         if self.is_entity_broadcast(app_message):
             # This means that an entity has changed state
 
-            self.remote.event_handler.run_entity_event(
-                app_message.broadcast.entityChanged.entityId,
+            await EventHandler.run_entity_event(
+                app_message.broadcast.entity_changed.entity_id,
                 app_message,
                 self.server_id,
             )
 
         elif self.is_camera_broadcast(app_message):
             if self.remote.camera_manager is not None:
-                self.remote.camera_manager.add_packet(
-                    RayPacket(app_message.broadcast.cameraRays)
+                await self.remote.camera_manager.add_packet(
+                    RayPacket(app_message.broadcast.camera_rays)
                 )
 
         elif self.is_team_broadcast(app_message):
             # This means that the team of the current player has changed
-            self.remote.event_handler.run_team_event(app_message, self.server_id)
+            await EventHandler.run_team_event(app_message, self.server_id)
 
         elif self.is_message(app_message):
             # This means that a message has been sent to the team chat
 
-            steam_id = int(app_message.broadcast.newTeamMessage.message.steamId)
-            message = str(app_message.broadcast.newTeamMessage.message.message)
+            steam_id = int(app_message.broadcast.team_message.message.steam_id)
+            message = str(app_message.broadcast.team_message.message.message)
 
             # Conversation API
             if self.remote.conversation_factory.has_conversation(steam_id):
                 if message not in self.outgoing_conversation_messages:
                     conversation: Conversation = (
                         self.remote.conversation_factory.get_conversation(steam_id)
                     )
 
                     conversation.get_answers().append(message)
-                    conversation.run_coro(
-                        conversation.get_current_prompt().on_response, args=[message]
-                    )
+                    await conversation.get_current_prompt().on_response(message)
 
                     if conversation.has_next():
                         conversation.increment_prompt()
                         prompt = conversation.get_current_prompt()
-                        prompt_string = conversation.run_coro(prompt.prompt, args=[])
-                        conversation.run_coro(
-                            conversation.send_prompt, args=[prompt_string]
-                        )
+                        prompt_string = await prompt.prompt()
+                        await conversation.send_prompt(prompt_string)
+
                     else:
                         prompt = conversation.get_current_prompt()
-                        prompt_string = conversation.run_coro(prompt.on_finish, args=[])
+                        prompt_string = await prompt.on_finish()
                         if prompt_string != "":
-                            conversation.run_coro(
-                                conversation.send_prompt, args=[prompt_string]
-                            )
+                            await conversation.send_prompt(prompt_string)
                         self.remote.conversation_factory.abort_conversation(steam_id)
                 else:
                     self.outgoing_conversation_messages.remove(message)
 
                 # Conversation API end
 
-            self.remote.event_handler.run_chat_event(app_message, self.server_id)
+            await EventHandler.run_chat_event(app_message, self.server_id)
 
         else:
             # This means that it wasn't sent by the server and is a message from the server in response to an action
-
-            self.remote.responses[app_message.response.seq] = app_message
+            event: YieldingEvent = self.remote.pending_response_events[
+                app_message.response.seq
+            ]
+            event.set_with_value(app_message)
 
     def get_prefix(self, message: str) -> Optional[str]:
         if self.remote.use_commands:
             if message.startswith(self.remote.command_options.prefix):
                 return self.remote.command_options.prefix
         else:
             return None
@@ -271,54 +256,50 @@
         for overrule in self.remote.command_options.overruling_commands:
             if message.startswith(overrule):
                 return overrule
 
         return None
 
     @staticmethod
-    def is_message(app_message) -> bool:
-        return str(app_message.broadcast.newTeamMessage.message.message) != ""
+    def is_message(app_message: AppMessage) -> bool:
+        return betterproto.serialized_on_wire(
+            app_message.broadcast.team_message.message
+        )
 
     @staticmethod
-    def is_camera_broadcast(app_message) -> bool:
-        return app_message.broadcast.HasField("cameraRays")
+    def is_camera_broadcast(app_message: AppMessage) -> bool:
+        return betterproto.serialized_on_wire(app_message.broadcast.camera_rays)
 
     @staticmethod
-    def is_entity_broadcast(app_message) -> bool:
-        return str(app_message.broadcast.entityChanged) != ""
+    def is_entity_broadcast(app_message: AppMessage) -> bool:
+        return betterproto.serialized_on_wire(app_message.broadcast.entity_changed)
 
     @staticmethod
-    def is_team_broadcast(app_message) -> bool:
-        return str(app_message.broadcast.teamChanged) != ""
-
-    async def _retry_failed_request(self, app_request: AppRequest) -> None:
-        """
-        Resends an AppRequest to the server if it has failed
-        """
-        await self.send_message(app_request)
+    def is_team_broadcast(app_message: AppMessage) -> bool:
+        return betterproto.serialized_on_wire(app_message.broadcast.team_changed)
 
     @staticmethod
-    def get_proto_cost(app_request) -> int:
+    def get_proto_cost(app_request: AppRequest) -> int:
         """
         Gets the cost of an AppRequest
         """
         costs = {
-            "getTime": 1,
-            "sendTeamMessage": 2,
-            "getInfo": 1,
-            "getTeamChat": 1,
-            "getTeamInfo": 1,
-            "getMapMarkers": 1,
-            "getMap": 5,
-            "setEntityValue": 1,
-            "getEntityInfo": 1,
-            "promoteToLeader": 1,
+            app_request.get_time: 1,
+            app_request.send_team_message: 2,
+            app_request.get_info: 1,
+            app_request.get_team_chat: 1,
+            app_request.get_team_info: 1,
+            app_request.get_map_markers: 1,
+            app_request.get_map: 5,
+            app_request.set_entity_value: 1,
+            app_request.get_entity_info: 1,
+            app_request.promote_to_leader: 1,
         }
         for request, cost in costs.items():
-            if app_request.HasField(request):
+            if betterproto.serialized_on_wire(request):
                 return cost
 
         raise ValueError()
 
     @staticmethod
     def error_present(message) -> bool:
         """
```

### Comparing `rustplus-5.5.8/rustplus/api/remote/server_checker.py` & `rustplus-5.6.0/rustplus/api/remote/server_checker.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,8 +17,10 @@
             req = requests.post(
                 f"https://companion-rust.facepunch.com/api/server/test_connection?address={self.ip}&port={self.port}"
             )
             for msg in req.json()["messages"]:
                 if "does not match your outgoing IP address" not in msg:
                     self.logger.warning(f"Error from server Checker: {msg}")
         except Exception:
-            pass
+            self.logger.exception(
+                f"Unable to test connection to server - {self.ip}:{self.port}"
+            )
```

### Comparing `rustplus-5.5.8/rustplus/api/rust_api.py` & `rustplus-5.6.0/rustplus/api/rust_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,15 +15,20 @@
     RustMarker,
     RustChatMessage,
     RustTeamInfo,
     RustEntityInfo,
     RustContents,
     RustItem,
 )
-from .remote.rustplus_proto import *
+from .remote.rustplus_proto import (
+    AppEmpty,
+    AppSendMessage,
+    AppSetEntityValue,
+    AppPromoteToLeader,
+)
 from .remote import HeartBeat, RateLimiter
 from ..commands import CommandOptions
 from ..exceptions import *
 from ..utils import (
     RustTime,
     format_time,
     format_coord,
@@ -63,102 +68,101 @@
             use_proxy=use_proxy,
             use_test_server=use_test_server,
             event_loop=event_loop,
             rate_limiter=rate_limiter,
         )
 
     async def get_time(self) -> RustTime:
-
         await self._handle_ratelimit()
 
         app_request = self._generate_protobuf()
-        app_request.getTime.CopyFrom(AppEmpty())
+        app_request.get_time = AppEmpty()
+        app_request.get_time._serialized_on_wire = True
 
         await self.remote.send_message(app_request)
 
         response = await self.remote.get_response(app_request.seq, app_request)
 
         return format_time(response)
 
     async def send_team_message(self, message: str) -> None:
-
         await self._handle_ratelimit(2)
 
         app_send_message = AppSendMessage()
         app_send_message.message = message
 
         app_request = self._generate_protobuf()
-        app_request.sendTeamMessage.CopyFrom(app_send_message)
+        app_request.send_team_message = app_send_message
 
-        self.remote.ignored_responses.append(app_request.seq)
+        await self.remote.add_ignored_response(app_request.seq)
 
         await self.remote.send_message(app_request)
 
     async def get_info(self) -> RustInfo:
-
         await self._handle_ratelimit()
 
         app_request = self._generate_protobuf()
-        app_request.getInfo.CopyFrom(AppEmpty())
+        app_request.get_info = AppEmpty()
+        app_request.get_info._serialized_on_wire = True
 
         await self.remote.send_message(app_request)
 
         response = await self.remote.get_response(app_request.seq, app_request)
 
         return RustInfo(response.response.info)
 
     async def get_team_chat(self) -> List[RustChatMessage]:
-
         await self._handle_ratelimit()
 
         app_request = self._generate_protobuf()
-        app_request.getTeamChat.CopyFrom(AppEmpty())
+        app_request.get_team_chat = AppEmpty()
+        app_request.get_team_chat._serialized_on_wire = True
 
         await self.remote.send_message(app_request)
 
         messages = (
             await self.remote.get_response(app_request.seq, app_request)
-        ).response.teamChat.messages
+        ).response.team_chat.messages
 
         return [RustChatMessage(message) for message in messages]
 
     async def get_team_info(self) -> RustTeamInfo:
-
         await self._handle_ratelimit()
 
         app_request = self._generate_protobuf()
-        app_request.getTeamInfo.CopyFrom(AppEmpty())
+        app_request.get_team_info = AppEmpty()
+        app_request.get_team_info._serialized_on_wire = True
 
         await self.remote.send_message(app_request)
 
         app_message = await self.remote.get_response(app_request.seq, app_request)
 
-        return RustTeamInfo(app_message.response.teamInfo)
+        return RustTeamInfo(app_message.response.team_info)
 
     async def get_markers(self) -> List[RustMarker]:
-
         await self._handle_ratelimit()
 
         app_request = self._generate_protobuf()
-        app_request.getMapMarkers.CopyFrom(AppEmpty())
+        app_request.get_map_markers = AppEmpty()
+        app_request.get_map_markers._serialized_on_wire = True
 
         await self.remote.send_message(app_request)
 
         app_message = await self.remote.get_response(app_request.seq, app_request)
 
         return [
-            RustMarker(marker) for marker in app_message.response.mapMarkers.markers
+            RustMarker(marker) for marker in app_message.response.map_markers.markers
         ]
 
     async def get_raw_map_data(self) -> RustMap:
-
         await self._handle_ratelimit(5)
 
         app_request = self._generate_protobuf()
-        app_request.getMap.CopyFrom(AppEmpty())
+        app_request.get_map = AppEmpty()
+        app_request.get_map._serialized_on_wire = True
 
         await self.remote.send_message(app_request)
 
         app_message = await self.remote.get_response(app_request.seq, app_request)
 
         return RustMap(app_message.response.map)
 
@@ -166,15 +170,14 @@
         self,
         add_icons: bool = False,
         add_events: bool = False,
         add_vending_machines: bool = False,
         override_images: dict = None,
         add_grid: bool = False,
     ) -> Image.Image:
-
         if override_images is None:
             override_images = {}
 
         map_size = int((await self.get_info()).size)
 
         await self._handle_ratelimit(
             5
@@ -182,25 +185,26 @@
                 1
                 if [add_icons, add_events, add_vending_machines].count(True) >= 1
                 else 0
             )
         )
 
         app_request = self._generate_protobuf()
-        app_request.getMap.CopyFrom(AppEmpty())
+        app_request.get_map = AppEmpty()
+        app_request.get_map._serialized_on_wire = True
 
         await self.remote.send_message(app_request)
 
         app_message = await self.remote.get_response(app_request.seq, app_request)
 
         game_map = app_message.response.map
         monuments = list(game_map.monuments)
 
         try:
-            image = Image.open(BytesIO(game_map.jpgImage))
+            image = Image.open(BytesIO(game_map.jpg_image))
         except Exception:
             raise ImageError("Invalid bytes for the image")
 
         if not self.use_test_server:
             image = image.crop((500, 500, game_map.height - 500, game_map.width - 500))
 
         game_map = image.resize((map_size, map_size), Image.ANTIALIAS).convert("RGBA")
@@ -279,93 +283,87 @@
                         (int(marker.x) - 50, map_size - int(marker.y) - 50),
                         vending_machine,
                     )
 
         return game_map.resize((2000, 2000), Image.ANTIALIAS)
 
     async def get_entity_info(self, eid: int = None) -> RustEntityInfo:
-
         await self._handle_ratelimit()
 
         if eid is None:
             raise ValueError("EID cannot be None")
 
         app_request = self._generate_protobuf()
-        app_request.entityId = eid
-        app_request.getEntityInfo.CopyFrom(AppEmpty())
+        app_request.entity_id = eid
+        app_request.get_entity_info = AppEmpty()
+        app_request.get_entity_info._serialized_on_wire = True
 
         await self.remote.send_message(app_request)
 
         app_message = await self.remote.get_response(app_request.seq, app_request)
 
-        return RustEntityInfo(app_message.response.entityInfo)
+        return RustEntityInfo(app_message.response.entity_info)
 
     async def _update_smart_device(self, eid: int, value: bool) -> None:
-
         await self._handle_ratelimit()
 
         entity_value = AppSetEntityValue()
         entity_value.value = value
 
         app_request = self._generate_protobuf()
 
-        app_request.entityId = eid
-        app_request.setEntityValue.CopyFrom(entity_value)
+        app_request.entity_id = eid
+        app_request.set_entity_value = entity_value
 
-        self.remote.ignored_responses.append(app_request.seq)
+        await self.remote.add_ignored_response(app_request.seq)
 
         await self.remote.send_message(app_request)
 
     async def turn_on_smart_switch(self, eid: int = None) -> None:
-
         if eid is None:
             raise ValueError("EID cannot be None")
 
         await self._update_smart_device(eid, True)
 
     async def turn_off_smart_switch(self, eid: int = None) -> None:
-
         if eid is None:
             raise ValueError("EID cannot be None")
 
         await self._update_smart_device(eid, False)
 
     async def promote_to_team_leader(self, steam_id: int = None) -> None:
-
         if steam_id is None:
             raise ValueError("SteamID cannot be None")
 
         await self._handle_ratelimit()
 
         leader_packet = AppPromoteToLeader()
-        leader_packet.steamId = steam_id
+        leader_packet.steam_id = steam_id
 
         app_request = self._generate_protobuf()
-        app_request.promoteToLeader.CopyFrom(leader_packet)
+        app_request.promote_to_leader = leader_packet
 
-        self.remote.ignored_responses.append(app_request.seq)
+        await self.remote.add_ignored_response(app_request.seq)
 
         await self.remote.send_message(app_request)
 
     async def get_current_events(self) -> List[RustMarker]:
-
         return [
             marker
             for marker in (await self.get_markers())
             if marker.type == 2
             or marker.type == 4
             or marker.type == 5
             or marker.type == 6
             or marker.type == 8
         ]
 
     async def get_contents(
         self, eid: int = None, combine_stacks: bool = False
     ) -> RustContents:
-
         if eid is None:
             raise ValueError("EID cannot be None")
 
         returned_data = await self.get_entity_info(eid)
 
         target_time = datetime.utcfromtimestamp(int(returned_data.protection_expiry))
         difference = target_time - datetime.utcnow()
@@ -411,9 +409,9 @@
 
     @deprecated("Use RustSocket.get_contents")
     async def get_tc_storage_contents(
         self, eid: int = None, combine_stacks: bool = False
     ) -> RustContents:
         return await self.get_contents(eid=eid, combine_stacks=combine_stacks)
 
-    async def get_camera_manager(self, id: str) -> CameraManager:
-        return await self.remote.create_camera_manager(id)
+    async def get_camera_manager(self, cam_id: str) -> CameraManager:
+        return await self.remote.create_camera_manager(cam_id)
```

### Comparing `rustplus-5.5.8/rustplus/api/structures/rust_chat_message.py` & `rustplus-5.6.0/rustplus/api/structures/rust_chat_message.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,13 @@
+from ..remote.rustplus_proto import AppTeamMessage
+
+
 class RustChatMessage:
-    def __init__(self, data):
-        self._steam_id: int = data.steamId
+    def __init__(self, data: AppTeamMessage):
+        self._steam_id: int = data.steam_id
         self._name: str = data.name
         self._message: str = data.message
         self._colour: str = data.color
         self._time: int = data.time
 
     @property
     def steam_id(self) -> int:
```

### Comparing `rustplus-5.5.8/rustplus/api/structures/rust_contents.py` & `rustplus-5.6.0/rustplus/api/structures/rust_contents.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.8/rustplus/api/structures/rust_entity_info.py` & `rustplus-5.6.0/rustplus/api/structures/rust_entity_info.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from typing import List
 
+from ..remote import AppEntityInfo, AppEntityPayloadItem
+
 
 class RustEntityInfoItem:
-    def __init__(self, data) -> None:
-        self._item_id: int = data.itemId
+    def __init__(self, data: AppEntityPayloadItem) -> None:
+        self._item_id: int = data.item_id
         self._quantity: int = data.quantity
-        self._item_is_blueprint: bool = data.itemIsBlueprint
+        self._item_is_blueprint: bool = data.item_is_blueprint
 
     @property
     def item_id(self) -> int:
         return self._item_id
 
     @property
     def quantity(self) -> int:
@@ -24,21 +26,21 @@
             "RustEntityInfoItem[item_id={}, quantity={}, item_is_blueprint={}]".format(
                 self._item_id, self._quantity, self._item_is_blueprint
             )
         )
 
 
 class RustEntityInfo:
-    def __init__(self, data) -> None:
+    def __init__(self, data: AppEntityInfo) -> None:
         self._type: int = data.type
         self._value: bool = data.payload.value
         self._items = [RustEntityInfoItem(item) for item in data.payload.items]
         self._capacity: int = data.payload.capacity
-        self._has_protection: bool = data.payload.hasProtection
-        self._protection_expiry: int = data.payload.protectionExpiry
+        self._has_protection: bool = data.payload.has_protection
+        self._protection_expiry: int = data.payload.protection_expiry
 
     @property
     def type(self) -> int:
         return self._type
 
     @property
     def value(self) -> bool:
```

### Comparing `rustplus-5.5.8/rustplus/api/structures/rust_info.py` & `rustplus-5.6.0/rustplus/api/structures/rust_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,23 @@
+from ..remote.rustplus_proto import AppInfo
+
+
 class RustInfo:
-    def __init__(self, data) -> None:
+    def __init__(self, data: AppInfo) -> None:
         self._name: str = data.name
         self._url: str = data.url
-        self._header_image: str = data.headerImage
+        self._header_image: str = data.header_image
         self._map: str = data.map
-        self._size: int = data.mapSize
-        self._wipe_time: int = data.wipeTime
+        self._size: int = data.map_size
+        self._wipe_time: int = data.wipe_time
         self._players: int = data.players
-        self._max_players: int = data.maxPlayers
-        self._queued_players: int = data.queuedPlayers
+        self._max_players: int = data.max_players
+        self._queued_players: int = data.queued_players
         self._seed: int = data.seed
-        self._logo_image: str = data.logoImage
+        self._logo_image: str = data.logo_image
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
     def name(self) -> str:
```

### Comparing `rustplus-5.5.8/rustplus/api/structures/rust_item.py` & `rustplus-5.6.0/rustplus/api/structures/rust_item.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+from typing import Union
+
+
 class RustItem:
     def __init__(
-        self, name: str, item_id: int, quantity: int, is_blueprint: bool
+        self, name: str, item_id: Union[str, int], quantity: int, is_blueprint: bool
     ) -> None:
         self._name: str = name
-        self._item_id: int = item_id
+        self._item_id: int = int(item_id)
         self._quantity: int = quantity
         self._is_blueprint: bool = is_blueprint
 
     @property
     def name(self) -> str:
         return self._name
```

### Comparing `rustplus-5.5.8/rustplus/api/structures/rust_map.py` & `rustplus-5.6.0/rustplus/api/structures/rust_map.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from typing import List
 
+from ..remote.rustplus_proto import AppMap
+
 
 class RustMonument:
     def __init__(self, token, x, y) -> None:
         self._token: str = token
         self._x: float = x
         self._y: float = y
 
@@ -22,19 +24,19 @@
     def __str__(self) -> str:
         return "RustMonument[token={}, x={}, y={}]".format(
             self._token, self._x, self._y
         )
 
 
 class RustMap:
-    def __init__(self, data) -> None:
+    def __init__(self, data: AppMap) -> None:
         self._width: int = data.width
         self._height: int = data.height
-        self._jpg_image: bytes = data.jpgImage
-        self._margin: int = data.oceanMargin
+        self._jpg_image: bytes = data.jpg_image
+        self._margin: int = data.ocean_margin
         self._monuments = [
             RustMonument(monument.token, monument.x, monument.y)
             for monument in data.monuments
         ]
         self._background: str = None if data.background == "" else data.background
 
     @property
```

### Comparing `rustplus-5.5.8/rustplus/api/structures/rust_marker.py` & `rustplus-5.6.0/rustplus/api/structures/rust_marker.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from typing import List
 
+from ..remote.rustplus_proto import Vector4, AppMarkerSellOrder, AppMarker
+
 
 class RustColour:
-    def __init__(self, data) -> None:
+    def __init__(self, data: Vector4) -> None:
         self._x: float = data.x
         self._y: float = data.y
         self._z: float = data.z
         self._w: float = data.w
 
     @property
     def x(self) -> float:
@@ -27,22 +29,22 @@
     def __str__(self) -> str:
         return "RustColour[x={}, y={}, z={}, w={}]".format(
             self._x, self._y, self._z, self._w
         )
 
 
 class RustSellOrder:
-    def __init__(self, data) -> None:
-        self._item_id: int = data.itemId
+    def __init__(self, data: AppMarkerSellOrder) -> None:
+        self._item_id: int = data.item_id
         self._quantity: int = data.quantity
-        self._currency_id: int = data.currencyId
-        self._cost_per_item: int = data.costPerItem
-        self._item_is_blueprint: bool = data.itemIsBlueprint
-        self._currency_is_blueprint: bool = data.currencyIsBlueprint
-        self._amount_in_stock: int = data.amountInStock
+        self._currency_id: int = data.currency_id
+        self._cost_per_item: int = data.cost_per_item
+        self._item_is_blueprint: bool = data.item_is_blueprint
+        self._currency_is_blueprint: bool = data.currency_is_blueprint
+        self._amount_in_stock: int = data.amount_in_stock
 
     @property
     def item_id(self) -> int:
         return self._item_id
 
     @property
     def quantity(self) -> int:
@@ -79,38 +81,37 @@
                 self._item_is_blueprint,
                 self._currency_is_blueprint,
             )
         )
 
 
 class RustMarker:
-
     PlayerMarker = 1
     ExplosionMarker = 2
     VendingMachineMarker = 3
     ChinookMarker = 4
     CargoShipMarker = 5
     CrateMarker = 6
     RadiusMarker = 7
     PatrolHelicopterMarker = 8
 
-    def __init__(self, data) -> None:
+    def __init__(self, data: AppMarker) -> None:
         self._id: int = data.id
         self._type: int = data.type
         self._x: float = data.x
         self._y: float = data.y
-        self._steam_id: int = data.steamId
+        self._steam_id: int = data.steam_id
         self._rotation: float = data.rotation
         self._radius: float = data.radius
         self._colour1 = RustColour(data.color1)
         self._colour2 = RustColour(data.color2)
         self._alpha: float = data.alpha
         self._name: str = data.name
-        self._out_of_stock: bool = data.outOfStock
-        self._sell_orders = [RustSellOrder(order) for order in data.sellOrders]
+        self._out_of_stock: bool = data.out_of_stock
+        self._sell_orders = [RustSellOrder(order) for order in data.sell_orders]
 
     @property
     def id(self) -> int:
         return self._id
 
     @property
     def type(self) -> int:
```

### Comparing `rustplus-5.5.8/rustplus/api/structures/rust_team_info.py` & `rustplus-5.6.0/rustplus/api/structures/rust_team_info.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from typing import List
 
+from ..remote.rustplus_proto import AppTeamInfoMember, AppTeamInfoNote, AppTeamInfo
+
 
 class RustTeamMember:
-    def __init__(self, data) -> None:
-        self._steam_id: int = data.steamId
+    def __init__(self, data: AppTeamInfoMember) -> None:
+        self._steam_id: int = data.steam_id
         self._name: str = data.name
         self._x: float = data.x
         self._y: float = data.y
-        self._is_online: bool = data.isOnline
-        self._spawn_time: int = data.spawnTime
-        self._is_alive: bool = data.isAlive
-        self._death_time: int = data.deathTime
+        self._is_online: bool = data.is_online
+        self._spawn_time: int = data.spawn_time
+        self._is_alive: bool = data.is_alive
+        self._death_time: int = data.death_time
 
     @property
     def steam_id(self) -> int:
         return self._steam_id
 
     @property
     def name(self) -> str:
@@ -54,15 +56,15 @@
             self._spawn_time,
             self._is_alive,
             self._death_time,
         )
 
 
 class RustTeamNote:
-    def __init__(self, data) -> None:
+    def __init__(self, data: AppTeamInfoNote) -> None:
         self._type: int = data.type
         self._x: float = data.x
         self._y: float = data.y
 
     @property
     def type(self) -> int:
         return self._type
@@ -76,19 +78,19 @@
         return self._y
 
     def __str__(self) -> str:
         return "RustTeamNote[type={}, x={}, y={}]".format(self._type, self._x, self._y)
 
 
 class RustTeamInfo:
-    def __init__(self, data) -> None:
-        self._leader_steam_id: int = data.leaderSteamId
+    def __init__(self, data: AppTeamInfo) -> None:
+        self._leader_steam_id: int = data.leader_steam_id
         self._members = [RustTeamMember(member) for member in data.members]
-        self._map_notes = [RustTeamNote(note) for note in data.mapNotes]
-        self._leader_map_notes = [RustTeamNote(note) for note in data.leaderMapNotes]
+        self._map_notes = [RustTeamNote(note) for note in data.map_notes]
+        self._leader_map_notes = [RustTeamNote(note) for note in data.leader_map_notes]
 
     @property
     def leader_steam_id(self) -> int:
         return self._leader_steam_id
 
     @property
     def members(self) -> List[RustTeamMember]:
```

### Comparing `rustplus-5.5.8/rustplus/api/structures/rust_time.py` & `rustplus-5.6.0/rustplus/api/structures/rust_time.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.8/rustplus/commands/command.py` & `rustplus-5.6.0/rustplus/commands/command.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.8/rustplus/commands/command_data.py` & `rustplus-5.6.0/rustplus/commands/command_data.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.8/rustplus/conversation/conversation.py` & `rustplus-5.6.0/rustplus/conversation/conversation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import asyncio
-from typing import List
+from typing import List, Any
 from .conversation_prompt import ConversationPrompt
 from ..api.remote.events import EventLoopManager
 
 
 class Conversation:
     def __init__(
         self,
         api,
         target: int = None,
         prompts: List[ConversationPrompt] = None,
         register=None,
     ) -> None:
-
         if target is None:
             raise ValueError("target must be specified")
         self._target = target
 
         if prompts is None:
             self._prompts = []
         else:
@@ -50,14 +49,14 @@
             self._api.remote.ws.outgoing_conversation_messages.append(message)
         await self._api.send_team_message(message)
 
     async def start(self) -> None:
         self._register(self._target, self)
         await self.send_prompt(await self._prompts[0].prompt())
 
-    def run_coro(self, coro, args) -> None:
+    def run_coro(self, coro, args) -> Any:
         return asyncio.run_coroutine_threadsafe(
             coro(*args), EventLoopManager.get_loop(self._api.server_id)
         ).result()
 
     def get_answers(self) -> List[str]:
         return self._answers
```

### Comparing `rustplus-5.5.8/rustplus/conversation/conversation_factory.py` & `rustplus-5.6.0/rustplus/conversation/conversation_factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
         self.api = api
         self.conversations = {}
         self.expires = {}
         self.gc_thread = Thread(target=self.garbage_collect, daemon=True)
         self.gc_thread.start()
 
     def create_conversation(self, steamid: int) -> Conversation:
-
         if steamid in self.conversations:
             raise ValueError("Conversation already exists")
 
         return Conversation(
             api=self.api, target=steamid, register=self._register_conversation
         )
```

### Comparing `rustplus-5.5.8/rustplus/exceptions/exceptions.py` & `rustplus-5.6.0/rustplus/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.8/rustplus/utils/deprecated.py` & `rustplus-5.6.0/rustplus/utils/deprecated.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
     """
     This is a decorator which can be used to mark functions
     as deprecated. It will result in a warning being emitted
     when the function is used.
     """
 
     def decorator(func1):
-
         if inspect.isclass(func1):
             fmt1 = "Call to deprecated class {name} ({reason})."
         else:
             fmt1 = "Call to deprecated function {name} ({reason})."
 
         @functools.wraps(func1)
         def new_func1(*args, **kwargs):
```

### Comparing `rustplus-5.5.8/rustplus/utils/grab_items.py` & `rustplus-5.6.0/rustplus/utils/grab_items.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Union
+
 import requests
 import json
 
 item_ids = {
     "-2139580305": "Auto Turret",
     "-2124352573": "Acoustic Guitar",
     "-2123125470": "Advanced Healing Tea",
@@ -721,15 +723,15 @@
     "2126889441": "Santa Beard",
     "2133269020": "Red Berry Clone",
     "-1843426638": "MLRS Rocket",
     "343045591": "MLRS Aiming Module",
 }
 
 
-def translate_id_to_stack(value_id: int) -> str:
+def translate_id_to_stack(value_id: Union[str, int]) -> str:
     global item_ids
     try:
         return item_ids[str(value_id)]
     except KeyError:
         return "Not Found"
```

### Comparing `rustplus-5.5.8/rustplus/utils/rust_utils.py` & `rustplus-5.6.0/rustplus/utils/rust_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 from importlib import resources
 from typing import Tuple
 from PIL import Image
 import logging
 import string
 
+from ..api.remote.rustplus_proto import AppMessage
 from ..api.structures import RustTime
 
 icons_path = "rustplus.api.icons"
 
 
-def format_time(protobuf) -> RustTime:
+def format_time(protobuf: AppMessage) -> RustTime:
     def convert_time(time) -> str:
         hours, minutes = divmod(time * 60, 60)
 
         return (
             f"{int(hours)}:0{int(minutes)}"
             if minutes <= 9
             else f"{int(hours)}:{int(minutes)}"
         )
 
     sunrise = convert_time(protobuf.response.time.sunrise)
     sunset = convert_time(protobuf.response.time.sunset)
     parsed_time = convert_time(protobuf.response.time.time)
 
     return RustTime(
-        protobuf.response.time.dayLengthMinutes,
+        protobuf.response.time.day_length_minutes,
         sunrise,
         sunset,
         parsed_time,
         protobuf.response.time.time,
-        protobuf.response.time.timeScale,
+        protobuf.response.time.time_scale,
     )
 
 
 def format_coord(x, y, map_size) -> tuple:
     y = map_size - y - 75
     x -= 75
```

### Comparing `rustplus-5.5.8/rustplus/utils/server_id.py` & `rustplus-5.6.0/rustplus/utils/server_id.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.8/rustplus.egg-info/PKG-INFO` & `rustplus-5.6.0/rustplus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rustplus
-Version: 5.5.8
+Version: 5.6.0
 Summary: A python wrapper for the Rust Plus API
 Home-page: https://github.com/olijeffers0n/rustplus
 Author: olijeffers0n
 License: MIT
 Project-URL: Issue tracker, https://github.com/olijeffers0n/rustplus/issues
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
```

### Comparing `rustplus-5.5.8/rustplus.egg-info/SOURCES.txt` & `rustplus-5.6.0/rustplus.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 rustplus/api/remote/events/event_handler.py
 rustplus/api/remote/events/event_loop_manager.py
 rustplus/api/remote/events/events.py
 rustplus/api/remote/events/handler_list.py
 rustplus/api/remote/events/map_event_listener.py
 rustplus/api/remote/events/registered_listener.py
 rustplus/api/remote/rustplus_proto/__init__.py
-rustplus/api/remote/rustplus_proto/rustplus_pb2.py
+rustplus/api/remote/rustplus_proto/rustplus.py
 rustplus/api/structures/__init__.py
 rustplus/api/structures/rust_chat_message.py
 rustplus/api/structures/rust_contents.py
 rustplus/api/structures/rust_entity_info.py
 rustplus/api/structures/rust_info.py
 rustplus/api/structures/rust_item.py
 rustplus/api/structures/rust_map.py
@@ -94,8 +94,11 @@
 rustplus/conversation/conversation_prompt.py
 rustplus/exceptions/__init__.py
 rustplus/exceptions/exceptions.py
 rustplus/utils/__init__.py
 rustplus/utils/deprecated.py
 rustplus/utils/grab_items.py
 rustplus/utils/rust_utils.py
-rustplus/utils/server_id.py
+rustplus/utils/server_id.py
+rustplus/utils/yielding_event.py
+rustplus/utils/fonts/PermanentMarker.ttf
+rustplus/utils/fonts/__init__.py
```

### Comparing `rustplus-5.5.8/setup.py` & `rustplus-5.6.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,14 +3,19 @@
 version = ""
 with open("rustplus/__init__.py") as input_file:
     for line in input_file.readlines():
         if line.startswith("__version__"):
             version = line.strip("__version__ =").strip().strip('"')
             break
 
+requirements = []
+with open("requirements.txt") as input_file:
+    for line in input_file.readlines():
+        requirements.append(line.strip())
+
 with open("README.md", errors='ignore') as input_file:
     readme = input_file.read()
 
 setup(
     name='rustplus',
     author='olijeffers0n',
     url='https://github.com/olijeffers0n/rustplus',
@@ -20,18 +25,10 @@
     version=version,
     packages=find_packages(include=['rustplus', 'rustplus.*']),
     license='MIT',
     description='A python wrapper for the Rust Plus API',
     long_description=readme,
     include_package_data=True,
     long_description_content_type='text/markdown',
-    install_requires=[
-        "websocket_client",
-        "Pillow",
-        "protobuf==4.21.6",
-        "asyncio",
-        "rustPlusPushReceiver==0.4.1",
-        "http-ece",
-        "requests"
-    ],
+    install_requires=requirements,
     python_requires='>=3.8.0',
 )
```

