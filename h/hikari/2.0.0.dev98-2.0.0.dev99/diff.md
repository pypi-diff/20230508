# Comparing `tmp/hikari-2.0.0.dev98.tar.gz` & `tmp/hikari-2.0.0.dev99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hikari-2.0.0.dev98.tar", last modified: Thu Jan 14 12:49:55 2021, max compression
+gzip compressed data, was "hikari-2.0.0.dev99.tar", last modified: Sat Jan 16 10:03:50 2021, max compression
```

## Comparing `hikari-2.0.0.dev98.tar` & `hikari-2.0.0.dev99.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-14 12:49:55.423911 hikari-2.0.0.dev98/
--rw-r--r--   0 runner    (1001) docker     (116)     1078 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      170 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)    12371 2021-01-14 12:49:55.423911 hikari-2.0.0.dev98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     8836 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-14 12:49:55.415911 hikari-2.0.0.dev98/hikari/
--rw-r--r--   0 runner    (1001) docker     (116)     3503 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1722 2021-01-14 12:49:54.000000 hikari-2.0.0.dev98/hikari/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (116)     1290 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/__main__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1906 2021-01-14 12:49:34.000000 hikari-2.0.0.dev98/hikari/_about.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-14 12:49:55.419911 hikari-2.0.0.dev98/hikari/api/
--rw-r--r--   0 runner    (1001) docker     (116)     1465 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    48574 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/api/cache.py
--rw-r--r--   0 runner    (1001) docker     (116)    36066 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/api/entity_factory.py
--rw-r--r--   0 runner    (1001) docker     (116)    14790 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/api/event_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (116)    28840 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/api/event_factory.py
--rw-r--r--   0 runner    (1001) docker     (116)   246526 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/api/rest.py
--rw-r--r--   0 runner    (1001) docker     (116)     9218 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/api/shard.py
--rw-r--r--   0 runner    (1001) docker     (116)    15460 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/api/special_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (116)     8213 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/api/voice.py
--rw-r--r--   0 runner    (1001) docker     (116)    16688 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/applications.py
--rw-r--r--   0 runner    (1001) docker     (116)    20481 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/audit_logs.py
--rw-r--r--   0 runner    (1001) docker     (116)     1098 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/banner.txt
--rw-r--r--   0 runner    (1001) docker     (116)    30929 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/channels.py
--rw-r--r--   0 runner    (1001) docker     (116)     2144 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/cli.py
--rw-r--r--   0 runner    (1001) docker     (116)    18698 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/colors.py
--rw-r--r--   0 runner    (1001) docker     (116)     1405 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/colours.py
--rw-r--r--   0 runner    (1001) docker     (116)    15449 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/config.py
--rw-r--r--   0 runner    (1001) docker     (116)    33779 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/embeds.py
--rw-r--r--   0 runner    (1001) docker     (116)    14001 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/emojis.py
--rw-r--r--   0 runner    (1001) docker     (116)    20030 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/errors.py
--rw-r--r--   0 runner    (1001) docker     (116)     9159 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/event_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-14 12:49:55.419911 hikari-2.0.0.dev98/hikari/events/
--rw-r--r--   0 runner    (1001) docker     (116)     1828 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      548 2021-01-14 12:49:54.000000 hikari-2.0.0.dev98/hikari/events/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (116)     8597 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/events/base_events.py
--rw-r--r--   0 runner    (1001) docker     (116)    21702 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/events/channel_events.py
--rw-r--r--   0 runner    (1001) docker     (116)    22707 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/events/guild_events.py
--rw-r--r--   0 runner    (1001) docker     (116)     5301 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/events/lifetime_events.py
--rw-r--r--   0 runner    (1001) docker     (116)     6437 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/events/member_events.py
--rw-r--r--   0 runner    (1001) docker     (116)    25512 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/events/message_events.py
--rw-r--r--   0 runner    (1001) docker     (116)    14235 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/events/reaction_events.py
--rw-r--r--   0 runner    (1001) docker     (116)     5215 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/events/role_events.py
--rw-r--r--   0 runner    (1001) docker     (116)     8597 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/events/shard_events.py
--rw-r--r--   0 runner    (1001) docker     (116)    10124 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/events/typing_events.py
--rw-r--r--   0 runner    (1001) docker     (116)     2341 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/events/user_events.py
--rw-r--r--   0 runner    (1001) docker     (116)     4979 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/events/voice_events.py
--rw-r--r--   0 runner    (1001) docker     (116)    36435 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/files.py
--rw-r--r--   0 runner    (1001) docker     (116)    54675 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/guilds.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-14 12:49:55.423911 hikari-2.0.0.dev98/hikari/impl/
--rw-r--r--   0 runner    (1001) docker     (116)     1487 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    44317 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/impl/bot.py
--rw-r--r--   0 runner    (1001) docker     (116)    26543 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/impl/buckets.py
--rw-r--r--   0 runner    (1001) docker     (116)    66102 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/impl/cache.py
--rw-r--r--   0 runner    (1001) docker     (116)    98041 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/impl/entity_factory.py
--rw-r--r--   0 runner    (1001) docker     (116)    28313 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/impl/event_factory.py
--rw-r--r--   0 runner    (1001) docker     (116)    22172 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/impl/event_manager.py
--rw-r--r--   0 runner    (1001) docker     (116)    12979 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/impl/event_manager_base.py
--rw-r--r--   0 runner    (1001) docker     (116)    19338 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/impl/rate_limits.py
--rw-r--r--   0 runner    (1001) docker     (116)   110990 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/impl/rest.py
--rw-r--r--   0 runner    (1001) docker     (116)    40971 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/impl/shard.py
--rw-r--r--   0 runner    (1001) docker     (116)    23764 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/impl/special_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (116)     9171 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/impl/voice.py
--rw-r--r--   0 runner    (1001) docker     (116)    11725 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/intents.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-14 12:49:55.423911 hikari-2.0.0.dev98/hikari/internal/
--rw-r--r--   0 runner    (1001) docker     (116)     1268 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     6525 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/internal/aio.py
--rw-r--r--   0 runner    (1001) docker     (116)     8820 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/internal/attr_extensions.py
--rw-r--r--   0 runner    (1001) docker     (116)    37693 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/internal/cache.py
--rw-r--r--   0 runner    (1001) docker     (116)    17189 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/internal/collections.py
--rw-r--r--   0 runner    (1001) docker     (116)    10976 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/internal/data_binding.py
--rw-r--r--   0 runner    (1001) docker     (116)    29632 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/internal/enums.py
--rw-r--r--   0 runner    (1001) docker     (116)     3443 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/internal/enums.pyi
--rw-r--r--   0 runner    (1001) docker     (116)     6267 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/internal/net.py
--rw-r--r--   0 runner    (1001) docker     (116)     3847 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/internal/reflect.py
--rw-r--r--   0 runner    (1001) docker     (116)    20215 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/internal/routes.py
--rw-r--r--   0 runner    (1001) docker     (116)     4673 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/internal/spel.py
--rw-r--r--   0 runner    (1001) docker     (116)     7594 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/internal/time.py
--rw-r--r--   0 runner    (1001) docker     (116)    13150 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/internal/ux.py
--rw-r--r--   0 runner    (1001) docker     (116)    11540 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/invites.py
--rw-r--r--   0 runner    (1001) docker     (116)    37049 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/iterators.py
--rw-r--r--   0 runner    (1001) docker     (116)    44984 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/messages.py
--rw-r--r--   0 runner    (1001) docker     (116)     6527 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/permissions.py
--rw-r--r--   0 runner    (1001) docker     (116)    10038 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/presences.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/py.typed
--rw-r--r--   0 runner    (1001) docker     (116)     3613 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/sessions.py
--rw-r--r--   0 runner    (1001) docker     (116)     7504 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/snowflakes.py
--rw-r--r--   0 runner    (1001) docker     (116)     7233 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/templates.py
--rw-r--r--   0 runner    (1001) docker     (116)    20706 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/traits.py
--rw-r--r--   0 runner    (1001) docker     (116)     4709 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/undefined.py
--rw-r--r--   0 runner    (1001) docker     (116)     1743 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/undefined.pyi
--rw-r--r--   0 runner    (1001) docker     (116)     1644 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/urls.py
--rw-r--r--   0 runner    (1001) docker     (116)    25173 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/users.py
--rw-r--r--   0 runner    (1001) docker     (116)     4741 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/voices.py
--rw-r--r--   0 runner    (1001) docker     (116)    28515 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/hikari/webhooks.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-14 12:49:55.415911 hikari-2.0.0.dev98/hikari.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)    12371 2021-01-14 12:49:55.000000 hikari-2.0.0.dev98/hikari.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2299 2021-01-14 12:49:55.000000 hikari-2.0.0.dev98/hikari.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-14 12:49:55.000000 hikari-2.0.0.dev98/hikari.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       44 2021-01-14 12:49:55.000000 hikari-2.0.0.dev98/hikari.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-14 12:49:55.000000 hikari-2.0.0.dev98/hikari.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)      134 2021-01-14 12:49:55.000000 hikari-2.0.0.dev98/hikari.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        7 2021-01-14 12:49:55.000000 hikari-2.0.0.dev98/hikari.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)     1296 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)       62 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2021-01-14 12:49:55.423911 hikari-2.0.0.dev98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     3927 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/setup.py
--rw-r--r--   0 runner    (1001) docker     (116)       60 2021-01-14 12:49:23.000000 hikari-2.0.0.dev98/speedup-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-16 10:03:50.961310 hikari-2.0.0.dev99/
+-rw-r--r--   0 runner    (1001) docker     (116)     1078 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)      170 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)    12371 2021-01-16 10:03:50.961310 hikari-2.0.0.dev99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     8836 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-16 10:03:50.953309 hikari-2.0.0.dev99/hikari/
+-rw-r--r--   0 runner    (1001) docker     (116)     3503 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1722 2021-01-16 10:03:50.000000 hikari-2.0.0.dev99/hikari/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (116)     1290 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1906 2021-01-16 10:03:26.000000 hikari-2.0.0.dev99/hikari/_about.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-16 10:03:50.953309 hikari-2.0.0.dev99/hikari/api/
+-rw-r--r--   0 runner    (1001) docker     (116)     1465 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    48574 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/api/cache.py
+-rw-r--r--   0 runner    (1001) docker     (116)    36066 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/api/entity_factory.py
+-rw-r--r--   0 runner    (1001) docker     (116)    14790 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/api/event_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (116)    28840 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/api/event_factory.py
+-rw-r--r--   0 runner    (1001) docker     (116)   246541 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/api/rest.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9218 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/api/shard.py
+-rw-r--r--   0 runner    (1001) docker     (116)    15460 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/api/special_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8213 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/api/voice.py
+-rw-r--r--   0 runner    (1001) docker     (116)    16688 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/applications.py
+-rw-r--r--   0 runner    (1001) docker     (116)    20481 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/audit_logs.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1098 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/banner.txt
+-rw-r--r--   0 runner    (1001) docker     (116)    30929 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/channels.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2151 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/cli.py
+-rw-r--r--   0 runner    (1001) docker     (116)    18698 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/colors.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1405 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/colours.py
+-rw-r--r--   0 runner    (1001) docker     (116)    15449 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/config.py
+-rw-r--r--   0 runner    (1001) docker     (116)    33779 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/embeds.py
+-rw-r--r--   0 runner    (1001) docker     (116)    14001 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/emojis.py
+-rw-r--r--   0 runner    (1001) docker     (116)    20030 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/errors.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9159 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/event_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-16 10:03:50.957310 hikari-2.0.0.dev99/hikari/events/
+-rw-r--r--   0 runner    (1001) docker     (116)     1828 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      548 2021-01-16 10:03:50.000000 hikari-2.0.0.dev99/hikari/events/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (116)     8597 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/events/base_events.py
+-rw-r--r--   0 runner    (1001) docker     (116)    21702 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/events/channel_events.py
+-rw-r--r--   0 runner    (1001) docker     (116)    22718 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/events/guild_events.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5301 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/events/lifetime_events.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6437 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/events/member_events.py
+-rw-r--r--   0 runner    (1001) docker     (116)    25512 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/events/message_events.py
+-rw-r--r--   0 runner    (1001) docker     (116)    14235 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/events/reaction_events.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5215 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/events/role_events.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8597 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/events/shard_events.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10124 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/events/typing_events.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2341 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/events/user_events.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4979 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/events/voice_events.py
+-rw-r--r--   0 runner    (1001) docker     (116)    36435 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/files.py
+-rw-r--r--   0 runner    (1001) docker     (116)    54675 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/guilds.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-16 10:03:50.957310 hikari-2.0.0.dev99/hikari/impl/
+-rw-r--r--   0 runner    (1001) docker     (116)     1487 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    44317 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/impl/bot.py
+-rw-r--r--   0 runner    (1001) docker     (116)    26543 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/impl/buckets.py
+-rw-r--r--   0 runner    (1001) docker     (116)    66102 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/impl/cache.py
+-rw-r--r--   0 runner    (1001) docker     (116)    98041 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/impl/entity_factory.py
+-rw-r--r--   0 runner    (1001) docker     (116)    28313 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/impl/event_factory.py
+-rw-r--r--   0 runner    (1001) docker     (116)    22166 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/impl/event_manager.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12979 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/impl/event_manager_base.py
+-rw-r--r--   0 runner    (1001) docker     (116)    19338 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/impl/rate_limits.py
+-rw-r--r--   0 runner    (1001) docker     (116)   110990 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/impl/rest.py
+-rw-r--r--   0 runner    (1001) docker     (116)    40971 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/impl/shard.py
+-rw-r--r--   0 runner    (1001) docker     (116)    23764 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/impl/special_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9171 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/impl/voice.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11725 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/intents.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-16 10:03:50.961310 hikari-2.0.0.dev99/hikari/internal/
+-rw-r--r--   0 runner    (1001) docker     (116)     1268 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6525 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/internal/aio.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8820 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/internal/attr_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (116)    37693 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/internal/cache.py
+-rw-r--r--   0 runner    (1001) docker     (116)    17189 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/internal/collections.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10976 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/internal/data_binding.py
+-rw-r--r--   0 runner    (1001) docker     (116)    29632 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/internal/enums.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3443 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/internal/enums.pyi
+-rw-r--r--   0 runner    (1001) docker     (116)     6267 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/internal/net.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3847 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/internal/reflect.py
+-rw-r--r--   0 runner    (1001) docker     (116)    20215 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/internal/routes.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4673 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/internal/spel.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7594 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/internal/time.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13362 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/internal/ux.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11540 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/invites.py
+-rw-r--r--   0 runner    (1001) docker     (116)    37049 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/iterators.py
+-rw-r--r--   0 runner    (1001) docker     (116)    44984 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/messages.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6527 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10038 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/presences.py
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/py.typed
+-rw-r--r--   0 runner    (1001) docker     (116)     3613 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7504 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/snowflakes.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7233 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/templates.py
+-rw-r--r--   0 runner    (1001) docker     (116)    20706 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/traits.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4709 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/undefined.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1743 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/undefined.pyi
+-rw-r--r--   0 runner    (1001) docker     (116)     1644 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/urls.py
+-rw-r--r--   0 runner    (1001) docker     (116)    25173 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/users.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4741 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/voices.py
+-rw-r--r--   0 runner    (1001) docker     (116)    28515 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/hikari/webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-16 10:03:50.953309 hikari-2.0.0.dev99/hikari.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)    12371 2021-01-16 10:03:50.000000 hikari-2.0.0.dev99/hikari.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     2299 2021-01-16 10:03:50.000000 hikari-2.0.0.dev99/hikari.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-16 10:03:50.000000 hikari-2.0.0.dev99/hikari.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       44 2021-01-16 10:03:50.000000 hikari-2.0.0.dev99/hikari.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-16 10:03:50.000000 hikari-2.0.0.dev99/hikari.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (116)      134 2021-01-16 10:03:50.000000 hikari-2.0.0.dev99/hikari.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        7 2021-01-16 10:03:50.000000 hikari-2.0.0.dev99/hikari.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)     1296 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (116)       62 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2021-01-16 10:03:50.961310 hikari-2.0.0.dev99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     3927 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/setup.py
+-rw-r--r--   0 runner    (1001) docker     (116)       60 2021-01-16 10:03:14.000000 hikari-2.0.0.dev99/speedup-requirements.txt
```

### Comparing `hikari-2.0.0.dev98/LICENSE` & `hikari-2.0.0.dev99/LICENSE`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/PKG-INFO` & `hikari-2.0.0.dev99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hikari
-Version: 2.0.0.dev98
+Version: 2.0.0.dev99
 Summary: A sane Discord API for Python 3 built on asyncio and good intentions
 Home-page: https://github.com/hikari-py/hikari
 Author: Nekokatt
 Maintainer: davfsa
 Maintainer-email: davfsa@gmail.com
 License: MIT
 Project-URL: Documentation, https://hikari-py.github.io/hikari/documentation
```

### Comparing `hikari-2.0.0.dev98/README.md` & `hikari-2.0.0.dev99/README.md`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/__init__.py` & `hikari-2.0.0.dev99/hikari/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/__init__.pyi` & `hikari-2.0.0.dev99/hikari/__init__.pyi`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/__main__.py` & `hikari-2.0.0.dev99/hikari/__main__.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/_about.py` & `hikari-2.0.0.dev99/hikari/_about.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,9 +32,9 @@
 __coverage__ = "https://codeclimate.com/github/hikari-py/hikari"
 __discord_invite__ = "https://discord.gg/Jx4cNGG"
 __docs__ = "https://hikari-py.github.io/hikari/documentation"
 __email__ = "davfsa@gmail.com"
 __issue_tracker__ = "https://github.com/hikari-py/hikari/issues"
 __license__ = "MIT"
 __url__ = "https://github.com/hikari-py/hikari"
-__version__ = "2.0.0.dev98"
-__git_sha1__ = "23a57e97ad649b1e1f6023c82addca160ea5dda6"
+__version__ = "2.0.0.dev99"
+__git_sha1__ = "f1337fe12729d335b92fd2bcf154f896a9ff6577"
```

### Comparing `hikari-2.0.0.dev98/hikari/api/__init__.py` & `hikari-2.0.0.dev99/hikari/api/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/api/cache.py` & `hikari-2.0.0.dev99/hikari/api/cache.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/api/entity_factory.py` & `hikari-2.0.0.dev99/hikari/api/entity_factory.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/api/event_dispatcher.py` & `hikari-2.0.0.dev99/hikari/api/event_dispatcher.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/api/event_factory.py` & `hikari-2.0.0.dev99/hikari/api/event_factory.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/api/rest.py` & `hikari-2.0.0.dev99/hikari/api/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -776,17 +776,17 @@
 
         Returns
         -------
         hikari.iterators.LazyIterator[hikari.messages.Message]
             An iterator to fetch the messages.
 
         !!! note
-           This call is not a coroutine function, it returns a special type of
-           lazy iterator that will perform API calls as you iterate across it.
-           See `hikari.iterators` for the full API for this iterator type.
+            This call is not a coroutine function, it returns a special type of
+            lazy iterator that will perform API calls as you iterate across it.
+            See `hikari.iterators` for the full API for this iterator type.
 
         Raises
         ------
         builtins.TypeError
             If you specify more than one of `before`, `after`, `about`.
         hikari.errors.UnauthorizedError
             If you are unauthorized to make the request (invalid/missing token).
@@ -1562,17 +1562,17 @@
 
         Returns
         -------
         hikari.iterators.LazyIterator[hikari.users.User]
             An iterator to fetch the users.
 
         !!! note
-           This call is not a coroutine function, it returns a special type of
-           lazy iterator that will perform API calls as you iterate across it.
-           See `hikari.iterators` for the full API for this iterator type.
+            This call is not a coroutine function, it returns a special type of
+            lazy iterator that will perform API calls as you iterate across it.
+            See `hikari.iterators` for the full API for this iterator type.
 
         Raises
         ------
         hikari.errors.BadRequestError
             If an invalid unicode emoji is given, or if the given custom emoji
             does not exist.
         hikari.errors.UnauthorizedError
@@ -2460,17 +2460,17 @@
 
         Returns
         -------
         hikari.iterators.LazyIterator[hikari.applications.OwnGuild]
             The token's associated guilds.
 
         !!! note
-           This call is not a coroutine function, it returns a special type of
-           lazy iterator that will perform API calls as you iterate across it.
-           See `hikari.iterators` for the full API for this iterator type.
+            This call is not a coroutine function, it returns a special type of
+            lazy iterator that will perform API calls as you iterate across it.
+            See `hikari.iterators` for the full API for this iterator type.
 
         Raises
         ------
         hikari.errors.BadRequestError
             If any of the fields that are passed have an invalid value.
         hikari.errors.UnauthorizedError
             If you are unauthorized to make the request (invalid/missing token).
@@ -2770,17 +2770,17 @@
 
         Returns
         -------
         hikari.iterators.LazyIterator[hikari.audit_logs.AuditLog]
             The guild's audit log.
 
         !!! note
-           This call is not a coroutine function, it returns a special type of
-           lazy iterator that will perform API calls as you iterate across it.
-           See `hikari.iterators` for the full API for this iterator type.
+            This call is not a coroutine function, it returns a special type of
+            lazy iterator that will perform API calls as you iterate across it.
+            See `hikari.iterators` for the full API for this iterator type.
 
         Raises
         ------
         hikari.errors.BadRequestError
             If any of the fields that are passed have an invalid value.
         hikari.errors.ForbiddenError
             If you are missing the `VIEW_AUDIT_LOG` permission.
@@ -3759,17 +3759,17 @@
 
         Returns
         -------
         hikari.iterators.LazyIterator[hikari.guilds.Member]
             An iterator to fetch the members.
 
         !!! note
-           This call is not a coroutine function, it returns a special type of
-           lazy iterator that will perform API calls as you iterate across it.
-           See `hikari.iterators` for the full API for this iterator type.
+            This call is not a coroutine function, it returns a special type of
+            lazy iterator that will perform API calls as you iterate across it.
+            See `hikari.iterators` for the full API for this iterator type.
 
         Raises
         ------
         hikari.errors.UnauthorizedError
             If you are unauthorized to make the request (invalid/missing token).
         hikari.errors.NotFoundError
             If the guild is not found.
```

### Comparing `hikari-2.0.0.dev98/hikari/api/shard.py` & `hikari-2.0.0.dev99/hikari/api/shard.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/api/special_endpoints.py` & `hikari-2.0.0.dev99/hikari/api/special_endpoints.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/api/voice.py` & `hikari-2.0.0.dev99/hikari/api/voice.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/applications.py` & `hikari-2.0.0.dev99/hikari/applications.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/audit_logs.py` & `hikari-2.0.0.dev99/hikari/audit_logs.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/banner.txt` & `hikari-2.0.0.dev99/hikari/banner.txt`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/channels.py` & `hikari-2.0.0.dev99/hikari/channels.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/cli.py` & `hikari-2.0.0.dev99/hikari/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,16 +33,16 @@
 
 
 def main() -> None:
     """Print package info and exit."""
     sourcefile = inspect.getsourcefile(_about)
     assert isinstance(sourcefile, str)
     path: typing.Final[str] = os.path.abspath(os.path.dirname(sourcefile))
-    sha1: typing.Final[str] = _about.__git_sha1__
+    sha1: typing.Final[str] = _about.__git_sha1__[:8]
     version: typing.Final[str] = _about.__version__
     py_impl: typing.Final[str] = platform.python_implementation()
     py_ver: typing.Final[str] = platform.python_version()
     py_compiler: typing.Final[str] = platform.python_compiler()
-    sys.stderr.write(f"hikari v{version} {sha1}\n")
+    sys.stderr.write(f"hikari ({version}) [{sha1}]\n")
     sys.stderr.write(f"located at {path}\n")
     sys.stderr.write(f"{py_impl} {py_ver} {py_compiler}\n")
     sys.stderr.write(" ".join(frag.strip() for frag in platform.uname() if frag and frag.strip()) + "\n")
```

### Comparing `hikari-2.0.0.dev98/hikari/colors.py` & `hikari-2.0.0.dev99/hikari/colors.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/colours.py` & `hikari-2.0.0.dev99/hikari/colours.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/config.py` & `hikari-2.0.0.dev99/hikari/config.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/embeds.py` & `hikari-2.0.0.dev99/hikari/embeds.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/emojis.py` & `hikari-2.0.0.dev99/hikari/emojis.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/errors.py` & `hikari-2.0.0.dev99/hikari/errors.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/event_stream.py` & `hikari-2.0.0.dev99/hikari/event_stream.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/events/__init__.py` & `hikari-2.0.0.dev99/hikari/events/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/events/__init__.pyi` & `hikari-2.0.0.dev99/hikari/events/__init__.pyi`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/events/base_events.py` & `hikari-2.0.0.dev99/hikari/events/base_events.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/events/channel_events.py` & `hikari-2.0.0.dev99/hikari/events/channel_events.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/events/guild_events.py` & `hikari-2.0.0.dev99/hikari/events/guild_events.py`

 * *Files 0% similar despite different names*

```diff
@@ -210,26 +210,26 @@
 
     Returns
     -------
     typing.Mapping[hikari.snowflakes.Snowflake, hikari.voices.VoiceState]
         The voice states active in the guild.
     """
 
-    guild_chunk_nonce: typing.Optional[str] = attr.ib(repr=False, default=None)
-    """Nonce used to request the guild chunks.
+    chunk_nonce: typing.Optional[str] = attr.ib(repr=False, default=None)
+    """Nonce used to request the member chunks for this guild.
 
     This will be `builtins.None` if no chunks were requested.
 
     !!! note
         This is a syntetic field.
 
     Returns
     -------
     typing.Optional[builtins.str]
-        The nonce used to request the guild chunks.
+        The nonce used to request the member chunks.
     """
 
     @property
     def guild_id(self) -> snowflakes.Snowflake:
         # <<inherited docstring from GuildEvent>>.
         return self.guild.id
```

### Comparing `hikari-2.0.0.dev98/hikari/events/lifetime_events.py` & `hikari-2.0.0.dev99/hikari/events/lifetime_events.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/events/member_events.py` & `hikari-2.0.0.dev99/hikari/events/member_events.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/events/message_events.py` & `hikari-2.0.0.dev99/hikari/events/message_events.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/events/reaction_events.py` & `hikari-2.0.0.dev99/hikari/events/reaction_events.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/events/role_events.py` & `hikari-2.0.0.dev99/hikari/events/role_events.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/events/shard_events.py` & `hikari-2.0.0.dev99/hikari/events/shard_events.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/events/typing_events.py` & `hikari-2.0.0.dev99/hikari/events/typing_events.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/events/user_events.py` & `hikari-2.0.0.dev99/hikari/events/user_events.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/events/voice_events.py` & `hikari-2.0.0.dev99/hikari/events/voice_events.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/files.py` & `hikari-2.0.0.dev99/hikari/files.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/guilds.py` & `hikari-2.0.0.dev99/hikari/guilds.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/impl/__init__.py` & `hikari-2.0.0.dev99/hikari/impl/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/impl/bot.py` & `hikari-2.0.0.dev99/hikari/impl/bot.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/impl/buckets.py` & `hikari-2.0.0.dev99/hikari/impl/buckets.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/impl/cache.py` & `hikari-2.0.0.dev99/hikari/impl/cache.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/impl/entity_factory.py` & `hikari-2.0.0.dev99/hikari/impl/entity_factory.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/impl/event_factory.py` & `hikari-2.0.0.dev99/hikari/impl/event_factory.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/impl/event_manager.py` & `hikari-2.0.0.dev99/hikari/impl/event_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,15 +145,15 @@
 
         # When intents are enabled discord will only send other member objects on the guild create
         # payload if presence intents are also declared, so if this isn't the case then we also want
         # to chunk small guilds.
         if members_declared and (event.guild.is_large or not presences_declared):
             # We create a task here instead of awaiting the result to avoid any rate-limits from delaying dispatch.
             nonce = f"{shard.id}.{time.uuid()}"
-            event.guild_chunk_nonce = nonce
+            event.chunk_nonce = nonce
             coroutine = shard.request_guild_members(
                 event.guild, include_presences=bool(presences_declared), nonce=nonce
             )
             asyncio.create_task(coroutine, name=f"{shard.id}:{event.guild.id} guild create members request")
 
         await self.dispatch(event)
```

### Comparing `hikari-2.0.0.dev98/hikari/impl/event_manager_base.py` & `hikari-2.0.0.dev99/hikari/impl/event_manager_base.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/impl/rate_limits.py` & `hikari-2.0.0.dev99/hikari/impl/rate_limits.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/impl/rest.py` & `hikari-2.0.0.dev99/hikari/impl/rest.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/impl/shard.py` & `hikari-2.0.0.dev99/hikari/impl/shard.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/impl/special_endpoints.py` & `hikari-2.0.0.dev99/hikari/impl/special_endpoints.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/impl/voice.py` & `hikari-2.0.0.dev99/hikari/impl/voice.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/intents.py` & `hikari-2.0.0.dev99/hikari/intents.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/internal/__init__.py` & `hikari-2.0.0.dev99/hikari/internal/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/internal/aio.py` & `hikari-2.0.0.dev99/hikari/internal/aio.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/internal/attr_extensions.py` & `hikari-2.0.0.dev99/hikari/internal/attr_extensions.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/internal/cache.py` & `hikari-2.0.0.dev99/hikari/internal/cache.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/internal/collections.py` & `hikari-2.0.0.dev99/hikari/internal/collections.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/internal/data_binding.py` & `hikari-2.0.0.dev99/hikari/internal/data_binding.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/internal/enums.py` & `hikari-2.0.0.dev99/hikari/internal/enums.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/internal/enums.pyi` & `hikari-2.0.0.dev99/hikari/internal/enums.pyi`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/internal/net.py` & `hikari-2.0.0.dev99/hikari/internal/net.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/internal/reflect.py` & `hikari-2.0.0.dev99/hikari/internal/reflect.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/internal/routes.py` & `hikari-2.0.0.dev99/hikari/internal/routes.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/internal/spel.py` & `hikari-2.0.0.dev99/hikari/internal/spel.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/internal/time.py` & `hikari-2.0.0.dev99/hikari/internal/time.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/internal/ux.py` & `hikari-2.0.0.dev99/hikari/internal/ux.py`

 * *Files 2% similar despite different names*

```diff
@@ -271,14 +271,22 @@
         self.version = (int(major), int(minor), int(patch) if patch else 0)
 
         if prerelease:
             self.prerelease = (prerelease, int(prerelease_num))
         else:
             self.prerelease = None
 
+    def __str__(self) -> str:
+        vstring = ".".join(map(str, self.version))
+
+        if self.prerelease:
+            vstring = vstring + self.prerelease[0] + str(self.prerelease[1])
+
+        return vstring
+
 
 async def check_for_updates(http_settings: config.HTTPSettings, proxy_settings: config.ProxySettings) -> None:
     """Perform a check for newer versions of the library, logging any found."""
     if about.__git_sha1__.casefold() == "head":
         # We are not in a PyPI release, return
         return
```

### Comparing `hikari-2.0.0.dev98/hikari/invites.py` & `hikari-2.0.0.dev99/hikari/invites.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/iterators.py` & `hikari-2.0.0.dev99/hikari/iterators.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/messages.py` & `hikari-2.0.0.dev99/hikari/messages.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/permissions.py` & `hikari-2.0.0.dev99/hikari/permissions.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/presences.py` & `hikari-2.0.0.dev99/hikari/presences.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/sessions.py` & `hikari-2.0.0.dev99/hikari/sessions.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/snowflakes.py` & `hikari-2.0.0.dev99/hikari/snowflakes.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/templates.py` & `hikari-2.0.0.dev99/hikari/templates.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/traits.py` & `hikari-2.0.0.dev99/hikari/traits.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/undefined.py` & `hikari-2.0.0.dev99/hikari/undefined.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/undefined.pyi` & `hikari-2.0.0.dev99/hikari/undefined.pyi`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/urls.py` & `hikari-2.0.0.dev99/hikari/urls.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/users.py` & `hikari-2.0.0.dev99/hikari/users.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/voices.py` & `hikari-2.0.0.dev99/hikari/voices.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari/webhooks.py` & `hikari-2.0.0.dev99/hikari/webhooks.py`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/hikari.egg-info/PKG-INFO` & `hikari-2.0.0.dev99/hikari.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hikari
-Version: 2.0.0.dev98
+Version: 2.0.0.dev99
 Summary: A sane Discord API for Python 3 built on asyncio and good intentions
 Home-page: https://github.com/hikari-py/hikari
 Author: Nekokatt
 Maintainer: davfsa
 Maintainer-email: davfsa@gmail.com
 License: MIT
 Project-URL: Documentation, https://hikari-py.github.io/hikari/documentation
```

### Comparing `hikari-2.0.0.dev98/hikari.egg-info/SOURCES.txt` & `hikari-2.0.0.dev99/hikari.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/pyproject.toml` & `hikari-2.0.0.dev99/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hikari-2.0.0.dev98/setup.py` & `hikari-2.0.0.dev99/setup.py`

 * *Files identical despite different names*

