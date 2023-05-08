# Comparing `tmp/pssapi-0.1.0.tar.gz` & `tmp/pssapi-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pssapi-0.1.0.tar", last modified: Mon May  8 10:09:59 2023, max compression
+gzip compressed data, was "pssapi-0.1.1.tar", last modified: Mon May  8 11:58:10 2023, max compression
```

## Comparing `pssapi-0.1.0.tar` & `pssapi-0.1.1.tar`

### file list

```diff
@@ -1,347 +1,347 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:09:59.365210 pssapi-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:09:59.329210 pssapi-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:09:59.333210 pssapi-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-08 10:09:45.000000 pssapi-0.1.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-08 10:09:45.000000 pssapi-0.1.0/.github/workflows/python-app.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1290 2023-05-08 10:09:45.000000 pssapi-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-08 10:09:45.000000 pssapi-0.1.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-08 10:09:45.000000 pssapi-0.1.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-08 10:09:59.365210 pssapi-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-08 10:09:45.000000 pssapi-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-08 10:09:45.000000 pssapi-0.1.0/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-08 10:09:45.000000 pssapi-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-08 10:09:45.000000 pssapi-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-08 10:09:59.369211 pssapi-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-08 10:09:45.000000 pssapi-0.1.0/showcase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:09:59.329210 pssapi-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:09:59.333210 pssapi-0.1.0/src/pssapi/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9191 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/client_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:09:59.341210 pssapi-0.1.0/src/pssapi/entities/
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/achievement_design.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/action_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/add_starbux.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/alliance.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/animation.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/background.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/battle.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/challenge_design.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/character.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/character_action.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/character_design.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/character_design_action.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/character_part.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/collection_design.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/condition_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/craft_design.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/division_design.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/draw_design.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/entity_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/friend.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/get_catalog_quantity.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/get_current_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/history.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/item.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/item_design.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/item_design_action.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/league.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/list_friends.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/live_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/message.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/missile_design.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/mission_design.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/mission_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/news_design.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/planet.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/prestige.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/promotion_design.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:09:59.345210 pssapi-0.1.0/src/pssapi/entities/raw/
--rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/achievement_design_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/action_type_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/add_starbux_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/alliance_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/animation_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/asset_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/background_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)    16784 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/battle_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     7813 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/challenge_design_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/character_action_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/character_design_action_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)    14337 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/character_design_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/character_part_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     8756 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/character_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/collection_design_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/condition_type_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/craft_design_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/division_design_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/draw_design_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/entity_base_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/file_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/friend_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/get_catalog_quantity_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/get_current_resources_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/history_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/item_design_action_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)    14590 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/item_design_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/item_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/league_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/list_friends_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     9147 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/live_ops_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/message_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     9230 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/missile_design_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     7963 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/mission_design_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/mission_event_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/news_design_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/planet_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/prestige_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)    10492 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/promotion_design_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/research_design_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/research_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/reward_design_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/room_action_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/room_design_purchase_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)    12719 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/room_design_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/room_design_sprite_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/room_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     4280 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/sale_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/season_design_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)    38318 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/setting_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)    14406 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/ship_design_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)    10469 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/ship_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/situation_design_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/sprite_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/star_system_link_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)    11839 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/star_system_marker_generator_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)    11134 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/star_system_marker_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/star_system_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/task_design_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     7068 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/training_design_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/user_email_password_authorize_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/user_login_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/user_marker_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)    29770 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/user_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/user_season_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/raw/user_star_system_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/research.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/research_design.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/reward_design.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/room.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/room_action.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/room_design.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/room_design_purchase.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/room_design_sprite.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/sale.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/season_design.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/setting.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/ship.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/ship_design.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/situation_design.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/sprite.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/star_system.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/star_system_link.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/star_system_marker.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/star_system_marker_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/task_design.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/training_design.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/user.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/user_email_password_authorize.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/user_login.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/user_marker.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/user_season.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/entities/user_star_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:09:59.357210 pssapi-0.1.0/src/pssapi/enums/
--rw-r--r--   0 runner    (1001) docker     (123)     6728 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/achievement_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/action_type_category.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/action_type_parameter_relativity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/activity_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/alliance_membership.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/ammo_category.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/animation_effect_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/argument.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/asset_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/authentication_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/background_effect_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/background_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/battle_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/behavior_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/category_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/challenge_scoring_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/challenge_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/change_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/character_design_flag_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/character_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/character_part_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/checksum_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/collection_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/completion_value_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/condition_type_category.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/condition_type_comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/condition_type_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/cost_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/craft_attack_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/craft_target_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/currency_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/daily_reward_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/daily_reward_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/device_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/division_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/download_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/draw_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/duration_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/email_verification_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/enhancement_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/environment_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/explosion_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/file_download_category.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/flight_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/friend_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/gender_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/generation_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/guide_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/hazard_category.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/hazard_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/history_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/item_design_flag_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/item_sub_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/item_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/language_key.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/league_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/marker_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/matching_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/message_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/missile_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/mission_design_flag.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/mission_design_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/mission_design_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/mission_event_flag.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/mission_event_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/module_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/movement_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/objective_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/orbit_anchor_alignment.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/outcome_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/progression_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/promotion_design_flag.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/promotion_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/purchase_vip_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/race_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/rarity.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/research_design_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/research_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/reward_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/room_design_sprite_flag.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/room_effect_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/room_sprite_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/room_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/room_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/sale_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/sale_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/season_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/setting_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/ship_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/ship_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/situation_design_flag.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/situation_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/special_ability_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/special_rule_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/status.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/target_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/task_category.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/task_design_flags_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/training_animation_style.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/trigger_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/user_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/user_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/enums/visibility_flags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:09:59.357210 pssapi-0.1.0/src/pssapi/raw/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/raw/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:09:59.361210 pssapi-0.1.0/src/pssapi/services/
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/services/achievement_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/services/alliance_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/services/animation_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/services/background_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/services/challenge_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/services/character_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/services/collection_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     6245 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/services/design_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/services/division_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/services/file_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/services/galaxy_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/services/history_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/services/item_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/services/ladder_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/services/league_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/services/live_ops_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/services/market_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/services/message_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/services/mission_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/services/promotion_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:09:59.365210 pssapi-0.1.0/src/pssapi/services/raw/
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/services/raw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/services/raw/achievement_service_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/services/raw/alliance_service_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/services/raw/animation_service_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/services/raw/background_service_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/services/raw/challenge_service_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/services/raw/character_service_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/services/raw/collection_service_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)    14935 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/services/raw/design_service_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/services/raw/division_service_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/services/raw/file_service_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/services/raw/galaxy_service_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/services/raw/history_service_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/services/raw/item_service_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/services/raw/ladder_service_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/services/raw/league_service_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/services/raw/live_ops_service_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/services/raw/market_service_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/services/raw/message_service_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/services/raw/mission_service_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/services/raw/promotion_service_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/services/raw/research_service_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/services/raw/reward_service_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/services/raw/room_design_sprite_service_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/services/raw/room_service_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/services/raw/season_service_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/services/raw/setting_service_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/services/raw/ship_service_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/services/raw/situation_service_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/services/raw/task_service_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/services/raw/training_service_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/services/raw/user_service_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/services/research_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/services/reward_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/services/room_design_sprite_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/services/room_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/services/season_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/services/service_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/services/setting_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/services/ship_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/services/situation_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/services/task_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/services/training_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/services/user_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:09:59.365210 pssapi-0.1.0/src/pssapi/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/utils/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-08 10:09:45.000000 pssapi-0.1.0/src/pssapi/utils/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:09:59.333210 pssapi-0.1.0/src/pssapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-08 10:09:59.000000 pssapi-0.1.0/src/pssapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12544 2023-05-08 10:09:59.000000 pssapi-0.1.0/src/pssapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 10:09:59.000000 pssapi-0.1.0/src/pssapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-08 10:09:59.000000 pssapi-0.1.0/src/pssapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-08 10:09:59.000000 pssapi-0.1.0/src/pssapi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:09:59.365210 pssapi-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-08 10:09:45.000000 pssapi-0.1.0/tests/test_core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:09:59.365210 pssapi-0.1.0/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-05-08 10:09:45.000000 pssapi-0.1.0/tests/utils/test_parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:58:10.030537 pssapi-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:58:09.994538 pssapi-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:58:09.994538 pssapi-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-08 11:58:02.000000 pssapi-0.1.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-08 11:58:02.000000 pssapi-0.1.1/.github/workflows/python-app.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1290 2023-05-08 11:58:02.000000 pssapi-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-08 11:58:02.000000 pssapi-0.1.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-08 11:58:02.000000 pssapi-0.1.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-08 11:58:10.030537 pssapi-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-08 11:58:02.000000 pssapi-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-08 11:58:02.000000 pssapi-0.1.1/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-08 11:58:02.000000 pssapi-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-08 11:58:02.000000 pssapi-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-08 11:58:10.030537 pssapi-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-08 11:58:02.000000 pssapi-0.1.1/showcase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:58:09.994538 pssapi-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:58:09.998538 pssapi-0.1.1/src/pssapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9191 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/client_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:58:10.006538 pssapi-0.1.1/src/pssapi/entities/
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/achievement_design.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/action_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/add_starbux.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/alliance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/background.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/battle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/challenge_design.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/character.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/character_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/character_design.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/character_design_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/character_part.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/collection_design.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/condition_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/craft_design.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/division_design.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/draw_design.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/entity_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/friend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/get_catalog_quantity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/get_current_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/item_design.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/item_design_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/league.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/list_friends.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/live_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/missile_design.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/mission_design.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/mission_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/news_design.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/planet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/prestige.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/promotion_design.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:58:10.010538 pssapi-0.1.1/src/pssapi/entities/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/achievement_design_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/action_type_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/add_starbux_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/alliance_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/animation_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/asset_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/background_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16784 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/battle_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7813 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/challenge_design_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/character_action_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/character_design_action_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14337 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/character_design_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/character_part_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8756 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/character_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/collection_design_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/condition_type_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/craft_design_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/division_design_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/draw_design_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/entity_base_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/file_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/friend_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/get_catalog_quantity_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/get_current_resources_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/history_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/item_design_action_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14590 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/item_design_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/item_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/league_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/list_friends_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9147 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/live_ops_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/message_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9230 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/missile_design_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7963 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/mission_design_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/mission_event_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/news_design_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/planet_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/prestige_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10492 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/promotion_design_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/research_design_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/research_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/reward_design_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/room_action_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/room_design_purchase_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12719 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/room_design_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/room_design_sprite_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/room_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4280 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/sale_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/season_design_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38318 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/setting_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14406 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/ship_design_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10469 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/ship_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/situation_design_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/sprite_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/star_system_link_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11839 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/star_system_marker_generator_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11134 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/star_system_marker_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/star_system_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/task_design_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7068 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/training_design_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/user_email_password_authorize_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/user_login_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/user_marker_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29770 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/user_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/user_season_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/raw/user_star_system_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/research.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/research_design.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/reward_design.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/room.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/room_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/room_design.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/room_design_purchase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/room_design_sprite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/sale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/season_design.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/ship.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/ship_design.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/situation_design.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/sprite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/star_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/star_system_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/star_system_marker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/star_system_marker_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/task_design.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/training_design.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/user_email_password_authorize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/user_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/user_marker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/user_season.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/entities/user_star_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:58:10.022538 pssapi-0.1.1/src/pssapi/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)     6728 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/achievement_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/action_type_category.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/action_type_parameter_relativity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/activity_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/alliance_membership.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/ammo_category.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/animation_effect_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/argument.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/asset_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/authentication_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/background_effect_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/background_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/battle_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/behavior_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/category_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/challenge_scoring_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/challenge_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/change_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/character_design_flag_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/character_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/character_part_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/checksum_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/collection_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/completion_value_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/condition_type_category.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/condition_type_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/condition_type_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/cost_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/craft_attack_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/craft_target_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/currency_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/daily_reward_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/daily_reward_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/device_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/division_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/download_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/draw_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/duration_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/email_verification_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/enhancement_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/environment_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/explosion_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/file_download_category.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/flight_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/friend_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/gender_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/generation_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/guide_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/hazard_category.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/hazard_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/history_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/item_design_flag_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/item_sub_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/item_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/language_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/league_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/marker_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/matching_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/message_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/missile_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/mission_design_flag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/mission_design_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/mission_design_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/mission_event_flag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/mission_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/module_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/movement_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/objective_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/orbit_anchor_alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/outcome_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/progression_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/promotion_design_flag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/promotion_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/purchase_vip_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/race_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/rarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/research_design_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/research_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/reward_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/room_design_sprite_flag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/room_effect_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/room_sprite_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/room_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/room_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/sale_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/sale_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/season_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/setting_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/ship_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/ship_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/situation_design_flag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/situation_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/special_ability_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/special_rule_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/target_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/task_category.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/task_design_flags_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/training_animation_style.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/trigger_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/user_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/user_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/enums/visibility_flags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:58:10.022538 pssapi-0.1.1/src/pssapi/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/raw/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:58:10.026538 pssapi-0.1.1/src/pssapi/services/
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/services/achievement_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/services/alliance_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/services/animation_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/services/background_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/services/challenge_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/services/character_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/services/collection_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6245 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/services/design_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/services/division_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/services/file_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/services/galaxy_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/services/history_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/services/item_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/services/ladder_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/services/league_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/services/live_ops_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/services/market_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/services/message_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/services/mission_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/services/promotion_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:58:10.030537 pssapi-0.1.1/src/pssapi/services/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/services/raw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/services/raw/achievement_service_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/services/raw/alliance_service_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/services/raw/animation_service_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/services/raw/background_service_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/services/raw/challenge_service_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/services/raw/character_service_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/services/raw/collection_service_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14935 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/services/raw/design_service_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/services/raw/division_service_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/services/raw/file_service_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/services/raw/galaxy_service_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/services/raw/history_service_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/services/raw/item_service_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/services/raw/ladder_service_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/services/raw/league_service_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/services/raw/live_ops_service_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/services/raw/market_service_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/services/raw/message_service_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/services/raw/mission_service_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/services/raw/promotion_service_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/services/raw/research_service_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/services/raw/reward_service_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/services/raw/room_design_sprite_service_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/services/raw/room_service_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/services/raw/season_service_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/services/raw/setting_service_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/services/raw/ship_service_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/services/raw/situation_service_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/services/raw/task_service_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/services/raw/training_service_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/services/raw/user_service_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/services/research_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/services/reward_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/services/room_design_sprite_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/services/room_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/services/season_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/services/service_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/services/setting_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/services/ship_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/services/situation_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/services/task_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/services/training_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/services/user_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:58:10.030537 pssapi-0.1.1/src/pssapi/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/utils/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-08 11:58:02.000000 pssapi-0.1.1/src/pssapi/utils/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:58:09.998538 pssapi-0.1.1/src/pssapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-08 11:58:09.000000 pssapi-0.1.1/src/pssapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12544 2023-05-08 11:58:09.000000 pssapi-0.1.1/src/pssapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 11:58:09.000000 pssapi-0.1.1/src/pssapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-08 11:58:09.000000 pssapi-0.1.1/src/pssapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-08 11:58:09.000000 pssapi-0.1.1/src/pssapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:58:10.030537 pssapi-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-08 11:58:02.000000 pssapi-0.1.1/tests/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:58:10.030537 pssapi-0.1.1/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-05-08 11:58:02.000000 pssapi-0.1.1/tests/utils/test_parse.py
```

### Comparing `pssapi-0.1.0/.github/workflows/python-app.yml` & `pssapi-0.1.1/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/.gitignore` & `pssapi-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/LICENSE.md` & `pssapi-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/Makefile` & `pssapi-0.1.1/Makefile`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/dev-requirements.txt` & `pssapi-0.1.1/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/pyproject.toml` & `pssapi-0.1.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pssapi"
-version = "0.1.0"
+dynamic = ["version"]
 authors = [
     { name = "The worst.", email = "theworstpss@gmail.com" },
     { name = "Solevis" },
 ]
 description = "Wrapper for the Pixel Starships API"
 readme = "README.md"
 requires-python = ">=3.11"
```

### Comparing `pssapi-0.1.0/requirements.txt` & `pssapi-0.1.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/setup.cfg` & `pssapi-0.1.1/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -20,15 +20,19 @@
 url = https://github.com/PSS-Tools-Development/pssapi.py
 project_urls = 
 	Bug Tracker = https://github.com/PSS-Tools-Development/pssapi.py/issues
 	Changelog = https://github.com/PSS-Tools-Development/pssapi.py/releases
 classifiers = 
 	Programming Language :: Python :: 3.11
 	License :: OSI Approved :: MIT License
+	Development Status :: 3 - Alpha
 	Intended Audience :: Developers
+	Topic :: Software Development :: Libraries
+	Natural Language :: English
+	Operating System :: OS Independent
 
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.11
```

### Comparing `pssapi-0.1.0/showcase.py` & `pssapi-0.1.1/showcase.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/client_base.py` & `pssapi-0.1.1/src/pssapi/client_base.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/core.py` & `pssapi-0.1.1/src/pssapi/core.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/__init__.py` & `pssapi-0.1.1/src/pssapi/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/__init__.py` & `pssapi-0.1.1/src/pssapi/entities/raw/__init__.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/achievement_design_raw.py` & `pssapi-0.1.1/src/pssapi/entities/raw/achievement_design_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/action_type_raw.py` & `pssapi-0.1.1/src/pssapi/entities/raw/action_type_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/add_starbux_raw.py` & `pssapi-0.1.1/src/pssapi/entities/raw/add_starbux_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/alliance_raw.py` & `pssapi-0.1.1/src/pssapi/entities/raw/alliance_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/animation_raw.py` & `pssapi-0.1.1/src/pssapi/entities/raw/animation_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/asset_raw.py` & `pssapi-0.1.1/src/pssapi/entities/raw/asset_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/background_raw.py` & `pssapi-0.1.1/src/pssapi/entities/raw/background_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/battle_raw.py` & `pssapi-0.1.1/src/pssapi/entities/raw/battle_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/challenge_design_raw.py` & `pssapi-0.1.1/src/pssapi/entities/raw/challenge_design_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/character_action_raw.py` & `pssapi-0.1.1/src/pssapi/entities/raw/character_action_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/character_design_action_raw.py` & `pssapi-0.1.1/src/pssapi/entities/raw/character_design_action_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/character_design_raw.py` & `pssapi-0.1.1/src/pssapi/entities/raw/character_design_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/character_part_raw.py` & `pssapi-0.1.1/src/pssapi/entities/raw/character_part_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/character_raw.py` & `pssapi-0.1.1/src/pssapi/entities/raw/character_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/collection_design_raw.py` & `pssapi-0.1.1/src/pssapi/entities/raw/collection_design_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/condition_type_raw.py` & `pssapi-0.1.1/src/pssapi/entities/raw/condition_type_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/craft_design_raw.py` & `pssapi-0.1.1/src/pssapi/entities/raw/craft_design_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/division_design_raw.py` & `pssapi-0.1.1/src/pssapi/entities/raw/division_design_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/draw_design_raw.py` & `pssapi-0.1.1/src/pssapi/entities/raw/draw_design_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/entity_base_raw.py` & `pssapi-0.1.1/src/pssapi/entities/raw/entity_base_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/file_raw.py` & `pssapi-0.1.1/src/pssapi/entities/raw/file_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/friend_raw.py` & `pssapi-0.1.1/src/pssapi/entities/raw/friend_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/get_catalog_quantity_raw.py` & `pssapi-0.1.1/src/pssapi/entities/raw/get_catalog_quantity_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/get_current_resources_raw.py` & `pssapi-0.1.1/src/pssapi/entities/raw/get_current_resources_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/history_raw.py` & `pssapi-0.1.1/src/pssapi/entities/raw/history_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/item_design_action_raw.py` & `pssapi-0.1.1/src/pssapi/entities/raw/item_design_action_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/item_design_raw.py` & `pssapi-0.1.1/src/pssapi/entities/raw/item_design_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/item_raw.py` & `pssapi-0.1.1/src/pssapi/entities/raw/item_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/league_raw.py` & `pssapi-0.1.1/src/pssapi/entities/raw/league_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/list_friends_raw.py` & `pssapi-0.1.1/src/pssapi/entities/raw/list_friends_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/live_ops_raw.py` & `pssapi-0.1.1/src/pssapi/entities/raw/live_ops_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/message_raw.py` & `pssapi-0.1.1/src/pssapi/entities/raw/message_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/missile_design_raw.py` & `pssapi-0.1.1/src/pssapi/entities/raw/missile_design_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/mission_design_raw.py` & `pssapi-0.1.1/src/pssapi/entities/raw/mission_design_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/mission_event_raw.py` & `pssapi-0.1.1/src/pssapi/entities/raw/mission_event_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/news_design_raw.py` & `pssapi-0.1.1/src/pssapi/entities/raw/news_design_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/prestige_raw.py` & `pssapi-0.1.1/src/pssapi/entities/raw/prestige_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/promotion_design_raw.py` & `pssapi-0.1.1/src/pssapi/entities/raw/promotion_design_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/research_design_raw.py` & `pssapi-0.1.1/src/pssapi/entities/raw/research_design_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/research_raw.py` & `pssapi-0.1.1/src/pssapi/entities/raw/research_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/reward_design_raw.py` & `pssapi-0.1.1/src/pssapi/entities/raw/reward_design_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/room_action_raw.py` & `pssapi-0.1.1/src/pssapi/entities/raw/room_action_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/room_design_purchase_raw.py` & `pssapi-0.1.1/src/pssapi/entities/raw/room_design_purchase_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/room_design_raw.py` & `pssapi-0.1.1/src/pssapi/entities/raw/room_design_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/room_design_sprite_raw.py` & `pssapi-0.1.1/src/pssapi/entities/raw/room_design_sprite_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/room_raw.py` & `pssapi-0.1.1/src/pssapi/entities/raw/room_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/sale_raw.py` & `pssapi-0.1.1/src/pssapi/entities/raw/sale_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/season_design_raw.py` & `pssapi-0.1.1/src/pssapi/entities/raw/season_design_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/setting_raw.py` & `pssapi-0.1.1/src/pssapi/entities/raw/setting_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/ship_design_raw.py` & `pssapi-0.1.1/src/pssapi/entities/raw/ship_design_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/ship_raw.py` & `pssapi-0.1.1/src/pssapi/entities/raw/ship_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/situation_design_raw.py` & `pssapi-0.1.1/src/pssapi/entities/raw/situation_design_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/sprite_raw.py` & `pssapi-0.1.1/src/pssapi/entities/raw/sprite_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/star_system_link_raw.py` & `pssapi-0.1.1/src/pssapi/entities/raw/star_system_link_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/star_system_marker_generator_raw.py` & `pssapi-0.1.1/src/pssapi/entities/raw/star_system_marker_generator_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/star_system_marker_raw.py` & `pssapi-0.1.1/src/pssapi/entities/raw/star_system_marker_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/star_system_raw.py` & `pssapi-0.1.1/src/pssapi/entities/raw/star_system_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/task_design_raw.py` & `pssapi-0.1.1/src/pssapi/entities/raw/task_design_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/training_design_raw.py` & `pssapi-0.1.1/src/pssapi/entities/raw/training_design_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/user_email_password_authorize_raw.py` & `pssapi-0.1.1/src/pssapi/entities/raw/user_email_password_authorize_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/user_login_raw.py` & `pssapi-0.1.1/src/pssapi/entities/raw/user_login_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/user_marker_raw.py` & `pssapi-0.1.1/src/pssapi/entities/raw/user_marker_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/user_raw.py` & `pssapi-0.1.1/src/pssapi/entities/raw/user_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/user_season_raw.py` & `pssapi-0.1.1/src/pssapi/entities/raw/user_season_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/entities/raw/user_star_system_raw.py` & `pssapi-0.1.1/src/pssapi/entities/raw/user_star_system_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/enums/__init__.py` & `pssapi-0.1.1/src/pssapi/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/enums/achievement_type.py` & `pssapi-0.1.1/src/pssapi/enums/achievement_type.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/enums/activity_type.py` & `pssapi-0.1.1/src/pssapi/enums/activity_type.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/enums/change_type.py` & `pssapi-0.1.1/src/pssapi/enums/change_type.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/enums/condition_type_category.py` & `pssapi-0.1.1/src/pssapi/enums/condition_type_category.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/enums/condition_type_comparison.py` & `pssapi-0.1.1/src/pssapi/enums/condition_type_comparison.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/enums/condition_type_parameter.py` & `pssapi-0.1.1/src/pssapi/enums/condition_type_parameter.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/enums/currency_type.py` & `pssapi-0.1.1/src/pssapi/enums/currency_type.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/enums/device_type.py` & `pssapi-0.1.1/src/pssapi/enums/device_type.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/enums/enhancement_type.py` & `pssapi-0.1.1/src/pssapi/enums/enhancement_type.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/enums/item_design_flag_type.py` & `pssapi-0.1.1/src/pssapi/enums/item_design_flag_type.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/enums/item_sub_type.py` & `pssapi-0.1.1/src/pssapi/enums/item_sub_type.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/enums/objective_type.py` & `pssapi-0.1.1/src/pssapi/enums/objective_type.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/enums/research_design_type.py` & `pssapi-0.1.1/src/pssapi/enums/research_design_type.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/enums/room_type.py` & `pssapi-0.1.1/src/pssapi/enums/room_type.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/enums/setting_flags.py` & `pssapi-0.1.1/src/pssapi/enums/setting_flags.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/enums/special_ability_type.py` & `pssapi-0.1.1/src/pssapi/enums/special_ability_type.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/enums/user_type.py` & `pssapi-0.1.1/src/pssapi/enums/user_type.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/services/__init__.py` & `pssapi-0.1.1/src/pssapi/services/__init__.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/services/achievement_service.py` & `pssapi-0.1.1/src/pssapi/services/achievement_service.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/services/alliance_service.py` & `pssapi-0.1.1/src/pssapi/services/alliance_service.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/services/animation_service.py` & `pssapi-0.1.1/src/pssapi/services/animation_service.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/services/background_service.py` & `pssapi-0.1.1/src/pssapi/services/background_service.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/services/challenge_service.py` & `pssapi-0.1.1/src/pssapi/services/challenge_service.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/services/character_service.py` & `pssapi-0.1.1/src/pssapi/services/character_service.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/services/collection_service.py` & `pssapi-0.1.1/src/pssapi/services/collection_service.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/services/design_service.py` & `pssapi-0.1.1/src/pssapi/services/design_service.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/services/division_service.py` & `pssapi-0.1.1/src/pssapi/services/division_service.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/services/file_service.py` & `pssapi-0.1.1/src/pssapi/services/file_service.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/services/galaxy_service.py` & `pssapi-0.1.1/src/pssapi/services/galaxy_service.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/services/item_service.py` & `pssapi-0.1.1/src/pssapi/services/item_service.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/services/ladder_service.py` & `pssapi-0.1.1/src/pssapi/services/ladder_service.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/services/league_service.py` & `pssapi-0.1.1/src/pssapi/services/league_service.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/services/live_ops_service.py` & `pssapi-0.1.1/src/pssapi/services/live_ops_service.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/services/market_service.py` & `pssapi-0.1.1/src/pssapi/services/market_service.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/services/message_service.py` & `pssapi-0.1.1/src/pssapi/services/message_service.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/services/mission_service.py` & `pssapi-0.1.1/src/pssapi/services/mission_service.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/services/promotion_service.py` & `pssapi-0.1.1/src/pssapi/services/promotion_service.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/services/raw/__init__.py` & `pssapi-0.1.1/src/pssapi/services/raw/__init__.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/services/raw/achievement_service_raw.py` & `pssapi-0.1.1/src/pssapi/services/raw/achievement_service_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/services/raw/alliance_service_raw.py` & `pssapi-0.1.1/src/pssapi/services/raw/alliance_service_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/services/raw/animation_service_raw.py` & `pssapi-0.1.1/src/pssapi/services/raw/animation_service_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/services/raw/background_service_raw.py` & `pssapi-0.1.1/src/pssapi/services/raw/background_service_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/services/raw/challenge_service_raw.py` & `pssapi-0.1.1/src/pssapi/services/raw/challenge_service_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/services/raw/character_service_raw.py` & `pssapi-0.1.1/src/pssapi/services/raw/character_service_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/services/raw/collection_service_raw.py` & `pssapi-0.1.1/src/pssapi/services/raw/collection_service_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/services/raw/design_service_raw.py` & `pssapi-0.1.1/src/pssapi/services/raw/design_service_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/services/raw/division_service_raw.py` & `pssapi-0.1.1/src/pssapi/services/raw/division_service_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/services/raw/file_service_raw.py` & `pssapi-0.1.1/src/pssapi/services/raw/file_service_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/services/raw/galaxy_service_raw.py` & `pssapi-0.1.1/src/pssapi/services/raw/galaxy_service_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/services/raw/history_service_raw.py` & `pssapi-0.1.1/src/pssapi/services/raw/history_service_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/services/raw/item_service_raw.py` & `pssapi-0.1.1/src/pssapi/services/raw/item_service_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/services/raw/ladder_service_raw.py` & `pssapi-0.1.1/src/pssapi/services/raw/ladder_service_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/services/raw/league_service_raw.py` & `pssapi-0.1.1/src/pssapi/services/raw/league_service_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/services/raw/live_ops_service_raw.py` & `pssapi-0.1.1/src/pssapi/services/raw/live_ops_service_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/services/raw/market_service_raw.py` & `pssapi-0.1.1/src/pssapi/services/raw/market_service_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/services/raw/message_service_raw.py` & `pssapi-0.1.1/src/pssapi/services/raw/message_service_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/services/raw/mission_service_raw.py` & `pssapi-0.1.1/src/pssapi/services/raw/mission_service_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/services/raw/promotion_service_raw.py` & `pssapi-0.1.1/src/pssapi/services/raw/promotion_service_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/services/raw/research_service_raw.py` & `pssapi-0.1.1/src/pssapi/services/raw/research_service_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/services/raw/reward_service_raw.py` & `pssapi-0.1.1/src/pssapi/services/raw/reward_service_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/services/raw/room_design_sprite_service_raw.py` & `pssapi-0.1.1/src/pssapi/services/raw/room_design_sprite_service_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/services/raw/room_service_raw.py` & `pssapi-0.1.1/src/pssapi/services/raw/room_service_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/services/raw/season_service_raw.py` & `pssapi-0.1.1/src/pssapi/services/raw/season_service_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/services/raw/setting_service_raw.py` & `pssapi-0.1.1/src/pssapi/services/raw/setting_service_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/services/raw/ship_service_raw.py` & `pssapi-0.1.1/src/pssapi/services/raw/ship_service_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/services/raw/situation_service_raw.py` & `pssapi-0.1.1/src/pssapi/services/raw/situation_service_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/services/raw/task_service_raw.py` & `pssapi-0.1.1/src/pssapi/services/raw/task_service_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/services/raw/training_service_raw.py` & `pssapi-0.1.1/src/pssapi/services/raw/training_service_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/services/raw/user_service_raw.py` & `pssapi-0.1.1/src/pssapi/services/raw/user_service_raw.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/services/research_service.py` & `pssapi-0.1.1/src/pssapi/services/research_service.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/services/reward_service.py` & `pssapi-0.1.1/src/pssapi/services/reward_service.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/services/room_design_sprite_service.py` & `pssapi-0.1.1/src/pssapi/services/room_design_sprite_service.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/services/room_service.py` & `pssapi-0.1.1/src/pssapi/services/room_service.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/services/season_service.py` & `pssapi-0.1.1/src/pssapi/services/season_service.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/services/service_base.py` & `pssapi-0.1.1/src/pssapi/services/service_base.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/services/setting_service.py` & `pssapi-0.1.1/src/pssapi/services/setting_service.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/services/ship_service.py` & `pssapi-0.1.1/src/pssapi/services/ship_service.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/services/situation_service.py` & `pssapi-0.1.1/src/pssapi/services/situation_service.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/services/task_service.py` & `pssapi-0.1.1/src/pssapi/services/task_service.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/services/training_service.py` & `pssapi-0.1.1/src/pssapi/services/training_service.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/services/user_service.py` & `pssapi-0.1.1/src/pssapi/services/user_service.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi/utils/parse.py` & `pssapi-0.1.1/src/pssapi/utils/parse.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/src/pssapi.egg-info/SOURCES.txt` & `pssapi-0.1.1/src/pssapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/tests/test_core.py` & `pssapi-0.1.1/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `pssapi-0.1.0/tests/utils/test_parse.py` & `pssapi-0.1.1/tests/utils/test_parse.py`

 * *Files identical despite different names*

