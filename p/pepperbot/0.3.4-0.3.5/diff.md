# Comparing `tmp/pepperbot-0.3.4.tar.gz` & `tmp/pepperbot-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pepperbot-0.3.4.tar", last modified: Sat Apr 22 16:22:16 2023, max compression
+gzip compressed data, was "pepperbot-0.3.5.tar", last modified: Mon May  8 13:11:47 2023, max compression
```

## Comparing `pepperbot-0.3.4.tar` & `pepperbot-0.3.5.tar`

### file list

```diff
@@ -1,78 +1,86 @@
--rw-r--r--   0        0        0     1084 2021-03-30 09:01:51.964858 pepperbot-0.3.4/LICENSE
--rw-r--r--   0        0        0     4242 2023-04-09 16:21:30.526457 pepperbot-0.3.4/README.md
--rw-r--r--   0        0        0      273 2023-04-10 16:48:13.652944 pepperbot-0.3.4/cli/__init__.py
--rw-r--r--   0        0        0      631 2023-04-22 14:40:27.359697 pepperbot-0.3.4/pepperbot/__init__.py
--rw-r--r--   0        0        0     2819 2023-04-15 23:10:33.259712 pepperbot-0.3.4/pepperbot/adapters/keaimao/__init__.py
--rw-r--r--   0        0        0     5722 2023-04-20 11:08:26.809253 pepperbot-0.3.4/pepperbot/adapters/keaimao/api/__init__.py
--rw-r--r--   0        0        0     2636 2023-04-15 23:07:16.981274 pepperbot-0.3.4/pepperbot/adapters/keaimao/event/__init__.py
--rw-r--r--   0        0        0    21222 2022-04-13 12:45:33.068068 pepperbot-0.3.4/pepperbot/adapters/keaimao/event/records/EventFriendMsg.js
--rw-r--r--   0        0        0    10263 2022-02-20 09:58:20.299888 pepperbot-0.3.4/pepperbot/adapters/keaimao/event/records/EventGroupMessage.js
--rw-r--r--   0        0        0     6524 2023-04-16 02:25:50.305638 pepperbot-0.3.4/pepperbot/adapters/onebot/__init__.py
--rw-r--r--   0        0        0    25015 2023-04-15 13:09:02.414734 pepperbot-0.3.4/pepperbot/adapters/onebot/api/__init__.py
--rw-r--r--   0        0        0    11305 2023-04-20 11:07:29.210764 pepperbot-0.3.4/pepperbot/adapters/onebot/event/__init__.py
--rw-r--r--   0        0        0       67 2023-04-14 16:22:16.875389 pepperbot-0.3.4/pepperbot/adapters/onebot/models/__init__.py
--rw-r--r--   0        0        0      696 2023-04-14 16:01:58.086198 pepperbot-0.3.4/pepperbot/adapters/onebot/models/group.py
--rw-r--r--   0        0        0      572 2022-02-20 09:58:20.311051 pepperbot-0.3.4/pepperbot/adapters/onebot/models/message.py
--rw-r--r--   0        0        0     1395 2023-04-14 16:22:28.359913 pepperbot-0.3.4/pepperbot/adapters/onebot/models/user.py
--rw-r--r--   0        0        0     9174 2023-04-19 05:26:45.684428 pepperbot-0.3.4/pepperbot/adapters/telegram/__init__.py
--rw-r--r--   0        0        0     2931 2023-04-20 11:10:48.986337 pepperbot-0.3.4/pepperbot/adapters/telegram/api/__init__.py
--rw-r--r--   0        0        0     4663 2023-04-19 05:22:27.264737 pepperbot-0.3.4/pepperbot/adapters/telegram/event/__init__.py
--rw-r--r--   0        0        0      900 2023-04-14 17:09:33.793304 pepperbot-0.3.4/pepperbot/adapters/universal/__init__.py
--rw-r--r--   0        0        0     2709 2023-04-20 11:10:48.986337 pepperbot-0.3.4/pepperbot/adapters/universal/api/__init__.py
--rw-r--r--   0        0        0     3245 2023-04-15 23:11:30.691877 pepperbot-0.3.4/pepperbot/adapters/universal/event/__init__.py
--rw-r--r--   0        0        0      766 2023-04-10 15:18:25.547755 pepperbot-0.3.4/pepperbot/config.py
--rw-r--r--   0        0        0        0 2022-02-20 09:58:20.315950 pepperbot-0.3.4/pepperbot/core/__init__.py
--rw-r--r--   0        0        0     2796 2023-04-14 15:03:07.150287 pepperbot-0.3.4/pepperbot/core/api/api_caller.py
--rw-r--r--   0        0        0      835 2022-02-20 09:58:20.317490 pepperbot-0.3.4/pepperbot/core/api/decorators.py
--rw-r--r--   0        0        0        0 2022-02-20 09:58:20.319000 pepperbot-0.3.4/pepperbot/core/event/__init__.py
--rw-r--r--   0        0        0     1514 2023-04-16 00:04:42.470521 pepperbot-0.3.4/pepperbot/core/event/base_adapter.py
--rw-r--r--   0        0        0    22216 2023-04-22 15:01:15.299917 pepperbot-0.3.4/pepperbot/core/event/handle.py
--rw-r--r--   0        0        0     1642 2023-04-19 05:27:57.642248 pepperbot-0.3.4/pepperbot/core/event/universal.py
--rw-r--r--   0        0        0     3020 2022-05-04 06:33:33.296283 pepperbot-0.3.4/pepperbot/core/event/utils.py
--rw-r--r--   0        0        0      931 2022-05-03 12:01:53.466811 pepperbot-0.3.4/pepperbot/core/message/base.py
--rw-r--r--   0        0        0    11166 2023-04-22 06:17:19.872292 pepperbot-0.3.4/pepperbot/core/message/chain.py
--rw-r--r--   0        0        0    16761 2023-04-22 07:06:21.608086 pepperbot-0.3.4/pepperbot/core/message/segment.py
--rw-r--r--   0        0        0       84 2023-04-22 12:37:07.245598 pepperbot-0.3.4/pepperbot/core/route/__init__.py
--rw-r--r--   0        0        0     5629 2023-04-22 14:47:07.876298 pepperbot-0.3.4/pepperbot/core/route/available/__init__.py
--rw-r--r--   0        0        0     1359 2023-04-22 15:10:40.463249 pepperbot-0.3.4/pepperbot/core/route/available/decorators.py
--rw-r--r--   0        0        0     4873 2023-04-20 12:01:02.327347 pepperbot-0.3.4/pepperbot/core/route/cache.py
--rw-r--r--   0        0        0      326 2022-02-20 09:58:20.368067 pepperbot-0.3.4/pepperbot/core/route/hook.py
--rw-r--r--   0        0        0     6520 2023-04-20 12:02:43.500740 pepperbot-0.3.4/pepperbot/core/route/parse.py
--rw-r--r--   0        0        0     1812 2023-04-11 17:35:49.039234 pepperbot-0.3.4/pepperbot/core/route/utils.py
--rw-r--r--   0        0        0    13071 2023-04-20 08:52:11.814433 pepperbot-0.3.4/pepperbot/core/route/validate.py
--rw-r--r--   0        0        0     1165 2023-04-20 10:22:17.059555 pepperbot-0.3.4/pepperbot/exceptions.py
--rw-r--r--   0        0        0        0 2022-02-20 09:58:20.371633 pepperbot-0.3.4/pepperbot/extensions/__init__.py
--rw-r--r--   0        0        0     2146 2022-07-12 14:55:41.437631 pepperbot-0.3.4/pepperbot/extensions/action/__init__.py
--rw-r--r--   0        0        0     1323 2022-02-20 09:58:20.372621 pepperbot-0.3.4/pepperbot/extensions/action/action.py
--rw-r--r--   0        0        0     9917 2022-02-20 09:58:20.372621 pepperbot-0.3.4/pepperbot/extensions/action/chain.py
--rw-r--r--   0        0        0     2813 2022-02-20 09:58:20.373773 pepperbot-0.3.4/pepperbot/extensions/action/decorators.py
--rw-r--r--   0        0        0     2413 2022-02-20 09:58:20.374299 pepperbot-0.3.4/pepperbot/extensions/action/runner.py
--rw-r--r--   0        0        0     5316 2023-04-20 14:56:40.268659 pepperbot-0.3.4/pepperbot/extensions/command/__init__.py
--rw-r--r--   0        0        0    31844 2023-04-22 15:51:38.702263 pepperbot-0.3.4/pepperbot/extensions/command/handle.py
--rw-r--r--   0        0        0    12345 2023-04-22 13:03:26.717222 pepperbot-0.3.4/pepperbot/extensions/command/pattern.py
--rw-r--r--   0        0        0     2491 2023-04-20 11:29:18.885191 pepperbot-0.3.4/pepperbot/extensions/command/sender.py
--rw-r--r--   0        0        0     3180 2023-04-20 11:24:06.077698 pepperbot-0.3.4/pepperbot/extensions/command/utils.py
--rw-r--r--   0        0        0     2093 2023-04-20 10:57:14.518991 pepperbot-0.3.4/pepperbot/extensions/log/__init__.py
--rw-r--r--   0        0        0      103 2023-04-07 14:00:53.161961 pepperbot-0.3.4/pepperbot/extensions/scheduler/__init__.py
--rw-r--r--   0        0        0     8449 2023-04-20 10:23:25.131218 pepperbot-0.3.4/pepperbot/initial.py
--rw-r--r--   0        0        0       79 2022-02-20 09:58:20.384843 pepperbot-0.3.4/pepperbot/store/__init__.py
--rw-r--r--   0        0        0     6047 2023-04-22 14:11:02.794934 pepperbot-0.3.4/pepperbot/store/command.py
--rw-r--r--   0        0        0     2421 2023-04-22 14:42:16.694644 pepperbot-0.3.4/pepperbot/store/event.py
--rw-r--r--   0        0        0    14141 2023-04-22 14:20:55.717103 pepperbot-0.3.4/pepperbot/store/meta.py
--rw-r--r--   0        0        0     2426 2023-04-12 14:36:34.483507 pepperbot-0.3.4/pepperbot/store/orm.py
--rw-r--r--   0        0        0     1539 2023-04-20 15:00:26.563551 pepperbot-0.3.4/pepperbot/types.py
--rw-r--r--   0        0        0        0 2021-05-20 10:22:56.350973 pepperbot-0.3.4/pepperbot/utils/__init__.py
--rw-r--r--   0        0        0     5480 2023-04-22 13:18:32.526987 pepperbot-0.3.4/pepperbot/utils/common.py
--rw-r--r--   0        0        0     1774 2023-04-22 16:22:16.096908 pepperbot-0.3.4/pyproject.toml
--rw-r--r--   0        0        0        0 2021-02-17 16:09:40.523059 pepperbot-0.3.4/tests/__init__.py
--rw-r--r--   0        0        0     5265 2022-02-20 09:58:20.393826 pepperbot-0.3.4/tests/command/test_parse.py
--rw-r--r--   0        0        0      458 2021-05-20 06:46:35.532000 pepperbot-0.3.4/tests/context.py
--rw-r--r--   0        0        0      334 2021-05-20 10:15:22.378106 pepperbot-0.3.4/tests/is_flash.py
--rw-r--r--   0        0        0     1775 2021-05-20 08:57:32.459172 pepperbot-0.3.4/tests/messageChain.py
--rw-r--r--   0        0        0      589 2021-12-19 07:28:12.204746 pepperbot-0.3.4/tests/parse_pattern.py
--rw-r--r--   0        0        0     3335 2023-04-20 10:31:00.764749 pepperbot-0.3.4/tests/pattern.py
--rw-r--r--   0        0        0        0 2021-05-29 16:07:13.445106 pepperbot-0.3.4/tests/response/__init__.py
--rw-r--r--   0        0        0     2148 2022-02-20 09:58:20.394827 pepperbot-0.3.4/tests/response/fake_server.py
--rw-r--r--   0        0        0     1304 2021-05-29 17:05:54.532212 pepperbot-0.3.4/tests/response/poke.py
--rw-r--r--   0        0        0     2640 2021-05-20 11:42:38.152329 pepperbot-0.3.4/tests/tree.py
--rw-r--r--   0        0        0     5389 1970-01-01 00:00:00.000000 pepperbot-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1084 2021-03-30 09:01:51.964858 pepperbot-0.3.5/LICENSE
+-rw-r--r--   0        0        0     4722 2023-05-08 13:06:57.517071 pepperbot-0.3.5/README.md
+-rw-r--r--   0        0        0      273 2023-04-10 16:48:13.652944 pepperbot-0.3.5/cli/__init__.py
+-rw-r--r--   0        0        0      631 2023-05-08 13:03:35.795139 pepperbot-0.3.5/pepperbot/__init__.py
+-rw-r--r--   0        0        0     2819 2023-04-15 23:10:33.259712 pepperbot-0.3.5/pepperbot/adapters/keaimao/__init__.py
+-rw-r--r--   0        0        0     5722 2023-04-20 11:08:26.809253 pepperbot-0.3.5/pepperbot/adapters/keaimao/api/__init__.py
+-rw-r--r--   0        0        0     2636 2023-04-15 23:07:16.981274 pepperbot-0.3.5/pepperbot/adapters/keaimao/event/__init__.py
+-rw-r--r--   0        0        0    21222 2022-04-13 12:45:33.068068 pepperbot-0.3.5/pepperbot/adapters/keaimao/event/records/EventFriendMsg.js
+-rw-r--r--   0        0        0    10263 2022-02-20 09:58:20.299888 pepperbot-0.3.5/pepperbot/adapters/keaimao/event/records/EventGroupMessage.js
+-rw-r--r--   0        0        0     6524 2023-04-16 02:25:50.305638 pepperbot-0.3.5/pepperbot/adapters/onebot/__init__.py
+-rw-r--r--   0        0        0    25015 2023-05-08 12:20:06.549164 pepperbot-0.3.5/pepperbot/adapters/onebot/api/__init__.py
+-rw-r--r--   0        0        0    11305 2023-04-20 11:07:29.210764 pepperbot-0.3.5/pepperbot/adapters/onebot/event/__init__.py
+-rw-r--r--   0        0        0       67 2023-04-14 16:22:16.875389 pepperbot-0.3.5/pepperbot/adapters/onebot/models/__init__.py
+-rw-r--r--   0        0        0      696 2023-04-14 16:01:58.086198 pepperbot-0.3.5/pepperbot/adapters/onebot/models/group.py
+-rw-r--r--   0        0        0      572 2022-02-20 09:58:20.311051 pepperbot-0.3.5/pepperbot/adapters/onebot/models/message.py
+-rw-r--r--   0        0        0     1395 2023-04-14 16:22:28.359913 pepperbot-0.3.5/pepperbot/adapters/onebot/models/user.py
+-rw-r--r--   0        0        0     9174 2023-04-19 05:26:45.684428 pepperbot-0.3.5/pepperbot/adapters/telegram/__init__.py
+-rw-r--r--   0        0        0     2931 2023-04-20 11:10:48.986337 pepperbot-0.3.5/pepperbot/adapters/telegram/api/__init__.py
+-rw-r--r--   0        0        0     4663 2023-04-19 05:22:27.264737 pepperbot-0.3.5/pepperbot/adapters/telegram/event/__init__.py
+-rw-r--r--   0        0        0      900 2023-04-14 17:09:33.793304 pepperbot-0.3.5/pepperbot/adapters/universal/__init__.py
+-rw-r--r--   0        0        0     2709 2023-04-20 11:10:48.986337 pepperbot-0.3.5/pepperbot/adapters/universal/api/__init__.py
+-rw-r--r--   0        0        0     3245 2023-04-15 23:11:30.691877 pepperbot-0.3.5/pepperbot/adapters/universal/event/__init__.py
+-rw-r--r--   0        0        0      766 2023-04-10 15:18:25.547755 pepperbot-0.3.5/pepperbot/config.py
+-rw-r--r--   0        0        0        0 2022-02-20 09:58:20.315950 pepperbot-0.3.5/pepperbot/core/__init__.py
+-rw-r--r--   0        0        0     2796 2023-04-14 15:03:07.150287 pepperbot-0.3.5/pepperbot/core/api/api_caller.py
+-rw-r--r--   0        0        0      835 2022-02-20 09:58:20.317490 pepperbot-0.3.5/pepperbot/core/api/decorators.py
+-rw-r--r--   0        0        0        0 2022-02-20 09:58:20.319000 pepperbot-0.3.5/pepperbot/core/event/__init__.py
+-rw-r--r--   0        0        0     1514 2023-04-16 00:04:42.470521 pepperbot-0.3.5/pepperbot/core/event/base_adapter.py
+-rw-r--r--   0        0        0    22212 2023-05-08 12:20:20.126205 pepperbot-0.3.5/pepperbot/core/event/handle.py
+-rw-r--r--   0        0        0     1642 2023-04-19 05:27:57.642248 pepperbot-0.3.5/pepperbot/core/event/universal.py
+-rw-r--r--   0        0        0     3020 2022-05-04 06:33:33.296283 pepperbot-0.3.5/pepperbot/core/event/utils.py
+-rw-r--r--   0        0        0      931 2022-05-03 12:01:53.466811 pepperbot-0.3.5/pepperbot/core/message/base.py
+-rw-r--r--   0        0        0    11258 2023-05-07 12:55:09.643864 pepperbot-0.3.5/pepperbot/core/message/chain.py
+-rw-r--r--   0        0        0    16761 2023-05-07 08:29:43.324781 pepperbot-0.3.5/pepperbot/core/message/segment.py
+-rw-r--r--   0        0        0       84 2023-04-22 12:37:07.245598 pepperbot-0.3.5/pepperbot/core/route/__init__.py
+-rw-r--r--   0        0        0     5435 2023-05-08 12:03:14.378466 pepperbot-0.3.5/pepperbot/core/route/available/__init__.py
+-rw-r--r--   0        0        0     1359 2023-04-22 15:10:40.463249 pepperbot-0.3.5/pepperbot/core/route/available/decorators.py
+-rw-r--r--   0        0        0     4624 2023-05-08 12:21:33.482763 pepperbot-0.3.5/pepperbot/core/route/cache.py
+-rw-r--r--   0        0        0      326 2022-02-20 09:58:20.368067 pepperbot-0.3.5/pepperbot/core/route/hook.py
+-rw-r--r--   0        0        0     6520 2023-04-20 12:02:43.500740 pepperbot-0.3.5/pepperbot/core/route/parse.py
+-rw-r--r--   0        0        0     1812 2023-05-08 12:21:46.168927 pepperbot-0.3.5/pepperbot/core/route/utils.py
+-rw-r--r--   0        0        0    15411 2023-05-08 12:58:11.471224 pepperbot-0.3.5/pepperbot/core/route/validate.py
+-rw-r--r--   0        0        0     1165 2023-04-20 10:22:17.059555 pepperbot-0.3.5/pepperbot/exceptions.py
+-rw-r--r--   0        0        0        0 2022-02-20 09:58:20.371633 pepperbot-0.3.5/pepperbot/extensions/__init__.py
+-rw-r--r--   0        0        0     2146 2022-07-12 14:55:41.437631 pepperbot-0.3.5/pepperbot/extensions/action/__init__.py
+-rw-r--r--   0        0        0     1323 2022-02-20 09:58:20.372621 pepperbot-0.3.5/pepperbot/extensions/action/action.py
+-rw-r--r--   0        0        0     9917 2022-02-20 09:58:20.372621 pepperbot-0.3.5/pepperbot/extensions/action/chain.py
+-rw-r--r--   0        0        0     2813 2022-02-20 09:58:20.373773 pepperbot-0.3.5/pepperbot/extensions/action/decorators.py
+-rw-r--r--   0        0        0     2413 2022-02-20 09:58:20.374299 pepperbot-0.3.5/pepperbot/extensions/action/runner.py
+-rw-r--r--   0        0        0     5383 2023-05-08 12:38:58.821743 pepperbot-0.3.5/pepperbot/extensions/command/__init__.py
+-rw-r--r--   0        0        0    29929 2023-05-08 12:41:31.503505 pepperbot-0.3.5/pepperbot/extensions/command/handle.py
+-rw-r--r--   0        0        0     1377 2023-05-07 08:19:44.268892 pepperbot-0.3.5/pepperbot/extensions/command/node.py
+-rw-r--r--   0        0        0      532 2023-05-07 08:20:17.196776 pepperbot-0.3.5/pepperbot/extensions/command/parser.py
+-rw-r--r--   0        0        0    25012 2023-05-08 12:58:08.158417 pepperbot-0.3.5/pepperbot/extensions/command/pattern.py
+-rw-r--r--   0        0        0     2491 2023-04-20 11:29:18.885191 pepperbot-0.3.5/pepperbot/extensions/command/sender.py
+-rw-r--r--   0        0        0     7978 2023-05-07 13:22:49.683674 pepperbot-0.3.5/pepperbot/extensions/command/utils.py
+-rw-r--r--   0        0        0     2093 2023-05-08 12:46:01.677718 pepperbot-0.3.5/pepperbot/extensions/log/__init__.py
+-rw-r--r--   0        0        0      103 2023-04-07 14:00:53.161961 pepperbot-0.3.5/pepperbot/extensions/scheduler/__init__.py
+-rw-r--r--   0        0        0     8449 2023-05-07 03:22:34.908784 pepperbot-0.3.5/pepperbot/initial.py
+-rw-r--r--   0        0        0       79 2022-02-20 09:58:20.384843 pepperbot-0.3.5/pepperbot/store/__init__.py
+-rw-r--r--   0        0        0     8636 2023-05-08 12:46:56.141148 pepperbot-0.3.5/pepperbot/store/command.py
+-rw-r--r--   0        0        0     2421 2023-04-22 14:42:16.694644 pepperbot-0.3.5/pepperbot/store/event.py
+-rw-r--r--   0        0        0    14722 2023-05-08 12:47:55.793372 pepperbot-0.3.5/pepperbot/store/meta.py
+-rw-r--r--   0        0        0     2426 2023-04-12 14:36:34.483507 pepperbot-0.3.5/pepperbot/store/orm.py
+-rw-r--r--   0        0        0     1750 2023-05-02 21:52:09.236997 pepperbot-0.3.5/pepperbot/types.py
+-rw-r--r--   0        0        0        0 2021-05-20 10:22:56.350973 pepperbot-0.3.5/pepperbot/utils/__init__.py
+-rw-r--r--   0        0        0     5637 2023-05-08 12:48:51.085527 pepperbot-0.3.5/pepperbot/utils/common.py
+-rw-r--r--   0        0        0     1880 2023-05-08 13:11:47.810059 pepperbot-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0      144 2023-05-07 11:36:54.700923 pepperbot-0.3.5/tests/__init__.py
+-rw-r--r--   0        0        0    12274 2023-05-08 12:43:16.485834 pepperbot-0.3.5/tests/command/test_cli_argument.py
+-rw-r--r--   0        0        0     1499 2023-05-08 12:43:24.446692 pepperbot-0.3.5/tests/command/test_lifecycle.py
+-rw-r--r--   0        0        0       87 2023-05-08 12:45:36.722837 pepperbot-0.3.5/tests/command/test_match.py
+-rw-r--r--   0        0        0     5980 2023-05-07 12:54:47.433922 pepperbot-0.3.5/tests/command/test_merge.py
+-rw-r--r--   0        0        0      400 2023-05-08 08:42:50.259215 pepperbot-0.3.5/tests/command/test_parameters.py
+-rw-r--r--   0        0        0    15309 2023-05-08 12:45:06.857956 pepperbot-0.3.5/tests/command/test_sub_command.py
+-rw-r--r--   0        0        0      619 2023-05-07 06:37:24.188198 pepperbot-0.3.5/tests/command/test_types.py
+-rw-r--r--   0        0        0       28 2023-05-08 12:43:01.486316 pepperbot-0.3.5/tests/command/test_validate.py
+-rw-r--r--   0        0        0     2481 2023-05-07 12:24:32.582530 pepperbot-0.3.5/tests/conftest.py
+-rw-r--r--   0        0        0      867 2023-05-07 13:50:57.563104 pepperbot-0.3.5/tests/core/test_available.py
+-rw-r--r--   0        0        0      214 2023-05-07 13:46:15.996945 pepperbot-0.3.5/tests/core/test_dispatch.py
+-rw-r--r--   0        0        0        0 2023-05-07 09:54:19.845047 pepperbot-0.3.5/tests/core/test_route.py
+-rw-r--r--   0        0        0     1818 2023-05-07 10:00:48.212139 pepperbot-0.3.5/tests/message/test_chain.py
+-rw-r--r--   0        0        0       87 2023-05-07 09:56:20.249411 pepperbot-0.3.5/tests/message/test_segment.py
+-rw-r--r--   0        0        0     2640 2021-05-20 11:42:38.152329 pepperbot-0.3.5/tests/tree.py
+-rw-r--r--   0        0        0     1096 2023-05-08 07:29:48.570650 pepperbot-0.3.5/tests/utils.py
+-rw-r--r--   0        0        0     5859 1970-01-01 00:00:00.000000 pepperbot-0.3.5/PKG-INFO
```

### Comparing `pepperbot-0.3.4/LICENSE` & `pepperbot-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.4/README.md` & `pepperbot-0.3.5/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -12,62 +12,66 @@
 
 <p align="center">
 <img src="./archive/coverage-badge.svg" />
 </p>
 
 ## 生而跨平台
 
-- QQ 基于 `Onebot`
+- QQ 基于 `Onebot`，`Mirai`(待实现)、`OPQ`(待实现)
 - 微信基于`可爱猫`
 - Telegram基于`Pyrogram`
 - 提供了跨平台、易用的消息类型(片段)
 - 通用事件，比如群消息、私聊消息等，提供了统一的接口，只需要写一次代码，就可以无缝应用到各个平台上，跨平台的消息传递从未如此轻松随意
-- [ ] 可以跨群、跨平台共享指令(的状态)
+- 可以跨群、跨平台共享指令(的状态)，或者全局锁定用户(不管用户是通过群聊还是私聊)
 
 ## 性能也够用
 
-- 底层基于异步的 Sanic 框架(目前有一定生态的 python web 框架，[性能最好的](https://www.techempower.com/benchmarks/))，性能相当不错
+- 底层基于异步的 Sanic 框架，目前有一定生态的 python web 框架中，[性能最好的](https://www.techempower.com/benchmarks/)
 - 轻量，主要处理消息，对于其他功能，暴露底层接口，方便实现深度定制
+- 几行代码，即可实现**多进程负载均衡**
 
 ## 自带全家桶
 
-- 支持 Django 风格集中化路由、flask 风格装饰器式**路由&权限系统**
-- Django 类视图风格/Vue 生命周期风格的**指令系统**，Fast Api 风格的**依赖注入**
+- 支持 `Django`或`starlette` 风格的集中化路由，或者`flask`或`fastAPI` 风格的装饰器式路由
+- 非常灵活的权限系统，支持路由、class、method级别的权限控制
+- Django 类视图风格或Vue 生命周期风格的**指令系统**
 - 定时任务
 - 日志支持
-- [ ] 数据库连接(内置 sqlite)
-- [ ] 链式调用 api(行为链，自动跨平台事件等待)
-- [ ] cli，快速创建项目，安装社区指令
+- 基于`ormar`的异步数据库支持(ormar基于`sqlalchemy` + `pydantic`)
+- 自带插件市场，可以安装社区指令
+- [ ] 提供cli工具，快速创建项目
+- [ ] 类似`Selenium`的事件等待
+- [ ] `fastAPI`风格的**依赖注入**
 
 ## 接口合语义
 
-- api 符合直觉，直观，流畅地把想法映射到代码上
+- API 符合直觉，直观，流畅地把想法映射到代码上
 - 基于 python3.6 之后的类型注解，提供了完全的类型提示
 - 大部分可以自动获取的参数，都会自动获取，不需要每次手动提供了
 - 只会动态注入用到的参数，没必要每次写一长串用不到的参数了！
-- API均有可直接复制使用的代码片段，快速开发
+- 文档中，均有可直接复制使用的代码片段，快速开发
 
 ## 测试文档全
 
+- 通过元编程(AST 之类)手段，对编写的各种代码进行规则检查，并输出易于理解的错误信息，将问题消灭在框架启动之前
 - 文档比较全
-- 测试在补了
+- 测试覆盖比较全面
 - 大量官方示例/指令
 - 来自作者的 QA(加群以获取)
-- 通过元编程(ast 之类)手段，对编写的各种代码进行规则检查，并输出易于理解的错误信息，将问题消灭在框架启动之前
 
 ## 安装
 
+目前只能3.10及以上，因为用了点新特性，之后会恢复对3.8的支持
+
 ```bash
 pip install pepperbot
 ```
 
 ## 使用
 
-<!-- - [Go to wiki](https://github.com/SSmJaE/PepperBot/wiki) -->
-
 [具体使用见文档](https://ssmjae.github.io/PepperBot/)
 
 ## 示例
 
 六行代码实现消息互转
 
 ```py
@@ -107,7 +111,13 @@
             await bot.group_message(
                 Text("没人"),
                 Image("http://123.jpg"),
             )
 ```
 
 ## 生态
+
+### 可以记忆上下文的GPT群聊机器人
+
+[PepperBot-GPT]( )
+
+### 通过GPT，自动检测群聊中的广告信息
```

#### html2text {}

```diff
@@ -1,38 +1,46 @@
                             ****** PepperBot ******
                              [./archive/icon.png]
 ä¸ä¸ªç¬¦åç´è§çè·¨ç¤¾äº¤å¹³å°æºå¨äººæ¡æ¶ï¼è½»æ¾å°å¨å¹³å°é´ä¼ éæ¶æ¯ï¼æ¯æQQãå¾®ä¿¡ãTelegram
                              ææ¡£ Â· QQäº¤æµç¾¤
                         [./archive/coverage-badge.svg]
-## çèè·¨å¹³å° - QQ åºäº `Onebot` - å¾®ä¿¡åºäº`å¯ç±ç«` -
-Telegramåºäº`Pyrogram` - æä¾äºè·¨å¹³å°ãæç¨çæ¶æ¯ç±»å(çæ®µ) -
+## çèè·¨å¹³å° - QQ åºäº `Onebot`ï¼`Mirai`(å¾å®ç°)ã`OPQ`(å¾å®ç°)
+- å¾®ä¿¡åºäº`å¯ç±ç«` - Telegramåºäº`Pyrogram` -
+æä¾äºè·¨å¹³å°ãæç¨çæ¶æ¯ç±»å(çæ®µ) -
 éç¨äºä»¶ï¼æ¯å¦ç¾¤æ¶æ¯ãç§èæ¶æ¯ç­ï¼æä¾äºç»ä¸çæ¥å£ï¼åªéè¦åä¸æ¬¡ä»£ç ï¼å°±å¯ä»¥æ ç¼åºç¨å°åä¸ªå¹³å°ä¸ï¼è·¨å¹³å°çæ¶æ¯ä¼ éä»æªå¦æ­¤è½»æ¾éæ
-- [ ] å¯ä»¥è·¨ç¾¤ãè·¨å¹³å°å±äº«æä»¤(çç¶æ) ## æ§è½ä¹å¤ç¨ -
-åºå±åºäºå¼æ­¥ç Sanic æ¡æ¶(ç®åæä¸å®çæç python web
-æ¡æ¶ï¼[æ§è½æå¥½ç](https://www.techempower.com/benchmarks/
-))ï¼æ§è½ç¸å½ä¸é -
+- å¯ä»¥è·¨ç¾¤ãè·¨å¹³å°å±äº«æä»¤(çç¶æ)ï¼æèå¨å±éå®ç¨æ·
+(ä¸ç®¡ç¨æ·æ¯éè¿ç¾¤èè¿æ¯ç§è) ## æ§è½ä¹å¤ç¨ -
+åºå±åºäºå¼æ­¥ç Sanic æ¡æ¶ï¼ç®åæä¸å®çæç python web
+æ¡æ¶ä¸­ï¼[æ§è½æå¥½ç](https://www.techempower.com/benchmarks/) -
 è½»éï¼ä¸»è¦å¤çæ¶æ¯ï¼å¯¹äºå¶ä»åè½ï¼æ´é²åºå±æ¥å£ï¼æ¹ä¾¿å®ç°æ·±åº¦å®å¶
-## èªå¸¦å¨å®¶æ¡¶ - æ¯æ Django é£æ ¼éä¸­åè·¯ç±ãflask
-é£æ ¼è£é¥°å¨å¼**è·¯ç±&æéç³»ç»** - Django ç±»è§å¾é£æ ¼/Vue
-çå½å¨æé£æ ¼ç**æä»¤ç³»ç»**ï¼Fast Api é£æ ¼ç**ä¾èµæ³¨å¥** -
-å®æ¶ä»»å¡ - æ¥å¿æ¯æ - [ ] æ°æ®åºè¿æ¥(åç½® sqlite) - [ ]
-é¾å¼è°ç¨ api(è¡ä¸ºé¾ï¼èªå¨è·¨å¹³å°äºä»¶ç­å¾) - [ ]
-cliï¼å¿«éåå»ºé¡¹ç®ï¼å®è£ç¤¾åºæä»¤ ## æ¥å£åè¯­ä¹ - api
+- å è¡ä»£ç ï¼å³å¯å®ç°**å¤è¿ç¨è´è½½åè¡¡** ## èªå¸¦å¨å®¶æ¡¶ -
+æ¯æ `Django`æ`starlette`
+é£æ ¼çéä¸­åè·¯ç±ï¼æè`flask`æ`fastAPI`
+é£æ ¼çè£é¥°å¨å¼è·¯ç± -
+éå¸¸çµæ´»çæéç³»ç»ï¼æ¯æè·¯ç±ãclassãmethodçº§å«çæéæ§å¶
+- Django ç±»è§å¾é£æ ¼æVue çå½å¨æé£æ ¼ç**æä»¤ç³»ç»** -
+å®æ¶ä»»å¡ - æ¥å¿æ¯æ - åºäº`ormar`çå¼æ­¥æ°æ®åºæ¯æ
+(ormaråºäº`sqlalchemy` + `pydantic`) -
+èªå¸¦æä»¶å¸åºï¼å¯ä»¥å®è£ç¤¾åºæä»¤ - [ ]
+æä¾cliå·¥å·ï¼å¿«éåå»ºé¡¹ç® - [ ] ç±»ä¼¼`Selenium`çäºä»¶ç­å¾ -
+[ ] `fastAPI`é£æ ¼ç**ä¾èµæ³¨å¥** ## æ¥å£åè¯­ä¹ - API
 ç¬¦åç´è§ï¼ç´è§ï¼æµçå°ææ³æ³æ å°å°ä»£ç ä¸ - åºäº python3.6
 ä¹åçç±»åæ³¨è§£ï¼æä¾äºå®å¨çç±»åæç¤º -
 å¤§é¨åå¯ä»¥èªå¨è·åçåæ°ï¼é½ä¼èªå¨è·åï¼ä¸éè¦æ¯æ¬¡æå¨æä¾äº
 -
 åªä¼å¨ææ³¨å¥ç¨å°çåæ°ï¼æ²¡å¿è¦æ¯æ¬¡åä¸é¿ä¸²ç¨ä¸å°çåæ°äºï¼
-- APIåæå¯ç´æ¥å¤å¶ä½¿ç¨çä»£ç çæ®µï¼å¿«éå¼å ##
-æµè¯ææ¡£å¨ - ææ¡£æ¯è¾å¨ - æµè¯å¨è¡¥äº - å¤§éå®æ¹ç¤ºä¾/æä»¤
-- æ¥èªä½èç QA(å ç¾¤ä»¥è·å) - éè¿åç¼ç¨(ast
+- ææ¡£ä¸­ï¼åæå¯ç´æ¥å¤å¶ä½¿ç¨çä»£ç çæ®µï¼å¿«éå¼å ##
+æµè¯ææ¡£å¨ - éè¿åç¼ç¨(AST
 ä¹ç±»)ææ®µï¼å¯¹ç¼åçåç§ä»£ç è¿è¡è§åæ£æ¥ï¼å¹¶è¾åºæäºçè§£çéè¯¯ä¿¡æ¯ï¼å°é®é¢æ¶ç­å¨æ¡æ¶å¯å¨ä¹å
-## å®è£ ```bash pip install pepperbot ``` ## ä½¿ç¨  [å·ä½ä½¿ç¨è§ææ¡£]
-(https://ssmjae.github.io/PepperBot/) ## ç¤ºä¾ å­è¡ä»£ç å®ç°æ¶æ¯äºè½¬
-```py class WhateverNameYouWant: async def group_message(self, bot:
+- ææ¡£æ¯è¾å¨ - æµè¯è¦çæ¯è¾å¨é¢ - å¤§éå®æ¹ç¤ºä¾/æä»¤ -
+æ¥èªä½èç QA(å ç¾¤ä»¥è·å) ## å®è£
+ç®ååªè½3.10åä»¥ä¸ï¼å ä¸ºç¨äºç¹æ°ç¹æ§ï¼ä¹åä¼æ¢å¤å¯¹3.8çæ¯æ
+```bash pip install pepperbot ``` ## ä½¿ç¨ [å·ä½ä½¿ç¨è§ææ¡£](https://
+ssmjae.github.io/PepperBot/) ## ç¤ºä¾ å­è¡ä»£ç å®ç°æ¶æ¯äºè½¬ ```py
+class WhateverNameYouWant: async def group_message(self, bot:
 UniversalGroupBot, chain: MessageChain): if bot.onebot: #
 è½¬åqqæ¶æ¯è³å¾®ä¿¡ãTG await bot.arbitrary.keaimao.group_message
 ("19521241254@chatroom", *chain.segments) await
 bot.arbitrary.telegram.group_message("bot_father", *chain.segments) if
 bot.keaimao: # è½¬åå¾®ä¿¡æ¶æ¯è³qqãTG await
 bot.arbitrary.onebot.group_message("1041902989", *chain.segments) await
 bot.arbitrary.telegram.group_message("bot_father", *chain.segments) ```
@@ -44,8 +52,9 @@
 å¯ä»¥ç´æ¥âæ¤åæ¶æ¯âï¼ç¬¦åç´è§ if "è¸¢åºæ" ==
 chain.pure_text: await sender.kickout() # å¯ä»¥ç´æ¥è¸¢åºåè¨ç¾¤å #
 ä¹å¯ä»¥å¯¹æ¶æ¯é¾è¿è¡inæä½ï¼ç¸å½äºin chain.pure_text if
 "ç¦è¨æ" in chain: await sender.ban(10) # å¯ä»¥ç´æ¥ç¦è¨åè¨ç¾¤å if
 chain.regex("æäºº(å¨|å|å|å¨å).?"): # åéä¸æ¡ç¾¤æ¶æ¯ #
 æ¥åä»»æä¸ªåæ°ï¼å¿é¡»æ¯åæ³çæ¶æ¯çæ®µï¼æ¯å¦Textï¼Faceï¼Image
 await bot.group_message( Text("æ²¡äºº"), Image("http://123.jpg"), ) ``` ##
-çæ
+çæ ### å¯ä»¥è®°å¿ä¸ä¸æçGPTç¾¤èæºå¨äºº [PepperBot-GPT]( ) ###
+éè¿GPTï¼èªå¨æ£æµç¾¤èä¸­çå¹¿åä¿¡æ¯
```

### Comparing `pepperbot-0.3.4/pepperbot/__init__.py` & `pepperbot-0.3.5/pepperbot/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from pepperbot.extensions.log import logger
 from pepperbot.extensions.scheduler import async_scheduler
 from pepperbot.store.meta import BotRoute
 
 from .initial import PepperBot
 
-__version__ = "0.3.4"
+__version__ = "0.3.5"
 __all__ = (
     "__version__",
     "PepperBot",
     "logger",
     "async_scheduler",
     "BotRoute",
 )
```

### Comparing `pepperbot-0.3.4/pepperbot/adapters/keaimao/__init__.py` & `pepperbot-0.3.5/pepperbot/adapters/keaimao/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.4/pepperbot/adapters/keaimao/api/__init__.py` & `pepperbot-0.3.5/pepperbot/adapters/keaimao/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.4/pepperbot/adapters/keaimao/event/__init__.py` & `pepperbot-0.3.5/pepperbot/adapters/keaimao/event/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.4/pepperbot/adapters/keaimao/event/records/EventFriendMsg.js` & `pepperbot-0.3.5/pepperbot/adapters/keaimao/event/records/EventFriendMsg.js`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.4/pepperbot/adapters/keaimao/event/records/EventGroupMessage.js` & `pepperbot-0.3.5/pepperbot/adapters/keaimao/event/records/EventGroupMessage.js`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.4/pepperbot/adapters/onebot/__init__.py` & `pepperbot-0.3.5/pepperbot/adapters/onebot/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.4/pepperbot/adapters/onebot/api/__init__.py` & `pepperbot-0.3.5/pepperbot/adapters/onebot/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.4/pepperbot/adapters/onebot/event/__init__.py` & `pepperbot-0.3.5/pepperbot/adapters/onebot/event/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.4/pepperbot/adapters/onebot/models/group.py` & `pepperbot-0.3.5/pepperbot/adapters/onebot/models/group.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.4/pepperbot/adapters/onebot/models/message.py` & `pepperbot-0.3.5/pepperbot/adapters/onebot/models/message.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.4/pepperbot/adapters/onebot/models/user.py` & `pepperbot-0.3.5/pepperbot/adapters/onebot/models/user.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.4/pepperbot/adapters/telegram/__init__.py` & `pepperbot-0.3.5/pepperbot/adapters/telegram/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.4/pepperbot/adapters/telegram/api/__init__.py` & `pepperbot-0.3.5/pepperbot/adapters/telegram/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.4/pepperbot/adapters/telegram/event/__init__.py` & `pepperbot-0.3.5/pepperbot/adapters/telegram/event/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.4/pepperbot/adapters/universal/__init__.py` & `pepperbot-0.3.5/pepperbot/adapters/universal/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.4/pepperbot/adapters/universal/api/__init__.py` & `pepperbot-0.3.5/pepperbot/adapters/universal/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.4/pepperbot/adapters/universal/event/__init__.py` & `pepperbot-0.3.5/pepperbot/adapters/universal/event/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.4/pepperbot/config.py` & `pepperbot-0.3.5/pepperbot/config.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.4/pepperbot/core/api/api_caller.py` & `pepperbot-0.3.5/pepperbot/core/api/api_caller.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.4/pepperbot/core/api/decorators.py` & `pepperbot-0.3.5/pepperbot/core/api/decorators.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.4/pepperbot/core/event/base_adapter.py` & `pepperbot-0.3.5/pepperbot/core/event/base_adapter.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.4/pepperbot/core/event/handle.py` & `pepperbot-0.3.5/pepperbot/core/event/handle.py`

 * *Files 0% similar despite different names*

```diff
@@ -166,15 +166,15 @@
         event_metadata, event_dispatch_metadata
     )
 
     ordered_handlers: List[T_DispatchHandler] = list(disordered_handlers)
     ordered_handlers.sort(key=lambda x: x[1], reverse=True)
     grouped_ordered_handlers = groupby(ordered_handlers, key=lambda x: x[0])
 
-    # debug_log(dict(grouped_ordered_handlers))
+    # debug(dict(grouped_ordered_handlers))
 
     groups = []
     for propagation_group, dispatch_handlers in grouped_ordered_handlers:
         groups.append(
             asyncio.create_task(
                 dispatch_propagation_group(
                     event_metadata,
```

### Comparing `pepperbot-0.3.4/pepperbot/core/event/universal.py` & `pepperbot-0.3.5/pepperbot/core/event/universal.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.4/pepperbot/core/event/utils.py` & `pepperbot-0.3.5/pepperbot/core/event/utils.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.4/pepperbot/core/message/base.py` & `pepperbot-0.3.5/pepperbot/core/message/base.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.4/pepperbot/core/message/chain.py` & `pepperbot-0.3.5/pepperbot/core/message/chain.py`

 * *Files 1% similar despite different names*

```diff
@@ -281,14 +281,16 @@
     @property
     def text(self) -> List[Text]:
         return self.__getItems(Text)
 
     @property
     def pure_text(self) -> str:
         result = ""
+
+        # 这里不+空格，因为从event解析，基本不存在连续的Text Segment
         for segment in self.text:
             result += segment.content
 
         return result
 
     def any(self, *parts: str):
         for part in parts:
```

### Comparing `pepperbot-0.3.4/pepperbot/core/message/segment.py` & `pepperbot-0.3.5/pepperbot/core/message/segment.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.4/pepperbot/core/route/available/__init__.py` & `pepperbot-0.3.5/pepperbot/core/route/available/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,32 +5,21 @@
 from typing import Any, Awaitable, Callable, Dict, Set, Tuple, Union
 
 from devtools import debug
 
 from pepperbot.exceptions import InitializationError
 from pepperbot.store.meta import CLASS_CHECKERS, T_AvailableChecker, checkers_cache
 from pepperbot.types import COMMAND_CONFIG, T
-from pepperbot.utils.common import await_or_sync, fit_kwargs
+from pepperbot.utils.common import await_or_sync, fit_kwargs, get_class_name_from_method
 from pepperbot.extensions.log import logger
 
 AVAILABLE_CHECKERS = "__available_checkers__"
 HAS_SET_AVAILABLE_CHECKERS = "__has_set_available_checkers__"
 
 
-def get_class_name_from_method(method: Callable) -> str:
-    """从method上获取class name
-
-    用于available装饰器
-    """
-
-    # debug(method.__qualname__)
-
-    return method.__qualname__.split(".")[0]
-
-
 def available(*checkers: T_AvailableChecker):
     """动态判断handler、command是否可用
 
     checker可以是同步函数，也可以是异步函数，返回bool即可
 
     只要有一个不满足，即为不可用
 
@@ -136,15 +125,15 @@
     if is_class:
         class_name = obj.__class__.__name__  # type: ignore
         field = CLASS_CHECKERS
     else:
         class_name = get_class_name_from_method(obj)  # type: ignore
         field = obj.__name__  # type: ignore
 
-    debug(checkers_cache)
+    # debug(checkers_cache)
 
     checkers = checkers_cache[class_name, field]
     if not checkers:
         return True
 
     available, checker_name = await concurrently_run_checkers(checkers, **kwargs)
     if not available:
```

### Comparing `pepperbot-0.3.4/pepperbot/core/route/available/decorators.py` & `pepperbot-0.3.5/pepperbot/core/route/available/decorators.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.4/pepperbot/core/route/parse.py` & `pepperbot-0.3.5/pepperbot/core/route/parse.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.4/pepperbot/core/route/utils.py` & `pepperbot-0.3.5/pepperbot/core/route/utils.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.4/pepperbot/core/route/validate.py` & `pepperbot-0.3.5/pepperbot/core/route/validate.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from ast import Call
 import ast
 import inspect
 import keyword
 import re
+import textwrap
 from typing import Any, Callable, Dict, List, Sequence, Set, Union, get_args, get_origin
 
 from devtools import debug
 from pepperbot.adapters.keaimao import KeaimaoAdapter
 from pepperbot.adapters.keaimao.event import KeaimaoEvent
 from pepperbot.adapters.onebot import OnebotV11Adapter
 from pepperbot.adapters.onebot.event import OnebotV11Event
@@ -17,18 +18,19 @@
 from pepperbot.core.event.universal import ALL_PROTOCOL_EVENT_NAMES
 from pepperbot.exceptions import InitializationError
 from pepperbot.extensions.command.handle import (
     COMMAND_DEFAULT_KWARGS,
     LIFECYCLE_WITHOUT_PATTERNS,
     COMMAND_COMMON_KWARGS,
 )
-from pepperbot.store.command import PATTERN_ARG_TYPES
+from pepperbot.store.command import PATTERN_ARG_TYPES, TemporaryPatternArg
 from pepperbot.store.event import EventHandlerKwarg
 from pepperbot.types import COMMAND_CONFIG
 from pepperbot.utils.common import get_own_methods
+from pepperbot.store.meta import command_relations_cache
 
 
 def is_valid_class_handler(class_handler: object):
     for method in get_own_methods(class_handler):
         method_name = method.__name__
 
         is_class_handler_method_name_valid(method_name)
@@ -172,22 +174,25 @@
 
     common_prefix = f"\n{source_file_name} 文件中的指令 {class_command_name} 的"
 
     methods = list(get_own_methods(class_command))
     method_names = [method.__name__ for method in methods]
     method_mapping = {method.__name__: method for method in methods}
 
+    sub_command_method_names = list(command_relations_cache[class_command_name].keys())
+    # debug(sub_command_method_names)
+
     if not "initial" in method_names:
         raise InitializationError("指令必须定义initial方法作为入口")
 
     for method in methods:
         method_name = method.__name__
 
         is_class_command_method_return_valid(
-            method, method_name, method_names, common_prefix
+            method, method_name, method_names, sub_command_method_names, common_prefix
         )
 
     # 先通过上面的验证，此时的方法一定有返回值，并且只返回了一个值
     involved_method_names = get_all_returned_identifiers(methods)
 
     # 只验证被返回的方法，其他的方法不需要验证
     for method_name in involved_method_names:
@@ -212,15 +217,17 @@
         # no *, **
         if p.kind == p.VAR_POSITIONAL or p.kind == p.VAR_KEYWORD:
             raise InitializationError(
                 common_prefix + "不需要提供*或者**参数，PepperBot会自动根据声明的参数以及类型注入"
             )
 
         ## has type hint
-        keyword_arguments = COMMAND_DEFAULT_KWARGS.get(method_name, COMMAND_COMMON_KWARGS)
+        keyword_arguments = COMMAND_DEFAULT_KWARGS.get(
+            method_name, COMMAND_COMMON_KWARGS
+        )
         kwarg_name_type_mapping, usable_kwargs_hint = gen_usable_kwargs_hint(
             keyword_arguments
         )
 
         if p.annotation == p.empty:
             raise InitializationError(
                 common_prefix
@@ -228,52 +235,69 @@
                 + usable_kwargs_hint
                 if arg_name in kwarg_name_type_mapping.keys()
                 else ""
             )
 
         else:
             # kwargs == no default value
-            if p.default != p.empty and p.default != "PatternArg":
-                raise InitializationError(
-                    common_prefix + f"不应为 {method_name} 除pattern外的参数设置默认值"
-                )
+            if p.default != p.empty and not isinstance(p.default, TemporaryPatternArg):
+                raise InitializationError(common_prefix + f"不应为除CLI，或者Depends外的参数设置默认值")
 
             # type hint correct
-            if p.default != "PatternArg":
+            if not isinstance(p.default, TemporaryPatternArg):
                 supposed_type = kwarg_name_type_mapping.get(arg_name)
                 if not supposed_type:
                     raise InitializationError(
                         common_prefix + f"中不存在参数 {arg_name} ，请确认该参数是否为有效参数"
                     )
 
                 is_kwarg_annotation_correct(
                     arg_name, p.annotation, supposed_type, common_prefix
                 )
 
         # pattern args
-        if p.default == "PatternArg":
+        if isinstance(p.default, TemporaryPatternArg):
             # no pattern in lifecycle hooks
             if method_name in LIFECYCLE_WITHOUT_PATTERNS:
                 raise InitializationError(common_prefix + f"这些生命周期不应支持pattern")
 
-            if p.annotation not in PATTERN_ARG_TYPES:
+            if p.annotation not in PATTERN_ARG_TYPES or p.annotation is Any:
                 raise InitializationError(
                     common_prefix + f"仅支持str, bool, int, float和所有消息类型"
                 )
 
 
+def get_ids_from_single_return(elt):
+    if isinstance(elt, (ast.Name,)):
+        return [elt.id]
+
+    # Return(
+    #     value=Attribute(
+    #         value=Name(id="self", ctx=Load()),
+    #         attr="privilege",
+    #         ctx=Load(),
+    #     )
+    # )
+    if isinstance(elt, (ast.Attribute,)):
+        if isinstance(elt.value, (ast.Name,)):
+            if elt.value.id == "self":  # 必须是self
+                return [elt.attr]
+
+    return []
+
+
 def get_ids(elt):
     """Extract identifiers if present. If not return None"""
 
     if isinstance(elt, (ast.Tuple,)):
-        # For tuple get id of each item if item is a Name
-        return [x.id for x in elt.elts if isinstance(x, (ast.Name,))]
+        results = []
+        for item in elt.elts:
+            results.append(*get_ids_from_single_return(item))
 
-    if isinstance(elt, (ast.Name,)):
-        return [elt.id]
+    return get_ids_from_single_return(elt)
 
 
 def get_return_identifiers(f: Callable):
     """
     [{'ids': ['x'],
      'lineno': 3,
      'statement': <_ast.Return object at 0x00000233AC624610>},
@@ -281,28 +305,44 @@
      'lineno': 5,
      'statement': <_ast.Return object at 0x00000233AC6240D0>},
     {'ids': ['x', 'y'],
      'lineno': 7,
      'statement': <_ast.Return object at 0x00000233AC624100>}]
     """
     function_source = inspect.getsource(f)
-    without_first_indent = function_source.lstrip()
+    # '    @sub_command(privilege)\n'
+    # '    async def delete(self, sender: CommandSender):\n'
+    # '        await sender.send_message(\n'
+    # '            At(sender.user_id),\n'
+    # '            Text("删除成功"),\n'
+    # '        )\n'
+
+    without_extra_indent = textwrap.dedent(function_source)
+    # '@sub_command(privilege)\n'
+    # 'async def delete(self, sender: CommandSender):\n'
+    # '    await sender.send_message(\n'
+    # '        At(sender.user_id),\n'
+    # '        Text("删除成功"),\n'
+    # '    )\n'
 
     # debug(function_source)
+    # debug(without_extra_indent)
 
-    while without_first_indent.startswith("@"):
-        without_decorator = without_first_indent[without_first_indent.index("\n") :]
-        without_first_indent = without_decorator.lstrip()
+    # 如果有装饰器，装饰器也会一并获取到，要手动去掉，不然无法正常解析函数定义
+    # 可能有多个装饰器
+    while without_extra_indent.startswith("@"):
+        without_decorator = without_extra_indent[without_extra_indent.index("\n") :]
+        without_extra_indent = textwrap.dedent(without_decorator)
 
         # debug(without_decorator)
         # debug(without_first_indent)
 
-    # 如果有装饰器，装饰器也会一并获取到，
-    # 要手动去掉，不然无法正常解析函数定义
-    (tree,) = ast.parse(without_first_indent).body
+    (tree,) = ast.parse(without_extra_indent).body
+
+    # debug(tree)
 
     return_statements: List = []
 
     for node in ast.walk(tree):
         if isinstance(node, (ast.Return,)):
             return_statements.append(
                 dict(
@@ -327,46 +367,68 @@
             if ids:  # 不为None，且len(ids) == 1
                 identifiers.update(ids)
 
     return identifiers
 
 
 def is_class_command_method_return_valid(
-    method: Callable, method_name: str, method_names: List[str], common_prefix: str
+    method: Callable,
+    method_name: str,
+    method_names: List[str],
+    sub_command_method_names: List[str],
+    common_prefix: str,
 ):
     """
     通过ast，保证方法返回值要么为None，要么是同一class的其它方法名
 
     同时不能是catch, timeout, exit，不应该由指令作者主动触发；initial和finish可以
 
     即使有了静态检测，运行时检测方法返回值也是需要的
     """
+
+    # debug(get_return_identifiers(method))
+
     for info in get_return_identifiers(method):
         ids = info["ids"]
 
         wrong = False
 
         if not ids:  # 不返回
             continue
 
         if len(ids) > 1:  # 不能返回多个值
             wrong = True
 
         identifier = ids[0]
+        # debug(identifier)
+
+        your_error = ""
+
         if identifier not in method_names:  # 要么返回下一步的方法名，要么不返回
             wrong = True
+            your_error = f"返回值 {identifier} 返回的不是指令的方法名，必须是当前class中的方法名"
 
         if identifier in LIFECYCLE_WITHOUT_PATTERNS:  # 不应该由指令作者主动触发
             wrong = True
+            your_error = f"返回值 {identifier} 是生命周期，不应该由指令作者主动触发"
+
+        if identifier in sub_command_method_names:  # sub command应该由框架调度，而不能直接返回
+            wrong = True
+            your_error = f"返回值 {identifier} 是sub command，应该由框架调度，而不能直接返回"
 
         if wrong:
             raise InitializationError(
                 common_prefix
-                + f"方法 {method_name} 的返回值只能是initial生命周期，或者用户自己定义的方法名，以继续会话；"
-                "直接返回None，或者不写返回语句，以结束会话"
+                + f"方法 {method_name} 的返回值未正确设置\n"
+                + f"{your_error}\n\n"
+                + "- 不能返回多个值\n"
+                + "- 不能是catch, timeout, exit之类的生命周期，这些不应该由指令作者主动触发\n"
+                + "- 可以返回initial生命周期\n"
+                + "- 不能是sub command，sub command应该由框架调度，而不能直接返回\n\n"
+                + "如果返回None，或者不写返回语句，会触发finish和cleanup生命周期，结束回话"
             )
 
 
 def is_valid_route_validator(validator: Callable):
     """参数检查"""
 
     validator.__annotations__
```

### Comparing `pepperbot-0.3.4/pepperbot/exceptions.py` & `pepperbot-0.3.5/pepperbot/exceptions.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.4/pepperbot/extensions/action/__init__.py` & `pepperbot-0.3.5/pepperbot/extensions/action/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.4/pepperbot/extensions/action/action.py` & `pepperbot-0.3.5/pepperbot/extensions/action/action.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.4/pepperbot/extensions/action/chain.py` & `pepperbot-0.3.5/pepperbot/extensions/action/chain.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.4/pepperbot/extensions/action/decorators.py` & `pepperbot-0.3.5/pepperbot/extensions/action/decorators.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.4/pepperbot/extensions/action/runner.py` & `pepperbot-0.3.5/pepperbot/extensions/action/runner.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.4/pepperbot/extensions/command/__init__.py` & `pepperbot-0.3.5/pepperbot/extensions/command/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,24 @@
-from typing import Any, Optional, Sequence, cast
+from typing import Any, Callable, Optional, Sequence, Union, cast
 
 from pepperbot.store.command import (
+    CLIArgument,
+    CLIOption,
     CommandConfig,
-    PatternArg,
     T_InteractiveStrategy,
 )
-from pepperbot.types import COMMAND_CONFIG, BaseClassCommand
+from pepperbot.store.meta import SubCommandRelation, command_relations_cache
+from pepperbot.types import COMMAND_CONFIG, BaseClassCommand, F
+from pepperbot.utils.common import get_class_name_from_method
 
-
-def permission():
-    # todo command的权限管理
-    # todo command的黑白名单，动态黑白名单(提供函数，参数为当前发言用户)
-    pass
+__all__ = (
+    "as_command",
+    "CLIArgument",
+    "CLIOption",
+)
 
 
 def as_command(
     *args,
     need_prefix: Optional[bool] = None,
     prefixes: Optional[Sequence[str]] = None,
     aliases: Optional[Sequence[str]] = None,
@@ -89,31 +92,31 @@
         # setattr(class_command, CUSTOM_COMMAND_CONFIG, config)
 
         return cast(BaseClassCommand, class_command)
 
     return decorator
 
 
-# class CommonEndMixin:
-#     # 用户主动退出
-#     async def exit(
-#         self, bot: GroupCommonBot, chain: MessageChain, sender: Sender, **kwargs
-#     ):
-#         await bot.group_msg(Text("用户主动退出"))
-
-#     # 流程正常退出(在中间的流程return None也是正常退出)
-#     async def finish(
-#         self, bot: GroupCommonBot, chain: MessageChain, sender: Sender, **kwargs
-#     ):
-#         # todo group_msg内部，自动合并相邻的Text
-#         await bot.group_msg(Text(f"{sender.user_id}"), Text("命令正常执行完毕后退出"))
-
-#     async def timeout(
-#         self, bot: GroupCommonBot, chain: MessageChain, sender: Sender, **kwargs
-#     ):
-#         await bot.group_msg(Text("用户超时未回复，结束会话"))
+def sub_command(
+    parent: Optional[Union[Callable, str]] = None, name: Optional[str] = None
+):
+    def decorator(method: F) -> F:
+        method_name: str = method.__name__  # type: ignore
 
-__all__ = (
-    "as_command",
-    "PatternArg",
-    "permission",
-)
+        if method_name not in command_relations_cache:
+            parent_method_name: Optional[str] = None
+            if parent is not None:
+                if isinstance(parent, str):
+                    parent_method_name = parent
+                else:
+                    parent_method_name = parent.__name__
+
+            class_name = get_class_name_from_method(method)
+
+            command_relations_cache[class_name][method_name] = SubCommandRelation(
+                parent_method_name=parent_method_name,
+                command_final_name=name or method_name,
+            )
+
+        return method
+
+    return decorator
```

### Comparing `pepperbot-0.3.4/pepperbot/extensions/command/handle.py` & `pepperbot-0.3.5/pepperbot/extensions/command/handle.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,64 +1,33 @@
-from collections import deque
 import pickle
 import time
+from collections import deque
 from inspect import isawaitable
-from typing import (
-    Any,
-    Callable,
-    Deque,
-    Dict,
-    Iterable,
-    List,
-    Optional,
-    Sequence,
-    Set,
-    Tuple,
-    Union,
-    cast,
-    final,
-)
+from typing import Any, Callable, Deque, Dict, Iterable, List, Set, Tuple, Union, cast
+
 from devtools import debug
 
-from pydantic import parse_obj_as
 from pepperbot.adapters.onebot.event import construct_chain
-
 from pepperbot.core.message.chain import MessageChain, chain_factory
 from pepperbot.core.route.available import check_available
 from pepperbot.exceptions import (
     ClassCommandDefinitionError,
     ClassCommandOnExit,
-    ClassCommandOnFinish,
-    ClassCommandOnTimeout,
+    PatternFormatError,
 )
 from pepperbot.extensions.command.pattern import parse_pattern
 from pepperbot.extensions.command.sender import CommandSender
 from pepperbot.extensions.command.utils import meet_command_exit, meet_command_prefix
 from pepperbot.extensions.log import debug_log, logger
-from pepperbot.store.command import (
-    ClassCommandStatus,
-    CommandConfig,
-    HistoryItem,
-)
+from pepperbot.store.command import ClassCommandStatus, CommandConfig, HistoryItem
 from pepperbot.store.event import EventHandlerKwarg, EventMetadata
-from pepperbot.store.meta import (
-    get_telegram_caller,
-    class_command_config_mapping,
-    class_command_mapping,
-)
-from pepperbot.types import (
-    T_BotProtocol,
-    T_ConversationType,
-    T_DispatchHandler,
-    T_HandlerType,
-    T_StopPropagation,
-)
+from pepperbot.store.meta import class_command_config_mapping, class_command_mapping
+from pepperbot.types import T_ConversationType, T_DispatchHandler, T_StopPropagation
 from pepperbot.utils.common import await_or_sync, fit_kwargs
 
-
 COMMAND_LIFECYCLE_EXCEPTIONS: Dict = {
     ClassCommandOnExit.__name__: "exit",
 }
 """ 这些生命周期通过抛出异常触发 
 finish是通过else:调用
 timeout需要在定时器中单独处理
 """
@@ -131,65 +100,14 @@
     event_metadata: EventMetadata,
     class_command_config_id: str,
     stop_propagation: Callable[[], None],
     running=False,
 ):
     """只有has_running时，或者has_available时，才会调用此函数"""
 
-    # locals中需要存在raw_event, chain, sender
-    # raw_event = event_metadata.raw_event
-    # chain = await chain_factory(event_metadata)
-    # sender = CommandSender(event_metadata)
-
-    # class_command_config_cache = class_command_config_mapping[class_command_config_id]
-
-    # command_name = class_command_config_cache.class_command_name
-    # command_config = class_command_config_cache.command_config
-
-    # status, created = await get_command_status(
-    #     event_metadata, command_name, command_config
-    # )
-    # if not running:
-    #     history: Deque[HistoryItem] = deque(maxlen=command_config.history_size)
-    # else:
-    #     history: Deque[HistoryItem] = pickle.loads(status.history)
-
-    # context: Dict = pickle.loads(status.context)
-
-    # # locals中需要prefix和alias，作为initial的可选参数
-    # # 如果一直return self.initial，那么从第二次运行开始，需要手动获取一下prefix和alias
-    # prefix = context.get("prefix")
-    # alias = context.get("alias")
-
-    # if not prefix or not alias:
-    #     # if not running:
-    #     # 没有正在运行中的指令，则需要找到一个可用的指令
-    #     # 所以都需要判断一下，是否满足条件
-
-    #     # locals中需要prefix和alias，作为initial的可选参数
-    #     meet_prefix, prefix_with_alias, prefix, alias = meet_command_prefix(
-    #         chain,
-    #         command_name,
-    #         command_config,
-    #     )
-
-    #     # if not meet_prefix:
-    #     #     logger.info(f"该事件不满足指令 {command_name} {class_command_config_id} 的执行条件")
-    #     #     # logger.info(f"<y>{chain.pure_text}</y> 不满足指令 <lc>{command_name}</lc> 的执行条件")
-    #     #     return
-
-    #     # logger.info(
-    #     #     f"<y>{chain.pure_text}</y> 满足指令 <lc>{command_name}</lc> {class_command_config_id} 的执行条件"
-    #     # )
-
-    #     context.update(dict(prefix=prefix, alias=alias))
-    #     status.context = pickle.dumps(context)
-    #     status.running = True
-    #     await status.update()
-
     command_kwargs = await construct_command_kwargs(
         event_metadata, class_command_config_id, stop_propagation, running
     )
 
     command_name = command_kwargs["command_name"]
     class_command_cache = class_command_mapping[command_name]
     command_method_mapping = class_command_cache.command_method_mapping
@@ -203,35 +121,42 @@
     status = command_kwargs["status"]
 
     try:
         if running and meet_command_exit(
             command_kwargs["chain"], command_kwargs["command_config"]
         ):
             logger.info(
-                f"<y>{command_kwargs['chain.pure_text']}</y> 满足指令 {command_name} 的退出条件"
+                f"<y>{command_kwargs['chain'].pure_text}</y> 满足指令 {command_name} 的退出条件"
             )
             raise ClassCommandOnExit()  # TODO 一并传递触发exit生命周期的exit_pattern，作为参数
 
         logger.info(f"开始执行指令 <lc>{command_name}</lc> 的 <lc>{pointer}</lc> 方法")
 
         # 当前指向的方法，或者说，当前激活的命令回调方法
         command_method_cache = command_method_mapping[pointer]
 
         # locals中需要
         # 如果解析出错，会直接抛出异常，所以不会修改pointer的指向
-        command_kwargs["patterns"] = await parse_pattern(
+        # TODO 这里抛出FormatException，不应该触发cleanup
+        returned_method_name = "has not set yet"
+        target_method_name, command_kwargs["patterns"] = await parse_pattern(
+            event_metadata,
+            class_command_cache,
             command_method_cache,
             pointer,
             command_kwargs,
+            command_name,
+            status,
         )
 
         status.last_updated_time = time.time()
         await status.update()
 
-        target_method = command_method_cache.method
+        # target_method = command_method_cache.method
+        target_method = command_method_mapping[target_method_name].method
         returned_method = await run_class_command_method(
             pointer, target_method, command_kwargs, running=running
         )
 
         # 判断是否正常退出
         returned_method_name = returned_method.__name__ if returned_method else "None"
         debug_log(
@@ -243,14 +168,19 @@
         #     returned_method_name,
         #     returned_method,
         # )
 
         # 设置下一次执行时要调用的方法
         await update_command_pointer(status, command_kwargs, returned_method_name)
 
+    except PatternFormatError:
+        #  PatternError，不应该被catch生命周期捕获
+        # 同时，也不应触发其他生命周期，比如finish和cleanup
+        pass
+
     except ClassCommandOnExit:
         # 当触发生命周期时，立即调用，而不是等到用户下一次交互
 
         try:
             # exception_name: str = exception.__class__.__qualname__  # type:ignore
 
             # 触发finally
```

### Comparing `pepperbot-0.3.4/pepperbot/extensions/command/sender.py` & `pepperbot-0.3.5/pepperbot/extensions/command/sender.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.4/pepperbot/extensions/log/__init__.py` & `pepperbot-0.3.5/pepperbot/extensions/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.4/pepperbot/initial.py` & `pepperbot-0.3.5/pepperbot/initial.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -162,16 +162,14 @@
     async def main_process_start(app, loop):
         """
         https://sanic.dev/en/guide/basics/listeners.html#asgi-mode
 
         If you are running your application with an ASGI server, main_process_start and main_process_stop will be ignored
         """
 
-        # TODO 主动获取bot info
-        await set_metadata("has_initial_bot_info", False)
 
         # TODO 在各adapter初始化完成之后，再获取
         # 所以需要实现一个hook，after_adapter_init
 
         # main process、worker process都需要读取.env
         # 主动读取一次，这样即使用户定义的BaseSetting中没有制定env_file，也能读取到
         # load_dotenv()  # take environment variables from .env.
@@ -182,14 +180,16 @@
         logger.success(f"PepperBot successfully create bot routes")
         # output_config()
         # debug(per_worker)
 
         # 必须放到最后，等model都定义好了再执行
         # note that this has to be the same metadata that is used in ormar Models definition
         metadata.create_all(engine)
+        # TODO 主动获取bot info
+        await set_metadata("has_initial_bot_info", False)
         # 保证过期(无效)的command status一定被清理，不会干扰has_running_command的判断
         await check_command_timeout()
 
     @staticmethod
     async def after_server_start(app, loop):
         # ensure that async_scheduler is created under same async context
         # https://github.com/sanic-org/sanic/issues/743
```

### Comparing `pepperbot-0.3.4/pepperbot/store/event.py` & `pepperbot-0.3.5/pepperbot/store/event.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.4/pepperbot/store/meta.py` & `pepperbot-0.3.5/pepperbot/store/meta.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,55 +1,48 @@
 from collections import defaultdict
+from inspect import isclass
 from typing import (
+    TYPE_CHECKING,
     Any,
     Awaitable,
     Callable,
     Dict,
     Iterable,
     List,
     Literal,
     Optional,
-    Sequence,
     Set,
     Tuple,
-    Type,
     Union,
     cast,
 )
-from uuid import UUID
+
+from pydantic import BaseModel, Field
+from pyrogram.client import Client
+from rich import print as rich_print
+from rich.tree import Tree
+from typing_extensions import NotRequired
 
 from pepperbot.core.api.api_caller import ApiCaller
 from pepperbot.exceptions import InitializationError
-from pepperbot.store.command import (
-    ClassCommandCache,
-    ClassCommandConfigCache,
-    CommandConfig,
-)
-from pepperbot.store.event import ProtocolEvent
+from pepperbot.store.command import ClassCommandCache, ClassCommandConfigCache
 from pepperbot.types import (
     BOT_PROTOCOLS,
     CONVERSATION_TYPES,
     BaseBot,
     BaseClassCommand,
     T_BotProtocol,
     T_ConversationType,
     T_HandlerType,
     T_RouteRelation,
     T_RouteValidator,
-    T_WebProtocol,
 )
-from pepperbot.utils.common import deepawait_or_sync, fit_kwargs
-from pydantic import BaseModel, Field
-from pyrogram.client import Client
-from rich import print as rich_print
-from rich.tree import Tree
-from typing_extensions import Annotated, NotRequired
-
-from inspect import isclass
 
+if TYPE_CHECKING:
+    from pepperbot.core.message.segment import T_SegmentInstance
 
 import sys
 
 if sys.version_info < (3, 11):
     from typing_extensions import TypedDict
 else:
     from typing import TypedDict
@@ -202,16 +195,40 @@
 
 checkers_cache: Dict[Tuple[str, str], Set[T_AvailableChecker]] = defaultdict(set)
 """ 应用available时，无法判断是否是command，所以不放在对应的cache里，单独建一个 
 {
     ("class.__name__", CLASS_CHECKERS) : set(checker),
     ("class.__name__", "method.__name__") : set(checker),
 }
+"""
+
+
+class SubCommandRelation(TypedDict):
+    parent_method_name: Optional[str]
+    """ 没有父指令时的情况 """
+    command_final_name: str
+    """ 如何设置了alias，这里就是alias，否则就是command_name """
+
+
+command_relations_cache: Dict[str, Dict[str, SubCommandRelation]] = defaultdict(dict)
+""" 保存command的子指令关系，用于检查指令是否存在
+
+{
+    "command_name" : {
+        "sub_command_name" : SubCommandRelation(
+            parent_method_name = "parent_method_name",
+            command_final_name = "command_final_name",
+        ),
+    },
+}
  """
 
+command_arguments_cache: Dict[str, "T_SegmentInstance"] = {}
+""" 解决pickle的问题 """
+
 api_callers: ApiCallerTypeMap = {}
 
 bot_info: Dict[T_BotProtocol, Dict] = defaultdict(dict)
 """ 保存每个协议的bot的自身信息
 id
 是否是管理员之类
 """
```

### Comparing `pepperbot-0.3.4/pepperbot/store/orm.py` & `pepperbot-0.3.5/pepperbot/store/orm.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.4/pepperbot/types.py` & `pepperbot-0.3.5/pepperbot/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,25 @@
     TypeVar,
     Union,
     get_args,
 )
 
 
 COMMAND_CONFIG = "__command_config__"
+COMMAND_RELATIONS = "__command_relations__"
+""" 存储子指令和父指令的关系
+
+{
+    "sub_command_real_name": {
+        "parent_command_name": "",
+        "sub_command_alias": "",
+    }
+}
+
+"""
 
 
 class BaseClassCommand:
     __command_config__: Dict[str, Any]
 
 
 class BaseBot:
```

### Comparing `pepperbot-0.3.4/pepperbot/utils/common.py` & `pepperbot-0.3.5/pepperbot/utils/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import asyncio
-import functools
 import inspect
-from inspect import isawaitable, iscoroutine
+from inspect import iscoroutine
 from types import FunctionType
 from typing import Any, Callable, Coroutine, Dict, List, Union, cast
+
 from devtools import debug
 from pydantic import BaseModel
 
 
 class DictNoNone(dict):
     def __setitem__(self, key, value):
         if key in self or value is not None:
@@ -32,14 +32,22 @@
     """从class上获取所有非__开头的属性"""
 
     for property in dir(instance):
         if not property.startswith("__"):
             yield property
 
 
+def get_class_name_from_method(method: Callable) -> str:
+    """从method上获取class name"""
+
+    # debug(method.__qualname__)
+
+    return method.__qualname__.split(".")[0]
+
+
 async def await_or_sync(obj: Union[Any, FunctionType], *args, **kwargs) -> Any:
     """
     针对bound method，iscoroutine和isawaitable对bound method无效
 
     判断__func__也不行
     """
```

### Comparing `pepperbot-0.3.4/pyproject.toml` & `pepperbot-0.3.5/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     "type-annotations",
     "type-hint",
     "wechat",
 ]
 name = "pepperbot"
 readme = "README.md"
 requires-python = ">=3.10"
-version = "0.3.4"
+version = "0.3.5"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 documentation = "https://SSmJaE.github.io/PepperBot"
 homepage = "https://github.com/SSmJaE/PepperBot"
@@ -63,15 +63,20 @@
 includes = [
     "cli",
     "pepperbot",
 ]
 
 [tool.pdm.dev-dependencies]
 test = [
+    "pytest-asyncio>=0.21.0",
     "pytest-cov>=4.0.0",
+    "pytest-mock>=3.10.0",
     "pytest>=7.2.2",
 ]
 
 [tool.pdm.scripts]
 badge = "pytest --cov-report xml --cov-branch --cov=pepperbot ./tests/command/test_parse.py && deactive && genbadge coverage -i ./coverage.xml "
 run = "python private/run.py"
 test = "pytest --cov-report html --cov-branch --cov=pepperbot ./tests"
+
+[tool.pytest.ini_options]
+asyncio_mode = "auto"
```

### Comparing `pepperbot-0.3.4/tests/messageChain.py` & `pepperbot-0.3.5/tests/message/test_chain.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,23 @@
-import sys
-from os import path
+from pepperbot.core.message.chain import MessageChain
+from pepperbot.core.message.segment import *
 
-BASE_DIR = path.dirname(path.dirname(path.abspath(__file__)))
-sys.path.append(BASE_DIR)
 
-
-from pepperbot.main import *
-
-mockEvent = {
+mock_event = {
     "message_id": 12345,
     "message": [
         {"type": "face", "data": {"id": 123}},
         {"type": "text", "data": {"text": "word word"}},
         {"type": "text", "data": {"text": "word word2"}},
     ],
 }
-mockEvent2 = {"message_id": 7238908, "message": []}
+mock_event2 = {"message_id": 7238908, "message": []}
 
-chain = MessageChain(mockEvent, 1234, None)
-chain2 = MessageChain(mockEvent2, 1234, None)
+chain = MessageChain("onebot", "group", mock_event, "123456789", "987654321")
+chain2 = MessageChain("onebot", "group", mock_event2, "123456789", "987654321")
 
 assert chain != chain2
 
 #
 assert chain.pure_text == "word wordword word2", "pure_text应只包含Text类型的内容"
 # 字符串可以直接in
 assert "word" in chain
@@ -32,23 +27,23 @@
 assert Text in chain
 assert chain.has(Text) == True
 # 可以判断是否指定类型的实例
 assert Text("word2") not in chain
 assert Text("word word") in chain
 assert chain.has(Text("word word")) == True
 assert chain.has(Text("word word1")) == False
-assert chain.has(Face(123)) == True
-assert chain.has(Face(124)) == False
-assert chain.has(Face("123")) == True, "如果从后端传入的数据未经过Pydantic类型转换"
+assert chain.has(OnebotFace(123)) == True
+assert chain.has(OnebotFace(124)) == False
+assert chain.has(OnebotFace(123)) == True, "如果从后端传入的数据未经过Pydantic类型转换"
 # 快捷方式
 assert chain.has_and_first(Text) == (True, Text("word word"))
 assert chain.has_and_last(Text) == (True, Text("word word2"))
 assert chain.has_and_all(Text) == (True, [Text("word word"), Text("word word2")])
 # 获取所有指定类型实例
-assert chain.faces == [Face(123)]
+assert chain.onebot_faces == [OnebotFace(123)]
 assert chain.text == [Text("word word"), Text("word word2")]
 # 按index取Segment
 assert chain[1] == Text("word word")
 
 # 可以直接判断实例
 assert Text("word word") == Text("word word")
 assert Text("word word") != Text("word word2")
```

### Comparing `pepperbot-0.3.4/tests/tree.py` & `pepperbot-0.3.5/tests/tree.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.4/PKG-INFO` & `pepperbot-0.3.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pepperbot
-Version: 0.3.4
+Version: 0.3.5
 Summary: An intuitive multi-platform bot framework, easily forward messages among platforms, support QQ, WeChat, Telegram. 一个符合直觉的跨社交平台机器人框架，轻松地在平台间传递消息，支持QQ、微信、Telegram
 Keywords: Telegram async asyncio bot chinese cqhttp cross-platform framework keaimao onebot pydantic pyrogram python qq type-annotations type-hint wechat
 Home-page: https://github.com/SSmJaE/PepperBot
 Author-Email: SSmJaE <ssmjae327@gmail.com>
 License: MIT
 Classifier: Programming Language :: Python
 Project-URL: Documentation, https://SSmJaE.github.io/PepperBot
@@ -40,62 +40,66 @@
 
 <p align="center">
 <img src="./archive/coverage-badge.svg" />
 </p>
 
 ## 生而跨平台
 
-- QQ 基于 `Onebot`
+- QQ 基于 `Onebot`，`Mirai`(待实现)、`OPQ`(待实现)
 - 微信基于`可爱猫`
 - Telegram基于`Pyrogram`
 - 提供了跨平台、易用的消息类型(片段)
 - 通用事件，比如群消息、私聊消息等，提供了统一的接口，只需要写一次代码，就可以无缝应用到各个平台上，跨平台的消息传递从未如此轻松随意
-- [ ] 可以跨群、跨平台共享指令(的状态)
+- 可以跨群、跨平台共享指令(的状态)，或者全局锁定用户(不管用户是通过群聊还是私聊)
 
 ## 性能也够用
 
-- 底层基于异步的 Sanic 框架(目前有一定生态的 python web 框架，[性能最好的](https://www.techempower.com/benchmarks/))，性能相当不错
+- 底层基于异步的 Sanic 框架，目前有一定生态的 python web 框架中，[性能最好的](https://www.techempower.com/benchmarks/)
 - 轻量，主要处理消息，对于其他功能，暴露底层接口，方便实现深度定制
+- 几行代码，即可实现**多进程负载均衡**
 
 ## 自带全家桶
 
-- 支持 Django 风格集中化路由、flask 风格装饰器式**路由&权限系统**
-- Django 类视图风格/Vue 生命周期风格的**指令系统**，Fast Api 风格的**依赖注入**
+- 支持 `Django`或`starlette` 风格的集中化路由，或者`flask`或`fastAPI` 风格的装饰器式路由
+- 非常灵活的权限系统，支持路由、class、method级别的权限控制
+- Django 类视图风格或Vue 生命周期风格的**指令系统**
 - 定时任务
 - 日志支持
-- [ ] 数据库连接(内置 sqlite)
-- [ ] 链式调用 api(行为链，自动跨平台事件等待)
-- [ ] cli，快速创建项目，安装社区指令
+- 基于`ormar`的异步数据库支持(ormar基于`sqlalchemy` + `pydantic`)
+- 自带插件市场，可以安装社区指令
+- [ ] 提供cli工具，快速创建项目
+- [ ] 类似`Selenium`的事件等待
+- [ ] `fastAPI`风格的**依赖注入**
 
 ## 接口合语义
 
-- api 符合直觉，直观，流畅地把想法映射到代码上
+- API 符合直觉，直观，流畅地把想法映射到代码上
 - 基于 python3.6 之后的类型注解，提供了完全的类型提示
 - 大部分可以自动获取的参数，都会自动获取，不需要每次手动提供了
 - 只会动态注入用到的参数，没必要每次写一长串用不到的参数了！
-- API均有可直接复制使用的代码片段，快速开发
+- 文档中，均有可直接复制使用的代码片段，快速开发
 
 ## 测试文档全
 
+- 通过元编程(AST 之类)手段，对编写的各种代码进行规则检查，并输出易于理解的错误信息，将问题消灭在框架启动之前
 - 文档比较全
-- 测试在补了
+- 测试覆盖比较全面
 - 大量官方示例/指令
 - 来自作者的 QA(加群以获取)
-- 通过元编程(ast 之类)手段，对编写的各种代码进行规则检查，并输出易于理解的错误信息，将问题消灭在框架启动之前
 
 ## 安装
 
+目前只能3.10及以上，因为用了点新特性，之后会恢复对3.8的支持
+
 ```bash
 pip install pepperbot
 ```
 
 ## 使用
 
-<!-- - [Go to wiki](https://github.com/SSmJaE/PepperBot/wiki) -->
-
 [具体使用见文档](https://ssmjae.github.io/PepperBot/)
 
 ## 示例
 
 六行代码实现消息互转
 
 ```py
@@ -135,7 +139,13 @@
             await bot.group_message(
                 Text("没人"),
                 Image("http://123.jpg"),
             )
 ```
 
 ## 生态
+
+### 可以记忆上下文的GPT群聊机器人
+
+[PepperBot-GPT]( )
+
+### 通过GPT，自动检测群聊中的广告信息
```

