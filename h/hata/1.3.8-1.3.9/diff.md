# Comparing `tmp/hata-1.3.8.tar.gz` & `tmp/hata-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hata-1.3.8.tar", last modified: Tue Sep 20 19:23:34 2022, max compression
+gzip compressed data, was "hata-1.3.9.tar", last modified: Mon Oct  3 12:28:55 2022, max compression
```

## Comparing `hata-1.3.8.tar` & `hata-1.3.9.tar`

### file list

```diff
@@ -1,609 +1,610 @@
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.160796 hata-1.3.8/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     8427 2022-09-20 19:23:34.160796 hata-1.3.8/PKG-INFO
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     5410 2022-08-13 12:35:16.000000 hata-1.3.8/README.md
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.052796 hata-1.3.8/hata/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3160 2022-09-20 18:20:16.000000 hata-1.3.8/hata/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1011 2022-07-22 10:09:55.000000 hata-1.3.8/hata/__main__.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.056796 hata-1.3.8/hata/backend/
--rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)      574 2022-03-30 17:00:03.000000 hata-1.3.8/hata/backend/__init__.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.056796 hata-1.3.8/hata/discord/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1624 2022-06-24 19:36:38.000000 hata-1.3.8/hata/discord/__init__.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.056796 hata-1.3.8/hata/discord/activity/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      686 2022-09-05 21:05:42.000000 hata-1.3.8/hata/discord/activity/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    23332 2022-09-13 10:43:13.000000 hata-1.3.8/hata/discord/activity/activity.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      408 2022-09-08 14:15:22.000000 hata-1.3.8/hata/discord/activity/constants.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.056796 hata-1.3.8/hata/discord/activity/fields/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      234 2022-09-06 15:02:25.000000 hata-1.3.8/hata/discord/activity/fields/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     9239 2022-09-04 15:55:06.000000 hata-1.3.8/hata/discord/activity/fields/assets.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1427 2022-09-04 13:32:06.000000 hata-1.3.8/hata/discord/activity/fields/base.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     6018 2022-09-04 15:52:11.000000 hata-1.3.8/hata/discord/activity/fields/party.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     6411 2022-09-04 19:14:48.000000 hata-1.3.8/hata/discord/activity/fields/secrets.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4963 2022-09-06 15:11:39.000000 hata-1.3.8/hata/discord/activity/fields/timestamps.py
--rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)     1756 2021-10-08 11:30:50.000000 hata-1.3.8/hata/discord/activity/flags.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.060796 hata-1.3.8/hata/discord/activity/metadata/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      136 2022-09-04 17:08:56.000000 hata-1.3.8/hata/discord/activity/metadata/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     9160 2022-09-13 10:27:02.000000 hata-1.3.8/hata/discord/activity/metadata/base.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     6045 2022-09-13 10:33:03.000000 hata-1.3.8/hata/discord/activity/metadata/custom.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    19600 2022-09-13 10:33:03.000000 hata-1.3.8/hata/discord/activity/metadata/rich.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4621 2022-09-10 17:20:10.000000 hata-1.3.8/hata/discord/activity/preinstanced.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    41730 2022-02-13 12:17:28.000000 hata-1.3.8/hata/discord/allowed_mentions.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    12248 2022-07-30 20:58:26.000000 hata-1.3.8/hata/discord/ansi_format.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.060796 hata-1.3.8/hata/discord/application/
--rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)      354 2022-02-15 15:10:02.000000 hata-1.3.8/hata/discord/application/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    23321 2022-03-30 17:00:03.000000 hata-1.3.8/hata/discord/application/application.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4702 2022-02-17 18:12:57.000000 hata-1.3.8/hata/discord/application/embedded_activity_configuration.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3719 2022-07-23 08:26:02.000000 hata-1.3.8/hata/discord/application/flags.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     9284 2022-01-22 18:27:00.000000 hata-1.3.8/hata/discord/application/miscellaneous.py
--rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)    22953 2022-07-29 14:09:19.000000 hata-1.3.8/hata/discord/application/preinstanced.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     5237 2022-02-22 17:34:04.000000 hata-1.3.8/hata/discord/application/team.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.060796 hata-1.3.8/hata/discord/auto_moderation/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      384 2022-09-17 11:24:36.000000 hata-1.3.8/hata/discord/auto_moderation/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     9884 2022-09-17 11:24:36.000000 hata-1.3.8/hata/discord/auto_moderation/action.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.060796 hata-1.3.8/hata/discord/auto_moderation/action_metadata/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      157 2022-09-17 11:24:36.000000 hata-1.3.8/hata/discord/auto_moderation/action_metadata/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3296 2022-09-17 11:24:36.000000 hata-1.3.8/hata/discord/auto_moderation/action_metadata/alert_message.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1705 2022-09-17 11:24:36.000000 hata-1.3.8/hata/discord/auto_moderation/action_metadata/base.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3128 2022-09-17 11:24:36.000000 hata-1.3.8/hata/discord/auto_moderation/action_metadata/timeout.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      106 2022-07-23 09:47:31.000000 hata-1.3.8/hata/discord/auto_moderation/constants.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     8719 2022-09-10 12:47:35.000000 hata-1.3.8/hata/discord/auto_moderation/event_types.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    14662 2022-09-17 11:24:36.000000 hata-1.3.8/hata/discord/auto_moderation/preinstanced.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    49626 2022-09-17 11:24:36.000000 hata-1.3.8/hata/discord/auto_moderation/rule.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.064796 hata-1.3.8/hata/discord/auto_moderation/trigger_metadata/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      254 2022-09-17 11:24:36.000000 hata-1.3.8/hata/discord/auto_moderation/trigger_metadata/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1741 2022-09-17 11:24:36.000000 hata-1.3.8/hata/discord/auto_moderation/trigger_metadata/base.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     7744 2022-09-17 11:24:36.000000 hata-1.3.8/hata/discord/auto_moderation/trigger_metadata/keyword.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    10806 2022-09-17 11:24:36.000000 hata-1.3.8/hata/discord/auto_moderation/trigger_metadata/keyword_preset.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3489 2022-09-17 11:24:36.000000 hata-1.3.8/hata/discord/auto_moderation/trigger_metadata/mention_spam.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      950 2022-09-17 11:24:36.000000 hata-1.3.8/hata/discord/auto_moderation/trigger_metadata/utils.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.064796 hata-1.3.8/hata/discord/bases/
--rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)      342 2022-09-12 06:18:05.000000 hata-1.3.8/hata/discord/bases/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     8061 2022-09-12 06:18:05.000000 hata-1.3.8/hata/discord/bases/entity.py
--rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)      920 2021-12-19 12:03:10.000000 hata-1.3.8/hata/discord/bases/event_types.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    16895 2022-03-06 13:34:11.000000 hata-1.3.8/hata/discord/bases/flags.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    16568 2022-09-17 11:24:36.000000 hata-1.3.8/hata/discord/bases/icon.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2886 2022-09-12 06:18:05.000000 hata-1.3.8/hata/discord/bases/place_holder.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     8363 2022-08-27 06:51:27.000000 hata-1.3.8/hata/discord/bases/preinstanced.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    12351 2022-01-03 06:21:48.000000 hata-1.3.8/hata/discord/bases/utils.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.064796 hata-1.3.8/hata/discord/channel/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      575 2022-09-11 16:08:40.000000 hata-1.3.8/hata/discord/channel/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    77410 2022-09-20 16:00:22.000000 hata-1.3.8/hata/discord/channel/channel.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.064796 hata-1.3.8/hata/discord/channel/channel_type/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      111 2022-09-10 12:01:02.000000 hata-1.3.8/hata/discord/channel/channel_type/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3511 2022-09-10 11:44:14.000000 hata-1.3.8/hata/discord/channel/channel_type/flags.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    13813 2022-09-10 12:25:11.000000 hata-1.3.8/hata/discord/channel/channel_type/preinstanced.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      450 2022-09-18 11:32:28.000000 hata-1.3.8/hata/discord/channel/constants.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    13279 2022-09-10 13:45:45.000000 hata-1.3.8/hata/discord/channel/deprecation.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.068796 hata-1.3.8/hata/discord/channel/fields/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1365 2022-09-17 11:24:36.000000 hata-1.3.8/hata/discord/channel/fields/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3289 2022-09-17 11:24:36.000000 hata-1.3.8/hata/discord/channel/fields/applied_tag_ids.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1598 2022-09-14 19:48:39.000000 hata-1.3.8/hata/discord/channel/fields/archived.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2343 2022-09-14 15:55:58.000000 hata-1.3.8/hata/discord/channel/fields/archived_at.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2325 2022-09-14 11:52:07.000000 hata-1.3.8/hata/discord/channel/fields/auto_archive_after.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2703 2022-09-17 15:29:16.000000 hata-1.3.8/hata/discord/channel/fields/available_tags.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1417 2022-09-17 11:24:36.000000 hata-1.3.8/hata/discord/channel/fields/bitrate.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2307 2022-09-14 13:04:36.000000 hata-1.3.8/hata/discord/channel/fields/created_at.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2327 2022-09-14 11:52:06.000000 hata-1.3.8/hata/discord/channel/fields/default_thread_auto_archive_after.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2342 2022-09-13 12:14:26.000000 hata-1.3.8/hata/discord/channel/fields/default_thread_reaction.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2008 2022-09-13 12:24:48.000000 hata-1.3.8/hata/discord/channel/fields/default_thread_slowmode.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1351 2022-09-13 12:41:43.000000 hata-1.3.8/hata/discord/channel/fields/flags.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1700 2022-09-14 19:59:35.000000 hata-1.3.8/hata/discord/channel/fields/invitable.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1501 2022-09-13 13:21:46.000000 hata-1.3.8/hata/discord/channel/fields/name.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1244 2022-09-14 19:48:51.000000 hata-1.3.8/hata/discord/channel/fields/nsfw.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1532 2022-09-14 19:48:26.000000 hata-1.3.8/hata/discord/channel/fields/open_.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2145 2022-09-14 15:25:40.000000 hata-1.3.8/hata/discord/channel/fields/owner_id.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2083 2022-09-14 15:25:20.000000 hata-1.3.8/hata/discord/channel/fields/parent_id.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3075 2022-09-14 10:32:58.000000 hata-1.3.8/hata/discord/channel/fields/permission_overwrites.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1494 2022-09-13 13:28:19.000000 hata-1.3.8/hata/discord/channel/fields/position.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1793 2022-09-17 11:24:36.000000 hata-1.3.8/hata/discord/channel/fields/region.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1691 2022-09-14 10:48:21.000000 hata-1.3.8/hata/discord/channel/fields/slowmode.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1610 2022-09-13 13:21:48.000000 hata-1.3.8/hata/discord/channel/fields/topic.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1568 2022-09-17 11:24:36.000000 hata-1.3.8/hata/discord/channel/fields/user_limit.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2402 2022-09-17 11:24:36.000000 hata-1.3.8/hata/discord/channel/fields/users.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2042 2022-09-14 21:24:46.000000 hata-1.3.8/hata/discord/channel/fields/video_quality_mode.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1232 2022-09-08 16:59:33.000000 hata-1.3.8/hata/discord/channel/flags.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    15196 2022-09-13 10:21:21.000000 hata-1.3.8/hata/discord/channel/forum_tag.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     6041 2022-03-29 16:37:14.000000 hata-1.3.8/hata/discord/channel/message_history.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     6721 2022-03-27 08:13:18.000000 hata-1.3.8/hata/discord/channel/message_iterator.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.072796 hata-1.3.8/hata/discord/channel/metadata/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1188 2022-09-10 16:36:03.000000 hata-1.3.8/hata/discord/channel/metadata/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    28373 2022-09-18 11:32:58.000000 hata-1.3.8/hata/discord/channel/metadata/base.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3397 2022-09-12 18:46:22.000000 hata-1.3.8/hata/discord/channel/metadata/guild_announcements.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    10718 2022-09-20 15:47:34.000000 hata-1.3.8/hata/discord/channel/metadata/guild_base.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1065 2022-09-12 18:46:13.000000 hata-1.3.8/hata/discord/channel/metadata/guild_category.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2158 2022-09-12 18:46:03.000000 hata-1.3.8/hata/discord/channel/metadata/guild_directory.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    11824 2022-09-18 10:23:05.000000 hata-1.3.8/hata/discord/channel/metadata/guild_forum.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    12197 2022-09-18 10:41:57.000000 hata-1.3.8/hata/discord/channel/metadata/guild_main_base.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4991 2022-09-18 10:09:48.000000 hata-1.3.8/hata/discord/channel/metadata/guild_stage.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4475 2022-09-18 10:11:00.000000 hata-1.3.8/hata/discord/channel/metadata/guild_store.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3080 2022-09-11 12:47:35.000000 hata-1.3.8/hata/discord/channel/metadata/guild_text.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     8763 2022-09-18 10:13:10.000000 hata-1.3.8/hata/discord/channel/metadata/guild_text_base.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1676 2022-09-12 18:49:28.000000 hata-1.3.8/hata/discord/channel/metadata/guild_thread_announcements.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    12444 2022-09-18 10:16:39.000000 hata-1.3.8/hata/discord/channel/metadata/guild_thread_base.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4293 2022-09-18 10:17:27.000000 hata-1.3.8/hata/discord/channel/metadata/guild_thread_private.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     5116 2022-09-17 11:24:36.000000 hata-1.3.8/hata/discord/channel/metadata/guild_thread_public.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     6224 2022-09-18 10:42:48.000000 hata-1.3.8/hata/discord/channel/metadata/guild_voice.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     5429 2022-09-18 10:20:20.000000 hata-1.3.8/hata/discord/channel/metadata/guild_voice_base.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2140 2022-09-20 15:49:31.000000 hata-1.3.8/hata/discord/channel/metadata/private.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2827 2022-09-20 16:03:03.000000 hata-1.3.8/hata/discord/channel/metadata/private_base.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     7222 2022-09-18 10:24:28.000000 hata-1.3.8/hata/discord/channel/metadata/private_group.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1938 2022-09-10 09:29:57.000000 hata-1.3.8/hata/discord/channel/preinstanced.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    25631 2022-09-20 19:07:06.000000 hata-1.3.8/hata/discord/channel/utils.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.076796 hata-1.3.8/hata/discord/client/
--rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)      341 2022-06-24 10:45:11.000000 hata-1.3.8/hata/discord/client/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    71537 2022-09-05 06:46:18.000000 hata-1.3.8/hata/discord/client/client.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.080796 hata-1.3.8/hata/discord/client/compounds/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3547 2022-07-23 10:23:30.000000 hata-1.3.8/hata/discord/client/compounds/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    22326 2022-08-27 13:40:29.000000 hata-1.3.8/hata/discord/client/compounds/achievement.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    33411 2022-08-27 17:24:17.000000 hata-1.3.8/hata/discord/client/compounds/application_command.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     7337 2022-07-09 07:24:07.000000 hata-1.3.8/hata/discord/client/compounds/auto_moderation.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    40521 2022-09-18 10:50:22.000000 hata-1.3.8/hata/discord/client/compounds/channel.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    20278 2022-08-13 12:52:25.000000 hata-1.3.8/hata/discord/client/compounds/client.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    14125 2022-09-13 10:35:29.000000 hata-1.3.8/hata/discord/client/compounds/client_gayteway.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    13119 2022-06-24 15:26:58.000000 hata-1.3.8/hata/discord/client/compounds/discovery.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    13922 2022-06-24 15:25:27.000000 hata-1.3.8/hata/discord/client/compounds/emoji.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    76341 2022-09-10 16:28:10.000000 hata-1.3.8/hata/discord/client/compounds/guild.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    10642 2022-07-23 11:06:48.000000 hata-1.3.8/hata/discord/client/compounds/guild_ban.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    10418 2022-06-24 10:55:13.000000 hata-1.3.8/hata/discord/client/compounds/integration.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    44383 2022-08-13 20:06:27.000000 hata-1.3.8/hata/discord/client/compounds/interaction.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    24933 2022-09-10 17:04:19.000000 hata-1.3.8/hata/discord/client/compounds/invite.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     7853 2022-06-24 10:53:08.000000 hata-1.3.8/hata/discord/client/compounds/locked.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    81858 2022-09-10 16:04:00.000000 hata-1.3.8/hata/discord/client/compounds/message.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     5476 2022-09-10 16:04:00.000000 hata-1.3.8/hata/discord/client/compounds/miscellaneous.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    18751 2022-08-28 11:05:03.000000 hata-1.3.8/hata/discord/client/compounds/oauth2.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    13727 2022-08-13 20:14:14.000000 hata-1.3.8/hata/discord/client/compounds/reaction.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    28535 2022-06-24 15:26:58.000000 hata-1.3.8/hata/discord/client/compounds/role.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    22947 2022-06-24 15:25:27.000000 hata-1.3.8/hata/discord/client/compounds/scheduled_event.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     7996 2022-06-24 10:52:15.000000 hata-1.3.8/hata/discord/client/compounds/stage.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    19362 2022-06-24 10:52:15.000000 hata-1.3.8/hata/discord/client/compounds/sticker.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    30693 2022-09-18 10:50:22.000000 hata-1.3.8/hata/discord/client/compounds/thread.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    22243 2022-08-21 19:02:35.000000 hata-1.3.8/hata/discord/client/compounds/user.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    39005 2022-09-10 16:28:10.000000 hata-1.3.8/hata/discord/client/compounds/webhook.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    38431 2022-09-18 10:50:22.000000 hata-1.3.8/hata/discord/client/functionality_helpers.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    14350 2022-03-29 18:05:43.000000 hata-1.3.8/hata/discord/client/ready_state.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    59497 2022-08-13 20:04:51.000000 hata-1.3.8/hata/discord/client/request_helpers.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    16687 2022-07-25 20:28:21.000000 hata-1.3.8/hata/discord/client/utils.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    18275 2022-06-12 11:16:32.000000 hata-1.3.8/hata/discord/color.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     5584 2022-09-09 16:10:40.000000 hata-1.3.8/hata/discord/core.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.080796 hata-1.3.8/hata/discord/embed/
--rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)      158 2021-10-08 11:30:50.000000 hata-1.3.8/hata/discord/embed/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    36833 2022-06-21 09:40:41.000000 hata-1.3.8/hata/discord/embed/embed.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    44944 2022-05-02 06:13:46.000000 hata-1.3.8/hata/discord/embed/embed_base.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    17615 2022-01-29 18:36:01.000000 hata-1.3.8/hata/discord/embed/embed_core.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.084796 hata-1.3.8/hata/discord/emoji/
--rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)      364 2022-08-18 15:16:50.000000 hata-1.3.8/hata/discord/emoji/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    21835 2022-09-04 09:28:51.000000 hata-1.3.8/hata/discord/emoji/emoji.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     5836 2022-08-18 15:08:52.000000 hata-1.3.8/hata/discord/emoji/emoji_all_pattern.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     7479 2022-08-13 20:08:29.000000 hata-1.3.8/hata/discord/emoji/event_types.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    10256 2022-06-05 12:43:45.000000 hata-1.3.8/hata/discord/emoji/reaction.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3049 2022-09-20 17:27:47.000000 hata-1.3.8/hata/discord/emoji/unicode_type.py
--rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)   590776 2022-09-20 18:10:21.000000 hata-1.3.8/hata/discord/emoji/unicodes.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    11078 2022-09-18 12:26:32.000000 hata-1.3.8/hata/discord/emoji/utils.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.084796 hata-1.3.8/hata/discord/events/
--rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)      573 2021-10-12 09:16:26.000000 hata-1.3.8/hata/discord/events/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    23100 2022-08-13 12:58:20.000000 hata-1.3.8/hata/discord/events/core.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     6026 2022-07-30 12:32:57.000000 hata-1.3.8/hata/discord/events/default_event_handlers.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    78354 2022-09-17 11:24:36.000000 hata-1.3.8/hata/discord/events/event_handler_manager.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    14276 2022-01-29 18:36:01.000000 hata-1.3.8/hata/discord/events/event_handler_plugin.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    15180 2022-09-10 12:33:40.000000 hata-1.3.8/hata/discord/events/event_types.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     9429 2022-02-26 09:10:25.000000 hata-1.3.8/hata/discord/events/filters.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3982 2021-12-31 07:39:40.000000 hata-1.3.8/hata/discord/events/guild_sync.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    87153 2022-09-08 19:51:58.000000 hata-1.3.8/hata/discord/events/handling_helpers.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    23989 2022-06-23 14:56:18.000000 hata-1.3.8/hata/discord/events/intent.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)   133557 2022-09-18 10:50:22.000000 hata-1.3.8/hata/discord/events/parsers.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.088796 hata-1.3.8/hata/discord/exceptions/
--rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)      395 2021-10-08 11:30:50.000000 hata-1.3.8/hata/discord/exceptions/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    17616 2022-09-04 09:28:51.000000 hata-1.3.8/hata/discord/exceptions/discord_exception.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2517 2022-03-21 15:50:31.000000 hata-1.3.8/hata/discord/exceptions/discord_gateway_exception.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    52202 2022-09-08 16:51:32.000000 hata-1.3.8/hata/discord/exceptions/error_codes.py
--rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)      249 2021-10-08 11:30:50.000000 hata-1.3.8/hata/discord/exceptions/invalid_token.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    10786 2022-09-04 19:34:56.000000 hata-1.3.8/hata/discord/exceptions/payload_renderer.py
--rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)      172 2021-10-08 11:30:50.000000 hata-1.3.8/hata/discord/exceptions/voice_error_codes.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.088796 hata-1.3.8/hata/discord/gateway/
--rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)      245 2021-10-08 11:30:50.000000 hata-1.3.8/hata/discord/gateway/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    28356 2022-09-13 10:34:32.000000 hata-1.3.8/hata/discord/gateway/client_gateway.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    13765 2022-01-03 06:21:48.000000 hata-1.3.8/hata/discord/gateway/heartbeat.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4031 2022-01-01 14:48:03.000000 hata-1.3.8/hata/discord/gateway/rate_limit.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    14823 2022-02-07 13:26:01.000000 hata-1.3.8/hata/discord/gateway/voice_client_gateway.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.092796 hata-1.3.8/hata/discord/guild/
--rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)      639 2021-12-19 21:12:03.000000 hata-1.3.8/hata/discord/guild/__init__.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.092796 hata-1.3.8/hata/discord/guild/audit_logs/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      570 2022-01-23 20:15:39.000000 hata-1.3.8/hata/discord/guild/audit_logs/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     7984 2022-09-18 10:50:22.000000 hata-1.3.8/hata/discord/guild/audit_logs/audit_log.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    19718 2022-09-17 11:24:36.000000 hata-1.3.8/hata/discord/guild/audit_logs/audit_log_change.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     6987 2022-07-02 19:19:40.000000 hata-1.3.8/hata/discord/guild/audit_logs/audit_log_entry.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     8217 2022-06-24 19:04:11.000000 hata-1.3.8/hata/discord/guild/audit_logs/audit_log_iterator.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1225 2022-01-22 18:30:13.000000 hata-1.3.8/hata/discord/guild/audit_logs/audit_log_role.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.096796 hata-1.3.8/hata/discord/guild/audit_logs/change_converters/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      816 2022-06-24 19:34:04.000000 hata-1.3.8/hata/discord/guild/audit_logs/change_converters/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2075 2022-06-25 07:26:50.000000 hata-1.3.8/hata/discord/guild/audit_logs/change_converters/all_.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      253 2022-05-02 14:45:16.000000 hata-1.3.8/hata/discord/guild/audit_logs/change_converters/application_command.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2662 2022-09-17 11:24:36.000000 hata-1.3.8/hata/discord/guild/audit_logs/change_converters/auto_moderation_rule.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4505 2022-09-13 13:40:27.000000 hata-1.3.8/hata/discord/guild/audit_logs/change_converters/channel.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      924 2022-01-23 20:07:49.000000 hata-1.3.8/hata/discord/guild/audit_logs/change_converters/channel_permission_overwrite.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      204 2022-01-23 20:07:49.000000 hata-1.3.8/hata/discord/guild/audit_logs/change_converters/emoji.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3133 2022-03-30 04:08:08.000000 hata-1.3.8/hata/discord/guild/audit_logs/change_converters/guild.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      206 2022-01-23 20:07:49.000000 hata-1.3.8/hata/discord/guild/audit_logs/change_converters/integration.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      326 2022-01-23 20:07:49.000000 hata-1.3.8/hata/discord/guild/audit_logs/change_converters/invite.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1157 2022-01-23 20:07:49.000000 hata-1.3.8/hata/discord/guild/audit_logs/change_converters/role.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2250 2022-09-17 11:24:36.000000 hata-1.3.8/hata/discord/guild/audit_logs/change_converters/scheduled_event.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2908 2022-06-24 19:21:30.000000 hata-1.3.8/hata/discord/guild/audit_logs/change_converters/shared.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      229 2022-01-23 20:07:49.000000 hata-1.3.8/hata/discord/guild/audit_logs/change_converters/stage.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1150 2022-01-25 20:26:40.000000 hata-1.3.8/hata/discord/guild/audit_logs/change_converters/sticker.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      877 2022-01-23 20:07:49.000000 hata-1.3.8/hata/discord/guild/audit_logs/change_converters/user.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      473 2022-01-25 20:33:06.000000 hata-1.3.8/hata/discord/guild/audit_logs/change_converters/webhook.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1894 2022-07-23 11:10:05.000000 hata-1.3.8/hata/discord/guild/audit_logs/detail_converters.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    33486 2022-07-09 16:06:54.000000 hata-1.3.8/hata/discord/guild/audit_logs/preinstanced.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3343 2022-06-24 19:34:04.000000 hata-1.3.8/hata/discord/guild/audit_logs/target_converters.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    22501 2022-01-29 18:36:01.000000 hata-1.3.8/hata/discord/guild/discovery.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    13396 2022-09-10 12:30:03.000000 hata-1.3.8/hata/discord/guild/embedded_activity_state.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    10844 2022-02-22 18:03:52.000000 hata-1.3.8/hata/discord/guild/event_types.py
--rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)     2737 2022-05-28 10:03:13.000000 hata-1.3.8/hata/discord/guild/flags.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)   105329 2022-09-18 10:50:22.000000 hata-1.3.8/hata/discord/guild/guild.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    45027 2022-09-08 16:24:18.000000 hata-1.3.8/hata/discord/guild/preinstanced.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     5521 2022-09-04 09:28:51.000000 hata-1.3.8/hata/discord/guild/preview.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2389 2022-01-03 06:21:48.000000 hata-1.3.8/hata/discord/guild/utils.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     9941 2022-02-14 09:44:43.000000 hata-1.3.8/hata/discord/guild/verification_screen.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    10089 2022-09-10 16:28:10.000000 hata-1.3.8/hata/discord/guild/welcome_screen.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     8377 2022-09-18 10:50:24.000000 hata-1.3.8/hata/discord/guild/widget.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.096796 hata-1.3.8/hata/discord/http/
--rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)      409 2021-10-08 11:30:50.000000 hata-1.3.8/hata/discord/http/__init__.py
--rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)      490 2022-01-01 14:53:39.000000 hata-1.3.8/hata/discord/http/headers.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    82534 2022-08-12 13:01:28.000000 hata-1.3.8/hata/discord/http/http_client.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    37398 2022-03-13 10:04:02.000000 hata-1.3.8/hata/discord/http/rate_limit.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    62840 2022-07-09 15:04:43.000000 hata-1.3.8/hata/discord/http/rate_limit_groups.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    16822 2022-03-28 16:04:08.000000 hata-1.3.8/hata/discord/http/rate_limit_proxy.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    52310 2022-09-08 16:05:56.000000 hata-1.3.8/hata/discord/http/urls.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.100796 hata-1.3.8/hata/discord/integration/
--rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)      377 2021-10-08 11:30:50.000000 hata-1.3.8/hata/discord/integration/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4645 2022-08-28 11:14:25.000000 hata-1.3.8/hata/discord/integration/integration.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1747 2022-08-27 10:21:08.000000 hata-1.3.8/hata/discord/integration/integration_account.py
--rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)     1566 2022-08-28 11:20:15.000000 hata-1.3.8/hata/discord/integration/integration_application.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3705 2022-08-28 11:45:38.000000 hata-1.3.8/hata/discord/integration/integration_detail.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3450 2022-08-27 11:50:28.000000 hata-1.3.8/hata/discord/integration/preinstanced.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1343 2022-01-29 18:36:01.000000 hata-1.3.8/hata/discord/integration/utils.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.100796 hata-1.3.8/hata/discord/interaction/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      474 2022-03-08 18:56:07.000000 hata-1.3.8/hata/discord/interaction/__init__.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.100796 hata-1.3.8/hata/discord/interaction/application_command/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      615 2022-03-13 07:29:07.000000 hata-1.3.8/hata/discord/interaction/application_command/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    49742 2022-09-09 16:44:27.000000 hata-1.3.8/hata/discord/interaction/application_command/application_command.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    48998 2022-09-20 19:08:40.000000 hata-1.3.8/hata/discord/interaction/application_command/application_command_option.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    11548 2022-09-04 11:12:06.000000 hata-1.3.8/hata/discord/interaction/application_command/application_command_option_choice.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    12027 2022-03-09 05:58:16.000000 hata-1.3.8/hata/discord/interaction/application_command/application_command_permission.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    17631 2022-06-22 06:26:56.000000 hata-1.3.8/hata/discord/interaction/application_command/application_command_permission_overwrite.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      993 2022-07-08 07:09:41.000000 hata-1.3.8/hata/discord/interaction/application_command/constants.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2312 2022-03-19 14:22:38.000000 hata-1.3.8/hata/discord/interaction/application_command/helpers.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     6930 2022-03-08 18:56:07.000000 hata-1.3.8/hata/discord/interaction/application_command/preinstanced.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.104796 hata-1.3.8/hata/discord/interaction/components/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      695 2022-01-11 10:30:08.000000 hata-1.3.8/hata/discord/interaction/components/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3554 2022-01-11 10:30:08.000000 hata-1.3.8/hata/discord/interaction/components/component_base.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    14224 2022-04-01 06:49:08.000000 hata-1.3.8/hata/discord/interaction/components/component_button.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     5841 2022-01-11 11:11:32.000000 hata-1.3.8/hata/discord/interaction/components/component_dynamic.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     6777 2022-06-25 10:46:39.000000 hata-1.3.8/hata/discord/interaction/components/component_row.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    15101 2022-01-29 18:36:01.000000 hata-1.3.8/hata/discord/interaction/components/component_select.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     9637 2022-02-16 21:39:18.000000 hata-1.3.8/hata/discord/interaction/components/component_select_option.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    17822 2022-02-16 21:36:54.000000 hata-1.3.8/hata/discord/interaction/components/component_text_input.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      513 2022-03-30 04:35:46.000000 hata-1.3.8/hata/discord/interaction/components/constants.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    15456 2022-02-09 06:14:38.000000 hata-1.3.8/hata/discord/interaction/components/debug.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     9797 2022-01-29 18:36:01.000000 hata-1.3.8/hata/discord/interaction/components/form.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     6219 2022-04-01 06:51:12.000000 hata-1.3.8/hata/discord/interaction/components/preinstanced.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2049 2022-02-16 21:42:14.000000 hata-1.3.8/hata/discord/interaction/components/utils.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.104796 hata-1.3.8/hata/discord/interaction/event_types/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      572 2022-01-11 10:30:08.000000 hata-1.3.8/hata/discord/interaction/event_types/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    12859 2022-03-09 06:10:58.000000 hata-1.3.8/hata/discord/interaction/event_types/application_command_autocomplete_interaction.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    18259 2022-03-28 16:04:08.000000 hata-1.3.8/hata/discord/interaction/event_types/application_command_interaction.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3779 2022-03-30 17:03:25.000000 hata-1.3.8/hata/discord/interaction/event_types/component_interaction.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    12015 2022-02-09 06:49:19.000000 hata-1.3.8/hata/discord/interaction/event_types/form_submit_interaction.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    21908 2022-09-10 12:29:21.000000 hata-1.3.8/hata/discord/interaction/event_types/interaction_event.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1032 2022-01-11 10:30:08.000000 hata-1.3.8/hata/discord/interaction/event_types/interaction_field_base.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2534 2022-01-11 10:30:08.000000 hata-1.3.8/hata/discord/interaction/event_types/preinstanced.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     5570 2022-02-18 11:53:58.000000 hata-1.3.8/hata/discord/interaction/interaction_response_context.py
--rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)     1885 2021-12-07 08:47:45.000000 hata-1.3.8/hata/discord/interaction/interaction_response_types.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.104796 hata-1.3.8/hata/discord/invite/
--rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)      167 2021-10-08 11:30:50.000000 hata-1.3.8/hata/discord/invite/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    21773 2022-06-05 09:34:02.000000 hata-1.3.8/hata/discord/invite/invite.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1565 2022-02-22 19:02:04.000000 hata-1.3.8/hata/discord/invite/invite_stage.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2911 2022-01-18 14:47:29.000000 hata-1.3.8/hata/discord/invite/preinstanced.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.104796 hata-1.3.8/hata/discord/localizations/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      156 2022-03-12 09:12:10.000000 hata-1.3.8/hata/discord/localizations/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     7705 2022-08-21 17:04:24.000000 hata-1.3.8/hata/discord/localizations/helpers.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    11917 2022-03-30 17:03:25.000000 hata-1.3.8/hata/discord/localizations/preinstanced.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1773 2022-09-04 09:37:06.000000 hata-1.3.8/hata/discord/localizations/utils.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.108796 hata-1.3.8/hata/discord/message/
--rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)      928 2022-08-13 20:21:13.000000 hata-1.3.8/hata/discord/message/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3826 2022-08-21 09:29:47.000000 hata-1.3.8/hata/discord/message/attachment.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     6007 2022-09-04 09:28:51.000000 hata-1.3.8/hata/discord/message/cross_mention.py
--rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)     2304 2022-07-07 19:10:42.000000 hata-1.3.8/hata/discord/message/flags.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)   148927 2022-09-20 16:34:13.000000 hata-1.3.8/hata/discord/message/message.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1729 2022-01-01 15:01:19.000000 hata-1.3.8/hata/discord/message/message_activity.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2465 2022-01-01 15:01:36.000000 hata-1.3.8/hata/discord/message/message_application.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3712 2022-07-09 10:52:01.000000 hata-1.3.8/hata/discord/message/message_interaction.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    26128 2022-09-10 11:59:07.000000 hata-1.3.8/hata/discord/message/preinstanced.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3256 2022-03-29 16:37:14.000000 hata-1.3.8/hata/discord/message/utils.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.108796 hata-1.3.8/hata/discord/oauth2/
--rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)      474 2022-08-27 13:45:12.000000 hata-1.3.8/hata/discord/oauth2/__init__.py
--rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)     8184 2022-09-04 09:28:51.000000 hata-1.3.8/hata/discord/oauth2/achievement.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2570 2022-06-21 11:48:16.000000 hata-1.3.8/hata/discord/oauth2/connection.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3494 2022-08-28 11:05:03.000000 hata-1.3.8/hata/discord/oauth2/helpers.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4539 2022-08-29 18:18:22.000000 hata-1.3.8/hata/discord/oauth2/oauth2_access.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     8184 2022-08-27 13:51:43.000000 hata-1.3.8/hata/discord/oauth2/oauth2_user.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    14685 2022-09-10 17:15:24.000000 hata-1.3.8/hata/discord/oauth2/preinstanced.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    19549 2022-07-01 11:26:24.000000 hata-1.3.8/hata/discord/object_binding.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.112796 hata-1.3.8/hata/discord/permission/
--rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)      232 2021-10-08 11:30:50.000000 hata-1.3.8/hata/discord/permission/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    21446 2022-07-29 14:28:34.000000 hata-1.3.8/hata/discord/permission/permission.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    13722 2022-09-14 06:51:25.000000 hata-1.3.8/hata/discord/permission/permission_overwrite.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3060 2022-01-01 15:04:25.000000 hata-1.3.8/hata/discord/permission/preinstanced.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2093 2022-01-01 15:04:47.000000 hata-1.3.8/hata/discord/permission/utils.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    18336 2022-09-11 11:14:33.000000 hata-1.3.8/hata/discord/preconverters.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.112796 hata-1.3.8/hata/discord/role/
--rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)      150 2021-10-08 11:30:50.000000 hata-1.3.8/hata/discord/role/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2132 2022-01-01 15:04:59.000000 hata-1.3.8/hata/discord/role/preinstanced.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    27319 2022-09-04 09:28:51.000000 hata-1.3.8/hata/discord/role/role.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3729 2022-01-29 18:36:01.000000 hata-1.3.8/hata/discord/role/utils.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.112796 hata-1.3.8/hata/discord/scheduled_event/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      237 2022-09-17 11:24:36.000000 hata-1.3.8/hata/discord/scheduled_event/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2876 2022-01-01 15:05:53.000000 hata-1.3.8/hata/discord/scheduled_event/event_types.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.112796 hata-1.3.8/hata/discord/scheduled_event/metadata/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      183 2022-09-17 11:24:36.000000 hata-1.3.8/hata/discord/scheduled_event/metadata/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1486 2022-09-17 11:24:36.000000 hata-1.3.8/hata/discord/scheduled_event/metadata/base.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2214 2022-09-15 16:21:10.000000 hata-1.3.8/hata/discord/scheduled_event/metadata/location.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     5276 2022-09-17 11:24:36.000000 hata-1.3.8/hata/discord/scheduled_event/metadata/stage.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      701 2022-09-17 11:24:36.000000 hata-1.3.8/hata/discord/scheduled_event/metadata/utils.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     7043 2022-09-17 11:24:36.000000 hata-1.3.8/hata/discord/scheduled_event/preinstanced.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    16054 2022-09-17 11:24:36.000000 hata-1.3.8/hata/discord/scheduled_event/scheduled_event.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.112796 hata-1.3.8/hata/discord/stage/
--rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)       56 2021-10-08 11:30:50.000000 hata-1.3.8/hata/discord/stage/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     5904 2022-09-10 12:34:35.000000 hata-1.3.8/hata/discord/stage/stage.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.116796 hata-1.3.8/hata/discord/sticker/
--rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)      170 2021-10-08 11:30:50.000000 hata-1.3.8/hata/discord/sticker/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4799 2022-01-01 15:08:23.000000 hata-1.3.8/hata/discord/sticker/preinstanced.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    18590 2022-06-20 13:29:34.000000 hata-1.3.8/hata/discord/sticker/sticker.py
--rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)     2986 2022-01-01 15:08:48.000000 hata-1.3.8/hata/discord/sticker/sticker_pack.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.116796 hata-1.3.8/hata/discord/user/
--rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)      579 2021-10-08 11:30:50.000000 hata-1.3.8/hata/discord/user/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     6900 2022-09-10 12:14:09.000000 hata-1.3.8/hata/discord/user/activity_change.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    26891 2022-09-13 19:32:36.000000 hata-1.3.8/hata/discord/user/client_user_base.py
--rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)     5530 2022-09-18 13:19:53.000000 hata-1.3.8/hata/discord/user/flags.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     9283 2022-01-29 18:36:01.000000 hata-1.3.8/hata/discord/user/guild_profile.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      464 2021-12-31 07:39:40.000000 hata-1.3.8/hata/discord/user/helpers.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    20668 2022-01-22 15:49:29.000000 hata-1.3.8/hata/discord/user/preinstanced.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     7586 2022-06-21 09:21:00.000000 hata-1.3.8/hata/discord/user/thread_profile.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    21060 2022-09-05 06:49:03.000000 hata-1.3.8/hata/discord/user/user.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    23150 2022-09-05 06:49:03.000000 hata-1.3.8/hata/discord/user/user_base.py
--rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)      673 2022-07-09 10:55:07.000000 hata-1.3.8/hata/discord/user/utils.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    10337 2022-09-10 12:27:33.000000 hata-1.3.8/hata/discord/user/voice_state.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    55293 2022-09-06 16:34:02.000000 hata-1.3.8/hata/discord/utils.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.116796 hata-1.3.8/hata/discord/voice/
--rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)      342 2021-10-14 06:02:06.000000 hata-1.3.8/hata/discord/voice/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    15612 2022-01-29 18:36:01.000000 hata-1.3.8/hata/discord/voice/audio_source.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    15456 2022-02-22 11:10:46.000000 hata-1.3.8/hata/discord/voice/opus.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     8497 2022-07-30 12:34:23.000000 hata-1.3.8/hata/discord/voice/player.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    10241 2022-07-30 13:45:52.000000 hata-1.3.8/hata/discord/voice/reader.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    11434 2022-01-03 06:21:48.000000 hata-1.3.8/hata/discord/voice/rtp_packet.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      570 2022-02-17 18:36:16.000000 hata-1.3.8/hata/discord/voice/utils.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    45620 2022-09-10 12:27:19.000000 hata-1.3.8/hata/discord/voice/voice_client.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.120796 hata-1.3.8/hata/discord/webhook/
--rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)      266 2021-10-08 11:30:50.000000 hata-1.3.8/hata/discord/webhook/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1586 2022-01-01 15:14:37.000000 hata-1.3.8/hata/discord/webhook/preinstanced.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1179 2022-01-29 18:36:01.000000 hata-1.3.8/hata/discord/webhook/utils.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    13167 2022-03-29 17:19:38.000000 hata-1.3.8/hata/discord/webhook/webhook.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3245 2022-09-10 12:26:03.000000 hata-1.3.8/hata/discord/webhook/webhook_base.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2296 2022-01-01 15:16:28.000000 hata-1.3.8/hata/discord/webhook/webhook_repr.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4787 2022-09-10 12:25:11.000000 hata-1.3.8/hata/discord/webhook/webhook_sources.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     7386 2022-09-11 18:16:21.000000 hata-1.3.8/hata/env.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.120796 hata-1.3.8/hata/ext/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    11631 2022-07-22 10:48:20.000000 hata-1.3.8/hata/ext/__init__.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.120796 hata-1.3.8/hata/ext/asyncio/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      114 2022-02-09 06:14:08.000000 hata-1.3.8/hata/ext/asyncio/__init__.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.120796 hata-1.3.8/hata/ext/command_utils/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3289 2022-01-01 15:20:05.000000 hata-1.3.8/hata/ext/command_utils/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     9827 2022-03-29 16:37:14.000000 hata-1.3.8/hata/ext/command_utils/bases.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    27542 2022-08-13 12:58:20.000000 hata-1.3.8/hata/ext/command_utils/choose_menu.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    10907 2022-08-13 12:58:20.000000 hata-1.3.8/hata/ext/command_utils/closer.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    27070 2022-03-28 16:09:00.000000 hata-1.3.8/hata/ext/command_utils/io.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    17045 2022-08-13 12:58:20.000000 hata-1.3.8/hata/ext/command_utils/pagination.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    33237 2022-08-13 12:54:24.000000 hata-1.3.8/hata/ext/command_utils/user_menu.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4721 2022-01-01 15:23:52.000000 hata-1.3.8/hata/ext/command_utils/utils.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     8318 2022-03-28 16:04:08.000000 hata-1.3.8/hata/ext/command_utils/waiters.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.124796 hata-1.3.8/hata/ext/commands_v2/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4154 2022-05-29 07:45:33.000000 hata-1.3.8/hata/ext/commands_v2/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    14211 2022-04-11 07:14:10.000000 hata-1.3.8/hata/ext/commands_v2/category.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    66402 2022-08-13 12:53:14.000000 hata-1.3.8/hata/ext/commands_v2/checks.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1782 2022-04-10 06:35:31.000000 hata-1.3.8/hata/ext/commands_v2/client_wrapper_extension.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    60780 2022-04-23 10:51:03.000000 hata-1.3.8/hata/ext/commands_v2/command.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    27582 2022-08-13 12:58:20.000000 hata-1.3.8/hata/ext/commands_v2/command_helpers.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    38215 2022-04-05 17:19:46.000000 hata-1.3.8/hata/ext/commands_v2/command_processor.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)   120687 2022-09-10 16:51:11.000000 hata-1.3.8/hata/ext/commands_v2/content_parser.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    15017 2022-07-01 11:26:24.000000 hata-1.3.8/hata/ext/commands_v2/context.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     9003 2022-03-29 17:40:55.000000 hata-1.3.8/hata/ext/commands_v2/cooldown.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2497 2021-12-31 07:39:40.000000 hata-1.3.8/hata/ext/commands_v2/exceptions.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1859 2022-01-01 15:34:50.000000 hata-1.3.8/hata/ext/commands_v2/extension_hook_command_utils.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.124796 hata-1.3.8/hata/ext/commands_v2/helps/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    35121 2022-09-20 13:44:47.000000 hata-1.3.8/hata/ext/commands_v2/helps/subterranean.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4922 2022-07-23 15:19:52.000000 hata-1.3.8/hata/ext/commands_v2/responding.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     5715 2022-05-29 07:45:33.000000 hata-1.3.8/hata/ext/commands_v2/snapshot.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1188 2021-12-31 07:39:40.000000 hata-1.3.8/hata/ext/commands_v2/utils.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    10142 2022-01-30 21:05:04.000000 hata-1.3.8/hata/ext/commands_v2/wrappers.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.124796 hata-1.3.8/hata/ext/extension_loader/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      644 2022-05-29 12:23:59.000000 hata-1.3.8/hata/ext/extension_loader/__init__.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.124796 hata-1.3.8/hata/ext/kokoro_sqlalchemy/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      204 2022-01-01 15:37:42.000000 hata-1.3.8/hata/ext/kokoro_sqlalchemy/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     8835 2022-01-03 06:21:48.000000 hata-1.3.8/hata/ext/kokoro_sqlalchemy/kokoro_sqlalchemy.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.128796 hata-1.3.8/hata/ext/patchouli/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      604 2022-01-01 15:44:54.000000 hata-1.3.8/hata/ext/patchouli/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    15872 2022-07-26 19:23:21.000000 hata-1.3.8/hata/ext/patchouli/builder_html.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    57153 2022-08-26 17:18:47.000000 hata-1.3.8/hata/ext/patchouli/builder_html_extended.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    64584 2022-01-30 21:05:04.000000 hata-1.3.8/hata/ext/patchouli/builder_text.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    25270 2022-08-26 12:27:00.000000 hata-1.3.8/hata/ext/patchouli/graver.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1709 2022-07-26 19:10:31.000000 hata-1.3.8/hata/ext/patchouli/highlight.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    33027 2022-08-26 12:46:41.000000 hata-1.3.8/hata/ext/patchouli/module_mapper.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    46381 2022-08-26 15:51:56.000000 hata-1.3.8/hata/ext/patchouli/parser.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     6215 2021-12-31 07:39:40.000000 hata-1.3.8/hata/ext/patchouli/qualpath.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.128796 hata-1.3.8/hata/ext/plugin_loader/
--rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)     1282 2022-05-29 12:30:57.000000 hata-1.3.8/hata/ext/plugin_loader/__init__.py
--rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)     1332 2022-05-29 11:35:41.000000 hata-1.3.8/hata/ext/plugin_loader/client_extension.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      545 2022-05-29 11:28:11.000000 hata-1.3.8/hata/ext/plugin_loader/constants.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1845 2022-05-29 11:28:11.000000 hata-1.3.8/hata/ext/plugin_loader/exceptions.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    15934 2022-07-09 16:42:54.000000 hata-1.3.8/hata/ext/plugin_loader/helpers.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.132796 hata-1.3.8/hata/ext/plugin_loader/import_overwrite/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      463 2022-05-29 11:48:55.000000 hata-1.3.8/hata/ext/plugin_loader/import_overwrite/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3324 2022-06-05 14:10:40.000000 hata-1.3.8/hata/ext/plugin_loader/import_overwrite/module_proxy_type.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1965 2022-05-29 11:38:58.000000 hata-1.3.8/hata/ext/plugin_loader/import_overwrite/module_spec_type.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1495 2022-05-29 11:48:29.000000 hata-1.3.8/hata/ext/plugin_loader/import_overwrite/plugin_finder.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2700 2022-05-29 11:38:58.000000 hata-1.3.8/hata/ext/plugin_loader/import_overwrite/source_loader.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3939 2022-04-23 08:16:05.000000 hata-1.3.8/hata/ext/plugin_loader/import_overwrite/spec_finder_helpers.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      700 2022-05-29 11:40:53.000000 hata-1.3.8/hata/ext/plugin_loader/import_overwrite/tools.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1258 2022-05-29 11:40:53.000000 hata-1.3.8/hata/ext/plugin_loader/import_overwrite/utils.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    32751 2022-06-24 18:59:56.000000 hata-1.3.8/hata/ext/plugin_loader/plugin.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    61737 2022-06-21 09:28:23.000000 hata-1.3.8/hata/ext/plugin_loader/plugin_loader.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1917 2022-05-29 10:44:16.000000 hata-1.3.8/hata/ext/plugin_loader/plugin_root.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.132796 hata-1.3.8/hata/ext/plugin_loader/snapshot/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      249 2022-04-03 20:17:22.000000 hata-1.3.8/hata/ext/plugin_loader/snapshot/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3131 2022-05-29 11:37:52.000000 hata-1.3.8/hata/ext/plugin_loader/snapshot/base_snapshot_type.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    10685 2022-04-13 18:56:01.000000 hata-1.3.8/hata/ext/plugin_loader/snapshot/event_handler_snapshot.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3561 2022-04-05 16:52:24.000000 hata-1.3.8/hata/ext/plugin_loader/snapshot/helpers.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2912 2022-04-03 20:19:43.000000 hata-1.3.8/hata/ext/plugin_loader/snapshot/snapshot.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.136796 hata-1.3.8/hata/ext/plugin_loader/utils/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1094 2022-06-04 17:11:21.000000 hata-1.3.8/hata/ext/plugin_loader/utils/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      279 2022-06-04 17:08:57.000000 hata-1.3.8/hata/ext/plugin_loader/utils/add_default_plugin_variables_.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      263 2022-06-04 17:09:15.000000 hata-1.3.8/hata/ext/plugin_loader/utils/clear_default_plugin_variables_.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      205 2022-05-29 13:39:45.000000 hata-1.3.8/hata/ext/plugin_loader/utils/get_plugin_.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1275 2022-06-05 15:43:34.000000 hata-1.3.8/hata/ext/plugin_loader/utils/get_plugin_like_.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1343 2022-06-05 14:31:43.000000 hata-1.3.8/hata/ext/plugin_loader/utils/get_plugins_like_.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     5202 2022-06-07 08:59:40.000000 hata-1.3.8/hata/ext/plugin_loader/utils/import_plugin_.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      232 2022-06-04 18:13:51.000000 hata-1.3.8/hata/ext/plugin_loader/utils/load_all_plugin_.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      254 2022-06-04 18:17:06.000000 hata-1.3.8/hata/ext/plugin_loader/utils/load_plugin_.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      351 2022-05-29 13:04:44.000000 hata-1.3.8/hata/ext/plugin_loader/utils/register_and_load_plugin_.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      303 2022-06-02 05:34:36.000000 hata-1.3.8/hata/ext/plugin_loader/utils/register_plugin_.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      238 2022-06-04 18:13:51.000000 hata-1.3.8/hata/ext/plugin_loader/utils/reload_all_plugin_.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      262 2022-05-29 13:16:20.000000 hata-1.3.8/hata/ext/plugin_loader/utils/reload_plugin_.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      277 2022-06-04 17:08:21.000000 hata-1.3.8/hata/ext/plugin_loader/utils/remove_default_plugin_variables_.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1049 2022-05-29 11:37:28.000000 hata-1.3.8/hata/ext/plugin_loader/utils/require_.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      238 2022-06-04 18:13:51.000000 hata-1.3.8/hata/ext/plugin_loader/utils/unload_all_plugin_.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      262 2022-05-29 13:15:10.000000 hata-1.3.8/hata/ext/plugin_loader/utils/unload_plugin_.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.136796 hata-1.3.8/hata/ext/prettyprint/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      339 2022-03-30 16:48:40.000000 hata-1.3.8/hata/ext/prettyprint/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    64461 2022-09-05 06:44:16.000000 hata-1.3.8/hata/ext/prettyprint/prettyprint.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.140796 hata-1.3.8/hata/ext/slash/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4768 2022-05-29 07:45:33.000000 hata-1.3.8/hata/ext/slash/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1790 2022-05-21 09:00:27.000000 hata-1.3.8/hata/ext/slash/client_wrapper_extension.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.140796 hata-1.3.8/hata/ext/slash/command/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      543 2022-05-22 08:21:16.000000 hata-1.3.8/hata/ext/slash/command/__init__.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.140796 hata-1.3.8/hata/ext/slash/command/command_base/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)       59 2022-05-21 08:50:27.000000 hata-1.3.8/hata/ext/slash/command/command_base/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     8010 2022-09-03 16:28:58.000000 hata-1.3.8/hata/ext/slash/command/command_base/command_base.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.140796 hata-1.3.8/hata/ext/slash/command/command_base_application_command/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      204 2022-05-22 08:10:06.000000 hata-1.3.8/hata/ext/slash/command/command_base_application_command/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    24199 2022-09-03 16:52:05.000000 hata-1.3.8/hata/ext/slash/command/command_base_application_command/command_base_application_command.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      602 2022-05-21 11:33:16.000000 hata-1.3.8/hata/ext/slash/command/command_base_application_command/constants.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     8109 2022-09-03 17:55:57.000000 hata-1.3.8/hata/ext/slash/command/command_base_application_command/helpers.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.140796 hata-1.3.8/hata/ext/slash/command/command_base_custom_id/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      135 2022-05-21 08:50:27.000000 hata-1.3.8/hata/ext/slash/command/command_base_custom_id/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     8230 2022-05-22 12:40:02.000000 hata-1.3.8/hata/ext/slash/command/command_base_custom_id/command_base_custom_id.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     5250 2022-05-21 08:17:58.000000 hata-1.3.8/hata/ext/slash/command/command_base_custom_id/helpers.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.140796 hata-1.3.8/hata/ext/slash/command/component_command/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      129 2022-05-21 09:08:00.000000 hata-1.3.8/hata/ext/slash/command/component_command/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     8436 2022-05-22 14:02:34.000000 hata-1.3.8/hata/ext/slash/command/component_command/component_command.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)       82 2022-05-21 09:06:28.000000 hata-1.3.8/hata/ext/slash/command/component_command/constants.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.144796 hata-1.3.8/hata/ext/slash/command/context_command/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)       66 2022-05-22 08:57:34.000000 hata-1.3.8/hata/ext/slash/command/context_command/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    17262 2022-09-03 16:48:22.000000 hata-1.3.8/hata/ext/slash/command/context_command/context_command.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.144796 hata-1.3.8/hata/ext/slash/command/form_submit_command/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      133 2022-05-21 09:09:22.000000 hata-1.3.8/hata/ext/slash/command/form_submit_command/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      102 2022-05-21 09:10:29.000000 hata-1.3.8/hata/ext/slash/command/form_submit_command/constants.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    11198 2022-05-22 14:02:34.000000 hata-1.3.8/hata/ext/slash/command/form_submit_command/form_submit_command.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2432 2022-05-22 08:23:25.000000 hata-1.3.8/hata/ext/slash/command/helpers.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.144796 hata-1.3.8/hata/ext/slash/command/slash_command/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      374 2022-05-22 08:10:06.000000 hata-1.3.8/hata/ext/slash/command/slash_command/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     6527 2022-05-22 08:58:01.000000 hata-1.3.8/hata/ext/slash/command/slash_command/helpers.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    34252 2022-09-03 16:53:33.000000 hata-1.3.8/hata/ext/slash/command/slash_command/slash_command.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    21492 2022-09-03 16:21:15.000000 hata-1.3.8/hata/ext/slash/command/slash_command/slash_command_category.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    20475 2022-09-03 16:15:30.000000 hata-1.3.8/hata/ext/slash/command/slash_command/slash_command_function.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    12765 2022-05-22 12:40:02.000000 hata-1.3.8/hata/ext/slash/command/slash_command/slash_command_parameter_auto_completer.py
--rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)     1464 2022-02-22 11:48:23.000000 hata-1.3.8/hata/ext/slash/components.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)   121565 2022-09-20 19:10:44.000000 hata-1.3.8/hata/ext/slash/converters.py
--rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)     3097 2022-01-01 16:00:19.000000 hata-1.3.8/hata/ext/slash/event_handlers.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    18385 2022-05-21 09:00:27.000000 hata-1.3.8/hata/ext/slash/exceptions.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    87061 2022-09-04 19:34:56.000000 hata-1.3.8/hata/ext/slash/expression_parser.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     5408 2022-03-13 15:01:47.000000 hata-1.3.8/hata/ext/slash/helpers.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.148796 hata-1.3.8/hata/ext/slash/menus/
--rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)      193 2021-10-08 11:30:50.000000 hata-1.3.8/hata/ext/slash/menus/__init__.py
--rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)     1142 2022-01-01 15:56:30.000000 hata-1.3.8/hata/ext/slash/menus/closer.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2693 2022-01-01 15:56:52.000000 hata-1.3.8/hata/ext/slash/menus/helpers.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    71347 2022-03-29 17:25:36.000000 hata-1.3.8/hata/ext/slash/menus/menu.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3056 2022-01-01 15:57:28.000000 hata-1.3.8/hata/ext/slash/menus/pagination.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    12486 2022-05-26 16:47:21.000000 hata-1.3.8/hata/ext/slash/permission_mismatch.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    28854 2022-07-23 15:19:52.000000 hata-1.3.8/hata/ext/slash/responding.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    12231 2022-05-22 07:41:34.000000 hata-1.3.8/hata/ext/slash/response_modifier.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)   138703 2022-09-03 17:46:13.000000 hata-1.3.8/hata/ext/slash/slasher.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    30311 2022-06-10 12:17:10.000000 hata-1.3.8/hata/ext/slash/snapshot.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4287 2022-05-21 09:00:27.000000 hata-1.3.8/hata/ext/slash/utils.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    20071 2022-01-30 21:05:04.000000 hata-1.3.8/hata/ext/slash/waiters.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    18356 2022-07-09 07:05:28.000000 hata-1.3.8/hata/ext/slash/wrappers.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.148796 hata-1.3.8/hata/ext/solarlink/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2828 2022-01-07 06:45:14.000000 hata-1.3.8/hata/ext/solarlink/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    20857 2022-06-24 15:31:16.000000 hata-1.3.8/hata/ext/solarlink/client.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     6341 2022-04-13 15:19:18.000000 hata-1.3.8/hata/ext/solarlink/constants.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3277 2022-04-12 18:06:32.000000 hata-1.3.8/hata/ext/solarlink/event_handler_plugin.py
--rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)     5189 2022-07-22 10:31:27.000000 hata-1.3.8/hata/ext/solarlink/event_handlers.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    14885 2022-04-12 17:03:54.000000 hata-1.3.8/hata/ext/solarlink/event_types.py
--rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)      797 2021-10-17 07:01:34.000000 hata-1.3.8/hata/ext/solarlink/exceptions.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    46416 2022-08-26 17:19:05.000000 hata-1.3.8/hata/ext/solarlink/filters.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    17384 2022-07-30 13:47:28.000000 hata-1.3.8/hata/ext/solarlink/node.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2469 2022-01-07 06:45:14.000000 hata-1.3.8/hata/ext/solarlink/parsers.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    17593 2022-01-30 21:05:04.000000 hata-1.3.8/hata/ext/solarlink/player.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    16714 2022-09-10 12:24:18.000000 hata-1.3.8/hata/ext/solarlink/player_base.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    10534 2022-04-12 16:01:31.000000 hata-1.3.8/hata/ext/solarlink/route_planner.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     6836 2022-04-12 16:01:31.000000 hata-1.3.8/hata/ext/solarlink/stats.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    22928 2022-04-12 17:18:47.000000 hata-1.3.8/hata/ext/solarlink/track.py
--rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)      126 2021-10-13 10:24:10.000000 hata-1.3.8/hata/ext/solarlink/track_end_reasons.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.152796 hata-1.3.8/hata/ext/top_gg/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2538 2021-12-31 07:39:40.000000 hata-1.3.8/hata/ext/top_gg/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     9987 2022-01-01 16:13:06.000000 hata-1.3.8/hata/ext/top_gg/bots_query.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    29423 2022-02-08 13:40:47.000000 hata-1.3.8/hata/ext/top_gg/client.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3042 2021-11-17 13:40:43.000000 hata-1.3.8/hata/ext/top_gg/constants.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2217 2022-01-01 16:15:52.000000 hata-1.3.8/hata/ext/top_gg/exceptions.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     7235 2022-02-14 09:47:14.000000 hata-1.3.8/hata/ext/top_gg/rate_limit_handling.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    21055 2022-01-03 06:21:48.000000 hata-1.3.8/hata/ext/top_gg/types.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.152796 hata-1.3.8/hata/main/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)       54 2022-07-13 16:54:39.000000 hata-1.3.8/hata/main/__init__.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.052796 hata-1.3.8/hata/main/commands/
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.152796 hata-1.3.8/hata/main/commands/default/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      103 2022-07-22 10:15:41.000000 hata-1.3.8/hata/main/commands/default/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2676 2022-07-20 14:41:30.000000 hata-1.3.8/hata/main/commands/default/help.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      723 2022-08-08 20:32:18.000000 hata-1.3.8/hata/main/commands/default/interpreter.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     8789 2022-07-22 11:39:24.000000 hata-1.3.8/hata/main/commands/default/run.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1422 2022-07-13 18:52:36.000000 hata-1.3.8/hata/main/commands/default/version.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.156796 hata-1.3.8/hata/main/core/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      345 2022-07-20 16:38:31.000000 hata-1.3.8/hata/main/core/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1997 2022-07-22 10:28:29.000000 hata-1.3.8/hata/main/core/call.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.156796 hata-1.3.8/hata/main/core/command/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      549 2022-07-16 08:18:34.000000 hata-1.3.8/hata/main/core/command/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    14229 2022-07-16 13:23:41.000000 hata-1.3.8/hata/main/core/command/category.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     8260 2022-07-18 17:24:18.000000 hata-1.3.8/hata/main/core/command/command.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    17685 2022-07-18 11:50:58.000000 hata-1.3.8/hata/main/core/command/function.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4806 2022-07-16 09:44:12.000000 hata-1.3.8/hata/main/core/command/helpers.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     7121 2022-07-16 12:58:19.000000 hata-1.3.8/hata/main/core/command/parameter.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    13820 2022-07-16 08:28:10.000000 hata-1.3.8/hata/main/core/command/parameter_renderer.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     8140 2022-07-16 08:45:29.000000 hata-1.3.8/hata/main/core/command/parameter_result.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1276 2022-07-16 12:03:37.000000 hata-1.3.8/hata/main/core/command/render_constants.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4699 2022-07-20 14:43:13.000000 hata-1.3.8/hata/main/core/command/rendering_helpers.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    13708 2022-07-20 14:44:44.000000 hata-1.3.8/hata/main/core/command/result.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      654 2022-07-19 13:26:33.000000 hata-1.3.8/hata/main/core/constants.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2980 2022-07-19 14:08:50.000000 hata-1.3.8/hata/main/core/external.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1835 2022-07-20 16:37:40.000000 hata-1.3.8/hata/main/core/helpers.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3443 2022-07-22 10:11:07.000000 hata-1.3.8/hata/main/core/lookup.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2420 2022-07-16 13:32:32.000000 hata-1.3.8/hata/main/core/registration.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.156796 hata-1.3.8/hata/utils/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      123 2022-03-27 19:55:08.000000 hata-1.3.8/hata/utils/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1447 2022-03-27 17:16:16.000000 hata-1.3.8/hata/utils/debug.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2848 2022-09-05 06:54:56.000000 hata-1.3.8/hata/utils/module_deprecation.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-09-20 19:23:34.056796 hata-1.3.8/hata.egg-info/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     8427 2022-09-20 19:23:33.000000 hata-1.3.8/hata.egg-info/PKG-INFO
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    21715 2022-09-20 19:23:33.000000 hata-1.3.8/hata.egg-info/SOURCES.txt
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)        1 2022-09-20 19:23:33.000000 hata-1.3.8/hata.egg-info/dependency_links.txt
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)       49 2022-09-20 19:23:33.000000 hata-1.3.8/hata.egg-info/entry_points.txt
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      125 2022-09-20 19:23:33.000000 hata-1.3.8/hata.egg-info/requires.txt
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)        5 2022-09-20 19:23:33.000000 hata-1.3.8/hata.egg-info/top_level.txt
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)       38 2022-09-20 19:23:34.160796 hata-1.3.8/setup.cfg
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     5166 2022-09-17 11:24:36.000000 hata-1.3.8/setup.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.837734 hata-1.3.9/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     8427 2022-10-03 12:28:55.837734 hata-1.3.9/PKG-INFO
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     5410 2022-08-13 12:35:16.000000 hata-1.3.9/README.md
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.709734 hata-1.3.9/hata/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3160 2022-10-03 11:13:41.000000 hata-1.3.9/hata/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1011 2022-07-22 10:09:55.000000 hata-1.3.9/hata/__main__.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.709734 hata-1.3.9/hata/backend/
+-rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)      574 2022-03-30 17:00:03.000000 hata-1.3.9/hata/backend/__init__.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.713734 hata-1.3.9/hata/discord/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1624 2022-06-24 19:36:38.000000 hata-1.3.9/hata/discord/__init__.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.713734 hata-1.3.9/hata/discord/activity/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      686 2022-09-05 21:05:42.000000 hata-1.3.9/hata/discord/activity/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    23332 2022-09-13 10:43:13.000000 hata-1.3.9/hata/discord/activity/activity.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      408 2022-09-08 14:15:22.000000 hata-1.3.9/hata/discord/activity/constants.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.717734 hata-1.3.9/hata/discord/activity/fields/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      234 2022-09-06 15:02:25.000000 hata-1.3.9/hata/discord/activity/fields/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     9239 2022-09-04 15:55:06.000000 hata-1.3.9/hata/discord/activity/fields/assets.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1427 2022-09-04 13:32:06.000000 hata-1.3.9/hata/discord/activity/fields/base.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     6018 2022-09-04 15:52:11.000000 hata-1.3.9/hata/discord/activity/fields/party.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     6411 2022-09-04 19:14:48.000000 hata-1.3.9/hata/discord/activity/fields/secrets.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4963 2022-09-06 15:11:39.000000 hata-1.3.9/hata/discord/activity/fields/timestamps.py
+-rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)     1756 2021-10-08 11:30:50.000000 hata-1.3.9/hata/discord/activity/flags.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.717734 hata-1.3.9/hata/discord/activity/metadata/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      136 2022-09-04 17:08:56.000000 hata-1.3.9/hata/discord/activity/metadata/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     9160 2022-09-13 10:27:02.000000 hata-1.3.9/hata/discord/activity/metadata/base.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     6045 2022-09-13 10:33:03.000000 hata-1.3.9/hata/discord/activity/metadata/custom.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    19600 2022-09-13 10:33:03.000000 hata-1.3.9/hata/discord/activity/metadata/rich.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4621 2022-09-10 17:20:10.000000 hata-1.3.9/hata/discord/activity/preinstanced.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    41730 2022-02-13 12:17:28.000000 hata-1.3.9/hata/discord/allowed_mentions.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    12248 2022-07-30 20:58:26.000000 hata-1.3.9/hata/discord/ansi_format.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.717734 hata-1.3.9/hata/discord/application/
+-rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)      354 2022-02-15 15:10:02.000000 hata-1.3.9/hata/discord/application/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    23321 2022-03-30 17:00:03.000000 hata-1.3.9/hata/discord/application/application.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4702 2022-02-17 18:12:57.000000 hata-1.3.9/hata/discord/application/embedded_activity_configuration.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3719 2022-07-23 08:26:02.000000 hata-1.3.9/hata/discord/application/flags.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     9284 2022-01-22 18:27:00.000000 hata-1.3.9/hata/discord/application/miscellaneous.py
+-rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)    22953 2022-07-29 14:09:19.000000 hata-1.3.9/hata/discord/application/preinstanced.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     5237 2022-02-22 17:34:04.000000 hata-1.3.9/hata/discord/application/team.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.721734 hata-1.3.9/hata/discord/auto_moderation/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      384 2022-09-17 11:24:36.000000 hata-1.3.9/hata/discord/auto_moderation/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     9884 2022-09-17 11:24:36.000000 hata-1.3.9/hata/discord/auto_moderation/action.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.721734 hata-1.3.9/hata/discord/auto_moderation/action_metadata/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      157 2022-09-17 11:24:36.000000 hata-1.3.9/hata/discord/auto_moderation/action_metadata/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3296 2022-09-17 11:24:36.000000 hata-1.3.9/hata/discord/auto_moderation/action_metadata/alert_message.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1705 2022-09-17 11:24:36.000000 hata-1.3.9/hata/discord/auto_moderation/action_metadata/base.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3128 2022-09-17 11:24:36.000000 hata-1.3.9/hata/discord/auto_moderation/action_metadata/timeout.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      106 2022-07-23 09:47:31.000000 hata-1.3.9/hata/discord/auto_moderation/constants.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     8719 2022-09-10 12:47:35.000000 hata-1.3.9/hata/discord/auto_moderation/event_types.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    14662 2022-09-17 11:24:36.000000 hata-1.3.9/hata/discord/auto_moderation/preinstanced.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    49626 2022-09-17 11:24:36.000000 hata-1.3.9/hata/discord/auto_moderation/rule.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.721734 hata-1.3.9/hata/discord/auto_moderation/trigger_metadata/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      254 2022-09-17 11:24:36.000000 hata-1.3.9/hata/discord/auto_moderation/trigger_metadata/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1741 2022-09-17 11:24:36.000000 hata-1.3.9/hata/discord/auto_moderation/trigger_metadata/base.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     7744 2022-09-17 11:24:36.000000 hata-1.3.9/hata/discord/auto_moderation/trigger_metadata/keyword.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    10806 2022-09-17 11:24:36.000000 hata-1.3.9/hata/discord/auto_moderation/trigger_metadata/keyword_preset.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3489 2022-09-17 11:24:36.000000 hata-1.3.9/hata/discord/auto_moderation/trigger_metadata/mention_spam.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      950 2022-09-17 11:24:36.000000 hata-1.3.9/hata/discord/auto_moderation/trigger_metadata/utils.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.725734 hata-1.3.9/hata/discord/bases/
+-rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)      342 2022-09-12 06:18:05.000000 hata-1.3.9/hata/discord/bases/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     8061 2022-09-12 06:18:05.000000 hata-1.3.9/hata/discord/bases/entity.py
+-rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)      920 2021-12-19 12:03:10.000000 hata-1.3.9/hata/discord/bases/event_types.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    16895 2022-03-06 13:34:11.000000 hata-1.3.9/hata/discord/bases/flags.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    16568 2022-09-17 11:24:36.000000 hata-1.3.9/hata/discord/bases/icon.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2886 2022-09-12 06:18:05.000000 hata-1.3.9/hata/discord/bases/place_holder.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     8363 2022-08-27 06:51:27.000000 hata-1.3.9/hata/discord/bases/preinstanced.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    12351 2022-01-03 06:21:48.000000 hata-1.3.9/hata/discord/bases/utils.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.725734 hata-1.3.9/hata/discord/channel/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      575 2022-09-11 16:08:40.000000 hata-1.3.9/hata/discord/channel/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    78641 2022-09-28 15:51:57.000000 hata-1.3.9/hata/discord/channel/channel.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.725734 hata-1.3.9/hata/discord/channel/channel_type/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      111 2022-09-10 12:01:02.000000 hata-1.3.9/hata/discord/channel/channel_type/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3511 2022-09-10 11:44:14.000000 hata-1.3.9/hata/discord/channel/channel_type/flags.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    13813 2022-09-10 12:25:11.000000 hata-1.3.9/hata/discord/channel/channel_type/preinstanced.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      450 2022-09-18 11:32:28.000000 hata-1.3.9/hata/discord/channel/constants.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    13279 2022-09-10 13:45:45.000000 hata-1.3.9/hata/discord/channel/deprecation.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.733734 hata-1.3.9/hata/discord/channel/fields/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1365 2022-09-17 11:24:36.000000 hata-1.3.9/hata/discord/channel/fields/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3289 2022-09-17 11:24:36.000000 hata-1.3.9/hata/discord/channel/fields/applied_tag_ids.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1598 2022-09-14 19:48:39.000000 hata-1.3.9/hata/discord/channel/fields/archived.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2343 2022-09-14 15:55:58.000000 hata-1.3.9/hata/discord/channel/fields/archived_at.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2325 2022-09-14 11:52:07.000000 hata-1.3.9/hata/discord/channel/fields/auto_archive_after.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2703 2022-09-17 15:29:16.000000 hata-1.3.9/hata/discord/channel/fields/available_tags.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1417 2022-09-17 11:24:36.000000 hata-1.3.9/hata/discord/channel/fields/bitrate.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2307 2022-09-14 13:04:36.000000 hata-1.3.9/hata/discord/channel/fields/created_at.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2327 2022-09-14 11:52:06.000000 hata-1.3.9/hata/discord/channel/fields/default_thread_auto_archive_after.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2342 2022-09-13 12:14:26.000000 hata-1.3.9/hata/discord/channel/fields/default_thread_reaction.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2008 2022-09-13 12:24:48.000000 hata-1.3.9/hata/discord/channel/fields/default_thread_slowmode.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1351 2022-09-13 12:41:43.000000 hata-1.3.9/hata/discord/channel/fields/flags.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1700 2022-09-14 19:59:35.000000 hata-1.3.9/hata/discord/channel/fields/invitable.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1501 2022-09-13 13:21:46.000000 hata-1.3.9/hata/discord/channel/fields/name.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1244 2022-09-14 19:48:51.000000 hata-1.3.9/hata/discord/channel/fields/nsfw.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1532 2022-09-14 19:48:26.000000 hata-1.3.9/hata/discord/channel/fields/open_.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2145 2022-09-14 15:25:40.000000 hata-1.3.9/hata/discord/channel/fields/owner_id.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2083 2022-09-14 15:25:20.000000 hata-1.3.9/hata/discord/channel/fields/parent_id.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3075 2022-09-14 10:32:58.000000 hata-1.3.9/hata/discord/channel/fields/permission_overwrites.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1494 2022-09-13 13:28:19.000000 hata-1.3.9/hata/discord/channel/fields/position.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1793 2022-09-17 11:24:36.000000 hata-1.3.9/hata/discord/channel/fields/region.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1691 2022-09-14 10:48:21.000000 hata-1.3.9/hata/discord/channel/fields/slowmode.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1610 2022-09-13 13:21:48.000000 hata-1.3.9/hata/discord/channel/fields/topic.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1568 2022-09-17 11:24:36.000000 hata-1.3.9/hata/discord/channel/fields/user_limit.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2402 2022-09-17 11:24:36.000000 hata-1.3.9/hata/discord/channel/fields/users.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2042 2022-09-14 21:24:46.000000 hata-1.3.9/hata/discord/channel/fields/video_quality_mode.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1232 2022-09-08 16:59:33.000000 hata-1.3.9/hata/discord/channel/flags.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    15196 2022-09-24 07:31:15.000000 hata-1.3.9/hata/discord/channel/forum_tag.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     6041 2022-03-29 16:37:14.000000 hata-1.3.9/hata/discord/channel/message_history.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     6721 2022-03-27 08:13:18.000000 hata-1.3.9/hata/discord/channel/message_iterator.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.737734 hata-1.3.9/hata/discord/channel/metadata/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1188 2022-09-10 16:36:03.000000 hata-1.3.9/hata/discord/channel/metadata/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    28373 2022-09-18 11:32:58.000000 hata-1.3.9/hata/discord/channel/metadata/base.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3397 2022-09-12 18:46:22.000000 hata-1.3.9/hata/discord/channel/metadata/guild_announcements.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    10718 2022-09-20 15:47:34.000000 hata-1.3.9/hata/discord/channel/metadata/guild_base.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1065 2022-09-12 18:46:13.000000 hata-1.3.9/hata/discord/channel/metadata/guild_category.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2158 2022-09-12 18:46:03.000000 hata-1.3.9/hata/discord/channel/metadata/guild_directory.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    11824 2022-09-18 10:23:05.000000 hata-1.3.9/hata/discord/channel/metadata/guild_forum.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    12197 2022-09-18 10:41:57.000000 hata-1.3.9/hata/discord/channel/metadata/guild_main_base.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4991 2022-09-18 10:09:48.000000 hata-1.3.9/hata/discord/channel/metadata/guild_stage.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4475 2022-09-18 10:11:00.000000 hata-1.3.9/hata/discord/channel/metadata/guild_store.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3080 2022-09-11 12:47:35.000000 hata-1.3.9/hata/discord/channel/metadata/guild_text.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     8763 2022-09-18 10:13:10.000000 hata-1.3.9/hata/discord/channel/metadata/guild_text_base.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1676 2022-09-12 18:49:28.000000 hata-1.3.9/hata/discord/channel/metadata/guild_thread_announcements.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    12444 2022-09-18 10:16:39.000000 hata-1.3.9/hata/discord/channel/metadata/guild_thread_base.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4293 2022-09-18 10:17:27.000000 hata-1.3.9/hata/discord/channel/metadata/guild_thread_private.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     5116 2022-09-17 11:24:36.000000 hata-1.3.9/hata/discord/channel/metadata/guild_thread_public.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     6224 2022-09-18 10:42:48.000000 hata-1.3.9/hata/discord/channel/metadata/guild_voice.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     5429 2022-09-18 10:20:20.000000 hata-1.3.9/hata/discord/channel/metadata/guild_voice_base.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2140 2022-09-20 15:49:31.000000 hata-1.3.9/hata/discord/channel/metadata/private.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2827 2022-09-20 16:03:03.000000 hata-1.3.9/hata/discord/channel/metadata/private_base.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     7222 2022-09-18 10:24:28.000000 hata-1.3.9/hata/discord/channel/metadata/private_group.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1938 2022-09-10 09:29:57.000000 hata-1.3.9/hata/discord/channel/preinstanced.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    25631 2022-09-20 19:07:06.000000 hata-1.3.9/hata/discord/channel/utils.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.737734 hata-1.3.9/hata/discord/client/
+-rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)      341 2022-06-24 10:45:11.000000 hata-1.3.9/hata/discord/client/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    71537 2022-09-05 06:46:18.000000 hata-1.3.9/hata/discord/client/client.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.745734 hata-1.3.9/hata/discord/client/compounds/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3547 2022-07-23 10:23:30.000000 hata-1.3.9/hata/discord/client/compounds/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    22326 2022-08-27 13:40:29.000000 hata-1.3.9/hata/discord/client/compounds/achievement.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    33411 2022-08-27 17:24:17.000000 hata-1.3.9/hata/discord/client/compounds/application_command.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     7337 2022-07-09 07:24:07.000000 hata-1.3.9/hata/discord/client/compounds/auto_moderation.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    40520 2022-09-25 10:27:24.000000 hata-1.3.9/hata/discord/client/compounds/channel.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    20278 2022-08-13 12:52:25.000000 hata-1.3.9/hata/discord/client/compounds/client.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    14125 2022-09-13 10:35:29.000000 hata-1.3.9/hata/discord/client/compounds/client_gayteway.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    13119 2022-06-24 15:26:58.000000 hata-1.3.9/hata/discord/client/compounds/discovery.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    13922 2022-06-24 15:25:27.000000 hata-1.3.9/hata/discord/client/compounds/emoji.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    76341 2022-09-10 16:28:10.000000 hata-1.3.9/hata/discord/client/compounds/guild.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    10642 2022-07-23 11:06:48.000000 hata-1.3.9/hata/discord/client/compounds/guild_ban.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    10418 2022-06-24 10:55:13.000000 hata-1.3.9/hata/discord/client/compounds/integration.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    44383 2022-08-13 20:06:27.000000 hata-1.3.9/hata/discord/client/compounds/interaction.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    24933 2022-09-10 17:04:19.000000 hata-1.3.9/hata/discord/client/compounds/invite.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     7853 2022-06-24 10:53:08.000000 hata-1.3.9/hata/discord/client/compounds/locked.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    81858 2022-09-10 16:04:00.000000 hata-1.3.9/hata/discord/client/compounds/message.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     5476 2022-09-10 16:04:00.000000 hata-1.3.9/hata/discord/client/compounds/miscellaneous.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    18751 2022-08-28 11:05:03.000000 hata-1.3.9/hata/discord/client/compounds/oauth2.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    13727 2022-08-13 20:14:14.000000 hata-1.3.9/hata/discord/client/compounds/reaction.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    28535 2022-06-24 15:26:58.000000 hata-1.3.9/hata/discord/client/compounds/role.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    22947 2022-06-24 15:25:27.000000 hata-1.3.9/hata/discord/client/compounds/scheduled_event.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     7996 2022-06-24 10:52:15.000000 hata-1.3.9/hata/discord/client/compounds/stage.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    19362 2022-06-24 10:52:15.000000 hata-1.3.9/hata/discord/client/compounds/sticker.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    30693 2022-09-18 10:50:22.000000 hata-1.3.9/hata/discord/client/compounds/thread.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    22243 2022-08-21 19:02:35.000000 hata-1.3.9/hata/discord/client/compounds/user.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    39005 2022-09-10 16:28:10.000000 hata-1.3.9/hata/discord/client/compounds/webhook.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    38431 2022-09-18 10:50:22.000000 hata-1.3.9/hata/discord/client/functionality_helpers.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    14350 2022-03-29 18:05:43.000000 hata-1.3.9/hata/discord/client/ready_state.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    59497 2022-08-13 20:04:51.000000 hata-1.3.9/hata/discord/client/request_helpers.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    16687 2022-07-25 20:28:21.000000 hata-1.3.9/hata/discord/client/utils.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    18275 2022-06-12 11:16:32.000000 hata-1.3.9/hata/discord/color.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     5584 2022-09-09 16:10:40.000000 hata-1.3.9/hata/discord/core.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.745734 hata-1.3.9/hata/discord/embed/
+-rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)      158 2021-10-08 11:30:50.000000 hata-1.3.9/hata/discord/embed/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    36833 2022-06-21 09:40:41.000000 hata-1.3.9/hata/discord/embed/embed.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    44944 2022-05-02 06:13:46.000000 hata-1.3.9/hata/discord/embed/embed_base.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    17615 2022-01-29 18:36:01.000000 hata-1.3.9/hata/discord/embed/embed_core.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.749734 hata-1.3.9/hata/discord/emoji/
+-rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)      633 2022-10-01 06:11:08.000000 hata-1.3.9/hata/discord/emoji/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    21835 2022-09-04 09:28:51.000000 hata-1.3.9/hata/discord/emoji/emoji.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     5836 2022-08-18 15:08:52.000000 hata-1.3.9/hata/discord/emoji/emoji_all_pattern.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     7479 2022-08-13 20:08:29.000000 hata-1.3.9/hata/discord/emoji/event_types.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    15397 2022-10-01 20:04:32.000000 hata-1.3.9/hata/discord/emoji/reaction_mapping.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    12515 2022-10-01 15:09:38.000000 hata-1.3.9/hata/discord/emoji/reaction_mapping_line.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3049 2022-09-20 17:27:47.000000 hata-1.3.9/hata/discord/emoji/unicode_type.py
+-rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)   590776 2022-09-20 18:10:21.000000 hata-1.3.9/hata/discord/emoji/unicodes.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    12844 2022-10-01 07:16:29.000000 hata-1.3.9/hata/discord/emoji/utils.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.753734 hata-1.3.9/hata/discord/events/
+-rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)      573 2021-10-12 09:16:26.000000 hata-1.3.9/hata/discord/events/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    23100 2022-08-13 12:58:20.000000 hata-1.3.9/hata/discord/events/core.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     6026 2022-07-30 12:32:57.000000 hata-1.3.9/hata/discord/events/default_event_handlers.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    78351 2022-09-29 17:05:20.000000 hata-1.3.9/hata/discord/events/event_handler_manager.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    14276 2022-01-29 18:36:01.000000 hata-1.3.9/hata/discord/events/event_handler_plugin.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    15180 2022-09-10 12:33:40.000000 hata-1.3.9/hata/discord/events/event_types.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     9429 2022-02-26 09:10:25.000000 hata-1.3.9/hata/discord/events/filters.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3982 2021-12-31 07:39:40.000000 hata-1.3.9/hata/discord/events/guild_sync.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    87153 2022-09-08 19:51:58.000000 hata-1.3.9/hata/discord/events/handling_helpers.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    23989 2022-06-23 14:56:18.000000 hata-1.3.9/hata/discord/events/intent.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)   133557 2022-09-18 10:50:22.000000 hata-1.3.9/hata/discord/events/parsers.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.753734 hata-1.3.9/hata/discord/exceptions/
+-rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)      395 2021-10-08 11:30:50.000000 hata-1.3.9/hata/discord/exceptions/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    17616 2022-09-04 09:28:51.000000 hata-1.3.9/hata/discord/exceptions/discord_exception.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2517 2022-03-21 15:50:31.000000 hata-1.3.9/hata/discord/exceptions/discord_gateway_exception.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    52202 2022-09-08 16:51:32.000000 hata-1.3.9/hata/discord/exceptions/error_codes.py
+-rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)      249 2021-10-08 11:30:50.000000 hata-1.3.9/hata/discord/exceptions/invalid_token.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    10786 2022-09-04 19:34:56.000000 hata-1.3.9/hata/discord/exceptions/payload_renderer.py
+-rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)      172 2021-10-08 11:30:50.000000 hata-1.3.9/hata/discord/exceptions/voice_error_codes.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.757734 hata-1.3.9/hata/discord/gateway/
+-rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)      245 2021-10-08 11:30:50.000000 hata-1.3.9/hata/discord/gateway/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    28356 2022-09-13 10:34:32.000000 hata-1.3.9/hata/discord/gateway/client_gateway.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    13765 2022-01-03 06:21:48.000000 hata-1.3.9/hata/discord/gateway/heartbeat.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4031 2022-01-01 14:48:03.000000 hata-1.3.9/hata/discord/gateway/rate_limit.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    14823 2022-02-07 13:26:01.000000 hata-1.3.9/hata/discord/gateway/voice_client_gateway.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.757734 hata-1.3.9/hata/discord/guild/
+-rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)      639 2021-12-19 21:12:03.000000 hata-1.3.9/hata/discord/guild/__init__.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.761734 hata-1.3.9/hata/discord/guild/audit_logs/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      570 2022-01-23 20:15:39.000000 hata-1.3.9/hata/discord/guild/audit_logs/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     7984 2022-09-18 10:50:22.000000 hata-1.3.9/hata/discord/guild/audit_logs/audit_log.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    19718 2022-09-17 11:24:36.000000 hata-1.3.9/hata/discord/guild/audit_logs/audit_log_change.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     6987 2022-07-02 19:19:40.000000 hata-1.3.9/hata/discord/guild/audit_logs/audit_log_entry.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     8217 2022-06-24 19:04:11.000000 hata-1.3.9/hata/discord/guild/audit_logs/audit_log_iterator.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1225 2022-01-22 18:30:13.000000 hata-1.3.9/hata/discord/guild/audit_logs/audit_log_role.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.765734 hata-1.3.9/hata/discord/guild/audit_logs/change_converters/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      816 2022-06-24 19:34:04.000000 hata-1.3.9/hata/discord/guild/audit_logs/change_converters/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2075 2022-06-25 07:26:50.000000 hata-1.3.9/hata/discord/guild/audit_logs/change_converters/all_.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      253 2022-05-02 14:45:16.000000 hata-1.3.9/hata/discord/guild/audit_logs/change_converters/application_command.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2662 2022-09-17 11:24:36.000000 hata-1.3.9/hata/discord/guild/audit_logs/change_converters/auto_moderation_rule.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4505 2022-09-13 13:40:27.000000 hata-1.3.9/hata/discord/guild/audit_logs/change_converters/channel.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      924 2022-01-23 20:07:49.000000 hata-1.3.9/hata/discord/guild/audit_logs/change_converters/channel_permission_overwrite.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      204 2022-01-23 20:07:49.000000 hata-1.3.9/hata/discord/guild/audit_logs/change_converters/emoji.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3133 2022-03-30 04:08:08.000000 hata-1.3.9/hata/discord/guild/audit_logs/change_converters/guild.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      206 2022-01-23 20:07:49.000000 hata-1.3.9/hata/discord/guild/audit_logs/change_converters/integration.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      326 2022-01-23 20:07:49.000000 hata-1.3.9/hata/discord/guild/audit_logs/change_converters/invite.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1157 2022-01-23 20:07:49.000000 hata-1.3.9/hata/discord/guild/audit_logs/change_converters/role.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2250 2022-09-17 11:24:36.000000 hata-1.3.9/hata/discord/guild/audit_logs/change_converters/scheduled_event.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2908 2022-06-24 19:21:30.000000 hata-1.3.9/hata/discord/guild/audit_logs/change_converters/shared.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      229 2022-01-23 20:07:49.000000 hata-1.3.9/hata/discord/guild/audit_logs/change_converters/stage.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1150 2022-01-25 20:26:40.000000 hata-1.3.9/hata/discord/guild/audit_logs/change_converters/sticker.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      877 2022-01-23 20:07:49.000000 hata-1.3.9/hata/discord/guild/audit_logs/change_converters/user.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      473 2022-01-25 20:33:06.000000 hata-1.3.9/hata/discord/guild/audit_logs/change_converters/webhook.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1894 2022-07-23 11:10:05.000000 hata-1.3.9/hata/discord/guild/audit_logs/detail_converters.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    33486 2022-07-09 16:06:54.000000 hata-1.3.9/hata/discord/guild/audit_logs/preinstanced.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3343 2022-06-24 19:34:04.000000 hata-1.3.9/hata/discord/guild/audit_logs/target_converters.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    22501 2022-01-29 18:36:01.000000 hata-1.3.9/hata/discord/guild/discovery.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    13396 2022-09-10 12:30:03.000000 hata-1.3.9/hata/discord/guild/embedded_activity_state.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    10844 2022-02-22 18:03:52.000000 hata-1.3.9/hata/discord/guild/event_types.py
+-rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)     2737 2022-05-28 10:03:13.000000 hata-1.3.9/hata/discord/guild/flags.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)   105329 2022-09-18 10:50:22.000000 hata-1.3.9/hata/discord/guild/guild.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    45027 2022-09-08 16:24:18.000000 hata-1.3.9/hata/discord/guild/preinstanced.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     5521 2022-09-04 09:28:51.000000 hata-1.3.9/hata/discord/guild/preview.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2389 2022-01-03 06:21:48.000000 hata-1.3.9/hata/discord/guild/utils.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     9941 2022-02-14 09:44:43.000000 hata-1.3.9/hata/discord/guild/verification_screen.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    10089 2022-09-10 16:28:10.000000 hata-1.3.9/hata/discord/guild/welcome_screen.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     8377 2022-09-18 10:50:24.000000 hata-1.3.9/hata/discord/guild/widget.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.769734 hata-1.3.9/hata/discord/http/
+-rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)      409 2021-10-08 11:30:50.000000 hata-1.3.9/hata/discord/http/__init__.py
+-rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)      490 2022-01-01 14:53:39.000000 hata-1.3.9/hata/discord/http/headers.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    82534 2022-08-12 13:01:28.000000 hata-1.3.9/hata/discord/http/http_client.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    37398 2022-03-13 10:04:02.000000 hata-1.3.9/hata/discord/http/rate_limit.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    62840 2022-07-09 15:04:43.000000 hata-1.3.9/hata/discord/http/rate_limit_groups.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    16822 2022-03-28 16:04:08.000000 hata-1.3.9/hata/discord/http/rate_limit_proxy.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    52310 2022-09-08 16:05:56.000000 hata-1.3.9/hata/discord/http/urls.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.769734 hata-1.3.9/hata/discord/integration/
+-rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)      377 2021-10-08 11:30:50.000000 hata-1.3.9/hata/discord/integration/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4645 2022-08-28 11:14:25.000000 hata-1.3.9/hata/discord/integration/integration.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1747 2022-08-27 10:21:08.000000 hata-1.3.9/hata/discord/integration/integration_account.py
+-rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)     1566 2022-08-28 11:20:15.000000 hata-1.3.9/hata/discord/integration/integration_application.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3705 2022-08-28 11:45:38.000000 hata-1.3.9/hata/discord/integration/integration_detail.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3450 2022-08-27 11:50:28.000000 hata-1.3.9/hata/discord/integration/preinstanced.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1343 2022-01-29 18:36:01.000000 hata-1.3.9/hata/discord/integration/utils.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.769734 hata-1.3.9/hata/discord/interaction/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      474 2022-03-08 18:56:07.000000 hata-1.3.9/hata/discord/interaction/__init__.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.773734 hata-1.3.9/hata/discord/interaction/application_command/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      615 2022-03-13 07:29:07.000000 hata-1.3.9/hata/discord/interaction/application_command/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    49742 2022-09-09 16:44:27.000000 hata-1.3.9/hata/discord/interaction/application_command/application_command.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    48998 2022-09-20 19:08:40.000000 hata-1.3.9/hata/discord/interaction/application_command/application_command_option.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    11548 2022-09-04 11:12:06.000000 hata-1.3.9/hata/discord/interaction/application_command/application_command_option_choice.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    12027 2022-03-09 05:58:16.000000 hata-1.3.9/hata/discord/interaction/application_command/application_command_permission.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    17631 2022-06-22 06:26:56.000000 hata-1.3.9/hata/discord/interaction/application_command/application_command_permission_overwrite.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      993 2022-07-08 07:09:41.000000 hata-1.3.9/hata/discord/interaction/application_command/constants.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2312 2022-03-19 14:22:38.000000 hata-1.3.9/hata/discord/interaction/application_command/helpers.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     6930 2022-03-08 18:56:07.000000 hata-1.3.9/hata/discord/interaction/application_command/preinstanced.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.773734 hata-1.3.9/hata/discord/interaction/components/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      695 2022-01-11 10:30:08.000000 hata-1.3.9/hata/discord/interaction/components/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3554 2022-01-11 10:30:08.000000 hata-1.3.9/hata/discord/interaction/components/component_base.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    14224 2022-04-01 06:49:08.000000 hata-1.3.9/hata/discord/interaction/components/component_button.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     5841 2022-01-11 11:11:32.000000 hata-1.3.9/hata/discord/interaction/components/component_dynamic.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     6777 2022-06-25 10:46:39.000000 hata-1.3.9/hata/discord/interaction/components/component_row.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    15101 2022-01-29 18:36:01.000000 hata-1.3.9/hata/discord/interaction/components/component_select.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     9637 2022-02-16 21:39:18.000000 hata-1.3.9/hata/discord/interaction/components/component_select_option.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    17822 2022-02-16 21:36:54.000000 hata-1.3.9/hata/discord/interaction/components/component_text_input.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      513 2022-03-30 04:35:46.000000 hata-1.3.9/hata/discord/interaction/components/constants.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    15456 2022-02-09 06:14:38.000000 hata-1.3.9/hata/discord/interaction/components/debug.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     9797 2022-01-29 18:36:01.000000 hata-1.3.9/hata/discord/interaction/components/form.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     6219 2022-04-01 06:51:12.000000 hata-1.3.9/hata/discord/interaction/components/preinstanced.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2049 2022-02-16 21:42:14.000000 hata-1.3.9/hata/discord/interaction/components/utils.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.777734 hata-1.3.9/hata/discord/interaction/event_types/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      572 2022-01-11 10:30:08.000000 hata-1.3.9/hata/discord/interaction/event_types/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    12859 2022-03-09 06:10:58.000000 hata-1.3.9/hata/discord/interaction/event_types/application_command_autocomplete_interaction.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    18259 2022-03-28 16:04:08.000000 hata-1.3.9/hata/discord/interaction/event_types/application_command_interaction.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3779 2022-03-30 17:03:25.000000 hata-1.3.9/hata/discord/interaction/event_types/component_interaction.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    12015 2022-02-09 06:49:19.000000 hata-1.3.9/hata/discord/interaction/event_types/form_submit_interaction.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    21908 2022-09-10 12:29:21.000000 hata-1.3.9/hata/discord/interaction/event_types/interaction_event.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1032 2022-01-11 10:30:08.000000 hata-1.3.9/hata/discord/interaction/event_types/interaction_field_base.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2534 2022-01-11 10:30:08.000000 hata-1.3.9/hata/discord/interaction/event_types/preinstanced.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     5570 2022-02-18 11:53:58.000000 hata-1.3.9/hata/discord/interaction/interaction_response_context.py
+-rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)     1885 2021-12-07 08:47:45.000000 hata-1.3.9/hata/discord/interaction/interaction_response_types.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.777734 hata-1.3.9/hata/discord/invite/
+-rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)      167 2021-10-08 11:30:50.000000 hata-1.3.9/hata/discord/invite/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    21773 2022-06-05 09:34:02.000000 hata-1.3.9/hata/discord/invite/invite.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1565 2022-02-22 19:02:04.000000 hata-1.3.9/hata/discord/invite/invite_stage.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2911 2022-01-18 14:47:29.000000 hata-1.3.9/hata/discord/invite/preinstanced.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.777734 hata-1.3.9/hata/discord/localizations/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      156 2022-03-12 09:12:10.000000 hata-1.3.9/hata/discord/localizations/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     7705 2022-08-21 17:04:24.000000 hata-1.3.9/hata/discord/localizations/helpers.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    11917 2022-03-30 17:03:25.000000 hata-1.3.9/hata/discord/localizations/preinstanced.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1773 2022-09-04 09:37:06.000000 hata-1.3.9/hata/discord/localizations/utils.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.781734 hata-1.3.9/hata/discord/message/
+-rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)      928 2022-08-13 20:21:13.000000 hata-1.3.9/hata/discord/message/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3826 2022-08-21 09:29:47.000000 hata-1.3.9/hata/discord/message/attachment.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     6007 2022-09-04 09:28:51.000000 hata-1.3.9/hata/discord/message/cross_mention.py
+-rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)     2304 2022-07-07 19:10:42.000000 hata-1.3.9/hata/discord/message/flags.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)   149162 2022-10-02 05:18:15.000000 hata-1.3.9/hata/discord/message/message.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1729 2022-01-01 15:01:19.000000 hata-1.3.9/hata/discord/message/message_activity.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2465 2022-01-01 15:01:36.000000 hata-1.3.9/hata/discord/message/message_application.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3712 2022-07-09 10:52:01.000000 hata-1.3.9/hata/discord/message/message_interaction.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    26128 2022-09-10 11:59:07.000000 hata-1.3.9/hata/discord/message/preinstanced.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3256 2022-03-29 16:37:14.000000 hata-1.3.9/hata/discord/message/utils.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.781734 hata-1.3.9/hata/discord/oauth2/
+-rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)      474 2022-08-27 13:45:12.000000 hata-1.3.9/hata/discord/oauth2/__init__.py
+-rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)     8184 2022-09-04 09:28:51.000000 hata-1.3.9/hata/discord/oauth2/achievement.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2570 2022-06-21 11:48:16.000000 hata-1.3.9/hata/discord/oauth2/connection.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3494 2022-08-28 11:05:03.000000 hata-1.3.9/hata/discord/oauth2/helpers.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4539 2022-08-29 18:18:22.000000 hata-1.3.9/hata/discord/oauth2/oauth2_access.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     8184 2022-08-27 13:51:43.000000 hata-1.3.9/hata/discord/oauth2/oauth2_user.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    14685 2022-09-10 17:15:24.000000 hata-1.3.9/hata/discord/oauth2/preinstanced.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    19549 2022-07-01 11:26:24.000000 hata-1.3.9/hata/discord/object_binding.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.785734 hata-1.3.9/hata/discord/permission/
+-rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)      232 2021-10-08 11:30:50.000000 hata-1.3.9/hata/discord/permission/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    21446 2022-07-29 14:28:34.000000 hata-1.3.9/hata/discord/permission/permission.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    13722 2022-09-14 06:51:25.000000 hata-1.3.9/hata/discord/permission/permission_overwrite.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3060 2022-01-01 15:04:25.000000 hata-1.3.9/hata/discord/permission/preinstanced.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2093 2022-01-01 15:04:47.000000 hata-1.3.9/hata/discord/permission/utils.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    18336 2022-09-11 11:14:33.000000 hata-1.3.9/hata/discord/preconverters.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.785734 hata-1.3.9/hata/discord/role/
+-rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)      150 2021-10-08 11:30:50.000000 hata-1.3.9/hata/discord/role/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2132 2022-01-01 15:04:59.000000 hata-1.3.9/hata/discord/role/preinstanced.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    27319 2022-09-04 09:28:51.000000 hata-1.3.9/hata/discord/role/role.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3729 2022-01-29 18:36:01.000000 hata-1.3.9/hata/discord/role/utils.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.785734 hata-1.3.9/hata/discord/scheduled_event/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      237 2022-09-17 11:24:36.000000 hata-1.3.9/hata/discord/scheduled_event/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2876 2022-01-01 15:05:53.000000 hata-1.3.9/hata/discord/scheduled_event/event_types.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.785734 hata-1.3.9/hata/discord/scheduled_event/metadata/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      183 2022-09-17 11:24:36.000000 hata-1.3.9/hata/discord/scheduled_event/metadata/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1486 2022-09-17 11:24:36.000000 hata-1.3.9/hata/discord/scheduled_event/metadata/base.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2214 2022-09-15 16:21:10.000000 hata-1.3.9/hata/discord/scheduled_event/metadata/location.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     5276 2022-09-17 11:24:36.000000 hata-1.3.9/hata/discord/scheduled_event/metadata/stage.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      701 2022-09-17 11:24:36.000000 hata-1.3.9/hata/discord/scheduled_event/metadata/utils.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     7043 2022-09-17 11:24:36.000000 hata-1.3.9/hata/discord/scheduled_event/preinstanced.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    16054 2022-09-17 11:24:36.000000 hata-1.3.9/hata/discord/scheduled_event/scheduled_event.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.785734 hata-1.3.9/hata/discord/stage/
+-rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)       56 2021-10-08 11:30:50.000000 hata-1.3.9/hata/discord/stage/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     5904 2022-09-10 12:34:35.000000 hata-1.3.9/hata/discord/stage/stage.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.785734 hata-1.3.9/hata/discord/sticker/
+-rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)      170 2021-10-08 11:30:50.000000 hata-1.3.9/hata/discord/sticker/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4799 2022-01-01 15:08:23.000000 hata-1.3.9/hata/discord/sticker/preinstanced.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    18590 2022-06-20 13:29:34.000000 hata-1.3.9/hata/discord/sticker/sticker.py
+-rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)     2986 2022-01-01 15:08:48.000000 hata-1.3.9/hata/discord/sticker/sticker_pack.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.789734 hata-1.3.9/hata/discord/user/
+-rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)      579 2021-10-08 11:30:50.000000 hata-1.3.9/hata/discord/user/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     6900 2022-09-10 12:14:09.000000 hata-1.3.9/hata/discord/user/activity_change.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    26891 2022-09-13 19:32:36.000000 hata-1.3.9/hata/discord/user/client_user_base.py
+-rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)     5530 2022-09-18 13:19:53.000000 hata-1.3.9/hata/discord/user/flags.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     9283 2022-01-29 18:36:01.000000 hata-1.3.9/hata/discord/user/guild_profile.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      464 2021-12-31 07:39:40.000000 hata-1.3.9/hata/discord/user/helpers.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    20668 2022-01-22 15:49:29.000000 hata-1.3.9/hata/discord/user/preinstanced.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     7586 2022-06-21 09:21:00.000000 hata-1.3.9/hata/discord/user/thread_profile.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    21060 2022-09-05 06:49:03.000000 hata-1.3.9/hata/discord/user/user.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    23150 2022-09-05 06:49:03.000000 hata-1.3.9/hata/discord/user/user_base.py
+-rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)      673 2022-07-09 10:55:07.000000 hata-1.3.9/hata/discord/user/utils.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    10337 2022-09-10 12:27:33.000000 hata-1.3.9/hata/discord/user/voice_state.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    55293 2022-09-06 16:34:02.000000 hata-1.3.9/hata/discord/utils.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.793734 hata-1.3.9/hata/discord/voice/
+-rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)      342 2021-10-14 06:02:06.000000 hata-1.3.9/hata/discord/voice/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    15612 2022-01-29 18:36:01.000000 hata-1.3.9/hata/discord/voice/audio_source.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    15456 2022-02-22 11:10:46.000000 hata-1.3.9/hata/discord/voice/opus.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     8497 2022-07-30 12:34:23.000000 hata-1.3.9/hata/discord/voice/player.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    10241 2022-07-30 13:45:52.000000 hata-1.3.9/hata/discord/voice/reader.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    11434 2022-01-03 06:21:48.000000 hata-1.3.9/hata/discord/voice/rtp_packet.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      570 2022-02-17 18:36:16.000000 hata-1.3.9/hata/discord/voice/utils.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    45620 2022-09-10 12:27:19.000000 hata-1.3.9/hata/discord/voice/voice_client.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.793734 hata-1.3.9/hata/discord/webhook/
+-rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)      266 2021-10-08 11:30:50.000000 hata-1.3.9/hata/discord/webhook/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1586 2022-01-01 15:14:37.000000 hata-1.3.9/hata/discord/webhook/preinstanced.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1179 2022-01-29 18:36:01.000000 hata-1.3.9/hata/discord/webhook/utils.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    13167 2022-03-29 17:19:38.000000 hata-1.3.9/hata/discord/webhook/webhook.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3245 2022-09-10 12:26:03.000000 hata-1.3.9/hata/discord/webhook/webhook_base.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2296 2022-01-01 15:16:28.000000 hata-1.3.9/hata/discord/webhook/webhook_repr.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4787 2022-09-10 12:25:11.000000 hata-1.3.9/hata/discord/webhook/webhook_sources.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     7386 2022-09-11 18:16:21.000000 hata-1.3.9/hata/env.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.793734 hata-1.3.9/hata/ext/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    11631 2022-07-22 10:48:20.000000 hata-1.3.9/hata/ext/__init__.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.793734 hata-1.3.9/hata/ext/asyncio/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      114 2022-02-09 06:14:08.000000 hata-1.3.9/hata/ext/asyncio/__init__.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.797734 hata-1.3.9/hata/ext/command_utils/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3289 2022-01-01 15:20:05.000000 hata-1.3.9/hata/ext/command_utils/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     9827 2022-03-29 16:37:14.000000 hata-1.3.9/hata/ext/command_utils/bases.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    27542 2022-08-13 12:58:20.000000 hata-1.3.9/hata/ext/command_utils/choose_menu.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    10907 2022-08-13 12:58:20.000000 hata-1.3.9/hata/ext/command_utils/closer.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    27070 2022-03-28 16:09:00.000000 hata-1.3.9/hata/ext/command_utils/io.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    17045 2022-08-13 12:58:20.000000 hata-1.3.9/hata/ext/command_utils/pagination.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    33237 2022-08-13 12:54:24.000000 hata-1.3.9/hata/ext/command_utils/user_menu.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4721 2022-01-01 15:23:52.000000 hata-1.3.9/hata/ext/command_utils/utils.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     8318 2022-03-28 16:04:08.000000 hata-1.3.9/hata/ext/command_utils/waiters.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.801734 hata-1.3.9/hata/ext/commands_v2/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4154 2022-05-29 07:45:33.000000 hata-1.3.9/hata/ext/commands_v2/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    14211 2022-04-11 07:14:10.000000 hata-1.3.9/hata/ext/commands_v2/category.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    66402 2022-08-13 12:53:14.000000 hata-1.3.9/hata/ext/commands_v2/checks.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1782 2022-04-10 06:35:31.000000 hata-1.3.9/hata/ext/commands_v2/client_wrapper_extension.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    60780 2022-04-23 10:51:03.000000 hata-1.3.9/hata/ext/commands_v2/command.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    27582 2022-08-13 12:58:20.000000 hata-1.3.9/hata/ext/commands_v2/command_helpers.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    38215 2022-04-05 17:19:46.000000 hata-1.3.9/hata/ext/commands_v2/command_processor.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)   120687 2022-09-10 16:51:11.000000 hata-1.3.9/hata/ext/commands_v2/content_parser.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    15017 2022-07-01 11:26:24.000000 hata-1.3.9/hata/ext/commands_v2/context.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     8997 2022-09-24 08:33:58.000000 hata-1.3.9/hata/ext/commands_v2/cooldown.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2497 2021-12-31 07:39:40.000000 hata-1.3.9/hata/ext/commands_v2/exceptions.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1859 2022-01-01 15:34:50.000000 hata-1.3.9/hata/ext/commands_v2/extension_hook_command_utils.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.801734 hata-1.3.9/hata/ext/commands_v2/helps/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    35121 2022-09-20 13:44:47.000000 hata-1.3.9/hata/ext/commands_v2/helps/subterranean.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4922 2022-07-23 15:19:52.000000 hata-1.3.9/hata/ext/commands_v2/responding.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     5715 2022-05-29 07:45:33.000000 hata-1.3.9/hata/ext/commands_v2/snapshot.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1188 2021-12-31 07:39:40.000000 hata-1.3.9/hata/ext/commands_v2/utils.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    10142 2022-01-30 21:05:04.000000 hata-1.3.9/hata/ext/commands_v2/wrappers.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.801734 hata-1.3.9/hata/ext/extension_loader/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      644 2022-05-29 12:23:59.000000 hata-1.3.9/hata/ext/extension_loader/__init__.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.801734 hata-1.3.9/hata/ext/kokoro_sqlalchemy/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      204 2022-01-01 15:37:42.000000 hata-1.3.9/hata/ext/kokoro_sqlalchemy/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     8835 2022-01-03 06:21:48.000000 hata-1.3.9/hata/ext/kokoro_sqlalchemy/kokoro_sqlalchemy.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.805734 hata-1.3.9/hata/ext/patchouli/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      604 2022-01-01 15:44:54.000000 hata-1.3.9/hata/ext/patchouli/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    15872 2022-07-26 19:23:21.000000 hata-1.3.9/hata/ext/patchouli/builder_html.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    57153 2022-08-26 17:18:47.000000 hata-1.3.9/hata/ext/patchouli/builder_html_extended.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    64584 2022-01-30 21:05:04.000000 hata-1.3.9/hata/ext/patchouli/builder_text.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    25270 2022-08-26 12:27:00.000000 hata-1.3.9/hata/ext/patchouli/graver.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1709 2022-07-26 19:10:31.000000 hata-1.3.9/hata/ext/patchouli/highlight.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    33027 2022-08-26 12:46:41.000000 hata-1.3.9/hata/ext/patchouli/module_mapper.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    46381 2022-08-26 15:51:56.000000 hata-1.3.9/hata/ext/patchouli/parser.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     6215 2021-12-31 07:39:40.000000 hata-1.3.9/hata/ext/patchouli/qualpath.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.805734 hata-1.3.9/hata/ext/plugin_loader/
+-rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)     1282 2022-05-29 12:30:57.000000 hata-1.3.9/hata/ext/plugin_loader/__init__.py
+-rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)     1332 2022-05-29 11:35:41.000000 hata-1.3.9/hata/ext/plugin_loader/client_extension.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      545 2022-05-29 11:28:11.000000 hata-1.3.9/hata/ext/plugin_loader/constants.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1845 2022-05-29 11:28:11.000000 hata-1.3.9/hata/ext/plugin_loader/exceptions.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    15934 2022-07-09 16:42:54.000000 hata-1.3.9/hata/ext/plugin_loader/helpers.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.805734 hata-1.3.9/hata/ext/plugin_loader/import_overwrite/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      463 2022-05-29 11:48:55.000000 hata-1.3.9/hata/ext/plugin_loader/import_overwrite/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3298 2022-09-25 13:36:04.000000 hata-1.3.9/hata/ext/plugin_loader/import_overwrite/module_proxy_type.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1965 2022-05-29 11:38:58.000000 hata-1.3.9/hata/ext/plugin_loader/import_overwrite/module_spec_type.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1495 2022-05-29 11:48:29.000000 hata-1.3.9/hata/ext/plugin_loader/import_overwrite/plugin_finder.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2700 2022-05-29 11:38:58.000000 hata-1.3.9/hata/ext/plugin_loader/import_overwrite/source_loader.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3939 2022-04-23 08:16:05.000000 hata-1.3.9/hata/ext/plugin_loader/import_overwrite/spec_finder_helpers.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      700 2022-05-29 11:40:53.000000 hata-1.3.9/hata/ext/plugin_loader/import_overwrite/tools.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1258 2022-05-29 11:40:53.000000 hata-1.3.9/hata/ext/plugin_loader/import_overwrite/utils.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    32862 2022-09-28 16:05:39.000000 hata-1.3.9/hata/ext/plugin_loader/plugin.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    61967 2022-09-28 16:18:54.000000 hata-1.3.9/hata/ext/plugin_loader/plugin_loader.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1917 2022-05-29 10:44:16.000000 hata-1.3.9/hata/ext/plugin_loader/plugin_root.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.809734 hata-1.3.9/hata/ext/plugin_loader/snapshot/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      249 2022-04-03 20:17:22.000000 hata-1.3.9/hata/ext/plugin_loader/snapshot/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3131 2022-05-29 11:37:52.000000 hata-1.3.9/hata/ext/plugin_loader/snapshot/base_snapshot_type.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    10685 2022-04-13 18:56:01.000000 hata-1.3.9/hata/ext/plugin_loader/snapshot/event_handler_snapshot.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3561 2022-04-05 16:52:24.000000 hata-1.3.9/hata/ext/plugin_loader/snapshot/helpers.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2912 2022-04-03 20:19:43.000000 hata-1.3.9/hata/ext/plugin_loader/snapshot/snapshot.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.813734 hata-1.3.9/hata/ext/plugin_loader/utils/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1094 2022-06-04 17:11:21.000000 hata-1.3.9/hata/ext/plugin_loader/utils/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      279 2022-06-04 17:08:57.000000 hata-1.3.9/hata/ext/plugin_loader/utils/add_default_plugin_variables_.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      263 2022-06-04 17:09:15.000000 hata-1.3.9/hata/ext/plugin_loader/utils/clear_default_plugin_variables_.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      205 2022-05-29 13:39:45.000000 hata-1.3.9/hata/ext/plugin_loader/utils/get_plugin_.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1275 2022-06-05 15:43:34.000000 hata-1.3.9/hata/ext/plugin_loader/utils/get_plugin_like_.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1343 2022-06-05 14:31:43.000000 hata-1.3.9/hata/ext/plugin_loader/utils/get_plugins_like_.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     5202 2022-09-25 13:35:52.000000 hata-1.3.9/hata/ext/plugin_loader/utils/import_plugin_.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      232 2022-06-04 18:13:51.000000 hata-1.3.9/hata/ext/plugin_loader/utils/load_all_plugin_.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      254 2022-06-04 18:17:06.000000 hata-1.3.9/hata/ext/plugin_loader/utils/load_plugin_.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      351 2022-05-29 13:04:44.000000 hata-1.3.9/hata/ext/plugin_loader/utils/register_and_load_plugin_.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      303 2022-06-02 05:34:36.000000 hata-1.3.9/hata/ext/plugin_loader/utils/register_plugin_.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      238 2022-06-04 18:13:51.000000 hata-1.3.9/hata/ext/plugin_loader/utils/reload_all_plugin_.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      262 2022-05-29 13:16:20.000000 hata-1.3.9/hata/ext/plugin_loader/utils/reload_plugin_.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      277 2022-06-04 17:08:21.000000 hata-1.3.9/hata/ext/plugin_loader/utils/remove_default_plugin_variables_.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1049 2022-05-29 11:37:28.000000 hata-1.3.9/hata/ext/plugin_loader/utils/require_.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      238 2022-06-04 18:13:51.000000 hata-1.3.9/hata/ext/plugin_loader/utils/unload_all_plugin_.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      262 2022-05-29 13:15:10.000000 hata-1.3.9/hata/ext/plugin_loader/utils/unload_plugin_.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.813734 hata-1.3.9/hata/ext/prettyprint/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      339 2022-03-30 16:48:40.000000 hata-1.3.9/hata/ext/prettyprint/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    64451 2022-09-29 17:05:20.000000 hata-1.3.9/hata/ext/prettyprint/prettyprint.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.817734 hata-1.3.9/hata/ext/slash/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4768 2022-05-29 07:45:33.000000 hata-1.3.9/hata/ext/slash/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1790 2022-05-21 09:00:27.000000 hata-1.3.9/hata/ext/slash/client_wrapper_extension.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.817734 hata-1.3.9/hata/ext/slash/command/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      543 2022-05-22 08:21:16.000000 hata-1.3.9/hata/ext/slash/command/__init__.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.817734 hata-1.3.9/hata/ext/slash/command/command_base/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)       59 2022-05-21 08:50:27.000000 hata-1.3.9/hata/ext/slash/command/command_base/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     8010 2022-09-03 16:28:58.000000 hata-1.3.9/hata/ext/slash/command/command_base/command_base.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.817734 hata-1.3.9/hata/ext/slash/command/command_base_application_command/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      204 2022-05-22 08:10:06.000000 hata-1.3.9/hata/ext/slash/command/command_base_application_command/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    24199 2022-09-03 16:52:05.000000 hata-1.3.9/hata/ext/slash/command/command_base_application_command/command_base_application_command.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      602 2022-05-21 11:33:16.000000 hata-1.3.9/hata/ext/slash/command/command_base_application_command/constants.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     8109 2022-09-03 17:55:57.000000 hata-1.3.9/hata/ext/slash/command/command_base_application_command/helpers.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.821734 hata-1.3.9/hata/ext/slash/command/command_base_custom_id/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      135 2022-05-21 08:50:27.000000 hata-1.3.9/hata/ext/slash/command/command_base_custom_id/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     8230 2022-05-22 12:40:02.000000 hata-1.3.9/hata/ext/slash/command/command_base_custom_id/command_base_custom_id.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     5250 2022-05-21 08:17:58.000000 hata-1.3.9/hata/ext/slash/command/command_base_custom_id/helpers.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.821734 hata-1.3.9/hata/ext/slash/command/component_command/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      129 2022-05-21 09:08:00.000000 hata-1.3.9/hata/ext/slash/command/component_command/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     8436 2022-05-22 14:02:34.000000 hata-1.3.9/hata/ext/slash/command/component_command/component_command.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)       82 2022-05-21 09:06:28.000000 hata-1.3.9/hata/ext/slash/command/component_command/constants.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.821734 hata-1.3.9/hata/ext/slash/command/context_command/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)       66 2022-05-22 08:57:34.000000 hata-1.3.9/hata/ext/slash/command/context_command/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    17262 2022-09-03 16:48:22.000000 hata-1.3.9/hata/ext/slash/command/context_command/context_command.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.821734 hata-1.3.9/hata/ext/slash/command/form_submit_command/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      133 2022-05-21 09:09:22.000000 hata-1.3.9/hata/ext/slash/command/form_submit_command/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      102 2022-05-21 09:10:29.000000 hata-1.3.9/hata/ext/slash/command/form_submit_command/constants.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    11198 2022-05-22 14:02:34.000000 hata-1.3.9/hata/ext/slash/command/form_submit_command/form_submit_command.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2432 2022-05-22 08:23:25.000000 hata-1.3.9/hata/ext/slash/command/helpers.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.821734 hata-1.3.9/hata/ext/slash/command/slash_command/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      374 2022-05-22 08:10:06.000000 hata-1.3.9/hata/ext/slash/command/slash_command/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     6527 2022-05-22 08:58:01.000000 hata-1.3.9/hata/ext/slash/command/slash_command/helpers.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    34252 2022-09-03 16:53:33.000000 hata-1.3.9/hata/ext/slash/command/slash_command/slash_command.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    21492 2022-09-03 16:21:15.000000 hata-1.3.9/hata/ext/slash/command/slash_command/slash_command_category.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    20475 2022-09-03 16:15:30.000000 hata-1.3.9/hata/ext/slash/command/slash_command/slash_command_function.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    12765 2022-05-22 12:40:02.000000 hata-1.3.9/hata/ext/slash/command/slash_command/slash_command_parameter_auto_completer.py
+-rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)     1464 2022-02-22 11:48:23.000000 hata-1.3.9/hata/ext/slash/components.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)   121565 2022-09-20 19:10:44.000000 hata-1.3.9/hata/ext/slash/converters.py
+-rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)     3097 2022-01-01 16:00:19.000000 hata-1.3.9/hata/ext/slash/event_handlers.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    18385 2022-05-21 09:00:27.000000 hata-1.3.9/hata/ext/slash/exceptions.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    87061 2022-09-04 19:34:56.000000 hata-1.3.9/hata/ext/slash/expression_parser.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     5408 2022-03-13 15:01:47.000000 hata-1.3.9/hata/ext/slash/helpers.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.825734 hata-1.3.9/hata/ext/slash/menus/
+-rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)      193 2021-10-08 11:30:50.000000 hata-1.3.9/hata/ext/slash/menus/__init__.py
+-rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)     1142 2022-01-01 15:56:30.000000 hata-1.3.9/hata/ext/slash/menus/closer.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2693 2022-01-01 15:56:52.000000 hata-1.3.9/hata/ext/slash/menus/helpers.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    71347 2022-03-29 17:25:36.000000 hata-1.3.9/hata/ext/slash/menus/menu.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3056 2022-01-01 15:57:28.000000 hata-1.3.9/hata/ext/slash/menus/pagination.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    12486 2022-05-26 16:47:21.000000 hata-1.3.9/hata/ext/slash/permission_mismatch.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    28854 2022-07-23 15:19:52.000000 hata-1.3.9/hata/ext/slash/responding.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    12231 2022-05-22 07:41:34.000000 hata-1.3.9/hata/ext/slash/response_modifier.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)   138703 2022-09-03 17:46:13.000000 hata-1.3.9/hata/ext/slash/slasher.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    30311 2022-06-10 12:17:10.000000 hata-1.3.9/hata/ext/slash/snapshot.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4287 2022-05-21 09:00:27.000000 hata-1.3.9/hata/ext/slash/utils.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    20071 2022-01-30 21:05:04.000000 hata-1.3.9/hata/ext/slash/waiters.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    18356 2022-07-09 07:05:28.000000 hata-1.3.9/hata/ext/slash/wrappers.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.829734 hata-1.3.9/hata/ext/solarlink/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2828 2022-01-07 06:45:14.000000 hata-1.3.9/hata/ext/solarlink/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    20857 2022-06-24 15:31:16.000000 hata-1.3.9/hata/ext/solarlink/client.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     6341 2022-04-13 15:19:18.000000 hata-1.3.9/hata/ext/solarlink/constants.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3277 2022-04-12 18:06:32.000000 hata-1.3.9/hata/ext/solarlink/event_handler_plugin.py
+-rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)     5189 2022-07-22 10:31:27.000000 hata-1.3.9/hata/ext/solarlink/event_handlers.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    14885 2022-04-12 17:03:54.000000 hata-1.3.9/hata/ext/solarlink/event_types.py
+-rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)      797 2021-10-17 07:01:34.000000 hata-1.3.9/hata/ext/solarlink/exceptions.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    46416 2022-08-26 17:19:05.000000 hata-1.3.9/hata/ext/solarlink/filters.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    17384 2022-07-30 13:47:28.000000 hata-1.3.9/hata/ext/solarlink/node.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2469 2022-01-07 06:45:14.000000 hata-1.3.9/hata/ext/solarlink/parsers.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    17593 2022-01-30 21:05:04.000000 hata-1.3.9/hata/ext/solarlink/player.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    16714 2022-09-10 12:24:18.000000 hata-1.3.9/hata/ext/solarlink/player_base.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    10534 2022-04-12 16:01:31.000000 hata-1.3.9/hata/ext/solarlink/route_planner.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     6836 2022-04-12 16:01:31.000000 hata-1.3.9/hata/ext/solarlink/stats.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    22928 2022-04-12 17:18:47.000000 hata-1.3.9/hata/ext/solarlink/track.py
+-rw-r--r--   0 huyanematsu  (1000) huyanematsu  (1000)      126 2021-10-13 10:24:10.000000 hata-1.3.9/hata/ext/solarlink/track_end_reasons.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.829734 hata-1.3.9/hata/ext/top_gg/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2538 2021-12-31 07:39:40.000000 hata-1.3.9/hata/ext/top_gg/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     9987 2022-01-01 16:13:06.000000 hata-1.3.9/hata/ext/top_gg/bots_query.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    29423 2022-02-08 13:40:47.000000 hata-1.3.9/hata/ext/top_gg/client.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3042 2021-11-17 13:40:43.000000 hata-1.3.9/hata/ext/top_gg/constants.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2217 2022-01-01 16:15:52.000000 hata-1.3.9/hata/ext/top_gg/exceptions.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     7235 2022-02-14 09:47:14.000000 hata-1.3.9/hata/ext/top_gg/rate_limit_handling.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    21055 2022-01-03 06:21:48.000000 hata-1.3.9/hata/ext/top_gg/types.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.829734 hata-1.3.9/hata/main/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)       54 2022-07-13 16:54:39.000000 hata-1.3.9/hata/main/__init__.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.709734 hata-1.3.9/hata/main/commands/
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.829734 hata-1.3.9/hata/main/commands/default/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      103 2022-07-22 10:15:41.000000 hata-1.3.9/hata/main/commands/default/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2676 2022-07-20 14:41:30.000000 hata-1.3.9/hata/main/commands/default/help.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      723 2022-08-08 20:32:18.000000 hata-1.3.9/hata/main/commands/default/interpreter.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     8789 2022-07-22 11:39:24.000000 hata-1.3.9/hata/main/commands/default/run.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1422 2022-07-13 18:52:36.000000 hata-1.3.9/hata/main/commands/default/version.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.833734 hata-1.3.9/hata/main/core/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      345 2022-07-20 16:38:31.000000 hata-1.3.9/hata/main/core/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1997 2022-07-22 10:28:29.000000 hata-1.3.9/hata/main/core/call.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.833734 hata-1.3.9/hata/main/core/command/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      549 2022-07-16 08:18:34.000000 hata-1.3.9/hata/main/core/command/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    14229 2022-07-16 13:23:41.000000 hata-1.3.9/hata/main/core/command/category.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     8260 2022-07-18 17:24:18.000000 hata-1.3.9/hata/main/core/command/command.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    17685 2022-07-18 11:50:58.000000 hata-1.3.9/hata/main/core/command/function.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4806 2022-07-16 09:44:12.000000 hata-1.3.9/hata/main/core/command/helpers.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     7121 2022-07-16 12:58:19.000000 hata-1.3.9/hata/main/core/command/parameter.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    13820 2022-07-16 08:28:10.000000 hata-1.3.9/hata/main/core/command/parameter_renderer.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     8140 2022-07-16 08:45:29.000000 hata-1.3.9/hata/main/core/command/parameter_result.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1276 2022-07-16 12:03:37.000000 hata-1.3.9/hata/main/core/command/render_constants.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4699 2022-07-20 14:43:13.000000 hata-1.3.9/hata/main/core/command/rendering_helpers.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    13708 2022-07-20 14:44:44.000000 hata-1.3.9/hata/main/core/command/result.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      654 2022-07-19 13:26:33.000000 hata-1.3.9/hata/main/core/constants.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2980 2022-07-19 14:08:50.000000 hata-1.3.9/hata/main/core/external.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1835 2022-07-20 16:37:40.000000 hata-1.3.9/hata/main/core/helpers.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3443 2022-07-22 10:11:07.000000 hata-1.3.9/hata/main/core/lookup.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2420 2022-07-16 13:32:32.000000 hata-1.3.9/hata/main/core/registration.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.837734 hata-1.3.9/hata/utils/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      123 2022-03-27 19:55:08.000000 hata-1.3.9/hata/utils/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1447 2022-03-27 17:16:16.000000 hata-1.3.9/hata/utils/debug.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2848 2022-09-05 06:54:56.000000 hata-1.3.9/hata/utils/module_deprecation.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-10-03 12:28:55.709734 hata-1.3.9/hata.egg-info/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     8427 2022-10-03 12:28:55.000000 hata-1.3.9/hata.egg-info/PKG-INFO
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    21767 2022-10-03 12:28:55.000000 hata-1.3.9/hata.egg-info/SOURCES.txt
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)        1 2022-10-03 12:28:55.000000 hata-1.3.9/hata.egg-info/dependency_links.txt
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)       49 2022-10-03 12:28:55.000000 hata-1.3.9/hata.egg-info/entry_points.txt
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      125 2022-10-03 12:28:55.000000 hata-1.3.9/hata.egg-info/requires.txt
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)        5 2022-10-03 12:28:55.000000 hata-1.3.9/hata.egg-info/top_level.txt
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)       38 2022-10-03 12:28:55.837734 hata-1.3.9/setup.cfg
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     5166 2022-10-03 11:14:10.000000 hata-1.3.9/setup.py
```

### Comparing `hata-1.3.8/PKG-INFO` & `hata-1.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hata
-Version: 1.3.8
+Version: 1.3.9
 Summary: A powerful asynchronous library for creating Discord bots in Python.
 Home-page: https://github.com/HuyaneMatsu/hata
 Author: HuyaneMatsu
 Author-email: re.ism.tm@gmail.com
 License: DBAD
 Description: <h1 align="center">
             <b>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hata Version: 1.3.8 Summary: A powerful
+Metadata-Version: 2.1 Name: hata Version: 1.3.9 Summary: A powerful
 asynchronous library for creating Discord bots in Python. Home-page: https://
 github.com/HuyaneMatsu/hata Author: HuyaneMatsu Author-email:
 re.ism.tm@gmail.com License: DBAD Description:
                               ****** Hata ******
             A blazing fast Discord API wrapper that you can't deny
  Support_Guild | Topical_documentation | Examples | Technical_documentation |
                                     Source
```

### Comparing `hata-1.3.8/README.md` & `hata-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/__init__.py` & `hata-1.3.9/hata/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 
 Sometimes leaving the main thread might cause problems when trying to shut down the bot(s). At this case, you might
 want to use `wait_for_interruption()`, which disconnects the clients gracefully and closes the event loop on keyboard
 interrupt.
 
 We got some tutorials on `github:https://github.com/HuyaneMatsu/hata/tree/master/docs` as well, please check them too!
 """
-__version__ = '1.3.8'
+__version__ = '1.3.9'
 
 from .utils.module_deprecation import get_deprecation_function
 
 from .discord import *
 from .ext import *
 from .utils import *
```

### Comparing `hata-1.3.8/hata/__main__.py` & `hata-1.3.9/hata/__main__.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/backend/__init__.py` & `hata-1.3.9/hata/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/__init__.py` & `hata-1.3.9/hata/discord/__init__.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/activity/__init__.py` & `hata-1.3.9/hata/discord/activity/__init__.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/activity/activity.py` & `hata-1.3.9/hata/discord/activity/activity.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/activity/fields/assets.py` & `hata-1.3.9/hata/discord/activity/fields/assets.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/activity/fields/base.py` & `hata-1.3.9/hata/discord/activity/fields/base.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/activity/fields/party.py` & `hata-1.3.9/hata/discord/activity/fields/party.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/activity/fields/secrets.py` & `hata-1.3.9/hata/discord/activity/fields/secrets.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/activity/fields/timestamps.py` & `hata-1.3.9/hata/discord/activity/fields/timestamps.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/activity/flags.py` & `hata-1.3.9/hata/discord/activity/flags.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/activity/metadata/base.py` & `hata-1.3.9/hata/discord/activity/metadata/base.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/activity/metadata/custom.py` & `hata-1.3.9/hata/discord/activity/metadata/custom.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/activity/metadata/rich.py` & `hata-1.3.9/hata/discord/activity/metadata/rich.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/activity/preinstanced.py` & `hata-1.3.9/hata/discord/activity/preinstanced.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/allowed_mentions.py` & `hata-1.3.9/hata/discord/allowed_mentions.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/ansi_format.py` & `hata-1.3.9/hata/discord/ansi_format.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/application/application.py` & `hata-1.3.9/hata/discord/application/application.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/application/embedded_activity_configuration.py` & `hata-1.3.9/hata/discord/application/embedded_activity_configuration.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/application/flags.py` & `hata-1.3.9/hata/discord/application/flags.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/application/miscellaneous.py` & `hata-1.3.9/hata/discord/application/miscellaneous.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/application/preinstanced.py` & `hata-1.3.9/hata/discord/application/preinstanced.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/application/team.py` & `hata-1.3.9/hata/discord/application/team.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/auto_moderation/action.py` & `hata-1.3.9/hata/discord/auto_moderation/action.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/auto_moderation/action_metadata/alert_message.py` & `hata-1.3.9/hata/discord/auto_moderation/action_metadata/alert_message.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/auto_moderation/action_metadata/base.py` & `hata-1.3.9/hata/discord/auto_moderation/action_metadata/base.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/auto_moderation/action_metadata/timeout.py` & `hata-1.3.9/hata/discord/auto_moderation/action_metadata/timeout.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/auto_moderation/event_types.py` & `hata-1.3.9/hata/discord/auto_moderation/event_types.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/auto_moderation/preinstanced.py` & `hata-1.3.9/hata/discord/auto_moderation/preinstanced.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/auto_moderation/rule.py` & `hata-1.3.9/hata/discord/auto_moderation/rule.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/auto_moderation/trigger_metadata/base.py` & `hata-1.3.9/hata/discord/auto_moderation/trigger_metadata/base.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/auto_moderation/trigger_metadata/keyword.py` & `hata-1.3.9/hata/discord/auto_moderation/trigger_metadata/keyword.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/auto_moderation/trigger_metadata/keyword_preset.py` & `hata-1.3.9/hata/discord/auto_moderation/trigger_metadata/keyword_preset.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/auto_moderation/trigger_metadata/mention_spam.py` & `hata-1.3.9/hata/discord/auto_moderation/trigger_metadata/mention_spam.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/auto_moderation/trigger_metadata/utils.py` & `hata-1.3.9/hata/discord/auto_moderation/trigger_metadata/utils.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/bases/entity.py` & `hata-1.3.9/hata/discord/bases/entity.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/bases/event_types.py` & `hata-1.3.9/hata/discord/bases/event_types.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/bases/flags.py` & `hata-1.3.9/hata/discord/bases/flags.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/bases/icon.py` & `hata-1.3.9/hata/discord/bases/icon.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/bases/place_holder.py` & `hata-1.3.9/hata/discord/bases/place_holder.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/bases/preinstanced.py` & `hata-1.3.9/hata/discord/bases/preinstanced.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/bases/utils.py` & `hata-1.3.9/hata/discord/bases/utils.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/channel/__init__.py` & `hata-1.3.9/hata/discord/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/channel/channel.py` & `hata-1.3.9/hata/discord/channel/channel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1260,14 +1260,60 @@
         applied_tag_ids = self.applied_tag_ids
         if (applied_tag_ids is None):
             return None
         
         return tuple(create_forum_tag_from_id(forum_tag_id) for forum_tag_id in applied_tag_ids)
     
     
+    def iter_applied_tag_ids(self):
+        """
+        Iterates over the applied tag identifiers of the channel.
+        
+        This method is an iterable generator.
+        
+        Yields
+        ------
+        applied_tag_id : `int`
+        """
+        applied_tag_ids = self.applied_tag_ids
+        if (applied_tag_ids is not None):
+            yield from applied_tag_ids
+    
+    
+    def iter_applied_tags(self):
+        """
+        Iterates over the applied tags of the channels.
+        
+        This method is an iterable generator.
+        
+        Yields
+        ------
+        applied_tag : ``ForumTag``
+        """
+        applied_tag_ids = self.applied_tag_ids
+        if (applied_tag_ids is not None):
+            for forum_tag_id in applied_tag_ids:
+                yield create_forum_tag_from_id(forum_tag_id)
+    
+    
+    def iter_available_tags(self):
+        """
+        Iterates over the available tags of the the forum channel.
+        
+        This method is an iterable generator.
+        
+        Yields
+        ------
+        available_tag : ``ForumTag``
+        """
+        available_tags = self.available_tags
+        if (available_tags is not None):
+            yield from available_tags
+    
+    
     @property
     def owner(self):
         """
         Returns the group channel's owner.
         
         Returns
         -------
```

### Comparing `hata-1.3.8/hata/discord/channel/channel_type/flags.py` & `hata-1.3.9/hata/discord/channel/channel_type/flags.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/channel/channel_type/preinstanced.py` & `hata-1.3.9/hata/discord/channel/channel_type/preinstanced.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/channel/deprecation.py` & `hata-1.3.9/hata/discord/channel/deprecation.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/channel/fields/__init__.py` & `hata-1.3.9/hata/discord/channel/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/channel/fields/applied_tag_ids.py` & `hata-1.3.9/hata/discord/channel/fields/applied_tag_ids.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/channel/fields/archived.py` & `hata-1.3.9/hata/discord/channel/fields/archived.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/channel/fields/archived_at.py` & `hata-1.3.9/hata/discord/channel/fields/archived_at.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/channel/fields/auto_archive_after.py` & `hata-1.3.9/hata/discord/channel/fields/auto_archive_after.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/channel/fields/available_tags.py` & `hata-1.3.9/hata/discord/channel/fields/available_tags.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/channel/fields/bitrate.py` & `hata-1.3.9/hata/discord/channel/fields/bitrate.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/channel/fields/created_at.py` & `hata-1.3.9/hata/discord/channel/fields/created_at.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/channel/fields/default_thread_auto_archive_after.py` & `hata-1.3.9/hata/discord/channel/fields/default_thread_auto_archive_after.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/channel/fields/default_thread_reaction.py` & `hata-1.3.9/hata/discord/channel/fields/default_thread_reaction.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/channel/fields/default_thread_slowmode.py` & `hata-1.3.9/hata/discord/channel/fields/default_thread_slowmode.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/channel/fields/flags.py` & `hata-1.3.9/hata/discord/channel/fields/flags.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/channel/fields/invitable.py` & `hata-1.3.9/hata/discord/channel/fields/invitable.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/channel/fields/name.py` & `hata-1.3.9/hata/discord/channel/fields/name.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/channel/fields/nsfw.py` & `hata-1.3.9/hata/discord/channel/fields/nsfw.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/channel/fields/open_.py` & `hata-1.3.9/hata/discord/channel/fields/open_.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/channel/fields/owner_id.py` & `hata-1.3.9/hata/discord/channel/fields/owner_id.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/channel/fields/parent_id.py` & `hata-1.3.9/hata/discord/channel/fields/parent_id.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/channel/fields/permission_overwrites.py` & `hata-1.3.9/hata/discord/channel/fields/permission_overwrites.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/channel/fields/position.py` & `hata-1.3.9/hata/discord/channel/fields/position.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/channel/fields/region.py` & `hata-1.3.9/hata/discord/channel/fields/region.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/channel/fields/slowmode.py` & `hata-1.3.9/hata/discord/channel/fields/slowmode.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/channel/fields/topic.py` & `hata-1.3.9/hata/discord/channel/fields/topic.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/channel/fields/user_limit.py` & `hata-1.3.9/hata/discord/channel/fields/user_limit.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/channel/fields/users.py` & `hata-1.3.9/hata/discord/channel/fields/users.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/channel/fields/video_quality_mode.py` & `hata-1.3.9/hata/discord/channel/fields/video_quality_mode.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/channel/flags.py` & `hata-1.3.9/hata/discord/channel/flags.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/channel/forum_tag.py` & `hata-1.3.9/hata/discord/channel/forum_tag.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,15 +133,15 @@
             return id_
         
         return self._get_hash_partial()
     
     
     def _get_hash_partial(self):
         """
-        Hashes the fields of teh forum tag.
+        Hashes the fields of the forum tag.
         
         Returns
         -------
         hash_value : `int`
         """
         hash_value = 0
```

### Comparing `hata-1.3.8/hata/discord/channel/message_history.py` & `hata-1.3.9/hata/discord/channel/message_history.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/channel/message_iterator.py` & `hata-1.3.9/hata/discord/channel/message_iterator.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/channel/metadata/__init__.py` & `hata-1.3.9/hata/discord/channel/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/channel/metadata/base.py` & `hata-1.3.9/hata/discord/channel/metadata/base.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/channel/metadata/guild_announcements.py` & `hata-1.3.9/hata/discord/channel/metadata/guild_announcements.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/channel/metadata/guild_base.py` & `hata-1.3.9/hata/discord/channel/metadata/guild_base.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/channel/metadata/guild_category.py` & `hata-1.3.9/hata/discord/channel/metadata/guild_category.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/channel/metadata/guild_directory.py` & `hata-1.3.9/hata/discord/channel/metadata/guild_directory.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/channel/metadata/guild_forum.py` & `hata-1.3.9/hata/discord/channel/metadata/guild_forum.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/channel/metadata/guild_main_base.py` & `hata-1.3.9/hata/discord/channel/metadata/guild_main_base.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/channel/metadata/guild_stage.py` & `hata-1.3.9/hata/discord/channel/metadata/guild_stage.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/channel/metadata/guild_store.py` & `hata-1.3.9/hata/discord/channel/metadata/guild_store.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/channel/metadata/guild_text.py` & `hata-1.3.9/hata/discord/channel/metadata/guild_text.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/channel/metadata/guild_text_base.py` & `hata-1.3.9/hata/discord/channel/metadata/guild_text_base.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/channel/metadata/guild_thread_announcements.py` & `hata-1.3.9/hata/discord/channel/metadata/guild_thread_announcements.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/channel/metadata/guild_thread_base.py` & `hata-1.3.9/hata/discord/channel/metadata/guild_thread_base.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/channel/metadata/guild_thread_private.py` & `hata-1.3.9/hata/discord/channel/metadata/guild_thread_private.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/channel/metadata/guild_thread_public.py` & `hata-1.3.9/hata/discord/channel/metadata/guild_thread_public.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/channel/metadata/guild_voice.py` & `hata-1.3.9/hata/discord/channel/metadata/guild_voice.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/channel/metadata/guild_voice_base.py` & `hata-1.3.9/hata/discord/channel/metadata/guild_voice_base.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/channel/metadata/private.py` & `hata-1.3.9/hata/discord/channel/metadata/private.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/channel/metadata/private_base.py` & `hata-1.3.9/hata/discord/channel/metadata/private_base.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/channel/metadata/private_group.py` & `hata-1.3.9/hata/discord/channel/metadata/private_group.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/channel/preinstanced.py` & `hata-1.3.9/hata/discord/channel/preinstanced.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/channel/utils.py` & `hata-1.3.9/hata/discord/channel/utils.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/client/client.py` & `hata-1.3.9/hata/discord/client/client.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/client/compounds/__init__.py` & `hata-1.3.9/hata/discord/client/compounds/__init__.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/client/compounds/achievement.py` & `hata-1.3.9/hata/discord/client/compounds/achievement.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/client/compounds/application_command.py` & `hata-1.3.9/hata/discord/client/compounds/application_command.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/client/compounds/auto_moderation.py` & `hata-1.3.9/hata/discord/client/compounds/auto_moderation.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/client/compounds/channel.py` & `hata-1.3.9/hata/discord/client/compounds/channel.py`

 * *Files 0% similar despite different names*

```diff
@@ -756,15 +756,15 @@
         
         if (name is not ...):
             channel_data['name'] = name
         
         if channel is None:
             channel_type = ChannelType.unknown
         else:
-            channel_type = channel.type_
+            channel_type = channel.type
         
         if (type_ is not ...):
             type_ = preconvert_preinstanced_type(type_, 'type_', ChannelType)
             assert _assert__channel_edit__type(type_, channel, channel_type)
         
         if (type_ is not ...):
             channel_data['type'] = type_
```

### Comparing `hata-1.3.8/hata/discord/client/compounds/client.py` & `hata-1.3.9/hata/discord/client/compounds/client.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/client/compounds/client_gayteway.py` & `hata-1.3.9/hata/discord/client/compounds/client_gayteway.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/client/compounds/discovery.py` & `hata-1.3.9/hata/discord/client/compounds/discovery.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/client/compounds/emoji.py` & `hata-1.3.9/hata/discord/client/compounds/emoji.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/client/compounds/guild.py` & `hata-1.3.9/hata/discord/client/compounds/guild.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/client/compounds/guild_ban.py` & `hata-1.3.9/hata/discord/client/compounds/guild_ban.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/client/compounds/integration.py` & `hata-1.3.9/hata/discord/client/compounds/integration.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/client/compounds/interaction.py` & `hata-1.3.9/hata/discord/client/compounds/interaction.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/client/compounds/invite.py` & `hata-1.3.9/hata/discord/client/compounds/invite.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/client/compounds/locked.py` & `hata-1.3.9/hata/discord/client/compounds/locked.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/client/compounds/message.py` & `hata-1.3.9/hata/discord/client/compounds/message.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/client/compounds/miscellaneous.py` & `hata-1.3.9/hata/discord/client/compounds/miscellaneous.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/client/compounds/oauth2.py` & `hata-1.3.9/hata/discord/client/compounds/oauth2.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/client/compounds/reaction.py` & `hata-1.3.9/hata/discord/client/compounds/reaction.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/client/compounds/role.py` & `hata-1.3.9/hata/discord/client/compounds/role.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/client/compounds/scheduled_event.py` & `hata-1.3.9/hata/discord/client/compounds/scheduled_event.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/client/compounds/stage.py` & `hata-1.3.9/hata/discord/client/compounds/stage.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/client/compounds/sticker.py` & `hata-1.3.9/hata/discord/client/compounds/sticker.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/client/compounds/thread.py` & `hata-1.3.9/hata/discord/client/compounds/thread.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/client/compounds/user.py` & `hata-1.3.9/hata/discord/client/compounds/user.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/client/compounds/webhook.py` & `hata-1.3.9/hata/discord/client/compounds/webhook.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/client/functionality_helpers.py` & `hata-1.3.9/hata/discord/client/functionality_helpers.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/client/ready_state.py` & `hata-1.3.9/hata/discord/client/ready_state.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/client/request_helpers.py` & `hata-1.3.9/hata/discord/client/request_helpers.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/client/utils.py` & `hata-1.3.9/hata/discord/client/utils.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/color.py` & `hata-1.3.9/hata/discord/color.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/core.py` & `hata-1.3.9/hata/discord/core.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/embed/embed.py` & `hata-1.3.9/hata/discord/embed/embed.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/embed/embed_base.py` & `hata-1.3.9/hata/discord/embed/embed_base.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/embed/embed_core.py` & `hata-1.3.9/hata/discord/embed/embed_core.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/emoji/emoji.py` & `hata-1.3.9/hata/discord/emoji/emoji.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/emoji/emoji_all_pattern.py` & `hata-1.3.9/hata/discord/emoji/emoji_all_pattern.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/emoji/event_types.py` & `hata-1.3.9/hata/discord/emoji/event_types.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/emoji/reaction.py` & `hata-1.3.9/hata/discord/emoji/reaction_mapping_line.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,249 +1,234 @@
-__all__ = ('reaction_mapping', 'reaction_mapping_line',)
-
-from scarletio import include, set_docs
-
-from .utils import create_partial_emoji_data, create_partial_emoji_from_data
+__all__ = ('ReactionMappingLine',)
 
+from scarletio import include
+from scarletio.utils.compact import NEEDS_DUMMY_INIT
 
 Client = include('Client')
+ClientUserBase = include('ClientUserBase')
 
 
-class reaction_mapping(dict):
+def _validate_reaction_mapping_line_initialise_with(reaction_mapping_line_type, initialize_with):
     """
-    A `dict` subclass, which contains the reactions on a ``Message`` with (``Emoji``, ``reaction_mapping_line``)
-    items.
+    Validates the `initialize_with` parameter of ``ReactionMappingLine``.
     
-    Attributes
+    Parameters
     ----------
-    fully_loaded : `bool`
-        Whether the reaction mapping line is fully loaded.
-    """
-    __slots__ = ('fully_loaded',)
+    reaction_mapping_line_type : `type`
+        The type of the reaction mapping line.
+    initialize_with : `None`, `iterable` of (`None`, ``ClientUserBase``), `instance<reaction_mapping_line_type>`
+        The value ot initialize the line with.
+    
+    Returns
+    -------
+    users : `None`, `list` of ``ClientUserBase``
+        The built users from the `initialize_with` parameter.
+    unknown : `int`
+        The amount of unknown users.
     
-    def __init__(self, data):
-        """
-        Fills the reaction mapping with the given data.
-        
-        Parameters
-        ----------
-        data : `None`, `dict` of (`str`, `Any`) items
-        """
-        if (data is None) or (not data):
-            self.fully_loaded = True
-            return
-        
-        self.fully_loaded = False
-        for line in data:
-            self[create_partial_emoji_from_data(line['emoji'])] = reaction_mapping_line(line.get('count', 1))
+    Raises
+    ------
+    TypeError
+        - If an element of `initialize_with` is not `None`, ``ClientUserBase``.
+    """
+    if initialize_with is None:
+        built_initialize_with = None, 0
     
-    emoji_count = set_docs(
-        property(dict.__len__),
-        """
-        The amount of different emojis, which were added on the reaction mapping's respective ``Message``.
-        
-        Returns
-        -------
-        emoji_count : `int`
-        """
-    )
+    elif type(initialize_with) is reaction_mapping_line_type:
+        built_initialize_with = _validate_reaction_mapping_line_initialise_with_same(initialize_with)
     
-    @property
-    def total_count(self):
-        """
-        The total amount reactions given on the reaction mapping's respective message.
-        
-        Returns
-        -------
-        total_count : `int`
-        """
-        count = 0
-        for line in self.values():
-            count += set.__len__(line)
-            count += line.unknown
-        return count
+    elif (getattr(initialize_with, '__iter__', None) is not None):
+        built_initialize_with = _validate_reaction_mapping_line_initialise_with_iterable(initialize_with)
     
+    else:
+        raise TypeError(
+            f'`initialize_with` can be `None`, `{reaction_mapping_line_type.__name__}`, '
+            f'`iterable` of (`{ClientUserBase.__name__}`, `None`), got '
+            f'{initialize_with.__class__.__name__}; {initialize_with!r}.'
+        )
     
-    def clear(self):
-        """
-        Clears the reaction mapping with clearing it's lines.
-        """
-        for value in self.values():
-            value.clear()
-        if self.fully_loaded:
-            self._full_check()
+    return built_initialize_with
+
+
+def _validate_reaction_mapping_line_initialise_with_same(initialize_with):
+    """
+    Validates the `initialize_with` parameter of ``ReactionMappingLine`` where it is the same type.
     
+    Parameters
+    ----------
+    initialize_with : ``ReactionMappingLine``
+        The value ot initialize the line with.
     
-    def add(self, emoji, user):
-        """
-        Adds a user to the reactors.
-        
-        Parameters
-        ----------
-        emoji : ``Emoji``
-            The reacted emoji.
-        user : ``ClientUserBase``
-            The reactor user.
-        """
-        try:
-            line = self[emoji]
-        except KeyError:
-            line = reaction_mapping_line(0)
-            self[emoji] = line
-        line.add(user)
+    Returns
+    -------
+    users : `None`, `list` of ``ClientUserBase``
+        The built users from the `initialize_with` parameter.
+    unknown : `int`
+        The amount of unknown users.
+    """
+    if set.__len__(initialize_with) == 0:
+        users = None
+    else:
+        users = [*set.__iter__(initialize_with)]
     
+    unknown = initialize_with.unknown
     
-    def remove(self, emoji, user):
-        """
-        Removes a user to the reactors.
-        
-        Parameters
-        ----------
-        emoji : ``Emoji``
-            The removed reacted emoji.
-        user : ``ClientUserBase``
-            The removed reactor user.
-        """
-        try:
-            line = self[emoji]
-        except KeyError:
-            return
+    return users, unknown
 
-        if set.__len__(line):
-            try:
-                line.remove(user)
-            except KeyError:
-                pass
-            else:
-                if set.__len__(line) or line.unknown:
-                    return
-                del self[emoji]
-                return
-        
-        if line.unknown:
-            line.unknown -=1
-            if set.__len__(line):
-                if line.unknown:
-                    return
-                self._full_check()
-                return
-            if line.unknown:
-                return
-            del self[emoji]
+
+def _validate_reaction_mapping_line_initialise_with_iterable(initialize_with):
+    """
+    Validates the `initialize_with` parameter of ``ReactionMappingLine`` where it is an iterable.
     
+    Parameters
+    ----------
+    initialize_with : `iterable` of (`None`, ``ClientUserBase``)
+        The value ot initialize the line with.
     
-    def remove_emoji(self, emoji):
-        """
-        Removes all the users who reacted with the given ``Emoji`` and then returns the stored line.
-        
-        Parameters
-        ----------
-        emoji : ``Emoji``
-            The emoji to remove.
-        
-        Returns
-        -------
-        line : `None`, ``reaction_mapping_line``
-        """
-        line = self.pop(emoji, None)
-        if line is None:
-            return
+    Returns
+    -------
+    users : `None`, `list` of ``ClientUserBase``
+        The built users from the `initialize_with` parameter.
+    unknown : `int`
+        The amount of unknown users.
+    
+    Raises
+    ------
+    TypeError
+        - If an element of `initialize_with` is not `None`, ``ClientUserBase``.
+    """
+    users = None
+    unknown = 0
+    
+    for user in initialize_with:
+        if user is None:
+            unknown += 1
+            continue
         
-        if line.unknown:
-            self._full_check()
+        if isinstance(user, ClientUserBase):
+            if users is None:
+                users = []
+            
+            users.append(user)
+            continue
         
-        return line
+        raise TypeError(
+            f'`initialize_with` can contain `{ClientUserBase.__name__}` elements, got '
+            f'{user.__class__.__name__}; {user!r}; initialize_with={initialize_with!r}.'
+        )
     
+    return users, unknown
+
+
+def _validate_reaction_mapping_line_unknown(unknown):
+    """
+    Validates the `unknown` parameter of ``ReactionMappingLine``.
     
-    # this function is called if an emoji loses all it's unknown reactors
-    def _full_check(self):
-        """
-        Checks whether the reaction mapping is fully loaded, by checking it's values' `.unknown` and sets the current
-        state to `.fully_loaded`.
-        """
-        for line in self.values():
-            if line.unknown:
-                self.fully_loaded = False
-                return
-        
-        self.fully_loaded = True
+    Parameters
+    ----------
+    unknown : `None, `int`
+        The given `unknown` value to initialize the reaction line with.
     
+    Returns
+    -------
+    validated_unknown : `int`
+    
+    Raises
+    ------
+    TypeError
+        - If `unknown` is not `int`, `None`.
+    ValueError
+        - If `unknown` is negative.
+    """
+    if unknown is None:
+        validated_unknown = 0
     
-    # we call this when we get SOME reactors of an emoji
-    def _update_some_users(self, emoji, users):
-        """
-        Called when some reactors of an emoji are updated.
-        
-        Parameters
-        ----------
-        emoji : ``Emoji``
-            The emoji, which's users' are updated.
-        users : `list` of ``ClientUserBase``
-            The added reactors.
-        """
-        self[emoji].update(users)
-        self._full_check()
-        
-    def _update_all_users(self, emoji, users):
-        """
-        Called when all the reactors of an emoji are updated of the reaction mapping.
+    elif isinstance(unknown, int):
+        if (unknown < 0):
+            raise ValueError(
+                f'`unknown` cannot be negative, got {unknown!r}.'
+            )
         
-        Parameters
-        ----------
-        emoji : ``Emoji``
-            The emoji, which's users' are updated.
-        users : `list` of ``ClientUserBase``
-            The added reactors.
-        """
-        self[emoji] = reaction_mapping_line._full(users)
-        self._full_check()
+        validated_unknown = unknown
     
+    else:
+        raise TypeError(
+            f'`unknown` can be `None`, `int`, got {unknown.__class__.__name__}; {unknown!r}.'
+        )
     
-    def to_data(self):
-        """
-        Tries to convert the reactions back to a json serializable list.
-        
-        Returns
-        -------
-        data : `list` of `dict` of (`str`, `Any`)
-        """
-        data = []
-        for emoji, users in self.items():
-            length = len(users)
-            if length:
-                data.append({
-                    'count': length,
-                    'me': False, # Me is always False
-                    'emoji': create_partial_emoji_data(emoji),
-                })
-        
-        return data
+    return validated_unknown
 
 
-class reaction_mapping_line(set):
+class ReactionMappingLine(set):
     """
     A `set` subclass which contains the users who reacted with the given ``Emoji`` on a ``Message``.
     
     Attributes
     ----------
     unknown : `int`
         The amount of not known reactors.
     """
     __slots__ = ('unknown',)
     
-    def __init__(self, unknown):
+    if NEEDS_DUMMY_INIT:
+        def __init__(self, *args, **kwargs):
+            pass
+    else:
+        __init__ = object.__init__
+    
+    
+    def __new__(cls, initialize_with=None, unknown=None):
         """
-        Creates a `reaction_mapping_line`.
+        Creates a new reaction mapping line
+        
+        Parameters
+        ----------
+        initialize_with : `None`, `iterable` of (`None`, ``ClientUserBase``), `instance<reaction_mapping_line_type>` \
+                = `None`, Optional
+            The value ot initialize the line with.
+        unknown : `None, `int` = `None`, Optional
+            The given `unknown` value to initialize the reaction line with.
+        
+        Raises
+        ------
+        TypeError
+            - If a parameter's type is not acceptable.
+        ValueError
+            - If a parameter's value is not acceptable.
+        """
+        validated_line, validated_unknown = _validate_reaction_mapping_line_initialise_with(cls, initialize_with)
+        validated_unknown += _validate_reaction_mapping_line_unknown(unknown)
+        
+        self = set.__new__(cls)
+        self.unknown = validated_unknown
+        
+        if (validated_line is not None):
+            set.update(self, validated_line)
+        
+        return self
+    
+    
+    @classmethod
+    def _create_empty(cls, unknown):
+        """
+        Creates a new reaction mapping line.
         
         Parameters
         ----------
         unknown : `int`
             The amount of not known reactors.
+        
+        Returns
+        -------
+        self : instance<cls>
         """
+        self = set.__new__(cls)
         self.unknown = unknown
+        return self
+    
     
     def __len__(self):
         """Returns the amount of users, who reacted with the given emoji on the respective message."""
         return set.__len__(self) + self.unknown
     
     
     def __repr__(self):
@@ -269,121 +254,203 @@
             repr_parts.append(repr(unknown))
         
         repr_parts.append(')')
         
         return ''.join(repr_parts)
     
     
+    def __bool__(self):
+        """Returns whether self has any elements."""
+        if self.unknown:
+            return True
+        
+        if set.__len__(self):
+            return True
+        
+        return False
+    
+    
+    def __eq__(self, other):
+        """Returns whether self equals to other."""
+        if type(self) is type(other):
+            return self._is_equal_same_type(other)
+            
+        if (getattr(other, '__iter__', None) is not None):
+            return self._is_equal_iterable(other)
+        
+        return NotImplemented
+    
+    
+    def _is_equal_same_type(self, other):
+        """
+        Returns whether self equals to other. `other` must be same type as self.
+        
+        Parameters
+        ----------
+        other : `instance<type<self>>`
+            The other reaction mapping line to compare self to.
+        
+        Returns
+        -------
+        is_equal : `bool`
+        """
+        if self.unknown != other.unknown:
+            return False
+        
+        if not set.__eq__(self, other):
+            return False
+        
+        return True
+    
+    
+    def _is_equal_iterable(self, other):
+        """
+        Returns whether self equals to other, where other is an iterable.
+        
+        Parameters
+        ----------
+        other : `iterable` of (`None`, ``ClientUserBase``)
+            The other object to compare self to.
+        
+        Returns
+        -------
+        is_equal : `NotImplemented`, `bool`
+        """
+        unknown = 0
+        users = set()
+        
+        for user in other:
+            if user is None:
+                unknown += 1
+                continue
+            
+            if isinstance(user, ClientUserBase):
+                users.add(user)
+                continue
+            
+            return NotImplemented
+        
+        
+        if self.unknown != unknown:
+            return False
+        
+        if not set.__eq__(self, users):
+            return False
+        
+        return True
+    
+    
     @classmethod
-    def _full(cls, users):
+    def _create_full(cls, users):
         """
-        Creates a new ``reaction_mapping_line`` with the given users with `.unknown` set to `0`.
+        Creates a new ``ReactionMappingLine`` with the given users with `.unknown` set to `0`.
         
         Parameters
         ----------
         users : `list` of ``ClientUserBase``
             A `list`, which should already contain all the users of the reaction mapping line.
 
         Returns
         -------
-        self : ``reaction_mapping_line``
+        self : ``ReactionMappingLine``
         """
         self = set.__new__(cls)
-        set.__init__(self, users)
         self.unknown = 0
+        set.update(self, users)
         return self
     
     
     def update(self, users):
         """
         Updates the reaction mapping line with the given users.
         
         Parameters
         ----------
         users : `list` of ``ClientUserBase``
             A `list` of users, who reacted on the respective `Message` with the respective ``Emoji``.
         """
-        ln_old = len(self)
+        length_old = len(self)
         set.update(self, users)
-        ln_new = len(self)
-        self.unknown -= (ln_new - ln_old)
+        length_new = len(self)
+        
+        unknown = self.unknown - (length_new - length_old)
+        if (unknown < 0):
+            unknown = 0
+        self.unknown = unknown
     
     
     def copy(self):
         """
         Copies the reaction mapping line.
         
         Returns
         -------
-        new : ``reaction_mapping_line``
+        new : ``ReactionMappingLine``
         """
         new = set.__new__(type(self))
-        set.__init__(new,self)
+        set.__init__(new, self)
         new.unknown = self.unknown
         return new
     
     
-    # executes an api request if we know we know all reactors
     def filter_after(self, limit, after):
         """
         If we know all the reactors, then instead of executing a Discord API request we filter the reactors locally
         using this method.
         
         Parameters
         ----------
         limit : `int`
             The maximal limit of the users to return.
         after : `int`
             Gets the users after this specified id.
         
         Returns
         -------
-        users : `
+        users : `list` of ``ClientUserBase``
         """
-        list_form = sorted(self)
-        
-        after = after + 1 # do not include the specified id
-        
-        bot = 0
-        top = len(list_form)
-        while True:
-            if bot < top:
-                half = (bot + top) >> 1
-                if list_form[half].id < after:
-                    bot = half + 1
-                else:
-                    top = half
-                continue
-            break
-        
-        index = bot
-        
-        length = len(list_form)
-        users = []
-        
-        while True:
-            if index == length:
-                break
-            
-            if limit <= 0:
-                break
-            
-            users.append(list_form[index])
-            index += 1
-            limit -= 1
-            continue
-        
-        return users
+        return sorted([user for user in set.__iter__(self) if user.id > after])[:limit]
     
     
     def clear(self):
         """
         Clears the reaction mapping line by removing every ``User`` object from it.
         """
         clients = []
         for user in self:
             if isinstance(user, Client):
                 clients.append(user)
 
         self.unknown += (set.__len__(self) - len(clients))
         set.clear(self)
         set.update(self, clients)
+    
+    
+    def remove(self, user):
+        """
+        Removes the given user from self.
+        
+        Parameters
+        ----------
+        user : ``ClientUserBase``
+            The user to remove.
+        
+        Returns
+        -------
+        success : `bool`
+            Whether the user was successfully removed.
+        """
+        try:
+            set.remove(self, user)
+        except KeyError:
+            unknown = self.unknown
+            if unknown > 0:
+                self.unknown = unknown - 1
+                success = True
+            
+            else:
+                success = False
+        
+        else:
+            success = True
+        
+        return success
```

### Comparing `hata-1.3.8/hata/discord/emoji/unicode_type.py` & `hata-1.3.9/hata/discord/emoji/unicode_type.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/emoji/unicodes.py` & `hata-1.3.9/hata/discord/emoji/unicodes.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/emoji/utils.py` & `hata-1.3.9/hata/discord/emoji/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 __all__ = (
-    'create_partial_emoji_data', 'create_partial_emoji_from_data', 'create_emoji_from_exclusive_data',
-    'create_unicode_emoji', 'parse_all_emojis', 'parse_all_emojis_ordered', 'parse_custom_emojis',
-    'parse_custom_emojis_ordered', 'parse_emoji', 'parse_reaction', 'put_exclusive_emoji_data_into',
-    'put_partial_emoji_data_into'
+    'create_partial_emoji_data', 'create_partial_emoji_from_data', 'create_partial_emoji_from_id',
+    'create_emoji_from_exclusive_data', 'create_unicode_emoji', 'parse_all_emojis', 'parse_all_emojis_ordered',
+    'parse_custom_emojis', 'parse_custom_emojis_ordered', 'parse_emoji', 'parse_reaction',
+    'put_exclusive_emoji_data_into', 'put_partial_emoji_data_into', 'merge_update_reaction_mapping'
 )
 
 import warnings
 
 from scarletio import export
 
-from ..core import BUILTIN_EMOJIS, UNICODE_TO_EMOJI
+from ..core import BUILTIN_EMOJIS, EMOJIS, UNICODE_TO_EMOJI
 from ..utils import EMOJI_RP, REACTION_RP
 
 from .emoji import Emoji
 from .emoji_all_pattern import EMOJI_ALL_RP
 from .unicode_type import Unicode, VARIATION_SELECTOR_16_POSTFIX
 
 
@@ -82,14 +82,36 @@
             emoji_name = ''
             
         emoji = Emoji._create_partial(int(emoji_id), emoji_name, emoji_animated)
     
     return emoji
 
 
+def create_partial_emoji_from_id(emoji_id):
+    """
+    Creates a partial emoji from the given id.
+    
+    Parameters
+    ----------
+    emoji_id : `int`
+        The emoji's identifier.
+    
+    Returns
+    -------
+    emoji : ``Emoji``
+    """
+    try:
+        emoji = EMOJIS[emoji_id]
+    except KeyError:
+        emoji = Emoji._create_empty(emoji_id)
+        EMOJIS[emoji_id] = emoji
+    
+    return emoji
+
+
 @export
 def create_partial_emoji_data(emoji):
     """
     Creates partial emoji data form the given emoji.
     
     Parameters
     ----------
@@ -170,15 +192,15 @@
     if (emoji_name is not None):
         try:
             emoji = UNICODE_TO_EMOJI[emoji_name]
         except KeyError:
             emoji = _create_new_unicode(emoji_name)
     
     elif (emoji_id is not None):
-        emoji = Emoji._create_partial(int(emoji_id), '', False)
+        emoji = create_partial_emoji_from_id(int(emoji_id))
     
     else:
         emoji = None
     
     return emoji
 
 
@@ -455,7 +477,51 @@
         warnings.warn(
             f'Undefined emoji : {unicode.encode()!r}\nPlease open an issue with this message.',
             RuntimeWarning,
         )
         unicode_emoji = Emoji._create_unicode(Unicode('', unicode, False, None, None), False)
     
     return unicode_emoji
+
+
+def merge_update_reaction_mapping(old_reactions, new_reactions):
+    """
+    Merges the two reaction mapping, so values wont be overwritten if not required.
+    
+    Parameters
+    ----------
+    old_reactions : `None`, ``ReactionMapping``
+        The old reactions on a message.
+    new_reactions : `None`, ``ReactionMapping``
+        The new reactions on a message.
+    
+    Returns
+    -------
+    real_reactions : `None`, ``ReactionMapping``
+        The real merged reactions on a message.
+    """
+    if (old_reactions is None):
+        return new_reactions
+    
+    elif (new_reactions is None):
+        old_reactions.clear()
+        return old_reactions
+    
+    old_emojis = {*old_reactions.keys()}
+    new_emojis = {*new_reactions.keys()}
+    
+    for emoji in old_emojis - new_emojis:
+        del old_reactions[emoji]
+    
+    for emoji in new_emojis - old_emojis:
+        old_reactions[emoji] = new_reactions[emoji].copy()
+    
+    for emoji in new_emojis & old_emojis:
+        old_users = old_reactions[emoji]
+        new_users = new_reactions[emoji]
+        
+        if (len(old_users) != len(new_users)) or (not (old_users >= new_users)):
+            old_reactions[emoji] = new_reactions[emoji].copy()
+    
+    old_reactions._full_check()
+    
+    return old_reactions
```

### Comparing `hata-1.3.8/hata/discord/events/__init__.py` & `hata-1.3.9/hata/discord/events/__init__.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/events/core.py` & `hata-1.3.9/hata/discord/events/core.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/events/default_event_handlers.py` & `hata-1.3.9/hata/discord/events/default_event_handlers.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/events/event_handler_manager.py` & `hata-1.3.9/hata/discord/events/event_handler_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -742,24 +742,24 @@
         `old_attributes` might contain also `embeds`.
         
         > If the message is partial (usually when it is not cached), `old_attributes` is passed as `None`.
     
     reaction_add(client: ``Client``, event: ``ReactionAddEvent``):
         Called when a user reacts on a message with the given emoji.
     
-    reaction_clear(client: ``Client``, message: ``Message``, reactions: {`None`, ``reaction_mapping``}):
+    reaction_clear(client: ``Client``, message: ``Message``, reactions: {`None`, ``ReactionMapping``}):
         Called when the reactions of a message are cleared. The passed `old_reactions` parameter are the old reactions
         of the message.
         
         > If the message is partial (usually when it is not cached), `reactions` is passed as `None`.
     
     reaction_delete(client: ``Client``, event: ``ReactionDeleteEvent``):
         Called when a user removes it's reaction from a message.
     
-    reaction_delete_emoji(client: ``Client``, message: ``Message``, users: {`None`, ``reaction_mapping_line``}):
+    reaction_delete_emoji(client: ``Client``, message: ``Message``, users: {`None`, ``ReactionMappingLine``}):
         Called when all the reactions of a specified emoji are removed from a message. The passed `users` parameter
         are the old reactor users of the given emoji.
         
         > If the message is partial (usually when it is not cached), `users` is passed as `None`.
     
     ready(client: ``Client``):
         Called when the client finishes logging in. The event might be called more times, because the clients might
```

### Comparing `hata-1.3.8/hata/discord/events/event_handler_plugin.py` & `hata-1.3.9/hata/discord/events/event_handler_plugin.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/events/event_types.py` & `hata-1.3.9/hata/discord/events/event_types.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/events/filters.py` & `hata-1.3.9/hata/discord/events/filters.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/events/guild_sync.py` & `hata-1.3.9/hata/discord/events/guild_sync.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/events/handling_helpers.py` & `hata-1.3.9/hata/discord/events/handling_helpers.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/events/intent.py` & `hata-1.3.9/hata/discord/events/intent.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/events/parsers.py` & `hata-1.3.9/hata/discord/events/parsers.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/exceptions/discord_exception.py` & `hata-1.3.9/hata/discord/exceptions/discord_exception.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/exceptions/discord_gateway_exception.py` & `hata-1.3.9/hata/discord/exceptions/discord_gateway_exception.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/exceptions/error_codes.py` & `hata-1.3.9/hata/discord/exceptions/error_codes.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/exceptions/payload_renderer.py` & `hata-1.3.9/hata/discord/exceptions/payload_renderer.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/gateway/client_gateway.py` & `hata-1.3.9/hata/discord/gateway/client_gateway.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/gateway/heartbeat.py` & `hata-1.3.9/hata/discord/gateway/heartbeat.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/gateway/rate_limit.py` & `hata-1.3.9/hata/discord/gateway/rate_limit.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/gateway/voice_client_gateway.py` & `hata-1.3.9/hata/discord/gateway/voice_client_gateway.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/guild/__init__.py` & `hata-1.3.9/hata/discord/guild/__init__.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/guild/audit_logs/__init__.py` & `hata-1.3.9/hata/discord/guild/audit_logs/__init__.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/guild/audit_logs/audit_log.py` & `hata-1.3.9/hata/discord/guild/audit_logs/audit_log.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/guild/audit_logs/audit_log_change.py` & `hata-1.3.9/hata/discord/guild/audit_logs/audit_log_change.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/guild/audit_logs/audit_log_entry.py` & `hata-1.3.9/hata/discord/guild/audit_logs/audit_log_entry.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/guild/audit_logs/audit_log_iterator.py` & `hata-1.3.9/hata/discord/guild/audit_logs/audit_log_iterator.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/guild/audit_logs/audit_log_role.py` & `hata-1.3.9/hata/discord/guild/audit_logs/audit_log_role.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/guild/audit_logs/change_converters/__init__.py` & `hata-1.3.9/hata/discord/guild/audit_logs/change_converters/__init__.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/guild/audit_logs/change_converters/all_.py` & `hata-1.3.9/hata/discord/guild/audit_logs/change_converters/all_.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/guild/audit_logs/change_converters/auto_moderation_rule.py` & `hata-1.3.9/hata/discord/guild/audit_logs/change_converters/auto_moderation_rule.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/guild/audit_logs/change_converters/channel.py` & `hata-1.3.9/hata/discord/guild/audit_logs/change_converters/channel.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/guild/audit_logs/change_converters/channel_permission_overwrite.py` & `hata-1.3.9/hata/discord/guild/audit_logs/change_converters/channel_permission_overwrite.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/guild/audit_logs/change_converters/guild.py` & `hata-1.3.9/hata/discord/guild/audit_logs/change_converters/guild.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/guild/audit_logs/change_converters/role.py` & `hata-1.3.9/hata/discord/guild/audit_logs/change_converters/role.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/guild/audit_logs/change_converters/scheduled_event.py` & `hata-1.3.9/hata/discord/guild/audit_logs/change_converters/scheduled_event.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/guild/audit_logs/change_converters/shared.py` & `hata-1.3.9/hata/discord/guild/audit_logs/change_converters/shared.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/guild/audit_logs/change_converters/sticker.py` & `hata-1.3.9/hata/discord/guild/audit_logs/change_converters/sticker.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/guild/audit_logs/change_converters/user.py` & `hata-1.3.9/hata/discord/guild/audit_logs/change_converters/user.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/guild/audit_logs/detail_converters.py` & `hata-1.3.9/hata/discord/guild/audit_logs/detail_converters.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/guild/audit_logs/preinstanced.py` & `hata-1.3.9/hata/discord/guild/audit_logs/preinstanced.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/guild/audit_logs/target_converters.py` & `hata-1.3.9/hata/discord/guild/audit_logs/target_converters.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/guild/discovery.py` & `hata-1.3.9/hata/discord/guild/discovery.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/guild/embedded_activity_state.py` & `hata-1.3.9/hata/discord/guild/embedded_activity_state.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/guild/event_types.py` & `hata-1.3.9/hata/discord/guild/event_types.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/guild/flags.py` & `hata-1.3.9/hata/discord/guild/flags.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/guild/guild.py` & `hata-1.3.9/hata/discord/guild/guild.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/guild/preinstanced.py` & `hata-1.3.9/hata/discord/guild/preinstanced.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/guild/preview.py` & `hata-1.3.9/hata/discord/guild/preview.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/guild/utils.py` & `hata-1.3.9/hata/discord/guild/utils.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/guild/verification_screen.py` & `hata-1.3.9/hata/discord/guild/verification_screen.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/guild/welcome_screen.py` & `hata-1.3.9/hata/discord/guild/welcome_screen.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/guild/widget.py` & `hata-1.3.9/hata/discord/guild/widget.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/http/http_client.py` & `hata-1.3.9/hata/discord/http/http_client.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/http/rate_limit.py` & `hata-1.3.9/hata/discord/http/rate_limit.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/http/rate_limit_groups.py` & `hata-1.3.9/hata/discord/http/rate_limit_groups.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/http/rate_limit_proxy.py` & `hata-1.3.9/hata/discord/http/rate_limit_proxy.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/http/urls.py` & `hata-1.3.9/hata/discord/http/urls.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/integration/integration.py` & `hata-1.3.9/hata/discord/integration/integration.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/integration/integration_account.py` & `hata-1.3.9/hata/discord/integration/integration_account.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/integration/integration_application.py` & `hata-1.3.9/hata/discord/integration/integration_application.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/integration/integration_detail.py` & `hata-1.3.9/hata/discord/integration/integration_detail.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/integration/preinstanced.py` & `hata-1.3.9/hata/discord/integration/preinstanced.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/integration/utils.py` & `hata-1.3.9/hata/discord/integration/utils.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/interaction/application_command/__init__.py` & `hata-1.3.9/hata/discord/interaction/application_command/__init__.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/interaction/application_command/application_command.py` & `hata-1.3.9/hata/discord/interaction/application_command/application_command.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/interaction/application_command/application_command_option.py` & `hata-1.3.9/hata/discord/interaction/application_command/application_command_option.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/interaction/application_command/application_command_option_choice.py` & `hata-1.3.9/hata/discord/interaction/application_command/application_command_option_choice.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/interaction/application_command/application_command_permission.py` & `hata-1.3.9/hata/discord/interaction/application_command/application_command_permission.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/interaction/application_command/application_command_permission_overwrite.py` & `hata-1.3.9/hata/discord/interaction/application_command/application_command_permission_overwrite.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/interaction/application_command/constants.py` & `hata-1.3.9/hata/discord/interaction/application_command/constants.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/interaction/application_command/helpers.py` & `hata-1.3.9/hata/discord/interaction/application_command/helpers.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/interaction/application_command/preinstanced.py` & `hata-1.3.9/hata/discord/interaction/application_command/preinstanced.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/interaction/components/__init__.py` & `hata-1.3.9/hata/discord/interaction/components/__init__.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/interaction/components/component_base.py` & `hata-1.3.9/hata/discord/interaction/components/component_base.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/interaction/components/component_button.py` & `hata-1.3.9/hata/discord/interaction/components/component_button.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/interaction/components/component_dynamic.py` & `hata-1.3.9/hata/discord/interaction/components/component_dynamic.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/interaction/components/component_row.py` & `hata-1.3.9/hata/discord/interaction/components/component_row.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/interaction/components/component_select.py` & `hata-1.3.9/hata/discord/interaction/components/component_select.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/interaction/components/component_select_option.py` & `hata-1.3.9/hata/discord/interaction/components/component_select_option.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/interaction/components/component_text_input.py` & `hata-1.3.9/hata/discord/interaction/components/component_text_input.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/interaction/components/constants.py` & `hata-1.3.9/hata/discord/interaction/components/constants.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/interaction/components/debug.py` & `hata-1.3.9/hata/discord/interaction/components/debug.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/interaction/components/form.py` & `hata-1.3.9/hata/discord/interaction/components/form.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/interaction/components/preinstanced.py` & `hata-1.3.9/hata/discord/interaction/components/preinstanced.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/interaction/components/utils.py` & `hata-1.3.9/hata/discord/interaction/components/utils.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/interaction/event_types/__init__.py` & `hata-1.3.9/hata/discord/interaction/event_types/__init__.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/interaction/event_types/application_command_autocomplete_interaction.py` & `hata-1.3.9/hata/discord/interaction/event_types/application_command_autocomplete_interaction.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/interaction/event_types/application_command_interaction.py` & `hata-1.3.9/hata/discord/interaction/event_types/application_command_interaction.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/interaction/event_types/component_interaction.py` & `hata-1.3.9/hata/discord/interaction/event_types/component_interaction.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/interaction/event_types/form_submit_interaction.py` & `hata-1.3.9/hata/discord/interaction/event_types/form_submit_interaction.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/interaction/event_types/interaction_event.py` & `hata-1.3.9/hata/discord/interaction/event_types/interaction_event.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/interaction/event_types/interaction_field_base.py` & `hata-1.3.9/hata/discord/interaction/event_types/interaction_field_base.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/interaction/event_types/preinstanced.py` & `hata-1.3.9/hata/discord/interaction/event_types/preinstanced.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/interaction/interaction_response_context.py` & `hata-1.3.9/hata/discord/interaction/interaction_response_context.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/interaction/interaction_response_types.py` & `hata-1.3.9/hata/discord/interaction/interaction_response_types.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/invite/invite.py` & `hata-1.3.9/hata/discord/invite/invite.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/invite/invite_stage.py` & `hata-1.3.9/hata/discord/invite/invite_stage.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/invite/preinstanced.py` & `hata-1.3.9/hata/discord/invite/preinstanced.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/localizations/helpers.py` & `hata-1.3.9/hata/discord/localizations/helpers.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/localizations/preinstanced.py` & `hata-1.3.9/hata/discord/localizations/preinstanced.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/localizations/utils.py` & `hata-1.3.9/hata/discord/localizations/utils.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/message/__init__.py` & `hata-1.3.9/hata/discord/message/__init__.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/message/attachment.py` & `hata-1.3.9/hata/discord/message/attachment.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/message/cross_mention.py` & `hata-1.3.9/hata/discord/message/cross_mention.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/message/flags.py` & `hata-1.3.9/hata/discord/message/flags.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/message/message.py` & `hata-1.3.9/hata/discord/message/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from datetime import datetime
 
 from scarletio import BaseMethodDescriptor, export, include
 
 from ..bases import DiscordEntity, id_sort_key
 from ..core import CHANNELS, GUILDS, MESSAGES
 from ..embed import EXTRA_EMBED_TYPES, EmbedBase, EmbedCore
-from ..emoji import reaction_mapping
+from ..emoji import ReactionMapping, merge_update_reaction_mapping
 from ..http import urls as module_urls
 from ..preconverters import (
     get_type_names, preconvert_bool, preconvert_flag, preconvert_preinstanced_type, preconvert_snowflake,
     preconvert_snowflake_array, preconvert_str
 )
 from ..role import Role, create_partial_role_from_id
 from ..sticker import Sticker
@@ -556,15 +556,21 @@
         # At this point every static field is set, now we switch to dynamic ones.
         
         reactions_data = data.get('reactions', None)
         if (reactions_data is not None) and reactions_data:
             _set_message_field(
                 self,
                 MESSAGE_FIELD_KEY_REACTIONS,
-                reaction_mapping(reactions_data),
+                merge_update_reaction_mapping(
+                    _get_message_field(
+                        self,
+                        MESSAGE_FIELD_KEY_REACTIONS,
+                    ),
+                    ReactionMapping.from_data(reactions_data),
+                )
             )
         
         referenced_message_data = data.get('referenced_message', None)
         if referenced_message_data is None:
             referenced_message_data = data.get('message_reference', None)
             if referenced_message_data is None:
                 referenced_message = None
@@ -909,15 +915,15 @@
         
         pinned : `bool`, `int` (`0`, `1`), Optional (Keyword only)
             The ``.pinned`` attribute of the message. Accepts other `int` as `bool` as well, but their value
             still cannot be other than `0`, `1`.
             
             If called as a classmethod, defaults to `False`.
         
-        reactions : `None`, ``reaction_mapping``, Optional (Keyword only)
+        reactions : `None`, ``ReactionMapping``, Optional (Keyword only)
             The ``.reactions`` attribute of the message.
             
             If called as a classmethod defaults to `None`.
         
         role_mentions : `None`, (`list`, `tuple`) of ``Role``, Optional (Keyword only)
             The ``.role_mentions`` attribute of the message. If passed as an empty `list`, will be set as `None`
             instead.
@@ -1365,30 +1371,30 @@
         else:
             pinned = preconvert_bool(pinned, 'pinned')
         
         try:
             reactions = kwargs.pop('reactions')
         except KeyError:
             if base is None:
-                reactions = reaction_mapping(None)
+                reactions = ReactionMapping()
             else:
                 reactions = base.reactions
                 if (reactions is not None):
                     # Copy it, because it might be modified
                     reactions = reactions.copy()
         else:
             if reactions is None:
                 # Lets accept `None` and create an empty one
-                reactions = reaction_mapping(None)
-            elif type(reactions) is reaction_mapping:
+                reactions = ReactionMapping()
+            elif type(reactions) is ReactionMapping:
                 # We expect this as default
                 pass
             else:
                 raise TypeError(
-                    f'`reactions`, can be `None`, `{reaction_mapping.__name__}`, got '
+                    f'`reactions`, can be `None`, `{ReactionMapping.__name__}`, got '
                     f'{reactions.__class__.__name__}; {reactions}.'
                 )
         
         try:
             role_mentions = kwargs.pop('role_mentions')
         except KeyError:
             if base is None:
@@ -2497,15 +2503,15 @@
         emoji : ``Emoji``
             The reacted emoji.
         user : ``ClientUserBase``
             The reactor user.
         """
         reactions = self.reactions
         if reactions is None:
-            reactions = reaction_mapping(None)
+            reactions = ReactionMapping(None)
             self.reactions = reactions
         
         return reactions.add(emoji, user)
     
     
     def _remove_reaction(self, emoji, user):
         """
@@ -2530,15 +2536,15 @@
         Parameters
         ----------
         emoji : ``Emoji``
             The emoji to remove it's reactions.
         
         Returns
         -------
-        line : `None`, ``reaction_mapping_line``
+        line : `None`, ``ReactionMappingLine``
         """
         reactions = self.reactions
         if (reactions is not None):
             return reactions.remove_emoji(emoji)
     
     
     @classmethod
@@ -2620,15 +2626,15 @@
             The ``.nonce`` attribute of the message. If passed as `str` can be between length `0` and `32`.
             
             If called as a classmethod defaults to `None`.
         pinned : `bool`, `int` (`0`, `1`), Optional (Keyword only)
             The ``.pinned`` attribute of the message. Accepts other `int` as `bool` as well, but their value
             still cannot be other than `0`, `1`.
         
-        reactions : `None`, ``reaction_mapping``, Optional (Keyword only)
+        reactions : `None`, ``ReactionMapping``, Optional (Keyword only)
             The ``.reactions`` attribute of the message.
         
         role_mentions : `None`, (`list`, `tuple`) of ``Role``, Optional (Keyword only)
             The ``.role_mentions`` attribute of the message. If passed as an empty `list`, will be set as `None`
             instead.
             
         stickers : `None`, (`list`, `tuple`) of ``Sticker``, Optional (Keyword only)
@@ -2689,15 +2695,15 @@
             
             for variable_field_key, variable_type, variable_name in (
                 (MESSAGE_FIELD_KEY_ACTIVITY, MessageActivity, 'activity'),
                 (MESSAGE_FIELD_KEY_APPLICATION, MessageApplication, 'application'),
                 (MESSAGE_FIELD_KEY_REFERENCED_MESSAGE, Message, 'referenced_message'),
                 (MESSAGE_FIELD_KEY_EDITED_AT, datetime, 'edited_at'),
                 (MESSAGE_FIELD_KEY_INTERACTION, MessageInteraction, 'interaction'),
-                (MESSAGE_FIELD_KEY_REACTIONS, reaction_mapping, 'reactions'),
+                (MESSAGE_FIELD_KEY_REACTIONS, ReactionMapping, 'reactions'),
                 (MESSAGE_FIELD_KEY_THREAD, Channel, 'thread'),
             ):
                 try:
                     variable_value = kwargs.pop(variable_name)
                 except KeyError:
                     pass
                 else:
@@ -4212,15 +4218,15 @@
         """
         A dictionary like object, which contains the reactions on the message.
         
         Defaults to `None`.
         
         Returns
         -------
-        reactions : `None`, ``reaction_mapping``
+        reactions : `None`, ``ReactionMapping``
         """
         return _get_message_field(
             self,
             MESSAGE_FIELD_KEY_REACTIONS,
         )
     
     @reactions.setter
```

### Comparing `hata-1.3.8/hata/discord/message/message_activity.py` & `hata-1.3.9/hata/discord/message/message_activity.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/message/message_application.py` & `hata-1.3.9/hata/discord/message/message_application.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/message/message_interaction.py` & `hata-1.3.9/hata/discord/message/message_interaction.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/message/preinstanced.py` & `hata-1.3.9/hata/discord/message/preinstanced.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/message/utils.py` & `hata-1.3.9/hata/discord/message/utils.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/oauth2/achievement.py` & `hata-1.3.9/hata/discord/oauth2/achievement.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/oauth2/connection.py` & `hata-1.3.9/hata/discord/oauth2/connection.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/oauth2/helpers.py` & `hata-1.3.9/hata/discord/oauth2/helpers.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/oauth2/oauth2_access.py` & `hata-1.3.9/hata/discord/oauth2/oauth2_access.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/oauth2/oauth2_user.py` & `hata-1.3.9/hata/discord/oauth2/oauth2_user.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/oauth2/preinstanced.py` & `hata-1.3.9/hata/discord/oauth2/preinstanced.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/object_binding.py` & `hata-1.3.9/hata/discord/object_binding.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/permission/permission.py` & `hata-1.3.9/hata/discord/permission/permission.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/permission/permission_overwrite.py` & `hata-1.3.9/hata/discord/permission/permission_overwrite.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/permission/preinstanced.py` & `hata-1.3.9/hata/discord/permission/preinstanced.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/permission/utils.py` & `hata-1.3.9/hata/discord/permission/utils.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/preconverters.py` & `hata-1.3.9/hata/discord/preconverters.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/role/preinstanced.py` & `hata-1.3.9/hata/discord/role/preinstanced.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/role/role.py` & `hata-1.3.9/hata/discord/role/role.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/role/utils.py` & `hata-1.3.9/hata/discord/role/utils.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/scheduled_event/event_types.py` & `hata-1.3.9/hata/discord/scheduled_event/event_types.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/scheduled_event/metadata/base.py` & `hata-1.3.9/hata/discord/scheduled_event/metadata/base.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/scheduled_event/metadata/location.py` & `hata-1.3.9/hata/discord/scheduled_event/metadata/location.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/scheduled_event/metadata/stage.py` & `hata-1.3.9/hata/discord/scheduled_event/metadata/stage.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/scheduled_event/metadata/utils.py` & `hata-1.3.9/hata/discord/scheduled_event/metadata/utils.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/scheduled_event/preinstanced.py` & `hata-1.3.9/hata/discord/scheduled_event/preinstanced.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/scheduled_event/scheduled_event.py` & `hata-1.3.9/hata/discord/scheduled_event/scheduled_event.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/stage/stage.py` & `hata-1.3.9/hata/discord/stage/stage.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/sticker/preinstanced.py` & `hata-1.3.9/hata/discord/sticker/preinstanced.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/sticker/sticker.py` & `hata-1.3.9/hata/discord/sticker/sticker.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/sticker/sticker_pack.py` & `hata-1.3.9/hata/discord/sticker/sticker_pack.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/user/__init__.py` & `hata-1.3.9/hata/discord/user/__init__.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/user/activity_change.py` & `hata-1.3.9/hata/discord/user/activity_change.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/user/client_user_base.py` & `hata-1.3.9/hata/discord/user/client_user_base.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/user/flags.py` & `hata-1.3.9/hata/discord/user/flags.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/user/guild_profile.py` & `hata-1.3.9/hata/discord/user/guild_profile.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/user/preinstanced.py` & `hata-1.3.9/hata/discord/user/preinstanced.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/user/thread_profile.py` & `hata-1.3.9/hata/discord/user/thread_profile.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/user/user.py` & `hata-1.3.9/hata/discord/user/user.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/user/user_base.py` & `hata-1.3.9/hata/discord/user/user_base.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/user/utils.py` & `hata-1.3.9/hata/discord/user/utils.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/user/voice_state.py` & `hata-1.3.9/hata/discord/user/voice_state.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/utils.py` & `hata-1.3.9/hata/discord/utils.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/voice/audio_source.py` & `hata-1.3.9/hata/discord/voice/audio_source.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/voice/opus.py` & `hata-1.3.9/hata/discord/voice/opus.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/voice/player.py` & `hata-1.3.9/hata/discord/voice/player.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/voice/reader.py` & `hata-1.3.9/hata/discord/voice/reader.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/voice/rtp_packet.py` & `hata-1.3.9/hata/discord/voice/rtp_packet.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/voice/utils.py` & `hata-1.3.9/hata/discord/voice/utils.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/voice/voice_client.py` & `hata-1.3.9/hata/discord/voice/voice_client.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/webhook/preinstanced.py` & `hata-1.3.9/hata/discord/webhook/preinstanced.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/webhook/utils.py` & `hata-1.3.9/hata/discord/webhook/utils.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/webhook/webhook.py` & `hata-1.3.9/hata/discord/webhook/webhook.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/webhook/webhook_base.py` & `hata-1.3.9/hata/discord/webhook/webhook_base.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/webhook/webhook_repr.py` & `hata-1.3.9/hata/discord/webhook/webhook_repr.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/discord/webhook/webhook_sources.py` & `hata-1.3.9/hata/discord/webhook/webhook_sources.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/env.py` & `hata-1.3.9/hata/env.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/__init__.py` & `hata-1.3.9/hata/ext/__init__.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/command_utils/__init__.py` & `hata-1.3.9/hata/ext/command_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/command_utils/bases.py` & `hata-1.3.9/hata/ext/command_utils/bases.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/command_utils/choose_menu.py` & `hata-1.3.9/hata/ext/command_utils/choose_menu.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/command_utils/closer.py` & `hata-1.3.9/hata/ext/command_utils/closer.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/command_utils/io.py` & `hata-1.3.9/hata/ext/command_utils/io.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/command_utils/pagination.py` & `hata-1.3.9/hata/ext/command_utils/pagination.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/command_utils/user_menu.py` & `hata-1.3.9/hata/ext/command_utils/user_menu.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/command_utils/utils.py` & `hata-1.3.9/hata/ext/command_utils/utils.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/command_utils/waiters.py` & `hata-1.3.9/hata/ext/command_utils/waiters.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/commands_v2/__init__.py` & `hata-1.3.9/hata/ext/commands_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/commands_v2/category.py` & `hata-1.3.9/hata/ext/commands_v2/category.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/commands_v2/checks.py` & `hata-1.3.9/hata/ext/commands_v2/checks.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/commands_v2/client_wrapper_extension.py` & `hata-1.3.9/hata/ext/commands_v2/client_wrapper_extension.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/commands_v2/command.py` & `hata-1.3.9/hata/ext/commands_v2/command.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/commands_v2/command_helpers.py` & `hata-1.3.9/hata/ext/commands_v2/command_helpers.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/commands_v2/command_processor.py` & `hata-1.3.9/hata/ext/commands_v2/command_processor.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/commands_v2/content_parser.py` & `hata-1.3.9/hata/ext/commands_v2/content_parser.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/commands_v2/context.py` & `hata-1.3.9/hata/ext/commands_v2/context.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/commands_v2/cooldown.py` & `hata-1.3.9/hata/ext/commands_v2/cooldown.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,15 +140,15 @@
     guild_id = channel.guild.id
     
     cache = cooldown_handler.cache
     try:
         unit = cache[guild_id]
     except KeyError:
         at_ = LOOP_TIME() + cooldown_handler.reset
-        cache[guild_id] = CooldownUnit(at_, command_context.self.limit)
+        cache[guild_id] = CooldownUnit(at_, cooldown_handler.limit)
         KOKORO.call_at(at_, dict.__delitem__, cache, guild_id)
         return 0.
     
     left = unit.uses_left
     if left > 0:
         unit.uses_left = left - cooldown_handler.weight
         return 0.
@@ -191,15 +191,15 @@
          
         reset : `float`
             The reset time of the cooldown.
         
         limit : `int` = `1`, Optional
             The amount of calls after the respective command goes on cooldown.
         
-        weight : `int` = `int`, Optional
+        weight : `int` = `1`, Optional
             The weight of one call. Defaults to `1`.
         
         Raises
         ------
         TypeError
             - If `str` is not given as `str`.
             - If `weight` is not numeric convertible to `int`.
```

### Comparing `hata-1.3.8/hata/ext/commands_v2/exceptions.py` & `hata-1.3.9/hata/ext/commands_v2/exceptions.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/commands_v2/extension_hook_command_utils.py` & `hata-1.3.9/hata/ext/commands_v2/extension_hook_command_utils.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/commands_v2/helps/subterranean.py` & `hata-1.3.9/hata/ext/commands_v2/helps/subterranean.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/commands_v2/responding.py` & `hata-1.3.9/hata/ext/commands_v2/responding.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/commands_v2/snapshot.py` & `hata-1.3.9/hata/ext/commands_v2/snapshot.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/commands_v2/utils.py` & `hata-1.3.9/hata/ext/commands_v2/utils.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/commands_v2/wrappers.py` & `hata-1.3.9/hata/ext/commands_v2/wrappers.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/extension_loader/__init__.py` & `hata-1.3.9/hata/ext/extension_loader/__init__.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/kokoro_sqlalchemy/kokoro_sqlalchemy.py` & `hata-1.3.9/hata/ext/kokoro_sqlalchemy/kokoro_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/patchouli/__init__.py` & `hata-1.3.9/hata/ext/patchouli/__init__.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/patchouli/builder_html.py` & `hata-1.3.9/hata/ext/patchouli/builder_html.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/patchouli/builder_html_extended.py` & `hata-1.3.9/hata/ext/patchouli/builder_html_extended.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/patchouli/builder_text.py` & `hata-1.3.9/hata/ext/patchouli/builder_text.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/patchouli/graver.py` & `hata-1.3.9/hata/ext/patchouli/graver.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/patchouli/highlight.py` & `hata-1.3.9/hata/ext/patchouli/highlight.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/patchouli/module_mapper.py` & `hata-1.3.9/hata/ext/patchouli/module_mapper.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/patchouli/parser.py` & `hata-1.3.9/hata/ext/patchouli/parser.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/patchouli/qualpath.py` & `hata-1.3.9/hata/ext/patchouli/qualpath.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/plugin_loader/__init__.py` & `hata-1.3.9/hata/ext/plugin_loader/__init__.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/plugin_loader/client_extension.py` & `hata-1.3.9/hata/ext/plugin_loader/client_extension.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/plugin_loader/constants.py` & `hata-1.3.9/hata/ext/plugin_loader/constants.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/plugin_loader/exceptions.py` & `hata-1.3.9/hata/ext/plugin_loader/exceptions.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/plugin_loader/helpers.py` & `hata-1.3.9/hata/ext/plugin_loader/helpers.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/plugin_loader/import_overwrite/module_proxy_type.py` & `hata-1.3.9/hata/ext/plugin_loader/import_overwrite/module_proxy_type.py`

 * *Files 5% similar despite different names*

```diff
@@ -69,30 +69,31 @@
         try:
             attribute_value = getattr(module, attribute_name)
         except AttributeError:
             raise AttributeError(
                 f'{self!r} has no attribute `{attribute_name}`.'
             ) from None
         
+        current_plugin = PLUGINS.get(spec.name, None)
+        
         frame = get_last_module_frame()
         if (frame is None):
             spec = None
         else:
             spec = frame.f_globals.get('__spec__', None)
         
         if spec is None:
             plugin = None
         else:
             plugin = PLUGINS.get(spec.name)
         
-        current_plugin = PLUGINS.get(spec.name, None)
         
-        if (plugin is not None) and (current_plugin is not None) and (plugin is not current_plugin):
-            plugin.add_child_plugin(current_plugin)
-            current_plugin.add_parent_plugin(plugin)
+        if (plugin is not None) and (current_plugin is not None):
+            plugin.add_child_plugin(plugin)
+            current_plugin.add_parent_plugin(current_plugin)
         
         return attribute_value
     
     
     def __repr__(self):
         spec = getattr(self, '__spec__', None)
```

### Comparing `hata-1.3.8/hata/ext/plugin_loader/import_overwrite/module_spec_type.py` & `hata-1.3.9/hata/ext/plugin_loader/import_overwrite/module_spec_type.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/plugin_loader/import_overwrite/plugin_finder.py` & `hata-1.3.9/hata/ext/plugin_loader/import_overwrite/plugin_finder.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/plugin_loader/import_overwrite/source_loader.py` & `hata-1.3.9/hata/ext/plugin_loader/import_overwrite/source_loader.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/plugin_loader/import_overwrite/spec_finder_helpers.py` & `hata-1.3.9/hata/ext/plugin_loader/import_overwrite/spec_finder_helpers.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/plugin_loader/import_overwrite/tools.py` & `hata-1.3.9/hata/ext/plugin_loader/import_overwrite/tools.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/plugin_loader/import_overwrite/utils.py` & `hata-1.3.9/hata/ext/plugin_loader/import_overwrite/utils.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/plugin_loader/plugin.py` & `hata-1.3.9/hata/ext/plugin_loader/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,31 +165,30 @@
         repr_parts.append(' name=')
         repr_parts.append(repr(self._spec.name))
         
         state = self._state
         repr_parts.append(', state=')
         state_name = PLUGIN_STATE_VALUE_TO_NAME.get(state, '???')
         repr_parts.append(state_name)
-        repr_parts.append(' (')
+        repr_parts.append('~')
         repr_parts.append(repr(state))
-        repr_parts.append(')')
         
         if self._locked:
             repr_parts.append(', locked=True')
         
         default_variables = self._default_variables
         if self._extend_default_variables:
             if (default_variables is not None):
-                repr_parts.append(' extends loader\'s defaults with: ')
+                repr_parts.append(' extends defaults with: ')
                 repr_parts.append(repr(default_variables))
         else:
             if default_variables is None:
-                repr_parts.append(' clears loader\'s defaults')
+                repr_parts.append(' clears defaults')
             else:
-                repr_parts.append(' clears loader\'s defaults and uses: ')
+                repr_parts.append(' clears defaults and uses: ')
                 repr_parts.append(repr(default_variables))
         
         repr_parts.append('>')
         
         return ''.join(repr_parts)
     
     
@@ -739,14 +738,17 @@
         Registers a child plugin.
         
         Parameters
         ----------
         plugin : ``Plugin``
             The plugin to register.
         """
+        if plugin is self:
+            return
+        
         child_plugins = self._child_plugins
         if (child_plugins is None):
             child_plugins = WeakSet()
             self._child_plugins = child_plugins
         
         child_plugins.add(plugin)
     
@@ -864,14 +866,17 @@
         Registers a parent plugin.
         
         Parameters
         ----------
         plugin : ``Plugin``
             The plugin to register.
         """
+        if plugin is self:
+            return
+        
         parent_plugins = self._parent_plugins
         if (parent_plugins is None):
             parent_plugins = WeakSet()
             self._parent_plugins = parent_plugins
         
         parent_plugins.add(plugin)
     
@@ -975,25 +980,28 @@
         Returns whether the plugin is a directory.
         
         Returns
         -------
         is_directory : `bool`
         """
         return split_file_name_and_extension(get_file_name(self._spec.origin))[0] == '__init__'
-
-
+    
+    
     def add_sub_module_plugin(self, plugin):
         """
         Registers a sub module plugin.
         
         Parameters
         ----------
         plugin : ``Plugin``
             The plugin to register.
         """
+        if plugin is self:
+            return
+        
         sub_module_plugins = self._sub_module_plugins
         if (sub_module_plugins is None):
             sub_module_plugins = WeakSet()
             self._sub_module_plugins = sub_module_plugins
         
         sub_module_plugins.add(plugin)
```

### Comparing `hata-1.3.8/hata/ext/plugin_loader/plugin_loader.py` & `hata-1.3.9/hata/ext/plugin_loader/plugin_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1399,21 +1399,30 @@
             False,
         )
         await self._check_for_syntax(plugins)
         
         for plugin in plugins:
             exception = await self._plugin_unloader(plugin)
             if (exception is None):
-                exception = await self._plugin_loader(plugin)
+                continue
             
-            if (exception is not None):
-                if error_messages is None:
-                    error_messages = []
-                
-                error_messages.append(exception.message)
+            if error_messages is None:
+                error_messages = []
+            
+            error_messages.append(exception.message)
+        
+        for plugin in reversed(plugins):
+            exception = await self._plugin_loader(plugin)
+            if (exception is None):
+                continue
+            
+            if error_messages is None:
+                error_messages = []
+            
+            error_messages.append(exception.message)
         
         if (error_messages is not None):
             raise PluginError(error_messages) from None
     
     
     async def _plugin_loader(self, plugin):
         """
```

### Comparing `hata-1.3.8/hata/ext/plugin_loader/plugin_root.py` & `hata-1.3.9/hata/ext/plugin_loader/plugin_root.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/plugin_loader/snapshot/base_snapshot_type.py` & `hata-1.3.9/hata/ext/plugin_loader/snapshot/base_snapshot_type.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/plugin_loader/snapshot/event_handler_snapshot.py` & `hata-1.3.9/hata/ext/plugin_loader/snapshot/event_handler_snapshot.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/plugin_loader/snapshot/helpers.py` & `hata-1.3.9/hata/ext/plugin_loader/snapshot/helpers.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/plugin_loader/snapshot/snapshot.py` & `hata-1.3.9/hata/ext/plugin_loader/snapshot/snapshot.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/plugin_loader/utils/__init__.py` & `hata-1.3.9/hata/ext/plugin_loader/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/plugin_loader/utils/get_plugin_like_.py` & `hata-1.3.9/hata/ext/plugin_loader/utils/get_plugin_like_.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/plugin_loader/utils/get_plugins_like_.py` & `hata-1.3.9/hata/ext/plugin_loader/utils/get_plugins_like_.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/plugin_loader/utils/import_plugin_.py` & `hata-1.3.9/hata/ext/plugin_loader/utils/import_plugin_.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/plugin_loader/utils/require_.py` & `hata-1.3.9/hata/ext/plugin_loader/utils/require_.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/prettyprint/prettyprint.py` & `hata-1.3.9/hata/ext/prettyprint/prettyprint.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,15 +181,15 @@
     
     application_id = message.application_id
     if application_id:
         result.append(f'- application_id: {application_id}', 1)
     
     reactions = message.reactions
     if (reactions is not None) and reactions:
-        result.append(str_reaction_mapping(reactions), 1)
+        result.append(str_ReactionMapping(reactions), 1)
     
     application = message.application
     if (application is not None):
         result.append(str_message_application(application, 1))
     
     interaction = message.interaction
     if (interaction is not None):
@@ -306,15 +306,15 @@
         result.append(f'- id: {thread.name}', 2)
     
     return result
 
 def reaction_item_sor_key(item):
     return item[0]
 
-def str_reaction_mapping(reactions, index=None, **kwargs): #ignore index, 1 message can have only 1
+def str_ReactionMapping(reactions, index=None, **kwargs): #ignore index, 1 message can have only 1
     result = PrettyBlock()
     reaction_count = len(reactions)
     result.append(f'Reactions: ({reaction_count})')
     reaction_ordering = list((len(v), k) for k, v in reactions.items())
     reaction_ordering.sort(reverse=True, key=reaction_item_sor_key)
     for times, emoji in reaction_ordering:
         if emoji.is_unicode_emoji():
@@ -325,15 +325,15 @@
             else:
                 animated = ''
         result.append(f'- {emoji} ({emoji.id}){animated} : {times} times', 1)
     #TODO: create a more accurate rendering for containers with small amount of emojis
     #    it will need to be able to handle unknown reactors too!
     return result
 
-def str_reaction_mapping_line(users, **kwargs): #ignore index
+def str_ReactionMappingLine(users, **kwargs): #ignore index
     result = PrettyBlock()
     user_count = len(users)
     unknown = users.unknown
     if unknown:
         result.append(f'Reactors: ({user_count}, unknown: {unknown})')
     else:
         result.append(f'Reactors: ({user_count})')
@@ -1809,16 +1809,16 @@
     user = message_interaction.user
     result.append(f'- user: {user.full_name} ({user.id})')
     
     return result
 
 
 PRETTY_PRINTERS['Message'] = str_message
-PRETTY_PRINTERS['reaction_mapping'] = str_reaction_mapping
-PRETTY_PRINTERS['reaction_mapping_line'] = str_reaction_mapping_line
+PRETTY_PRINTERS['ReactionMapping'] = str_ReactionMapping
+PRETTY_PRINTERS['ReactionMappingLine'] = str_ReactionMappingLine
 PRETTY_PRINTERS['MessageApplication'] = str_message_application
 PRETTY_PRINTERS['Attachment'] = str_attachment
 PRETTY_PRINTERS['EmbedCore'] = str_embed_core
 PRETTY_PRINTERS['Role'] = str_role
 PRETTY_PRINTERS['ChannelText'] = str_channel_text
 PRETTY_PRINTERS['ChannelPrivate'] = str_channel_private
 PRETTY_PRINTERS['ChannelVoice'] = str_channel_voice
```

### Comparing `hata-1.3.8/hata/ext/slash/__init__.py` & `hata-1.3.9/hata/ext/slash/__init__.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/slash/client_wrapper_extension.py` & `hata-1.3.9/hata/ext/slash/client_wrapper_extension.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/slash/command/__init__.py` & `hata-1.3.9/hata/ext/slash/command/__init__.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/slash/command/command_base/command_base.py` & `hata-1.3.9/hata/ext/slash/command/command_base/command_base.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/slash/command/command_base_application_command/command_base_application_command.py` & `hata-1.3.9/hata/ext/slash/command/command_base_application_command/command_base_application_command.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/slash/command/command_base_application_command/constants.py` & `hata-1.3.9/hata/ext/slash/command/command_base_application_command/constants.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/slash/command/command_base_application_command/helpers.py` & `hata-1.3.9/hata/ext/slash/command/command_base_application_command/helpers.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/slash/command/command_base_custom_id/command_base_custom_id.py` & `hata-1.3.9/hata/ext/slash/command/command_base_custom_id/command_base_custom_id.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/slash/command/command_base_custom_id/helpers.py` & `hata-1.3.9/hata/ext/slash/command/command_base_custom_id/helpers.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/slash/command/component_command/component_command.py` & `hata-1.3.9/hata/ext/slash/command/component_command/component_command.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/slash/command/context_command/context_command.py` & `hata-1.3.9/hata/ext/slash/command/context_command/context_command.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/slash/command/form_submit_command/form_submit_command.py` & `hata-1.3.9/hata/ext/slash/command/form_submit_command/form_submit_command.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/slash/command/helpers.py` & `hata-1.3.9/hata/ext/slash/command/helpers.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/slash/command/slash_command/helpers.py` & `hata-1.3.9/hata/ext/slash/command/slash_command/helpers.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/slash/command/slash_command/slash_command.py` & `hata-1.3.9/hata/ext/slash/command/slash_command/slash_command.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/slash/command/slash_command/slash_command_category.py` & `hata-1.3.9/hata/ext/slash/command/slash_command/slash_command_category.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/slash/command/slash_command/slash_command_function.py` & `hata-1.3.9/hata/ext/slash/command/slash_command/slash_command_function.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/slash/command/slash_command/slash_command_parameter_auto_completer.py` & `hata-1.3.9/hata/ext/slash/command/slash_command/slash_command_parameter_auto_completer.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/slash/components.py` & `hata-1.3.9/hata/ext/slash/components.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/slash/converters.py` & `hata-1.3.9/hata/ext/slash/converters.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/slash/event_handlers.py` & `hata-1.3.9/hata/ext/slash/event_handlers.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/slash/exceptions.py` & `hata-1.3.9/hata/ext/slash/exceptions.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/slash/expression_parser.py` & `hata-1.3.9/hata/ext/slash/expression_parser.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/slash/helpers.py` & `hata-1.3.9/hata/ext/slash/helpers.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/slash/menus/closer.py` & `hata-1.3.9/hata/ext/slash/menus/closer.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/slash/menus/helpers.py` & `hata-1.3.9/hata/ext/slash/menus/helpers.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/slash/menus/menu.py` & `hata-1.3.9/hata/ext/slash/menus/menu.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/slash/menus/pagination.py` & `hata-1.3.9/hata/ext/slash/menus/pagination.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/slash/permission_mismatch.py` & `hata-1.3.9/hata/ext/slash/permission_mismatch.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/slash/responding.py` & `hata-1.3.9/hata/ext/slash/responding.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/slash/response_modifier.py` & `hata-1.3.9/hata/ext/slash/response_modifier.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/slash/slasher.py` & `hata-1.3.9/hata/ext/slash/slasher.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/slash/snapshot.py` & `hata-1.3.9/hata/ext/slash/snapshot.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/slash/utils.py` & `hata-1.3.9/hata/ext/slash/utils.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/slash/waiters.py` & `hata-1.3.9/hata/ext/slash/waiters.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/slash/wrappers.py` & `hata-1.3.9/hata/ext/slash/wrappers.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/solarlink/__init__.py` & `hata-1.3.9/hata/ext/solarlink/__init__.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/solarlink/client.py` & `hata-1.3.9/hata/ext/solarlink/client.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/solarlink/constants.py` & `hata-1.3.9/hata/ext/solarlink/constants.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/solarlink/event_handler_plugin.py` & `hata-1.3.9/hata/ext/solarlink/event_handler_plugin.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/solarlink/event_handlers.py` & `hata-1.3.9/hata/ext/solarlink/event_handlers.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/solarlink/event_types.py` & `hata-1.3.9/hata/ext/solarlink/event_types.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/solarlink/exceptions.py` & `hata-1.3.9/hata/ext/solarlink/exceptions.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/solarlink/filters.py` & `hata-1.3.9/hata/ext/solarlink/filters.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/solarlink/node.py` & `hata-1.3.9/hata/ext/solarlink/node.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/solarlink/parsers.py` & `hata-1.3.9/hata/ext/solarlink/parsers.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/solarlink/player.py` & `hata-1.3.9/hata/ext/solarlink/player.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/solarlink/player_base.py` & `hata-1.3.9/hata/ext/solarlink/player_base.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/solarlink/route_planner.py` & `hata-1.3.9/hata/ext/solarlink/route_planner.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/solarlink/stats.py` & `hata-1.3.9/hata/ext/solarlink/stats.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/solarlink/track.py` & `hata-1.3.9/hata/ext/solarlink/track.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/top_gg/__init__.py` & `hata-1.3.9/hata/ext/top_gg/__init__.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/top_gg/bots_query.py` & `hata-1.3.9/hata/ext/top_gg/bots_query.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/top_gg/client.py` & `hata-1.3.9/hata/ext/top_gg/client.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/top_gg/constants.py` & `hata-1.3.9/hata/ext/top_gg/constants.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/top_gg/exceptions.py` & `hata-1.3.9/hata/ext/top_gg/exceptions.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/top_gg/rate_limit_handling.py` & `hata-1.3.9/hata/ext/top_gg/rate_limit_handling.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/ext/top_gg/types.py` & `hata-1.3.9/hata/ext/top_gg/types.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/main/commands/default/help.py` & `hata-1.3.9/hata/main/commands/default/help.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/main/commands/default/interpreter.py` & `hata-1.3.9/hata/main/commands/default/interpreter.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/main/commands/default/run.py` & `hata-1.3.9/hata/main/commands/default/run.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/main/commands/default/version.py` & `hata-1.3.9/hata/main/commands/default/version.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/main/core/call.py` & `hata-1.3.9/hata/main/core/call.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/main/core/command/__init__.py` & `hata-1.3.9/hata/main/core/command/__init__.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/main/core/command/category.py` & `hata-1.3.9/hata/main/core/command/category.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/main/core/command/command.py` & `hata-1.3.9/hata/main/core/command/command.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/main/core/command/function.py` & `hata-1.3.9/hata/main/core/command/function.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/main/core/command/helpers.py` & `hata-1.3.9/hata/main/core/command/helpers.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/main/core/command/parameter.py` & `hata-1.3.9/hata/main/core/command/parameter.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/main/core/command/parameter_renderer.py` & `hata-1.3.9/hata/main/core/command/parameter_renderer.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/main/core/command/parameter_result.py` & `hata-1.3.9/hata/main/core/command/parameter_result.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/main/core/command/render_constants.py` & `hata-1.3.9/hata/main/core/command/render_constants.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/main/core/command/rendering_helpers.py` & `hata-1.3.9/hata/main/core/command/rendering_helpers.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/main/core/command/result.py` & `hata-1.3.9/hata/main/core/command/result.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/main/core/constants.py` & `hata-1.3.9/hata/main/core/constants.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/main/core/external.py` & `hata-1.3.9/hata/main/core/external.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/main/core/helpers.py` & `hata-1.3.9/hata/main/core/helpers.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/main/core/lookup.py` & `hata-1.3.9/hata/main/core/lookup.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/main/core/registration.py` & `hata-1.3.9/hata/main/core/registration.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/utils/debug.py` & `hata-1.3.9/hata/utils/debug.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata/utils/module_deprecation.py` & `hata-1.3.9/hata/utils/module_deprecation.py`

 * *Files identical despite different names*

### Comparing `hata-1.3.8/hata.egg-info/PKG-INFO` & `hata-1.3.9/hata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hata
-Version: 1.3.8
+Version: 1.3.9
 Summary: A powerful asynchronous library for creating Discord bots in Python.
 Home-page: https://github.com/HuyaneMatsu/hata
 Author: HuyaneMatsu
 Author-email: re.ism.tm@gmail.com
 License: DBAD
 Description: <h1 align="center">
             <b>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hata Version: 1.3.8 Summary: A powerful
+Metadata-Version: 2.1 Name: hata Version: 1.3.9 Summary: A powerful
 asynchronous library for creating Discord bots in Python. Home-page: https://
 github.com/HuyaneMatsu/hata Author: HuyaneMatsu Author-email:
 re.ism.tm@gmail.com License: DBAD Description:
                               ****** Hata ******
             A blazing fast Discord API wrapper that you can't deny
  Support_Guild | Topical_documentation | Examples | Technical_documentation |
                                     Source
```

### Comparing `hata-1.3.8/hata.egg-info/SOURCES.txt` & `hata-1.3.9/hata.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -160,15 +160,16 @@
 hata/discord/embed/embed.py
 hata/discord/embed/embed_base.py
 hata/discord/embed/embed_core.py
 hata/discord/emoji/__init__.py
 hata/discord/emoji/emoji.py
 hata/discord/emoji/emoji_all_pattern.py
 hata/discord/emoji/event_types.py
-hata/discord/emoji/reaction.py
+hata/discord/emoji/reaction_mapping.py
+hata/discord/emoji/reaction_mapping_line.py
 hata/discord/emoji/unicode_type.py
 hata/discord/emoji/unicodes.py
 hata/discord/emoji/utils.py
 hata/discord/events/__init__.py
 hata/discord/events/core.py
 hata/discord/events/default_event_handlers.py
 hata/discord/events/event_handler_manager.py
```

### Comparing `hata-1.3.8/setup.py` & `hata-1.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,15 +129,15 @@
         'hata.discord.bin' : [
             'libopus-0.x64.dll',
             'libopus-0.x86.dll',
         ],
     },
     python_requires = '>=3.6',
     install_requires = [
-        'scarletio>=1.0.35',
+        'scarletio>=1.0.42',
         'chardet>=2.0',
     ],
     extras_require = {
         'voice' : [
             'PyNaCl>=1.3.0',
         ],
         'relativedelta' : [
```

